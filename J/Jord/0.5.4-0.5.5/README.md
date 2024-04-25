# Comparing `tmp/jord-0.5.4.tar.gz` & `tmp/jord-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jord-0.5.4.tar", last modified: Fri Apr 19 13:31:30 2024, max compression
+gzip compressed data, was "jord-0.5.5.tar", last modified: Thu Apr 25 16:34:30 2024, max compression
```

## Comparing `jord-0.5.4.tar` & `jord-0.5.5.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.082290 jord-0.5.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.050290 jord-0.5.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-19 13:31:23.000000 jord-0.5.4/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-19 13:31:23.000000 jord-0.5.4/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-19 13:31:23.000000 jord-0.5.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:23.000000 jord-0.5.4/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.074290 jord-0.5.4/Jord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-04-19 13:31:30.000000 jord-0.5.4/Jord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-19 13:31:30.000000 jord-0.5.4/Jord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:31:30.000000 jord-0.5.4/Jord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-19 13:31:30.000000 jord-0.5.4/Jord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-19 13:31:30.000000 jord-0.5.4/Jord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-19 13:31:23.000000 jord-0.5.4/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-04-19 13:31:23.000000 jord-0.5.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-19 13:31:23.000000 jord-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-04-19 13:31:30.082290 jord-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-19 13:31:23.000000 jord-0.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-19 13:31:23.000000 jord-0.5.4/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.050290 jord-0.5.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-19 13:31:23.000000 jord-0.5.4/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.050290 jord-0.5.4/jord/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 13:31:24.000000 jord-0.5.4/jord/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1484 2024-04-19 13:31:24.000000 jord-0.5.4/jord/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.050290 jord-0.5.4/jord/fiona_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:24.000000 jord-0.5.4/jord/fiona_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-04-19 13:31:24.000000 jord-0.5.4/jord/fiona_utilities/deserialise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.054290 jord-0.5.4/jord/gdal_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 13:31:24.000000 jord-0.5.4/jord/gdal_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      672 2024-04-19 13:31:24.000000 jord-0.5.4/jord/gdal_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1087 2024-04-19 13:31:24.000000 jord-0.5.4/jord/gdal_utilities/cloning.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1077 2024-04-19 13:31:24.000000 jord-0.5.4/jord/gdal_utilities/context.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2228 2024-04-19 13:31:24.000000 jord-0.5.4/jord/gdal_utilities/conversion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      491 2024-04-19 13:31:24.000000 jord-0.5.4/jord/gdal_utilities/drivers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      404 2024-04-19 13:31:24.000000 jord-0.5.4/jord/gdal_utilities/enums.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      768 2024-04-19 13:31:24.000000 jord-0.5.4/jord/gdal_utilities/error_handling.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1231 2024-04-19 13:31:24.000000 jord-0.5.4/jord/gdal_utilities/importing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2750 2024-04-19 13:31:24.000000 jord-0.5.4/jord/gdal_utilities/persistence.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-19 13:31:24.000000 jord-0.5.4/jord/gdal_utilities/spatial_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.054290 jord-0.5.4/jord/geojson_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-19 13:31:24.000000 jord-0.5.4/jord/geojson_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-19 13:31:24.000000 jord-0.5.4/jord/geojson_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      704 2024-04-19 13:31:24.000000 jord-0.5.4/jord/geojson_utilities/geometry_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.054290 jord-0.5.4/jord/geometric_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-19 13:31:24.000000 jord-0.5.4/jord/geometric_analysis/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-19 13:31:24.000000 jord-0.5.4/jord/geometric_analysis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5638 2024-04-19 13:31:24.000000 jord-0.5.4/jord/geometric_analysis/center_line.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      394 2024-04-19 13:31:24.000000 jord-0.5.4/jord/geometric_analysis/degrees_of_freedom.py
--rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-19 13:31:24.000000 jord-0.5.4/jord/geometric_analysis/intersections.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-04-19 13:31:24.000000 jord-0.5.4/jord/geometric_analysis/tracing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.054290 jord-0.5.4/jord/geopandas_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-19 13:31:24.000000 jord-0.5.4/jord/geopandas_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       82 2024-04-19 13:31:24.000000 jord-0.5.4/jord/geopandas_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      756 2024-04-19 13:31:24.000000 jord-0.5.4/jord/geopandas_utilities/geometry_filtering.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      108 2024-04-19 13:31:24.000000 jord-0.5.4/jord/geopandas_utilities/importing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.058290 jord-0.5.4/jord/geopandas_utilities/serialisation/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-19 13:31:24.000000 jord-0.5.4/jord/geopandas_utilities/serialisation/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      303 2024-04-19 13:31:24.000000 jord-0.5.4/jord/geopandas_utilities/serialisation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      673 2024-04-19 13:31:24.000000 jord-0.5.4/jord/geopandas_utilities/serialisation/well_known_binary.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1226 2024-04-19 13:31:24.000000 jord-0.5.4/jord/geopandas_utilities/serialisation/well_known_text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.058290 jord-0.5.4/jord/networkx_utilities/
--rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-04-19 13:31:24.000000 jord-0.5.4/jord/networkx_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-19 13:31:24.000000 jord-0.5.4/jord/networkx_utilities/construction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.058290 jord-0.5.4/jord/pillow_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-19 13:31:24.000000 jord-0.5.4/jord/pillow_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      455 2024-04-19 13:31:24.000000 jord-0.5.4/jord/pillow_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      280 2024-04-19 13:31:24.000000 jord-0.5.4/jord/pillow_utilities/exif.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      476 2024-04-19 13:31:24.000000 jord-0.5.4/jord/pillow_utilities/tiff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.062290 jord-0.5.4/jord/qgis_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      937 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3521 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/categorisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.062290 jord-0.5.4/jord/qgis_utilities/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/configuration/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      300 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/configuration/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1057 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/configuration/plugin_settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3233 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/configuration/project_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.062290 jord-0.5.4/jord/qgis_utilities/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/conversion/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/conversion/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      128 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/conversion/parsing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14840 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/data_provider.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1296 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/geo_interface_serialisation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      915 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/geometry_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.066290 jord-0.5.4/jord/qgis_utilities/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/helpers/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      502 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/helpers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2484 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/helpers/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/helpers/copying.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1088 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/helpers/drawing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6589 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/helpers/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/helpers/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/helpers/logging.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1780 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/helpers/models.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3566 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/helpers/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/helpers/randomize.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1208 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/helpers/sessions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2077 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/helpers/signals.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1223 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/helpers/timestamp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      460 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/importing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13965 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/layer_creation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2128 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/layer_serialisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.066290 jord-0.5.4/jord/qgis_utilities/numpy_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/numpy_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/numpy_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2676 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/numpy_utilities/conversion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4075 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/numpy_utilities/data_type.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2925 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      474 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/numpy_utilities/rasters.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      392 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/plugin_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/styles.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1978 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qgis_utilities/styling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.066290 jord-0.5.4/jord/qlive_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qlive_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qlive_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1862 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qlive_utilities/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.066290 jord-0.5.4/jord/qlive_utilities/clients/
--rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qlive_utilities/clients/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      447 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qlive_utilities/clients/arguments.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2865 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qlive_utilities/clients/auto.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qlive_utilities/clients/batching.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qlive_utilities/clients/interfaced.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qlive_utilities/pandas_procedures.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20181 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qlive_utilities/procedures.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2544 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qlive_utilities/serialisation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qlive_utilities/uri_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.070290 jord-0.5.4/jord/qt_utilities/
--rwxr-xr-x   0 runner    (1001) docker     (127)      240 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qt_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23855 2024-04-19 13:31:24.000000 jord-0.5.4/jord/qt_utilities/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.070290 jord-0.5.4/jord/rasterio_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 13:31:24.000000 jord-0.5.4/jord/rasterio_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-19 13:31:24.000000 jord-0.5.4/jord/rasterio_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.070290 jord-0.5.4/jord/shapely_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 13:31:24.000000 jord-0.5.4/jord/shapely_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      558 2024-04-19 13:31:24.000000 jord-0.5.4/jord/shapely_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-19 13:31:24.000000 jord-0.5.4/jord/shapely_utilities/base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8327 2024-04-19 13:31:24.000000 jord-0.5.4/jord/shapely_utilities/clamp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1907 2024-04-19 13:31:24.000000 jord-0.5.4/jord/shapely_utilities/geometry_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-19 13:31:24.000000 jord-0.5.4/jord/shapely_utilities/grouping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27412 2024-04-19 13:31:24.000000 jord-0.5.4/jord/shapely_utilities/lines.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      918 2024-04-19 13:31:24.000000 jord-0.5.4/jord/shapely_utilities/mirroring.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10107 2024-04-19 13:31:24.000000 jord-0.5.4/jord/shapely_utilities/morphology.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4177 2024-04-19 13:31:24.000000 jord-0.5.4/jord/shapely_utilities/points.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12570 2024-04-19 13:31:24.000000 jord-0.5.4/jord/shapely_utilities/polygons.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5885 2024-04-19 13:31:24.000000 jord-0.5.4/jord/shapely_utilities/projection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2796 2024-04-19 13:31:24.000000 jord-0.5.4/jord/shapely_utilities/rings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      585 2024-04-19 13:31:24.000000 jord-0.5.4/jord/shapely_utilities/selection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2902 2024-04-19 13:31:24.000000 jord-0.5.4/jord/shapely_utilities/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.074290 jord-0.5.4/jord/spatialite_utilities/
--rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-04-19 13:31:24.000000 jord-0.5.4/jord/spatialite_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      241 2024-04-19 13:31:24.000000 jord-0.5.4/jord/spatialite_utilities/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.074290 jord-0.5.4/jord/torch_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:24.000000 jord-0.5.4/jord/torch_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-19 13:31:24.000000 jord-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-19 13:31:24.000000 jord-0.5.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-19 13:31:30.082290 jord-0.5.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     9495 2024-04-19 13:31:24.000000 jord-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.074290 jord-0.5.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:31:30.074290 jord-0.5.4/tests/qgis/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-19 13:31:24.000000 jord-0.5.4/tests/qgis/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1997 2024-04-19 13:31:24.000000 jord-0.5.4/tests/test_import.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      471 2024-04-19 13:31:24.000000 jord-0.5.4/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.569846 jord-0.5.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.541846 jord-0.5.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-25 16:34:25.000000 jord-0.5.5/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-25 16:34:25.000000 jord-0.5.5/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 16:34:25.000000 jord-0.5.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:25.000000 jord-0.5.5/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.561846 jord-0.5.5/Jord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-04-25 16:34:30.000000 jord-0.5.5/Jord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-25 16:34:30.000000 jord-0.5.5/Jord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:34:30.000000 jord-0.5.5/Jord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-25 16:34:30.000000 jord-0.5.5/Jord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 16:34:30.000000 jord-0.5.5/Jord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-25 16:34:25.000000 jord-0.5.5/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-04-25 16:34:25.000000 jord-0.5.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-25 16:34:25.000000 jord-0.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-04-25 16:34:30.569846 jord-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-25 16:34:25.000000 jord-0.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-25 16:34:25.000000 jord-0.5.5/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.545846 jord-0.5.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-25 16:34:25.000000 jord-0.5.5/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.545846 jord-0.5.5/jord/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 16:34:25.000000 jord-0.5.5/jord/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1484 2024-04-25 16:34:25.000000 jord-0.5.5/jord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.545846 jord-0.5.5/jord/fiona_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:25.000000 jord-0.5.5/jord/fiona_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-04-25 16:34:25.000000 jord-0.5.5/jord/fiona_utilities/deserialise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.545846 jord-0.5.5/jord/gdal_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 16:34:25.000000 jord-0.5.5/jord/gdal_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      672 2024-04-25 16:34:25.000000 jord-0.5.5/jord/gdal_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1087 2024-04-25 16:34:25.000000 jord-0.5.5/jord/gdal_utilities/cloning.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1077 2024-04-25 16:34:25.000000 jord-0.5.5/jord/gdal_utilities/context.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2228 2024-04-25 16:34:25.000000 jord-0.5.5/jord/gdal_utilities/conversion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      491 2024-04-25 16:34:25.000000 jord-0.5.5/jord/gdal_utilities/drivers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      404 2024-04-25 16:34:25.000000 jord-0.5.5/jord/gdal_utilities/enums.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      768 2024-04-25 16:34:25.000000 jord-0.5.5/jord/gdal_utilities/error_handling.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1231 2024-04-25 16:34:25.000000 jord-0.5.5/jord/gdal_utilities/importing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2750 2024-04-25 16:34:25.000000 jord-0.5.5/jord/gdal_utilities/persistence.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-25 16:34:25.000000 jord-0.5.5/jord/gdal_utilities/spatial_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.549846 jord-0.5.5/jord/geojson_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geojson_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geojson_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      704 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geojson_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.549846 jord-0.5.5/jord/geometric_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geometric_analysis/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geometric_analysis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5638 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geometric_analysis/center_line.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      394 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geometric_analysis/degrees_of_freedom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geometric_analysis/intersections.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geometric_analysis/tracing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.549846 jord-0.5.5/jord/geopandas_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geopandas_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       82 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geopandas_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      756 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geopandas_utilities/geometry_filtering.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      108 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geopandas_utilities/importing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.549846 jord-0.5.5/jord/geopandas_utilities/serialisation/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geopandas_utilities/serialisation/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      303 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geopandas_utilities/serialisation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      673 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geopandas_utilities/serialisation/well_known_binary.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1401 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geopandas_utilities/serialisation/well_known_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.549846 jord-0.5.5/jord/networkx_utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-04-25 16:34:25.000000 jord-0.5.5/jord/networkx_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-25 16:34:25.000000 jord-0.5.5/jord/networkx_utilities/construction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.549846 jord-0.5.5/jord/pillow_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-25 16:34:25.000000 jord-0.5.5/jord/pillow_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      455 2024-04-25 16:34:25.000000 jord-0.5.5/jord/pillow_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      280 2024-04-25 16:34:25.000000 jord-0.5.5/jord/pillow_utilities/exif.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      476 2024-04-25 16:34:25.000000 jord-0.5.5/jord/pillow_utilities/tiff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.553846 jord-0.5.5/jord/qgis_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      937 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3521 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/categorisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.553846 jord-0.5.5/jord/qgis_utilities/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/configuration/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      300 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/configuration/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1057 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/configuration/plugin_settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3233 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/configuration/project_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.553846 jord-0.5.5/jord/qgis_utilities/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/conversion/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/conversion/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      128 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/conversion/parsing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14840 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/data_provider.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1296 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/geo_interface_serialisation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      915 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.557846 jord-0.5.5/jord/qgis_utilities/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      502 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2484 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/actions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      398 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/copying.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1088 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/drawing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6589 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/environment.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3357 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1780 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3566 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/progress_bar.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2877 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/randomize.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1208 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/sessions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2077 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/signals.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1223 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/timestamp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      460 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/importing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13965 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/layer_creation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2128 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/layer_serialisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.557846 jord-0.5.5/jord/qgis_utilities/numpy_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/numpy_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/numpy_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2676 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/numpy_utilities/conversion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4075 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/numpy_utilities/data_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2925 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      474 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/numpy_utilities/rasters.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      392 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/plugin_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/styles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1978 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/styling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.557846 jord-0.5.5/jord/qlive_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qlive_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qlive_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1862 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qlive_utilities/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.557846 jord-0.5.5/jord/qlive_utilities/clients/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qlive_utilities/clients/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      447 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qlive_utilities/clients/arguments.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2865 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qlive_utilities/clients/auto.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qlive_utilities/clients/batching.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qlive_utilities/clients/interfaced.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qlive_utilities/pandas_procedures.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20181 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qlive_utilities/procedures.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2566 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qlive_utilities/serialisation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qlive_utilities/uri_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.557846 jord-0.5.5/jord/qt_utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      240 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qt_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23855 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qt_utilities/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.557846 jord-0.5.5/jord/rasterio_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 16:34:25.000000 jord-0.5.5/jord/rasterio_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-25 16:34:25.000000 jord-0.5.5/jord/rasterio_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.561846 jord-0.5.5/jord/shapely_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      558 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8327 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/clamp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1907 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/geometry_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/grouping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27441 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/lines.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      918 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/mirroring.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10107 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/morphology.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4177 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/points.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12570 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/polygons.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5885 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/projection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2796 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/rings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      585 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/selection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2902 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.561846 jord-0.5.5/jord/spatialite_utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-04-25 16:34:25.000000 jord-0.5.5/jord/spatialite_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      241 2024-04-25 16:34:25.000000 jord-0.5.5/jord/spatialite_utilities/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.561846 jord-0.5.5/jord/torch_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:25.000000 jord-0.5.5/jord/torch_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-25 16:34:25.000000 jord-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-25 16:34:25.000000 jord-0.5.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-25 16:34:30.569846 jord-0.5.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9495 2024-04-25 16:34:25.000000 jord-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.561846 jord-0.5.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.561846 jord-0.5.5/tests/qgis/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-25 16:34:25.000000 jord-0.5.5/tests/qgis/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1997 2024-04-25 16:34:25.000000 jord-0.5.5/tests/test_import.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      471 2024-04-25 16:34:25.000000 jord-0.5.5/tests/test_sanity.py
```

### Comparing `jord-0.5.4/.github/CODE_OF_CONDUCT.md` & `jord-0.5.5/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/.github/CONTRIBUTING.md` & `jord-0.5.5/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/Jord.egg-info/PKG-INFO` & `jord-0.5.5/Jord.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jord
-Version: 0.5.4
+Version: 0.5.5
 Home-page: https://github.com/aivclab/jord
 Download-URL: https://github.com/aivclab/jord/releases
 Author: Christian Heider Lindbjerg
 Author-email: chen@mapspeople.dk
 Maintainer: Christian Heider Lindbjerg
 Maintainer-email: chen@mapspeople.dk
 License: Apache License, Version 2.0
@@ -36,87 +36,87 @@
 Provides-Extra: qgis
 Requires-Dist: PySide2; extra == "qgis"
 Provides-Extra: samples
 Provides-Extra: geopandas
 Requires-Dist: geopandas; extra == "geopandas"
 Provides-Extra: extra
 Provides-Extra: docs
-Requires-Dist: sphinx>=4.0.1; extra == "docs"
 Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
+Requires-Dist: sphinx>=4.0.1; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Provides-Extra: fiona
 Requires-Dist: fiona>=1.1.1; extra == "fiona"
 Provides-Extra: gdal
 Provides-Extra: tests
-Requires-Dist: pytest>=4.4.1; extra == "tests"
 Requires-Dist: mock; extra == "tests"
+Requires-Dist: pytest>=4.4.1; extra == "tests"
 Provides-Extra: shapely
-Requires-Dist: shapely; extra == "shapely"
 Requires-Dist: pyproj; extra == "shapely"
+Requires-Dist: shapely; extra == "shapely"
 Provides-Extra: network
 Requires-Dist: networkx; extra == "network"
 Provides-Extra: dev
-Requires-Dist: sphinx>=4.0.1; extra == "dev"
+Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
 Requires-Dist: twine>=1.13.0; extra == "dev"
-Requires-Dist: warg>=1.1.6; extra == "dev"
+Requires-Dist: pip>=22.1.2; extra == "dev"
 Requires-Dist: wheel>=0.33.0; extra == "dev"
 Requires-Dist: pytest>=4.3.0; extra == "dev"
-Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
-Requires-Dist: pytest>=4.4.1; extra == "dev"
-Requires-Dist: black[jupyter]>=21.5b0; extra == "dev"
+Requires-Dist: coveralls>=1.6.0; extra == "dev"
 Requires-Dist: mock; extra == "dev"
-Requires-Dist: pre-commit>=2.17.0; extra == "dev"
-Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
+Requires-Dist: sphinx>=4.0.1; extra == "dev"
+Requires-Dist: pytest>=4.4.1; extra == "dev"
 Requires-Dist: apppath>=1.0.2; extra == "dev"
-Requires-Dist: pip>=22.1.2; extra == "dev"
 Requires-Dist: draugr>=1.0.9; extra == "dev"
-Requires-Dist: pyzmq>=1.1.1; extra == "dev"
+Requires-Dist: sympy>=1.1.1; extra == "dev"
+Requires-Dist: pre-commit>=2.17.0; extra == "dev"
+Requires-Dist: tqdm>=1.1.1; extra == "dev"
 Requires-Dist: numpy>=1.20.0; extra == "dev"
-Requires-Dist: sorcery>=0.2.0; extra == "dev"
 Requires-Dist: furo; extra == "dev"
-Requires-Dist: tqdm>=1.1.1; extra == "dev"
-Requires-Dist: coveralls>=1.6.0; extra == "dev"
-Requires-Dist: sympy>=1.1.1; extra == "dev"
+Requires-Dist: sorcery>=0.2.0; extra == "dev"
+Requires-Dist: black[jupyter]>=21.5b0; extra == "dev"
+Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
+Requires-Dist: pyzmq>=1.1.1; extra == "dev"
+Requires-Dist: warg>=1.1.6; extra == "dev"
 Provides-Extra: pil
 Requires-Dist: Pillow; extra == "pil"
 Provides-Extra: legacy
 Requires-Dist: importlib-metadata; extra == "legacy"
 Requires-Dist: importlib-resources; extra == "legacy"
 Provides-Extra: setup
 Provides-Extra: all
-Requires-Dist: sphinx>=4.0.1; extra == "all"
+Requires-Dist: Pillow; extra == "all"
+Requires-Dist: importlib-metadata; extra == "all"
+Requires-Dist: pytest-cov>=2.11.1; extra == "all"
 Requires-Dist: twine>=1.13.0; extra == "all"
-Requires-Dist: warg>=1.1.6; extra == "all"
+Requires-Dist: pip>=22.1.2; extra == "all"
+Requires-Dist: PySide2; extra == "all"
 Requires-Dist: wheel>=0.33.0; extra == "all"
-Requires-Dist: importlib-resources; extra == "all"
 Requires-Dist: pytest>=4.3.0; extra == "all"
-Requires-Dist: importlib-metadata; extra == "all"
-Requires-Dist: sphinxcontrib-programoutput; extra == "all"
-Requires-Dist: pytest>=4.4.1; extra == "all"
-Requires-Dist: black[jupyter]>=21.5b0; extra == "all"
+Requires-Dist: fiona>=1.1.1; extra == "all"
 Requires-Dist: mock; extra == "all"
-Requires-Dist: shapely; extra == "all"
-Requires-Dist: pre-commit>=2.17.0; extra == "all"
-Requires-Dist: pytest-cov>=2.11.1; extra == "all"
+Requires-Dist: sphinx>=4.0.1; extra == "all"
+Requires-Dist: geopandas; extra == "all"
+Requires-Dist: coveralls>=1.6.0; extra == "all"
+Requires-Dist: pyproj; extra == "all"
+Requires-Dist: pytest>=4.4.1; extra == "all"
 Requires-Dist: apppath>=1.0.2; extra == "all"
-Requires-Dist: pip>=22.1.2; extra == "all"
 Requires-Dist: draugr>=1.0.9; extra == "all"
-Requires-Dist: pyproj; extra == "all"
-Requires-Dist: pyzmq>=1.1.1; extra == "all"
-Requires-Dist: numpy>=1.20.0; extra == "all"
-Requires-Dist: sorcery>=0.2.0; extra == "all"
-Requires-Dist: fiona>=1.1.1; extra == "all"
+Requires-Dist: sympy>=1.1.1; extra == "all"
+Requires-Dist: pre-commit>=2.17.0; extra == "all"
+Requires-Dist: tqdm>=1.1.1; extra == "all"
+Requires-Dist: importlib-resources; extra == "all"
+Requires-Dist: warg>=1.1.6; extra == "all"
 Requires-Dist: furo; extra == "all"
+Requires-Dist: sorcery>=0.2.0; extra == "all"
+Requires-Dist: shapely; extra == "all"
+Requires-Dist: black[jupyter]>=21.5b0; extra == "all"
+Requires-Dist: sphinxcontrib-programoutput; extra == "all"
 Requires-Dist: networkx; extra == "all"
-Requires-Dist: Pillow; extra == "all"
-Requires-Dist: tqdm>=1.1.1; extra == "all"
-Requires-Dist: coveralls>=1.6.0; extra == "all"
-Requires-Dist: sympy>=1.1.1; extra == "all"
-Requires-Dist: geopandas; extra == "all"
-Requires-Dist: PySide2; extra == "all"
+Requires-Dist: pyzmq>=1.1.1; extra == "all"
+Requires-Dist: numpy>=1.20.0; extra == "all"
 
 <!--![header](.github/images/header.png)-->
 
 <p align="center">
   <img src=".github/images/header.svg" alt='header' />
 </p>
```

### Comparing `jord-0.5.4/Jord.egg-info/SOURCES.txt` & `jord-0.5.5/Jord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/Jord.egg-info/requires.txt` & `jord-0.5.5/Jord.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -4,71 +4,71 @@
 pyzmq>=1.1.1
 sorcery>=0.2.0
 sympy>=1.1.1
 tqdm>=1.1.1
 warg>=1.1.6
 
 [all]
-sphinx>=4.0.1
+Pillow
+importlib-metadata
+pytest-cov>=2.11.1
 twine>=1.13.0
-warg>=1.1.6
+pip>=22.1.2
+PySide2
 wheel>=0.33.0
-importlib-resources
 pytest>=4.3.0
-importlib-metadata
-sphinxcontrib-programoutput
-pytest>=4.4.1
-black[jupyter]>=21.5b0
+fiona>=1.1.1
 mock
-shapely
-pre-commit>=2.17.0
-pytest-cov>=2.11.1
+sphinx>=4.0.1
+geopandas
+coveralls>=1.6.0
+pyproj
+pytest>=4.4.1
 apppath>=1.0.2
-pip>=22.1.2
 draugr>=1.0.9
-pyproj
-pyzmq>=1.1.1
-numpy>=1.20.0
-sorcery>=0.2.0
-fiona>=1.1.1
+sympy>=1.1.1
+pre-commit>=2.17.0
+tqdm>=1.1.1
+importlib-resources
+warg>=1.1.6
 furo
+sorcery>=0.2.0
+shapely
+black[jupyter]>=21.5b0
+sphinxcontrib-programoutput
 networkx
-Pillow
-tqdm>=1.1.1
-coveralls>=1.6.0
-sympy>=1.1.1
-geopandas
-PySide2
+pyzmq>=1.1.1
+numpy>=1.20.0
 
 [dev]
-sphinx>=4.0.1
+pytest-cov>=2.11.1
 twine>=1.13.0
-warg>=1.1.6
+pip>=22.1.2
 wheel>=0.33.0
 pytest>=4.3.0
-sphinxcontrib-programoutput
-pytest>=4.4.1
-black[jupyter]>=21.5b0
+coveralls>=1.6.0
 mock
-pre-commit>=2.17.0
-pytest-cov>=2.11.1
+sphinx>=4.0.1
+pytest>=4.4.1
 apppath>=1.0.2
-pip>=22.1.2
 draugr>=1.0.9
-pyzmq>=1.1.1
+sympy>=1.1.1
+pre-commit>=2.17.0
+tqdm>=1.1.1
 numpy>=1.20.0
-sorcery>=0.2.0
 furo
-tqdm>=1.1.1
-coveralls>=1.6.0
-sympy>=1.1.1
+sorcery>=0.2.0
+black[jupyter]>=21.5b0
+sphinxcontrib-programoutput
+pyzmq>=1.1.1
+warg>=1.1.6
 
 [docs]
-sphinx>=4.0.1
 sphinxcontrib-programoutput
+sphinx>=4.0.1
 furo
 
 [extra]
 
 [fiona]
 fiona>=1.1.1
 
@@ -94,13 +94,13 @@
 PySide2
 
 [samples]
 
 [setup]
 
 [shapely]
-shapely
 pyproj
+shapely
 
 [tests]
-pytest>=4.4.1
 mock
+pytest>=4.4.1
```

### Comparing `jord-0.5.4/LICENSE.md` & `jord-0.5.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/PKG-INFO` & `jord-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jord
-Version: 0.5.4
+Version: 0.5.5
 Home-page: https://github.com/aivclab/jord
 Download-URL: https://github.com/aivclab/jord/releases
 Author: Christian Heider Lindbjerg
 Author-email: chen@mapspeople.dk
 Maintainer: Christian Heider Lindbjerg
 Maintainer-email: chen@mapspeople.dk
 License: Apache License, Version 2.0
@@ -36,87 +36,87 @@
 Provides-Extra: qgis
 Requires-Dist: PySide2; extra == "qgis"
 Provides-Extra: samples
 Provides-Extra: geopandas
 Requires-Dist: geopandas; extra == "geopandas"
 Provides-Extra: extra
 Provides-Extra: docs
-Requires-Dist: sphinx>=4.0.1; extra == "docs"
 Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
+Requires-Dist: sphinx>=4.0.1; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Provides-Extra: fiona
 Requires-Dist: fiona>=1.1.1; extra == "fiona"
 Provides-Extra: gdal
 Provides-Extra: tests
-Requires-Dist: pytest>=4.4.1; extra == "tests"
 Requires-Dist: mock; extra == "tests"
+Requires-Dist: pytest>=4.4.1; extra == "tests"
 Provides-Extra: shapely
-Requires-Dist: shapely; extra == "shapely"
 Requires-Dist: pyproj; extra == "shapely"
+Requires-Dist: shapely; extra == "shapely"
 Provides-Extra: network
 Requires-Dist: networkx; extra == "network"
 Provides-Extra: dev
-Requires-Dist: sphinx>=4.0.1; extra == "dev"
+Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
 Requires-Dist: twine>=1.13.0; extra == "dev"
-Requires-Dist: warg>=1.1.6; extra == "dev"
+Requires-Dist: pip>=22.1.2; extra == "dev"
 Requires-Dist: wheel>=0.33.0; extra == "dev"
 Requires-Dist: pytest>=4.3.0; extra == "dev"
-Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
-Requires-Dist: pytest>=4.4.1; extra == "dev"
-Requires-Dist: black[jupyter]>=21.5b0; extra == "dev"
+Requires-Dist: coveralls>=1.6.0; extra == "dev"
 Requires-Dist: mock; extra == "dev"
-Requires-Dist: pre-commit>=2.17.0; extra == "dev"
-Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
+Requires-Dist: sphinx>=4.0.1; extra == "dev"
+Requires-Dist: pytest>=4.4.1; extra == "dev"
 Requires-Dist: apppath>=1.0.2; extra == "dev"
-Requires-Dist: pip>=22.1.2; extra == "dev"
 Requires-Dist: draugr>=1.0.9; extra == "dev"
-Requires-Dist: pyzmq>=1.1.1; extra == "dev"
+Requires-Dist: sympy>=1.1.1; extra == "dev"
+Requires-Dist: pre-commit>=2.17.0; extra == "dev"
+Requires-Dist: tqdm>=1.1.1; extra == "dev"
 Requires-Dist: numpy>=1.20.0; extra == "dev"
-Requires-Dist: sorcery>=0.2.0; extra == "dev"
 Requires-Dist: furo; extra == "dev"
-Requires-Dist: tqdm>=1.1.1; extra == "dev"
-Requires-Dist: coveralls>=1.6.0; extra == "dev"
-Requires-Dist: sympy>=1.1.1; extra == "dev"
+Requires-Dist: sorcery>=0.2.0; extra == "dev"
+Requires-Dist: black[jupyter]>=21.5b0; extra == "dev"
+Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
+Requires-Dist: pyzmq>=1.1.1; extra == "dev"
+Requires-Dist: warg>=1.1.6; extra == "dev"
 Provides-Extra: pil
 Requires-Dist: Pillow; extra == "pil"
 Provides-Extra: legacy
 Requires-Dist: importlib-metadata; extra == "legacy"
 Requires-Dist: importlib-resources; extra == "legacy"
 Provides-Extra: setup
 Provides-Extra: all
-Requires-Dist: sphinx>=4.0.1; extra == "all"
+Requires-Dist: Pillow; extra == "all"
+Requires-Dist: importlib-metadata; extra == "all"
+Requires-Dist: pytest-cov>=2.11.1; extra == "all"
 Requires-Dist: twine>=1.13.0; extra == "all"
-Requires-Dist: warg>=1.1.6; extra == "all"
+Requires-Dist: pip>=22.1.2; extra == "all"
+Requires-Dist: PySide2; extra == "all"
 Requires-Dist: wheel>=0.33.0; extra == "all"
-Requires-Dist: importlib-resources; extra == "all"
 Requires-Dist: pytest>=4.3.0; extra == "all"
-Requires-Dist: importlib-metadata; extra == "all"
-Requires-Dist: sphinxcontrib-programoutput; extra == "all"
-Requires-Dist: pytest>=4.4.1; extra == "all"
-Requires-Dist: black[jupyter]>=21.5b0; extra == "all"
+Requires-Dist: fiona>=1.1.1; extra == "all"
 Requires-Dist: mock; extra == "all"
-Requires-Dist: shapely; extra == "all"
-Requires-Dist: pre-commit>=2.17.0; extra == "all"
-Requires-Dist: pytest-cov>=2.11.1; extra == "all"
+Requires-Dist: sphinx>=4.0.1; extra == "all"
+Requires-Dist: geopandas; extra == "all"
+Requires-Dist: coveralls>=1.6.0; extra == "all"
+Requires-Dist: pyproj; extra == "all"
+Requires-Dist: pytest>=4.4.1; extra == "all"
 Requires-Dist: apppath>=1.0.2; extra == "all"
-Requires-Dist: pip>=22.1.2; extra == "all"
 Requires-Dist: draugr>=1.0.9; extra == "all"
-Requires-Dist: pyproj; extra == "all"
-Requires-Dist: pyzmq>=1.1.1; extra == "all"
-Requires-Dist: numpy>=1.20.0; extra == "all"
-Requires-Dist: sorcery>=0.2.0; extra == "all"
-Requires-Dist: fiona>=1.1.1; extra == "all"
+Requires-Dist: sympy>=1.1.1; extra == "all"
+Requires-Dist: pre-commit>=2.17.0; extra == "all"
+Requires-Dist: tqdm>=1.1.1; extra == "all"
+Requires-Dist: importlib-resources; extra == "all"
+Requires-Dist: warg>=1.1.6; extra == "all"
 Requires-Dist: furo; extra == "all"
+Requires-Dist: sorcery>=0.2.0; extra == "all"
+Requires-Dist: shapely; extra == "all"
+Requires-Dist: black[jupyter]>=21.5b0; extra == "all"
+Requires-Dist: sphinxcontrib-programoutput; extra == "all"
 Requires-Dist: networkx; extra == "all"
-Requires-Dist: Pillow; extra == "all"
-Requires-Dist: tqdm>=1.1.1; extra == "all"
-Requires-Dist: coveralls>=1.6.0; extra == "all"
-Requires-Dist: sympy>=1.1.1; extra == "all"
-Requires-Dist: geopandas; extra == "all"
-Requires-Dist: PySide2; extra == "all"
+Requires-Dist: pyzmq>=1.1.1; extra == "all"
+Requires-Dist: numpy>=1.20.0; extra == "all"
 
 <!--![header](.github/images/header.png)-->
 
 <p align="center">
   <img src=".github/images/header.svg" alt='header' />
 </p>
```

### Comparing `jord-0.5.4/README.md` & `jord-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/SECURITY.md` & `jord-0.5.5/SECURITY.md`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/__init__.py` & `jord-0.5.5/jord/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     from importlib_metadata import PackageNotFoundError
     from importlib_resources import files
 
 from warg import package_is_editable, clean_string, get_version
 
 __project__ = "Jord"
 __author__ = "Christian Heider Lindbjerg"
-__version__ = "0.5.4"
+__version__ = "0.5.5"
 __doc__ = r"""
 .. module:: jord
    :platform: Unix, Windows
    :synopsis: A set of general tools build for geo data.
 
 .. moduleauthor:: Christian Heider Lindbjerg <chen@mapspeople.dk>
```

### Comparing `jord-0.5.4/jord/fiona_utilities/deserialise.py` & `jord-0.5.5/jord/fiona_utilities/deserialise.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/gdal_utilities/__init__.py` & `jord-0.5.5/jord/gdal_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/gdal_utilities/cloning.py` & `jord-0.5.5/jord/gdal_utilities/cloning.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/gdal_utilities/context.py` & `jord-0.5.5/jord/gdal_utilities/context.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/gdal_utilities/conversion.py` & `jord-0.5.5/jord/gdal_utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/gdal_utilities/error_handling.py` & `jord-0.5.5/jord/gdal_utilities/error_handling.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/gdal_utilities/importing.py` & `jord-0.5.5/jord/gdal_utilities/importing.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/gdal_utilities/persistence.py` & `jord-0.5.5/jord/gdal_utilities/persistence.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/geojson_utilities/geometry_types.py` & `jord-0.5.5/jord/geojson_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/geometric_analysis/center_line.py` & `jord-0.5.5/jord/geometric_analysis/center_line.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/geometric_analysis/intersections.py` & `jord-0.5.5/jord/geometric_analysis/intersections.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/geopandas_utilities/geometry_filtering.py` & `jord-0.5.5/jord/geopandas_utilities/geometry_filtering.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/geopandas_utilities/serialisation/well_known_binary.py` & `jord-0.5.5/jord/geopandas_utilities/serialisation/well_known_binary.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/geopandas_utilities/serialisation/well_known_text.py` & `jord-0.5.5/jord/geopandas_utilities/serialisation/well_known_text.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,27 +6,36 @@
 
 import pandas
 from pandas import DataFrame
 from shapely import wkt
 
 __all__ = ["load_wkts_from_csv", "csv_wkt_generator"]
 
-from sorcery import assigned_names
+
+# from sorcery import assigned_names
 
 
 class WktTypeEnum(Enum):
     (
         point,
         multipoint,
         linestring,
         multilinestring,
         polygon,
         multipolygon,
         geometrycollection,
-    ) = assigned_names()
+    ) = (
+        "point",
+        "multipoint",
+        "linestring",
+        "multilinestring",
+        "polygon",
+        "multipolygon",
+        "geometrycollection",
+    )  # assigned_names()
 
 
 def load_wkts_from_csv(
     csv_file_path: Path, geometry_column: str = "Shape", additional_cols: Sequence = ()
 ) -> DataFrame:
     """
     Well-Known Text
```

### Comparing `jord-0.5.4/jord/networkx_utilities/construction.py` & `jord-0.5.5/jord/networkx_utilities/construction.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qgis_utilities/__init__.py` & `jord-0.5.5/jord/qgis_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qgis_utilities/categorisation.py` & `jord-0.5.5/jord/qgis_utilities/categorisation.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qgis_utilities/configuration/plugin_settings.py` & `jord-0.5.5/jord/qgis_utilities/configuration/plugin_settings.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qgis_utilities/configuration/project_settings.py` & `jord-0.5.5/jord/qgis_utilities/configuration/project_settings.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qgis_utilities/data_provider.py` & `jord-0.5.5/jord/qgis_utilities/data_provider.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qgis_utilities/enums.py` & `jord-0.5.5/jord/qgis_utilities/enums.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qgis_utilities/geo_interface_serialisation.py` & `jord-0.5.5/jord/qgis_utilities/geo_interface_serialisation.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qgis_utilities/geometry_types.py` & `jord-0.5.5/jord/qgis_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qgis_utilities/helpers/actions.py` & `jord-0.5.5/jord/qgis_utilities/helpers/actions.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qgis_utilities/helpers/drawing.py` & `jord-0.5.5/jord/qgis_utilities/helpers/drawing.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qgis_utilities/helpers/environment.py` & `jord-0.5.5/jord/qgis_utilities/helpers/environment.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qgis_utilities/helpers/groups.py` & `jord-0.5.5/jord/qgis_utilities/helpers/groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,108 +1,110 @@
 import logging
 from typing import Optional, Any, Union
 
 # noinspection PyUnresolvedReferences
 from qgis.core import QgsLayerTreeGroup, QgsLayerTreeLayer, QgsProject
-
 # noinspection PyUnresolvedReferences
 from qgis.utils import iface
 
 __all__ = ["duplicate_groups", "select_layer_in_group", "is_group_selected"]
 
 from jord.qgis_utilities.helpers.copying import deepcopy_layer
 
 try:
-    from types import EllipsisType
+  from types import EllipsisType
 except ImportError:
-    EllipsisType = type(...)
+  EllipsisType = type(...)
 
 logger = logging.getLogger(__name__)
 
 
 def duplicate_groups(
     group_to_duplicate,
     *,
     group_parent: Optional[Any] = None,
     new_name: Union[str, EllipsisType, None] = None,
 ) -> QgsLayerTreeGroup:
-    if group_to_duplicate is None:
-        logger.error("Group was None")
-        return
-
-    logger.info(f"Duplicating {group_to_duplicate.name()}")
-
-    if new_name is ... or new_name == "" or new_name is None:
-        new_name = f"{group_to_duplicate.name()} (Copy)"
-
-    sub_items = []
-    assert (
-        group_to_duplicate is not None
-    ), f"{group_to_duplicate=} is required to create a duplicate group"
-
-    if group_parent is None:
-        group_parent = group_to_duplicate.parent()
-
-    if group_parent is None:
-        raise ValueError(f"Group parent was not found for {group_to_duplicate}")
-
-    new_group_parent = group_parent.addGroup(new_name)
-    for original_group_child in group_to_duplicate.children():
-        if isinstance(original_group_child, QgsLayerTreeGroup):
-            new_sub_group, sub_sub_items = duplicate_groups(
-                original_group_child, group_parent=new_group_parent, new_name=...
-            )
-            sub_items.extend([new_sub_group, *sub_sub_items])
-        elif isinstance(original_group_child, QgsLayerTreeLayer):
-            sub_items.append(
-                duplicate_tree_node(new_group_parent, original_group_child)
-            )
-        else:
-            logger.error(f"{original_group_child} no supported in duplication")
+  if group_to_duplicate is None:
+    logger.error("Group was None")
+    return
+
+  logger.info(f"Duplicating {group_to_duplicate.name()}")
+
+  if new_name is ... or new_name == "" or new_name is None:
+    new_name = f"{group_to_duplicate.name()} (Copy)"
+
+  sub_items = []
+  assert (
+      group_to_duplicate is not None
+  ), f"{group_to_duplicate=} is required to create a duplicate group"
+
+  if group_parent is None:
+    group_parent = group_to_duplicate.parent()
+
+  if group_parent is None:
+    raise ValueError(f"Group parent was not found for {group_to_duplicate}")
+
+  new_group_parent = group_parent.addGroup(new_name)
+  for original_group_child in group_to_duplicate.children():
+    if isinstance(original_group_child, QgsLayerTreeGroup):
+      new_sub_group, sub_sub_items = duplicate_groups(
+        original_group_child, group_parent=new_group_parent, new_name=...
+      )
+      sub_items.extend([new_sub_group, *sub_sub_items])
+    elif isinstance(original_group_child, QgsLayerTreeLayer):
+      sub_items.append(
+        duplicate_tree_node(new_group_parent, original_group_child)
+      )
+    else:
+      logger.error(f"{original_group_child} no supported in duplication")
 
-    return new_group_parent, sub_items
+  return new_group_parent, sub_items
 
 
 def duplicate_tree_node(new_group_parent, original_group_child):
-    original_layer = original_group_child.layer()
-    new_layer_copy = deepcopy_layer(original_layer)
-    QgsProject.instance().addMapLayer(new_layer_copy, False)
-
-    if True:
-        new_layer_tree_node = QgsLayerTreeLayer(
-            new_layer_copy
-        )  # WORKS BUT MISSING STYLING
-    elif False:
-        # Does not WORK EITHER
-        new_layer_tree_node = QgsLayerTreeLayer(
-            new_layer_copy.id(),
-            original_layer.name(),
-            new_layer_copy.source(),
-            original_layer.providerType(),
-        )
-    elif False:
-        # THIS DOES NOT WORK!!!
-        new_layer_tree_node = (
-            original_group_child.clone()
-        )  # THIS JUST CREATES NEW VIEW of the same data!!!!
-        new_layer_tree_node.layer().setDataSource(
-            new_layer_copy.source(),
-            new_layer_copy.name(),
-            new_layer_copy.providerType(),
-        )
-    else:
-        raise Exception()
-
+  original_layer = original_group_child.layer()
+  new_layer_copy = deepcopy_layer(original_layer)
+  QgsProject.instance().addMapLayer(new_layer_copy, False)
+
+  if False:
+    new_layer_tree_node = QgsLayerTreeLayer(
+      new_layer_copy
+    )  # WORKS BUT MISSING STYLING
     new_group_parent.addChildNode(new_layer_tree_node)
+  elif False:
+    # Does not WORK EITHER
+    new_layer_tree_node = QgsLayerTreeLayer(
+      new_layer_copy.id(),
+      original_layer.name(),
+      new_layer_copy.source(),
+      original_layer.providerType(),
+    )
+  elif False:
+    # THIS DOES NOT WORK!!!
+    new_layer_tree_node = (
+      original_group_child.clone()
+    )  # THIS JUST CREATES NEW VIEW of the same data!!!!
+    new_layer_tree_node.layer().setDataSource(
+      new_layer_copy.source(),
+      new_layer_copy.name(),
+      new_layer_copy.providerType(),
+    )
+  elif True:
+    new_group_parent.insertLayer(0, new_layer_copy)
+  else:
+    raise Exception()
+
+  return new_layer_copy
 
 
 def select_layer_in_group(layer_name, group_name):
-    group = QgsProject.instance().layerTreeRoot().findGroup(group_name)
-    if group is not None:
-        for child in group.children():
-            if child.name() == layer_name:
-                iface.setActiveLayer(child.layer())
+  group = QgsProject.instance().layerTreeRoot().findGroup(group_name)
+  if group is not None:
+    for child in group.children():
+      if child.name() == layer_name:
+        iface.setActiveLayer(child.layer())
 
 
 def is_group_selected(group_name):
-    group = QgsProject.instance().layerTreeRoot().findGroup(group_name)
-    return group in iface.layerTreeView().selectedNodes()
+  group = QgsProject.instance().layerTreeRoot().findGroup(group_name)
+  return group in iface.layerTreeView().selectedNodes()
```

### Comparing `jord-0.5.4/jord/qgis_utilities/helpers/logging.py` & `jord-0.5.5/jord/qgis_utilities/helpers/logging.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qgis_utilities/helpers/models.py` & `jord-0.5.5/jord/qgis_utilities/helpers/models.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qgis_utilities/helpers/progress_bar.py` & `jord-0.5.5/jord/qgis_utilities/helpers/progress_bar.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qgis_utilities/helpers/randomize.py` & `jord-0.5.5/jord/qgis_utilities/helpers/randomize.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,79 @@
 import logging
 import uuid
 
 __all__ = ["randomize_field", "randomize_sub_tree_field"]
 
+from typing import Collection, Union, Any
+
 logger = logging.getLogger(__name__)
 
 
-def randomize_sub_tree_field(selected_nodes, field_name: str) -> None:
-    # noinspection PyUnresolvedReferences
-    from qgis.core import QgsLayerTreeGroup, QgsLayerTreeLayer
-
-    if isinstance(selected_nodes, QgsLayerTreeLayer):
-        randomize_field(selected_nodes, field_name=field_name)
-    elif isinstance(selected_nodes, QgsLayerTreeGroup):
-        randomize_sub_tree_field(selected_nodes.children(), field_name=field_name)
-    else:
-        for group in iter(selected_nodes):
-            if isinstance(group, QgsLayerTreeLayer):
-                randomize_field(group, field_name=field_name)
-            elif isinstance(group, QgsLayerTreeGroup):
-                randomize_sub_tree_field(group.children(), field_name=field_name)
-            else:
-                ...
-
-
-def randomize_field(tree_layer, field_name: str) -> None:  #: QgsLayerTreeLayer
-    """
-        https://qgis.org/pyqgis/3.28/core/QgsVectorLayer.html#qgis.core.QgsVectorLayer.changeAttributeValues
-
-    changeAttributeValues
-    fid: int, newValues: Dict[int, Any], oldValues: Dict[int, Any] = {}, skipDefaultValues: bool = False
-
-        :param field_name:
-        :param tree_layer:
-        :return:
-    """
-    if tree_layer is None:
-        logger.error(f"Tree layer was None")
-        return
-    # logger.info(f'Randomizing {field_name} in {tree_layer.layer().name()}')
-
-    layer = tree_layer.layer()
-
-    field_idx = layer.fields().indexFromName(field_name)
-
-    if field_idx >= 0:
-        layer.startEditing()
-        # layer.beginEditCommand(f"Regenerate {field_name}")
-        logger.info(
-            f"Randomizing {field_name}:{field_idx} in {tree_layer.layer().name()}"
-        )
-
-        for i in range(layer.featureCount() + 1):
-            layer.changeAttributeValue(i, field_idx, uuid.uuid4().hex)
-
-        # layer.rollBack()
-        # layer.endEditCommand()
-        layer.commitChanges()
+def randomize_sub_tree_field(selected_nodes: Union[Any, Collection[Any]], field_name: str) -> None:
+  # noinspection PyUnresolvedReferences
+  from qgis.core import QgsLayerTreeGroup, QgsLayerTreeLayer, QgsLayerTreeNode
+
+  if isinstance(selected_nodes, QgsLayerTreeLayer):
+    randomize_field(selected_nodes, field_name=field_name)
+  elif isinstance(selected_nodes, QgsLayerTreeGroup):
+    randomize_sub_tree_field(selected_nodes.children(), field_name=field_name)
+  elif isinstance(selected_nodes, QgsLayerTreeNode):
+    if selected_nodes.nodeType() == QgsLayerTreeNode.NodeGroup:
+      randomize_sub_tree_field(selected_nodes.children(), field_name=field_name)
     else:
-        logger.error(f"Did not find {field_name} in {layer.name()}")
+      logger.error(f'Node {selected_nodes} was not supported in randomize_sub_tree_field, skipping')
+  else:
+    if len(selected_nodes) == 0:
+      logger.error(
+        f"'Number of selected nodes was {len(selected_nodes)}, please supply some"
+      )
+      return
+
+    for group in iter(selected_nodes):
+      if isinstance(group, QgsLayerTreeLayer):
+        randomize_field(group, field_name=field_name)
+      elif isinstance(group, QgsLayerTreeGroup):
+        randomize_sub_tree_field(group.children(), field_name=field_name)
+      elif isinstance(group, QgsLayerTreeNode):
+        if group.nodeType() == QgsLayerTreeNode.NodeGroup:
+          randomize_sub_tree_field(group.children(), field_name=field_name)
+        else:
+          logger.error(f'Node {group} was not supported in randomize_sub_tree_field, skipping')
+      else:
+        logger.error(f'Node {group} was not supported in randomize_sub_tree_field, skipping')
+
+
+def randomize_field(tree_layer: Any, field_name: str) -> None:  #: QgsLayerTreeLayer
+  """
+      https://qgis.org/pyqgis/3.28/core/QgsVectorLayer.html#qgis.core.QgsVectorLayer.changeAttributeValues
+
+  changeAttributeValues
+  fid: int, newValues: Dict[int, Any], oldValues: Dict[int, Any] = {}, skipDefaultValues: bool = False
+
+      :param field_name:
+      :param tree_layer:
+      :return:
+  """
+  if tree_layer is None:
+    logger.error(f"Tree layer was None")
+    return
+  # logger.info(f'Randomizing {field_name} in {tree_layer.layer().name()}')
+
+  layer = tree_layer.layer()
+
+  field_idx = layer.fields().indexFromName(field_name)
+
+  if field_idx >= 0:
+    layer.startEditing()
+    # layer.beginEditCommand(f"Regenerate {field_name}")
+    logger.info(
+      f"Randomizing {field_name}:{field_idx} in {tree_layer.layer().name()}"
+    )
+
+    for i in range(layer.featureCount() + 1):
+      layer.changeAttributeValue(i, field_idx, uuid.uuid4().hex)
+
+    # layer.rollBack()
+    # layer.endEditCommand()
+    layer.commitChanges()
+  else:
+    logger.error(f"Did not find {field_name} in {layer.name()}")
```

### Comparing `jord-0.5.4/jord/qgis_utilities/helpers/sessions.py` & `jord-0.5.5/jord/qgis_utilities/helpers/sessions.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qgis_utilities/helpers/signals.py` & `jord-0.5.5/jord/qgis_utilities/helpers/signals.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qgis_utilities/helpers/timestamp.py` & `jord-0.5.5/jord/qgis_utilities/helpers/timestamp.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qgis_utilities/layer_creation.py` & `jord-0.5.5/jord/qgis_utilities/layer_creation.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qgis_utilities/layer_serialisation.py` & `jord-0.5.5/jord/qgis_utilities/layer_serialisation.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qgis_utilities/numpy_utilities/conversion.py` & `jord-0.5.5/jord/qgis_utilities/numpy_utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qgis_utilities/numpy_utilities/data_type.py` & `jord-0.5.5/jord/qgis_utilities/numpy_utilities/data_type.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py` & `jord-0.5.5/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qgis_utilities/styles.py` & `jord-0.5.5/jord/qgis_utilities/styles.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qgis_utilities/styling.py` & `jord-0.5.5/jord/qgis_utilities/styling.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qlive_utilities/client.py` & `jord-0.5.5/jord/qlive_utilities/client.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qlive_utilities/clients/auto.py` & `jord-0.5.5/jord/qlive_utilities/clients/auto.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qlive_utilities/procedures.py` & `jord-0.5.5/jord/qlive_utilities/procedures.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qlive_utilities/serialisation.py` & `jord-0.5.5/jord/qlive_utilities/serialisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import json
 import pickle
 from enum import Enum
 from typing import Tuple, Sequence, Any, Callable, Mapping, Union
 
 __all__ = ["build_package", "read_package"]
 
-from sorcery import assigned_names
+# from sorcery import assigned_names
 
 from jord.qlive_utilities.procedures import QliveRPCMethodEnum, QliveRPCMethodMap
 
 
 class SerialisationMethodEnum(Enum):
-    json, pickle = assigned_names()
+    json, pickle = "json", "pickle"  # assigned_names()
 
 
 SERIALISATION_METHOD = SerialisationMethodEnum.pickle
 VERBOSE = False
 
 
 def build_package(
```

### Comparing `jord-0.5.4/jord/qlive_utilities/uri_utilities.py` & `jord-0.5.5/jord/qlive_utilities/uri_utilities.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/qt_utilities/enums.py` & `jord-0.5.5/jord/qt_utilities/enums.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/shapely_utilities/__init__.py` & `jord-0.5.5/jord/shapely_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/shapely_utilities/base.py` & `jord-0.5.5/jord/shapely_utilities/base.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/shapely_utilities/clamp.py` & `jord-0.5.5/jord/shapely_utilities/clamp.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/shapely_utilities/geometry_types.py` & `jord-0.5.5/jord/shapely_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/shapely_utilities/grouping.py` & `jord-0.5.5/jord/shapely_utilities/grouping.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/shapely_utilities/lines.py` & `jord-0.5.5/jord/shapely_utilities/lines.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,16 @@
     MultiPoint,
     Point,
     box,
 )
 from shapely.geometry import LinearRing
 from shapely.geometry.base import BaseGeometry
 from shapely.ops import linemerge as shapely_linemerge
-from sorcery import assigned_names
+
+# from sorcery import assigned_names
 from warg import Number, pairs
 
 from .points import (
     azimuth,
     nearest_neighbor_within,
     shift_point,
     unique_line_points,
@@ -600,15 +601,15 @@
 
     return azimuth(Point(coords[0]), Point(coords[-1]))
 
 
 class ExtensionDirectionEnum(Enum):
     """ """
 
-    start, end, both = assigned_names()
+    start, end, both = "start", "end", "both"  # assigned_names()
 
 
 def extend_line(
     line: LineString,
     offset: float,
     side=ExtensionDirectionEnum.both,
     simplify: bool = True,
```

### Comparing `jord-0.5.4/jord/shapely_utilities/mirroring.py` & `jord-0.5.5/jord/shapely_utilities/mirroring.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/shapely_utilities/morphology.py` & `jord-0.5.5/jord/shapely_utilities/morphology.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/shapely_utilities/points.py` & `jord-0.5.5/jord/shapely_utilities/points.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/shapely_utilities/polygons.py` & `jord-0.5.5/jord/shapely_utilities/polygons.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/shapely_utilities/projection.py` & `jord-0.5.5/jord/shapely_utilities/projection.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/shapely_utilities/rings.py` & `jord-0.5.5/jord/shapely_utilities/rings.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/shapely_utilities/selection.py` & `jord-0.5.5/jord/shapely_utilities/selection.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/jord/shapely_utilities/transformation.py` & `jord-0.5.5/jord/shapely_utilities/transformation.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/setup.py` & `jord-0.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.4/tests/test_import.py` & `jord-0.5.5/tests/test_import.py`

 * *Files identical despite different names*


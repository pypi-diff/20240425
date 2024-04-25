# Comparing `tmp/meshiphi-1.1.6.tar.gz` & `tmp/meshiphi-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshiphi-1.1.6.tar", last modified: Tue Feb 20 14:51:41 2024, max compression
+gzip compressed data, was "meshiphi-2.0.8.tar", last modified: Thu Apr 25 14:59:18 2024, max compression
```

## Comparing `meshiphi-1.1.6.tar` & `meshiphi-2.0.8.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-02-20 14:51:41.908253 meshiphi-1.1.6/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1081 2023-11-28 10:35:02.000000 meshiphi-1.1.6/LICENSE
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       51 2023-11-28 10:35:02.000000 meshiphi-1.1.6/MANIFEST.in
--rw-r--r--   0 gecoomb   (1001) gecoomb   (1001)     5271 2024-02-20 14:51:41.908253 meshiphi-1.1.6/PKG-INFO
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3721 2024-02-19 11:33:08.000000 meshiphi-1.1.6/README.md
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-02-20 14:51:41.888252 meshiphi-1.1.6/meshiphi/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      760 2024-02-16 13:24:06.000000 meshiphi-1.1.6/meshiphi/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4566 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/cli.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-02-20 14:51:41.892252 meshiphi-1.1.6/meshiphi/config_validation/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/config_validation/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     7225 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/config_validation/config_validator.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1624 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/config_validation/mesh_schema.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1144 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/config_validation/route_schema.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      471 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/config_validation/vessel_schema.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       64 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/config_validation/waypoints_schema.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-02-20 14:51:41.892252 meshiphi-1.1.6/meshiphi/dataloaders/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1196 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/dataloader_interface.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     7957 2024-02-16 14:58:20.000000 meshiphi-1.1.6/meshiphi/dataloaders/factory.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-02-20 14:51:41.896252 meshiphi-1.1.6/meshiphi/dataloaders/lut/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/lut/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    16805 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/lut/abstract_lut.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2473 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/lut/density.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2174 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/lut/lut_csv.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2771 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/lut/lut_geojson.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2744 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/lut/lut_shapefile.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1672 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/lut/scotland_ncmpa.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4298 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/lut/thickness.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-02-20 14:51:41.900252 meshiphi-1.1.6/meshiphi/dataloaders/scalar/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/scalar/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    43865 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/scalar/abstract_scalar.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3831 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/scalar/amsr.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1241 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/scalar/baltic_sea_ice.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1584 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/scalar/bsose_depth.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2207 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/scalar/bsose_sea_ice.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3811 2024-02-16 14:58:20.000000 meshiphi-1.1.6/meshiphi/dataloaders/scalar/ecmwf_sig_wave_height.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1854 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/scalar/era5_max_wave_height.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1843 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/scalar/era5_mean_wave_direction.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1855 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/scalar/era5_sig_wave_height.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1843 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/scalar/era5_wave_period.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2053 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/scalar/era5_wind_dir.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1997 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/scalar/era5_wind_mag.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1007 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/scalar/gebco.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4479 2024-02-16 14:58:20.000000 meshiphi-1.1.6/meshiphi/dataloaders/scalar/icenet.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1108 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/scalar/modis.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      934 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/scalar/scalar_csv.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     5039 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/scalar/scalar_grf.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     9220 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/scalar/shape.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2874 2024-02-16 14:58:20.000000 meshiphi-1.1.6/meshiphi/dataloaders/scalar/visual_iced.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-02-20 14:51:41.900252 meshiphi-1.1.6/meshiphi/dataloaders/vector/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/vector/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    50874 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/vector/abstract_vector.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1204 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/vector/baltic_current.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1697 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/vector/duacs_current.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2459 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/vector/era5_wave_direction_vector.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1846 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/vector/era5_wind.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1251 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/vector/north_sea_current.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1331 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/vector/oras5_current.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1271 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/vector/sose.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      934 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/vector/vector_csv.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3828 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/dataloaders/vector/vector_grf.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-02-20 14:51:41.904252 meshiphi-1.1.6/meshiphi/mesh_generation/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/mesh_generation/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4389 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/mesh_generation/aggregated_cellbox.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    11761 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/mesh_generation/boundary.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    14292 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/mesh_generation/cellbox.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      367 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/mesh_generation/direction.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    23449 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/mesh_generation/environment_mesh.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2724 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/mesh_generation/jgrid_aggregated_cellbox.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     7494 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/mesh_generation/jgrid_cellbox.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     5342 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/mesh_generation/mesh.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    28589 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/mesh_generation/mesh_builder.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2122 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/mesh_generation/metadata.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    18340 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/mesh_generation/neighbour_graph.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-02-20 14:51:41.904252 meshiphi-1.1.6/meshiphi/mesh_plotting/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2024-02-20 13:19:59.000000 meshiphi-1.1.6/meshiphi/mesh_plotting/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2839 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/mesh_plotting/mesh_plotter.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-02-20 14:51:41.908253 meshiphi-1.1.6/meshiphi/mesh_validation/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/mesh_validation/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     6913 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/mesh_validation/mesh_validator.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1565 2023-11-28 10:35:02.000000 meshiphi-1.1.6/meshiphi/mesh_validation/sampler.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     8643 2023-11-30 10:48:02.000000 meshiphi-1.1.6/meshiphi/utils.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-02-20 14:51:41.888252 meshiphi-1.1.6/meshiphi.egg-info/
--rw-r--r--   0 gecoomb   (1001) gecoomb   (1001)     5271 2024-02-20 14:51:41.000000 meshiphi-1.1.6/meshiphi.egg-info/PKG-INFO
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3058 2024-02-20 14:51:41.000000 meshiphi-1.1.6/meshiphi.egg-info/SOURCES.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2024-02-20 14:51:41.000000 meshiphi-1.1.6/meshiphi.egg-info/dependency_links.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      149 2024-02-20 14:51:41.000000 meshiphi-1.1.6/meshiphi.egg-info/entry_points.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2023-11-28 10:39:12.000000 meshiphi-1.1.6/meshiphi.egg-info/not-zip-safe
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      193 2024-02-20 14:51:41.000000 meshiphi-1.1.6/meshiphi.egg-info/requires.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        9 2024-02-20 14:51:41.000000 meshiphi-1.1.6/meshiphi.egg-info/top_level.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       38 2024-02-20 14:51:41.908253 meshiphi-1.1.6/setup.cfg
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1690 2023-11-28 10:35:02.000000 meshiphi-1.1.6/setup.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 14:59:18.947528 meshiphi-2.0.8/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1081 2023-11-28 10:35:02.000000 meshiphi-2.0.8/LICENSE
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       51 2023-11-28 10:35:02.000000 meshiphi-2.0.8/MANIFEST.in
+-rw-r--r--   0 gecoomb   (1001) gecoomb   (1001)     5140 2024-04-25 14:59:18.947528 meshiphi-2.0.8/PKG-INFO
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3721 2024-03-06 13:55:59.000000 meshiphi-2.0.8/README.md
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 14:59:18.939529 meshiphi-2.0.8/meshiphi/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      722 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4566 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/cli.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 14:59:18.943529 meshiphi-2.0.8/meshiphi/config_validation/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/config_validation/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     7230 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/config_validation/config_validator.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1624 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/config_validation/mesh_schema.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1144 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/config_validation/route_schema.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      471 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/config_validation/vessel_schema.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       64 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/config_validation/waypoints_schema.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 14:59:18.943529 meshiphi-2.0.8/meshiphi/dataloaders/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1196 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/dataloader_interface.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     7957 2024-03-06 13:55:59.000000 meshiphi-2.0.8/meshiphi/dataloaders/factory.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 14:59:18.943529 meshiphi-2.0.8/meshiphi/dataloaders/lut/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/lut/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    15677 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/dataloaders/lut/abstract_lut.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3031 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/dataloaders/lut/density.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2174 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/lut/lut_csv.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2771 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/lut/lut_geojson.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2744 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/lut/lut_shapefile.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1672 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/lut/scotland_ncmpa.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     5196 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/dataloaders/lut/thickness.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 14:59:18.947528 meshiphi-2.0.8/meshiphi/dataloaders/scalar/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    39720 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/abstract_scalar.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3831 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/amsr.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1241 2024-03-14 13:28:05.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/baltic_sea_ice.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1584 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/bsose_depth.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2207 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/bsose_sea_ice.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3811 2024-02-22 16:13:29.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/ecmwf_sig_wave_height.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1854 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/era5_max_wave_height.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1843 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/era5_mean_wave_direction.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1855 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/era5_sig_wave_height.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1843 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/era5_wave_period.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2053 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/era5_wind_dir.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1997 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/era5_wind_mag.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1007 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/gebco.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4479 2024-02-22 16:13:29.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/icenet.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1108 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/modis.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      934 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/scalar_csv.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     5039 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/scalar_grf.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     9724 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/shape.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2874 2024-03-06 13:55:59.000000 meshiphi-2.0.8/meshiphi/dataloaders/scalar/visual_iced.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 14:59:18.947528 meshiphi-2.0.8/meshiphi/dataloaders/vector/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/vector/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    48488 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/dataloaders/vector/abstract_vector.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1393 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/dataloaders/vector/baltic_current.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1747 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/dataloaders/vector/duacs_current.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2459 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/vector/era5_wave_direction_vector.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1846 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/vector/era5_wind.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1251 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/vector/north_sea_current.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1331 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/vector/oras5_current.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1271 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/vector/sose.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      934 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/vector/vector_csv.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3828 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/dataloaders/vector/vector_grf.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 14:59:18.947528 meshiphi-2.0.8/meshiphi/mesh_generation/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/mesh_generation/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     5456 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/mesh_generation/aggregated_cellbox.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    16466 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/mesh_generation/boundary.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    16632 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/mesh_generation/cellbox.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      367 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/mesh_generation/direction.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    66036 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/mesh_generation/environment_mesh.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2724 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/mesh_generation/jgrid_aggregated_cellbox.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     7494 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/mesh_generation/jgrid_cellbox.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     5342 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/mesh_generation/mesh.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    31997 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/mesh_generation/mesh_builder.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2751 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/mesh_generation/metadata.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    21832 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/mesh_generation/neighbour_graph.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 14:59:18.947528 meshiphi-2.0.8/meshiphi/mesh_plotting/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2024-03-06 13:55:59.000000 meshiphi-2.0.8/meshiphi/mesh_plotting/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2839 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/mesh_plotting/mesh_plotter.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 14:59:18.947528 meshiphi-2.0.8/meshiphi/mesh_validation/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/mesh_validation/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     6913 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/mesh_validation/mesh_validator.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1565 2023-11-28 10:35:02.000000 meshiphi-2.0.8/meshiphi/mesh_validation/sampler.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     9506 2024-04-25 14:57:45.000000 meshiphi-2.0.8/meshiphi/utils.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 14:59:18.943529 meshiphi-2.0.8/meshiphi.egg-info/
+-rw-r--r--   0 gecoomb   (1001) gecoomb   (1001)     5140 2024-04-25 14:59:18.000000 meshiphi-2.0.8/meshiphi.egg-info/PKG-INFO
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3058 2024-04-25 14:59:18.000000 meshiphi-2.0.8/meshiphi.egg-info/SOURCES.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2024-04-25 14:59:18.000000 meshiphi-2.0.8/meshiphi.egg-info/dependency_links.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      149 2024-04-25 14:59:18.000000 meshiphi-2.0.8/meshiphi.egg-info/entry_points.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2023-11-28 10:39:12.000000 meshiphi-2.0.8/meshiphi.egg-info/not-zip-safe
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      169 2024-04-25 14:59:18.000000 meshiphi-2.0.8/meshiphi.egg-info/requires.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        9 2024-04-25 14:59:18.000000 meshiphi-2.0.8/meshiphi.egg-info/top_level.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       38 2024-04-25 14:59:18.951528 meshiphi-2.0.8/setup.cfg
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1676 2024-04-25 14:59:09.000000 meshiphi-2.0.8/setup.py
```

### Comparing `meshiphi-1.1.6/LICENSE` & `meshiphi-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/PKG-INFO` & `meshiphi-2.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 Metadata-Version: 2.1
 Name: meshiphi
-Version: 1.1.6
-Summary: meshiphi: Earth's digital twin mapped on a non-uniform mesh
+Version: 2.0.8
+Summary: MeshiPhi: Earth's digital twin mapped on a non-uniform mesh
 Home-page: https://www.github.com/antarctica
-Author: Samuel Hall, George Coombs, Harrison Abbot, Ayat Fekry, Jonathan Smith, Maria Fox, James Byrne, Michael Thorne
-Author-email: polarroute@bas.ac.uk
-Maintainer: Samuel Hall, George Coombs, Harrison Abbot, Ayat Fekry, Jonathan Smith, Maria Fox, James Byrne, Michael Thorne
-Maintainer-email: polarroute@bas.ac.uk
+Author: Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey
+Author-email: amop@bas.ac.uk
+Maintainer: Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey
+Maintainer-email: amop@bas.ac.uk
 License: MIT
-Classifier: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
-Classifier: 
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dask
 Requires-Dist: geopandas
 Requires-Dist: jsonschema
 Requires-Dist: matplotlib
 Requires-Dist: netcdf4
-Requires-Dist: cfgrib
-Requires-Dist: numpy<=1.24.1,>=1.21.6
-Requires-Dist: pandas<=1.4.4,>=1.3.5
+Requires-Dist: numpy>=1.21.6
+Requires-Dist: pandas>=1.3.5
 Requires-Dist: pytest
 Requires-Dist: rioxarray
 Requires-Dist: shapely>=2.0.1
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Requires-Dist: xarray
```

#### html2text {}

```diff
@@ -1,32 +1,30 @@
-Metadata-Version: 2.1 Name: meshiphi Version: 1.1.6 Summary: meshiphi: Earth's
+Metadata-Version: 2.1 Name: meshiphi Version: 2.0.8 Summary: MeshiPhi: Earth's
 digital twin mapped on a non-uniform mesh Home-page: https://www.github.com/
-antarctica Author: Samuel Hall, George Coombs, Harrison Abbot, Ayat Fekry,
-Jonathan Smith, Maria Fox, James Byrne, Michael Thorne Author-email:
-polarroute@bas.ac.uk Maintainer: Samuel Hall, George Coombs, Harrison Abbot,
-Ayat Fekry, Jonathan Smith, Maria Fox, James Byrne, Michael Thorne Maintainer-
-email: polarroute@bas.ac.uk License: MIT Classifier: Classifier: Development
-Status :: 3 - Alpha Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: System Administrators Classifier: License ::
-OSI Approved :: MIT License Classifier: Natural Language :: English Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Topic :: Scientific/Engineering
-Classifier: Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: dask Requires-Dist: geopandas Requires-Dist: jsonschema
-Requires-Dist: matplotlib Requires-Dist: netcdf4 Requires-Dist: cfgrib
-Requires-Dist: numpy<=1.24.1,>=1.21.6 Requires-Dist: pandas<=1.4.4,>=1.3.5
-Requires-Dist: pytest Requires-Dist: rioxarray Requires-Dist: shapely>=2.0.1
-Requires-Dist: scikit-learn Requires-Dist: scipy Requires-Dist: tqdm Requires-
-Dist: xarray Requires-Dist: cartopy Requires-Dist: rasterio Provides-Extra:
-tests Requires-Dist: pytest; extra == "tests" # MeshiÏ (MeshiPhi) ![]
-(logo.jpg) _[_M_a_n_u_a_l_ _P_a_g_e_]_[_P_y_P_i_]_[_R_e_l_e_a_s_e_ _T_a_g_]_[_I_s_s_u_e_s_]_[_L_i_c_e_n_s_e_]Introducing
-MeshiÏ, a versatile software package designed for comprehensive earth modeling
-and navigation planning. MeshiÏ works by discretizing the Earth's surface into
-a non-uniform grid, allocating higher resolution in regions of geographic
+antarctica Author: Autonomous Marine Operations Planning (AMOP) Team, AI Lab,
+British Antarctic Survey Author-email: amop@bas.ac.uk Maintainer: Autonomous
+Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey
+Maintainer-email: amop@bas.ac.uk License: MIT Classifier: Development Status ::
+3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
+Intended Audience :: System Administrators Classifier: License :: OSI Approved
+:: MIT License Classifier: Natural Language :: English Classifier: Operating
+System :: OS Independent Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.7 Classifier: Topic :: Scientific/Engineering Description-Content-Type:
+text/markdown License-File: LICENSE Requires-Dist: dask Requires-Dist:
+geopandas Requires-Dist: jsonschema Requires-Dist: matplotlib Requires-Dist:
+netcdf4 Requires-Dist: numpy>=1.21.6 Requires-Dist: pandas>=1.3.5 Requires-
+Dist: pytest Requires-Dist: rioxarray Requires-Dist: shapely>=2.0.1 Requires-
+Dist: scikit-learn Requires-Dist: scipy Requires-Dist: tqdm Requires-Dist:
+xarray Requires-Dist: cartopy Requires-Dist: rasterio Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests" # MeshiÏ (MeshiPhi) ![](logo.jpg)
+_[_M_a_n_u_a_l_ _P_a_g_e_]_[_P_y_P_i_]_[_R_e_l_e_a_s_e_ _T_a_g_]_[_I_s_s_u_e_s_]_[_L_i_c_e_n_s_e_]Introducing MeshiÏ, a
+versatile software package designed for comprehensive earth modeling and
+navigation planning. MeshiÏ works by discretizing the Earth's surface into a
+non-uniform grid, allocating higher resolution in regions of geographic
 diversity, and conserving lower resolution in more uniform regions. The
 software also incorporates data-driven vehicle models, with the ability to
 calculate speed limits and fuel needs for specific vessels within each grid
 cell. These mesh objects can be output in standard formats, such as GeoJSON and
 GeoTIFF, enabling data-visualisation via GIS software such as ArcGIS. ##
 Installation MeshiÏ can be installed via pip or by cloning the repository from
 GitHub. Pip: ``` pip install meshiphi ``` Github: (for local development) ```
```

### Comparing `meshiphi-1.1.6/README.md` & `meshiphi-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/cli.py` & `meshiphi-2.0.8/meshiphi/cli.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/config_validation/config_validator.py` & `meshiphi-2.0.8/meshiphi/config_validation/config_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             time_str (str): 
                 String from config. Expects 'YYYY-MM-DD' or 'TODAY +- n'
         Raises:
             ValueError: String not in a valid date format
         """
         correctly_formatted = False
         # If relative time is parsed
-        if re.match('TODAY[+,-]\d+', time_str.replace(' ','')):
+        if re.match(r'TODAY[+,-]\d+', time_str.replace(' ','')):
             correctly_formatted = True
         elif time_str == 'TODAY':
             correctly_formatted = True
         # Otherwise check if date is parsed correctly
         else:
             try:
                 # Checks if formatted as YYYY-MM-DD with a valid date
@@ -90,15 +90,15 @@
         boundary.
 
         Args:
             bound_min (float): Minimum value of boundary in one axis
             bound_max (float): Maximum value of boundary in the same axis
             cell_size (float): Initial cellbox size in the same axis
         """
-        assert((bound_max - bound_min)%cell_size == 0), \
+        assert(((bound_max - bound_min)/cell_size)%1 == 0), \
             f"{bound_max}-{bound_min}={bound_max-bound_min} is not evenly "+\
             f"divided by {cell_size}"
         
         
     # Deals with flexible input
     config_json = flexi_json_input(config)
     # Validate against the schema to check syntax is correct
```

### Comparing `meshiphi-1.1.6/meshiphi/config_validation/mesh_schema.py` & `meshiphi-2.0.8/meshiphi/config_validation/mesh_schema.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/config_validation/route_schema.py` & `meshiphi-2.0.8/meshiphi/config_validation/route_schema.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/dataloader_interface.py` & `meshiphi-2.0.8/meshiphi/dataloaders/dataloader_interface.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/factory.py` & `meshiphi-2.0.8/meshiphi/dataloaders/factory.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/lut/abstract_lut.py` & `meshiphi-2.0.8/meshiphi/dataloaders/lut/abstract_lut.py`

 * *Files 3% similar despite different names*

```diff
@@ -192,19 +192,19 @@
         if data.empty:
             return 0
         else:    
             # Calculate coverage fraction
             bounds_polygon = bounds.to_polygon()
             # Extract out polygons, add to multipolygon
             data_polygon = unary_union([datum for datum in data.tolist()])
-            coverage = data_polygon.area / bounds_polygon.area
 
-            # Cap output at 100%
-            if coverage >= 1:   return 1
-            else:               return coverage
+            overlap_area = data_polygon.intersection(bounds_polygon).area
+            total_area = bounds_polygon.area
+
+            return overlap_area / total_area
         
 
     def trim_datapoints(self, bounds, data=None):
         '''
         Trims datapoints from self.data within boundary defined by 'bounds'.
         self.data can be pd.DataFrame or xr.Dataset
         
@@ -223,45 +223,16 @@
             
         # Find intersection of each polygon to the boundary
         bounds_polygon = bounds.to_polygon()    
         lut_polys = STRtree(list(data['geometry']))
         intersections = lut_polys.query(bounds_polygon, predicate='intersects').tolist()
         # Return only rows intersecting with cellbox boundary
         return data.iloc[intersections]
-
-    def get_val_from_coord(self, long=None, lat=None, return_coords=False):
-        '''
-        Extracts value from self.data with lat and long specified in kwargs.
-        
-        Args:
-            long (float): Longitude coordinate to search for
-            lat (float) : Latitude coordinate to search for
-            return_coords (boolean): 
-                Flag for whether to return coordinates with the value or not
-            
-        Returns:
-            pd.DataFrame: 
-                Either with one entry (the value at the coords), 
-                Optionaly with coordinates associated with it if 
-                return_coords = True
-        '''
-        # Check if lat/long point is within any of the data polygons
-        point = Point(long, lat)
-        values = self.data[point.within(self.data['geometry'])][self.data_name]
-        # Add lat/long coords to df if return_coords True
-        if return_coords:
-            data = pd.DataFrame({'lat': lat,
-                                 'long': long,
-                                 self.data_name: values})
-        else:
-            data = values
-            
-        return data
     
-    def get_value(self, bounds, agg_type=None, skipna=False):
+    def get_value(self, bounds, agg_type=None, skipna=False, data=None):
         '''
         Retrieve aggregated value from within bounds
         
         Args:
             aggregation_type (str): Method of aggregation of datapoints within
                 bounds. Can be upper or lower case. 
                 Accepts 'MIN', 'MAX', 'MEAN', 'MEDIAN', 'STD', 'COUNT'
@@ -273,15 +244,15 @@
             dict: 
                 {variable (str): aggregated_value (float)}
                 Aggregated value within bounds following aggregation_type
                 
         Raises:
             ValueError: aggregation type not in list of available methods
         '''
-        polygons = self.trim_datapoints(bounds)
+        polygons = self.trim_datapoints(bounds, data=data)
         logging.debug(f"\t{len(polygons)} polygons found for attribute " + \
                       f"'{self.data_name}' within bounds '{bounds}'")
         
         ret_val = np.nan
         
         if agg_type is None:
             agg_type = self.aggregate_type
@@ -333,15 +304,15 @@
         
         # Convert numpy bool to python bool for JSON serialisation
         if type(ret_val) is np.bool_:
             ret_val = bool(ret_val)
         
         return { self.data_name: ret_val}
 
-    def get_hom_condition(self, bounds, splitting_conds):
+    def get_hom_condition(self, bounds, splitting_conds, data=None):
         '''
         Retrieves homogeneity condition of data within
         boundary.
          
         Args: 
             bounds (Boundary): Boundary object with limits of datarange to analyse
             splitting_conds (dict): Containing the following keys: \n
@@ -357,15 +328,15 @@
                 'MIN' = the boundary contains no LUT data, can't split \n
                 'HET' = the boundary contains an edge within the LUT data, 
                 should split
                 
         '''
         bounds_polygon = bounds.to_polygon()
         # Extract polygons that overlap the boundary
-        polygons = self.trim_datapoints(bounds)['geometry'].tolist()
+        polygons = self.trim_datapoints(bounds, data=data)['geometry'].tolist()
         
     
         # If there's no polygon that overlaps with bounds        
         if not any([polygon.intersects(bounds_polygon) for polygon in polygons]):
             return 'CLR'
         # If we want to split on the boundary
         elif splitting_conds['boundary']:
```

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/lut/density.py` & `meshiphi-2.0.8/meshiphi/dataloaders/lut/density.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from meshiphi.dataloaders.lut.abstract_lut import LutDataLoader
 
 import logging
 
+import geopandas as gpd
 import pandas as pd
-from shapely import wkt
+from shapely import wkt, Polygon, MultiPolygon
 
 class DensityDataLoader(LutDataLoader):
     def import_data(self, bounds):
         '''
         Creates a simulated dataset of sea ice density based on 
         scientific literature.
         
@@ -21,14 +22,15 @@
                 and variable 'density'
         '''
         
         # Look up table parameters hardcoded
         northern_hemisphere = wkt.loads('POLYGON((-180 0, -180 90, 180 90, 180 0, -180 0))')
         southern_hemisphere = wkt.loads('POLYGON((-180 -90, -180 0, 180 0, 180 -90, -180 -90))')
         
+        # su = summer, au = autumn, wi = winter, sp = spring
         northern_seasons = {
             1: 'wi',  2: 'wi', 12: 'wi',
             3: 'sp',  4: 'sp',  5: 'sp', 
             6: 'su',  7: 'su',  8: 'su', 
             9: 'au', 10: 'au', 11: 'au',
             }
         southern_seasons = {
@@ -57,10 +59,21 @@
                             'geometry': northern_hemisphere & bounds_polygon,    # Intersect shapes
                             'density': [densities[northern_seasons[month]] for month in dates.month]}),
                         pd.DataFrame(
                             {'time': dates,
                             'geometry': southern_hemisphere & bounds_polygon,    # Intersect shapes
                             'density': [densities[southern_seasons[month]] for month in dates.month]})
                         ]
-        )
+        ).reset_index()
+        # Remove empty geometry rows from df
+        drop_idxs = []
+        for idx, row in density_df.iterrows():
+            if row['geometry'].is_empty or \
+               row['geometry'].geom_type not in ['Polygon', 'MultiPolygon']:
+                drop_idxs += [idx]
+
+        density_df.drop(index=drop_idxs, inplace=True)
+        density_df.drop(columns=['index'], inplace=True)
+
+        density_df = density_df.drop_duplicates()
         density_df = density_df.set_index('time').sort_index()
         return density_df
```

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/lut/lut_csv.py` & `meshiphi-2.0.8/meshiphi/dataloaders/lut/lut_csv.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/lut/lut_geojson.py` & `meshiphi-2.0.8/meshiphi/dataloaders/lut/lut_geojson.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/lut/lut_shapefile.py` & `meshiphi-2.0.8/meshiphi/dataloaders/lut/lut_shapefile.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/lut/scotland_ncmpa.py` & `meshiphi-2.0.8/meshiphi/dataloaders/lut/scotland_ncmpa.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/lut/thickness.py` & `meshiphi-2.0.8/meshiphi/dataloaders/lut/thickness.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from meshiphi.dataloaders.lut.abstract_lut import LutDataLoader
 from meshiphi.mesh_generation.boundary import Boundary
 import logging
 
 import pandas as pd
-from shapely import wkt
+from shapely import wkt, Polygon
 
 
 # Mapping of month number to season per hemisphere
 northern_seasons = {
     1: 'wi',  2: 'wi', 12: 'wi',
     3: 'sp',  4: 'sp',  5: 'sp', 
     6: 'su',  7: 'su',  8: 'su', 
@@ -16,14 +16,15 @@
 southern_seasons = {
     1: 'su',  2: 'su', 12: 'su',
     3: 'au',  4: 'au',  5: 'au', 
     6: 'wi',  7: 'wi',  8: 'wi', 
     9: 'sp', 10: 'sp', 11: 'sp',
     }
 
+
 class ThicknessDataLoader(LutDataLoader):
     
     class Region:
         """
         Data storage object with region boundary as polygon, seasonal 
         sea ice densities, and a dict mapping from integer month to season
         """
@@ -41,16 +42,15 @@
             Args:
                 month (int): Month as an integer (1 = Jan ... 12 = Dec)
 
             Returns:
                 float: Sea Ice Density in the specified season
             """
             return self.value_dict[self.month_to_season[month]]
-        
-    
+
     def import_data(self, bounds):
         """
         Creates a simulated dataset of sea ice thickness based on 
         scientific literature.
         
         Args:
             bounds (Boundary): Initial boundary to limit the dataset to
@@ -79,30 +79,48 @@
                         {'wi': 0.59, 'sp': 0.78, 'su': 1.05, 'au': 0.45, 'y': 0.68}),
             self.Region('West Pacific',
                         Boundary([-90, 0], [90, 160]).to_polygon(),
                         {'wi': 0.72, 'sp': 0.68, 'su': 1.17, 'au': 0.75, 'y': 0.79}),
             self.Region('Ross W', 
                         Boundary([-90, 0], [160,   180]).to_polygon(),
                         {'wi': 0.72, 'sp': 0.67, 'su': 1.32, 'au': 0.82, 'y': 1.07}),
+            # Baltic thickness to match example from arxiv paper
+            self.Region('Baltic',
+                        Boundary([54, 66], [12, 32]).to_polygon(),
+                        {'wi': 0.3, 'sp': 0.3, 'su': 0.3, 'au': 0.3, 'y': 0.3},
+                        seasons=northern_seasons),
+            # Keep previous defaults everywhere else
             self.Region('None',
-                        Boundary([0, 90], [-180, 180]).to_polygon(),
+                        Polygon([(-180, 0), (180, 0), (180, 90), (-180, 90)],
+                                holes=[[(12, 54), (32, 54), (32, 66), (12, 66)]]),
                         {'wi': 0.72, 'sp': 0.67, 'su': 1.32, 'au': 0.82, 'y': 1.07},
                         seasons=northern_seasons),
         ]
         
         # Create shape to intersect regions with
         bounds_polygon = bounds.to_polygon()
         
         # For every date in range, create a new shape and value pair
         dates = pd.date_range(start=bounds.get_time_min(), 
                               end=bounds.get_time_max())
         
-        thickness_df = pd.concat([
-                pd.DataFrame({'time': dates,
-                              'geometry': region.geometry & bounds_polygon,
-                              'thickness': region.get_value(month)})
-                for region in regions for month  in dates.month
-            ])
+        thickness_df = pd.DataFrame()
         
+        for region in regions:
+            
+            intersection = region.geometry & bounds_polygon
+            if intersection.geom_type in ['Polygon', 'MultiPolygon'] and \
+               intersection != Polygon():
+                    
+                region_df = pd.concat([
+                        pd.DataFrame({'time': dates,
+                                      'geometry': region.geometry & bounds_polygon,
+                                      'thickness': region.get_value(month)})
+                        for month in dates.month
+                    ])
+                
+                thickness_df = pd.concat([thickness_df, region_df])
+                
+        thickness_df = thickness_df.drop_duplicates()
         thickness_df = thickness_df.set_index('time').sort_index()
         
-        return thickness_df
+        return thickness_df
```

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/scalar/abstract_scalar.py` & `meshiphi-2.0.8/meshiphi/dataloaders/scalar/abstract_scalar.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import logging
 import numpy as np
 import xarray as xr
 import pandas as pd
 from rasterio.enums import Resampling
 
-from meshiphi.utils import round_to_sigfig
+from meshiphi.mesh_generation.boundary import Boundary
 
 
 
 class ScalarDataLoader(DataLoaderInterface):
     '''
     Abstract class for all scalar Datasets.
     '''
@@ -77,17 +77,17 @@
         # Calculate fraction of boundary that data covers
         data_coverage = self.calculate_coverage(bounds)
         logging.info("\tMercator data range (roughly) covers "+\
                     f"{np.round(data_coverage*100,0).astype(int)}% "+\
                      "of initial boundary")
         # If there's 0 datapoints in the initial boundary, raise ValueError
         if data_coverage == 0:
-            logging.error('\tDataloader has no data in initial region!')
-            raise ValueError(f"Dataloader {params['dataloader_name']}"+\
-                              " contains no data within initial region!")
+            logging.warning('\tDataloader has no data in initial region!')
+            #raise ValueError(f"Dataloader {params['dataloader_name']}"+\
+            #                  " contains no data within initial region!")
         else:
             # Cut dataset down to initial boundary
             logging.info(
                 "\tTrimming data to initial boundary: {min} to {max}".format(
                     min=(bounds.get_lat_min(), bounds.get_long_min()),
                     max=(bounds.get_lat_max(), bounds.get_long_max())
                 ))
@@ -185,56 +185,49 @@
                 return 0
             # If no valid coordinates within data range, 0% coverage
             elif data.lat.size == 0 or data.long.size == 0:
                 return 0
             # Otherwise, calculate coverage, assuming rectangular region 
             # in mercator projection
             else:
-                # Get range of latitude values
-                data_lat_range = data.lat.max() - data.lat.min()
-                bounds_lat_range = bounds.get_lat_max() - bounds.get_lat_min()
-                # Get range of longitude values
-                data_long_range = data.long.max() - data.long.min()
-                bounds_long_range = bounds.get_long_max() - bounds.get_long_min()
-                # Calcualte area of each region
-                data_area = data_lat_range * data_long_range
-                bounds_area = bounds_lat_range * bounds_long_range
-                # If data area completely covers bounds, 100% coverage
-                if data_area >= bounds_area:
-                    return 1
-                # Otherwise return decimal fraction
-                else:
-                    return data_area / bounds_area
-                
+                # Create a polygon to calculate overlap region from
+                data_boundary = Boundary([data.lat.min(), data.lat.max()],
+                                         [data.long.min(), data.long.max()])
+                data_polygon = data_boundary.to_polygon()
+                bounds_polygon = bounds.to_polygon()
+
+                # Get fraction of bounds covered by data
+                overlap_area = data_polygon.intersection(bounds_polygon).area
+                total_area = bounds_polygon.area
+
+                return overlap_area / total_area
+
                 
         def calculate_coverage_from_xr(bounds, data):
             # Remove all NaN columns/rows
             data = data.dropna(dim="lat", how="all")
             data = data.dropna(dim="long", how="all")
             # If no valid coordinates within data range, 0% coverage
             if data.lat.size == 0 or data.long.size == 0:
                 return 0
             # Otherwise, calculate coverage, assuming rectangular region 
             # in mercator projection
             else:
-                # Get range of latitude values
-                data_lat_range = data.lat.max().item() - data.lat.min().item()
-                bounds_lat_range = bounds.get_lat_max() - bounds.get_lat_min()
-                # Get range of longitude values
-                data_long_range = data.long.max().item() - data.long.min().item()
-                bounds_long_range = bounds.get_long_max() - bounds.get_long_min()
-                # Calcualte area of each region
-                data_area = data_lat_range * data_long_range
-                bounds_area = bounds_lat_range * bounds_long_range
-                # If data area completely covers bounds, 100% coverage
-                if data_area >= bounds_area:
-                    return 1
-                # Otherwise return decimal fraction
-                else:
-                    return data_area / bounds_area
+                # Create a polygon to calculate overlap region from
+                data_boundary = Boundary([data.lat.min().item(), data.lat.max().item()],
+                                         [data.long.min().item(), data.long.max().item()])
+                data_polygon = data_boundary.to_polygon()
+                bounds_polygon = bounds.to_polygon()
+
+                # Get fraction of bounds covered by data
+                overlap_area = data_polygon.intersection(bounds_polygon).area
+                total_area = bounds_polygon.area
+
+                return overlap_area / total_area
+
         # Use self.data if not no explicit dataset specified
         if data is None:
             data = self.data
         # Calculate data coverage fraction
         if type(self.data) == pd.core.frame.DataFrame:
             return calculate_coverage_from_df(bounds, data)
         elif type(self.data) == xr.core.dataset.Dataset:
@@ -266,18 +259,25 @@
             Returns:
                 pd.DataFrame:
                     Trimmed dataset inclusive of spatial upper bound, and 
                     exclusive of spatial lower bound. Inclusive of both
                     upper and lower time bounds
             '''
             # Mask off any positions not within spatial bounds
-            mask = (data['lat']  > bounds.get_lat_min())  & \
-                   (data['lat']  <= bounds.get_lat_max())  & \
-                   (data['long'] > bounds.get_long_min()) & \
-                   (data['long'] <= bounds.get_long_max())
+            # If not going through antimeridian
+            if bounds.get_long_min() < bounds.get_long_max():
+                mask = (data['lat']  > bounds.get_lat_min())  & \
+                    (data['lat']  <= bounds.get_lat_max())  & \
+                    (data['long'] > bounds.get_long_min()) & \
+                    (data['long'] <= bounds.get_long_max())
+            else:
+                mask = (data['lat']  > bounds.get_lat_min())  & \
+                    (data['lat']  <= bounds.get_lat_max())  & \
+                    (data['long'] <= bounds.get_long_min()) & \
+                    (data['long'] > bounds.get_long_max())
             # Mask with time if time column exists
             if 'time' in data.columns:
                 mask &= (data['time'] >= bounds.get_time_min()) & \
                         (data['time'] <= bounds.get_time_max())
                         
             # Return column of data from within bounds
             return data.loc[mask]
@@ -297,16 +297,22 @@
                 xr.Dataset:
                     Trimmed dataset inclusive of spatial upper bound, and 
                     exclusive of spatial lower bound. Inclusive of both
                     upper and lower time bounds
             '''
             # Select data region within spatial bounds
             # NOTE slice in xarray is inclusive of bounds
-            data = data.sel(lat=slice(bounds.get_lat_min(),  bounds.get_lat_max() ))
-            data = data.sel(long=slice(bounds.get_long_min(), bounds.get_long_max()))
+            data = data.sel(lat=slice(bounds.get_lat_min(), bounds.get_lat_max()))
+            # If not going over antimeridian
+            if bounds.get_long_min() < bounds.get_long_max():
+                data = data.sel(long=slice(bounds.get_long_min(), bounds.get_long_max()))
+            else:
+                data_lhs = data.sel(long=slice(-180, bounds.get_long_max()))
+                data_rhs = data.sel(long=slice(bounds.get_long_min(), 180))
+                data = xr.concat([data_lhs, data_rhs], 'long')
             # Select data region within temporal bounds if time exists as a coordinate
             if 'time' in data.coords.keys():
                 data = data.sel(time=slice(bounds.get_time_min(),  bounds.get_time_max()))
 
             # Trim off any data on the min boundary to be consistent with df
             if bounds.get_lat_min() in data.lat:
                 data = data.where(data.lat  != bounds.get_lat_min(), drop=True)
@@ -316,121 +322,20 @@
             # Return column of data from within bounds
             return data
         
         # If no specific data passed in, default to entire dataset
         if data is None:
             data = self.data
         
-        # Skip trimming if data already completely within bounds
-        if data.lat.min() >  bounds.get_lat_min() and \
-           data.lat.max() <= bounds.get_lat_max() and \
-           data.long.min() >  bounds.get_long_min() and \
-           data.long.max() <= bounds.get_long_max():
-            logging.debug('\tData is already trimmed to bounds!')
-            return data
-        
         if type(data) == pd.core.frame.DataFrame:
             return trim_datapoints_from_df(data, bounds)
         elif type(data) == xr.core.dataset.Dataset:
             return trim_datapoints_from_xr(data, bounds)
-
-    def get_dp_from_coord(self, long=None, lat=None, return_coords=False):
-        '''
-        Extracts datapoint from self.data with lat and long specified in kwargs.
-        self.data can be pd.DataFrame or xr.Dataset. Will return multiple values
-        if one set of coordinates have multiple entries (e.g. time series data)
-        
-        Args:
-            long (float): Longitude coordinate to search for
-            lat (float) : Latitude coordinate to search for
-            
-        Returns:
-            pd.Series:  Column of data values with chosen lat/long. Could be many 
-                datapoints because either bad data or multiple time steps 
-        '''
-        def get_dp_from_coord_df(data, name, long, lat, return_coords):
-            '''
-            Extracts a singular datapoint from dataframe
-            
-            Args:
-                data (pd.DataFrame): 
-                    Dataset to search within
-                name (str): 
-                    Variable name to extract
-                long (float): 
-                    Longitude of datapoint requested
-                lat (float): 
-                    Latitude of datapoint requested
-                return_coords (bool): 
-                    Flag to choose if coords 
-                    are returned with the datapoint or not
-                    
-            Returns:
-                pd.DataFrame:  
-                    Dataframe containing one row with the datapoint
-                    (and coords if requested). If no datapoint found,
-                    returns empty DataFrame.
-            '''
-            # Mask off any positions not within spatial bounds
-            mask = (data['lat']  == lat)  & \
-                   (data['long'] == long) 
-
-            # Include lat/long/time if requested
-            if return_coords: columns = list(data.columns)
-            else:             columns = [name]
-            # Return column of data from within bounds
-            return data.loc[mask][columns]
-        
-        def get_dp_from_coord_xr(data, name, long, lat, return_coords):
-            '''
-            Extracts a singular datapoint from xr.Dataset
-            
-            Args:
-                data (xr.Dataset): 
-                    Dataset to search within
-                name (str): 
-                    Variable name to extract
-                long (float): 
-                    Longitude of datapoint requested
-                lat (float): 
-                    Latitude of datapoint requested
-                return_coords (bool): 
-                    Flag to choose if coords 
-                    are returned with the datapoint or not
-                    
-            Returns:
-                pd.DataFrame:  
-                    Dataframe containing one row with the datapoint
-                    (and coords if requested). If no datapoint found,
-                    returns empty DataFrame.
-            '''
-            # Select data region within spatial bounds
-            data = data.sel(lat=lat, long=long)
-            # Cast as a pd.DataFrame
-            data = data.to_dataframe().reset_index()
-            # Include lat/long/time if requested
-            if return_coords: columns = list(data.columns)
-            else:             columns = [name]
-            # Return column of data from within bounds
-            return data[columns]
-        
-        # Ensure that lat and long provided
-        assert (lat is not None) and (long) is not None, \
-            'Must provide lat and long to this method!'
-            
-        # Choose which method to retrieve data based on input type
-        if hasattr(self, 'data_name'): data_name = self.data_name
-        else:                          data_name = self.get_data_col_name()
-        
-        if type(self.data) == pd.core.frame.DataFrame:
-            return get_dp_from_coord_df(self.data, data_name, long, lat, return_coords)
-        elif type(self.data) == xr.core.dataset.Dataset:
-            return get_dp_from_coord_xr(self.data, data_name, long, lat, return_coords)
     
-    def get_value(self, bounds, agg_type=None, skipna=True):
+    def get_value(self, bounds, data=None, agg_type=None, skipna=True):
         '''
         Retrieve aggregated value from within bounds
         
         Args:
             aggregation_type (str): Method of aggregation of datapoints within
                 bounds. Can be upper or lower case. 
                 Accepts 'MIN', 'MAX', 'MEAN', 'MEDIAN', 'STD', 'COUNT'
@@ -546,25 +451,25 @@
                 raise ValueError(f'Unknown aggregation type {agg_type}')
 
         # Set to params if no specific aggregate type specified
         if agg_type is None:
             agg_type = self.aggregate_type
             
         # Limit data series to just the data, excluding coords/index
-        dps = self.trim_datapoints(bounds)[self.data_name]
+        dps = self.trim_datapoints(bounds, data=data)[self.data_name]
 
         if type(self.data) == pd.core.frame.DataFrame:
             value = get_value_from_df(dps, bounds, agg_type, skipna)
         elif type(self.data) == xr.core.dataset.Dataset:
             value = get_value_from_xr(dps, bounds, agg_type, skipna)
             
         # Cast to regular float before returning so can be saved in JSON later
         return {self.data_name: float(value)}
 
-    def get_hom_condition(self, bounds, splitting_conds):
+    def get_hom_condition(self, bounds, splitting_conds, data=None):
         '''
         Retrieves homogeneity condition of data within
         boundary.
          
         Args: 
             bounds (Boundary): Boundary object with limits of datarange to analyse
             splitting_conds (dict): Containing the following keys: \n
@@ -652,15 +557,14 @@
             if dps.size < self.min_dp: 
                 hom_type = "CLR"
                 logging.debug(f"\t{dps.size} datapoints found for attribute '{self.data_name}' within bounds '{bounds}'")
             else:
                 # Determine fraction of datapoints over threshold value
                 num_over_threshold = np.count_nonzero(dps > splitting_conds['threshold'])
                 frac_over_threshold = num_over_threshold/dps.size
-                       
                 # Return homogeneity condition
                 if   frac_over_threshold <= splitting_conds['lower_bound']: hom_type = "CLR"
                 elif frac_over_threshold >= splitting_conds['upper_bound']: 
                     if splitting_conds['split_lock'] == True:
                         hom_type = "HOM"
                         logging.debug(f"\tSplitting locked by attribute: '{self.data_name}' in bounds:'{bounds}'")
                     else: hom_type = "CLR"
@@ -669,16 +573,19 @@
             logging.debug(f"\thom_condition for attribute: '{self.data_name}' in bounds:'{bounds}' returned '{hom_type}'")
             
             return hom_type
         
         # Set default values for splitting_conds if not provided
         if 'split_lock' not in splitting_conds:
             splitting_conds['split_lock'] = False
+        if data is None:
+            dps = self.trim_datapoints(bounds)[self.data_name]
+        else:
+            dps = data[self.data_name]
 
-        dps = self.trim_datapoints(bounds)[self.data_name]
         # Retrieve datapoints to analyse
         if type(dps) == pd.core.series.Series:
             return get_hom_condition_from_df(dps, splitting_conds)
         elif type(dps) == xr.core.dataarray.DataArray:
             return get_hom_condition_from_xr(dps, splitting_conds)
         else:
             raise TypeError(f'Unknown type {type(dps)}')
```

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/scalar/amsr.py` & `meshiphi-2.0.8/meshiphi/dataloaders/scalar/amsr.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/scalar/baltic_sea_ice.py` & `meshiphi-2.0.8/meshiphi/dataloaders/scalar/baltic_sea_ice.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/scalar/bsose_depth.py` & `meshiphi-2.0.8/meshiphi/dataloaders/scalar/bsose_depth.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/scalar/bsose_sea_ice.py` & `meshiphi-2.0.8/meshiphi/dataloaders/scalar/bsose_sea_ice.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/scalar/ecmwf_sig_wave_height.py` & `meshiphi-2.0.8/meshiphi/dataloaders/scalar/ecmwf_sig_wave_height.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/scalar/era5_max_wave_height.py` & `meshiphi-2.0.8/meshiphi/dataloaders/scalar/era5_max_wave_height.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/scalar/era5_mean_wave_direction.py` & `meshiphi-2.0.8/meshiphi/dataloaders/scalar/era5_mean_wave_direction.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/scalar/era5_sig_wave_height.py` & `meshiphi-2.0.8/meshiphi/dataloaders/scalar/era5_sig_wave_height.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/scalar/era5_wave_period.py` & `meshiphi-2.0.8/meshiphi/dataloaders/scalar/era5_wave_period.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/scalar/era5_wind_dir.py` & `meshiphi-2.0.8/meshiphi/dataloaders/scalar/era5_wind_dir.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/scalar/era5_wind_mag.py` & `meshiphi-2.0.8/meshiphi/dataloaders/scalar/era5_wind_mag.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/scalar/gebco.py` & `meshiphi-2.0.8/meshiphi/dataloaders/scalar/gebco.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/scalar/icenet.py` & `meshiphi-2.0.8/meshiphi/dataloaders/scalar/icenet.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/scalar/modis.py` & `meshiphi-2.0.8/meshiphi/dataloaders/scalar/modis.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/scalar/scalar_csv.py` & `meshiphi-2.0.8/meshiphi/dataloaders/scalar/scalar_csv.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/scalar/scalar_grf.py` & `meshiphi-2.0.8/meshiphi/dataloaders/scalar/scalar_grf.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/scalar/shape.py` & `meshiphi-2.0.8/meshiphi/dataloaders/scalar/shape.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,20 +123,22 @@
         # For each combination of lat/long
         for i in range(self.ny):
             for j in range(self.nx):
                 # Create a new row, adding mask value
                 row = pd.DataFrame(data={'lat':self.lat[i], 
                                          'long':self.long[j], 
                                          'dummy_data':mask[i][j]}, index=[0])
-                dummy_df = pd.concat([dummy_df, row], ignore_index=True)
+                # Avoid concat with empty df
+                if dummy_df.empty: dummy_df = row
+                else:              dummy_df = pd.concat([dummy_df, row], 
+                                                        ignore_index=True)
                 
         # Change boolean values to int
-        dummy_df = dummy_df.replace(False, 0)
-        dummy_df = dummy_df.replace(True, 1)
-
+        dummy_df['dummy_data'] = dummy_df['dummy_data'].astype(int)
+        
         return dummy_df
 
     def gen_gradient(self, bounds):
         """
             Generates a gradient within bounds of lat/long min/max.
             Gradient direction can be defined in the config, as well as
             resolution of simulated datapoints
@@ -165,15 +167,18 @@
             for j in range(self.nx):
                 # Change dummy data depending on which axis to gradient
                 datum = gradient[i] if self.vertical else gradient[j]
                 # Create a new row, adding datum value
                 row = pd.DataFrame(data={'lat':self.lat[i], 
                                          'long':self.long[j], 
                                          'dummy_data':datum}, index=[0])
-                dummy_df = pd.concat([dummy_df, row], ignore_index=True)  
+                # Avoid concat with empty df
+                if dummy_df.empty:  dummy_df = row
+                else:               dummy_df = pd.concat([dummy_df, row], 
+                                                         ignore_index=True)  
         
         return dummy_df
 
     def gen_checkerboard(self, bounds):
         """
             Generates a checkerboard pattern within bounds of lat/long min/max
             Square size can be defined in the config, as well as resolution of 
@@ -206,12 +211,15 @@
             for j in range(self.nx):
                 # Horizontal XOR Vertical should create boxes
                 datum = (horizontal[i] + vertical[j]) % 2
                 # Create a new row, adding datum value
                 row = pd.DataFrame(data={'lat':self.lat[i], 
                                          'long':self.long[j], 
                                          'dummy_data':datum}, index=[0])
-                dummy_df = pd.concat([dummy_df, row], ignore_index=True)
+                # Avoid concat with empty df
+                if dummy_df.empty:  dummy_df = row
+                else:               dummy_df = pd.concat([dummy_df, row], 
+                                                         ignore_index=True)
         
         return dummy_df    
 
     # TODO Add square
```

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/scalar/visual_iced.py` & `meshiphi-2.0.8/meshiphi/dataloaders/scalar/visual_iced.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/vector/abstract_vector.py` & `meshiphi-2.0.8/meshiphi/dataloaders/vector/abstract_vector.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import logging
 import numpy as np
 import xarray as xr
 import pandas as pd
 from rasterio.enums import Resampling
 
-from meshiphi.utils import round_to_sigfig
+from meshiphi.mesh_generation.boundary import Boundary
 
 
 class VectorDataLoader(DataLoaderInterface):
     '''
     Abstract class for all vector Datasets.
     '''
     def __init__(self, bounds, params):
@@ -79,17 +79,17 @@
         # Calculate fraction of boundary that data covers
         data_coverage = self.calculate_coverage(bounds)
         logging.info("\tMercator data range (roughly) covers "+\
                     f"{np.round(data_coverage*100,0).astype(int)}% "+\
                      "of initial boundary")
         # If there's 0 datapoints in the initial boundary, raise ValueError
         if data_coverage == 0:
-            logging.error('\tDataloader has no data in initial region!')
-            raise ValueError(f"Dataloader {params['dataloader_name']}"+\
-                              " contains no data within initial region!")
+            logging.warning('\tDataloader has no data in initial region!')
+            # raise ValueError(f"Dataloader {params['dataloader_name']}"+\
+                            #   " contains no data within initial region!")
         else:
             # Cut dataset down to initial boundary
             logging.info(
                 "\tTrimming data to initial boundary: {min} to {max}".format(
                     min=(bounds.get_lat_min(), bounds.get_long_min()),
                     max=(bounds.get_lat_max(), bounds.get_long_max())
                 ))
@@ -252,57 +252,50 @@
                 return 0
             # If no valid coordinates within data range, 0% coverage
             elif data.lat.size == 0 or data.long.size == 0:
                 return 0
             # Otherwise, calculate coverage, assuming rectangular region 
             # in mercator projection
             else:
-                # Get range of latitude values
-                data_lat_range = data.lat.max() - data.lat.min()
-                bounds_lat_range = bounds.get_lat_max() - bounds.get_lat_min()
-                # Get range of longitude values
-                data_long_range = data.long.max() - data.long.min()
-                bounds_long_range = bounds.get_long_max() - bounds.get_long_min()
-                # Calcualte area of each region
-                data_area = data_lat_range * data_long_range
-                bounds_area = bounds_lat_range * bounds_long_range
-                # If data area completely covers bounds, 100% coverage
-                if data_area >= bounds_area:
-                    return 1
-                # Otherwise return decimal fraction
-                else:
-                    return data_area / bounds_area
+                # Create a polygon to calculate overlap region from
+                data_boundary = Boundary([data.lat.min(), data.lat.max()],
+                                         [data.long.min(), data.long.max()])
+                data_polygon = data_boundary.to_polygon()
+                bounds_polygon = bounds.to_polygon()
+
+                # Get fraction of bounds covered by data
+                overlap_area = data_polygon.intersection(bounds_polygon).area
+                total_area = bounds_polygon.area
+
+                return overlap_area / total_area
                 
                 
         def calculate_coverage_from_xr(bounds, data):
             # Remove all NaN columns/rows
             data = data.dropna(dim="lat", how="all")
             data = data.dropna(dim="long", how="all")
             
             # If no valid coordinates within data range, 0% coverage
             if data.lat.size == 0 or data.long.size == 0:
                 return 0
             # Otherwise, calculate coverage, assuming rectangular region 
             # in mercator projection
             else:
-                # Get range of latitude values
-                data_lat_range = data.lat.max().item() - data.lat.min().item()
-                bounds_lat_range = bounds.get_lat_max() - bounds.get_lat_min()
-                # Get range of longitude values
-                data_long_range = data.long.max().item() - data.long.min().item()
-                bounds_long_range = bounds.get_long_max() - bounds.get_long_min()
-                # Calcualte area of each region
-                data_area = data_lat_range * data_long_range
-                bounds_area = bounds_lat_range * bounds_long_range
-                # If data area completely covers bounds, 100% coverage
-                if data_area >= bounds_area:
-                    return 1
-                # Otherwise return decimal fraction
-                else:
-                    return data_area / bounds_area
+                # Create a polygon to calculate overlap region from
+                data_boundary = Boundary([data.lat.min().item(), data.lat.max().item()],
+                                         [data.long.min().item(), data.long.max().item()])
+                data_polygon = data_boundary.to_polygon()
+                bounds_polygon = bounds.to_polygon()
+
+                # Get fraction of bounds covered by data
+                overlap_area = data_polygon.intersection(bounds_polygon).area
+                total_area = bounds_polygon.area
+
+                return overlap_area / total_area
+            
         # Use self.data if not no explicit dataset specified
         if data is None:
             data = self.data
         # Calculate data coverage fraction
         if type(self.data) == pd.core.frame.DataFrame:
             return calculate_coverage_from_df(bounds, data)
         elif type(self.data) == xr.core.dataset.Dataset:
@@ -321,18 +314,25 @@
                 Trimmed dataset in same format as self.data
         '''
         def trim_datapoints_from_df(data, bounds):
             '''
             Extracts data from a pd.DataFrame
             '''
             # Mask off any positions not within spatial bounds
-            mask = (data['lat']  > bounds.get_lat_min())  & \
-                   (data['lat']  <= bounds.get_lat_max())  & \
-                   (data['long'] > bounds.get_long_min()) & \
-                   (data['long'] <= bounds.get_long_max())
+            # If not going through antimeridian
+            if bounds.get_long_min() < bounds.get_long_max():
+                mask = (data['lat']  > bounds.get_lat_min())  & \
+                    (data['lat']  <= bounds.get_lat_max())  & \
+                    (data['long'] > bounds.get_long_min()) & \
+                    (data['long'] <= bounds.get_long_max())
+            else:
+                mask = (data['lat']  > bounds.get_lat_min())  & \
+                    (data['lat']  <= bounds.get_lat_max())  & \
+                    (data['long'] <= bounds.get_long_min()) & \
+                    (data['long'] > bounds.get_long_max())
             # Mask with time if time column exists
             if 'time' in data.columns:
                 mask &= (data['time'] >= bounds.get_time_min()) & \
                         (data['time'] <= bounds.get_time_max())
                         
             # Return column of data from within bounds
             return data.loc[mask]
@@ -341,15 +341,21 @@
             '''
             Extracts data from a xr.Dataset
             '''
 
             # Select data region within spatial bounds
             # NOTE slice in xarray is inclusive of bounds
             data = data.sel(lat=slice(bounds.get_lat_min(),  bounds.get_lat_max() ))
-            data = data.sel(long=slice(bounds.get_long_min(), bounds.get_long_max()))
+            # If not going over antimeridian
+            if bounds.get_long_min() < bounds.get_long_max():
+                data = data.sel(long=slice(bounds.get_long_min(), bounds.get_long_max()))
+            else:
+                data_lhs = data.sel(long=slice(-180, bounds.get_long_max()))
+                data_rhs = data.sel(long=slice(bounds.get_long_min(), 180))
+                data = xr.concat([data_lhs, data_rhs], 'long')
             # Select data region within temporal bounds if time exists as a coordinate
             if 'time' in data.coords.keys():
                 data = data.sel(time=slice(bounds.get_time_min(),  bounds.get_time_max()))
 
             # Trim off any data on the min boundary to be consistent with df
             if bounds.get_lat_min() in data.lat:
                 data = data.where(data.lat  != bounds.get_lat_min(), drop=True)
@@ -358,82 +364,21 @@
             
             # Return column of data from within bounds
             return data
         
         # If no specific data passed in, default to entire dataset
         if data is None:
             data = self.data
-            
-        # Skip trimming if data already completely within bounds
-        if data.lat.min() >  bounds.get_lat_min() and \
-           data.lat.max() <= bounds.get_lat_max() and \
-           data.long.min() >  bounds.get_long_min() and \
-           data.long.max() <= bounds.get_long_max():
-            logging.debug('\tData is already trimmed to bounds!')
-            return data
         
         if type(data) == pd.core.frame.DataFrame:
             return trim_datapoints_from_df(data, bounds)
         elif type(data) == xr.core.dataset.Dataset:
             return trim_datapoints_from_xr(data, bounds)
-
-    def get_dp_from_coord(self, long=None, lat=None, return_coords=False):
-        '''
-        Extracts datapoint from self.data with lat and long specified in kwargs.
-        self.data can be pd.DataFrame or xr.Dataset. Will return multiple values
-        if one set of coordinates have multiple entries (e.g. time series data)
-        
-        Args:
-            long (float): Longitude coordinate to search for
-            lat (float) : Latitude coordinate to search for
-            
-        Returns:
-            pd.Dataframe:  
-                Column of data values with chosen lat/long. Could be many 
-                datapoints because either bad data or multiple time steps 
-        '''
-        def get_dp_from_coord_df(data, names, long, lat, return_coords):
-            '''
-            Extracts data from a pd.DataFrame
-            '''
-            # Mask off any positions not within spatial bounds
-            mask = (data['lat']  == lat)  & \
-                   (data['long'] == long) 
-
-            # Include lat/long/time if requested
-            if return_coords: columns = list(data.columns)
-            else:             columns = names
-            # Return column of data from within bounds
-            return data.loc[mask][columns]
-        
-        def get_dp_from_coord_xr(data, names, long, lat, return_coords):
-            '''
-            Extracts data from a xr.Dataset
-            '''
-            # Select data region within spatial bounds
-            data = data.sel(lat=lat, long=long)
-            # Cast as a pd.DataFrame
-            data = data.to_dataframe().reset_index()
-            # Include lat/long/time if requested
-            if return_coords: columns = list(data.columns)
-            else:             columns = names
-            # Return column of data from within bounds
-            return data[columns]
-        
-        # Ensure that lat and long provided
-        assert (lat is not None) and (long) is not None, \
-            'Must provide lat and long to this method!'
-            
-        # Choose which method to retrieve data based on input type
-        if type(self.data) == pd.core.frame.DataFrame:
-            return get_dp_from_coord_df(self.data, self.data_name_list, long, lat, return_coords)
-        elif type(self.data) == xr.core.dataset.Dataset:
-            return get_dp_from_coord_xr(self.data, self.data_name_list, long, lat, return_coords)
     
-    def get_value(self, bounds, agg_type=None, skipna=True):
+    def get_value(self, bounds, agg_type=None, skipna=True, data=None):
         '''
         Retrieve aggregated value from within bounds
         
         Args:
             aggregation_type (str): Method of aggregation of datapoints within
                 bounds. Can be upper or lower case. 
                 Accepts 'MIN', 'MAX', 'MEAN', 'MEDIAN', 'STD', 'COUNT'
@@ -556,25 +501,28 @@
     
 
         # Set to params if no specific aggregate type specified
         if agg_type is None:
             agg_type = self.aggregate_type
             
         # Limit data to boundary
-        dps = self.trim_datapoints(bounds)
+        if data is None:
+            dps = self.trim_datapoints(bounds, data=data)
+        else:
+            dps = data
         # Get list of values
         if type(self.data) == pd.core.frame.DataFrame:
             values = get_value_from_df(dps, self.data_name_list, bounds, agg_type, skipna)
         elif type(self.data) == xr.core.dataset.Dataset:
             values = get_value_from_xr(dps, self.data_name_list, bounds, agg_type, skipna)
             
         # Put in dict to map variable to values
         return {self.data_name_list[i]: values[i] for i in range(len(self.data_name_list))}
 
-    def get_hom_condition(self, bounds, splitting_conds, agg_type='MEAN'):
+    def get_hom_condition(self, bounds, splitting_conds, agg_type='MEAN', data=None):
         '''
         Retrieves homogeneity condition of data within boundary. 
          
         Args: 
             bounds (Boundary): Boundary object with limits of datarange to analyse
             splitting_conds (dict): Containing the following keys: \n
                 'threshold':  
@@ -586,14 +534,17 @@
             str:
                 The homogeniety condtion returned is of the form: \n
                 'MIN' = the cellbox contains less than a minimum number of 
                 data points \n
                 'HET' = Threshold values defined in config are exceeded \n
                 'CLR' = None of the HET conditions were triggered \n
         '''
+        if data is None:
+            data = self.trim_datapoints(bounds)
+
         # Get length of dataset in bounds  
         if type(self.data) == pd.core.frame.DataFrame:
             num_dp = len(self.trim_datapoints(bounds))
         elif type(self.data) == xr.core.dataset.Dataset:
             num_dp = min(self.trim_datapoints(bounds).count().values())
 
         # Set default homogeneity 
@@ -1171,16 +1122,16 @@
             # Combine into field of vectors
             vector_field = np.stack((vector_x_field, vector_y_field), axis=-1)
             vector_field = np.swapaxes(vector_field, 0, 1)
             return vector_field
         
         def meshgrid_from_xr(data, data_name_list):
             # Extract out each variable and combine as tuple
-            data_arrays = (data[name].values 
-                           for name in data_name_list)
+            data_arrays = [data[name].values 
+                                for name in data_name_list]
             # Zip them together to make 2D array of n-dimensional vectors
             return np.dstack(data_arrays)
         
         if type(data) == pd.core.frame.DataFrame:
             return meshgrid_from_df(data, data_name_list)
         elif type(data) == xr.core.dataset.Dataset:
             return meshgrid_from_xr(data, data_name_list)
```

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/vector/baltic_current.py` & `meshiphi-2.0.8/meshiphi/dataloaders/vector/oras5_current.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from meshiphi.dataloaders.vector.abstract_vector import VectorDataLoader
 
 import logging
- 
+
 import xarray as xr
+import numpy as np
 
-class BalticCurrentDataLoader(VectorDataLoader):
+#TODO Read in 2 files, combine to one object
+class ORAS5CurrentDataLoader(VectorDataLoader):
     def import_data(self, bounds):
         '''
-        Reads in current data from a copernicus baltic sea physics reanalysis NetCDF file.
+        Reads in data from a ORAS5 Depth NetCDF files. 
         Renames coordinates to 'lat' and 'long', and renames variable to 
         'uC, vC'
         
         Args:
             bounds (Boundary): Initial boundary to limit the dataset to
             
         Returns:
             xr.Dataset: 
-                Baltic currents dataset within limits of bounds. 
+                ORAS5 currents dataset within limits of bounds. 
                 Dataset has coordinates 'lat', 'long', and variable 'uC', 'vC'
         '''
         # Open Dataset
         if len(self.files) == 1:    data = xr.open_dataset(self.files[0])
         else:                       data = xr.open_mfdataset(self.files)
+        
         # Change column names
-        data = data.rename({'latitude': 'lat',
-                            'longitude': 'long',
+        data = data.rename({'nav_lon': 'long',
+                            'nav_lat': 'lat',
                             'uo': 'uC',
                             'vo': 'vC'})
+        # Limit to just these coords and variables
+        data = data[['lat','long','uC','vC']]
         
-        # Trim to initial datapoints
+        # Limit to initial boundary
         data = self.trim_datapoints(bounds, data=data)
         
-        return data
+        return data
```

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/vector/duacs_current.py` & `meshiphi-2.0.8/meshiphi/dataloaders/vector/duacs_current.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         if len(self.files) == 1:    data = xr.open_dataset(self.files[0])
         else:                       data = xr.open_mfdataset(self.files).compute()
         # Change column names
         data = data.rename({'latitude': 'lat',
                             'longitude': 'long',
                             'ugos': 'uC',
                             'vgos': 'vC'})
-        # Drop unnecessary variable
-        data = data.drop_vars('crs')
+
+        # Drop unnecessary variable, if present
+        if 'crs' in data.keys():
+            data = data.drop_vars('crs')
 
         # Trim to initial datapoints
         data = self.trim_datapoints(bounds, data=data)
 
         return data
```

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/vector/era5_wave_direction_vector.py` & `meshiphi-2.0.8/meshiphi/dataloaders/vector/era5_wave_direction_vector.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/vector/era5_wind.py` & `meshiphi-2.0.8/meshiphi/dataloaders/vector/era5_wind.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/vector/north_sea_current.py` & `meshiphi-2.0.8/meshiphi/dataloaders/vector/north_sea_current.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/vector/oras5_current.py` & `meshiphi-2.0.8/meshiphi/dataloaders/vector/baltic_current.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 from meshiphi.dataloaders.vector.abstract_vector import VectorDataLoader
 
 import logging
-
+ 
 import xarray as xr
-import numpy as np
 
-#TODO Read in 2 files, combine to one object
-class ORAS5CurrentDataLoader(VectorDataLoader):
+
+class BalticCurrentDataLoader(VectorDataLoader):
     def import_data(self, bounds):
-        '''
-        Reads in data from a ORAS5 Depth NetCDF files. 
-        Renames coordinates to 'lat' and 'long', and renames variable to 
+        """
+        Reads in current data from a copernicus baltic sea physics reanalysis NetCDF file.
+        Renames coordinates to 'lat' and 'long', and renames variable to
         'uC, vC'
-        
+
         Args:
             bounds (Boundary): Initial boundary to limit the dataset to
-            
+
         Returns:
-            xr.Dataset: 
-                ORAS5 currents dataset within limits of bounds. 
+            xr.Dataset:
+                Baltic currents dataset within limits of bounds.
                 Dataset has coordinates 'lat', 'long', and variable 'uC', 'vC'
-        '''
+        """
         # Open Dataset
         if len(self.files) == 1:    data = xr.open_dataset(self.files[0])
         else:                       data = xr.open_mfdataset(self.files)
-        
+
+        # Reduce and drop unused depth dimension
+        data = data.isel(depth=0)
+        data = data.reset_coords(names="depth", drop=True)
         # Change column names
-        data = data.rename({'nav_lon': 'long',
-                            'nav_lat': 'lat',
+        data = data.rename({'latitude': 'lat',
+                            'longitude': 'long',
                             'uo': 'uC',
                             'vo': 'vC'})
-        # Limit to just these coords and variables
-        data = data[['lat','long','uC','vC']]
-        
-        # Limit to initial boundary
+
+        # Trim to initial datapoints
         data = self.trim_datapoints(bounds, data=data)
+
+        # Reduce along time dimension
+        data = data.mean(dim="time")
         
-        return data
+        return data
```

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/vector/sose.py` & `meshiphi-2.0.8/meshiphi/dataloaders/vector/sose.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/vector/vector_csv.py` & `meshiphi-2.0.8/meshiphi/dataloaders/vector/vector_csv.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/dataloaders/vector/vector_grf.py` & `meshiphi-2.0.8/meshiphi/dataloaders/vector/vector_grf.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/mesh_generation/aggregated_cellbox.py` & `meshiphi-2.0.8/meshiphi/mesh_generation/aggregated_cellbox.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,19 +19,39 @@
         """
 
             Args:
                 cellbox_json(Json): json object that encapsulates boundary, agg_data and id of the CellBox
         """
         cellbox_id = cellbox_json ['id']
         def load_boundary (cellbox_json):
-        
             shape = shapely.wkt.loads (cellbox_json ["geometry"])
-            bounds = shape.bounds
-            lat_range = [bounds[1] , bounds[3]]
-            long_range = [bounds [0], bounds [2]]
+            # Take case where crossing antimeridian
+            if shape.geom_type == 'MultiPolygon':
+                shapes = list(shape.geoms)
+                assert (len(shapes) == 2), 'Too many polygons in MultiPolygon boundary!'
+                bounds_a = shapes[0].bounds
+                bounds_b = shapes[1].bounds
+
+                # Bottom left should be origin from which all polygons are defined
+                # They should have the same lat range
+                lat_range = [bounds_a[1] , bounds_a[3]]
+                # Left most boundary and right most boundary are from two different polygons
+                # Right boundary of bounds_a should be 180, 
+                # and left boundary of bounds_b should be -180
+                long_range = [bounds_a [0], bounds_b [2]]
+
+            # Otherwise it's just a normal cellbox
+            elif shape.geom_type == 'Polygon':
+                bounds = shape.bounds
+                lat_range = [bounds[1] , bounds[3]]
+                long_range = [bounds [0], bounds [2]]
+            # Or something is wrong with the mesh
+            else:
+                raise TypeError(f'Expected Polygon or MultiPolygon, instead got {shape.geom_type}')
+            
             return Boundary (lat_range , long_range)
 
         def load_agg_data (cellbox_json):
             dict_obj = {}
             for key in cellbox_json:
                 if key  not in [  "geometry","cx", "cy", "dcx", "dcy"]:
                     dict_obj[key] = cellbox_json[key]
@@ -114,15 +134,15 @@
                     ...,\n
                     "agg_value_n" (float): ...\n
                 }\n
             Returns:
                 cell_json (dict): A JSON parsable dictionary representation of this AggregatedCellBox
         '''
         cell_json = {
-            "geometry": str(Polygon(self.get_bounds().get_bounds())),
+            "geometry": str(self.get_bounds().to_poly_string()),
             'cx': float(self.get_bounds().getcx()),
             'cy': float(self.get_bounds().getcy()),
             'dcx': float(self.get_bounds().getdcx()),
             'dcy': float(self.get_bounds().getdcy()),
            
         }
 
@@ -141,12 +161,12 @@
                 lat (float): latitude of a given point
                 long (float): longitude of a given point
 
             Returns:
                 contains_points (bool): True if this CellBox contains a point given by
                     parameters (lat, long)
         """
-        if (lat >= self.boundary.get_lat_min()) & (lat <= self.boundary.get_lat_max()):
-            if (long >= self.boundary.get_long_min()) & (long <= self.boundary.get_long_max()):
+        if (lat >= self.boundary.get_lat_min()) & (lat < self.boundary.get_lat_max()):
+            if (long >= self.boundary.get_long_min()) & (long < self.boundary.get_long_max()):
                 return True
         return False
```

### Comparing `meshiphi-1.1.6/meshiphi/mesh_generation/cellbox.py` & `meshiphi-2.0.8/meshiphi/mesh_generation/cellbox.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 
 """
 
 
 import numpy as np
 from meshiphi.mesh_generation.boundary import Boundary
 from meshiphi.mesh_generation.aggregated_cellbox import AggregatedCellBox
+from meshiphi.mesh_generation.metadata import Metadata
 import logging
+import time
+from meshiphi.utils import longitude_domain
 
 
 
 class CellBox:
     """
     A CellBox represnts a geo-spatial/temporal boundary that enables projecting to information within.
     Information about any given value of a CellBox is calculated from aggregating all data points of within those bounds.
@@ -166,19 +169,19 @@
         """
         hom_conditions = []
 
         current_data_source = None
         for index in range(0, stop_index):
             current_data_source = self.get_data_source()[index]
             data_loader = current_data_source.get_data_loader()
+            data_subset = current_data_source.get_data_subset()
             for splitting_cond in current_data_source.get_splitting_conditions():
                 hom_cond = data_loader.get_hom_condition(
-                    self.bounds, splitting_cond)
+                    self.bounds, splitting_cond, data=data_subset)
                 hom_conditions.append(hom_cond)
-
         if "HOM" in hom_conditions:
             return False
         if "MIN" in hom_conditions:
             return False
         if hom_conditions.count("CLR") == len(hom_conditions):
             return False
 
@@ -203,17 +206,18 @@
             Returns:
                 should_split (bool): True if the splitting_conditions of this CellBox
                     will result in the CellBox being split.
         """
         hom_conditions = []
         for current_data_source in self.data_source:
             data_loader = current_data_source.get_data_loader()
+            data_subset = current_data_source.get_data_subset()
             for splitting_cond in current_data_source.get_splitting_conditions():
                 hom_cond = data_loader.get_hom_condition(
-                    self.bounds, splitting_cond)
+                    self.bounds, splitting_cond, data=data_subset)
                 hom_conditions.append(hom_cond)
 
         if "HOM" in hom_conditions:
             return False
         if "MIN" in hom_conditions:
             return False
         if hom_conditions.count("CLR") == len(hom_conditions):
@@ -233,49 +237,63 @@
                  the cellbox uniformly.
         """
         split_boxes = self.create_splitted_cell_boxes(start_id)
 
         # set CellBox split_depth, data_source and parent
         for split_box in split_boxes:
             split_box.set_split_depth(self.get_split_depth() + 1)
-            split_box.set_data_source(self.get_data_source())
+            # Create metadata with data subset
+            split_box_data_sources = []
+            for source in self.get_data_source():
+                # Extract data for each new cellbox
+                data_subset = source.data_loader.trim_datapoints(split_box.bounds, data=source.data_subset)
+                # Update metadata with that (rest stays the same)             
+                split_box_data_source = Metadata(source.get_data_loader(), 
+                                                 source.get_splitting_conditions(),
+                                                 source.get_value_fill_type(),
+                                                 data_subset)
+                split_box_data_sources += [split_box_data_source]
+            split_box.set_data_source(split_box_data_sources)
             split_box.set_parent(self)
-
         return split_boxes
 
     def create_splitted_cell_boxes(self, index):
         """
         method that creates 4 splitted cellbox
         """
         half_width = self.bounds.get_width() / 2
         half_height = self.bounds.get_height() / 2
 
         # create 4 new cellboxes
         time_range = self.bounds.get_time_range()
         lat = self.bounds.get_lat_min()
         lat_range = [lat + half_height, lat + self.bounds.get_height()]
         long = self.bounds.get_long_min()
-        long_range = [long, long + half_width]
+        long_range = [long, 
+                      longitude_domain(long + half_width)]
         boundary = Boundary(lat_range, long_range, time_range)
         north_west = CellBox(boundary, str(index))
 
         lat_range = [lat + half_height, lat + self.bounds.get_height()]
-        long_range = [long + half_width, long + self.bounds.get_width()]
+        long_range = [longitude_domain(long + half_width), 
+                      longitude_domain(long + self.bounds.get_width())]
         boundary = Boundary(lat_range, long_range, time_range)
         index += 1
         north_east = CellBox(boundary, str(index))
 
         lat_range = [lat, lat + half_height]
-        long_range = [long, long + half_width]
+        long_range = [long, 
+                      longitude_domain(long + half_width)]
         boundary = Boundary(lat_range, long_range, time_range)
         index += 1
         south_west = CellBox(boundary, str(index))
 
         lat_range = [lat, lat + half_height]
-        long_range = [long + half_width, long + self.bounds.get_width()]
+        long_range = [longitude_domain(long + half_width), 
+                      longitude_domain(long + self.bounds.get_width())]
         boundary = Boundary(lat_range, long_range, time_range)
         index += 1
         south_east = CellBox(boundary, str(index))
 
         split_boxes = [north_west, north_east, south_west, south_east]
         return split_boxes
 
@@ -286,28 +304,38 @@
 
             Returns:
                 AggregatedCellbox: object contains the aggregated data within cellbox bounds.
         '''
         agg_dict = {}
         for source in self.get_data_source():
             loader = source.get_data_loader()
+            data_subset = source.get_data_subset()
+
             # get the aggregated value from the associated DataLoader
-            agg_value = loader.get_value(self.bounds)
+            agg_value = loader.get_value(self.bounds, data=data_subset)
             data_name = loader.data_name
             parent = self.get_parent()
             # check if the data name has many entries (ex. uC,uV)
             if ',' in data_name:
                 agg_value = self.check_vector_data(
                     source, loader, agg_value, data_name)
 
             elif np.isnan(agg_value[data_name]):
                 if source.get_value_fill_type() == 'parent':
                     # if the agg_value empty and get_value_fill_type is parent, then use the parent bounds
                     while parent is not None and np.isnan(agg_value[data_name]):
-                        agg_value = loader.get_value(parent.bounds)
+                        # Search through parent metadata to find match
+                        for parent_source in parent.get_data_source():
+                            if parent_source.get_data_loader() == source.get_data_loader():
+                                break
+                        # If no match found
+                        else:
+                            raise ValueError('Dataloader not found in parent')
+                        parent_data_subset = parent_source.get_data_subset()
+                        agg_value = loader.get_value(parent.bounds, data=parent_data_subset)
                         parent = parent.get_parent()
                 else:  # not parent, so either float or Nan so set the agg_Data to value_fill_type
                     agg_value[data_name] = source.get_value_fill_type()
                     
             # If already and value for {data_name} in cellbox and it's a NaN, overwrite
             if (data_name in agg_dict):
                 if np.isnan(agg_dict[data_name]):
@@ -328,15 +356,23 @@
         data_name_list = data_name.split(',')
         for name in data_name_list:
             parent = self.get_parent()
             if np.isnan(agg_value[name]):
                 if source.get_value_fill_type() == 'parent':
                     # if the agg_value empty and get_value_fill_type is parent, then use the parent bounds
                     while parent is not None and np.isnan(agg_value[name]):
-                        agg_value[name] = loader.get_value(parent.bounds)[name]
+                        # Search through parent metadata to find match
+                        for parent_source in parent.get_data_source():
+                            if parent_source.get_data_loader() == source.get_data_loader():
+                                break
+                        # If no match found
+                        else:
+                            raise ValueError('Dataloader not found in parent')
+                        parent_data_subset = parent_source.get_data_subset()
+                        agg_value[name] = loader.get_value(parent.bounds, data=parent_data_subset)[name]
                         parent = parent.get_parent()
                 else:  # not parent, so either float or Nan so set the agg_Data to value_fill_type
                     agg_value[data_name] = source.get_value_fill_type()
         return agg_value
 
     def deallocate_cellbox(self):
         """
```

### Comparing `meshiphi-1.1.6/meshiphi/mesh_generation/jgrid_aggregated_cellbox.py` & `meshiphi-2.0.8/meshiphi/mesh_generation/jgrid_aggregated_cellbox.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/mesh_generation/jgrid_cellbox.py` & `meshiphi-2.0.8/meshiphi/mesh_generation/jgrid_cellbox.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/mesh_generation/mesh.py` & `meshiphi-2.0.8/meshiphi/mesh_generation/mesh.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/mesh_generation/mesh_builder.py` & `meshiphi-2.0.8/meshiphi/mesh_generation/mesh_builder.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 from meshiphi.mesh_generation.environment_mesh import EnvironmentMesh
 from meshiphi.mesh_generation.metadata import Metadata
 from meshiphi.mesh_generation.neighbour_graph import NeighbourGraph
 from meshiphi.mesh_generation.mesh import Mesh
 from meshiphi.dataloaders.factory import DataLoaderFactory
 from meshiphi.config_validation.config_validator import validate_mesh_config
 
+from meshiphi.utils import longitude_distance, longitude_domain
+
 
 class MeshBuilder:
     """
 
        A class resposible for building an environment mesh based on a provided config file.
        
     """
@@ -95,32 +97,40 @@
         self.validate_bounds(bounds, cell_width, cell_height)
 
         logging.info("Initialising mesh...")
         logging.info("Initialising cellboxes...")
      
         cellboxes = []
         cellboxes = self.initialize_cellboxes(bounds, cell_width, cell_height)
-
-        grid_width = (bounds.get_long_max() -
-                      bounds.get_long_min()) / cell_width
-
-  
-
+        
+        # Account for going over the antimeridian with longitude_distance        
+        grid_width = np.divide(bounds.get_long_max() - bounds.get_long_min(),
+                               cell_width)
+        
         min_datapoints = 5
         if 'splitting' in self.config:
             min_datapoints = self.config['splitting']['minimum_datapoints']
         meta_data_list = self.initialize_meta_data(bounds, min_datapoints)
 
-        # checking to avoid any dummy cellboxes (the ones that was splitted and replaced)
-        logging.info("Assigning data sources to cellboxes...")
-        for cellbox in cellboxes:
+        # Initialise the metadata for each cellbox, including subsets of each
+        # dataloader's data set
+        logging.info("Initialising cellbox metadata...")
+        for cellbox in tqdm(cellboxes, 
+                            bar_format='{desc}{n_fmt}/{total_fmt} |{bar}| {percentage:3.0f}%, [{elapsed} elapsed] '):
+            # checking to avoid any dummy cellboxes 
+            # (the ones that were split and replaced)
             if isinstance(cellbox, CellBox):
                 cellbox.set_minimum_datapoints(min_datapoints)
+                # Update metadata with cellbox's data subset
+                updated_meta_data_list = self.initialize_meta_data_subsets(
+                                                    cellbox.bounds, 
+                                                    meta_data_list)
                 # assign meta data to each cellbox
-                cellbox.set_data_source(meta_data_list)
+                cellbox.set_data_source(updated_meta_data_list)
+
 
         
         logging.info("Initialising neighbour graph...")
         self.neighbour_graph = NeighbourGraph(cellboxes, grid_width)
         self.neighbour_graph.set_global_mesh (self.check_global_mesh(bounds, cellboxes, int(grid_width)))
 
         max_split_depth = 0
@@ -130,14 +140,29 @@
                          self.neighbour_graph, max_split_depth)
         self.mesh.set_config(config)
         if self.is_jgrid_mesh():
             logging.warning("We're using the legacy Java style cell grid")
 
 
     def initialize_meta_data(self, bounds, min_datapoints):
+        '''
+        Creates a metadata object which holds information about the data sources
+        within a cellbox. 
+
+        Args:
+            bounds (Boundary):
+                Outer boundary of the mesh being created
+                
+            min_datapoints (int):
+                Minimum number of datapoints each dataloader is allowed to 
+                aggregate 
+        Returns:
+            list(Metadata):
+                Array of metadata objects; one for each data source
+        '''
         meta_data_list = []
         splitting_conds = []
         if 'data_sources' in self.config.keys():
             for data_source in self.config['data_sources']:
                 loader_name = data_source['loader']
                 loader = DataLoaderFactory.get_dataloader(
                     loader_name, bounds, data_source['params'], min_datapoints)
@@ -154,19 +179,53 @@
                 value_fill_type = self.check_value_fill_type(data_source)
 
                 # Update list of files in config to match the ones read in by dataloader
                 if 'files' in data_source['params']:
                     data_source['params']['files'] = loader.files
 
                 meta_data_obj = Metadata(
-                    loader, updated_splitting_cond,  value_fill_type)
+                    loader, updated_splitting_cond,  value_fill_type, loader.data)
                 meta_data_list.append(meta_data_obj)
 
         return meta_data_list
         
+    def initialize_meta_data_subsets(self, bounds, meta_data_list):
+        '''
+        Updates cellbox metadata objects to include data subsets which contain
+        datapoints from only within the cellbox boundaries (as opposed to the
+        entire mesh's boundary)
+
+        Args:
+            bounds (Boundary):
+                Outer boundary of the cellbox
+                
+            meta_data_list (list(Metadata)):
+                Cellbox's metadata that needs to be updated with data subsets
+
+        Returns:
+            list(Metadata):
+                Array of metadata objects; one for each data source. Includes
+                data_subsets
+        '''
+        logging.debug(f'Initilizing data subset for {bounds}')
+        updated_meta_data_list = []
+        # For each set of data within the cellbox
+        for source in meta_data_list:
+            # Limit data within dataloader to just that within cellbox boundary
+            data_subset = source.data_loader.trim_datapoints(bounds)
+            # Update metadata object with this data subset
+            updated_meta_data_list += [Metadata(source.get_data_loader(),
+                                                source.get_splitting_conditions(),
+                                                source.get_value_fill_type(),
+                                                data_subset)]
+            
+        return updated_meta_data_list
+            
+
+
     def check_value_fill_type(self, data_source):
         def is_float(element: any) -> bool:
             if element is None: 
                     return False
             try:
                     float(element)
                     return True
@@ -184,22 +243,41 @@
         if 'j_grid' in self.config.keys():
             if  self.config['j_grid'] == "True":
                 return True
         return False
 
     def initialize_cellboxes(self, bounds, cell_width, cell_height):
         cellboxes = []
-        grid_width = (bounds.get_long_max() -
-                      bounds.get_long_min()) / cell_width
         grid_height = (bounds.get_lat_max() -
                        bounds.get_lat_min()) / cell_height
-        for lat in np.arange(bounds.get_lat_min(), bounds.get_lat_max(), cell_height):
-            for long in np.arange(bounds.get_long_min(), bounds.get_long_max(), cell_width):
+        
+        lat_range = np.arange(bounds.get_lat_min(), bounds.get_lat_max(), cell_height)
+
+
+        # Account for going over the antimeridian with longitude_distance
+        grid_width = longitude_distance(bounds.get_long_min(), 
+                                        bounds.get_long_max()) / cell_width
+        
+        if bounds.get_long_min() < bounds.get_long_max():
+            long_range = np.arange(bounds.get_long_min(),
+                                   bounds.get_long_max(), 
+                                   cell_width)
+        else:
+            long_range = np.arange(bounds.get_long_min(),
+                                   bounds.get_long_max() + 360, 
+                                   cell_width)
+        # Cast to within -180:180
+        long_range = longitude_domain(long_range)
+
+        for lat in lat_range:
+            for long in long_range:
                 cell_lat_range = [lat, lat+cell_height]
-                cell_long_range = [long, long+cell_width]
+                # If doesn't go over anti-meridian
+                if long + cell_width <= 180: cell_long_range = [long, long+cell_width]
+                else:                        cell_long_range = [long, long+cell_width-360]
                 cell_bounds = Boundary(
                     cell_lat_range, cell_long_range, bounds.get_time_range())
                 cell_id = str(len(cellboxes))
                 if self.is_jgrid_mesh():
                     cellbox_indx = len(cellboxes)
                     cellbox = JGridCellBox(cell_bounds, cell_id)
                     x_coord = cellbox_indx % grid_width
```

### Comparing `meshiphi-1.1.6/meshiphi/mesh_generation/metadata.py` & `meshiphi-2.0.8/meshiphi/mesh_generation/metadata.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,60 +13,77 @@
        splitting_conditions: list of conditions that determine how to split the data accessed by data_loader 
        value_fill_type (string): indicates how to fill a CellBox if it has void data
          (ex. use the data in the parent cellbox or assign 0 to the data)
 
     """
    
 
-    def __init__(self, data_loader , spliiting_conditions =None, value_fill_type= ""):
+    def __init__(self, data_loader , splitting_conditions =None, value_fill_type= "", data_subset=None):
         """
 
             Args:
                data_loader (DataLoader): object of the DataLoader class that enables projecting to the cellbox data
                splitting_conditions (List<dict>): list of conditions that determine how to split CellBox
                value_fill_tyep (string): represents the way the data of a cellbox will be filled
                  in case it has void data (ex. parent , 0 )
                 
         """ 
         self.data_loader = data_loader
-        self.splitting_conditions = spliiting_conditions
+        self.splitting_conditions = splitting_conditions
         self.value_fill_type = value_fill_type
+        self.data_name = data_loader.data_name
+        if data_subset is None:
+            if ',' in data_loader.data_name:
+                self.data_subset = data_loader.data[data_loader.data_name.split(',')]
+            else:
+                self.data_subset = data_loader.data[data_loader.data_name]
+        else:
+            self.data_subset = data_subset
   
     def get_data_loader(self): 
         """
         returns the data loader
         """
         return self.data_loader
 
+    def set_data_loader(self , data_loader): 
+        """
+        sets the data loader
+        """
+        self.data_loader = data_loader
+
     def get_splitting_conditions(self):
         """
         returns a list of the splitting conditions
         """
         
         return self.splitting_conditions
 
-    def set_data_loader(self , data_loader): 
-        """
-        sets the data loader
-        """
-        self.data_loader = data_loader
- 
-
     def set_splitting_conditions(self ,  splitting_conditions):
         """
         sets the splitting conditions
         """
         self.splitting_conditions = splitting_conditions
 
+    def get_value_fill_type(self ):
+        """
+        returns thevalue fill type
+        """
+        return self.value_fill_type   
+
     def set_value_fill_type(self , value_fill_type): 
         """
         sets the value fill type
         """
         self.value_fill_type = value_fill_type
 
-    def get_value_fill_type(self ):
+    def get_data_subset(self):
         """
-        returns thevalue fill type
+        gets the data subset
         """
-        return self.value_fill_type   
-  
-
+        return self.data_subset
+    
+    def set_data_subset(self, data_subset):
+        """
+        sets the data subset
+        """
+        self.data_subset = data_subset
```

### Comparing `meshiphi-1.1.6/meshiphi/mesh_generation/neighbour_graph.py` & `meshiphi-2.0.8/meshiphi/mesh_generation/neighbour_graph.py`

 * *Files 17% similar despite different names*

```diff
@@ -50,14 +50,35 @@
         neighbour_graph = {}
         for key in ng_json:
             neighbour_graph[key] = ng_json[key]
         obj = NeighbourGraph()
         obj.neighbour_graph = neighbour_graph
         return obj
 
+    def increment_ids(self, inc):
+        """
+        Increments all ID's within the neighbour_graph by a given int inc
+
+            Args: 
+                inc (int): The number to increment all ID's in the neighbour_graph by
+        """
+
+        ng = self.get_graph()
+        new_ng = {}
+
+        for node in ng:
+            for direction in ng[node]:
+                inc_neighbours = [x + inc for x in ng[node][direction]]
+                ng[node][direction] = inc_neighbours
+
+            new_ng[str( int(node) + inc)] = ng[node]
+
+        self.neighbour_graph = new_ng
+
+
     def get_graph(self):
         """
         returns the graph dict
         """
         return self.neighbour_graph
 
     def update_neighbour(self, index, direction, neighbours):
@@ -111,15 +132,16 @@
             Args: 
             cellbox_index (int): the index of the cellbox that will get removed from the neoghbpur_graph
         '''
         self.neighbour_graph.pop(cellbox_index)
 
     def update_neighbours(self, cellbox_indx, new_neighbours_indx, direction, cellboxes):
         '''
-            method that updates the neighbour of a certain cellbox in a specific direction. It removes cellbox_indx from the neighbour_map of its neighbours in a specific direction and add new_neighbour_indx
+            method that updates the neighbour of a certain cellbox in a specific direction. 
+            It removes cellbox_indx from the neighbour_map of its neighbours in a specific direction and add new_neighbour_indx
 
             Args: 
                 cellbox_index (int): index of the cellbox that its neighbour will be updated
                 new_neighbour_indx (int): the index of the new neighbour that will replace cellbox_index
                 direction (int): an int that represents the direction of the neighbours that will get updated (e.g. north, south ,..)
                 cellboxes(list<CellBox>): the list that contains all the cellboxes of the mesh
 
@@ -156,15 +178,15 @@
             neighbour_indx_list = self.neighbour_graph[cellbox_indx][str(direction)]
 
         for indx in neighbour_indx_list:
             try:
                 self.neighbour_graph[indx][-1*direction].remove(cellbox_indx)
             except KeyError:
                 self.neighbour_graph[str(indx)][str(-1*direction)].remove(int(cellbox_indx))
-
+                
     def update_corner_neighbours(self, cellbox_indx, north_west_indx, north_east_indx, south_west_indx, south_east_indx):
         '''
             method that updates the corner neighbours of cellbox_indx with the given indeces
         '''
         north_east_corner_indx = self.neighbour_graph[cellbox_indx][Direction.north_east]
         if len(north_east_corner_indx) > 0:
             self.neighbour_graph[north_east_corner_indx[0]][Direction.south_west] = [north_east_indx]
@@ -177,14 +199,80 @@
         if len(south_east_corner_indx) > 0:
             self.neighbour_graph[south_east_corner_indx[0]][Direction.north_west] = [south_east_indx]
 
         south_west_corner_indx = self.neighbour_graph[cellbox_indx][Direction.south_west]
         if len(south_west_corner_indx) > 0:
             self.neighbour_graph[south_west_corner_indx[0]][Direction.north_east] = [south_west_indx]
     
+    def get_neighbour_case_bounds(self, bounds_a, bounds_b):
+        """
+            Given two bounds (bounds_a, bounds_b) returns a case number
+            representing where the two bounds are touching.
+
+            Args:
+                bounds_a (Bounds): starting Bounds
+                bounds_b (Bounds): destination Bounds
+
+            Returns:
+                int: an int representing the direction of the adjacency between input bounds_a and bounds_b. The meaning of each case is as follows -
+
+                        case 0 -> Bounds are not neighbours
+
+                        case 1 -> bounds_b is the North-East corner of bounds_a\n
+                        case 2 -> bounds_b is East of bounds_a\n
+                        case 3 -> bounds_b is the South-East corner of bounds_a\n
+                        case 4 -> bounds_b is South of bounds_a\n
+                        case -1 -> bounds_b is the South-West corner of bounds_a\n
+                        case -2 -> bounds_b is West of bounds_a\n
+                        case -3 -> bounds_b is the North-West corner of bounds_a\n
+                        case -4 -> bounds_b is North of bounds_a\n
+        """
+        long_a = bounds_a.get_long_min()
+        lat_a = bounds_a.get_lat_min()
+        long_b = bounds_b.get_long_min()
+        lat_b = bounds_b.get_lat_min()
+
+        if (long_a + bounds_a.get_width()) == long_b and (
+                lat_a + bounds_a.get_height()) == lat_b:
+            return Direction.north_east
+
+        if (long_a + bounds_a.get_width() == long_b) and (
+                lat_b < (lat_a + bounds_a.get_height())) and (
+                (lat_b + bounds_b.get_height()) > lat_a):
+            return Direction.east
+
+        if (long_a + bounds_a.get_width()) == long_b and (
+                lat_a == lat_b + bounds_b.get_height()):
+            return Direction.south_east
+
+        if ((lat_b + bounds_b.get_height()) == lat_a) and (
+                (long_b + bounds_b.get_width()) > long_a) and (
+                long_b < (long_a + bounds_a.get_width())):
+            return Direction.south
+
+        if long_a == (long_b + bounds_b.get_width()) and lat_a == (
+                lat_b + bounds_b.get_height()):
+            return Direction.south_west
+
+        if (long_b + bounds_b.get_width() == long_a) and (
+                lat_b < (lat_a + bounds_a.get_height())) and (
+                (lat_b + bounds_b.get_height()) > lat_a):
+            return Direction.west
+
+        if long_a == (long_b + bounds_b.get_width()) and (
+                lat_a + bounds_a.get_height() == lat_b):
+            return Direction.north_west
+
+        if (lat_b == (lat_a + bounds_a.get_height())) and (
+                (long_b + bounds_b.get_width()) > long_a) and (
+                long_b < (long_a + bounds_a.get_width())):
+            return Direction.north
+
+        return 0  # Cells are not neighbours.
+
     def get_neighbour_case(self, cellbox_a, cellbox_b):
         """
             Given two cellboxes (cellbox_a, cellbox_b) returns a case number
             representing where the two cellboxes are touching.
 
             Args:
                 cellbox_a (CellBox): starting CellBox
@@ -205,14 +293,15 @@
                         case -4 -> cellbox_b is North of cellbox_a\n
         """
    
         long_a = cellbox_a.get_bounds().get_long_min()
         lat_a = cellbox_a.get_bounds().get_lat_min()
         long_b = cellbox_b.get_bounds().get_long_min()
         lat_b = cellbox_b.get_bounds().get_lat_min()
+
         def on_global_bound(cellbox_a , cellbox_b):
             """
             Given two cellboxes (cellbox_a, cellbox_b) returns a boolean
             representing whether the two cellboxes are touching on the global bound (-180,180).
 
             Args:
                 cellbox_a (CellBox): starting CellBox
@@ -220,38 +309,46 @@
 
             Returns:
                 bool: a boolean representing if the two cellboxes are touching on the global bound (-180,180).            
             """
             return long_a == -180  and cellbox_b.get_bounds().get_long_max() == 180 or long_b == -180 and cellbox_a.get_bounds().get_long_max() == 180 
         if self.is_global_mesh() and on_global_bound (cellbox_a , cellbox_b) :
             return self.get_global_mesh_neighbour_case(cellbox_a, cellbox_b)
+        
         if (long_a + cellbox_a.get_bounds().get_width()) == long_b and (
                 lat_a + cellbox_a.get_bounds().get_height()) == lat_b:
             return Direction.north_east
+
         if (long_a + cellbox_a.get_bounds().get_width() == long_b) and (
                 lat_b < (lat_a + cellbox_a.get_bounds().get_height())) and (
                 (lat_b + cellbox_b.get_bounds().get_height()) > lat_a):
             return Direction.east
+
         if (long_a + cellbox_a.get_bounds().get_width()) == long_b and (
                 lat_a == lat_b + cellbox_b.get_bounds().get_height()):
             return Direction.south_east
+
         if ((lat_b + cellbox_b.get_bounds().get_height()) == lat_a) and (
                 (long_b + cellbox_b.get_bounds().get_width()) > long_a) and (
                 long_b < (long_a + cellbox_a.get_bounds().get_width())):
             return Direction.south
+
         if long_a == (long_b + cellbox_b.get_bounds().get_width()) and lat_a == (
                 lat_b + cellbox_b.get_bounds().get_height()):
             return Direction.south_west
+
         if (long_b + cellbox_b.get_bounds().get_width() == long_a) and (
                 lat_b < (lat_a + cellbox_a.get_bounds().get_height())) and (
                 (lat_b + cellbox_b.get_bounds().get_height()) > lat_a):
             return Direction.west
+
         if long_a == (long_b + cellbox_b.get_bounds().get_width()) and (
                 lat_a + cellbox_a.get_bounds().get_height() == lat_b):
             return Direction.north_west
+
         if (lat_b == (lat_a + cellbox_a.get_bounds().get_height())) and (
                 (long_b + cellbox_b.get_bounds().get_width()) > long_a) and (
                 long_b < (long_a + cellbox_a.get_bounds().get_width())):
             return Direction.north
         return 0  # Cells are not neighbours.
     
     def get_global_mesh_neighbour_case(self, cellbox_a, cellbox_b):
```

### Comparing `meshiphi-1.1.6/meshiphi/mesh_plotting/mesh_plotter.py` & `meshiphi-2.0.8/meshiphi/mesh_plotting/mesh_plotter.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/mesh_validation/mesh_validator.py` & `meshiphi-2.0.8/meshiphi/mesh_validation/mesh_validator.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/mesh_validation/sampler.py` & `meshiphi-2.0.8/meshiphi/mesh_validation/sampler.py`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/meshiphi/utils.py` & `meshiphi-2.0.8/meshiphi/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,43 @@
 import numpy as np
 
 from datetime import datetime, timedelta
 from functools import wraps
 from calendar import monthrange
 from scipy.fftpack import fftshift
 
-    
+def longitude_domain(long):
+    """
+    Converts any longitude degree value into one between -180:180
+    """
+    # Allow input type to be list or ndarray
+    if isinstance(long, list):
+        return [longitude_domain(x) for x in long]
+    elif isinstance(long, np.ndarray):
+        return np.array([longitude_domain(x) for x in long])
+    # Return same format as input at antimeridian
+    elif long in [-180, 180]:
+        return long
+    # Otherwise convert it to be within domain
+    else:    
+        return (long + 180) % 360 - 180
+
+def longitude_distance(long_a, long_b):
+    """
+    Calculates the angular distance between two longitude values
+    """
+
+    long_dist = np.abs(longitude_domain(long_b) - longitude_domain(long_a))
+    long_dist = np.mod(long_dist, 360)
+
+    if long_dist > 180:
+        return 360 - long_dist
+    else:
+        return long_dist
+
 def frac_of_month(year, month, start_date=None, end_date=None):
     
     # Determine the number of days in the month specified
     days_in_month = monthrange(year, month)[1]
     # If not specified, default to beginning/end of month
     if start_date is None:
         start_date = str_to_datetime(f'{year}-{month}-01')
```

### Comparing `meshiphi-1.1.6/meshiphi.egg-info/PKG-INFO` & `meshiphi-2.0.8/meshiphi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 Metadata-Version: 2.1
 Name: meshiphi
-Version: 1.1.6
-Summary: meshiphi: Earth's digital twin mapped on a non-uniform mesh
+Version: 2.0.8
+Summary: MeshiPhi: Earth's digital twin mapped on a non-uniform mesh
 Home-page: https://www.github.com/antarctica
-Author: Samuel Hall, George Coombs, Harrison Abbot, Ayat Fekry, Jonathan Smith, Maria Fox, James Byrne, Michael Thorne
-Author-email: polarroute@bas.ac.uk
-Maintainer: Samuel Hall, George Coombs, Harrison Abbot, Ayat Fekry, Jonathan Smith, Maria Fox, James Byrne, Michael Thorne
-Maintainer-email: polarroute@bas.ac.uk
+Author: Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey
+Author-email: amop@bas.ac.uk
+Maintainer: Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey
+Maintainer-email: amop@bas.ac.uk
 License: MIT
-Classifier: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
-Classifier: 
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dask
 Requires-Dist: geopandas
 Requires-Dist: jsonschema
 Requires-Dist: matplotlib
 Requires-Dist: netcdf4
-Requires-Dist: cfgrib
-Requires-Dist: numpy<=1.24.1,>=1.21.6
-Requires-Dist: pandas<=1.4.4,>=1.3.5
+Requires-Dist: numpy>=1.21.6
+Requires-Dist: pandas>=1.3.5
 Requires-Dist: pytest
 Requires-Dist: rioxarray
 Requires-Dist: shapely>=2.0.1
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Requires-Dist: xarray
```

#### html2text {}

```diff
@@ -1,32 +1,30 @@
-Metadata-Version: 2.1 Name: meshiphi Version: 1.1.6 Summary: meshiphi: Earth's
+Metadata-Version: 2.1 Name: meshiphi Version: 2.0.8 Summary: MeshiPhi: Earth's
 digital twin mapped on a non-uniform mesh Home-page: https://www.github.com/
-antarctica Author: Samuel Hall, George Coombs, Harrison Abbot, Ayat Fekry,
-Jonathan Smith, Maria Fox, James Byrne, Michael Thorne Author-email:
-polarroute@bas.ac.uk Maintainer: Samuel Hall, George Coombs, Harrison Abbot,
-Ayat Fekry, Jonathan Smith, Maria Fox, James Byrne, Michael Thorne Maintainer-
-email: polarroute@bas.ac.uk License: MIT Classifier: Classifier: Development
-Status :: 3 - Alpha Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: System Administrators Classifier: License ::
-OSI Approved :: MIT License Classifier: Natural Language :: English Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Topic :: Scientific/Engineering
-Classifier: Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: dask Requires-Dist: geopandas Requires-Dist: jsonschema
-Requires-Dist: matplotlib Requires-Dist: netcdf4 Requires-Dist: cfgrib
-Requires-Dist: numpy<=1.24.1,>=1.21.6 Requires-Dist: pandas<=1.4.4,>=1.3.5
-Requires-Dist: pytest Requires-Dist: rioxarray Requires-Dist: shapely>=2.0.1
-Requires-Dist: scikit-learn Requires-Dist: scipy Requires-Dist: tqdm Requires-
-Dist: xarray Requires-Dist: cartopy Requires-Dist: rasterio Provides-Extra:
-tests Requires-Dist: pytest; extra == "tests" # MeshiÏ (MeshiPhi) ![]
-(logo.jpg) _[_M_a_n_u_a_l_ _P_a_g_e_]_[_P_y_P_i_]_[_R_e_l_e_a_s_e_ _T_a_g_]_[_I_s_s_u_e_s_]_[_L_i_c_e_n_s_e_]Introducing
-MeshiÏ, a versatile software package designed for comprehensive earth modeling
-and navigation planning. MeshiÏ works by discretizing the Earth's surface into
-a non-uniform grid, allocating higher resolution in regions of geographic
+antarctica Author: Autonomous Marine Operations Planning (AMOP) Team, AI Lab,
+British Antarctic Survey Author-email: amop@bas.ac.uk Maintainer: Autonomous
+Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey
+Maintainer-email: amop@bas.ac.uk License: MIT Classifier: Development Status ::
+3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
+Intended Audience :: System Administrators Classifier: License :: OSI Approved
+:: MIT License Classifier: Natural Language :: English Classifier: Operating
+System :: OS Independent Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.7 Classifier: Topic :: Scientific/Engineering Description-Content-Type:
+text/markdown License-File: LICENSE Requires-Dist: dask Requires-Dist:
+geopandas Requires-Dist: jsonschema Requires-Dist: matplotlib Requires-Dist:
+netcdf4 Requires-Dist: numpy>=1.21.6 Requires-Dist: pandas>=1.3.5 Requires-
+Dist: pytest Requires-Dist: rioxarray Requires-Dist: shapely>=2.0.1 Requires-
+Dist: scikit-learn Requires-Dist: scipy Requires-Dist: tqdm Requires-Dist:
+xarray Requires-Dist: cartopy Requires-Dist: rasterio Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests" # MeshiÏ (MeshiPhi) ![](logo.jpg)
+_[_M_a_n_u_a_l_ _P_a_g_e_]_[_P_y_P_i_]_[_R_e_l_e_a_s_e_ _T_a_g_]_[_I_s_s_u_e_s_]_[_L_i_c_e_n_s_e_]Introducing MeshiÏ, a
+versatile software package designed for comprehensive earth modeling and
+navigation planning. MeshiÏ works by discretizing the Earth's surface into a
+non-uniform grid, allocating higher resolution in regions of geographic
 diversity, and conserving lower resolution in more uniform regions. The
 software also incorporates data-driven vehicle models, with the ability to
 calculate speed limits and fuel needs for specific vessels within each grid
 cell. These mesh objects can be output in standard formats, such as GeoJSON and
 GeoTIFF, enabling data-visualisation via GIS software such as ArcGIS. ##
 Installation MeshiÏ can be installed via pip or by cloning the repository from
 GitHub. Pip: ``` pip install meshiphi ``` Github: (for local development) ```
```

### Comparing `meshiphi-1.1.6/meshiphi.egg-info/SOURCES.txt` & `meshiphi-2.0.8/meshiphi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meshiphi-1.1.6/setup.py` & `meshiphi-2.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,26 +21,24 @@
     author=meshiphi.__author__,
     author_email=meshiphi.__email__,
     maintainer=meshiphi.__author__,
     maintainer_email=meshiphi.__email__,
     url="https://www.github.com/antarctica",
     project_urls={
     },
-    classifiers=[el.lstrip() for el in """
-        Development Status :: 3 - Alpha
+    classifiers=[el.lstrip() for el in """Development Status :: 3 - Alpha
         Intended Audience :: Science/Research
         Intended Audience :: System Administrators
         License :: OSI Approved :: MIT License
         Natural Language :: English
         Operating System :: OS Independent
         Programming Language :: Python
         Programming Language :: Python :: 3
         Programming Language :: Python :: 3.7
-        Topic :: Scientific/Engineering
-    """.split('\n')],
+        Topic :: Scientific/Engineering""".split('\n')],
     entry_points={
         'console_scripts': [
             "create_mesh=meshiphi.cli:create_mesh_cli",
             "export_mesh=meshiphi.cli:export_mesh_cli",
             "rebuild_mesh=meshiphi.cli:rebuild_mesh_cli"],
     },
     keywords=[],
```


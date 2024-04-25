# Comparing `tmp/orix-0.9.0.post0.tar.gz` & `tmp/orix-0.9.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orix-0.9.0.post0.tar", last modified: Wed May 18 12:48:54 2022, max compression
+gzip compressed data, was "orix-0.9.0rc2.tar", last modified: Wed May 11 13:28:03 2022, max compression
```

## Comparing `orix-0.9.0.post0.tar` & `orix-0.9.0rc2.tar`

### file list

```diff
@@ -1,171 +1,170 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:54.474393 orix-0.9.0.post0/
--rw-r--r--   0 runner    (1001) docker     (121)    11808 2022-05-18 12:48:39.000000 orix-0.9.0.post0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12822 2022-05-18 12:48:39.000000 orix-0.9.0.post0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)    34494 2022-05-18 12:48:39.000000 orix-0.9.0.post0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-05-18 12:48:39.000000 orix-0.9.0.post0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3376 2022-05-18 12:48:54.474393 orix-0.9.0.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2743 2022-05-18 12:48:39.000000 orix-0.9.0.post0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1881 2022-05-18 12:48:39.000000 orix-0.9.0.post0/RELEASE.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:54.458393 orix-0.9.0.post0/doc/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:54.450394 orix-0.9.0.post0/doc/_static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:54.462393 orix-0.9.0.post0/doc/_static/img/
--rw-r--r--   0 runner    (1001) docker     (121)    18674 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/_static/img/inversion.png
--rw-r--r--   0 runner    (1001) docker     (121)     8955 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/_static/img/inversion.svg
--rw-r--r--   0 runner    (1001) docker     (121)   123767 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/_static/img/orientation-region-Oq.png
--rw-r--r--   0 runner    (1001) docker     (121)    61766 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/_static/img/orientation.png
--rw-r--r--   0 runner    (1001) docker     (121)   109074 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/_static/img/orientation.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7809 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/_static/img/orix_logo.png
--rw-r--r--   0 runner    (1001) docker     (121)   115208 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/_static/img/rotation.png
--rw-r--r--   0 runner    (1001) docker     (121)    15316 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/_static/img/rotation.svg
--rw-r--r--   0 runner    (1001) docker     (121)   534148 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/_static/img/spherical-region-D3.png
--rw-r--r--   0 runner    (1001) docker     (121)    21445 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/_static/img/triad-object.png
--rw-r--r--   0 runner    (1001) docker     (121)     4528 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/bibliography.bib
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/bibliography.rst
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7605 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/clustering_across_fundamental_region_boundaries.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    14926 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/clustering_misorientations.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      431 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/clustering_of_orientations.rst
--rw-r--r--   0 runner    (1001) docker     (121)   972665 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/clustering_orientations.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     6481 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)    28745 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/crystal_directions.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/crystal_geometry.rst
--rw-r--r--   0 runner    (1001) docker     (121)    41352 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/crystal_map.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    11565 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/crystal_reference_frame.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/crystallographic_maps.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1589 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1643 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7894 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/inverse_pole_figures.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/orientations.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4351 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/point_groups.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    10684 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/reference.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1546 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/related_projects.rst
--rw-r--r--   0 runner    (1001) docker     (121)    21994 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/stereographic_projection.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    10199 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/uniform_sampling_of_orientation_space.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-05-18 12:48:39.000000 orix-0.9.0.post0/doc/vectors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-05-18 12:48:39.000000 orix-0.9.0.post0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2154 2022-05-18 12:48:39.000000 orix-0.9.0.post0/getting_started.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:54.462393 orix-0.9.0.post0/orix/
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5567 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:54.462393 orix-0.9.0.post0/orix/base/
--rw-r--r--   0 runner    (1001) docker     (121)     8785 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:54.462393 orix-0.9.0.post0/orix/crystal_map/
--rw-r--r--   0 runner    (1001) docker     (121)     1337 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/crystal_map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    37942 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/crystal_map/crystal_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     3319 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/crystal_map/crystal_map_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)    31552 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/crystal_map/phase_list.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:54.462393 orix-0.9.0.post0/orix/data/
--rw-r--r--   0 runner    (1001) docker     (121)     6855 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/data/_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:54.462393 orix-0.9.0.post0/orix/io/
--rw-r--r--   0 runner    (1001) docker     (121)     6772 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:54.462393 orix-0.9.0.post0/orix/io/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      864 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/io/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4551 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/io/plugins/_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (121)    23061 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/io/plugins/ang.py
--rw-r--r--   0 runner    (1001) docker     (121)    10463 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/io/plugins/bruker_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (121)     7340 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/io/plugins/emsoft_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (121)    14158 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/io/plugins/orix_hdf5.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:54.466393 orix-0.9.0.post0/orix/plot/
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2762 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/plot/_symmetry_marker.py
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/plot/_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    18395 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/plot/crystal_map_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:54.466393 orix-0.9.0.post0/orix/plot/direction_color_keys/
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/plot/direction_color_keys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7346 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/plot/direction_color_keys/_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     1327 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/plot/direction_color_keys/direction_color_key.py
--rw-r--r--   0 runner    (1001) docker     (121)     4588 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/plot/direction_color_keys/direction_color_key_tsl.py
--rw-r--r--   0 runner    (1001) docker     (121)    12717 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/plot/inverse_pole_figure_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:54.466393 orix-0.9.0.post0/orix/plot/orientation_color_keys/
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/plot/orientation_color_keys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4603 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/plot/orientation_color_keys/euler_color_key.py
--rw-r--r--   0 runner    (1001) docker     (121)     1749 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/plot/orientation_color_keys/ipf_color_key.py
--rw-r--r--   0 runner    (1001) docker     (121)     3023 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/plot/orientation_color_keys/ipf_color_key_tsl.py
--rw-r--r--   0 runner    (1001) docker     (121)     6594 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/plot/rotation_plot.py
--rw-r--r--   0 runner    (1001) docker     (121)    27998 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/plot/stereographic_plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     7024 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/plot/unit_cell_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:54.466393 orix-0.9.0.post0/orix/projections/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/projections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10841 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/projections/stereographic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:54.466393 orix-0.9.0.post0/orix/quaternion/
--rw-r--r--   0 runner    (1001) docker     (121)     1855 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/quaternion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16224 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/quaternion/_conversions.py
--rw-r--r--   0 runner    (1001) docker     (121)    36368 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/quaternion/orientation.py
--rw-r--r--   0 runner    (1001) docker     (121)     7327 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/quaternion/orientation_region.py
--rw-r--r--   0 runner    (1001) docker     (121)    13369 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/quaternion/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (121)    23823 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/quaternion/rotation.py
--rw-r--r--   0 runner    (1001) docker     (121)    30239 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/quaternion/symmetry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:54.466393 orix-0.9.0.post0/orix/sampling/
--rw-r--r--   0 runner    (1001) docker     (121)     4426 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/sampling/S2_sampling.py
--rw-r--r--   0 runner    (1001) docker     (121)     7005 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/sampling/SO3_sampling.py
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4243 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/sampling/_cubochoric_sampling.py
--rw-r--r--   0 runner    (1001) docker     (121)     4715 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/sampling/sample_generators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:54.470393 orix-0.9.0.post0/orix/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23852 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:54.470393 orix-0.9.0.post0/orix/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2311 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/data/test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:54.470393 orix-0.9.0.post0/orix/tests/io/
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25671 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/io/test_ang.py
--rw-r--r--   0 runner    (1001) docker     (121)     4790 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/io/test_bruker_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (121)     4183 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/io/test_emsoft_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1392 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/io/test_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (121)     5932 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/io/test_io.py
--rw-r--r--   0 runner    (1001) docker     (121)    10144 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/io/test_orix_hdf5.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:54.474393 orix-0.9.0.post0/orix/tests/plot/
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15366 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/plot/test_crystal_map_plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     1464 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/plot/test_direction_color_keys.py
--rw-r--r--   0 runner    (1001) docker     (121)     4524 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/plot/test_inverse_pole_figure_plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     5287 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/plot/test_orientation_color_keys.py
--rw-r--r--   0 runner    (1001) docker     (121)     4131 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/plot/test_rotation_plot.py
--rw-r--r--   0 runner    (1001) docker     (121)    16266 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/plot/test_stereographic_plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     5279 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/plot/test_unit_cell_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:54.474393 orix-0.9.0.post0/orix/tests/quaternion/
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/quaternion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6712 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/quaternion/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (121)    26074 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/quaternion/test_orientation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4617 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/quaternion/test_orientation_region.py
--rw-r--r--   0 runner    (1001) docker     (121)     9743 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/quaternion/test_quaternion.py
--rw-r--r--   0 runner    (1001) docker     (121)    21660 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/quaternion/test_rotation.py
--rw-r--r--   0 runner    (1001) docker     (121)    32685 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/quaternion/test_symmetry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:54.474393 orix-0.9.0.post0/orix/tests/sampling/
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4346 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/sampling/test_cubochoric_sampling.py
--rw-r--r--   0 runner    (1001) docker     (121)     2399 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/sampling/test_s2_sampling.py
--rw-r--r--   0 runner    (1001) docker     (121)     4527 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/sampling/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (121)     2291 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/test_axangle.py
--rw-r--r--   0 runner    (1001) docker     (121)    37004 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/test_crystal_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     4042 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/test_crystal_map_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     2002 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/test_fundamental_sector.py
--rw-r--r--   0 runner    (1001) docker     (121)    86877 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/test_miller.py
--rw-r--r--   0 runner    (1001) docker     (121)     1907 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/test_neoeuler.py
--rw-r--r--   0 runner    (1001) docker     (121)     5756 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/test_object3d.py
--rw-r--r--   0 runner    (1001) docker     (121)    26968 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/test_phase_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1838 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/test_spherical_region.py
--rw-r--r--   0 runner    (1001) docker     (121)     4898 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/test_stereographic_projection.py
--rw-r--r--   0 runner    (1001) docker     (121)     4927 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    21110 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/tests/test_vector3d.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:54.474393 orix-0.9.0.post0/orix/vector/
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5753 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/vector/fundamental_sector.py
--rw-r--r--   0 runner    (1001) docker     (121)    33226 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/vector/miller.py
--rw-r--r--   0 runner    (1001) docker     (121)     4162 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/vector/neo_euler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1967 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/vector/spherical_region.py
--rw-r--r--   0 runner    (1001) docker     (121)    33825 2022-05-18 12:48:39.000000 orix-0.9.0.post0/orix/vector/vector3d.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 12:48:54.462393 orix-0.9.0.post0/orix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3376 2022-05-18 12:48:53.000000 orix-0.9.0.post0/orix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4398 2022-05-18 12:48:54.000000 orix-0.9.0.post0/orix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-18 12:48:53.000000 orix-0.9.0.post0/orix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      547 2022-05-18 12:48:54.000000 orix-0.9.0.post0/orix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-05-18 12:48:54.000000 orix-0.9.0.post0/orix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-05-18 12:48:39.000000 orix-0.9.0.post0/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-05-18 12:48:54.474393 orix-0.9.0.post0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2775 2022-05-18 12:48:39.000000 orix-0.9.0.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 13:28:03.596073 orix-0.9.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (121)    11703 2022-05-11 13:27:50.000000 orix-0.9.0rc2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    12486 2022-05-11 13:27:50.000000 orix-0.9.0rc2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    34494 2022-05-11 13:27:50.000000 orix-0.9.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      317 2022-05-11 13:27:50.000000 orix-0.9.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3373 2022-05-11 13:28:03.596073 orix-0.9.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2743 2022-05-11 13:27:50.000000 orix-0.9.0rc2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1540 2022-05-11 13:27:50.000000 orix-0.9.0rc2/RELEASE.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 13:28:03.584073 orix-0.9.0rc2/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 13:28:03.580073 orix-0.9.0rc2/doc/_static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 13:28:03.584073 orix-0.9.0rc2/doc/_static/img/
+-rw-r--r--   0 runner    (1001) docker     (121)    18674 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/_static/img/inversion.png
+-rw-r--r--   0 runner    (1001) docker     (121)     8955 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/_static/img/inversion.svg
+-rw-r--r--   0 runner    (1001) docker     (121)   123767 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/_static/img/orientation-region-Oq.png
+-rw-r--r--   0 runner    (1001) docker     (121)    61766 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/_static/img/orientation.png
+-rw-r--r--   0 runner    (1001) docker     (121)   109074 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/_static/img/orientation.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     7809 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/_static/img/orix_logo.png
+-rw-r--r--   0 runner    (1001) docker     (121)   115208 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/_static/img/rotation.png
+-rw-r--r--   0 runner    (1001) docker     (121)    15316 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/_static/img/rotation.svg
+-rw-r--r--   0 runner    (1001) docker     (121)   534148 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/_static/img/spherical-region-D3.png
+-rw-r--r--   0 runner    (1001) docker     (121)    21445 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/_static/img/triad-object.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4528 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/bibliography.bib
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/bibliography.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     7605 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/clustering_across_fundamental_region_boundaries.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    14881 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/clustering_misorientations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)      431 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/clustering_of_orientations.rst
+-rw-r--r--   0 runner    (1001) docker     (121)   972665 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/clustering_orientations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     6363 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    28745 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/crystal_directions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/crystal_geometry.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    41352 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/crystal_map.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    11565 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/crystal_reference_frame.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/crystallographic_maps.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1589 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1643 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     7894 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/inverse_pole_figures.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)      795 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/orientations.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4351 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/point_groups.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    10684 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1546 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/related_projects.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    21994 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/stereographic_projection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    10199 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/uniform_sampling_of_orientation_space.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-05-11 13:27:50.000000 orix-0.9.0rc2/doc/vectors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2154 2022-05-11 13:27:50.000000 orix-0.9.0rc2/getting_started.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 13:28:03.584073 orix-0.9.0rc2/orix/
+-rw-r--r--   0 runner    (1001) docker     (121)      471 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5567 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 13:28:03.588074 orix-0.9.0rc2/orix/base/
+-rw-r--r--   0 runner    (1001) docker     (121)     8785 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 13:28:03.588074 orix-0.9.0rc2/orix/crystal_map/
+-rw-r--r--   0 runner    (1001) docker     (121)     1337 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/crystal_map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37942 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/crystal_map/crystal_map.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3319 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/crystal_map/crystal_map_properties.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31552 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/crystal_map/phase_list.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 13:28:03.588074 orix-0.9.0rc2/orix/data/
+-rw-r--r--   0 runner    (1001) docker     (121)     6855 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/data/_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 13:28:03.588074 orix-0.9.0rc2/orix/io/
+-rw-r--r--   0 runner    (1001) docker     (121)     6772 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 13:28:03.588074 orix-0.9.0rc2/orix/io/plugins/
+-rw-r--r--   0 runner    (1001) docker     (121)      864 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/io/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4551 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/io/plugins/_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23061 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/io/plugins/ang.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10463 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/io/plugins/bruker_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7340 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/io/plugins/emsoft_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14158 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/io/plugins/orix_hdf5.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 13:28:03.588074 orix-0.9.0rc2/orix/plot/
+-rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2762 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/plot/_symmetry_marker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/plot/_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18395 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/plot/crystal_map_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 13:28:03.588074 orix-0.9.0rc2/orix/plot/direction_color_keys/
+-rw-r--r--   0 runner    (1001) docker     (121)      980 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/plot/direction_color_keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7346 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/plot/direction_color_keys/_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1327 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/plot/direction_color_keys/direction_color_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4588 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/plot/direction_color_keys/direction_color_key_tsl.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12717 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/plot/inverse_pole_figure_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 13:28:03.588074 orix-0.9.0rc2/orix/plot/orientation_color_keys/
+-rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/plot/orientation_color_keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4603 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/plot/orientation_color_keys/euler_color_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1749 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/plot/orientation_color_keys/ipf_color_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3023 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/plot/orientation_color_keys/ipf_color_key_tsl.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6594 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/plot/rotation_plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27998 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/plot/stereographic_plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7024 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/plot/unit_cell_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 13:28:03.588074 orix-0.9.0rc2/orix/projections/
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/projections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10841 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/projections/stereographic.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 13:28:03.592074 orix-0.9.0rc2/orix/quaternion/
+-rw-r--r--   0 runner    (1001) docker     (121)     1855 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/quaternion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16224 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/quaternion/_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36226 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/quaternion/orientation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7327 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/quaternion/orientation_region.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13369 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/quaternion/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23823 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/quaternion/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30239 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/quaternion/symmetry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 13:28:03.592074 orix-0.9.0rc2/orix/sampling/
+-rw-r--r--   0 runner    (1001) docker     (121)     4426 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/sampling/S2_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7005 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/sampling/SO3_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4243 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/sampling/_cubochoric_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4715 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/sampling/sample_generators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 13:28:03.592074 orix-0.9.0rc2/orix/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23852 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 13:28:03.592074 orix-0.9.0rc2/orix/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      709 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2311 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/data/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 13:28:03.592074 orix-0.9.0rc2/orix/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (121)      709 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25671 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/io/test_ang.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4790 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/io/test_bruker_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4183 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/io/test_emsoft_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1392 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/io/test_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5932 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/io/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10144 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/io/test_orix_hdf5.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 13:28:03.592074 orix-0.9.0rc2/orix/tests/plot/
+-rw-r--r--   0 runner    (1001) docker     (121)      709 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15366 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/plot/test_crystal_map_plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1464 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/plot/test_direction_color_keys.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4524 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/plot/test_inverse_pole_figure_plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5287 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/plot/test_orientation_color_keys.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4131 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/plot/test_rotation_plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16266 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/plot/test_stereographic_plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5279 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/plot/test_unit_cell_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 13:28:03.596073 orix-0.9.0rc2/orix/tests/quaternion/
+-rw-r--r--   0 runner    (1001) docker     (121)      709 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/quaternion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6712 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/quaternion/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25914 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/quaternion/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4617 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/quaternion/test_orientation_region.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9743 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/quaternion/test_quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21660 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/quaternion/test_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32685 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/quaternion/test_symmetry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 13:28:03.596073 orix-0.9.0rc2/orix/tests/sampling/
+-rw-r--r--   0 runner    (1001) docker     (121)      709 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4346 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/sampling/test_cubochoric_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2399 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/sampling/test_s2_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4527 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/sampling/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2291 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/test_axangle.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37004 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/test_crystal_map.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4042 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/test_crystal_map_properties.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2002 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/test_fundamental_sector.py
+-rw-r--r--   0 runner    (1001) docker     (121)    86877 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/test_miller.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1907 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/test_neoeuler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5756 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/test_object3d.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26968 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/test_phase_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1838 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/test_spherical_region.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4898 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/test_stereographic_projection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4927 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21110 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/tests/test_vector3d.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 13:28:03.596073 orix-0.9.0rc2/orix/vector/
+-rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5753 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/vector/fundamental_sector.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33226 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/vector/miller.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4162 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/vector/neo_euler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1967 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/vector/spherical_region.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33825 2022-05-11 13:27:50.000000 orix-0.9.0rc2/orix/vector/vector3d.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 13:28:03.588074 orix-0.9.0rc2/orix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3373 2022-05-11 13:28:03.000000 orix-0.9.0rc2/orix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4382 2022-05-11 13:28:03.000000 orix-0.9.0rc2/orix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-11 13:28:03.000000 orix-0.9.0rc2/orix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      547 2022-05-11 13:28:03.000000 orix-0.9.0rc2/orix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-05-11 13:28:03.000000 orix-0.9.0rc2/orix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      459 2022-05-11 13:27:50.000000 orix-0.9.0rc2/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      329 2022-05-11 13:28:03.596073 orix-0.9.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2775 2022-05-11 13:27:50.000000 orix-0.9.0rc2/setup.py
```

### Comparing `orix-0.9.0.post0/CHANGELOG.rst` & `orix-0.9.0rc2/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 =========
 
 All notable changes to the ``orix`` project are documented in this file.
 
 The format is based on `Keep a Changelog <https://keepachangelog.com/en/1.0.0/>`_, and
 this project adheres to `Semantic Versioning <https://semver.org/spec/v2.0.0.html>`_.
 
-2022-05-16 - version 0.9.0
-==========================
+2022-05-16 v0.9.0
+=================
 
 Added
 -----
 - Dask computation of ``Quaternion`` and ``Rotation`` ``outer()`` methods through
   addition of a ``lazy`` parameter. This is useful to reduce memory usage when working
   with large arrays.
 - Dask implementation of the ``Quaternion`` - ``Vector3d`` outer product.
@@ -51,15 +51,14 @@
 - Organized user guide documentation into topics.
 
 Deprecated
 ----------
 - The ``convention`` parameter in ``from_euler()`` and ``to_euler()`` methods has been
   deprecated, in favour of ``direction`` in the former. This parameter will be removed
   in release 1.0.
-- ``Misorientation.distance()`` in favour of ``Misorientation.get_distance_matrix()``.
 
 Fixed
 -----
 - Fixed bug in ``sample_S2_uv_mesh()`` and removed duplicate vectors at poles.
 - The results from ``Orientation.dot_outer()`` are now returned as
   ``self.shape + other.shape``, which is consistent with ``Rotation.dot_outer()``.
 - Writing of property arrays in .ang writer from masked CrystalMap.
```

### Comparing `orix-0.9.0.post0/CONTRIBUTING.rst` & `orix-0.9.0rc2/CONTRIBUTING.rst`

 * *Files 2% similar despite different names*

```diff
@@ -194,20 +194,15 @@
 In general, we run all notebooks every time the documentation is built with Sphinx, to
 ensure that all notebooks are compatible with the current API at all times. This is
 important! For computationally expensive notebooks however, we store the cell outputs so
 the documentation doesn't take too long to build, either by us locally or the Read The
 Docs GitHub action. To check that the notebooks with stored cell outputs are compatible
 with the current API, we run a scheduled GitHub Action every Monday morning which checks
 that the notebooks run OK and that they produce the same output now as when they were
-last executed. We use `nbval <https://nbval.readthedocs.io>`_ for this.
-
-The user guide notebooks can be run interactively in the browser with the help of
-`Binder <https://mybinder.readthedocs.io>`_. When creating a server from the orix source
-code, Binder installs the packages listed in the `environment.yml` configuration file,
-which must include all `doc` dependencies in `setup.py` necessary to run the notebooks.
+last executed. We use `nbval <https://nbval.readthedocs.io/en/latest/>`_ for this.
 
 Deprecations
 ============
 
 We attempt to adhere to semantic versioning as best we can. This means that as little,
 ideally no, functionality should break between minor releases. Deprecation warnings are
 raised whenever possible and feasible for functions/methods/properties/arguments, so
```

### Comparing `orix-0.9.0.post0/LICENSE` & `orix-0.9.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/PKG-INFO` & `orix-0.9.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orix
-Version: 0.9.0.post0
+Version: 0.9.0rc2
 Summary: orix is an open-source Python library for handling crystal orientation mapping data.
 Home-page: https://orix.readthedocs.io
 Author: orix developers
 Author-email: pyxem.team@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `orix-0.9.0.post0/README.rst` & `orix-0.9.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/RELEASE.rst` & `orix-0.9.0rc2/RELEASE.rst`

 * *Files 8% similar despite different names*

```diff
@@ -8,32 +8,26 @@
 - Run all user guide notebooks locally and confirm that they produce the expected
   results.
 - Review the contributor list ``__credits__`` in ``orix/__init__.py`` to ensure all
   contributors are included and sorted correctly. Use the same ordering in the
   ``.zenodo.json`` file.
 - Bump ``__version__`` in ``orix/__init__.py``, for example to "0.8.2".
 - Update the changelog ``CHANGELOG.rst``.
-- Let the PR collect comments for a day to ensure that other maintainers are comfortable
-  with releasing. Merge.
+- Let the PR collect comments for a day to ensure that other maintainers are
+  comfortable with releasing. Merge.
 
-Tag and release
----------------
-- Create a tagged and annotated (meaning with text) release with the name "v0.8.2" and
-  title "orix 0.8.2". The tag target will be the ``master`` branch. Draw inspiration
-  from previous release texts. Publish the release.
-- Monitor the publish GitHub Action to ensure the release is successfully published to
-  PyPI.
+Release (and tag)
+-----------------
+- Create a tagged, annotated (meaning with a release text) with the name 
+  v0.8.2" and title "orix 0.8.2". The tag target will be the ``master`` branch.
+  Draw inspiration from previous release texts. Publish the release.
+- Monitor the publish GitHub Action to ensure the release is successfully 
+  published to PyPI.
 
 Post-release action
 -------------------
 - Monitor the `documentation build <https://readthedocs.org/projects/orix/builds>`_ to
   ensure that the new stable documentation is successfully built from the release.
-- Ensure that `Zenodo <https://doi.org/10.5281/zenodo.3459662>`_ received the new
-  release.
-- Ensure that Binder can run the user guide notebooks by clicking the Binder badges in
-  the top banner of one of the user guide notebooks via
-  `Read The Docs <https://orix.readthedocs.io/en/stable>`_.
-- Make a post-release PR to ``master`` with ``__version__`` updated (or reverted), e.g.
-  to "0.9.dev0", the "Unreleased" header added to the changelog, and any updates to this
-  guide if necessary.
+- Make a post-release PR to ``master`` with ``__version__`` updated (or 
+  reverted), e.g. to "0.9.dev0", and any updates to this guide if necessary.
 - Tidy up GitHub issues and close the corresponding milestone.
 - A PR to the conda-forge feedstock will be created by the conda-forge bot.
```

### Comparing `orix-0.9.0.post0/doc/Makefile` & `orix-0.9.0rc2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/_static/img/inversion.png` & `orix-0.9.0rc2/doc/_static/img/inversion.png`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/_static/img/inversion.svg` & `orix-0.9.0rc2/doc/_static/img/inversion.svg`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/_static/img/orientation-region-Oq.png` & `orix-0.9.0rc2/doc/_static/img/orientation-region-Oq.png`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/_static/img/orientation.png` & `orix-0.9.0rc2/doc/_static/img/orientation.png`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/_static/img/orientation.svg` & `orix-0.9.0rc2/doc/_static/img/orientation.svg`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/_static/img/orix_logo.png` & `orix-0.9.0rc2/doc/_static/img/orix_logo.png`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/_static/img/rotation.png` & `orix-0.9.0rc2/doc/_static/img/rotation.png`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/_static/img/rotation.svg` & `orix-0.9.0rc2/doc/_static/img/rotation.svg`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/_static/img/spherical-region-D3.png` & `orix-0.9.0rc2/doc/_static/img/spherical-region-D3.png`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/_static/img/triad-object.png` & `orix-0.9.0rc2/doc/_static/img/triad-object.png`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/bibliography.bib` & `orix-0.9.0rc2/doc/bibliography.bib`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/clustering_across_fundamental_region_boundaries.ipynb` & `orix-0.9.0rc2/doc/clustering_across_fundamental_region_boundaries.ipynb`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/clustering_misorientations.ipynb` & `orix-0.9.0rc2/doc/clustering_misorientations.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996069182389937%*

 * *Differences: {"'cells'": "{0: {'metadata': {replace: OrderedDict()}}}"}*

```diff
@@ -1,15 +1,12 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "metadata": {
-                "nbsphinx": "hidden",
-                "tags": []
-            },
+            "metadata": {},
             "source": [
                 "This notebook is part of the *orix* documentation https://orix.readthedocs.io. Links to the documentation won\u2019t work from the notebook."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `orix-0.9.0.post0/doc/clustering_orientations.ipynb` & `orix-0.9.0rc2/doc/clustering_orientations.ipynb`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/conf.py` & `orix-0.9.0rc2/doc/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 from datetime import datetime
 import inspect
 import os
 from os.path import relpath, dirname
 import re
 import sys
 
-import orix
+from orix import __author__, __version__
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 # sys.path.insert(0, os.path.abspath("."))
 sys.path.append("../")
 
 project = "orix"
-copyright = f"2018-{str(datetime.now().year)}, {orix.__author__}"
-author = orix.__author__
-release = orix.__version__
+copyright = f"2018-{str(datetime.now().year)}, {__author__}"
+author = __author__
+release = __version__
 
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinxcontrib.bibtex",
@@ -77,18 +77,18 @@
 html_favicon = "_static/img/orix_logo.png"
 
 # nbsphinx configuration
 # Taken from nbsphinx' own nbsphinx configuration file, with slight
 # modification to point nbviewer and Binder to the GitHub master links
 # when the documentation is launched from a orix version with "dev" in
 # the version
-if "dev" in orix.__version__:
+if "dev" in __version__:
     release_version = "master"
 else:
-    release_version = "v" + orix.__version__
+    release_version = "v" + __version__
 # This is processed by Jinja2 and inserted before each notebook
 nbsphinx_prolog = (
     r"""
 {% set docname = 'doc/' + env.doc2path(env.docname, base=None) %}
 
 .. raw:: html
 
@@ -134,16 +134,16 @@
 # sphinxcontrib-bibtex configuration
 bibtex_bibfiles = ["bibliography.bib"]
 
 
 def linkcode_resolve(domain, info):
     """Determine the URL corresponding to Python object.
 
-    This is taken from SciPy's ``conf.py``:
-    https://github.com/scipy/scipy/blob/main/doc/source/conf.py.
+    This is taken from SciPy's conf.py:
+    https://github.com/scipy/scipy/blob/master/doc/source/conf.py.
     """
     if domain != "py":
         return None
 
     modname = info["module"]
     fullname = info["fullname"]
 
@@ -154,17 +154,14 @@
     obj = submod
     for part in fullname.split("."):
         try:
             obj = getattr(obj, part)
         except Exception:
             return None
 
-    # Use the original function object if it is wrapped.
-    obj = getattr(obj, "__wrapped__", obj)
-
     try:
         fn = inspect.getsourcefile(obj)
     except Exception:
         fn = None
     if not fn:
         try:
             fn = inspect.getsourcefile(sys.modules[obj.__module__])
@@ -179,21 +176,21 @@
         lineno = None
 
     if lineno:
         linespec = "#L%d-L%d" % (lineno, lineno + len(source) - 1)
     else:
         linespec = ""
 
-    startdir = os.path.abspath(os.path.join(dirname(orix.__file__), ".."))
+    startdir = os.path.abspath(os.path.join(dirname(__file__), ".."))
     fn = relpath(fn, start=startdir).replace(os.path.sep, "/")
 
     if fn.startswith("orix/"):
-        m = re.match(r"^.*dev0\+([a-f\d]+)$", orix.__version__)
+        m = re.match(r"^.*dev0\+([a-f0-9]+)$", __version__)
         pre_link = "https://github.com/pyxem/orix/blob/"
         if m:
             return pre_link + "%s/%s%s" % (m.group(1), fn, linespec)
-        elif "dev" in orix.__version__:
+        elif "dev" in __version__:
             return pre_link + "master/%s%s" % (fn, linespec)
         else:
-            return pre_link + "v%s/%s%s" % (orix.__version__, fn, linespec)
+            return pre_link + "v%s/%s%s" % (__version__, fn, linespec)
     else:
         return None
```

### Comparing `orix-0.9.0.post0/doc/crystal_directions.ipynb` & `orix-0.9.0rc2/doc/crystal_directions.ipynb`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/crystal_map.ipynb` & `orix-0.9.0rc2/doc/crystal_map.ipynb`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/crystal_reference_frame.ipynb` & `orix-0.9.0rc2/doc/crystal_reference_frame.ipynb`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/index.rst` & `orix-0.9.0rc2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/installation.rst` & `orix-0.9.0rc2/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/inverse_pole_figures.ipynb` & `orix-0.9.0rc2/doc/inverse_pole_figures.ipynb`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/make.bat` & `orix-0.9.0rc2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/point_groups.ipynb` & `orix-0.9.0rc2/doc/point_groups.ipynb`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/reference.rst` & `orix-0.9.0rc2/doc/reference.rst`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/related_projects.rst` & `orix-0.9.0rc2/doc/related_projects.rst`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/stereographic_projection.ipynb` & `orix-0.9.0rc2/doc/stereographic_projection.ipynb`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/doc/uniform_sampling_of_orientation_space.ipynb` & `orix-0.9.0rc2/doc/uniform_sampling_of_orientation_space.ipynb`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/getting_started.rst` & `orix-0.9.0rc2/getting_started.rst`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/_util.py` & `orix-0.9.0rc2/orix/_util.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/base/__init__.py` & `orix-0.9.0rc2/orix/base/__init__.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/crystal_map/__init__.py` & `orix-0.9.0rc2/orix/crystal_map/__init__.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/crystal_map/crystal_map.py` & `orix-0.9.0rc2/orix/crystal_map/crystal_map.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/crystal_map/crystal_map_properties.py` & `orix-0.9.0rc2/orix/crystal_map/crystal_map_properties.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/crystal_map/phase_list.py` & `orix-0.9.0rc2/orix/crystal_map/phase_list.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/data/__init__.py` & `orix-0.9.0rc2/orix/data/__init__.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/data/_registry.py` & `orix-0.9.0rc2/orix/data/_registry.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/io/__init__.py` & `orix-0.9.0rc2/orix/io/__init__.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/io/plugins/__init__.py` & `orix-0.9.0rc2/orix/io/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/io/plugins/_h5ebsd.py` & `orix-0.9.0rc2/orix/io/plugins/_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/io/plugins/ang.py` & `orix-0.9.0rc2/orix/io/plugins/ang.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/io/plugins/bruker_h5ebsd.py` & `orix-0.9.0rc2/orix/io/plugins/bruker_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/io/plugins/emsoft_h5ebsd.py` & `orix-0.9.0rc2/orix/io/plugins/emsoft_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/io/plugins/orix_hdf5.py` & `orix-0.9.0rc2/orix/io/plugins/orix_hdf5.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/plot/__init__.py` & `orix-0.9.0rc2/orix/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/plot/_symmetry_marker.py` & `orix-0.9.0rc2/orix/plot/_symmetry_marker.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/plot/_util.py` & `orix-0.9.0rc2/orix/plot/_util.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/plot/crystal_map_plot.py` & `orix-0.9.0rc2/orix/plot/crystal_map_plot.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/plot/direction_color_keys/__init__.py` & `orix-0.9.0rc2/orix/plot/direction_color_keys/__init__.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/plot/direction_color_keys/_util.py` & `orix-0.9.0rc2/orix/plot/direction_color_keys/_util.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/plot/direction_color_keys/direction_color_key.py` & `orix-0.9.0rc2/orix/plot/direction_color_keys/direction_color_key.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/plot/direction_color_keys/direction_color_key_tsl.py` & `orix-0.9.0rc2/orix/plot/direction_color_keys/direction_color_key_tsl.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/plot/inverse_pole_figure_plot.py` & `orix-0.9.0rc2/orix/plot/inverse_pole_figure_plot.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/plot/orientation_color_keys/__init__.py` & `orix-0.9.0rc2/orix/plot/orientation_color_keys/__init__.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/plot/orientation_color_keys/euler_color_key.py` & `orix-0.9.0rc2/orix/plot/orientation_color_keys/euler_color_key.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/plot/orientation_color_keys/ipf_color_key.py` & `orix-0.9.0rc2/orix/plot/orientation_color_keys/ipf_color_key.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/plot/orientation_color_keys/ipf_color_key_tsl.py` & `orix-0.9.0rc2/orix/plot/orientation_color_keys/ipf_color_key_tsl.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/plot/rotation_plot.py` & `orix-0.9.0rc2/orix/plot/rotation_plot.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/plot/stereographic_plot.py` & `orix-0.9.0rc2/orix/plot/stereographic_plot.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/plot/unit_cell_plot.py` & `orix-0.9.0rc2/orix/plot/unit_cell_plot.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/projections/__init__.py` & `orix-0.9.0rc2/orix/projections/__init__.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/projections/stereographic.py` & `orix-0.9.0rc2/orix/projections/stereographic.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/quaternion/__init__.py` & `orix-0.9.0rc2/orix/quaternion/__init__.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/quaternion/_conversions.py` & `orix-0.9.0rc2/orix/quaternion/_conversions.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/quaternion/orientation.py` & `orix-0.9.0rc2/orix/quaternion/orientation.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,19 +230,14 @@
             o_inside[outside] = o_transformed
             outside = ~(o_inside < orientation_region)
             if not np.any(outside):
                 break
         o_inside._symmetry = (Gl, Gr)
         return o_inside
 
-    @deprecated(
-        since="0.9",
-        alternative="orix.quaternion.Misorientation.get_distance_matrix",
-        removal="0.10",
-    )
     def distance(self, verbose=False, split_size=100):
         """Symmetry reduced distance.
 
         Compute the shortest distance between all orientations
         considering symmetries.
 
         Parameters
```

### Comparing `orix-0.9.0.post0/orix/quaternion/orientation_region.py` & `orix-0.9.0rc2/orix/quaternion/orientation_region.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/quaternion/quaternion.py` & `orix-0.9.0rc2/orix/quaternion/quaternion.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/quaternion/rotation.py` & `orix-0.9.0rc2/orix/quaternion/rotation.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/quaternion/symmetry.py` & `orix-0.9.0rc2/orix/quaternion/symmetry.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/sampling/S2_sampling.py` & `orix-0.9.0rc2/orix/sampling/S2_sampling.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/sampling/SO3_sampling.py` & `orix-0.9.0rc2/orix/sampling/SO3_sampling.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/sampling/__init__.py` & `orix-0.9.0rc2/orix/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/sampling/_cubochoric_sampling.py` & `orix-0.9.0rc2/orix/sampling/_cubochoric_sampling.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/sampling/sample_generators.py` & `orix-0.9.0rc2/orix/sampling/sample_generators.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/conftest.py` & `orix-0.9.0rc2/orix/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/data/__init__.py` & `orix-0.9.0rc2/orix/tests/data/__init__.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/data/test_data.py` & `orix-0.9.0rc2/orix/tests/data/test_data.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/io/__init__.py` & `orix-0.9.0rc2/orix/tests/io/__init__.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/io/test_ang.py` & `orix-0.9.0rc2/orix/tests/io/test_ang.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/io/test_bruker_h5ebsd.py` & `orix-0.9.0rc2/orix/tests/io/test_bruker_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/io/test_emsoft_h5ebsd.py` & `orix-0.9.0rc2/orix/tests/io/test_emsoft_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/io/test_h5ebsd.py` & `orix-0.9.0rc2/orix/tests/io/test_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/io/test_io.py` & `orix-0.9.0rc2/orix/tests/io/test_io.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/io/test_orix_hdf5.py` & `orix-0.9.0rc2/orix/tests/io/test_orix_hdf5.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/plot/__init__.py` & `orix-0.9.0rc2/orix/tests/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/plot/test_crystal_map_plot.py` & `orix-0.9.0rc2/orix/tests/plot/test_crystal_map_plot.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/plot/test_direction_color_keys.py` & `orix-0.9.0rc2/orix/tests/plot/test_direction_color_keys.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/plot/test_inverse_pole_figure_plot.py` & `orix-0.9.0rc2/orix/tests/plot/test_inverse_pole_figure_plot.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/plot/test_orientation_color_keys.py` & `orix-0.9.0rc2/orix/tests/plot/test_orientation_color_keys.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/plot/test_rotation_plot.py` & `orix-0.9.0rc2/orix/tests/plot/test_rotation_plot.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/plot/test_stereographic_plot.py` & `orix-0.9.0rc2/orix/tests/plot/test_stereographic_plot.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/plot/test_unit_cell_plot.py` & `orix-0.9.0rc2/orix/tests/plot/test_unit_cell_plot.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/quaternion/__init__.py` & `orix-0.9.0rc2/orix/tests/quaternion/__init__.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/quaternion/test_conversions.py` & `orix-0.9.0rc2/orix/tests/quaternion/test_conversions.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/quaternion/test_orientation.py` & `orix-0.9.0rc2/orix/tests/quaternion/test_orientation.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,14 @@
     v1 = o * v
     v1 = Vector3d(v1.data.round(4))
     v2 = oc * v
     v2 = Vector3d(v2.data.round(4))
     assert v1._tuples == v2._tuples
 
 
-# TODO: Remove in 0.10
 @pytest.mark.parametrize(
     "orientation, symmetry, expected",
     [
         ((1, 0, 0, 0), C1, [0]),
         ([(1, 0, 0, 0), (0.7071, 0.7071, 0, 0)], C1, [[0, np.pi / 2], [np.pi / 2, 0]]),
         ([(1, 0, 0, 0), (0.7071, 0.7071, 0, 0)], C4, [[0, np.pi / 2], [np.pi / 2, 0]]),
         ([(1, 0, 0, 0), (0.7071, 0, 0, 0.7071)], C4, [[0, 0], [0, 0]]),
@@ -112,16 +111,15 @@
         ),
     ],
     indirect=["orientation"],
 )
 def test_distance(orientation, symmetry, expected):
     orientation.symmetry = symmetry
     orientation = orientation.map_into_symmetry_reduced_zone(verbose=True)
-    with pytest.warns(np.VisibleDeprecationWarning, match="Function "):
-        distance = orientation.distance(verbose=True)
+    distance = orientation.distance(verbose=True)
     assert np.allclose(distance, expected, atol=1e-3)
 
 
 @pytest.mark.parametrize("symmetry", [C1, C2, C4, D2, D6, T, O])
 def test_getitem(orientation, symmetry):
     orientation.symmetry = symmetry
     assert orientation[0].symmetry._tuples == symmetry._tuples
@@ -374,28 +372,27 @@
         # for identical symmetries this is equivalent to the old
         # distance function:
         # d = s2.outer(~m).outer(s1.outer(s1)).outer(m).outer(s2)
         p12 = p1.outer(p2)
         angle2 = p12.angle.min(axis=(0, 2, 3, 5))
         assert np.allclose(angle1, angle2)
 
-    # TODO: Remove in 0.10
+    # TODO: remove when distance() is removed
     @pytest.mark.parametrize("symmetry", _groups[:-1])
     def test_get_distance_matrix_equal_distance(self, symmetry):
         # do not test Oh, as this takes ~4 GB
         shape = (3, 2)
         n = np.prod(shape)
         m = Misorientation.random(shape)
         m.symmetry = (symmetry, symmetry)
         angle1 = m.get_distance_matrix().reshape(n, n, order="F")
         m1 = m.flatten()
         angle2 = m1.get_distance_matrix()
         assert np.allclose(angle1, angle2)
-        with pytest.warns(np.VisibleDeprecationWarning, match="Function "):
-            angle3 = m1.distance()
+        angle3 = m1.distance()
         assert np.allclose(angle1, angle3)
 
 
 def test_orientation_equality():
     # symmetries must also be the same to be equal
     o1 = Orientation.random((6, 5))
     o2 = Orientation(o1)
```

### Comparing `orix-0.9.0.post0/orix/tests/quaternion/test_orientation_region.py` & `orix-0.9.0rc2/orix/tests/quaternion/test_orientation_region.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/quaternion/test_quaternion.py` & `orix-0.9.0rc2/orix/tests/quaternion/test_quaternion.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/quaternion/test_rotation.py` & `orix-0.9.0rc2/orix/tests/quaternion/test_rotation.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/quaternion/test_symmetry.py` & `orix-0.9.0rc2/orix/tests/quaternion/test_symmetry.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/sampling/__init__.py` & `orix-0.9.0rc2/orix/tests/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/sampling/test_cubochoric_sampling.py` & `orix-0.9.0rc2/orix/tests/sampling/test_cubochoric_sampling.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/sampling/test_s2_sampling.py` & `orix-0.9.0rc2/orix/tests/sampling/test_s2_sampling.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/sampling/test_sampling.py` & `orix-0.9.0rc2/orix/tests/sampling/test_sampling.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/test_axangle.py` & `orix-0.9.0rc2/orix/tests/test_axangle.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/test_crystal_map.py` & `orix-0.9.0rc2/orix/tests/test_crystal_map.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/test_crystal_map_properties.py` & `orix-0.9.0rc2/orix/tests/test_crystal_map_properties.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/test_fundamental_sector.py` & `orix-0.9.0rc2/orix/tests/test_fundamental_sector.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/test_miller.py` & `orix-0.9.0rc2/orix/tests/test_miller.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/test_neoeuler.py` & `orix-0.9.0rc2/orix/tests/test_neoeuler.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/test_object3d.py` & `orix-0.9.0rc2/orix/tests/test_object3d.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/test_phase_list.py` & `orix-0.9.0rc2/orix/tests/test_phase_list.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/test_spherical_region.py` & `orix-0.9.0rc2/orix/tests/test_spherical_region.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/test_stereographic_projection.py` & `orix-0.9.0rc2/orix/tests/test_stereographic_projection.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/test_util.py` & `orix-0.9.0rc2/orix/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/tests/test_vector3d.py` & `orix-0.9.0rc2/orix/tests/test_vector3d.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/vector/__init__.py` & `orix-0.9.0rc2/orix/vector/__init__.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/vector/fundamental_sector.py` & `orix-0.9.0rc2/orix/vector/fundamental_sector.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/vector/miller.py` & `orix-0.9.0rc2/orix/vector/miller.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/vector/neo_euler.py` & `orix-0.9.0rc2/orix/vector/neo_euler.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/vector/spherical_region.py` & `orix-0.9.0rc2/orix/vector/spherical_region.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix/vector/vector3d.py` & `orix-0.9.0rc2/orix/vector/vector3d.py`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/orix.egg-info/PKG-INFO` & `orix-0.9.0rc2/orix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orix
-Version: 0.9.0.post0
+Version: 0.9.0rc2
 Summary: orix is an open-source Python library for handling crystal orientation mapping data.
 Home-page: https://orix.readthedocs.io
 Author: orix developers
 Author-email: pyxem.team@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `orix-0.9.0.post0/orix.egg-info/SOURCES.txt` & `orix-0.9.0rc2/orix.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.rst
 RELEASE.rst
-environment.yml
 getting_started.rst
 readthedocs.yml
 setup.cfg
 setup.py
 doc/Makefile
 doc/bibliography.bib
 doc/bibliography.rst
```

### Comparing `orix-0.9.0.post0/orix.egg-info/requires.txt` & `orix-0.9.0rc2/orix.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `orix-0.9.0.post0/setup.py` & `orix-0.9.0rc2/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/eotdl-2024.3.15.tar.gz` & `tmp/eotdl-2024.4.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eotdl-2024.3.15.tar", max compression
+gzip compressed data, was "eotdl-2024.4.25.tar", max compression
```

## Comparing `eotdl-2024.3.15.tar` & `eotdl-2024.4.25.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rwxr-xr-x   0        0        0     2849 2024-02-15 09:14:02.115016 eotdl-2024.3.15/README.md
--rwxr-xr-x   0        0        0       27 2024-03-15 08:29:52.982117 eotdl-2024.3.15/eotdl/__init__.py
--rwxr-xr-x   0        0        0      231 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/access/__init__.py
--rwxr-xr-x   0        0        0      107 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/access/airbus/__init__.py
--rwxr-xr-x   0        0        0    12018 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/access/airbus/client.py
--rwxr-xr-x   0        0        0     1009 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/access/airbus/parameters.py
--rwxr-xr-x   0        0        0      652 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/access/airbus/utils.py
--rwxr-xr-x   0        0        0     1568 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/access/download.py
--rwxr-xr-x   0        0        0      633 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/access/search.py
--rwxr-xr-x   0        0        0      238 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/access/sentinelhub/__init__.py
--rwxr-xr-x   0        0        0     4098 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/access/sentinelhub/client.py
--rwxr-xr-x   0        0        0     4142 2023-11-03 17:10:29.372943 eotdl-2024.3.15/eotdl/access/sentinelhub/evalscripts.py
--rwxr-xr-x   0        0        0     2061 2023-11-03 17:10:29.372943 eotdl-2024.3.15/eotdl/access/sentinelhub/parameters.py
--rwxr-xr-x   0        0        0     3295 2023-11-03 17:10:29.372943 eotdl-2024.3.15/eotdl/access/sentinelhub/utils.py
--rwxr-xr-x   0        0        0       99 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/auth/__init__.py
--rwxr-xr-x   0        0        0     2029 2024-02-15 10:15:50.924638 eotdl-2024.3.15/eotdl/auth/auth.py
--rwxr-xr-x   0        0        0      308 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/auth/errors.py
--rwxr-xr-x   0        0        0      115 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/auth/is_logged.py
--rwxr-xr-x   0        0        0      161 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/auth/logout.py
--rwxr-xr-x   0        0        0      660 2024-03-14 14:19:45.079563 eotdl-2024.3.15/eotdl/cli.py
--rwxr-xr-x   0        0        0        0 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/commands/__init__.py
--rwxr-xr-x   0        0        0     1544 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/commands/auth.py
--rwxr-xr-x   0        0        0     5205 2024-03-14 14:19:45.079563 eotdl-2024.3.15/eotdl/commands/datasets.py
--rwxr-xr-x   0        0        0     4873 2024-03-14 14:19:45.079563 eotdl-2024.3.15/eotdl/commands/models.py
--rwxr-xr-x   0        0        0      269 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/curation/__init__.py
--rwxr-xr-x   0        0        0      220 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/curation/stac/__init__.py
--rwxr-xr-x   0        0        0     3347 2023-11-03 17:10:29.372943 eotdl-2024.3.15/eotdl/curation/stac/assets.py
--rwxr-xr-x   0        0        0     5540 2023-12-11 13:21:31.120571 eotdl-2024.3.15/eotdl/curation/stac/dataframe.py
--rwxr-xr-x   0        0        0     8493 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/curation/stac/dataframe_bck.py
--rwxr-xr-x   0        0        0     1520 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/curation/stac/dataframe_labeling.py
--rwxr-xr-x   0        0        0      629 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/curation/stac/extensions/__init__.py
--rwxr-xr-x   0        0        0      671 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/curation/stac/extensions/base.py
--rwxr-xr-x   0        0        0      370 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/curation/stac/extensions/dem.py
--rwxr-xr-x   0        0        0     4004 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/curation/stac/extensions/eo.py
--rwxr-xr-x   0        0        0      159 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/curation/stac/extensions/label/__init__.py
--rwxr-xr-x   0        0        0     4069 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/curation/stac/extensions/label/base.py
--rwxr-xr-x   0        0        0     8074 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/curation/stac/extensions/label/image_name_labeler.py
--rwxr-xr-x   0        0        0     8787 2023-11-03 17:10:29.372943 eotdl-2024.3.15/eotdl/curation/stac/extensions/label/scaneo.py
--rwxr-xr-x   0        0        0    21429 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/curation/stac/extensions/ml_dataset.py
--rwxr-xr-x   0        0        0     1236 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/curation/stac/extensions/projection.py
--rwxr-xr-x   0        0        0     1540 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/curation/stac/extensions/raster.py
--rwxr-xr-x   0        0        0     1633 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/curation/stac/extensions/sar.py
--rwxr-xr-x   0        0        0     5108 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/curation/stac/extent.py
--rwxr-xr-x   0        0        0     1529 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/curation/stac/parsers.py
--rwxr-xr-x   0        0        0    13180 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/curation/stac/stac.py
--rwxr-xr-x   0        0        0      170 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/datasets/__init__.py
--rwxr-xr-x   0        0        0     3880 2024-03-14 14:19:45.079563 eotdl-2024.3.15/eotdl/datasets/download.py
--rwxr-xr-x   0        0        0     5782 2024-03-14 15:01:37.236856 eotdl-2024.3.15/eotdl/datasets/ingest.py
--rwxr-xr-x   0        0        0     1457 2024-03-14 14:19:45.079563 eotdl-2024.3.15/eotdl/datasets/metadata.py
--rwxr-xr-x   0        0        0     1041 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/datasets/retrieve.py
--rw-r--r--   0        0        0      386 2024-03-14 14:19:45.079563 eotdl-2024.3.15/eotdl/datasets/update.py
--rwxr-xr-x   0        0        0       53 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/files/__init__.py
--rwxr-xr-x   0        0        0     6185 2024-03-14 14:19:45.079563 eotdl-2024.3.15/eotdl/files/ingest.py
--rwxr-xr-x   0        0        0      108 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/models/__init__.py
--rwxr-xr-x   0        0        0     4119 2024-03-14 14:19:45.079563 eotdl-2024.3.15/eotdl/models/download.py
--rwxr-xr-x   0        0        0     3381 2024-03-15 08:28:10.281823 eotdl-2024.3.15/eotdl/models/ingest.py
--rwxr-xr-x   0        0        0     1443 2024-03-15 08:29:00.669967 eotdl-2024.3.15/eotdl/models/metadata.py
--rwxr-xr-x   0        0        0      664 2023-11-03 16:15:15.223318 eotdl-2024.3.15/eotdl/models/retrieve.py
--rw-r--r--   0        0        0      374 2024-03-14 14:19:45.079563 eotdl-2024.3.15/eotdl/models/update.py
--rwxr-xr-x   0        0        0      791 2024-03-14 14:19:45.079563 eotdl-2024.3.15/eotdl/repos/APIRepo.py
--rwxr-xr-x   0        0        0      957 2024-02-15 09:10:12.234799 eotdl-2024.3.15/eotdl/repos/AuthAPIRepo.py
--rwxr-xr-x   0        0        0     1154 2024-02-15 09:10:12.234799 eotdl-2024.3.15/eotdl/repos/AuthRepo.py
--rwxr-xr-x   0        0        0     2660 2024-03-14 14:19:45.079563 eotdl-2024.3.15/eotdl/repos/DatasetsAPIRepo.py
--rwxr-xr-x   0        0        0     6768 2024-02-15 09:10:12.234799 eotdl-2024.3.15/eotdl/repos/FilesAPIRepo.py
--rwxr-xr-x   0        0        0     1677 2024-03-14 14:19:45.079563 eotdl-2024.3.15/eotdl/repos/ModelsAPIRepo.py
--rwxr-xr-x   0        0        0      222 2023-11-03 16:15:15.227318 eotdl-2024.3.15/eotdl/repos/__init__.py
--rwxr-xr-x   0        0        0       41 2023-11-03 16:15:15.227318 eotdl-2024.3.15/eotdl/shared/__init__.py
--rwxr-xr-x   0        0        0      479 2023-11-03 16:15:15.227318 eotdl-2024.3.15/eotdl/shared/checksum.py
--rwxr-xr-x   0        0        0      178 2023-11-03 16:15:15.227318 eotdl-2024.3.15/eotdl/tools/__init__.py
--rwxr-xr-x   0        0        0     7320 2023-11-03 16:15:15.227318 eotdl-2024.3.15/eotdl/tools/geo_utils.py
--rwxr-xr-x   0        0        0     1664 2023-11-03 16:15:15.227318 eotdl-2024.3.15/eotdl/tools/metadata.py
--rwxr-xr-x   0        0        0     1152 2023-11-03 16:15:15.227318 eotdl-2024.3.15/eotdl/tools/paths.py
--rwxr-xr-x   0        0        0     5763 2023-11-03 16:15:15.227318 eotdl-2024.3.15/eotdl/tools/stac.py
--rwxr-xr-x   0        0        0     4691 2023-11-03 16:15:15.227318 eotdl-2024.3.15/eotdl/tools/time_utils.py
--rwxr-xr-x   0        0        0     6354 2023-11-03 17:10:29.372943 eotdl-2024.3.15/eotdl/tools/tools.py
--rwxr-xr-x   0        0        0      944 2024-03-15 08:29:52.982117 eotdl-2024.3.15/pyproject.toml
--rw-r--r--   0        0        0     4052 1970-01-01 00:00:00.000000 eotdl-2024.3.15/PKG-INFO
+-rwxr-xr-x   0        0        0     2849 2024-04-25 07:56:54.008592 eotdl-2024.4.25/README.md
+-rwxr-xr-x   0        0        0       27 2024-04-25 10:44:50.799369 eotdl-2024.4.25/eotdl/__init__.py
+-rwxr-xr-x   0        0        0      231 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/access/__init__.py
+-rwxr-xr-x   0        0        0      107 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/access/airbus/__init__.py
+-rwxr-xr-x   0        0        0    12018 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/access/airbus/client.py
+-rwxr-xr-x   0        0        0     1009 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/access/airbus/parameters.py
+-rwxr-xr-x   0        0        0      652 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/access/airbus/utils.py
+-rwxr-xr-x   0        0        0     1568 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/access/download.py
+-rwxr-xr-x   0        0        0      633 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/access/search.py
+-rwxr-xr-x   0        0        0      238 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/access/sentinelhub/__init__.py
+-rwxr-xr-x   0        0        0     4098 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/access/sentinelhub/client.py
+-rwxr-xr-x   0        0        0     4142 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/access/sentinelhub/evalscripts.py
+-rwxr-xr-x   0        0        0     2061 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/access/sentinelhub/parameters.py
+-rwxr-xr-x   0        0        0     3295 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/access/sentinelhub/utils.py
+-rwxr-xr-x   0        0        0       99 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/auth/__init__.py
+-rwxr-xr-x   0        0        0     2029 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/auth/auth.py
+-rwxr-xr-x   0        0        0      308 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/auth/errors.py
+-rwxr-xr-x   0        0        0      115 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/auth/is_logged.py
+-rwxr-xr-x   0        0        0      161 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/auth/logout.py
+-rwxr-xr-x   0        0        0      660 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/cli.py
+-rwxr-xr-x   0        0        0        0 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/commands/__init__.py
+-rwxr-xr-x   0        0        0     1544 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/commands/auth.py
+-rwxr-xr-x   0        0        0     5205 2024-04-25 08:14:02.237444 eotdl-2024.4.25/eotdl/commands/datasets.py
+-rwxr-xr-x   0        0        0     4873 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/commands/models.py
+-rwxr-xr-x   0        0        0      269 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/curation/__init__.py
+-rwxr-xr-x   0        0        0      220 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/curation/stac/__init__.py
+-rwxr-xr-x   0        0        0     3347 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/curation/stac/assets.py
+-rwxr-xr-x   0        0        0     5503 2024-04-25 10:24:33.763860 eotdl-2024.4.25/eotdl/curation/stac/dataframe.py
+-rwxr-xr-x   0        0        0     8493 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/curation/stac/dataframe_bck.py
+-rwxr-xr-x   0        0        0     1520 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/curation/stac/dataframe_labeling.py
+-rwxr-xr-x   0        0        0      629 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/curation/stac/extensions/__init__.py
+-rwxr-xr-x   0        0        0      671 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/curation/stac/extensions/base.py
+-rwxr-xr-x   0        0        0      370 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/extensions/dem.py
+-rwxr-xr-x   0        0        0     4004 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/extensions/eo.py
+-rwxr-xr-x   0        0        0      159 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/extensions/label/__init__.py
+-rwxr-xr-x   0        0        0     4069 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/extensions/label/base.py
+-rwxr-xr-x   0        0        0     8074 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/extensions/label/image_name_labeler.py
+-rwxr-xr-x   0        0        0     8787 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/extensions/label/scaneo.py
+-rwxr-xr-x   0        0        0    21429 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/extensions/ml_dataset.py
+-rwxr-xr-x   0        0        0     1236 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/extensions/projection.py
+-rwxr-xr-x   0        0        0     1540 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/extensions/raster.py
+-rwxr-xr-x   0        0        0     1633 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/extensions/sar.py
+-rwxr-xr-x   0        0        0     5108 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/extent.py
+-rwxr-xr-x   0        0        0     1529 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/parsers.py
+-rwxr-xr-x   0        0        0    13180 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/stac.py
+-rwxr-xr-x   0        0        0      170 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/datasets/__init__.py
+-rwxr-xr-x   0        0        0     3667 2024-04-25 10:24:33.763860 eotdl-2024.4.25/eotdl/datasets/download.py
+-rwxr-xr-x   0        0        0     5806 2024-04-25 10:24:33.763860 eotdl-2024.4.25/eotdl/datasets/ingest.py
+-rwxr-xr-x   0        0        0     1457 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/datasets/metadata.py
+-rwxr-xr-x   0        0        0     1041 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/datasets/retrieve.py
+-rw-r--r--   0        0        0      386 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/datasets/update.py
+-rwxr-xr-x   0        0        0       53 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/files/__init__.py
+-rwxr-xr-x   0        0        0     6185 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/files/ingest.py
+-rwxr-xr-x   0        0        0      108 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/models/__init__.py
+-rwxr-xr-x   0        0        0     4119 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/models/download.py
+-rwxr-xr-x   0        0        0     3381 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/models/ingest.py
+-rwxr-xr-x   0        0        0     1443 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/models/metadata.py
+-rwxr-xr-x   0        0        0      664 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/models/retrieve.py
+-rw-r--r--   0        0        0      374 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/models/update.py
+-rwxr-xr-x   0        0        0      791 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/repos/APIRepo.py
+-rwxr-xr-x   0        0        0      957 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/repos/AuthAPIRepo.py
+-rwxr-xr-x   0        0        0     1154 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/repos/AuthRepo.py
+-rwxr-xr-x   0        0        0     2660 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/repos/DatasetsAPIRepo.py
+-rwxr-xr-x   0        0        0     6768 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/repos/FilesAPIRepo.py
+-rwxr-xr-x   0        0        0     1677 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/repos/ModelsAPIRepo.py
+-rwxr-xr-x   0        0        0      222 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/repos/__init__.py
+-rwxr-xr-x   0        0        0       41 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/shared/__init__.py
+-rwxr-xr-x   0        0        0      479 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/shared/checksum.py
+-rwxr-xr-x   0        0        0      178 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/tools/__init__.py
+-rwxr-xr-x   0        0        0     7320 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/tools/geo_utils.py
+-rwxr-xr-x   0        0        0     1664 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/tools/metadata.py
+-rwxr-xr-x   0        0        0     1152 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/tools/paths.py
+-rwxr-xr-x   0        0        0     5763 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/tools/stac.py
+-rwxr-xr-x   0        0        0     4691 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/tools/time_utils.py
+-rwxr-xr-x   0        0        0     6354 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/tools/tools.py
+-rwxr-xr-x   0        0        0      944 2024-04-25 10:44:50.795369 eotdl-2024.4.25/pyproject.toml
+-rw-r--r--   0        0        0     4052 1970-01-01 00:00:00.000000 eotdl-2024.4.25/PKG-INFO
```

### Comparing `eotdl-2024.3.15/README.md` & `eotdl-2024.4.25/README.md`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/access/airbus/client.py` & `eotdl-2024.4.25/eotdl/access/airbus/client.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/access/airbus/parameters.py` & `eotdl-2024.4.25/eotdl/access/airbus/parameters.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/access/airbus/utils.py` & `eotdl-2024.4.25/eotdl/access/airbus/utils.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/access/download.py` & `eotdl-2024.4.25/eotdl/access/download.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/access/search.py` & `eotdl-2024.4.25/eotdl/access/search.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/access/sentinelhub/client.py` & `eotdl-2024.4.25/eotdl/access/sentinelhub/client.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/access/sentinelhub/evalscripts.py` & `eotdl-2024.4.25/eotdl/access/sentinelhub/evalscripts.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/access/sentinelhub/parameters.py` & `eotdl-2024.4.25/eotdl/access/sentinelhub/parameters.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/access/sentinelhub/utils.py` & `eotdl-2024.4.25/eotdl/access/sentinelhub/utils.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/auth/auth.py` & `eotdl-2024.4.25/eotdl/auth/auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/cli.py` & `eotdl-2024.4.25/eotdl/cli.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/commands/auth.py` & `eotdl-2024.4.25/eotdl/commands/auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/commands/datasets.py` & `eotdl-2024.4.25/eotdl/commands/datasets.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/commands/models.py` & `eotdl-2024.4.25/eotdl/commands/models.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/curation/stac/assets.py` & `eotdl-2024.4.25/eotdl/curation/stac/assets.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/curation/stac/dataframe.py` & `eotdl-2024.4.25/eotdl/curation/stac/dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,17 +153,15 @@
     Read a STAC file and return a STACDataFrame
 
     :param stac_file: STAC file to read
     :param geometry_column: name of the geometry column
     """
     if isinstance(stac_file, (str, Path)):
         stac_file = pystac.read_file(stac_file)  # we assume this is always a catalog
-    print(stac_file)
     stac_file.make_all_asset_hrefs_absolute()
-    print("ie")
     children = get_all_children(stac_file)
 
     # Convert Dataframe to STACDataFrame
     dataframe = pd.DataFrame(children)
     dataframe[geometry_column] = dataframe.apply(convert_df_geom_to_shape, axis=1)
     stac_dataframe = STACDataFrame(
         dataframe,
```

### Comparing `eotdl-2024.3.15/eotdl/curation/stac/dataframe_bck.py` & `eotdl-2024.4.25/eotdl/curation/stac/dataframe_bck.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/curation/stac/dataframe_labeling.py` & `eotdl-2024.4.25/eotdl/curation/stac/dataframe_labeling.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/curation/stac/extensions/__init__.py` & `eotdl-2024.4.25/eotdl/curation/stac/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/curation/stac/extensions/base.py` & `eotdl-2024.4.25/eotdl/curation/stac/extensions/base.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/curation/stac/extensions/eo.py` & `eotdl-2024.4.25/eotdl/curation/stac/extensions/eo.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/curation/stac/extensions/label/base.py` & `eotdl-2024.4.25/eotdl/curation/stac/extensions/label/base.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/curation/stac/extensions/label/image_name_labeler.py` & `eotdl-2024.4.25/eotdl/curation/stac/extensions/label/image_name_labeler.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/curation/stac/extensions/label/scaneo.py` & `eotdl-2024.4.25/eotdl/curation/stac/extensions/label/scaneo.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/curation/stac/extensions/ml_dataset.py` & `eotdl-2024.4.25/eotdl/curation/stac/extensions/ml_dataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/curation/stac/extensions/projection.py` & `eotdl-2024.4.25/eotdl/curation/stac/extensions/projection.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/curation/stac/extensions/raster.py` & `eotdl-2024.4.25/eotdl/curation/stac/extensions/raster.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/curation/stac/extensions/sar.py` & `eotdl-2024.4.25/eotdl/curation/stac/extensions/sar.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/curation/stac/extent.py` & `eotdl-2024.4.25/eotdl/curation/stac/extent.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/curation/stac/parsers.py` & `eotdl-2024.4.25/eotdl/curation/stac/parsers.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/curation/stac/stac.py` & `eotdl-2024.4.25/eotdl/curation/stac/stac.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/datasets/download.py` & `eotdl-2024.4.25/eotdl/datasets/download.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,19 +56,18 @@
                 dataset["id"],
                 filename,
                 user,
                 download_path,
                 file_version,
                 progress=True,
             )
-            # if calculate_checksum(dst_path) != checksum:
-            #     logger(f"Checksum for {file} does not match")
-
+            if verbose:
+                logger("Generating README.md ...")
+            generate_metadata(download_path, dataset)
     else:
-        # raise NotImplementedError("Downloading a STAC dataset is not implemented")
         if verbose:
             logger("Downloading STAC metadata...")
         repo = DatasetsAPIRepo()
         gdf, error = repo.download_stac(
             dataset["id"],
             user,
         )
@@ -88,19 +87,15 @@
                     href = v["href"]
                     _, filename = href.split("/download/")
                     # will overwrite assets with same name :(
                     repo.download_file_url(
                         href, filename, f"{download_path}/assets", user
                     )
         else:
-            if verbose:
-                logger("To download assets, set assets=True or -a in the CLI.")
-    if verbose:
-        logger("Generating README.md ...")
-    generate_metadata(download_path, dataset)
+            logger("To download assets, set assets=True or -a in the CLI.")
     if verbose:
         logger("Done")
     return download_path
 
 
 @with_auth
 def download_file_url(url, path, progress=True, logger=print, user=None):
```

### Comparing `eotdl-2024.3.15/eotdl/datasets/ingest.py` & `eotdl-2024.4.25/eotdl/datasets/ingest.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
         # load metadata (legacy)
         metadata = (
             yaml.safe_load(open(folder.joinpath("metadata.yml"), "r").read()) or {}
         )
         metadata = Metadata(**metadata)
         content = None
     except Exception as e:
+        # print(str(e))
         raise Exception("Error loading metadata")
     # retrieve dataset (create if doesn't exist)
     dataset = retrieve_dataset(metadata, user)
     if content:
         content = markdown.markdown(content)
     update_metadata = True
     if "description" in dataset:
```

### Comparing `eotdl-2024.3.15/eotdl/datasets/metadata.py` & `eotdl-2024.4.25/eotdl/datasets/metadata.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/datasets/retrieve.py` & `eotdl-2024.4.25/eotdl/datasets/retrieve.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/files/ingest.py` & `eotdl-2024.4.25/eotdl/files/ingest.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/models/download.py` & `eotdl-2024.4.25/eotdl/models/download.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/models/ingest.py` & `eotdl-2024.4.25/eotdl/models/ingest.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/models/metadata.py` & `eotdl-2024.4.25/eotdl/models/metadata.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/models/retrieve.py` & `eotdl-2024.4.25/eotdl/models/retrieve.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/repos/APIRepo.py` & `eotdl-2024.4.25/eotdl/repos/APIRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/repos/AuthAPIRepo.py` & `eotdl-2024.4.25/eotdl/repos/AuthAPIRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/repos/AuthRepo.py` & `eotdl-2024.4.25/eotdl/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/repos/DatasetsAPIRepo.py` & `eotdl-2024.4.25/eotdl/repos/DatasetsAPIRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/repos/FilesAPIRepo.py` & `eotdl-2024.4.25/eotdl/repos/FilesAPIRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/repos/ModelsAPIRepo.py` & `eotdl-2024.4.25/eotdl/repos/ModelsAPIRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/tools/geo_utils.py` & `eotdl-2024.4.25/eotdl/tools/geo_utils.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/tools/metadata.py` & `eotdl-2024.4.25/eotdl/tools/metadata.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/tools/paths.py` & `eotdl-2024.4.25/eotdl/tools/paths.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/tools/stac.py` & `eotdl-2024.4.25/eotdl/tools/stac.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/tools/time_utils.py` & `eotdl-2024.4.25/eotdl/tools/time_utils.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/eotdl/tools/tools.py` & `eotdl-2024.4.25/eotdl/tools/tools.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.3.15/pyproject.toml` & `eotdl-2024.4.25/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eotdl"
-version = "2024.03.15"
+version = "2024.04.25"
 description = "Earth Observation Training Data Lab"
 authors = ["EarthPulse <it@earthpulse.es>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "eotdl"}]
 
 [tool.poetry.scripts]
```

### Comparing `eotdl-2024.3.15/PKG-INFO` & `eotdl-2024.4.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eotdl
-Version: 2024.3.15
+Version: 2024.4.25
 Summary: Earth Observation Training Data Lab
 License: MIT
 Author: EarthPulse
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eotdl Version: 2024.3.15 Summary: Earth Observation
+Metadata-Version: 2.1 Name: eotdl Version: 2024.4.25 Summary: Earth Observation
 Training Data Lab License: MIT Author: EarthPulse Author-email:
 it@earthpulse.es Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: black
 (>=23.10.1,<24.0.0) Requires-Dist: geomet (>=1.0.0,<2.0.0) Requires-Dist:
```


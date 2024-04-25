# Comparing `tmp/asf_search-7.1.0.tar.gz` & `tmp/asf_search-7.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asf_search-7.1.0.tar", last modified: Fri Apr 19 17:32:55 2024, max compression
+gzip compressed data, was "asf_search-7.1.1.tar", last modified: Thu Apr 25 18:54:17 2024, max compression
```

## Comparing `asf_search-7.1.0.tar` & `asf_search-7.1.1.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.625616 asf_search-7.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-19 17:32:51.000000 asf_search-7.1.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.589616 asf_search-7.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.593616 asf_search-7.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-19 17:32:51.000000 asf_search-7.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-19 17:32:51.000000 asf_search-7.1.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-19 17:32:51.000000 asf_search-7.1.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.593616 asf_search-7.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-19 17:32:51.000000 asf_search-7.1.0/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-19 17:32:51.000000 asf_search-7.1.0/.github/workflows/label-prod-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-19 17:32:51.000000 asf_search-7.1.0/.github/workflows/prod-request-merged.yml
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-19 17:32:51.000000 asf_search-7.1.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-19 17:32:51.000000 asf_search-7.1.0/.github/workflows/run-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-19 17:32:51.000000 asf_search-7.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    29172 2024-04-19 17:32:51.000000 asf_search-7.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-19 17:32:51.000000 asf_search-7.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-04-19 17:32:55.625616 asf_search-7.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-04-19 17:32:51.000000 asf_search-7.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.597616 asf_search-7.1.0/asf_search/
--rw-r--r--   0 runner    (1001) docker     (127)    16945 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/ASFProduct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.597616 asf_search-7.1.0/asf_search/ASFSearchOptions/
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/ASFSearchOptions/ASFSearchOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/ASFSearchOptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/ASFSearchOptions/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/ASFSearchOptions/validator_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/ASFSearchOptions/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/ASFSearchResults.py
--rw-r--r--   0 runner    (1001) docker     (127)    10680 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/ASFSession.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/ASFStackableProduct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.597616 asf_search-7.1.0/asf_search/CMR/
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/CMR/MissionList.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/CMR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44421 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/CMR/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/CMR/field_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/CMR/subquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/CMR/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.601616 asf_search-7.1.0/asf_search/Products/
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/AIRSARProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/ALOSProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/ARIAS1GUNWProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/ERSProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/JERSProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/NISARProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/OPERAS1Product.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/RADARSATProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/S1BurstProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/S1Product.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/SEASATProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/SIRCProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/SMAPProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/UAVSARProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/Products/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.601616 asf_search-7.1.0/asf_search/WKT/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/WKT/RepairEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/WKT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/WKT/validate_wkt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.601616 asf_search-7.1.0/asf_search/baseline/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/baseline/calc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/baseline/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.605616 asf_search-7.1.0/asf_search/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/constants/BEAMMODE.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/constants/DATASET.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/constants/FLIGHT_DIRECTION.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/constants/INSTRUMENT.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/constants/INTERNAL.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/constants/PLATFORM.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/constants/POLARIZATION.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/constants/PRODUCT_TYPE.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.605616 asf_search-7.1.0/asf_search/download/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/download/download.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/download/file_download_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.605616 asf_search-7.1.0/asf_search/export/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/export/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/export/export_translators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/export/geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/export/jsonlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/export/jsonlite2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/export/kml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/export/metalink.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.605616 asf_search-7.1.0/asf_search/health/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/health/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/health/health.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.605616 asf_search-7.1.0/asf_search/search/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/search/baseline_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/search/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/search/error_reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/search/geo_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/search/granule_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/search/product_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7338 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/search/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/search/search_count.py
--rw-r--r--   0 runner    (1001) docker     (127)    13707 2024-04-19 17:32:51.000000 asf_search-7.1.0/asf_search/search/search_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.621616 asf_search-7.1.0/asf_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-04-19 17:32:55.000000 asf_search-7.1.0/asf_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-04-19 17:32:55.000000 asf_search-7.1.0/asf_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 17:32:55.000000 asf_search-7.1.0/asf_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-19 17:32:55.000000 asf_search-7.1.0/asf_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 17:32:55.000000 asf_search-7.1.0/asf_search.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-19 17:32:51.000000 asf_search-7.1.0/examples/0-Intro.md
--rw-r--r--   0 runner    (1001) docker     (127)    13465 2024-04-19 17:32:51.000000 asf_search-7.1.0/examples/1-Basic_Overview.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-19 17:32:51.000000 asf_search-7.1.0/examples/2-Geographic_Search.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10801 2024-04-19 17:32:51.000000 asf_search-7.1.0/examples/3-Granule_Search.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-04-19 17:32:51.000000 asf_search-7.1.0/examples/4-Baseline_Search.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    14428 2024-04-19 17:32:51.000000 asf_search-7.1.0/examples/5-Download.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-19 17:32:51.000000 asf_search-7.1.0/examples/6-Outro.md
--rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-04-19 17:32:51.000000 asf_search-7.1.0/examples/Advanced-Custom-ASFProduct-Subclassing.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-19 17:32:51.000000 asf_search-7.1.0/examples/hello_world.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-19 17:32:51.000000 asf_search-7.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 17:32:55.625616 asf_search-7.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-19 17:32:51.000000 asf_search-7.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/tests/ASFProduct/
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/ASFProduct/test_ASFProduct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/tests/ASFSearchOptions/
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/ASFSearchOptions/test_ASFSearchOptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/tests/ASFSearchResults/
--rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/ASFSearchResults/test_ASFSearchResults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/tests/ASFSession/
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/ASFSession/test_ASFSession.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/tests/BaselineSearch/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/tests/BaselineSearch/Stack/
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/BaselineSearch/Stack/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/BaselineSearch/test_baseline_search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/tests/CMR/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/CMR/test_MissionList.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/tests/Search/
--rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/Search/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/Search/test_search_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/tests/Serialization/
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/Serialization/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/tests/WKT/
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/WKT/test_validate_wkt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.609616 asf_search-7.1.0/tests/download/
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/download/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/pytest-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)    18837 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/pytest-managers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.613616 asf_search-7.1.0/tests/yml_tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:55.621616 asf_search-7.1.0/tests/yml_tests/Resources/
--rw-r--r--   0 runner    (1001) docker     (127)    11951 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Alos_response.yml
--rw-r--r--   0 runner    (1001) docker     (127)    23351 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Alos_response_maxResults3.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11957 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Alos_response_missing_baseline.yml
--rw-r--r--   0 runner    (1001) docker     (127)    10954 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_L1.yml
--rw-r--r--   0 runner    (1001) docker     (127)    31136 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_S1_stack incomplete.yml
--rw-r--r--   0 runner    (1001) docker     (127)    48181 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_S1_stack.yml
--rw-r--r--   0 runner    (1001) docker     (127)    46473 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed.yml
--rw-r--r--   0 runner    (1001) docker     (127)    44452 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed_incomplete.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC.kml
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC.metalink
--rw-r--r--   0 runner    (1001) docker     (127)    14418 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC_Incomplete_Meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite.json
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite2.json
--rw-r--r--   0 runner    (1001) docker     (127)    12816 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC_no_stateVectors.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_ers_reference.yml
--rw-r--r--   0 runner    (1001) docker     (127)    52821 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_ers_stack preprocessed.yml
--rw-r--r--   0 runner    (1001) docker     (127)    53132 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_ers_stack.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/JERS.yml
--rw-r--r--   0 runner    (1001) docker     (127)    83735 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/JERS_stack.yml
--rw-r--r--   0 runner    (1001) docker     (127)    63985 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/OPERA_Products.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/RADARSAT.yml
--rw-r--r--   0 runner    (1001) docker     (127)   308082 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/RADARSAT_stack.yml
--rw-r--r--   0 runner    (1001) docker     (127)   376802 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/S1_Interferogram_(beta)_cmr_ummjson.yml
--rw-r--r--   0 runner    (1001) docker     (127)    38828 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/S1_baseline_stack.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/S1_response.yml
--rw-r--r--   0 runner    (1001) docker     (127)    18407 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/SLC_BURST.yml
--rw-r--r--   0 runner    (1001) docker     (127)  1807159 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/SLC_BURST_stack.yml
--rw-r--r--   0 runner    (1001) docker     (127)    16602 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/SMAP_response.yml
--rw-r--r--   0 runner    (1001) docker     (127)   600436 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/ShorelineMask26.shp
--rw-r--r--   0 runner    (1001) docker     (127)    20991 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/Resources/Shovel_Creek_many_points.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_ASFProduct.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_ASFSearchOptions.yml
--rw-r--r--   0 runner    (1001) docker     (127)    22399 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_ASFSearchResults.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_ASFSession.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_baseline_search.yml
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_campaigns.yml
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_download.yml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_known_bugs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_notebooks.yml
--rw-r--r--   0 runner    (1001) docker     (127)    20759 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_search.yml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_search_generator.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_serialization.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_stack.yml
--rw-r--r--   0 runner    (1001) docker     (127)    30725 2024-04-19 17:32:51.000000 asf_search-7.1.0/tests/yml_tests/test_validate_wkt.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.182212 asf_search-7.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-25 18:54:12.000000 asf_search-7.1.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.150212 asf_search-7.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.154212 asf_search-7.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-25 18:54:12.000000 asf_search-7.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-25 18:54:12.000000 asf_search-7.1.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-25 18:54:12.000000 asf_search-7.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.154212 asf_search-7.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-25 18:54:12.000000 asf_search-7.1.1/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-25 18:54:12.000000 asf_search-7.1.1/.github/workflows/label-prod-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-25 18:54:12.000000 asf_search-7.1.1/.github/workflows/prod-request-merged.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-25 18:54:12.000000 asf_search-7.1.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-25 18:54:12.000000 asf_search-7.1.1/.github/workflows/run-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-25 18:54:12.000000 asf_search-7.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    29667 2024-04-25 18:54:12.000000 asf_search-7.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-25 18:54:12.000000 asf_search-7.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-04-25 18:54:17.182212 asf_search-7.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-04-25 18:54:12.000000 asf_search-7.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.154212 asf_search-7.1.1/asf_search/
+-rw-r--r--   0 runner    (1001) docker     (127)    17769 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/ASFProduct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.154212 asf_search-7.1.1/asf_search/ASFSearchOptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/ASFSearchOptions/ASFSearchOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/ASFSearchOptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/ASFSearchOptions/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/ASFSearchOptions/validator_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/ASFSearchOptions/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/ASFSearchResults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10680 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/ASFSession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/ASFStackableProduct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.158212 asf_search-7.1.1/asf_search/CMR/
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/CMR/MissionList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/CMR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44421 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/CMR/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/CMR/field_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/CMR/subquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/CMR/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.158212 asf_search-7.1.1/asf_search/Products/
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/AIRSARProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/ALOSProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/ARIAS1GUNWProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/ERSProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/JERSProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/NISARProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/OPERAS1Product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/RADARSATProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/S1BurstProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/S1Product.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/SEASATProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/SIRCProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/SMAPProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/UAVSARProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.158212 asf_search-7.1.1/asf_search/WKT/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/WKT/RepairEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/WKT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13339 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/WKT/validate_wkt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.158212 asf_search-7.1.1/asf_search/baseline/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/baseline/calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/baseline/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.162212 asf_search-7.1.1/asf_search/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/constants/BEAMMODE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/constants/DATASET.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/constants/FLIGHT_DIRECTION.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/constants/INSTRUMENT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/constants/INTERNAL.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/constants/PLATFORM.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/constants/POLARIZATION.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/constants/PRODUCT_TYPE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.162212 asf_search-7.1.1/asf_search/download/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/download/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/download/file_download_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.162212 asf_search-7.1.1/asf_search/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/export/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/export/export_translators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/export/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/export/jsonlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/export/jsonlite2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/export/kml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/export/metalink.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.162212 asf_search-7.1.1/asf_search/health/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/health/health.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.166212 asf_search-7.1.1/asf_search/search/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/search/baseline_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/search/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/search/error_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/search/geo_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/search/granule_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/search/product_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/search/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/search/search_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15751 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/search/search_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.182212 asf_search-7.1.1/asf_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-04-25 18:54:17.000000 asf_search-7.1.1/asf_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-04-25 18:54:17.000000 asf_search-7.1.1/asf_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:54:17.000000 asf_search-7.1.1/asf_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-25 18:54:17.000000 asf_search-7.1.1/asf_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 18:54:17.000000 asf_search-7.1.1/asf_search.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.166212 asf_search-7.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-25 18:54:12.000000 asf_search-7.1.1/examples/0-Intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13465 2024-04-25 18:54:12.000000 asf_search-7.1.1/examples/1-Basic_Overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-25 18:54:12.000000 asf_search-7.1.1/examples/2-Geographic_Search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10801 2024-04-25 18:54:12.000000 asf_search-7.1.1/examples/3-Granule_Search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-04-25 18:54:12.000000 asf_search-7.1.1/examples/4-Baseline_Search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    14428 2024-04-25 18:54:12.000000 asf_search-7.1.1/examples/5-Download.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-25 18:54:12.000000 asf_search-7.1.1/examples/6-Outro.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-04-25 18:54:12.000000 asf_search-7.1.1/examples/Advanced-Custom-ASFProduct-Subclassing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-25 18:54:12.000000 asf_search-7.1.1/examples/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-25 18:54:12.000000 asf_search-7.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 18:54:17.182212 asf_search-7.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-25 18:54:12.000000 asf_search-7.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.166212 asf_search-7.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.166212 asf_search-7.1.1/tests/ASFProduct/
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/ASFProduct/test_ASFProduct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.166212 asf_search-7.1.1/tests/ASFSearchOptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/ASFSearchOptions/test_ASFSearchOptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.166212 asf_search-7.1.1/tests/ASFSearchResults/
+-rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/ASFSearchResults/test_ASFSearchResults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.166212 asf_search-7.1.1/tests/ASFSession/
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/ASFSession/test_ASFSession.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.166212 asf_search-7.1.1/tests/BaselineSearch/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.166212 asf_search-7.1.1/tests/BaselineSearch/Stack/
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/BaselineSearch/Stack/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/BaselineSearch/test_baseline_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.166212 asf_search-7.1.1/tests/CMR/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/CMR/test_MissionList.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.166212 asf_search-7.1.1/tests/Search/
+-rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/Search/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/Search/test_search_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.170212 asf_search-7.1.1/tests/Serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/Serialization/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.170212 asf_search-7.1.1/tests/WKT/
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/WKT/test_validate_wkt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.170212 asf_search-7.1.1/tests/download/
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/download/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/pytest-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    18837 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/pytest-managers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.170212 asf_search-7.1.1/tests/yml_tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.182212 asf_search-7.1.1/tests/yml_tests/Resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    11951 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Alos_response.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    23351 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Alos_response_maxResults3.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11957 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Alos_response_missing_baseline.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    10954 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_L1.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    31136 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_S1_stack incomplete.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    48181 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_S1_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    46473 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    44452 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed_incomplete.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC.kml
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC.metalink
+-rw-r--r--   0 runner    (1001) docker     (127)    14418 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC_Incomplete_Meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12816 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC_no_stateVectors.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_ers_reference.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    52821 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_ers_stack preprocessed.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    53132 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_ers_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/JERS.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    83735 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/JERS_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    63985 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/OPERA_Products.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/RADARSAT.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   308082 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/RADARSAT_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   376802 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/S1_Interferogram_(beta)_cmr_ummjson.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    38828 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/S1_baseline_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/S1_response.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    18407 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/SLC_BURST.yml
+-rw-r--r--   0 runner    (1001) docker     (127)  1807159 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/SLC_BURST_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16602 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/SMAP_response.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   600436 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/ShorelineMask26.shp
+-rw-r--r--   0 runner    (1001) docker     (127)    20991 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Shovel_Creek_many_points.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_ASFProduct.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_ASFSearchOptions.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    22399 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_ASFSearchResults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_ASFSession.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_baseline_search.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_campaigns.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_download.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_known_bugs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_notebooks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    20759 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_search.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_search_generator.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_serialization.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    30725 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_validate_wkt.yml
```

### Comparing `asf_search-7.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `asf_search-7.1.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `asf_search-7.1.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/.github/workflows/prod-request-merged.yml` & `asf_search-7.1.1/.github/workflows/prod-request-merged.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/.github/workflows/pypi-publish.yml` & `asf_search-7.1.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/.github/workflows/run-pytest.yml` & `asf_search-7.1.1/.github/workflows/run-pytest.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/.gitignore` & `asf_search-7.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/CHANGELOG.md` & `asf_search-7.1.1/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -22,22 +22,31 @@
 - 
 
 ### Removed:
 -
 
 -->
 ------
+## [v7.1.1](https://github.com/asfadmin/Discovery-asf_search/compare/v7.1.0...v7.1.1)
+### Changed
+- Uses `ciso8601.parse_datetime()` in baseline calculations, speeds up calculations on larger stacks
+### Added
+- Adds `ASF_LOGGER` logging in `search_generator()` and related methods
+### Fixed
+- `ASFProduct.get_sort_keys()` will no longer returns `None` if missing sort key, defaults to empty string 
+
+------
 ## [v7.1.0](https://github.com/asfadmin/Discovery-asf_search/compare/v7.0.9...v7.1.0)
 ### Added
 - Improved logging in `ASFSession` authentication methods
-
 ### Changed
 - Uses `ciso8601` module for parsing dates from CMR response, significant performance improvement post-query
 - `ASFSession` now allows for authorized user access to hidden/restricted CMR datasets via `auth_with_creds()` or `auth_with_cookiejar()` authentication methods (previously only supported via `auth_with_token()` method)
 - `ASFSession.auth_with_token()` now authenticates directly against EDL endpoint
+- UMM Platform ShortName used as final fallback criteria for product subclass assignment
 
 ------
 ## [v7.0.9](https://github.com/asfadmin/Discovery-asf_search/compare/v7.0.8...v7.0.9)
 ### Changed
 - collection "ARIA_S1_GUNW" added to `ARIA_S1_GUNW` dataset, V3 products now loaded as `ARIAS1GUNWProduct` subclass
 - `ARIAS1GUNWProduct` now exposes `ariaVersion` and (for V3 products) `inputGranules` in `ARIAS1GUNWProduct.properties`
```

### Comparing `asf_search-7.1.0/LICENSE` & `asf_search-7.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/PKG-INFO` & `asf_search-7.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 Metadata-Version: 2.1
 Name: asf_search
-Version: 7.1.0
+Version: 7.1.1
 Summary: Python wrapper for ASF's SearchAPI
 Home-page: https://github.com/asfadmin/Discovery-asf_search.git
 Author: Alaska Satellite Facility Discovery Team
 Author-email: uaf-asf-discovery@alaska.edu
 License: BSD
 Project-URL: Documentation, https://docs.asf.alaska.edu/asf_search/basics/
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: shapely
-Requires-Dist: python-dateutil
 Requires-Dist: pytz
 Requires-Dist: importlib_metadata
 Requires-Dist: numpy
 Requires-Dist: dateparser
 Requires-Dist: tenacity==8.2.2
 Requires-Dist: ciso8601
 Provides-Extra: test
-Requires-Dist: pytest<7.2.0; extra == "test"
-Requires-Dist: pytest-automation; extra == "test"
+Requires-Dist: pytest==8.1.1; extra == "test"
+Requires-Dist: pytest-automation==3.0.0; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: requests-mock; extra == "test"
 Requires-Dist: nbformat; extra == "test"
 Requires-Dist: nbconvert; extra == "test"
 Requires-Dist: ipykernel; extra == "test"
```

### Comparing `asf_search-7.1.0/README.md` & `asf_search-7.1.1/README.md`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/ASFProduct.py` & `asf_search-7.1.1/asf_search/ASFProduct.py`

 * *Files 4% similar despite different names*

```diff
@@ -280,20 +280,40 @@
 
         (See `S1Product.get_property_paths()` for example of combining _base_properties of multiple classes)
 
         :returns dictionary, {`PROPERTY_NAME`: {'path': [umm, path, to, value], 'cast (optional)': Callable_to_cast_value}, ...}
         """
         return ASFProduct._base_properties
 
-    def get_sort_keys(self) -> Tuple:
+    def get_sort_keys(self) -> Tuple[str, str]:
         """
         Returns tuple of primary and secondary date values used for sorting final search results
+        Any subclasses must return string for final `sort()` to work
         """
-        return (self.properties.get('stopTime'), self.properties.get('fileID', 'sceneName'))
-
+        # `sort()` will raise an error when comparing `NoneType`,
+        # using self._read_property() to wrap standard `dict.get()` for possible `None` values
+        primary_key = self._read_property(key='stopTime', default='')
+        secondary_key = self._read_property(
+            key='fileID', 
+            default=self._read_property('sceneName', '')
+        )
+        
+        return (primary_key, secondary_key)
+    
+    def _read_property(self, key: str, default: Any = None) -> Any:
+        """
+        Helper method wraps `properties.get()`.
+        Since a property can be `None`, if the key exists `dict.get('key', 'default')` will never return the default
+        """
+        output = default
+        if (value:=self.properties.get(key)) is not None:
+            output = value
+        
+        return output
+            
     @final
     @staticmethod
     def umm_get(item: Dict, *args):
         """
         Used to search for values in CMR UMM
 
         :param item: the umm dict returned from CMR
```

### Comparing `asf_search-7.1.0/asf_search/ASFSearchOptions/ASFSearchOptions.py` & `asf_search-7.1.1/asf_search/ASFSearchOptions/ASFSearchOptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                 value = self.__getattribute__(key)
                 yield key, value
 
     def __str__(self):
         """
         What to display if `print(opts)` is called.
         """
-        return json.dumps(dict(self), indent=4)
+        return json.dumps(dict(self), indent=4, default=str)
 
     # Default is set to '...', since 'None' is a very valid value here
     def pop(self, key, default=...):
         """
         Removes 'key' from self and returns it's value. Throws KeyError if doesn't exist
 
         :param key: name of key to return value of, and delete
```

### Comparing `asf_search-7.1.0/asf_search/ASFSearchOptions/validator_map.py` & `asf_search-7.1.1/asf_search/ASFSearchOptions/validator_map.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/ASFSearchOptions/validators.py` & `asf_search-7.1.1/asf_search/ASFSearchOptions/validators.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/ASFSearchResults.py` & `asf_search-7.1.1/asf_search/ASFSearchResults.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/ASFSession.py` & `asf_search-7.1.1/asf_search/ASFSession.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/ASFStackableProduct.py` & `asf_search-7.1.1/asf_search/ASFStackableProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/CMR/MissionList.py` & `asf_search-7.1.1/asf_search/CMR/MissionList.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/CMR/datasets.py` & `asf_search-7.1.1/asf_search/CMR/datasets.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/CMR/field_map.py` & `asf_search-7.1.1/asf_search/CMR/field_map.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/CMR/subquery.py` & `asf_search-7.1.1/asf_search/CMR/subquery.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/CMR/translate.py` & `asf_search-7.1.1/asf_search/CMR/translate.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/Products/AIRSARProduct.py` & `asf_search-7.1.1/asf_search/Products/AIRSARProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/Products/ALOSProduct.py` & `asf_search-7.1.1/asf_search/Products/ALOSProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/Products/ARIAS1GUNWProduct.py` & `asf_search-7.1.1/asf_search/Products/ARIAS1GUNWProduct.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Dict
 from asf_search import ASFSession
+from asf_search.ASFProduct import ASFProduct
 from asf_search.ASFSearchOptions import ASFSearchOptions
 from asf_search.Products import S1Product
 from asf_search.CMR.translate import try_parse_float
 
 
 class ARIAS1GUNWProduct(S1Product):
     """
@@ -50,8 +51,17 @@
         return False
     
     @staticmethod
     def get_default_baseline_product_type() -> None:
         """
         Returns the product type to search for when building a baseline stack.
         """
-        return None
+        return None
+
+    @staticmethod
+    def is_ARIAS1GUNWProduct(item: Dict) -> bool:
+        platform = ASFProduct.umm_get(item['umm'], 'Platforms', 0, 'ShortName')
+        if platform in ['SENTINEL-1A', 'SENTINEL-1B']:
+            asf_platform = ASFProduct.umm_get(item['umm'], 'AdditionalAttributes', ('Name', 'ASF_PLATFORM'), 'Values', 0)
+            return 'Sentinel-1 Interferogram' in asf_platform
+
+        return False
```

### Comparing `asf_search-7.1.0/asf_search/Products/ERSProduct.py` & `asf_search-7.1.1/asf_search/Products/ERSProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/Products/JERSProduct.py` & `asf_search-7.1.1/asf_search/Products/JERSProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/Products/NISARProduct.py` & `asf_search-7.1.1/asf_search/Products/NISARProduct.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Union
+from typing import Dict, Tuple, Union
 from asf_search import ASFSearchOptions, ASFSession, ASFStackableProduct
 from asf_search.CMR.translate import try_parse_float, try_parse_int, try_round_float
 from asf_search.constants import PRODUCT_TYPE
 
 
 class NISARProduct(ASFStackableProduct):
     """
@@ -44,14 +44,14 @@
     @staticmethod
     def get_property_paths() -> Dict:
         return {
             **ASFStackableProduct.get_property_paths(),
             **NISARProduct._base_properties
         }
 
-    def get_sort_keys(self):
+    def get_sort_keys(self) -> Tuple[str, str]:
         keys = super().get_sort_keys()
-
-        if keys[0] is None:
-            return (self.properties.get('processingDate', ''), keys[1])
+        
+        if keys[0] == '':
+            return (self._read_property('processingDate', ''), keys[1])
 
         return keys
```

### Comparing `asf_search-7.1.0/asf_search/Products/OPERAS1Product.py` & `asf_search-7.1.1/asf_search/Products/OPERAS1Product.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict
+from typing import Dict, Tuple
 from asf_search import ASFSearchOptions, ASFSession
 from asf_search.CMR.translate import try_parse_date
 from asf_search.Products import S1Product
 
 
 class OPERAS1Product(S1Product):
     """
@@ -67,14 +67,14 @@
         """
         Build search options that can be used to find an insar stack for this product
 
         :return: ASFSearchOptions describing appropriate options for building a stack from this product
         """
         return None
 
-    def get_sort_keys(self):
+    def get_sort_keys(self) -> Tuple[str, str]:
         keys = super().get_sort_keys()
 
-        if keys[0] is None:
-            keys = self.properties.get('validityStartDate'), keys[1]
+        if keys[0] == '':
+            return (self._read_property('validityStartDate', ''), keys[1])
 
         return keys
```

### Comparing `asf_search-7.1.0/asf_search/Products/RADARSATProduct.py` & `asf_search-7.1.1/asf_search/Products/RADARSATProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/Products/S1BurstProduct.py` & `asf_search-7.1.1/asf_search/Products/S1BurstProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/Products/S1Product.py` & `asf_search-7.1.1/asf_search/Products/S1Product.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/Products/SEASATProduct.py` & `asf_search-7.1.1/asf_search/Products/SEASATProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/Products/SIRCProduct.py` & `asf_search-7.1.1/asf_search/Products/SIRCProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/Products/SMAPProduct.py` & `asf_search-7.1.1/asf_search/Products/SMAPProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/Products/UAVSARProduct.py` & `asf_search-7.1.1/asf_search/Products/UAVSARProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/Products/__init__.py` & `asf_search-7.1.1/asf_search/Products/__init__.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/WKT/validate_wkt.py` & `asf_search-7.1.1/asf_search/WKT/validate_wkt.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from shapely.geometry.polygon import orient
 from shapely.ops import transform, orient, unary_union
 from .RepairEntry import RepairEntry
 
 from asf_search.exceptions import ASFWKTError
 
 
-def validate_wkt(aoi: Union[str, BaseGeometry]) -> Tuple[BaseGeometry, List[RepairEntry]]:
+def validate_wkt(aoi: Union[str, BaseGeometry]) -> Tuple[BaseGeometry, BaseGeometry, List[RepairEntry]]:
     """
     Param aoi: the WKT string or Shapely Geometry to validate and prepare for the CMR query
     Validates the given area of interest, and returns a validated and simplified WKT string
     returns: The input AOI's CMR ready WKT string
     """
     if isinstance(aoi, str):
         aoi_shape = wkt.loads(aoi)
@@ -48,15 +48,15 @@
 
         return MultiPolygon(output)
                          
     
     if isinstance(shape, Polygon):
         return orient(Polygon(shape.exterior), sign=1.0)
 
-def _simplify_geometry(geometry: BaseGeometry) -> Tuple[BaseGeometry, List[RepairEntry]]:
+def _simplify_geometry(geometry: BaseGeometry) -> Tuple[BaseGeometry, BaseGeometry, List[RepairEntry]]:
     """
     param geometry: AOI Shapely Geometry to be prepped for CMR 
     prepares geometry for CMR by:
         1. Flattening any nested multi-part geometry into single collection
         2. clamping latitude +/-90, unwrapping longitude +/-180, removing coordinate dimensions higher than 2 (lon,lat)
         3. Merging any overlapping shapes
         4. convex-hulling the remainder into a single shape
@@ -161,15 +161,15 @@
         # if the vertice ordering has changed
         if reoriented.exterior.is_ccw != geometry.exterior.is_ccw:
             return reoriented, reoriented_report
 
     return reoriented, None
 
 
-def _get_clamped_and_wrapped_geometry(shape: BaseGeometry) -> Tuple[BaseGeometry, List[RepairEntry]]:
+def _get_clamped_and_wrapped_geometry(shape: BaseGeometry) -> Tuple[BaseGeometry, BaseGeometry, List[RepairEntry]]:
     """
     param geometry: Shapely geometry to clamp    
     Clamps geometry to +/-90 latitude and wraps longitude +/-180
     output: clamped shapely geometry
     """
     coords_clamped = 0
     coords_wrapped = 0
```

### Comparing `asf_search-7.1.0/asf_search/__init__.py` & `asf_search-7.1.1/asf_search/__init__.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/baseline/calc.py` & `asf_search-7.1.1/asf_search/baseline/calc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from math import sqrt, cos, sin, radians
 from typing import List
 
 import numpy as np
-from dateutil.parser import parse
+from ciso8601 import parse_datetime
 
 from asf_search import ASFProduct
 # WGS84 constants
 a = 6378137
 f = pow((1.0 - 1 / 298.257224), 2)
 # Technically f is normally considered to just be that 298... part but this is all we ever use, so
 # pre-calc and cache and call it all f anyhow
@@ -19,25 +19,25 @@
         if len(positionProperties.keys()) == 0:
             baselineProperties['noStateVectors'] = True
             continue
         if None in [positionProperties['prePositionTime'], positionProperties['postPositionTime'], positionProperties['prePosition'], positionProperties['postPosition']]:
             baselineProperties['noStateVectors'] = True
             continue
 
-        asc_node_time = parse(baselineProperties['ascendingNodeTime']).timestamp()
+        asc_node_time = parse_datetime(baselineProperties['ascendingNodeTime']).timestamp()
 
-        start = parse(product.properties['startTime']).timestamp()
-        end = parse(product.properties['stopTime']).timestamp()
+        start = parse_datetime(product.properties['startTime']).timestamp()
+        end = parse_datetime(product.properties['stopTime']).timestamp()
         center = start + ((end - start) / 2)
         baselineProperties['relative_start_time'] = start - asc_node_time
         baselineProperties['relative_center_time'] = center - asc_node_time
         baselineProperties['relative_end_time'] = end - asc_node_time
 
-        t_pre = parse(positionProperties['prePositionTime']).timestamp()
-        t_post = parse(positionProperties['postPositionTime']).timestamp()
+        t_pre = parse_datetime(positionProperties['prePositionTime']).timestamp()
+        t_post = parse_datetime(positionProperties['postPositionTime']).timestamp()
         product.baseline['relative_sv_pre_time'] = t_pre - asc_node_time
         product.baseline['relative_sv_post_time'] = t_post - asc_node_time
 
     for product in stack:
         # product.properties['granulePosition'] = get_granule_position(reference.properties['centerLat'], reference.properties['centerLon'])
         
         if product.properties['sceneName'] == reference:
```

### Comparing `asf_search-7.1.0/asf_search/baseline/stack.py` & `asf_search-7.1.1/asf_search/baseline/stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Tuple, List
-from dateutil.parser import parse
+from ciso8601 import parse_datetime
 import pytz
 
 from .calc import calculate_perpendicular_baselines
 from asf_search import ASFProduct, ASFStackableProduct, ASFSearchResults
 
 
 def get_baseline_from_stack(reference: ASFProduct, stack: ASFSearchResults) -> Tuple[ASFSearchResults, List[dict]]:
@@ -62,20 +62,20 @@
     """
     Calculates temporal baselines for a stack of products based on a reference scene and injects those values into the stack.
 
     :param reference: The reference product from which to calculate temporal baselines.
     :param stack: The stack to operate on.
     :return: None, as the operation occurs in-place on the stack provided.
     """
-    reference_time = parse(reference.properties['startTime'])
+    reference_time = parse_datetime(reference.properties['startTime'])
     if reference_time.tzinfo is None:
         reference_time = pytz.utc.localize(reference_time)
 
     for secondary in stack:
-        secondary_time = parse(secondary.properties['startTime'])
+        secondary_time = parse_datetime(secondary.properties['startTime'])
         if secondary_time.tzinfo is None:
             secondary_time = pytz.utc.localize(secondary_time)
         secondary.properties['temporalBaseline'] = (secondary_time.date() - reference_time.date()).days
 
     return stack
 
 def offset_perpendicular_baselines(reference: ASFProduct, stack: ASFSearchResults):
```

### Comparing `asf_search-7.1.0/asf_search/constants/BEAMMODE.py` & `asf_search-7.1.1/asf_search/constants/BEAMMODE.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/constants/INTERNAL.py` & `asf_search-7.1.1/asf_search/constants/INTERNAL.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/constants/PRODUCT_TYPE.py` & `asf_search-7.1.1/asf_search/constants/PRODUCT_TYPE.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/download/download.py` & `asf_search-7.1.1/asf_search/download/download.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/exceptions.py` & `asf_search-7.1.1/asf_search/exceptions.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/export/csv.py` & `asf_search-7.1.1/asf_search/export/csv.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/export/export_translators.py` & `asf_search-7.1.1/asf_search/export/export_translators.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/export/geojson.py` & `asf_search-7.1.1/asf_search/export/geojson.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/export/jsonlite.py` & `asf_search-7.1.1/asf_search/export/jsonlite.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/export/jsonlite2.py` & `asf_search-7.1.1/asf_search/export/jsonlite2.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/export/kml.py` & `asf_search-7.1.1/asf_search/export/kml.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/export/metalink.py` & `asf_search-7.1.1/asf_search/export/metalink.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/health/health.py` & `asf_search-7.1.1/asf_search/health/health.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/search/baseline_search.py` & `asf_search-7.1.1/asf_search/search/baseline_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/search/campaigns.py` & `asf_search-7.1.1/asf_search/search/campaigns.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/search/error_reporting.py` & `asf_search-7.1.1/asf_search/search/error_reporting.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/search/geo_search.py` & `asf_search-7.1.1/asf_search/search/geo_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/search/granule_search.py` & `asf_search-7.1.1/asf_search/search/granule_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/search/product_search.py` & `asf_search-7.1.1/asf_search/search/product_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/search/search.py` & `asf_search-7.1.1/asf_search/search/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Union, Sequence, Tuple
 from copy import copy
 import datetime
 
-from asf_search import ASFSearchResults
+from asf_search import ASF_LOGGER, ASFSearchResults
 from asf_search.ASFSearchOptions import ASFSearchOptions
 from asf_search.search.search_generator import search_generator
 
 def search(
         absoluteOrbit: Union[int, Tuple[int, int], range, Sequence[Union[int, Tuple[int, int], range]]] = None,
         asfFrame: Union[int, Tuple[int, int], range, Sequence[Union[int, Tuple[int, int], range]]] = None,
         beamMode: Union[str, Sequence[str]] = None,
@@ -95,10 +95,13 @@
     
     # The last page will be marked as complete if results sucessful
     for page in search_generator(opts=opts):
         results.extend(page)
         results.searchComplete = page.searchComplete
         results.searchOptions = page.searchOptions
     
-    results.sort(key=lambda p: p.get_sort_keys(), reverse=True)
+    try:
+        results.sort(key=lambda p: p.get_sort_keys(), reverse=True)
+    except TypeError as exc:
+        ASF_LOGGER.warning(f"Failed to sort final results, leaving results unsorted. Reason: {exc}")
     
     return results
```

### Comparing `asf_search-7.1.0/asf_search/search/search_count.py` & `asf_search-7.1.1/asf_search/search/search_count.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/asf_search/search/search_generator.py` & `asf_search-7.1.1/asf_search/search/search_generator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-import logging
 from typing import Dict, Generator, Union, Sequence, Tuple, List
 from copy import copy
 from requests.exceptions import HTTPError
 from requests import ReadTimeout, Response
 from tenacity import retry, retry_if_exception_type, stop_after_attempt, wait_exponential, wait_fixed
 import datetime
 import dateparser
-import warnings
 
-from asf_search import __version__
+from asf_search import ASF_LOGGER, __version__
 
 from asf_search.ASFSearchResults import ASFSearchResults
 from asf_search.ASFSearchOptions import ASFSearchOptions
 from asf_search.CMR import build_subqueries, translate_opts
 from asf_search.CMR.datasets import dataset_collections
 
 from asf_search.ASFSession import ASFSession
 from asf_search.ASFProduct import ASFProduct
 from asf_search.exceptions import ASFSearch4xxError, ASFSearch5xxError, ASFSearchError, CMRIncompleteError
 from asf_search.constants import INTERNAL
 from asf_search.WKT.validate_wkt import validate_wkt
 from asf_search.search.error_reporting import report_search_error
 import asf_search.Products as ASFProductType
-
+from shapely.geometry.base import BaseGeometry
 
 def search_generator(
         absoluteOrbit: Union[int, Tuple[int, int], range, Sequence[Union[int, Tuple[int, int], range]]] = None,
         asfFrame: Union[int, Tuple[int, int], range, Sequence[Union[int, Tuple[int, int], range]]] = None,
         beamMode: Union[str, Sequence[str]] = None,
         beamSwath: Union[str, Sequence[str]] = None,
         campaign: Union[str, Sequence[str]] = None,
@@ -78,51 +76,71 @@
 
     maxResults = opts.pop("maxResults", None)
 
     if maxResults is not None and \
         (getattr(opts, 'granule_list', False) or getattr(opts, 'product_list', False)):
             raise ValueError("Cannot use maxResults along with product_list/granule_list.")
     
+    ASF_LOGGER.debug(f'SEARCH: preprocessing opts: {opts}')
     preprocess_opts(opts)
+    ASF_LOGGER.debug(f'SEARCH: preprocessed opts: {opts}')
+    
+    ASF_LOGGER.info(f'SEARCH: Using search opts {opts}')
 
     url = '/'.join(s.strip('/') for s in [f'https://{opts.host}', f'{INTERNAL.CMR_GRANULE_PATH}'])
     total = 0
 
     queries = build_subqueries(opts)
-    for query in queries:
+
+    ASF_LOGGER.info(f'SEARCH: Using cmr endpoint: "{url}"')
+    ASF_LOGGER.debug(f'SEARCH: Built {len(queries)} subqueries')
+    
+    for subquery_idx, query in enumerate(queries):
+        ASF_LOGGER.info(f'SUBQUERY {subquery_idx + 1}: Beginning subquery with opts: {query}')
+
+        ASF_LOGGER.debug(f'TRANSLATION: Translating subquery:\n{query}')
         translated_opts = translate_opts(query)
+        ASF_LOGGER.debug(f'TRANSLATION: Subquery translated to cmr keywords:\n{translated_opts}')
         cmr_search_after_header = ""
         subquery_count = 0
 
+        page_number = 1
         while(cmr_search_after_header is not None):
             try:
+                ASF_LOGGER.debug(f'SUBQUERY {subquery_idx + 1}: Fetching page {page_number}')
                 items, subquery_max_results, cmr_search_after_header = query_cmr(opts.session, url, translated_opts, subquery_count)
             except (ASFSearchError, CMRIncompleteError) as e:
                 message = str(e)
-                logging.error(message)
+                ASF_LOGGER.error(message)
                 report_search_error(query, message)
                 opts.session.headers.pop('CMR-Search-After', None)
                 return
 
+            ASF_LOGGER.debug(f'SUBQUERY {subquery_idx + 1}: Page {page_number} fetched, returned {len(items)} items.')
             opts.session.headers.update({'CMR-Search-After': cmr_search_after_header})
             last_page = process_page(items, maxResults, subquery_max_results, total, subquery_count, opts)
             subquery_count += len(last_page)
             total += len(last_page)
             last_page.searchComplete = subquery_count == subquery_max_results or total == maxResults
             yield last_page
 
             if last_page.searchComplete:
                 if total == maxResults: # the user has as many results as they wanted
+                    ASF_LOGGER.info(f'SEARCH COMPLETE: MaxResults ({maxResults}) reached')
                     opts.session.headers.pop('CMR-Search-After', None)
                     return
                 else: # or we've gotten all possible results for this subquery
+                    ASF_LOGGER.info(f'SUBQUERY {subquery_idx + 1} COMPLETE: results exhausted for subquery')
                     cmr_search_after_header = None
+            
+            page_number += 1
 
         opts.session.headers.pop('CMR-Search-After', None)
 
+    ASF_LOGGER.info(f'SEARCH COMPLETE: results exhausted for search opts {opts}')
 
 @retry(reraise=True,
        retry=retry_if_exception_type(CMRIncompleteError),
        wait=wait_fixed(2),
        stop=stop_after_attempt(3),
     )
 def query_cmr(session: ASFSession, url: str, translated_opts: Dict, sub_query_count: int):
@@ -176,27 +194,29 @@
 
     # Platform Alias logic:
     set_platform_alias(opts=opts)
 
 
 def wrap_wkt(opts: ASFSearchOptions):
     if opts.intersectsWith is not None:
-        wrapped, _, __ = validate_wkt(opts.intersectsWith)
+        wrapped, _, repairs = validate_wkt(opts.intersectsWith)
         opts.intersectsWith = wrapped.wkt
+        if len(repairs):
+            ASF_LOGGER.warning(f"WKT REPAIR/VALIDATION: The following repairs were performed on the provided AOI:\n{[str(repair) for repair in repairs]}")
 
 
 def set_default_dates(opts: ASFSearchOptions):
     if opts.start is not None and isinstance(opts.start, str):
         opts.start = dateparser.parse(opts.start, settings={'RETURN_AS_TIMEZONE_AWARE': True})
     if opts.end is not None and isinstance(opts.end, str):
         opts.end = dateparser.parse(opts.end, settings={'RETURN_AS_TIMEZONE_AWARE': True})
     # If both are used, make sure they're in the right order:
     if opts.start is not None and opts.end is not None:
         if opts.start > opts.end:
-            warnings.warn(f"Start date ({opts.start}) is after end date ({opts.end}). Switching the two.")
+            ASF_LOGGER.warning(f"Start date ({opts.start}) is after end date ({opts.end}). Switching the two.")
             opts.start, opts.end = opts.end, opts.start
     # Can't do this sooner, since you need to compare start vs end:
     if opts.start is not None:
         opts.start = opts.start.strftime('%Y-%m-%dT%H:%M:%SZ')
     if opts.end is not None:
         opts.end = opts.end.strftime('%Y-%m-%dT%H:%M:%SZ')
 
@@ -249,43 +269,58 @@
     product_type_key = _get_product_type_key(item)
 
     # if there's a direct entry in our dataset to product type dict
     subclass = dataset_to_product_types.get(product_type_key)
     if subclass is not None:
         return subclass(item, session=session)
 
-    # or if the key matches one of the shortnames in any of our datasets
+    # if the key matches one of the shortnames in any of our datasets
     for dataset, collections in dataset_collections.items():
         if collections.get(product_type_key) is not None:
             subclass = dataset_to_product_types.get(dataset)
             if subclass is not None:
                 return subclass(item, session=session)
             break # dataset exists, but is not in dataset_to_product_types yet
 
-    return ASFProduct(item, session=session)
+    # If the platform exists, try to match it
+    platform = _get_platform(item=item)
+    if ASFProductType.ARIAS1GUNWProduct.is_ARIAS1GUNWProduct(item=item):
+        return dataset_to_product_types.get('ARIA S1 GUNW')(item, session=session)
+    elif (subclass := dataset_to_product_types.get(platform)) is not None:
+        return subclass(item, session=session)
+    
+    output = ASFProduct(item, session=session)
+    
+    granule_concept_id = output.meta.get('concept-id', 'Missing Granule Concept ID')
+    fileID = output.properties.get('fileID', output.properties.get('sceneName', 'fileID and sceneName Missing'))
+
+    ASF_LOGGER.warning(f'Failed to find corresponding ASFProduct subclass for \
+                       Product: "{fileID}", Granule Concept ID: "{granule_concept_id}", default to "ASFProduct"')
+    return output
 
 def _get_product_type_key(item: Dict) -> str:
     """Match the umm response to the right ASFProduct subclass by returning one of the following:
         1. collection shortName (Ideal case)
         2. platform_shortName (Fallback)
             - special case: Aria S1 GUNW
     """
     collection_shortName = ASFProduct.umm_get(item['umm'], 'CollectionReference', 'ShortName')
 
     if collection_shortName is None:
-        platform_shortname = ASFProduct.umm_get(item['umm'], 'Platforms', 0, 'ShortName')
-        if platform_shortname in ['SENTINEL-1A', 'SENTINEL-1B']:
-            asf_platform = ASFProduct.umm_get(item['umm'], 'AdditionalAttributes', ('Name', 'ASF_PLATFORM'), 'Values', 0)
-            if 'Sentinel-1 Interferogram' in asf_platform:
-                return 'ARIA S1 GUNW'
+        platform = _get_platform(item=item)
+        if ASFProductType.ARIAS1GUNWProduct.is_ARIAS1GUNWProduct(item=item):
+            return 'ARIA S1 GUNW'
 
-        return platform_shortname
+        return platform
 
     return collection_shortName
 
+def _get_platform(item: Dict):
+    return ASFProduct.umm_get(item['umm'], 'Platforms', 0, 'ShortName')
+
 # Maps datasets from DATASET.py and collection/platform shortnames to ASFProduct subclasses
 dataset_to_product_types = {
     'SENTINEL-1': ASFProductType.S1Product,
     'OPERA-S1': ASFProductType.OPERAS1Product,
     'OPERA-S1-CALVAL': ASFProductType.OPERAS1Product,
     'SLC-BURST': ASFProductType.S1BurstProduct,
```

### Comparing `asf_search-7.1.0/asf_search.egg-info/PKG-INFO` & `asf_search-7.1.1/asf_search.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 Metadata-Version: 2.1
 Name: asf_search
-Version: 7.1.0
+Version: 7.1.1
 Summary: Python wrapper for ASF's SearchAPI
 Home-page: https://github.com/asfadmin/Discovery-asf_search.git
 Author: Alaska Satellite Facility Discovery Team
 Author-email: uaf-asf-discovery@alaska.edu
 License: BSD
 Project-URL: Documentation, https://docs.asf.alaska.edu/asf_search/basics/
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: shapely
-Requires-Dist: python-dateutil
 Requires-Dist: pytz
 Requires-Dist: importlib_metadata
 Requires-Dist: numpy
 Requires-Dist: dateparser
 Requires-Dist: tenacity==8.2.2
 Requires-Dist: ciso8601
 Provides-Extra: test
-Requires-Dist: pytest<7.2.0; extra == "test"
-Requires-Dist: pytest-automation; extra == "test"
+Requires-Dist: pytest==8.1.1; extra == "test"
+Requires-Dist: pytest-automation==3.0.0; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: requests-mock; extra == "test"
 Requires-Dist: nbformat; extra == "test"
 Requires-Dist: nbconvert; extra == "test"
 Requires-Dist: ipykernel; extra == "test"
```

### Comparing `asf_search-7.1.0/asf_search.egg-info/SOURCES.txt` & `asf_search-7.1.1/asf_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/examples/0-Intro.md` & `asf_search-7.1.1/examples/0-Intro.md`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/examples/1-Basic_Overview.ipynb` & `asf_search-7.1.1/examples/1-Basic_Overview.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/examples/2-Geographic_Search.ipynb` & `asf_search-7.1.1/examples/2-Geographic_Search.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/examples/3-Granule_Search.ipynb` & `asf_search-7.1.1/examples/3-Granule_Search.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/examples/4-Baseline_Search.ipynb` & `asf_search-7.1.1/examples/4-Baseline_Search.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/examples/5-Download.ipynb` & `asf_search-7.1.1/examples/5-Download.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/examples/6-Outro.md` & `asf_search-7.1.1/examples/6-Outro.md`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/examples/Advanced-Custom-ASFProduct-Subclassing.ipynb` & `asf_search-7.1.1/examples/Advanced-Custom-ASFProduct-Subclassing.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/examples/hello_world.py` & `asf_search-7.1.1/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/setup.py` & `asf_search-7.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """asf_search setuptools configuration"""
 from setuptools import find_packages, setup
 
 requirements = [
     "requests",
     "shapely",
-    "python-dateutil",
     "pytz",
     "importlib_metadata",
     "numpy",
     "dateparser",
     "tenacity == 8.2.2",
     "ciso8601"
 ]
 
 test_requirements = [
-    "pytest < 7.2.0",
-    "pytest-automation",
+    "pytest==8.1.1",
+    "pytest-automation==3.0.0",
     "pytest-cov",
     "pytest-xdist",
     "coverage",
     "requests-mock",
     "nbformat",
     "nbconvert",
     "ipykernel",
@@ -50,23 +49,26 @@
     include_package_data=True,
     python_requires='>=3.8',
     install_requires=requirements,
     extras_require={ "test": test_requirements, "extras": extra_requirements},
     license='BSD',
     license_files=('LICENSE',),
     classifiers=[
-        "Development Status :: 2 - Pre-Alpha",
+        "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Software Development",
         "Topic :: Scientific/Engineering :: Atmospheric Science",
         "Topic :: Scientific/Engineering :: GIS",
         "Topic :: Scientific/Engineering :: Hydrology",
         "Topic :: Utilities"
     ],
 )
```

### Comparing `asf_search-7.1.0/tests/ASFProduct/test_ASFProduct.py` & `asf_search-7.1.1/tests/ASFProduct/test_ASFProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/ASFSearchOptions/test_ASFSearchOptions.py` & `asf_search-7.1.1/tests/ASFSearchOptions/test_ASFSearchOptions.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/ASFSearchResults/test_ASFSearchResults.py` & `asf_search-7.1.1/tests/ASFSearchResults/test_ASFSearchResults.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/ASFSession/test_ASFSession.py` & `asf_search-7.1.1/tests/ASFSession/test_ASFSession.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/BaselineSearch/Stack/test_stack.py` & `asf_search-7.1.1/tests/BaselineSearch/Stack/test_stack.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/BaselineSearch/test_baseline_search.py` & `asf_search-7.1.1/tests/BaselineSearch/test_baseline_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/CMR/test_MissionList.py` & `asf_search-7.1.1/tests/CMR/test_MissionList.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/Search/test_search.py` & `asf_search-7.1.1/tests/Search/test_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/Search/test_search_generator.py` & `asf_search-7.1.1/tests/Search/test_search_generator.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/Serialization/test_serialization.py` & `asf_search-7.1.1/tests/Serialization/test_serialization.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/WKT/test_validate_wkt.py` & `asf_search-7.1.1/tests/WKT/test_validate_wkt.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/download/test_download.py` & `asf_search-7.1.1/tests/download/test_download.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/pytest-config.yml` & `asf_search-7.1.1/tests/pytest-config.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/pytest-managers.py` & `asf_search-7.1.1/tests/pytest-managers.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/Alos_response.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/Alos_response.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/Alos_response_maxResults3.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/Alos_response_maxResults3.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/Alos_response_missing_baseline.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/Alos_response_missing_baseline.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_L1.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_L1.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_S1_stack incomplete.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_S1_stack incomplete.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_S1_stack.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_S1_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed_incomplete.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed_incomplete.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC.csv` & `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC.csv`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC.kml` & `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC.kml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC.metalink` & `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC.metalink`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC_Incomplete_Meta.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC_Incomplete_Meta.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite.json` & `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite.json`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite2.json` & `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite2.json`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_SLC_no_stateVectors.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC_no_stateVectors.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_ers_reference.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_ers_reference.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_ers_stack preprocessed.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_ers_stack preprocessed.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/Fairbanks_ers_stack.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_ers_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/JERS.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/JERS.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/JERS_stack.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/JERS_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/OPERA_Products.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/OPERA_Products.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/RADARSAT.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/RADARSAT.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/RADARSAT_stack.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/RADARSAT_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/S1_Interferogram_(beta)_cmr_ummjson.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/S1_Interferogram_(beta)_cmr_ummjson.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/S1_baseline_stack.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/S1_baseline_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/S1_response.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/S1_response.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/SLC_BURST.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/SLC_BURST.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/SLC_BURST_stack.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/SLC_BURST_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/SMAP_response.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/SMAP_response.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/ShorelineMask26.shp` & `asf_search-7.1.1/tests/yml_tests/Resources/ShorelineMask26.shp`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/Resources/Shovel_Creek_many_points.yml` & `asf_search-7.1.1/tests/yml_tests/Resources/Shovel_Creek_many_points.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/test_ASFProduct.yml` & `asf_search-7.1.1/tests/yml_tests/test_ASFProduct.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/test_ASFSearchOptions.yml` & `asf_search-7.1.1/tests/yml_tests/test_ASFSearchOptions.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/test_ASFSearchResults.yml` & `asf_search-7.1.1/tests/yml_tests/test_ASFSearchResults.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/test_ASFSession.yml` & `asf_search-7.1.1/tests/yml_tests/test_ASFSession.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/test_baseline_search.yml` & `asf_search-7.1.1/tests/yml_tests/test_baseline_search.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/test_download.yml` & `asf_search-7.1.1/tests/yml_tests/test_download.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/test_search.yml` & `asf_search-7.1.1/tests/yml_tests/test_search.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/test_serialization.yml` & `asf_search-7.1.1/tests/yml_tests/test_serialization.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/test_stack.yml` & `asf_search-7.1.1/tests/yml_tests/test_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.0/tests/yml_tests/test_validate_wkt.yml` & `asf_search-7.1.1/tests/yml_tests/test_validate_wkt.yml`

 * *Files identical despite different names*


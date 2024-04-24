# Comparing `tmp/aind_metadata_mapper-0.6.4.tar.gz` & `tmp/aind_metadata_mapper-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_metadata_mapper-0.6.4.tar", last modified: Thu Apr 18 19:24:50 2024, max compression
+gzip compressed data, was "aind_metadata_mapper-0.6.5.tar", last modified: Wed Apr 24 23:21:47 2024, max compression
```

## Comparing `aind_metadata_mapper-0.6.4.tar` & `aind_metadata_mapper-0.6.5.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.123520 aind_metadata_mapper-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.103520 aind_metadata_mapper-0.6.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.107520 aind_metadata_mapper-0.6.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.107520 aind_metadata_mapper-0.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-04-18 19:24:50.123520 aind_metadata_mapper-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.107520 aind_metadata_mapper-0.6.4/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.107520 aind_metadata_mapper-0.6.4/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.107520 aind_metadata_mapper-0.6.4/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/doc_template/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.107520 aind_metadata_mapper-0.6.4/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/examples/bergamo_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.107520 aind_metadata_mapper-0.6.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/scripts/singularity_build.def
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:24:50.123520 aind_metadata_mapper-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.103520 aind_metadata_mapper-0.6.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.111520 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-18 19:24:41.000000 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.111520 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/bergamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23421 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/bergamo/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.111520 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/ephys/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/ephys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/ephys/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.111520 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/fib/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/fib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/fib/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    10639 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/gather_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.111520 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/mesoscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/mesoscope/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.111520 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/neuropixels/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/neuropixels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/neuropixels/mvr_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/neuropixels/neuropixels_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/neuropixels/open_ephys_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/neuropixels/sync_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/neuropixels/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.123520 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-04-18 19:24:50.000000 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-18 19:24:50.000000 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:24:50.000000 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-18 19:24:50.000000 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 19:24:50.000000 aind_metadata_mapper-0.6.4/src/aind_metadata_mapper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.115520 aind_metadata_mapper-0.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.107520 aind_metadata_mapper-0.6.4/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.115520 aind_metadata_mapper-0.6.4/tests/resources/bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/bergamo/cropped_neuron50_00001.tif
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/bergamo/example_description0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    76696 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/bergamo/example_metadata.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/bergamo/expected_session.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.115520 aind_metadata_mapper-0.6.4/tests/resources/ephys/
--rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/ephys/ephys_session.json
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/ephys/newscale_main.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/ephys/newscale_surface_finding.csv
--rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/ephys/settings_main.xml
--rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/ephys/settings_surface_finding.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.115520 aind_metadata_mapper-0.6.4/tests/resources/fib/
--rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/fib/000000_ophys_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/fib/000000_ophys_session.json
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/fib/example_from_teensy.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.115520 aind_metadata_mapper-0.6.4/tests/resources/gather_metadata_job/
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/gather_metadata_job/example_procedures_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/gather_metadata_job/example_subject_response.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.115520 aind_metadata_mapper-0.6.4/tests/resources/gather_metadata_job/metadata_files/
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/gather_metadata_job/metadata_files/data_description.json
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/gather_metadata_job/metadata_files/procedures.json
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/gather_metadata_job/metadata_files/processing.json
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/gather_metadata_job/metadata_files/subject.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.119520 aind_metadata_mapper-0.6.4/tests/resources/mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/mesoscope/0123456789_Face_20240212T091444.json
--rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/mesoscope/example_extract.json
--rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/mesoscope/example_platform.json
--rw-r--r--   0 runner    (1001) docker     (127)    12038 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/mesoscope/expected_session.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.119520 aind_metadata_mapper-0.6.4/tests/resources/neuropixels/
--rw-r--r--   0 runner    (1001) docker     (127)    39424 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/neuropixels/base-missing-probe_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    40853 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/neuropixels/base_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/neuropixels/mvr.ini
--rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/neuropixels/mvr_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    42283 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/neuropixels/open-ephys-inferred_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    42266 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/neuropixels/open-ephys_rig.json
--rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/neuropixels/settings.mislabeled-probes-0.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/neuropixels/settings.mislabeled-probes-1.xml
--rw-r--r--   0 runner    (1001) docker     (127)   132751 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/neuropixels/settings.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/neuropixels/sync.yml
--rw-r--r--   0 runner    (1001) docker     (127)    46653 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/resources/neuropixels/sync_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    13902 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/test_bergamo.py
--rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/test_ephys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/test_fib.py
--rw-r--r--   0 runner    (1001) docker     (127)    15172 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/test_gather_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/test_legacy_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/test_mesoscope.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:24:50.123520 aind_metadata_mapper-0.6.4/tests/test_neuropixels/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/test_neuropixels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/test_neuropixels/test_mvr_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/test_neuropixels/test_neuropixels_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/test_neuropixels/test_open_ephys_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/test_neuropixels/test_open_ephys_rig_inferrred.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/test_neuropixels/test_sync_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-18 19:24:40.000000 aind_metadata_mapper-0.6.4/tests/test_neuropixels/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.734520 aind_metadata_mapper-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.714519 aind_metadata_mapper-0.6.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.718519 aind_metadata_mapper-0.6.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.722519 aind_metadata_mapper-0.6.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-04-24 23:21:47.734520 aind_metadata_mapper-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.722519 aind_metadata_mapper-0.6.5/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.722519 aind_metadata_mapper-0.6.5/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.722519 aind_metadata_mapper-0.6.5/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/doc_template/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.722519 aind_metadata_mapper-0.6.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/examples/bergamo_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.722519 aind_metadata_mapper-0.6.5/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/scripts/singularity_build.def
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 23:21:47.734520 aind_metadata_mapper-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.718519 aind_metadata_mapper-0.6.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.722519 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-24 23:21:38.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.722519 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/bergamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23421 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/bergamo/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.722519 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/ephys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/ephys/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.726519 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/fib/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/fib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/fib/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/gather_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.726519 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/mesoscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/mesoscope/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.726519 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/neuropixels/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/neuropixels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/neuropixels/mvr_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/neuropixels/neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/neuropixels/open_ephys_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/neuropixels/sync_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/neuropixels/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.734520 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-04-24 23:21:47.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-24 23:21:47.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 23:21:47.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-24 23:21:47.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 23:21:47.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.726519 aind_metadata_mapper-0.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.718519 aind_metadata_mapper-0.6.5/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.726519 aind_metadata_mapper-0.6.5/tests/resources/bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/bergamo/cropped_neuron50_00001.tif
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/bergamo/example_description0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    76696 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/bergamo/example_metadata.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/bergamo/expected_session.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.730519 aind_metadata_mapper-0.6.5/tests/resources/ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/ephys/ephys_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/ephys/newscale_main.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/ephys/newscale_surface_finding.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/ephys/settings_main.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/ephys/settings_surface_finding.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.730519 aind_metadata_mapper-0.6.5/tests/resources/fib/
+-rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/fib/000000_ophys_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/fib/000000_ophys_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/fib/example_from_teensy.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.730519 aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/example_procedures_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/example_subject_response.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.730519 aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/metadata_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/metadata_files/data_description.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/metadata_files/procedures.json
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/metadata_files/processing.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/metadata_files/subject.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.730519 aind_metadata_mapper-0.6.5/tests/resources/mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/mesoscope/0123456789_Face_20240212T091444.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/mesoscope/example_extract.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/mesoscope/example_platform.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12038 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/mesoscope/expected_session.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.734520 aind_metadata_mapper-0.6.5/tests/resources/neuropixels/
+-rw-r--r--   0 runner    (1001) docker     (127)    39424 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/neuropixels/base-missing-probe_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    40853 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/neuropixels/base_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/neuropixels/mvr.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/neuropixels/mvr_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42283 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/neuropixels/open-ephys-inferred_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42266 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/neuropixels/open-ephys_rig.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/neuropixels/settings.mislabeled-probes-0.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/neuropixels/settings.mislabeled-probes-1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   132751 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/neuropixels/settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/neuropixels/sync.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    46653 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/neuropixels/sync_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13902 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_bergamo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_ephys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_fib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15172 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_gather_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_legacy_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_mesoscope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.734520 aind_metadata_mapper-0.6.5/tests/test_neuropixels/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_neuropixels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_neuropixels/test_mvr_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_neuropixels/test_neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_neuropixels/test_open_ephys_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_neuropixels/test_open_ephys_rig_inferrred.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_neuropixels/test_sync_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_neuropixels/utils.py
```

### Comparing `aind_metadata_mapper-0.6.4/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_metadata_mapper-0.6.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_metadata_mapper-0.6.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/.github/ISSUE_TEMPLATE/user-story.md` & `aind_metadata_mapper-0.6.5/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/.github/workflows/tag_and_publish.yml` & `aind_metadata_mapper-0.6.5/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/.github/workflows/test_and_lint.yml` & `aind_metadata_mapper-0.6.5/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/.gitignore` & `aind_metadata_mapper-0.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/LICENSE` & `aind_metadata_mapper-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/PKG-INFO` & `aind_metadata_mapper-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-mapper
-Version: 0.6.4
+Version: 0.6.5
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_metadata_mapper-0.6.4/README.md` & `aind_metadata_mapper-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/doc_template/Makefile` & `aind_metadata_mapper-0.6.5/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/doc_template/make.bat` & `aind_metadata_mapper-0.6.5/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/doc_template/source/_static/dark-logo.svg` & `aind_metadata_mapper-0.6.5/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/doc_template/source/_static/favicon.ico` & `aind_metadata_mapper-0.6.5/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/doc_template/source/_static/light-logo.svg` & `aind_metadata_mapper-0.6.5/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/doc_template/source/conf.py` & `aind_metadata_mapper-0.6.5/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/examples/bergamo_session.py` & `aind_metadata_mapper-0.6.5/examples/bergamo_session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/pyproject.toml` & `aind_metadata_mapper-0.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/bergamo/session.py` & `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/bergamo/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/core.py` & `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/core.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/ephys/session.py` & `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/ephys/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/fib/session.py` & `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/fib/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/gather_metadata.py` & `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/gather_metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,22 +59,22 @@
 
 
 class MetadataSettings(BaseSettings):
     """Fields needed to retrieve main Metadata"""
 
     name: str
     location: str
-    subject_filepath: Optional[Path]
-    data_description_filepath: Optional[Path]
-    procedures_filepath: Optional[Path]
-    session_filepath: Optional[Path]
-    rig_filepath: Optional[Path]
-    processing_filepath: Optional[Path]
-    acquisition_filepath: Optional[Path]
-    instrument_filepath: Optional[Path]
+    subject_filepath: Optional[Path] = None
+    data_description_filepath: Optional[Path] = None
+    procedures_filepath: Optional[Path] = None
+    session_filepath: Optional[Path] = None
+    rig_filepath: Optional[Path] = None
+    processing_filepath: Optional[Path] = None
+    acquisition_filepath: Optional[Path] = None
+    instrument_filepath: Optional[Path] = None
 
 
 class JobSettings(BaseSettings):
     """Fields needed to gather all metadata"""
 
     subject_settings: Optional[SubjectSettings] = None
     data_description_settings: Optional[DataDescriptionSettings] = None
```

### Comparing `aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/mesoscope/session.py` & `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/mesoscope/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/neuropixels/mvr_rig.py` & `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/neuropixels/mvr_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/neuropixels/neuropixels_rig.py` & `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/neuropixels/neuropixels_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/neuropixels/open_ephys_rig.py` & `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/neuropixels/open_ephys_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/neuropixels/sync_rig.py` & `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/neuropixels/sync_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/src/aind_metadata_mapper/neuropixels/utils.py` & `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/neuropixels/utils.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/src/aind_metadata_mapper.egg-info/PKG-INFO` & `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-mapper
-Version: 0.6.4
+Version: 0.6.5
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_metadata_mapper-0.6.4/src/aind_metadata_mapper.egg-info/SOURCES.txt` & `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/bergamo/cropped_neuron50_00001.tif` & `aind_metadata_mapper-0.6.5/tests/resources/bergamo/cropped_neuron50_00001.tif`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/bergamo/example_description0.txt` & `aind_metadata_mapper-0.6.5/tests/resources/bergamo/example_description0.txt`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/bergamo/example_metadata.txt.gz` & `aind_metadata_mapper-0.6.5/tests/resources/bergamo/example_metadata.txt.gz`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/bergamo/expected_session.json` & `aind_metadata_mapper-0.6.5/tests/resources/bergamo/expected_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/ephys/ephys_session.json` & `aind_metadata_mapper-0.6.5/tests/resources/ephys/ephys_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/ephys/newscale_main.csv` & `aind_metadata_mapper-0.6.5/tests/resources/ephys/newscale_main.csv`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/ephys/newscale_surface_finding.csv` & `aind_metadata_mapper-0.6.5/tests/resources/ephys/newscale_surface_finding.csv`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/ephys/settings_main.xml` & `aind_metadata_mapper-0.6.5/tests/resources/ephys/settings_main.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/ephys/settings_surface_finding.xml` & `aind_metadata_mapper-0.6.5/tests/resources/ephys/settings_surface_finding.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/fib/000000_ophys_rig.json` & `aind_metadata_mapper-0.6.5/tests/resources/fib/000000_ophys_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/fib/000000_ophys_session.json` & `aind_metadata_mapper-0.6.5/tests/resources/fib/000000_ophys_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/gather_metadata_job/example_procedures_response.json` & `aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/example_procedures_response.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/gather_metadata_job/example_subject_response.json` & `aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/example_subject_response.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/gather_metadata_job/metadata_files/data_description.json` & `aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/metadata_files/data_description.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/gather_metadata_job/metadata_files/procedures.json` & `aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/metadata_files/procedures.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/gather_metadata_job/metadata_files/processing.json` & `aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/metadata_files/processing.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/gather_metadata_job/metadata_files/subject.json` & `aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/metadata_files/subject.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json` & `aind_metadata_mapper-0.6.5/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json` & `aind_metadata_mapper-0.6.5/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/mesoscope/0123456789_Face_20240212T091444.json` & `aind_metadata_mapper-0.6.5/tests/resources/mesoscope/0123456789_Face_20240212T091444.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/mesoscope/example_extract.json` & `aind_metadata_mapper-0.6.5/tests/resources/mesoscope/example_extract.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/mesoscope/example_platform.json` & `aind_metadata_mapper-0.6.5/tests/resources/mesoscope/example_platform.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/mesoscope/expected_session.json` & `aind_metadata_mapper-0.6.5/tests/resources/mesoscope/expected_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/neuropixels/base-missing-probe_rig.json` & `aind_metadata_mapper-0.6.5/tests/resources/neuropixels/base-missing-probe_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/neuropixels/base_rig.json` & `aind_metadata_mapper-0.6.5/tests/resources/neuropixels/base_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/neuropixels/mvr.ini` & `aind_metadata_mapper-0.6.5/tests/resources/neuropixels/mvr.ini`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/neuropixels/mvr_rig.json` & `aind_metadata_mapper-0.6.5/tests/resources/neuropixels/mvr_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/neuropixels/open-ephys-inferred_rig.json` & `aind_metadata_mapper-0.6.5/tests/resources/neuropixels/open-ephys-inferred_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/neuropixels/open-ephys_rig.json` & `aind_metadata_mapper-0.6.5/tests/resources/neuropixels/open-ephys_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/neuropixels/settings.mislabeled-probes-0.xml` & `aind_metadata_mapper-0.6.5/tests/resources/neuropixels/settings.mislabeled-probes-0.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/neuropixels/settings.mislabeled-probes-1.xml` & `aind_metadata_mapper-0.6.5/tests/resources/neuropixels/settings.mislabeled-probes-1.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/neuropixels/settings.xml` & `aind_metadata_mapper-0.6.5/tests/resources/neuropixels/settings.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/neuropixels/sync.yml` & `aind_metadata_mapper-0.6.5/tests/resources/neuropixels/sync.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/resources/neuropixels/sync_rig.json` & `aind_metadata_mapper-0.6.5/tests/resources/neuropixels/sync_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/test_bergamo.py` & `aind_metadata_mapper-0.6.5/tests/test_bergamo.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/test_ephys.py` & `aind_metadata_mapper-0.6.5/tests/test_ephys.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/test_fib.py` & `aind_metadata_mapper-0.6.5/tests/test_fib.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/test_gather_metadata.py` & `aind_metadata_mapper-0.6.5/tests/test_gather_metadata.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/test_legacy_core.py` & `aind_metadata_mapper-0.6.5/tests/test_legacy_core.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/test_mesoscope.py` & `aind_metadata_mapper-0.6.5/tests/test_mesoscope.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/test_neuropixels/test_mvr_rig.py` & `aind_metadata_mapper-0.6.5/tests/test_neuropixels/test_mvr_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/test_neuropixels/test_neuropixels_rig.py` & `aind_metadata_mapper-0.6.5/tests/test_neuropixels/test_neuropixels_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/test_neuropixels/test_open_ephys_rig.py` & `aind_metadata_mapper-0.6.5/tests/test_neuropixels/test_open_ephys_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/test_neuropixels/test_open_ephys_rig_inferrred.py` & `aind_metadata_mapper-0.6.5/tests/test_neuropixels/test_open_ephys_rig_inferrred.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/test_neuropixels/test_sync_rig.py` & `aind_metadata_mapper-0.6.5/tests/test_neuropixels/test_sync_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.4/tests/test_neuropixels/utils.py` & `aind_metadata_mapper-0.6.5/tests/test_neuropixels/utils.py`

 * *Files identical despite different names*


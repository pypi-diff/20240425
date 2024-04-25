# Comparing `tmp/telemetry_tempest_plugin-2.0.0.tar.gz` & `tmp/telemetry_tempest_plugin-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telemetry_tempest_plugin-2.0.0.tar", last modified: Fri Mar 22 17:36:01 2024, max compression
+gzip compressed data, was "telemetry_tempest_plugin-2.1.0.tar", last modified: Thu Apr 25 11:21:59 2024, max compression
```

## Comparing `telemetry_tempest_plugin-2.0.0.tar` & `telemetry_tempest_plugin-2.1.0.tar`

### file list

```diff
@@ -1,91 +1,93 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:36:01.811319 telemetry_tempest_plugin-2.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5263 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2337 2024-03-22 17:36:01.000000 telemetry_tempest_plugin-2.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      670 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8204 2024-03-22 17:36:01.000000 telemetry_tempest_plugin-2.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1419 2024-03-22 17:36:01.811319 telemetry_tempest_plugin-2.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:36:01.807319 telemetry_tempest_plugin-2.0.0/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/devstack/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:36:01.807319 telemetry_tempest_plugin-2.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:36:01.811319 telemetry_tempest_plugin-2.0.0/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2637 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/doc/source/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      415 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/doc/source/readme.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1048 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/doc/source/test_additions.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:36:01.811319 telemetry_tempest_plugin-2.0.0/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/playbooks/enable-fips.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:36:01.807319 telemetry_tempest_plugin-2.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:36:01.811319 telemetry_tempest_plugin-2.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/releasenotes/notes/drop-py-2-7-b86d74653b14779b.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:36:01.811319 telemetry_tempest_plugin-2.0.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:36:01.811319 telemetry_tempest_plugin-2.0.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:36:01.811319 telemetry_tempest_plugin-2.0.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9124 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2024-03-22 17:36:01.815319 telemetry_tempest_plugin-2.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:36:01.811319 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:36:01.811319 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:36:01.811319 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2140 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/api/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:36:01.811319 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/api/gnocchi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/api/gnocchi/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7084 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/api/gnocchi/test_alarming_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22170 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/api/gnocchi/test_alarming_api_negative.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:36:01.811319 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/api/prometheus/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/api/prometheus/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:36:01.811319 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/api/sql/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/api/sql/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4440 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/api/sql/test_alarming_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15801 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/api/test_alarming_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4466 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/api/test_alarming_api_negative.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:36:01.811319 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/service/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/service/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5978 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/service/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5720 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5320 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2503 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:36:01.811319 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/scenario/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:36:01.811319 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/scenario/gnocchi_gabbits/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23344 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/scenario/gnocchi_gabbits/live.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9570 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/scenario/gnocchi_gabbits/search-resource.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:36:01.811319 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/scenario/telemetry_integration_gabbits/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11464 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/scenario/telemetry_integration_gabbits/aodh-gnocchi-threshold-alarm.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4629 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/scenario/telemetry_integration_gabbits/autoscaling.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5136 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/scenario/telemetry_integration_gabbits/create_stack.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:36:01.811319 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/scenario/telemetry_integration_prometheus_gabbits/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/scenario/telemetry_integration_prometheus_gabbits/ceilometer-sg-core-integration.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1619 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/scenario/test_gnocchi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4461 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/scenario/test_telemetry_integration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1666 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/scenario/test_telemetry_integration_prometheus.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2814 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/scenario/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-22 17:36:01.811319 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1419 2024-03-22 17:36:01.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2679 2024-03-22 17:36:01.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-22 17:36:01.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2024-03-22 17:36:01.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-22 17:36:01.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-03-22 17:36:01.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2024-03-22 17:36:01.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2024-03-22 17:36:01.000000 telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1166 2024-03-22 17:35:37.000000 telemetry_tempest_plugin-2.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:59.140996 telemetry_tempest_plugin-2.1.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5316 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2368 2024-04-25 11:21:59.000000 telemetry_tempest_plugin-2.1.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      670 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8257 2024-04-25 11:21:58.000000 telemetry_tempest_plugin-2.1.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1419 2024-04-25 11:21:59.140996 telemetry_tempest_plugin-2.1.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:59.132996 telemetry_tempest_plugin-2.1.0/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/devstack/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:59.132996 telemetry_tempest_plugin-2.1.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:59.136996 telemetry_tempest_plugin-2.1.0/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2637 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/doc/source/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      415 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/doc/source/readme.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1048 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/doc/source/test_additions.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:59.136996 telemetry_tempest_plugin-2.1.0/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/playbooks/enable-fips.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:59.128996 telemetry_tempest_plugin-2.1.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:59.136996 telemetry_tempest_plugin-2.1.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/releasenotes/notes/drop-py-2-7-b86d74653b14779b.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:59.136996 telemetry_tempest_plugin-2.1.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:59.136996 telemetry_tempest_plugin-2.1.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:59.136996 telemetry_tempest_plugin-2.1.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9124 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2024-04-25 11:21:59.144996 telemetry_tempest_plugin-2.1.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:59.136996 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:59.136996 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:59.136996 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2140 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/api/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:59.140996 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/api/gnocchi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/api/gnocchi/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7084 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/api/gnocchi/test_alarming_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22170 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/api/gnocchi/test_alarming_api_negative.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:59.140996 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/api/prometheus/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/api/prometheus/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:59.140996 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/api/sql/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/api/sql/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4440 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/api/sql/test_alarming_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15801 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/api/test_alarming_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4466 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/api/test_alarming_api_negative.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:59.140996 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/service/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/service/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5978 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/service/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6001 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5320 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2503 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:59.140996 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:59.140996 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/gnocchi_gabbits/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23344 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/gnocchi_gabbits/live.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9570 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/gnocchi_gabbits/search-resource.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:59.140996 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/telemetry_integration_gabbits/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11464 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/telemetry_integration_gabbits/aodh-gnocchi-threshold-alarm.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4629 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/telemetry_integration_gabbits/autoscaling.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5136 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/telemetry_integration_gabbits/create_stack.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:59.140996 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/telemetry_integration_prometheus_gabbits/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4698 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/telemetry_integration_prometheus_gabbits/autoscaling.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/telemetry_integration_prometheus_gabbits/ceilometer-sg-core-integration.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3945 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/telemetry_integration_prometheus_gabbits/create_stack.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1619 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/test_gnocchi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4461 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/test_telemetry_integration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4541 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/test_telemetry_integration_prometheus.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2814 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:21:59.136996 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1419 2024-04-25 11:21:59.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2864 2024-04-25 11:21:59.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-25 11:21:59.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2024-04-25 11:21:59.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-25 11:21:59.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-04-25 11:21:59.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2024-04-25 11:21:59.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2024-04-25 11:21:59.000000 telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1166 2024-04-25 11:21:17.000000 telemetry_tempest_plugin-2.1.0/tox.ini
```

### Comparing `telemetry_tempest_plugin-2.0.0/.zuul.yaml` & `telemetry_tempest_plugin-2.1.0/.zuul.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         # the ceilometer devstack plugin doesn't support the CEILOMETER_BACKENDS,
         # it'll just ignore it and use the CEILOMETER_BACKEND. In versions, where
         # CEILOMETER_BACKENDS is supported, the ceilometer devstack plugin will
         # just try to merge the variables, so the final contents in this casse will
         # be "gnocchi,sg-core"
         CEILOMETER_BACKEND: "gnocchi"
         CEILOMETER_BACKENDS: "gnocchi,sg-core"
+        PROMETHEUS_SERVICE_SCRAPE_TARGETS: "sg-core"
         CEILOMETER_PIPELINE_INTERVAL: 15
         CEILOMETER_ALARM_THRESHOLD: 6000000000
         GLOBAL_VENV: False
       devstack_local_conf:
         test-config:
           $TEMPEST_CONFIG:
             service_available:
```

### Comparing `telemetry_tempest_plugin-2.0.0/AUTHORS` & `telemetry_tempest_plugin-2.1.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 ghanshyam <ghanshyammann@gmail.com>
 gord chung <gord@live.ca>
 gordon chung <gord@live.ca>
 huang.zhiping <huang.zhiping@99cloud.net>
 inspurericzhang <zhanglf01@inspur.com>
 liusheng <liusheng@huawei.com>
 maaoyu <maaoyu@inspur.com>
+mgirgisf <mgirgisf@redhat.com>
 pengyuesheng <pengyuesheng@gohighsec.com>
 qingszhao <zhao.daqing@99cloud.net>
 ricolin <ricolin@ricolky.com>
 wangjiaqi07 <wangjiaqi07@inspur.com>
 yatin <ykarel@redhat.com>
 zhangboye <zhangboye@inspur.com>
 zhufl <zhu.fanglei@zte.com.cn>
```

### Comparing `telemetry_tempest_plugin-2.0.0/CONTRIBUTING.rst` & `telemetry_tempest_plugin-2.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/ChangeLog` & `telemetry_tempest_plugin-2.1.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+2.1.0
+-----
+
+* Add Autoscaling test with prometheus
+
 2.0.0
 -----
 
 * Make regex for excluding tests more specific
 * Revert "Make centos 9 stream jobs non-voting"
 * Fix sg-core test scenario
 * Drop dib-utils
```

### Comparing `telemetry_tempest_plugin-2.0.0/LICENSE` & `telemetry_tempest_plugin-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/PKG-INFO` & `telemetry_tempest_plugin-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: telemetry_tempest_plugin
-Version: 2.0.0
+Version: 2.1.0
 Summary: Tempest plugin for Telemetry Projects
 Home-page: https://www.openstack.org/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Telemetry Tempest Plugin
```

### Comparing `telemetry_tempest_plugin-2.0.0/devstack/README.rst` & `telemetry_tempest_plugin-2.1.0/devstack/README.rst`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/doc/source/conf.py` & `telemetry_tempest_plugin-2.1.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/doc/source/index.rst` & `telemetry_tempest_plugin-2.1.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/doc/source/test_additions.rst` & `telemetry_tempest_plugin-2.1.0/doc/source/test_additions.rst`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/releasenotes/source/conf.py` & `telemetry_tempest_plugin-2.1.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/setup.cfg` & `telemetry_tempest_plugin-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/setup.py` & `telemetry_tempest_plugin-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/api/base.py` & `telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/api/base.py`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/api/gnocchi/test_alarming_api.py` & `telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/api/gnocchi/test_alarming_api.py`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/api/gnocchi/test_alarming_api_negative.py` & `telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/api/gnocchi/test_alarming_api_negative.py`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/api/sql/test_alarming_api.py` & `telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/api/sql/test_alarming_api.py`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/api/test_alarming_api.py` & `telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/api/test_alarming_api.py`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/api/test_alarming_api_negative.py` & `telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/api/test_alarming_api_negative.py`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/aodh/service/client.py` & `telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/aodh/service/client.py`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/config.py` & `telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,21 +72,27 @@
                help="Name of the metric to create an alarm on."),
     cfg.StrOpt('alarm_aggregation_method',
                default="rate:mean",
                help="Aggregation method to use for alarm."),
     cfg.IntOpt('alarm_threshold',
                default=10,
                help="Threshold to cross for the alarm to trigger."),
+    cfg.IntOpt('scaledown_alarm_threshold',
+               default=2000000000,
+               help="Threshold to cross for the alarm to trigger."),
     cfg.BoolOpt("disable_ssl_certificate_validation",
                 default=False,
                 help="Disable SSL certificate validation when running "
                      "scenario tests"),
     cfg.StrOpt('sg_core_service_url',
                default="127.0.0.1:3000",
                help="URL to sg-core prometheus endpoint"),
+    cfg.StrOpt('prometheus_service_url',
+               default="127.0.0.1:9090",
+               help="URL to prometheus endpoint"),
     cfg.IntOpt('ceilometer_polling_interval',
                default=300,
                help="Polling interval configured for ceilometer. This can "
                     "be used in test cases to wait for metrics to appear.")
 ]
 
 telemetry_services_opts = [
```

### Comparing `telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/exceptions.py` & `telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/exceptions.py`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/plugin.py` & `telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/scenario/gnocchi_gabbits/live.yaml` & `telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/gnocchi_gabbits/live.yaml`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/scenario/gnocchi_gabbits/search-resource.yaml` & `telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/gnocchi_gabbits/search-resource.yaml`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/scenario/telemetry_integration_gabbits/aodh-gnocchi-threshold-alarm.yaml` & `telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/telemetry_integration_gabbits/aodh-gnocchi-threshold-alarm.yaml`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/scenario/telemetry_integration_gabbits/autoscaling.yaml` & `telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/telemetry_integration_gabbits/autoscaling.yaml`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/scenario/telemetry_integration_gabbits/create_stack.json` & `telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/telemetry_integration_gabbits/create_stack.json`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/scenario/test_gnocchi.py` & `telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/test_gnocchi.py`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/scenario/test_telemetry_integration.py` & `telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/test_telemetry_integration.py`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin/scenario/utils.py` & `telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin/scenario/utils.py`

 * *Files identical despite different names*

### Comparing `telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin.egg-info/PKG-INFO` & `telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: telemetry-tempest-plugin
-Version: 2.0.0
+Version: 2.1.0
 Summary: Tempest plugin for Telemetry Projects
 Home-page: https://www.openstack.org/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Telemetry Tempest Plugin
```

### Comparing `telemetry_tempest_plugin-2.0.0/telemetry_tempest_plugin.egg-info/SOURCES.txt` & `telemetry_tempest_plugin-2.1.0/telemetry_tempest_plugin.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -61,8 +61,10 @@
 telemetry_tempest_plugin/scenario/test_telemetry_integration_prometheus.py
 telemetry_tempest_plugin/scenario/utils.py
 telemetry_tempest_plugin/scenario/gnocchi_gabbits/live.yaml
 telemetry_tempest_plugin/scenario/gnocchi_gabbits/search-resource.yaml
 telemetry_tempest_plugin/scenario/telemetry_integration_gabbits/aodh-gnocchi-threshold-alarm.yaml
 telemetry_tempest_plugin/scenario/telemetry_integration_gabbits/autoscaling.yaml
 telemetry_tempest_plugin/scenario/telemetry_integration_gabbits/create_stack.json
-telemetry_tempest_plugin/scenario/telemetry_integration_prometheus_gabbits/ceilometer-sg-core-integration.yaml
+telemetry_tempest_plugin/scenario/telemetry_integration_prometheus_gabbits/autoscaling.yaml
+telemetry_tempest_plugin/scenario/telemetry_integration_prometheus_gabbits/ceilometer-sg-core-integration.yaml
+telemetry_tempest_plugin/scenario/telemetry_integration_prometheus_gabbits/create_stack.json
```

### Comparing `telemetry_tempest_plugin-2.0.0/tox.ini` & `telemetry_tempest_plugin-2.1.0/tox.ini`

 * *Files identical despite different names*


# Comparing `tmp/python-observabilityclient-0.1.1.tar.gz` & `tmp/python-observabilityclient-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-observabilityclient-0.1.1.tar", last modified: Mon Jan 15 13:27:34 2024, max compression
+gzip compressed data, was "python-observabilityclient-0.2.0.tar", last modified: Thu Apr 25 11:19:56 2024, max compression
```

## Comparing `python-observabilityclient-0.1.1.tar` & `python-observabilityclient-0.2.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:27:34.045104 python-observabilityclient-0.1.1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2332 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2024-01-15 13:27:33.000000 python-observabilityclient-0.1.1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2024-01-15 13:27:33.000000 python-observabilityclient-0.1.1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11343 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3296 2024-01-15 13:27:34.045104 python-observabilityclient-0.1.1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1719 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:27:34.041104 python-observabilityclient-0.1.1/observabilityclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/observabilityclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      828 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/observabilityclient/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      790 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/observabilityclient/i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2262 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/observabilityclient/plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7093 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/observabilityclient/prometheus_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:27:34.037104 python-observabilityclient-0.1.1/observabilityclient/tests/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:27:34.041104 python-observabilityclient-0.1.1/observabilityclient/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/observabilityclient/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6523 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/observabilityclient/tests/functional/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4856 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/observabilityclient/tests/functional/test_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3310 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/observabilityclient/tests/functional/test_python_api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:27:34.041104 python-observabilityclient-0.1.1/observabilityclient/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/observabilityclient/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5964 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/observabilityclient/tests/unit/test_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18801 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/observabilityclient/tests/unit/test_prometheus_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4760 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/observabilityclient/tests/unit/test_python_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5692 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/observabilityclient/tests/unit/test_rbac.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5370 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/observabilityclient/tests/unit/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:27:34.041104 python-observabilityclient-0.1.1/observabilityclient/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/observabilityclient/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3153 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/observabilityclient/utils/metric_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:27:34.045104 python-observabilityclient-0.1.1/observabilityclient/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/observabilityclient/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2556 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/observabilityclient/v1/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4028 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/observabilityclient/v1/cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1643 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/observabilityclient/v1/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3916 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/observabilityclient/v1/python_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6115 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/observabilityclient/v1/rbac.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/pyproject.toml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:27:34.045104 python-observabilityclient-0.1.1/python_observabilityclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3296 2024-01-15 13:27:33.000000 python-observabilityclient-0.1.1/python_observabilityclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1487 2024-01-15 13:27:34.000000 python-observabilityclient-0.1.1/python_observabilityclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-01-15 13:27:33.000000 python-observabilityclient-0.1.1/python_observabilityclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2024-01-15 13:27:33.000000 python-observabilityclient-0.1.1/python_observabilityclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-01-15 13:27:33.000000 python-observabilityclient-0.1.1/python_observabilityclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-01-15 13:27:33.000000 python-observabilityclient-0.1.1/python_observabilityclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2024-01-15 13:27:33.000000 python-observabilityclient-0.1.1/python_observabilityclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2024-01-15 13:27:33.000000 python-observabilityclient-0.1.1/python_observabilityclient.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1866 2024-01-15 13:27:34.045104 python-observabilityclient-0.1.1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:27:34.045104 python-observabilityclient-0.1.1/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1529 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/tools/fix_ca_bundle.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      593 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/tools/install_deps.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2540 2024-01-15 13:27:01.000000 python-observabilityclient-0.1.1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:56.985143 python-observabilityclient-0.2.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2332 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      393 2024-04-25 11:19:56.000000 python-observabilityclient-0.2.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      851 2024-04-25 11:19:56.000000 python-observabilityclient-0.2.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11343 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3296 2024-04-25 11:19:56.985143 python-observabilityclient-0.2.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1719 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:56.981143 python-observabilityclient-0.2.0/observabilityclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/observabilityclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      828 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/observabilityclient/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      790 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/observabilityclient/i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2262 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/observabilityclient/plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7467 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/observabilityclient/prometheus_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:56.981143 python-observabilityclient-0.2.0/observabilityclient/tests/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:56.981143 python-observabilityclient-0.2.0/observabilityclient/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/observabilityclient/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6523 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/observabilityclient/tests/functional/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4856 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/observabilityclient/tests/functional/test_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3310 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/observabilityclient/tests/functional/test_python_api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:56.985143 python-observabilityclient-0.2.0/observabilityclient/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/observabilityclient/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5964 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/observabilityclient/tests/unit/test_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18801 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/observabilityclient/tests/unit/test_prometheus_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4760 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/observabilityclient/tests/unit/test_python_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5692 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/observabilityclient/tests/unit/test_rbac.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7387 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/observabilityclient/tests/unit/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:56.985143 python-observabilityclient-0.2.0/observabilityclient/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/observabilityclient/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3425 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/observabilityclient/utils/metric_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:56.985143 python-observabilityclient-0.2.0/observabilityclient/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/observabilityclient/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2556 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/observabilityclient/v1/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4028 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/observabilityclient/v1/cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1643 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/observabilityclient/v1/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3916 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/observabilityclient/v1/python_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6115 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/observabilityclient/v1/rbac.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/pyproject.toml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:56.985143 python-observabilityclient-0.2.0/python_observabilityclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3296 2024-04-25 11:19:56.000000 python-observabilityclient-0.2.0/python_observabilityclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1487 2024-04-25 11:19:56.000000 python-observabilityclient-0.2.0/python_observabilityclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-25 11:19:56.000000 python-observabilityclient-0.2.0/python_observabilityclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2024-04-25 11:19:56.000000 python-observabilityclient-0.2.0/python_observabilityclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-25 11:19:56.000000 python-observabilityclient-0.2.0/python_observabilityclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-04-25 11:19:56.000000 python-observabilityclient-0.2.0/python_observabilityclient.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2024-04-25 11:19:56.000000 python-observabilityclient-0.2.0/python_observabilityclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2024-04-25 11:19:56.000000 python-observabilityclient-0.2.0/python_observabilityclient.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1866 2024-04-25 11:19:56.985143 python-observabilityclient-0.2.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:56.985143 python-observabilityclient-0.2.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1529 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/tools/fix_ca_bundle.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      593 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/tools/install_deps.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2540 2024-04-25 11:19:28.000000 python-observabilityclient-0.2.0/tox.ini
```

### Comparing `python-observabilityclient-0.1.1/.zuul.yaml` & `python-observabilityclient-0.2.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `python-observabilityclient-0.1.1/ChangeLog` & `python-observabilityclient-0.2.0/ChangeLog`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+0.2.0
+-----
+
+* Sort column order in cli output
+* Fix table formatter
+* Remove AUTHORS file
+* Add TLS support
+
 0.1.1
 -----
 
 * Update python classifier in setup.cfg
 * Add functional tests
 * Fix cli commands
 * Add i18n.py and use it in v1/base.py and v1/cli.py
```

### Comparing `python-observabilityclient-0.1.1/LICENSE` & `python-observabilityclient-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-observabilityclient-0.1.1/PKG-INFO` & `python-observabilityclient-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-observabilityclient
-Version: 0.1.1
+Version: 0.2.0
 Summary: OpenStack Observability Client
 Home-page: https://infrawatch.github.io/documentation/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License, Version 2.0
 Description: # python-observabilityclient
```

### Comparing `python-observabilityclient-0.1.1/README.md` & `python-observabilityclient-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `python-observabilityclient-0.1.1/observabilityclient/client.py` & `python-observabilityclient-0.2.0/observabilityclient/client.py`

 * *Files identical despite different names*

### Comparing `python-observabilityclient-0.1.1/observabilityclient/i18n.py` & `python-observabilityclient-0.2.0/observabilityclient/i18n.py`

 * *Files identical despite different names*

### Comparing `python-observabilityclient-0.1.1/observabilityclient/plugin.py` & `python-observabilityclient-0.2.0/observabilityclient/plugin.py`

 * *Files identical despite different names*

### Comparing `python-observabilityclient-0.1.1/observabilityclient/prometheus_client.py` & `python-observabilityclient-0.2.0/observabilityclient/prometheus_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,29 +11,36 @@
 #   WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #   License for the specific language governing permissions and limitations
 #   under the License.
 
 import logging
 
 import requests
+import simplejson
 
 
 LOG = logging.getLogger(__name__)
 
 
 class PrometheusAPIClientError(Exception):
     def __init__(self, response):
         self.resp = response
 
     def __str__(self) -> str:
         if self.resp.status_code != requests.codes.ok:
             if self.resp.status_code != 204:
-                decoded = self.resp.json()
-                if 'error' in decoded:
-                    return f'[{self.resp.status_code}] {decoded["error"]}'
+                try:
+                    decoded = self.resp.json()
+                    if 'error' in decoded:
+                        return f'[{self.resp.status_code}] {decoded["error"]}'
+                except simplejson.errors.JSONDecodeError:
+                    # If an https endpoint is accessed as http,
+                    # we get 400 status with plain text instead of
+                    # json and decoding it raises exception.
+                    return f'[{self.resp.status_code}] {self.resp.text}'
             return f'[{self.resp.status_code}] {self.resp.reason}'
         else:
             decoded = self.resp.json()
             return f'[{decoded.status}]'
 
     def __repr__(self) -> str:
         if self.resp.status_code != requests.codes.ok:
```

### Comparing `python-observabilityclient-0.1.1/observabilityclient/tests/functional/base.py` & `python-observabilityclient-0.2.0/observabilityclient/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `python-observabilityclient-0.1.1/observabilityclient/tests/functional/test_cli.py` & `python-observabilityclient-0.2.0/observabilityclient/tests/functional/test_cli.py`

 * *Files identical despite different names*

### Comparing `python-observabilityclient-0.1.1/observabilityclient/tests/functional/test_python_api.py` & `python-observabilityclient-0.2.0/observabilityclient/tests/functional/test_python_api.py`

 * *Files identical despite different names*

### Comparing `python-observabilityclient-0.1.1/observabilityclient/tests/unit/test_cli.py` & `python-observabilityclient-0.2.0/observabilityclient/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `python-observabilityclient-0.1.1/observabilityclient/tests/unit/test_prometheus_client.py` & `python-observabilityclient-0.2.0/observabilityclient/tests/unit/test_prometheus_client.py`

 * *Files identical despite different names*

### Comparing `python-observabilityclient-0.1.1/observabilityclient/tests/unit/test_python_api.py` & `python-observabilityclient-0.2.0/observabilityclient/tests/unit/test_python_api.py`

 * *Files identical despite different names*

### Comparing `python-observabilityclient-0.1.1/observabilityclient/tests/unit/test_rbac.py` & `python-observabilityclient-0.2.0/observabilityclient/tests/unit/test_rbac.py`

 * *Files identical despite different names*

### Comparing `python-observabilityclient-0.1.1/observabilityclient/utils/metric_utils.py` & `python-observabilityclient-0.2.0/observabilityclient/utils/metric_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -41,33 +41,41 @@
             return open(full_filename, "r")
     return None
 
 
 def get_prometheus_client():
     host = None
     port = None
+    ca_cert = None
     conf_file = get_config_file()
     if conf_file is not None:
         conf = yaml.safe_load(conf_file)
         if 'host' in conf:
             host = conf['host']
         if 'port' in conf:
             port = conf['port']
+        if 'ca_cert' in conf:
+            ca_cert = conf['ca_cert']
         conf_file.close()
 
     # NOTE(jwysogla): We allow to overide the prometheus.yaml by
     #                 the environment variables
     if 'PROMETHEUS_HOST' in os.environ:
         host = os.environ['PROMETHEUS_HOST']
     if 'PROMETHEUS_PORT' in os.environ:
         port = os.environ['PROMETHEUS_PORT']
+    if 'PROMETHEUS_CA_CERT' in os.environ:
+        ca_cert = os.environ['PROMETHEUS_CA_CERT']
     if host is None or port is None:
         raise ConfigurationError("Can't find prometheus host and "
                                  "port configuration.")
-    return PrometheusAPIClient(f"{host}:{port}")
+    client = PrometheusAPIClient(f"{host}:{port}")
+    if ca_cert is not None:
+        client.set_ca_cert(ca_cert)
+    return client
 
 
 def get_client(obj):
     return obj.app.client_manager.observabilityclient
 
 
 def format_labels(d: dict) -> str:
@@ -86,22 +94,19 @@
     while ret != old:
         old = ret
         ret = replace_doubled_quotes(ret)
     return ret
 
 
 def metrics2cols(m):
-    cols = []
+    # get all label keys
+    cols = list(set().union(*(d.labels.keys() for d in m)))
+    cols.sort()
+    cols.append("value")
     fields = []
-    first = True
     for metric in m:
-        row = []
+        row = [""] * len(cols)
         for key, value in metric.labels.items():
-            if first:
-                cols.append(key)
-            row.append(value)
-        if first:
-            cols.append("value")
-        row.append(metric.value)
+            row[cols.index(key)] = value
+        row[cols.index("value")] = metric.value
         fields.append(row)
-        first = False
     return cols, fields
```

### Comparing `python-observabilityclient-0.1.1/observabilityclient/v1/base.py` & `python-observabilityclient-0.2.0/observabilityclient/v1/base.py`

 * *Files identical despite different names*

### Comparing `python-observabilityclient-0.1.1/observabilityclient/v1/cli.py` & `python-observabilityclient-0.2.0/observabilityclient/v1/cli.py`

 * *Files identical despite different names*

### Comparing `python-observabilityclient-0.1.1/observabilityclient/v1/client.py` & `python-observabilityclient-0.2.0/observabilityclient/v1/client.py`

 * *Files identical despite different names*

### Comparing `python-observabilityclient-0.1.1/observabilityclient/v1/python_api.py` & `python-observabilityclient-0.2.0/observabilityclient/v1/python_api.py`

 * *Files identical despite different names*

### Comparing `python-observabilityclient-0.1.1/observabilityclient/v1/rbac.py` & `python-observabilityclient-0.2.0/observabilityclient/v1/rbac.py`

 * *Files identical despite different names*

### Comparing `python-observabilityclient-0.1.1/python_observabilityclient.egg-info/PKG-INFO` & `python-observabilityclient-0.2.0/python_observabilityclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-observabilityclient
-Version: 0.1.1
+Version: 0.2.0
 Summary: OpenStack Observability Client
 Home-page: https://infrawatch.github.io/documentation/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License, Version 2.0
 Description: # python-observabilityclient
```

### Comparing `python-observabilityclient-0.1.1/python_observabilityclient.egg-info/SOURCES.txt` & `python-observabilityclient-0.2.0/python_observabilityclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-observabilityclient-0.1.1/setup.cfg` & `python-observabilityclient-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-observabilityclient-0.1.1/setup.py` & `python-observabilityclient-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-observabilityclient-0.1.1/tools/fix_ca_bundle.sh` & `python-observabilityclient-0.2.0/tools/fix_ca_bundle.sh`

 * *Files identical despite different names*

### Comparing `python-observabilityclient-0.1.1/tools/install_deps.sh` & `python-observabilityclient-0.2.0/tools/install_deps.sh`

 * *Files identical despite different names*

### Comparing `python-observabilityclient-0.1.1/tox.ini` & `python-observabilityclient-0.2.0/tox.ini`

 * *Files identical despite different names*


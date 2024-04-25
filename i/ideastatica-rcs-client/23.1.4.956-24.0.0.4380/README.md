# Comparing `tmp/ideastatica_rcs_client-23.1.4.956.tar.gz` & `tmp/ideastatica_rcs_client-24.0.0.4380.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ideastatica_rcs_client-23.1.4.956.tar", last modified: Thu Feb  1 21:41:08 2024, max compression
+gzip compressed data, was "ideastatica_rcs_client-24.0.0.4380.tar", last modified: Thu Apr 25 07:45:59 2024, max compression
```

## Comparing `ideastatica_rcs_client-23.1.4.956.tar` & `ideastatica_rcs_client-24.0.0.4380.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:41:08.413580 ideastatica_rcs_client-23.1.4.956/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-01 21:41:00.000000 ideastatica_rcs_client-23.1.4.956/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-01 21:41:08.413580 ideastatica_rcs_client-23.1.4.956/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-02-01 21:41:00.000000 ideastatica_rcs_client-23.1.4.956/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:41:08.409580 ideastatica_rcs_client-23.1.4.956/ideastatica_rcs_client/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-01 21:41:00.000000 ideastatica_rcs_client-23.1.4.956/ideastatica_rcs_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-02-01 21:41:00.000000 ideastatica_rcs_client-23.1.4.956/ideastatica_rcs_client/brief_result_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-02-01 21:41:00.000000 ideastatica_rcs_client-23.1.4.956/ideastatica_rcs_client/detail_results_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-02-01 21:41:00.000000 ideastatica_rcs_client-23.1.4.956/ideastatica_rcs_client/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-02-01 21:41:00.000000 ideastatica_rcs_client-23.1.4.956/ideastatica_rcs_client/idea_statica_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-02-01 21:41:00.000000 ideastatica_rcs_client-23.1.4.956/ideastatica_rcs_client/ideastatica_rcs_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-01 21:41:00.000000 ideastatica_rcs_client-23.1.4.956/ideastatica_rcs_client/loading_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-02-01 21:41:00.000000 ideastatica_rcs_client-23.1.4.956/ideastatica_rcs_client/rcsproject.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:41:08.413580 ideastatica_rcs_client-23.1.4.956/ideastatica_rcs_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-01 21:41:08.000000 ideastatica_rcs_client-23.1.4.956/ideastatica_rcs_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-02-01 21:41:08.000000 ideastatica_rcs_client-23.1.4.956/ideastatica_rcs_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 21:41:08.000000 ideastatica_rcs_client-23.1.4.956/ideastatica_rcs_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-01 21:41:08.000000 ideastatica_rcs_client-23.1.4.956/ideastatica_rcs_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-02-01 21:41:00.000000 ideastatica_rcs_client-23.1.4.956/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-01 21:41:08.413580 ideastatica_rcs_client-23.1.4.956/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-01 21:41:00.000000 ideastatica_rcs_client-23.1.4.956/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:45:59.706339 ideastatica_rcs_client-24.0.0.4380/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-25 07:45:49.000000 ideastatica_rcs_client-24.0.0.4380/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-25 07:45:59.706339 ideastatica_rcs_client-24.0.0.4380/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-25 07:45:49.000000 ideastatica_rcs_client-24.0.0.4380/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:45:59.706339 ideastatica_rcs_client-24.0.0.4380/ideastatica_rcs_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 07:45:49.000000 ideastatica_rcs_client-24.0.0.4380/ideastatica_rcs_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-25 07:45:49.000000 ideastatica_rcs_client-24.0.0.4380/ideastatica_rcs_client/brief_result_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-25 07:45:49.000000 ideastatica_rcs_client-24.0.0.4380/ideastatica_rcs_client/detail_results_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-25 07:45:49.000000 ideastatica_rcs_client-24.0.0.4380/ideastatica_rcs_client/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-25 07:45:49.000000 ideastatica_rcs_client-24.0.0.4380/ideastatica_rcs_client/idea_statica_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-25 07:45:49.000000 ideastatica_rcs_client-24.0.0.4380/ideastatica_rcs_client/loading_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-04-25 07:45:49.000000 ideastatica_rcs_client-24.0.0.4380/ideastatica_rcs_client/rcs_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-25 07:45:49.000000 ideastatica_rcs_client-24.0.0.4380/ideastatica_rcs_client/rcsproject.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:45:59.706339 ideastatica_rcs_client-24.0.0.4380/ideastatica_rcs_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-25 07:45:59.000000 ideastatica_rcs_client-24.0.0.4380/ideastatica_rcs_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-25 07:45:59.000000 ideastatica_rcs_client-24.0.0.4380/ideastatica_rcs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:45:59.000000 ideastatica_rcs_client-24.0.0.4380/ideastatica_rcs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-25 07:45:59.000000 ideastatica_rcs_client-24.0.0.4380/ideastatica_rcs_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-25 07:45:49.000000 ideastatica_rcs_client-24.0.0.4380/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 07:45:59.706339 ideastatica_rcs_client-24.0.0.4380/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-25 07:45:49.000000 ideastatica_rcs_client-24.0.0.4380/setup.py
```

### Comparing `ideastatica_rcs_client-23.1.4.956/LICENSE` & `ideastatica_rcs_client-24.0.0.4380/LICENSE`

 * *Files identical despite different names*

### Comparing `ideastatica_rcs_client-23.1.4.956/ideastatica_rcs_client/brief_result_tools.py` & `ideastatica_rcs_client-24.0.0.4380/ideastatica_rcs_client/brief_result_tools.py`

 * *Files identical despite different names*

### Comparing `ideastatica_rcs_client-23.1.4.956/ideastatica_rcs_client/detail_results_tools.py` & `ideastatica_rcs_client-24.0.0.4380/ideastatica_rcs_client/detail_results_tools.py`

 * *Files identical despite different names*

### Comparing `ideastatica_rcs_client-23.1.4.956/ideastatica_rcs_client/idea_statica_setup.py` & `ideastatica_rcs_client-24.0.0.4380/ideastatica_rcs_client/idea_statica_setup.py`

 * *Files identical despite different names*

### Comparing `ideastatica_rcs_client-23.1.4.956/ideastatica_rcs_client/loading_tools.py` & `ideastatica_rcs_client-24.0.0.4380/ideastatica_rcs_client/loading_tools.py`

 * *Files identical despite different names*

### Comparing `ideastatica_rcs_client-23.1.4.956/ideastatica_rcs_client/rcsproject.py` & `ideastatica_rcs_client-24.0.0.4380/ideastatica_rcs_client/rcsproject.py`

 * *Files identical despite different names*

### Comparing `ideastatica_rcs_client-23.1.4.956/ideastatica_rcs_client.egg-info/SOURCES.txt` & `ideastatica_rcs_client-24.0.0.4380/ideastatica_rcs_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 pyproject.toml
 setup.py
 ideastatica_rcs_client/__init__.py
 ideastatica_rcs_client/brief_result_tools.py
 ideastatica_rcs_client/detail_results_tools.py
 ideastatica_rcs_client/helpers.py
 ideastatica_rcs_client/idea_statica_setup.py
-ideastatica_rcs_client/ideastatica_rcs_client.py
 ideastatica_rcs_client/loading_tools.py
+ideastatica_rcs_client/rcs_client.py
 ideastatica_rcs_client/rcsproject.py
 ideastatica_rcs_client.egg-info/PKG-INFO
 ideastatica_rcs_client.egg-info/SOURCES.txt
 ideastatica_rcs_client.egg-info/dependency_links.txt
 ideastatica_rcs_client.egg-info/top_level.txt
```

### Comparing `ideastatica_rcs_client-23.1.4.956/pyproject.toml` & `ideastatica_rcs_client-24.0.0.4380/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ideastatica_rcs_client"
-version = "23.1.4.0956"
+version = "24.0.0.4380"
 authors = [
   { name="Martin Pospisil", email="martin.pospisil@ideastatica.com" },
 ]
 description = "IDEA StatiCa RCS client fo Python"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```


# Comparing `tmp/ad_sdl_wei-0.5.7.tar.gz` & `tmp/ad_sdl_wei-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ad_sdl_wei-0.5.7.tar", last modified: Wed Apr 17 20:08:20 2024, max compression
+gzip compressed data, was "ad_sdl_wei-0.5.8.tar", last modified: Thu Apr 25 15:54:54 2024, max compression
```

## Comparing `ad_sdl_wei-0.5.7.tar` & `ad_sdl_wei-0.5.8.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:08:20.085303 ad_sdl_wei-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-17 20:08:20.085303 ad_sdl_wei-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:08:20.081303 ad_sdl_wei-0.5.7/ad_sdl.wei.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-17 20:08:20.000000 ad_sdl_wei-0.5.7/ad_sdl.wei.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-17 20:08:20.000000 ad_sdl_wei-0.5.7/ad_sdl.wei.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:08:20.000000 ad_sdl_wei-0.5.7/ad_sdl.wei.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-17 20:08:20.000000 ad_sdl_wei-0.5.7/ad_sdl.wei.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-17 20:08:20.000000 ad_sdl_wei-0.5.7/ad_sdl.wei.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 20:08:20.085303 ad_sdl_wei-0.5.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:08:20.073303 ad_sdl_wei-0.5.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/tests/test_wei_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/tests/test_workcell.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/tests/test_workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:08:20.077303 ad_sdl_wei-0.5.7/wei/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:08:20.077303 ad_sdl_wei-0.5.7/wei/core/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    17284 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11112 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:08:20.081303 ad_sdl_wei-0.5.7/wei/core/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/interfaces/rest_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/interfaces/ros2_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/interfaces/simulate_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/interfaces/tcp_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/interfaces/zmq_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8547 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/state_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/workcell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    12557 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/experiment_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:08:20.081303 ad_sdl_wei-0.5.7/wei/routers/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/routers/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/routers/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/routers/experiments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/routers/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/routers/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/routers/workcells.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/routers/workflow_runs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:54:54.856871 ad_sdl_wei-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-25 15:54:54.856871 ad_sdl_wei-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:54:54.852872 ad_sdl_wei-0.5.8/ad_sdl.wei.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-25 15:54:54.000000 ad_sdl_wei-0.5.8/ad_sdl.wei.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-25 15:54:54.000000 ad_sdl_wei-0.5.8/ad_sdl.wei.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:54:54.000000 ad_sdl_wei-0.5.8/ad_sdl.wei.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-25 15:54:54.000000 ad_sdl_wei-0.5.8/ad_sdl.wei.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-25 15:54:54.000000 ad_sdl_wei-0.5.8/ad_sdl.wei.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:54:54.856871 ad_sdl_wei-0.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:54:54.848871 ad_sdl_wei-0.5.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/tests/test_wei_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/tests/test_workcell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/tests/test_workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:54:54.848871 ad_sdl_wei-0.5.8/wei/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:54:54.848871 ad_sdl_wei-0.5.8/wei/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/core/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17284 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/core/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11112 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/core/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/core/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:54:54.852872 ad_sdl_wei-0.5.8/wei/core/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/core/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/core/interfaces/rest_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/core/interfaces/ros2_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/core/interfaces/simulate_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/core/interfaces/tcp_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/core/interfaces/zmq_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/core/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/core/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/core/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/core/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8547 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/core/state_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/core/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/core/workcell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/core/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12557 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/experiment_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:54:54.852872 ad_sdl_wei-0.5.8/wei/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/routers/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/routers/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/routers/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/routers/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/routers/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/routers/workcells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/routers/workflow_runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-25 15:54:17.000000 ad_sdl_wei-0.5.8/wei/server.py
```

### Comparing `ad_sdl_wei-0.5.7/LICENSE` & `ad_sdl_wei-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/PKG-INFO` & `ad_sdl_wei-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ad_sdl.wei
-Version: 0.5.7
+Version: 0.5.8
 Summary: The Rapid Prototyping Laboratory's Workflow Execution Interface.
 Author-email: Rafael Vescovi <ravescovi@anl.gov>, Tobias Ginsburg <tginsburg@anl.gov>, "Ryan D. Lewis" <ryan.lewis@anl.gov>, Casey Stone <cstone@anl.gov>, Doga Ozgulbas <dozgulbas@anl.gov>, Kyle Hippe <khippe@anl.gov>
 License: MIT
 Project-URL: Homepage, https://github.com/AD-SDL/wei
 Project-URL: Downloads, https://github.com/AD-SDL/wei/archive/refs/tags/0.5.1.tar.gz
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
```

### Comparing `ad_sdl_wei-0.5.7/README.md` & `ad_sdl_wei-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/ad_sdl.wei.egg-info/PKG-INFO` & `ad_sdl_wei-0.5.8/ad_sdl.wei.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ad_sdl.wei
-Version: 0.5.7
+Version: 0.5.8
 Summary: The Rapid Prototyping Laboratory's Workflow Execution Interface.
 Author-email: Rafael Vescovi <ravescovi@anl.gov>, Tobias Ginsburg <tginsburg@anl.gov>, "Ryan D. Lewis" <ryan.lewis@anl.gov>, Casey Stone <cstone@anl.gov>, Doga Ozgulbas <dozgulbas@anl.gov>, Kyle Hippe <khippe@anl.gov>
 License: MIT
 Project-URL: Homepage, https://github.com/AD-SDL/wei
 Project-URL: Downloads, https://github.com/AD-SDL/wei/archive/refs/tags/0.5.1.tar.gz
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
```

### Comparing `ad_sdl_wei-0.5.7/ad_sdl.wei.egg-info/SOURCES.txt` & `ad_sdl_wei-0.5.8/ad_sdl.wei.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/pyproject.toml` & `ad_sdl_wei-0.5.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ad_sdl.wei"
-version = "0.5.7"
+version = "0.5.8"
 description = "The Rapid Prototyping Laboratory's Workflow Execution Interface."
 authors = [
     {name = "Rafael Vescovi", email = "ravescovi@anl.gov"},
     {name = "Tobias Ginsburg", email = "tginsburg@anl.gov"},
     {name = "Ryan D. Lewis", email = "ryan.lewis@anl.gov"},
     {name = "Casey Stone", email = "cstone@anl.gov"},
     {name = "Doga Ozgulbas", email = "dozgulbas@anl.gov"},
```

### Comparing `ad_sdl_wei-0.5.7/tests/test_base.py` & `ad_sdl_wei-0.5.8/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/tests/test_wei_locations.py` & `ad_sdl_wei-0.5.8/tests/test_wei_locations.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/tests/test_workcell.py` & `ad_sdl_wei-0.5.8/tests/test_workcell.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/tests/test_workflows.py` & `ad_sdl_wei-0.5.8/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/core/admin.py` & `ad_sdl_wei-0.5.8/wei/core/admin.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/core/data_classes.py` & `ad_sdl_wei-0.5.8/wei/core/data_classes.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/core/events.py` & `ad_sdl_wei-0.5.8/wei/core/events.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/core/experiment.py` & `ad_sdl_wei-0.5.8/wei/core/experiment.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,21 +68,25 @@
     @property
     def run_dir(self) -> Path:
         """Path to the result directory"""
         return self.experiment_dir / "runs"
 
 
 def list_experiments():
-    """Return a list of all experiments in the Config folger
+    """Return a list of all experiments in the Config folder
 
     Returns
     -------
     all_exps Dict
     """
     experiments_dir = Config.data_directory / "experiments"
     all_exps_raw = os.listdir(experiments_dir)
     pat1 = r"(.+)_id_(.+)"
     all_exps = {}
     for exp in all_exps_raw:
-        test = re.match(pat1, exp)
-        all_exps[test[2]] = test[1]
+        try:
+            test = re.match(pat1, exp)
+            all_exps[test[2]] = test[1]
+        except Exception:
+            # Incorrectly formatted folder name, ignore
+            pass
     return all_exps
```

### Comparing `ad_sdl_wei-0.5.7/wei/core/interface.py` & `ad_sdl_wei-0.5.8/wei/core/interface.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/core/interfaces/rest_interface.py` & `ad_sdl_wei-0.5.8/wei/core/interfaces/rest_interface.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/core/interfaces/ros2_interface.py` & `ad_sdl_wei-0.5.8/wei/core/interfaces/ros2_interface.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/core/interfaces/simulate_interface.py` & `ad_sdl_wei-0.5.8/wei/core/interfaces/simulate_interface.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/core/interfaces/tcp_interface.py` & `ad_sdl_wei-0.5.8/wei/core/interfaces/tcp_interface.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/core/interfaces/zmq_interface.py` & `ad_sdl_wei-0.5.8/wei/core/interfaces/zmq_interface.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/core/location.py` & `ad_sdl_wei-0.5.8/wei/core/location.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/core/loggers.py` & `ad_sdl_wei-0.5.8/wei/core/loggers.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/core/module.py` & `ad_sdl_wei-0.5.8/wei/core/module.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/core/scheduler.py` & `ad_sdl_wei-0.5.8/wei/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/core/state_manager.py` & `ad_sdl_wei-0.5.8/wei/core/state_manager.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/core/step.py` & `ad_sdl_wei-0.5.8/wei/core/step.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/core/workcell.py` & `ad_sdl_wei-0.5.8/wei/core/workcell.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/core/workflow.py` & `ad_sdl_wei-0.5.8/wei/core/workflow.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/engine.py` & `ad_sdl_wei-0.5.8/wei/engine.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/experiment_client.py` & `ad_sdl_wei-0.5.8/wei/experiment_client.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/helpers.py` & `ad_sdl_wei-0.5.8/wei/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,14 +52,17 @@
     from wei.config import Config
     from wei.core.data_classes import Workcell
     from wei.core.location import initialize_workcell_locations
     from wei.core.module import initialize_workcell_modules
     from wei.core.state_manager import StateManager
 
     state_manager = StateManager()
+    Config.data_directory.mkdir(parents=True, exist_ok=True)
+    (Config.data_directory / "experiments").mkdir(exist_ok=True)
+    (Config.data_directory / "temp").mkdir(exist_ok=True)
     state_manager.set_workcell(Workcell.from_yaml(Config.workcell_file))
     initialize_workcell_modules()
     initialize_workcell_locations()
 
 
 def parse_args() -> Namespace:
     """Parse WEI's command line arguments and populate the config."""
```

### Comparing `ad_sdl_wei-0.5.7/wei/routers/admin.py` & `ad_sdl_wei-0.5.8/wei/routers/admin.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/routers/experiments.py` & `ad_sdl_wei-0.5.8/wei/routers/experiments.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/routers/locations.py` & `ad_sdl_wei-0.5.8/wei/routers/locations.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/routers/modules.py` & `ad_sdl_wei-0.5.8/wei/routers/modules.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/routers/workcells.py` & `ad_sdl_wei-0.5.8/wei/routers/workcells.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/routers/workflow_runs.py` & `ad_sdl_wei-0.5.8/wei/routers/workflow_runs.py`

 * *Files identical despite different names*

### Comparing `ad_sdl_wei-0.5.7/wei/server.py` & `ad_sdl_wei-0.5.8/wei/server.py`

 * *Files identical despite different names*


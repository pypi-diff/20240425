# Comparing `tmp/cloth_tools-0.3.1.tar.gz` & `tmp/cloth_tools-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloth_tools-0.3.1.tar", last modified: Mon Apr 22 09:56:16 2024, max compression
+gzip compressed data, was "cloth_tools-0.3.2.tar", last modified: Thu Apr 25 15:09:21 2024, max compression
```

## Comparing `cloth_tools-0.3.1.tar` & `cloth_tools-0.3.2.tar`

### file list

```diff
@@ -1,55 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:56:16.850142 cloth_tools-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-22 09:56:16.850142 cloth_tools-0.3.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:56:16.846142 cloth_tools-0.3.1/cloth_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:56:16.846142 cloth_tools-0.3.1/cloth_tools/annotation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14195 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/annotation/grasp_annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/bounding_boxes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:56:16.846142 cloth_tools-0.3.1/cloth_tools/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/dataset/bookkeeping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/dataset/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/dataset/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     9970 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/dataset/format.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/dataset/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:56:16.846142 cloth_tools-0.3.1/cloth_tools/drake/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/drake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/drake/scenes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:56:16.846142 cloth_tools-0.3.1/cloth_tools/kinematics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/kinematics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/kinematics/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/kinematics/inverse_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/motion_blur_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:56:16.846142 cloth_tools-0.3.1/cloth_tools/planning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/planning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14641 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/planning/grasp_planning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:56:16.850142 cloth_tools-0.3.1/cloth_tools/point_clouds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/point_clouds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/point_clouds/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/point_clouds/cloth_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/point_clouds/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:56:16.850142 cloth_tools-0.3.1/cloth_tools/stations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/stations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10806 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/stations/competition_station.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/stations/coordinate_frames.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/stations/dual_arm_station.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/trajectory_execution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:56:16.850142 cloth_tools-0.3.1/cloth_tools/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/visualization/open3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/visualization/opencv.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/visualization/rerun.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/cloth_tools/wrench_smoother.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:56:16.850142 cloth_tools-0.3.1/cloth_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-22 09:56:16.000000 cloth_tools-0.3.1/cloth_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-22 09:56:16.000000 cloth_tools-0.3.1/cloth_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 09:56:16.000000 cloth_tools-0.3.1/cloth_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-22 09:56:16.000000 cloth_tools-0.3.1/cloth_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 09:56:16.000000 cloth_tools-0.3.1/cloth_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 09:56:16.850142 cloth_tools-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:56:16.850142 cloth_tools-0.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-22 09:56:13.000000 cloth_tools-0.3.1/test/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:09:21.057238 cloth_tools-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-25 15:09:21.057238 cloth_tools-0.3.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:09:21.049238 cloth_tools-0.3.2/cloth_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:09:21.049238 cloth_tools-0.3.2/cloth_tools/annotation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14195 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/annotation/grasp_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/bounding_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:09:21.049238 cloth_tools-0.3.2/cloth_tools/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/controllers/basic_home_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/controllers/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/controllers/dry_run_grasp_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11632 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/controllers/grasp_hanging_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13520 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/controllers/grasp_highest_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21567 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/controllers/grasp_lowest_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/controllers/hang_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/controllers/home_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14564 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/controllers/stretch_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:09:21.053238 cloth_tools-0.3.2/cloth_tools/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/dataset/bookkeeping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/dataset/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/dataset/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/dataset/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/dataset/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:09:21.053238 cloth_tools-0.3.2/cloth_tools/drake/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/drake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8009 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/drake/scenes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:09:21.053238 cloth_tools-0.3.2/cloth_tools/kinematics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/kinematics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/kinematics/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/kinematics/inverse_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/motion_blur_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/multiprocess_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:09:21.053238 cloth_tools-0.3.2/cloth_tools/planning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/planning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14634 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/planning/grasp_planning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:09:21.053238 cloth_tools-0.3.2/cloth_tools/point_clouds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/point_clouds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/point_clouds/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/point_clouds/cloth_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/point_clouds/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:09:21.053238 cloth_tools-0.3.2/cloth_tools/stations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/stations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/stations/competition_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/stations/coordinate_frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/stations/dual_arm_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/trajectory_execution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:09:21.057238 cloth_tools-0.3.2/cloth_tools/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/visualization/open3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/visualization/opencv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/visualization/rerun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/cloth_tools/wrench_smoother.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:09:21.057238 cloth_tools-0.3.2/cloth_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-25 15:09:21.000000 cloth_tools-0.3.2/cloth_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-25 15:09:21.000000 cloth_tools-0.3.2/cloth_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:09:21.000000 cloth_tools-0.3.2/cloth_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-25 15:09:21.000000 cloth_tools-0.3.2/cloth_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 15:09:21.000000 cloth_tools-0.3.2/cloth_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:09:21.057238 cloth_tools-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:09:21.057238 cloth_tools-0.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-25 15:09:17.000000 cloth_tools-0.3.2/test/test_dummy.py
```

### Comparing `cloth_tools-0.3.1/PKG-INFO` & `cloth_tools-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloth-tools
-Version: 0.3.1
+Version: 0.3.2
 Summary: Official package for the ICRA 2024 Cloth Competition
 Author-email: Victor-Louis De Gusseme <victorlouisdg@gmail.com>
 Project-URL: Homepage, https://github.com/Victorlouisdg/cloth-competition
 Project-URL: Issues, https://github.com/Victorlouisdg/cloth-competition/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cloth_tools-0.3.1/cloth_tools/annotation/grasp_annotation.py` & `cloth_tools-0.3.2/cloth_tools/annotation/grasp_annotation.py`

 * *Files identical despite different names*

### Comparing `cloth_tools-0.3.1/cloth_tools/bounding_boxes.py` & `cloth_tools-0.3.2/cloth_tools/bounding_boxes.py`

 * *Files identical despite different names*

### Comparing `cloth_tools-0.3.1/cloth_tools/config.py` & `cloth_tools-0.3.2/cloth_tools/config.py`

 * *Files identical despite different names*

### Comparing `cloth_tools-0.3.1/cloth_tools/dataset/bookkeeping.py` & `cloth_tools-0.3.2/cloth_tools/dataset/bookkeeping.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,14 +5,15 @@
         - sample_000000
             sample_000000.png
             sample_000000.ply
         - sample_000001
 """
 
 import datetime
+import glob
 import os
 
 
 def datetime_for_filename(include_us=True, use_UTC=True) -> str:
     """Return a string with the current date and time formatted for use in filenames.
 
     Based on the ISO 8601 standard but optionally adds microseconds.
@@ -59,14 +60,24 @@
     index_most_recent = suffixes.index(max(suffixes))
 
     sample_dir_most_recent = sample_dirs[index_most_recent]
 
     return os.path.join(dir, sample_dir_most_recent)
 
 
+def find_latest_sample_dir_with_observation_start(base_dir: str) -> str:
+    # TODO handle case when there are none
+    sample_dirs = glob.glob(f"{str(base_dir)}/**/sample_*")  # Recursively search for sample directories
+    sample_dirs += glob.glob(f"{str(base_dir)}/sample_*")  # Search for sample directories in the base directory
+    sample_dirs_with_observation_start = [d for d in sample_dirs if os.path.exists(f"{d}/observation_start")]
+    base_names = [os.path.basename(d) for d in sample_dirs_with_observation_start]
+    sorted_sample_dirs = [x for _, x in sorted(zip(base_names, sample_dirs_with_observation_start), reverse=True)]
+    return sorted_sample_dirs[0]
+
+
 def find_highest_suffix(dir: str, name: str, extension: str | None = None) -> int:
     """Find the highest suffix of files or directories in a directory with a given name.
     Only files with exactly the same extension are considered.
 
     For example if the directory contains files with the names:
         sample_000000.png
         sample_000001.png
```

### Comparing `cloth_tools-0.3.1/cloth_tools/dataset/collection.py` & `cloth_tools-0.3.2/cloth_tools/dataset/collection.py`

 * *Files identical despite different names*

### Comparing `cloth_tools-0.3.1/cloth_tools/dataset/download.py` & `cloth_tools-0.3.2/cloth_tools/dataset/download.py`

 * *Files identical despite different names*

### Comparing `cloth_tools-0.3.1/cloth_tools/dataset/format.py` & `cloth_tools-0.3.2/cloth_tools/dataset/format.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     CameraResolutionType,
     HomogeneousMatrixType,
     JointConfigurationType,
     NumpyDepthMapType,
     NumpyIntImageType,
     PointCloud,
 )
+from cloth_tools.dataset.bookkeeping import datetime_for_filename
 from loguru import logger
 from pydantic import BaseModel
 
 
 class JointConfigurationModel(BaseModel):
     values: List[float]
 
@@ -215,7 +216,20 @@
         arm_right_joints=arm_right_joints,
         arm_left_tcp_pose_in_world=arm_left_tcp_pose_in_world,
         arm_right_tcp_pose_in_world=arm_right_tcp_pose_in_world,
         right_camera_pose_in_left_camera=right_camera_pose_in_left_camera,
         camera_intrinsics=camera_intrinsics,
         camera_resolution=camera_resolution,
     )
+
+
+def save_grasp_pose(dir: str, grasp_pose: HomogeneousMatrixType) -> str:
+    os.makedirs(dir, exist_ok=True)
+
+    grasp_pose_name = f"grasp_pose_{datetime_for_filename()}.json"
+    grasp_pose_file = os.path.join(dir, grasp_pose_name)
+
+    with open(grasp_pose_file, "w") as f:
+        grasp_pose_model = Pose.from_homogeneous_matrix(grasp_pose)
+        json.dump(grasp_pose_model.model_dump(exclude_none=False), f, indent=4)
+
+    return grasp_pose_file
```

### Comparing `cloth_tools-0.3.1/cloth_tools/dataset/upload.py` & `cloth_tools-0.3.2/cloth_tools/dataset/upload.py`

 * *Files identical despite different names*

### Comparing `cloth_tools-0.3.1/cloth_tools/kinematics/inverse_kinematics.py` & `cloth_tools-0.3.2/cloth_tools/kinematics/inverse_kinematics.py`

 * *Files identical despite different names*

### Comparing `cloth_tools-0.3.1/cloth_tools/motion_blur_detector.py` & `cloth_tools-0.3.2/cloth_tools/motion_blur_detector.py`

 * *Files identical despite different names*

### Comparing `cloth_tools-0.3.1/cloth_tools/planning/grasp_planning.py` & `cloth_tools-0.3.2/cloth_tools/planning/grasp_planning.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     start_configuration_left: JointConfigurationType,
     start_configuration_right: JointConfigurationType,
     inverse_kinematics_left_fn: InverseKinematicsFunctionType,  # same comment as for is_state_valid_fn_grasp
     inverse_kinematics_right_fn: InverseKinematicsFunctionType,
     is_state_valid_fn_grasp: JointConfigurationCheckerType,  # could make this optional and use planner's by default
     plant_toppra: MultibodyPlant,
     with_left: bool = True,
-) -> tuple[Trajectory]:
+) -> Trajectory:
 
     # We add 1.0 so at least one pregrasp distance fails:
     # pregrasp_distances_to_try = [0.05, 0.1, 0.15]  # , 0.2, 0.25]
     distance_min = 0.05
     distance_max = 0.25
     step = 0.01
     steps = int(np.rint((distance_max - distance_min) / step)) + 1
```

### Comparing `cloth_tools-0.3.1/cloth_tools/point_clouds/camera.py` & `cloth_tools-0.3.2/cloth_tools/point_clouds/camera.py`

 * *Files identical despite different names*

### Comparing `cloth_tools-0.3.1/cloth_tools/point_clouds/operations.py` & `cloth_tools-0.3.2/cloth_tools/point_clouds/operations.py`

 * *Files identical despite different names*

### Comparing `cloth_tools-0.3.1/cloth_tools/stations/competition_station.py` & `cloth_tools-0.3.2/cloth_tools/stations/competition_station.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,28 +191,32 @@
 
 if __name__ == "__main__":
     import cv2
     import rerun as rr
     from airo_camera_toolkit.utils.image_converter import ImageConverter
     from cloth_tools.visualization.opencv import draw_pose
 
+    rr.init("Competition Station - Point cloud")
+    rr.spawn(memory_limit="25%")
+
     # Check whether all hardware is connected
     station = CompetitionStation()
     camera = station.camera
     dual_arm = station.dual_arm
 
     X_W_C = station.camera_pose
     X_W_LCB = station.left_arm_pose
     X_W_RCB = station.right_arm_pose
 
     window_name = "Competiton station"
     cv2.namedWindow(window_name, cv2.WINDOW_NORMAL)
     cv2.resizeWindow(window_name, 1600, 800)
 
-    rr.init("Competition Station - Point cloud", spawn=True)
+    # rr.spawn(memory_limit="25%")
+    # rr.init("Competition Station - Point cloud")
 
     while True:
         image_rgb = camera.get_rgb_image_as_int()
         image_right_rgb = camera._retrieve_rgb_image_as_int(StereoRGBDCamera.RIGHT_RGB)
         point_cloud = camera._retrieve_colored_point_cloud()
         confidence_map = camera._retrieve_confidence_map()
         depth_map = camera._retrieve_depth_map()
```

### Comparing `cloth_tools-0.3.1/cloth_tools/stations/coordinate_frames.py` & `cloth_tools-0.3.2/cloth_tools/stations/coordinate_frames.py`

 * *Files identical despite different names*

### Comparing `cloth_tools-0.3.1/cloth_tools/stations/dual_arm_station.py` & `cloth_tools-0.3.2/cloth_tools/stations/dual_arm_station.py`

 * *Files identical despite different names*

### Comparing `cloth_tools-0.3.1/cloth_tools/trajectory_execution.py` & `cloth_tools-0.3.2/cloth_tools/trajectory_execution.py`

 * *Files identical despite different names*

### Comparing `cloth_tools-0.3.1/cloth_tools/visualization/open3d.py` & `cloth_tools-0.3.2/cloth_tools/visualization/open3d.py`

 * *Files identical despite different names*

### Comparing `cloth_tools-0.3.1/cloth_tools/visualization/opencv.py` & `cloth_tools-0.3.2/cloth_tools/visualization/opencv.py`

 * *Files identical despite different names*

### Comparing `cloth_tools-0.3.1/cloth_tools/visualization/rerun.py` & `cloth_tools-0.3.2/cloth_tools/visualization/rerun.py`

 * *Files identical despite different names*

### Comparing `cloth_tools-0.3.1/cloth_tools/wrench_smoother.py` & `cloth_tools-0.3.2/cloth_tools/wrench_smoother.py`

 * *Files identical despite different names*

### Comparing `cloth_tools-0.3.1/cloth_tools.egg-info/PKG-INFO` & `cloth_tools-0.3.2/cloth_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloth-tools
-Version: 0.3.1
+Version: 0.3.2
 Summary: Official package for the ICRA 2024 Cloth Competition
 Author-email: Victor-Louis De Gusseme <victorlouisdg@gmail.com>
 Project-URL: Homepage, https://github.com/Victorlouisdg/cloth-competition
 Project-URL: Issues, https://github.com/Victorlouisdg/cloth-competition/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cloth_tools-0.3.1/pyproject.toml` & `cloth_tools-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cloth-tools"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name = "Victor-Louis De Gusseme", email = "victorlouisdg@gmail.com" },
 ]
 description = "Official package for the ICRA 2024 Cloth Competition"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```


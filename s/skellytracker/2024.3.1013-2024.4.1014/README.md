# Comparing `tmp/skellytracker-2024.3.1013.tar.gz` & `tmp/skellytracker-2024.4.1014.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skellytracker-2024.3.1013.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "skellytracker-2024.4.1014.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `skellytracker-2024.3.1013.tar` & `skellytracker-2024.4.1014.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0       65 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/.gitattributes
--rw-r--r--   0        0        0     1138 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/.github/workflows/flit_publish_to_pypi.yml
--rw-r--r--   0        0        0     2903 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/.gitignore
--rw-r--r--   0        0        0      364 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/CITATION.cff
--rw-r--r--   0        0        0    34523 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/LICENSE
--rw-r--r--   0        0        0      766 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/README.md
--rw-r--r--   0        0        0        0 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/__init__.py
--rw-r--r--   0        0        0      897 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/poetry_pyproject.toml
--rw-r--r--   0        0        0     2635 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/pyproject.toml
--rw-r--r--   0        0        0     1614 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/RUN_ME.py
--rw-r--r--   0        0        0     1388 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/SINGLE_IMAGE_RUN.py
--rw-r--r--   0        0        0     1252 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/__init__.py
--rw-r--r--   0        0        0      606 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/__main__.py
--rw-r--r--   0        0        0     7234 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/process_folder_of_videos.py
--rw-r--r--   0        0        0        0 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/system/__init__.py
--rw-r--r--   0        0        0     1424 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/system/default_paths.py
--rw-r--r--   0        0        0     1405 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/system/logging_configuration.py
--rw-r--r--   0        0        0        0 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/test/__init__.py
--rw-r--r--   0        0        0      305 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/test/test_test.py
--rw-r--r--   0        0        0        0 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/trackers/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/trackers/base_tracker/__init__.py
--rw-r--r--   0        0        0     1711 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/trackers/base_tracker/base_recorder.py
--rw-r--r--   0        0        0     5055 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/trackers/base_tracker/base_tracker.py
--rw-r--r--   0        0        0      132 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/trackers/base_tracker/base_tracking_params.py
--rw-r--r--   0        0        0      409 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/trackers/base_tracker/tracked_object.py
--rw-r--r--   0        0        0     1199 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/trackers/base_tracker/video_handler.py
--rw-r--r--   0        0        0        0 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/trackers/bright_point_tracker/__init__.py
--rw-r--r--   0        0        0      908 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/trackers/bright_point_tracker/brightest_point_recorder.py
--rw-r--r--   0        0        0     3262 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/trackers/bright_point_tracker/brightest_point_tracker.py
--rw-r--r--   0        0        0     3399 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/trackers/charuco_tracker/charuco_tracker.py
--rw-r--r--   0        0        0      802 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/trackers/image_demo_viewer/image_demo_viewer.py
--rw-r--r--   0        0        0     2807 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/trackers/mediapipe_tracker/mediapipe_holistic_recorder.py
--rw-r--r--   0        0        0     3469 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/trackers/mediapipe_tracker/mediapipe_holistic_tracker.py
--rw-r--r--   0        0        0     1635 2024-03-26 03:31:17.568391 skellytracker-2024.3.1013/skellytracker/trackers/mediapipe_tracker/mediapipe_model_info.py
--rw-r--r--   0        0        0     1610 2024-03-26 03:31:17.572391 skellytracker-2024.3.1013/skellytracker/trackers/mmpose_tracker/mmpose_tracker.py
--rw-r--r--   0        0        0      827 2024-03-26 03:31:17.572391 skellytracker-2024.3.1013/skellytracker/trackers/segment_anything_tracker/segment_anything_tracker.py
--rw-r--r--   0        0        0     1207 2024-03-26 03:31:17.572391 skellytracker-2024.3.1013/skellytracker/trackers/tracker_manager.py
--rw-r--r--   0        0        0     3049 2024-03-26 03:31:17.572391 skellytracker-2024.3.1013/skellytracker/trackers/webcam_demo_viewer/webcam_demo_viewer.py
--rw-r--r--   0        0        0     8817 2024-03-26 03:31:17.572391 skellytracker-2024.3.1013/skellytracker/trackers/yolo_mediapipe_combo_tracker/yolo_mediapipe_combo_tracker.py
--rw-r--r--   0        0        0      418 2024-03-26 03:31:17.572391 skellytracker-2024.3.1013/skellytracker/trackers/yolo_object_tracker/yolo_object_model_info.py
--rw-r--r--   0        0        0      751 2024-03-26 03:31:17.572391 skellytracker-2024.3.1013/skellytracker/trackers/yolo_object_tracker/yolo_object_recorder.py
--rw-r--r--   0        0        0     1980 2024-03-26 03:31:17.572391 skellytracker-2024.3.1013/skellytracker/trackers/yolo_object_tracker/yolo_object_tracker.py
--rw-r--r--   0        0        0     1974 2024-03-26 03:31:17.572391 skellytracker-2024.3.1013/skellytracker/trackers/yolo_tracker/yolo_model_info.py
--rw-r--r--   0        0        0     1202 2024-03-26 03:31:17.572391 skellytracker-2024.3.1013/skellytracker/trackers/yolo_tracker/yolo_recorder.py
--rw-r--r--   0        0        0     2176 2024-03-26 03:31:17.572391 skellytracker-2024.3.1013/skellytracker/trackers/yolo_tracker/yolo_tracker.py
--rw-r--r--   0        0        0        0 2024-03-26 03:31:17.572391 skellytracker-2024.3.1013/skellytracker/utilities/__init__.py
--rw-r--r--   0        0        0      702 2024-03-26 03:31:17.572391 skellytracker-2024.3.1013/skellytracker/utilities/get_video_paths.py
--rw-r--r--   0        0        0        0 2024-03-26 03:31:17.572391 skellytracker-2024.3.1013/skellytracker/utilities/quine_directory_printer/__init__.py
--rw-r--r--   0        0        0     4294 2024-03-26 03:31:17.572391 skellytracker-2024.3.1013/skellytracker/utilities/quine_directory_printer/quine.py
--rw-r--r--   0        0        0     2935 1970-01-01 00:00:00.000000 skellytracker-2024.3.1013/PKG-INFO
+-rw-r--r--   0        0        0       65 2024-04-25 17:24:39.293578 skellytracker-2024.4.1014/.gitattributes
+-rw-r--r--   0        0        0     1138 2024-04-25 17:24:39.293578 skellytracker-2024.4.1014/.github/workflows/flit_publish_to_pypi.yml
+-rw-r--r--   0        0        0     2903 2024-04-25 17:24:39.293578 skellytracker-2024.4.1014/.gitignore
+-rw-r--r--   0        0        0      364 2024-04-25 17:24:39.293578 skellytracker-2024.4.1014/CITATION.cff
+-rw-r--r--   0        0        0    34523 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/LICENSE
+-rw-r--r--   0        0        0      765 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/README.md
+-rw-r--r--   0        0        0        0 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/__init__.py
+-rw-r--r--   0        0        0      897 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/poetry_pyproject.toml
+-rw-r--r--   0        0        0     2717 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/pyproject.toml
+-rw-r--r--   0        0        0     1824 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/RUN_ME.py
+-rw-r--r--   0        0        0     1550 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/SINGLE_IMAGE_RUN.py
+-rw-r--r--   0        0        0     1557 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/__init__.py
+-rw-r--r--   0        0        0      606 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/__main__.py
+-rw-r--r--   0        0        0     8114 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/process_folder_of_videos.py
+-rw-r--r--   0        0        0        0 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/system/__init__.py
+-rw-r--r--   0        0        0     1424 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/system/default_paths.py
+-rw-r--r--   0        0        0     1405 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/system/logging_configuration.py
+-rw-r--r--   0        0        0        0 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/test/__init__.py
+-rw-r--r--   0        0        0      305 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/test/test_test.py
+-rw-r--r--   0        0        0        0 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/base_tracker/__init__.py
+-rw-r--r--   0        0        0     1711 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/base_tracker/base_recorder.py
+-rw-r--r--   0        0        0     5055 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/base_tracker/base_tracker.py
+-rw-r--r--   0        0        0      132 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/base_tracker/base_tracking_params.py
+-rw-r--r--   0        0        0      409 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/base_tracker/tracked_object.py
+-rw-r--r--   0        0        0     1199 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/base_tracker/video_handler.py
+-rw-r--r--   0        0        0        0 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/bright_point_tracker/__init__.py
+-rw-r--r--   0        0        0      908 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/bright_point_tracker/brightest_point_recorder.py
+-rw-r--r--   0        0        0     3262 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/bright_point_tracker/brightest_point_tracker.py
+-rw-r--r--   0        0        0     3399 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/charuco_tracker/charuco_tracker.py
+-rw-r--r--   0        0        0      802 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/image_demo_viewer/image_demo_viewer.py
+-rw-r--r--   0        0        0     2807 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/mediapipe_tracker/mediapipe_holistic_recorder.py
+-rw-r--r--   0        0        0     3469 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/mediapipe_tracker/mediapipe_holistic_tracker.py
+-rw-r--r--   0        0        0     1635 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/mediapipe_tracker/mediapipe_model_info.py
+-rw-r--r--   0        0        0     1610 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/mmpose_tracker/mmpose_tracker.py
+-rw-r--r--   0        0        0      827 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/segment_anything_tracker/segment_anything_tracker.py
+-rw-r--r--   0        0        0     1207 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/tracker_manager.py
+-rw-r--r--   0        0        0     3049 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/webcam_demo_viewer/webcam_demo_viewer.py
+-rw-r--r--   0        0        0     8817 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/yolo_mediapipe_combo_tracker/yolo_mediapipe_combo_tracker.py
+-rw-r--r--   0        0        0      418 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/yolo_object_tracker/yolo_object_model_info.py
+-rw-r--r--   0        0        0      751 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/yolo_object_tracker/yolo_object_recorder.py
+-rw-r--r--   0        0        0     1980 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/yolo_object_tracker/yolo_object_tracker.py
+-rw-r--r--   0        0        0     1974 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/yolo_tracker/yolo_model_info.py
+-rw-r--r--   0        0        0     1202 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/yolo_tracker/yolo_recorder.py
+-rw-r--r--   0        0        0     2176 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/trackers/yolo_tracker/yolo_tracker.py
+-rw-r--r--   0        0        0        0 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/utilities/__init__.py
+-rw-r--r--   0        0        0      702 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/utilities/get_video_paths.py
+-rw-r--r--   0        0        0        0 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/utilities/quine_directory_printer/__init__.py
+-rw-r--r--   0        0        0     4294 2024-04-25 17:24:39.297578 skellytracker-2024.4.1014/skellytracker/utilities/quine_directory_printer/quine.py
+-rw-r--r--   0        0        0     3170 1970-01-01 00:00:00.000000 skellytracker-2024.4.1014/PKG-INFO
```

### Comparing `skellytracker-2024.3.1013/.github/workflows/flit_publish_to_pypi.yml` & `skellytracker-2024.4.1014/.github/workflows/flit_publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/.gitignore` & `skellytracker-2024.4.1014/.gitignore`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/LICENSE` & `skellytracker-2024.4.1014/LICENSE`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/README.md` & `skellytracker-2024.4.1014/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # skellytracker
 
 The tracking backend for freemocap. Collects different pose estimation tools and aggregates them using a consistent API. Can run pose estimation on images, webcams, and videos.
 
 ## Run skelly_tracker
 
-Installation: `pip install skellytracker``
+Installation: `pip install skellytracker`
 Then it can be run with `skellytracker`.
 
 Running the basic `skellytracker` will open the first webcam port on your computer and run pose estimaiton in realtime with mediapipe holistic as a tracker. You can specify the tracker with `skellytracker TRACKER_NAME`, where `TRACKER_NAME` is the name of an available tracker. To view the names of all available trackers, see `RUN_ME.py`.
 
 It will take some time to initialize the tracker the first time you run it, as it will likely need to download the model.
```

### Comparing `skellytracker-2024.3.1013/poetry_pyproject.toml` & `skellytracker-2024.4.1014/poetry_pyproject.toml`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/pyproject.toml` & `skellytracker-2024.4.1014/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -53,29 +53,31 @@
     "computer vision"
 ]
 
 #dynamic = ["dependencies"]
 dependencies = [
     "opencv-contrib-python==4.8.*",
     "pydantic==1.*",
-    "mediapipe==0.10.9",
-    "ultralytics~=8.0.202",
+    "tqdm==4.*",
 ]
 requires-python = ">=3.9,<3.12"
 
 dynamic = ["version", "description"]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
+mediapipe = ["mediapipe==0.10.9"]
+yolo = ["ultralytics~=8.0.202"]
+all = ["ultralytics~=8.0.202", "mediapipe==0.10.9"]
 
 [project.urls]
 Homepage = "https://github.com/freemocap/skellytracker"
 
 [tool.bumpver]
-current_version = "v2024.03.1013"
+current_version = "v2024.04.1014"
 
 version_pattern = "vYYYY.0M.BUILD[-TAG]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = true
```

### Comparing `skellytracker-2024.3.1013/skellytracker/RUN_ME.py` & `skellytracker-2024.4.1014/skellytracker/RUN_ME.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 import cv2
 
+
 from skellytracker.trackers.bright_point_tracker.brightest_point_tracker import (
     BrightestPointTracker,
 )
 from skellytracker.trackers.charuco_tracker.charuco_tracker import CharucoTracker
-from skellytracker.trackers.mediapipe_tracker.mediapipe_holistic_tracker import (
-    MediapipeHolisticTracker,
-)
-from skellytracker.trackers.segment_anything_tracker.segment_anything_tracker import (
-    SAMTracker,
-)
-from skellytracker.trackers.yolo_tracker.yolo_tracker import YOLOPoseTracker
-from skellytracker.trackers.yolo_object_tracker.yolo_object_tracker import (
-    YOLOObjectTracker,
-)
+try:
+    from skellytracker.trackers.mediapipe_tracker.mediapipe_holistic_tracker import (
+        MediapipeHolisticTracker,
+    )
+except:
+    print("To use mediapipe_holistic_tracker, install skellytracker[mediapipe]")
+try:
+    from skellytracker.trackers.yolo_tracker.yolo_tracker import YOLOPoseTracker
+    from skellytracker.trackers.yolo_object_tracker.yolo_object_tracker import (
+        YOLOObjectTracker,
+    )
+    from skellytracker.trackers.segment_anything_tracker.segment_anything_tracker import (
+        SAMTracker,
+    )
+except:
+    print("To use yolo_tracker, install skellytracker[yolo]")
 
 
 def main(demo_tracker: str = "mediapipe_holistic_tracker"):
 
     if demo_tracker == "brightest_point_tracker":
         BrightestPointTracker().demo()
```

### Comparing `skellytracker-2024.3.1013/skellytracker/SINGLE_IMAGE_RUN.py` & `skellytracker-2024.4.1014/skellytracker/SINGLE_IMAGE_RUN.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,45 @@
 import cv2
 from pathlib import Path
 
-from skellytracker.trackers.bright_point_tracker.brightest_point_tracker import BrightestPointTracker
+from skellytracker.trackers.bright_point_tracker.brightest_point_tracker import (
+    BrightestPointTracker,
+)
 from skellytracker.trackers.charuco_tracker.charuco_tracker import CharucoTracker
-from skellytracker.trackers.mediapipe_tracker.mediapipe_holistic_tracker import MediapipeHolisticTracker
-from skellytracker.trackers.yolo_tracker.yolo_tracker import YOLOPoseTracker
+
+try:
+    from skellytracker.trackers.mediapipe_tracker.mediapipe_holistic_tracker import (
+        MediapipeHolisticTracker,
+    )
+except:
+    print("\n\nTo use mediapipe_holistic_tracker, install skellytracker[mediapipe]\n\n")
+try:
+    from skellytracker.trackers.yolo_tracker.yolo_tracker import YOLOPoseTracker
+except:
+    print("\n\nTo use yolo_tracker, install skellytracker[yolo]\n\n")
+
 
 if __name__ == "__main__":
     demo_tracker = "brightest_point_tracker"
     image_path = Path("/Path/To/Your/Image.jpg")
 
     if demo_tracker == "brightest_point_tracker":
         BrightestPointTracker().image_demo(image_path=image_path)
 
     elif demo_tracker == "charuco_tracker":
-        CharucoTracker(squaresX=7,
-                       squaresY=5,
-                       dictionary=cv2.aruco.getPredefinedDictionary(cv2.aruco.DICT_4X4_250)).image_demo(image_path=image_path)
+        CharucoTracker(
+            squaresX=7,
+            squaresY=5,
+            dictionary=cv2.aruco.getPredefinedDictionary(cv2.aruco.DICT_4X4_250),
+        ).image_demo(image_path=image_path)
 
     elif demo_tracker == "mediapipe_holistic_tracker":
-        MediapipeHolisticTracker(model_complexity=2,
-                                 min_detection_confidence=0.5,
-                                 min_tracking_confidence=0.5,
-                                 static_image_mode=False,
-                                 smooth_landmarks=True).image_demo(image_path=image_path)
+        MediapipeHolisticTracker(
+            model_complexity=2,
+            min_detection_confidence=0.5,
+            min_tracking_confidence=0.5,
+            static_image_mode=False,
+            smooth_landmarks=True,
+        ).image_demo(image_path=image_path)
 
     elif demo_tracker == "yolo_tracker":
-        YOLOPoseTracker(model_size="high_res").image_demo(image_path=image_path)
+        YOLOPoseTracker(model_size="high_res").image_demo(image_path=image_path)
```

### Comparing `skellytracker-2024.3.1013/skellytracker/__main__.py` & `skellytracker-2024.4.1014/skellytracker/__main__.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/skellytracker/process_folder_of_videos.py` & `skellytracker-2024.4.1014/skellytracker/process_folder_of_videos.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 import logging
 from multiprocessing import Pool, cpu_count
 from pathlib import Path
 import sys
-from typing import Any, Optional, Type
+from typing import Optional
 import numpy as np
 from pydantic import BaseModel
 
 
 from skellytracker.trackers.base_tracker.base_tracker import BaseTracker
 from skellytracker.trackers.bright_point_tracker.brightest_point_tracker import (
     BrightestPointTracker,
 )
-from skellytracker.trackers.mediapipe_tracker.mediapipe_holistic_tracker import (
-    MediapipeHolisticTracker,
-)
-from skellytracker.trackers.yolo_mediapipe_combo_tracker.yolo_mediapipe_combo_tracker import (
-    YOLOMediapipeComboTracker,
-)
-from skellytracker.trackers.yolo_tracker.yolo_tracker import YOLOPoseTracker
-from skellytracker.trackers.mediapipe_tracker.mediapipe_model_info import (
-    MediapipeTrackingParams,
-)
 from skellytracker.utilities.get_video_paths import get_video_paths
+try:
+    from skellytracker.trackers.yolo_mediapipe_combo_tracker.yolo_mediapipe_combo_tracker import (
+        YOLOMediapipeComboTracker,
+    )
+except:
+    print("\n\nTo use yolo_mediapipe_combo_tracker, install skellytracker[yolo, mediapipe]\n\n")
+try:
+    from skellytracker.trackers.yolo_tracker.yolo_tracker import YOLOPoseTracker
+    from skellytracker.trackers.yolo_tracker.yolo_model_info import YOLOTrackingParams
+except:
+    print("To use yolo_tracker, install skellytracker[yolo]")
+try:
+    from skellytracker.trackers.mediapipe_tracker.mediapipe_holistic_tracker import (
+        MediapipeHolisticTracker,
+    )
+    from skellytracker.trackers.mediapipe_tracker.mediapipe_model_info import (
+        MediapipeTrackingParams,
+    )
+except:
+    print("To use mediapipe_holistic_tracker, install skellytracker[mediapipe]")
 
 logger = logging.getLogger(__name__)
 
 file_name_dictionary = {
     "MediapipeHolisticTracker": "mediapipe2dData_numCams_numFrames_numTrackedPoints_pixelXY.npy",
     "YOLOMediapipeComboTracker": "mediapipe2dData_numCams_numFrames_numTrackedPoints_pixelXY.npy",
     "YOLOPoseTracker": "yolo2dData_numCams_numFrames_numTrackedPoints_pixelXY.npy",
@@ -35,15 +45,15 @@
 
 def process_folder_of_videos(
     tracker_name: str,
     tracking_params: BaseModel,
     synchronized_video_path: Path,
     output_folder_path: Optional[Path] = None,
     annotated_video_path: Optional[Path] = None,
-    num_processes: int = None,
+    num_processes: Optional[int] = None,
 ) -> np.ndarray:
     """
     Process a folder of synchronized videos with the given tracker.
     Tracked data will be saved to a .npy file with the shape (numCams, numFrames, numTrackedPoints, pixelXYZ).
 
     :param tracker_name: Tracker to use.
     :param tracking_params: Tracking parameters to use.
@@ -166,21 +176,33 @@
         tracker = BrightestPointTracker()
 
     else:
         raise ValueError("Invalid tracker type")
 
     return tracker
 
+def get_tracker_params(tracker_name: str) -> BaseModel:
+    if tracker_name == "MediapipeHolisticTracker":
+        return MediapipeTrackingParams()
+    elif tracker_name == "YOLOMediapipeComboTracker":
+        return YOLOTrackingParams()
+    elif tracker_name == "YOLOPoseTracker":
+        return YOLOTrackingParams()
+    elif tracker_name == "BrightestPointTracker":
+        return BaseModel()
+    else:
+        raise ValueError("Invalid tracker type")
+
 
 if __name__ == "__main__":
     synchronized_video_path = Path(
         "/Users/philipqueen/freemocap_data/recording_sessions/freemocap_sample_data/synchronized_videos"
     )
     tracker_name = "YOLOMediapipeComboTracker"
     num_processes = None
 
     process_folder_of_videos(
         tracker_name=tracker_name,
-        tracking_params=MediapipeTrackingParams(),
+        tracking_params=get_tracker_params(tracker_name=tracker_name),
         synchronized_video_path=synchronized_video_path,
         num_processes=num_processes,
     )
```

### Comparing `skellytracker-2024.3.1013/skellytracker/system/default_paths.py` & `skellytracker-2024.4.1014/skellytracker/system/default_paths.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/skellytracker/system/logging_configuration.py` & `skellytracker-2024.4.1014/skellytracker/system/logging_configuration.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/skellytracker/trackers/base_tracker/base_recorder.py` & `skellytracker-2024.4.1014/skellytracker/trackers/base_tracker/base_recorder.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/skellytracker/trackers/base_tracker/base_tracker.py` & `skellytracker-2024.4.1014/skellytracker/trackers/base_tracker/base_tracker.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/skellytracker/trackers/base_tracker/video_handler.py` & `skellytracker-2024.4.1014/skellytracker/trackers/base_tracker/video_handler.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/skellytracker/trackers/bright_point_tracker/brightest_point_recorder.py` & `skellytracker-2024.4.1014/skellytracker/trackers/bright_point_tracker/brightest_point_recorder.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/skellytracker/trackers/bright_point_tracker/brightest_point_tracker.py` & `skellytracker-2024.4.1014/skellytracker/trackers/bright_point_tracker/brightest_point_tracker.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/skellytracker/trackers/charuco_tracker/charuco_tracker.py` & `skellytracker-2024.4.1014/skellytracker/trackers/charuco_tracker/charuco_tracker.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/skellytracker/trackers/image_demo_viewer/image_demo_viewer.py` & `skellytracker-2024.4.1014/skellytracker/trackers/image_demo_viewer/image_demo_viewer.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/skellytracker/trackers/mediapipe_tracker/mediapipe_holistic_recorder.py` & `skellytracker-2024.4.1014/skellytracker/trackers/mediapipe_tracker/mediapipe_holistic_recorder.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/skellytracker/trackers/mediapipe_tracker/mediapipe_holistic_tracker.py` & `skellytracker-2024.4.1014/skellytracker/trackers/mediapipe_tracker/mediapipe_holistic_tracker.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/skellytracker/trackers/mediapipe_tracker/mediapipe_model_info.py` & `skellytracker-2024.4.1014/skellytracker/trackers/mediapipe_tracker/mediapipe_model_info.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/skellytracker/trackers/mmpose_tracker/mmpose_tracker.py` & `skellytracker-2024.4.1014/skellytracker/trackers/mmpose_tracker/mmpose_tracker.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/skellytracker/trackers/segment_anything_tracker/segment_anything_tracker.py` & `skellytracker-2024.4.1014/skellytracker/trackers/segment_anything_tracker/segment_anything_tracker.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/skellytracker/trackers/tracker_manager.py` & `skellytracker-2024.4.1014/skellytracker/trackers/tracker_manager.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/skellytracker/trackers/webcam_demo_viewer/webcam_demo_viewer.py` & `skellytracker-2024.4.1014/skellytracker/trackers/webcam_demo_viewer/webcam_demo_viewer.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/skellytracker/trackers/yolo_mediapipe_combo_tracker/yolo_mediapipe_combo_tracker.py` & `skellytracker-2024.4.1014/skellytracker/trackers/yolo_mediapipe_combo_tracker/yolo_mediapipe_combo_tracker.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/skellytracker/trackers/yolo_object_tracker/yolo_object_recorder.py` & `skellytracker-2024.4.1014/skellytracker/trackers/yolo_object_tracker/yolo_object_recorder.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/skellytracker/trackers/yolo_object_tracker/yolo_object_tracker.py` & `skellytracker-2024.4.1014/skellytracker/trackers/yolo_object_tracker/yolo_object_tracker.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/skellytracker/trackers/yolo_tracker/yolo_model_info.py` & `skellytracker-2024.4.1014/skellytracker/trackers/yolo_tracker/yolo_model_info.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/skellytracker/trackers/yolo_tracker/yolo_recorder.py` & `skellytracker-2024.4.1014/skellytracker/trackers/yolo_tracker/yolo_recorder.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/skellytracker/trackers/yolo_tracker/yolo_tracker.py` & `skellytracker-2024.4.1014/skellytracker/trackers/yolo_tracker/yolo_tracker.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/skellytracker/utilities/get_video_paths.py` & `skellytracker-2024.4.1014/skellytracker/utilities/get_video_paths.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/skellytracker/utilities/quine_directory_printer/quine.py` & `skellytracker-2024.4.1014/skellytracker/utilities/quine_directory_printer/quine.py`

 * *Files identical despite different names*

### Comparing `skellytracker-2024.3.1013/PKG-INFO` & `skellytracker-2024.4.1014/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skellytracker
-Version: 2024.3.1013
+Version: 2024.4.1014
 Summary: Top-level package for skellytracker
 Keywords: camera,stream,video,image,opencv,skelly,freemocap,motion capture,synchronization,computer vision
 Author-email: Skelly FreeMoCap <info@freemocap.org>
 Requires-Python: >=3.9,<3.12
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Intended Audience :: Developers
@@ -30,30 +30,36 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: System :: Hardware
 Classifier: Topic :: System :: Hardware :: Universal Serial Bus (USB)
 Classifier: Topic :: System :: Hardware :: Universal Serial Bus (USB) :: Video (UVC)
 Requires-Dist: opencv-contrib-python==4.8.*
 Requires-Dist: pydantic==1.*
-Requires-Dist: mediapipe==0.10.9
-Requires-Dist: ultralytics~=8.0.202
+Requires-Dist: tqdm==4.*
+Requires-Dist: ultralytics~=8.0.202 ; extra == "all"
+Requires-Dist: mediapipe==0.10.9 ; extra == "all"
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: bumpver ; extra == "dev"
 Requires-Dist: isort ; extra == "dev"
 Requires-Dist: pip-tools ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
+Requires-Dist: mediapipe==0.10.9 ; extra == "mediapipe"
+Requires-Dist: ultralytics~=8.0.202 ; extra == "yolo"
 Project-URL: Homepage, https://github.com/freemocap/skellytracker
+Provides-Extra: all
 Provides-Extra: dev
+Provides-Extra: mediapipe
+Provides-Extra: yolo
 
 # skellytracker
 
 The tracking backend for freemocap. Collects different pose estimation tools and aggregates them using a consistent API. Can run pose estimation on images, webcams, and videos.
 
 ## Run skelly_tracker
 
-Installation: `pip install skellytracker``
+Installation: `pip install skellytracker`
 Then it can be run with `skellytracker`.
 
 Running the basic `skellytracker` will open the first webcam port on your computer and run pose estimaiton in realtime with mediapipe holistic as a tracker. You can specify the tracker with `skellytracker TRACKER_NAME`, where `TRACKER_NAME` is the name of an available tracker. To view the names of all available trackers, see `RUN_ME.py`.
 
 It will take some time to initialize the tracker the first time you run it, as it will likely need to download the model.
```


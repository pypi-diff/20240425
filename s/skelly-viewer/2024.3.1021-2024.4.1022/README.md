# Comparing `tmp/skelly_viewer-2024.3.1021.tar.gz` & `tmp/skelly_viewer-2024.4.1022.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skelly_viewer-2024.3.1021.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "skelly_viewer-2024.4.1022.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `skelly_viewer-2024.3.1021.tar` & `skelly_viewer-2024.4.1022.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0       66 2024-03-18 12:52:27.877558 skelly_viewer-2024.3.1021/.gitattributes
--rw-r--r--   0        0        0     1087 2024-03-18 12:52:27.877558 skelly_viewer-2024.3.1021/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
--rw-r--r--   0        0        0     2784 2024-03-18 12:52:27.877558 skelly_viewer-2024.3.1021/.gitignore
--rw-r--r--   0        0        0     1067 2024-03-18 12:52:27.877558 skelly_viewer-2024.3.1021/LICENSE
--rw-r--r--   0        0        0      989 2024-03-18 12:52:27.877558 skelly_viewer-2024.3.1021/README.md
--rw-r--r--   0        0        0     1647 2024-03-18 12:52:27.877558 skelly_viewer-2024.3.1021/pyproject.toml
--rw-r--r--   0        0        0       50 2024-03-18 12:52:27.877558 skelly_viewer-2024.3.1021/setup.py
--rw-r--r--   0        0        0      794 2024-03-18 12:52:27.877558 skelly_viewer-2024.3.1021/skelly_viewer/__init__.py
--rw-r--r--   0        0        0      116 2024-03-18 12:52:27.877558 skelly_viewer-2024.3.1021/skelly_viewer/__main__.py
--rw-r--r--   0        0        0        0 2024-03-18 12:52:27.877558 skelly_viewer-2024.3.1021/skelly_viewer/config/__init__.py
--rw-r--r--   0        0        0     1382 2024-03-18 12:52:27.877558 skelly_viewer-2024.3.1021/skelly_viewer/config/default_paths.py
--rw-r--r--   0        0        0      478 2024-03-18 12:52:27.877558 skelly_viewer-2024.3.1021/skelly_viewer/config/folder_and_file_names.py
--rw-r--r--   0        0        0        0 2024-03-18 12:52:27.877558 skelly_viewer-2024.3.1021/skelly_viewer/config/init.py
--rw-r--r--   0        0        0     1406 2024-03-18 12:52:27.877558 skelly_viewer-2024.3.1021/skelly_viewer/config/logging_configuration.py
--rw-r--r--   0        0        0     1556 2024-03-18 12:52:27.877558 skelly_viewer-2024.3.1021/skelly_viewer/experimental/checkable_combo_box.py
--rw-r--r--   0        0        0     1155 2024-03-18 12:52:27.877558 skelly_viewer-2024.3.1021/skelly_viewer/experimental/plotly/plotly_gpt_anim_working1.py
--rw-r--r--   0        0        0        0 2024-03-18 12:52:27.881558 skelly_viewer-2024.3.1021/skelly_viewer/gui/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 12:52:27.881558 skelly_viewer-2024.3.1021/skelly_viewer/gui/qt/__init__.py
--rw-r--r--   0        0        0     3418 2024-03-18 12:52:27.881558 skelly_viewer-2024.3.1021/skelly_viewer/gui/qt/skelly_viewer_widget.py
--rw-r--r--   0        0        0     2727 2024-03-18 12:52:27.881558 skelly_viewer-2024.3.1021/skelly_viewer/gui/qt/skellyview_main_window.py
--rw-r--r--   0        0        0        0 2024-03-18 12:52:27.881558 skelly_viewer-2024.3.1021/skelly_viewer/gui/qt/widgets/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 12:52:27.881558 skelly_viewer-2024.3.1021/skelly_viewer/gui/qt/widgets/init.py
--rw-r--r--   0        0        0     5658 2024-03-18 12:52:27.881558 skelly_viewer-2024.3.1021/skelly_viewer/gui/qt/widgets/multi_video_display.py
--rw-r--r--   0        0        0     6315 2024-03-18 12:52:27.881558 skelly_viewer-2024.3.1021/skelly_viewer/gui/qt/widgets/skeleton_view_widget.py
--rw-r--r--   0        0        0     2632 2024-03-18 12:52:27.881558 skelly_viewer-2024.3.1021/skelly_viewer/gui/qt/widgets/slider_widget.py
--rw-r--r--   0        0        0        0 2024-03-18 12:52:27.881558 skelly_viewer-2024.3.1021/skelly_viewer/gui/qt/widgets/time_series_widgets/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 12:52:27.881558 skelly_viewer-2024.3.1021/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/__init__.py
--rw-r--r--   0        0        0      961 2024-03-18 12:52:27.881558 skelly_viewer-2024.3.1021/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/marker_selector_widget.py
--rw-r--r--   0        0        0     1898 2024-03-18 12:52:27.881558 skelly_viewer-2024.3.1021/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/time_series_viewer_widget.py
--rw-r--r--   0        0        0     2170 2024-03-18 12:52:27.881558 skelly_viewer-2024.3.1021/skelly_viewer/gui/qt/widgets/time_series_widgets/trajectory_view_widget.py
--rw-r--r--   0        0        0      134 2024-03-18 12:52:27.881558 skelly_viewer-2024.3.1021/skelly_viewer/test_test.py
--rw-r--r--   0        0        0        0 2024-03-18 12:52:27.881558 skelly_viewer-2024.3.1021/skelly_viewer/utilities/__init__.py
--rw-r--r--   0        0        0     2329 2024-03-18 12:52:27.881558 skelly_viewer-2024.3.1021/skelly_viewer/utilities/freemocap_data_loader.py
--rw-r--r--   0        0        0      691 2024-03-18 12:52:27.881558 skelly_viewer-2024.3.1021/skelly_viewer/utilities/get_video_paths.py
--rw-r--r--   0        0        0      832 2024-03-18 12:52:27.881558 skelly_viewer-2024.3.1021/skelly_viewer/utilities/load_sample_data.py
--rw-r--r--   0        0        0     6077 2024-03-18 12:52:27.881558 skelly_viewer-2024.3.1021/skelly_viewer/utilities/mediapipe_skeleton_builder.py
--rw-r--r--   0        0        0     1809 2024-03-18 12:52:27.881558 skelly_viewer-2024.3.1021/skelly_viewer/utilities/video_handler.py
--rw-r--r--   0        0        0     1859 1970-01-01 00:00:00.000000 skelly_viewer-2024.3.1021/PKG-INFO
+-rw-r--r--   0        0        0       66 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/.gitattributes
+-rw-r--r--   0        0        0     1087 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
+-rw-r--r--   0        0        0     2784 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/.gitignore
+-rw-r--r--   0        0        0     1067 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/LICENSE
+-rw-r--r--   0        0        0      981 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/README.md
+-rw-r--r--   0        0        0     1647 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/pyproject.toml
+-rw-r--r--   0        0        0       50 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/setup.py
+-rw-r--r--   0        0        0      794 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/__init__.py
+-rw-r--r--   0        0        0      116 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/config/__init__.py
+-rw-r--r--   0        0        0     1382 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/config/default_paths.py
+-rw-r--r--   0        0        0      478 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/config/folder_and_file_names.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/config/init.py
+-rw-r--r--   0        0        0     1406 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/config/logging_configuration.py
+-rw-r--r--   0        0        0     1556 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/experimental/checkable_combo_box.py
+-rw-r--r--   0        0        0     1155 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/experimental/plotly/plotly_gpt_anim_working1.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/gui/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/gui/qt/__init__.py
+-rw-r--r--   0        0        0     3418 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/gui/qt/skelly_viewer_widget.py
+-rw-r--r--   0        0        0     2727 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/gui/qt/skellyview_main_window.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/gui/qt/widgets/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/gui/qt/widgets/init.py
+-rw-r--r--   0        0        0     5658 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/gui/qt/widgets/multi_video_display.py
+-rw-r--r--   0        0        0     6315 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/gui/qt/widgets/skeleton_view_widget.py
+-rw-r--r--   0        0        0     2632 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/gui/qt/widgets/slider_widget.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/gui/qt/widgets/time_series_widgets/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/__init__.py
+-rw-r--r--   0        0        0      961 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/marker_selector_widget.py
+-rw-r--r--   0        0        0     1898 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/time_series_viewer_widget.py
+-rw-r--r--   0        0        0     2170 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/gui/qt/widgets/time_series_widgets/trajectory_view_widget.py
+-rw-r--r--   0        0        0      134 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/test_test.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/utilities/__init__.py
+-rw-r--r--   0        0        0     2458 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/utilities/freemocap_data_loader.py
+-rw-r--r--   0        0        0      691 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/utilities/get_video_paths.py
+-rw-r--r--   0        0        0      832 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/utilities/load_sample_data.py
+-rw-r--r--   0        0        0     6077 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/utilities/mediapipe_skeleton_builder.py
+-rw-r--r--   0        0        0     1809 2024-04-25 16:31:19.269834 skelly_viewer-2024.4.1022/skelly_viewer/utilities/video_handler.py
+-rw-r--r--   0        0        0     1851 1970-01-01 00:00:00.000000 skelly_viewer-2024.4.1022/PKG-INFO
```

### Comparing `skelly_viewer-2024.3.1021/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml` & `skelly_viewer-2024.4.1022/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2024.3.1021/.gitignore` & `skelly_viewer-2024.4.1022/.gitignore`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2024.3.1021/LICENSE` & `skelly_viewer-2024.4.1022/LICENSE`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2024.3.1021/README.md` & `skelly_viewer-2024.4.1022/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Installation
 
-Create a conda environment using Python 3.9 (though 3.8/3.10 should work too, if that matters) and activate your conda environment 
+Create a conda environment using Python 3.11 (recommended, untested on other versions) and activate your conda environment 
 
 Install skelly_viewer using `pip install skelly_viewer`
 
 # Usage
 
 After installing, in your conda terminal (with the right environment active), type `skelly_viewer'
```

### Comparing `skelly_viewer-2024.3.1021/pyproject.toml` & `skelly_viewer-2024.4.1022/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver] #bump the version by entering `bumpver update` in the terminal
-current_version = "v2024.03.1021"
+current_version = "v2024.04.1022"
 version_pattern = "vYYYY.0M.BUILD[-TAG]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `skelly_viewer-2024.3.1021/skelly_viewer/__init__.py` & `skelly_viewer-2024.4.1022/skelly_viewer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Top-level package for basic_template_repo."""
 
 __package_name__ = "skelly_viewer"
-__version__ = "v2024.03.1021"
+__version__ = "v2024.04.1022"
 
 __author__ = """Skelly FreeMoCap"""
 __email__ = "info@freemocap.org"
 __repo_owner_github_user_name__ = "freemocap"
 __repo_url__ = f"https://github.com/{__repo_owner_github_user_name__}/{__package_name__}/"
 __repo_issues_url__ = f"{__repo_url__}issues"
```

### Comparing `skelly_viewer-2024.3.1021/skelly_viewer/config/default_paths.py` & `skelly_viewer-2024.4.1022/skelly_viewer/config/default_paths.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2024.3.1021/skelly_viewer/config/logging_configuration.py` & `skelly_viewer-2024.4.1022/skelly_viewer/config/logging_configuration.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2024.3.1021/skelly_viewer/experimental/checkable_combo_box.py` & `skelly_viewer-2024.4.1022/skelly_viewer/experimental/checkable_combo_box.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2024.3.1021/skelly_viewer/experimental/plotly/plotly_gpt_anim_working1.py` & `skelly_viewer-2024.4.1022/skelly_viewer/experimental/plotly/plotly_gpt_anim_working1.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2024.3.1021/skelly_viewer/gui/qt/skelly_viewer_widget.py` & `skelly_viewer-2024.4.1022/skelly_viewer/gui/qt/skelly_viewer_widget.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2024.3.1021/skelly_viewer/gui/qt/skellyview_main_window.py` & `skelly_viewer-2024.4.1022/skelly_viewer/gui/qt/skellyview_main_window.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2024.3.1021/skelly_viewer/gui/qt/widgets/multi_video_display.py` & `skelly_viewer-2024.4.1022/skelly_viewer/gui/qt/widgets/multi_video_display.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2024.3.1021/skelly_viewer/gui/qt/widgets/skeleton_view_widget.py` & `skelly_viewer-2024.4.1022/skelly_viewer/gui/qt/widgets/skeleton_view_widget.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2024.3.1021/skelly_viewer/gui/qt/widgets/slider_widget.py` & `skelly_viewer-2024.4.1022/skelly_viewer/gui/qt/widgets/slider_widget.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2024.3.1021/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/marker_selector_widget.py` & `skelly_viewer-2024.4.1022/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/marker_selector_widget.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2024.3.1021/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/time_series_viewer_widget.py` & `skelly_viewer-2024.4.1022/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/time_series_viewer_widget.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2024.3.1021/skelly_viewer/gui/qt/widgets/time_series_widgets/trajectory_view_widget.py` & `skelly_viewer-2024.4.1022/skelly_viewer/gui/qt/widgets/time_series_widgets/trajectory_view_widget.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2024.3.1021/skelly_viewer/utilities/freemocap_data_loader.py` & `skelly_viewer-2024.4.1022/skelly_viewer/utilities/freemocap_data_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,16 +38,17 @@
 
         if 'mediapipe_body_3d_xyz.npy' in npy_path_list:
             return self.find_output_data_folder_path() / 'mediapipe_body_3d_xyz.npy'
 
         raise Exception(f"Could not find a skeleton NPY file in path {str(self.find_output_data_folder_path())}")
 
     def find_synchronized_videos_folder_path(self) -> Path:
-        for subfolder_path in self._recording_folder_path.iterdir():
-            if subfolder_path.name == 'annotated_videos':
-                return subfolder_path
-            if subfolder_path.name == 'synchronized_videos':
-                return subfolder_path
-            if subfolder_path.name == 'SyncedVideos':
-                return subfolder_path
+        subpaths = list(self._recording_folder_path.glob('*'))
+
+        if self._recording_folder_path / 'annotated_videos' in subpaths:
+            return self._recording_folder_path / 'annotated_videos'
+        if self._recording_folder_path / 'synchronized_videos' in subpaths:
+            return self._recording_folder_path / 'synchronized_videos'
+        if self._recording_folder_path / 'SyncedVideos' in subpaths:
+            return self._recording_folder_path / 'SyncedVideos'
 
         raise Exception(f"Could not find a videos folder in path {str(self._recording_folder_path)}")
```

### Comparing `skelly_viewer-2024.3.1021/skelly_viewer/utilities/get_video_paths.py` & `skelly_viewer-2024.4.1022/skelly_viewer/utilities/get_video_paths.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2024.3.1021/skelly_viewer/utilities/load_sample_data.py` & `skelly_viewer-2024.4.1022/skelly_viewer/utilities/load_sample_data.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2024.3.1021/skelly_viewer/utilities/mediapipe_skeleton_builder.py` & `skelly_viewer-2024.4.1022/skelly_viewer/utilities/mediapipe_skeleton_builder.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2024.3.1021/skelly_viewer/utilities/video_handler.py` & `skelly_viewer-2024.4.1022/skelly_viewer/utilities/video_handler.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2024.3.1021/PKG-INFO` & `skelly_viewer-2024.4.1022/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skelly_viewer
-Version: 2024.3.1021
+Version: 2024.4.1022
 Summary: View a skelly
 Keywords: basic,template,python,repository
 Author-email: Skelly FreeMoCap <info@freemocap.org>
 Requires-Python: >=3.9,<3.12
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
@@ -21,15 +21,15 @@
 Requires-Dist: isort ; extra == "dev"
 Requires-Dist: pip-tools ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Provides-Extra: dev
 
 # Installation
 
-Create a conda environment using Python 3.9 (though 3.8/3.10 should work too, if that matters) and activate your conda environment 
+Create a conda environment using Python 3.11 (recommended, untested on other versions) and activate your conda environment 
 
 Install skelly_viewer using `pip install skelly_viewer`
 
 # Usage
 
 After installing, in your conda terminal (with the right environment active), type `skelly_viewer'
```


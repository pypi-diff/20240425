# Comparing `tmp/face_rhythm-0.2.4.tar.gz` & `tmp/face_rhythm-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "face_rhythm-0.2.4.tar", last modified: Wed Mar  6 04:26:48 2024, max compression
+gzip compressed data, was "face_rhythm-0.2.5.tar", last modified: Thu Apr 25 05:04:06 2024, max compression
```

## Comparing `face_rhythm-0.2.4.tar` & `face_rhythm-0.2.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 04:26:48.092897 face_rhythm-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-06 04:26:41.000000 face_rhythm-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-06 04:26:41.000000 face_rhythm-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12905 2024-03-06 04:26:48.092897 face_rhythm-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-03-06 04:26:41.000000 face_rhythm-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 04:26:48.080897 face_rhythm-0.2.4/face_rhythm/
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-03-06 04:26:41.000000 face_rhythm-0.2.4/face_rhythm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-03-06 04:26:41.000000 face_rhythm-0.2.4/face_rhythm/data_importing.py
--rw-r--r--   0 runner    (1001) docker     (127)    32003 2024-03-06 04:26:41.000000 face_rhythm-0.2.4/face_rhythm/decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)    11872 2024-03-06 04:26:41.000000 face_rhythm-0.2.4/face_rhythm/h5_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)   163845 2024-03-06 04:26:41.000000 face_rhythm-0.2.4/face_rhythm/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15836 2024-03-06 04:26:41.000000 face_rhythm-0.2.4/face_rhythm/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)    30371 2024-03-06 04:26:41.000000 face_rhythm-0.2.4/face_rhythm/point_tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-03-06 04:26:41.000000 face_rhythm-0.2.4/face_rhythm/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    67744 2024-03-06 04:26:41.000000 face_rhythm-0.2.4/face_rhythm/rois.py
--rw-r--r--   0 runner    (1001) docker     (127)    14544 2024-03-06 04:26:41.000000 face_rhythm-0.2.4/face_rhythm/spectral_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    48471 2024-03-06 04:26:41.000000 face_rhythm-0.2.4/face_rhythm/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    31423 2024-03-06 04:26:41.000000 face_rhythm-0.2.4/face_rhythm/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 04:26:48.080897 face_rhythm-0.2.4/face_rhythm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12905 2024-03-06 04:26:48.000000 face_rhythm-0.2.4/face_rhythm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-06 04:26:48.000000 face_rhythm-0.2.4/face_rhythm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 04:26:48.000000 face_rhythm-0.2.4/face_rhythm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-03-06 04:26:48.000000 face_rhythm-0.2.4/face_rhythm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-06 04:26:48.000000 face_rhythm-0.2.4/face_rhythm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-06 04:26:42.000000 face_rhythm-0.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-06 04:26:48.092897 face_rhythm-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-03-06 04:26:42.000000 face_rhythm-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 04:26:48.080897 face_rhythm-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-03-06 04:26:42.000000 face_rhythm-0.2.4/tests/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-03-06 04:26:42.000000 face_rhythm-0.2.4/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-06 04:26:42.000000 face_rhythm-0.2.4/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 05:04:06.428621 face_rhythm-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-25 05:04:01.000000 face_rhythm-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-25 05:04:01.000000 face_rhythm-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-04-25 05:04:06.428621 face_rhythm-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-04-25 05:04:01.000000 face_rhythm-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 05:04:06.416621 face_rhythm-0.2.5/face_rhythm/
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-25 05:04:01.000000 face_rhythm-0.2.5/face_rhythm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-04-25 05:04:01.000000 face_rhythm-0.2.5/face_rhythm/data_importing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32003 2024-04-25 05:04:01.000000 face_rhythm-0.2.5/face_rhythm/decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11872 2024-04-25 05:04:01.000000 face_rhythm-0.2.5/face_rhythm/h5_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)   163845 2024-04-25 05:04:01.000000 face_rhythm-0.2.5/face_rhythm/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15836 2024-04-25 05:04:01.000000 face_rhythm-0.2.5/face_rhythm/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30371 2024-04-25 05:04:01.000000 face_rhythm-0.2.5/face_rhythm/point_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-04-25 05:04:01.000000 face_rhythm-0.2.5/face_rhythm/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67744 2024-04-25 05:04:01.000000 face_rhythm-0.2.5/face_rhythm/rois.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15192 2024-04-25 05:04:01.000000 face_rhythm-0.2.5/face_rhythm/spectral_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48471 2024-04-25 05:04:01.000000 face_rhythm-0.2.5/face_rhythm/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31916 2024-04-25 05:04:01.000000 face_rhythm-0.2.5/face_rhythm/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 05:04:06.420621 face_rhythm-0.2.5/face_rhythm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-04-25 05:04:06.000000 face_rhythm-0.2.5/face_rhythm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-25 05:04:06.000000 face_rhythm-0.2.5/face_rhythm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 05:04:06.000000 face_rhythm-0.2.5/face_rhythm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-25 05:04:06.000000 face_rhythm-0.2.5/face_rhythm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 05:04:06.000000 face_rhythm-0.2.5/face_rhythm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-25 05:04:01.000000 face_rhythm-0.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-25 05:04:06.428621 face_rhythm-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-25 05:04:01.000000 face_rhythm-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 05:04:06.420621 face_rhythm-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-25 05:04:02.000000 face_rhythm-0.2.5/tests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-04-25 05:04:02.000000 face_rhythm-0.2.5/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-25 05:04:02.000000 face_rhythm-0.2.5/tests/test_unit.py
```

### Comparing `face_rhythm-0.2.4/PKG-INFO` & `face_rhythm-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: face_rhythm
-Version: 0.2.4
+Version: 0.2.5
 Summary: A pipeline for analysis of facial behavior using optical flow
 Home-page: https://github.com/RichieHakim/face-rhythm
 Author: Rich Hakim
 License: LICENSE
 Keywords: neuroscience,neuroimaging,machine learning
 Platform: Any
 Classifier: Development Status :: 4 - Beta
@@ -16,15 +16,15 @@
 Provides-Extra: all
 Requires-Dist: numpy==1.26.4; extra == "all"
 Requires-Dist: jupyter; extra == "all"
 Requires-Dist: notebook<7; extra == "all"
 Requires-Dist: tensorly==0.8.1; extra == "all"
 Requires-Dist: opencv_contrib_python==4.9.0.80; extra == "all"
 Requires-Dist: matplotlib; extra == "all"
-Requires-Dist: scikit_learn==1.4.1.post1; extra == "all"
+Requires-Dist: scikit_learn==1.4.2; extra == "all"
 Requires-Dist: scikit_image; extra == "all"
 Requires-Dist: pyyaml; extra == "all"
 Requires-Dist: tqdm; extra == "all"
 Requires-Dist: h5py; extra == "all"
 Requires-Dist: ipywidgets; extra == "all"
 Requires-Dist: Pillow; extra == "all"
 Requires-Dist: eva_decord; extra == "all"
@@ -72,15 +72,15 @@
 Provides-Extra: all-cv2headless
 Requires-Dist: numpy==1.26.4; extra == "all-cv2headless"
 Requires-Dist: jupyter; extra == "all-cv2headless"
 Requires-Dist: notebook<7; extra == "all-cv2headless"
 Requires-Dist: tensorly==0.8.1; extra == "all-cv2headless"
 Requires-Dist: opencv_contrib_python_headless<=4.9.0.80; extra == "all-cv2headless"
 Requires-Dist: matplotlib; extra == "all-cv2headless"
-Requires-Dist: scikit_learn==1.4.1.post1; extra == "all-cv2headless"
+Requires-Dist: scikit_learn==1.4.2; extra == "all-cv2headless"
 Requires-Dist: scikit_image; extra == "all-cv2headless"
 Requires-Dist: pyyaml; extra == "all-cv2headless"
 Requires-Dist: tqdm; extra == "all-cv2headless"
 Requires-Dist: h5py; extra == "all-cv2headless"
 Requires-Dist: ipywidgets; extra == "all-cv2headless"
 Requires-Dist: Pillow; extra == "all-cv2headless"
 Requires-Dist: eva_decord; extra == "all-cv2headless"
@@ -128,15 +128,15 @@
 Provides-Extra: core
 Requires-Dist: numpy==1.26.4; extra == "core"
 Requires-Dist: jupyter; extra == "core"
 Requires-Dist: notebook<7; extra == "core"
 Requires-Dist: tensorly==0.8.1; extra == "core"
 Requires-Dist: opencv_contrib_python==4.9.0.80; extra == "core"
 Requires-Dist: matplotlib; extra == "core"
-Requires-Dist: scikit_learn==1.4.1.post1; extra == "core"
+Requires-Dist: scikit_learn==1.4.2; extra == "core"
 Requires-Dist: scikit_image; extra == "core"
 Requires-Dist: pyyaml; extra == "core"
 Requires-Dist: tqdm; extra == "core"
 Requires-Dist: h5py; extra == "core"
 Requires-Dist: ipywidgets; extra == "core"
 Requires-Dist: Pillow; extra == "core"
 Requires-Dist: eva_decord; extra == "core"
```

### Comparing `face_rhythm-0.2.4/README.md` & `face_rhythm-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.2.4/face_rhythm/__init__.py` & `face_rhythm-0.2.5/face_rhythm/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     # 'tests',
 ]
 
 import torch  ## For some reason, it crashes if I don't import torch before other packages... RH 20221128
 
 
 ## Prepare cv2.imshow
-import pkg_resources
-installed_packages = {pkg.key for pkg in pkg_resources.working_set}
+import importlib.metadata
+installed_packages = {dist.metadata['Name'] for dist in importlib.metadata.distributions()}
 has_cv2_headless = 'opencv-contrib-python-headless' in installed_packages
 has_cv2_normal = 'opencv-contrib-python' in installed_packages
 if has_cv2_normal and not has_cv2_headless:
     run_cv2_imshow = True
 elif has_cv2_headless and not has_cv2_normal:
     run_cv2_imshow = False
 elif has_cv2_headless and has_cv2_normal:
@@ -62,8 +62,8 @@
     prepare_cv2_imshow()
 
 
 for pkg in __all__:
     exec('from . import ' + pkg)
 
 
-__version__ = '0.2.4'
+__version__ = '0.2.5'
```

### Comparing `face_rhythm-0.2.4/face_rhythm/data_importing.py` & `face_rhythm-0.2.5/face_rhythm/data_importing.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.2.4/face_rhythm/decomposition.py` & `face_rhythm-0.2.5/face_rhythm/decomposition.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.2.4/face_rhythm/h5_handling.py` & `face_rhythm-0.2.5/face_rhythm/h5_handling.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.2.4/face_rhythm/helpers.py` & `face_rhythm-0.2.5/face_rhythm/helpers.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.2.4/face_rhythm/pipelines.py` & `face_rhythm-0.2.5/face_rhythm/pipelines.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.2.4/face_rhythm/point_tracking.py` & `face_rhythm-0.2.5/face_rhythm/point_tracking.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.2.4/face_rhythm/project.py` & `face_rhythm-0.2.5/face_rhythm/project.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.2.4/face_rhythm/rois.py` & `face_rhythm-0.2.5/face_rhythm/rois.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.2.4/face_rhythm/spectral_analysis.py` & `face_rhythm-0.2.5/face_rhythm/spectral_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,28 @@
 
 class VQT_Analyzer(FR_Module):
     """
     A class for generating normalized spectrograms for point
      displacement traces. The spectrograms are generated using
      the Variable Q-Transform (VQT) algorithm.
     RH 2022
+
+    Args:
+        params_VQT (dict):
+            A dictionary of parameters to pass to the VQT class (Variable
+            Q-Transform) in helpers.py.
+        normalization_factor (float):
+            A float between 0 and 1 to normalize the spectrograms. 0 means no
+            normalization. 1 means every time point has the same power.
+        spectrogram_exponent (float):
+            A float to raise the spectrogram to before normalizing.
+        one_over_f_exponent (float):
+            A float to raise the frequency axis to before doing 1/f correction.
+        verbose (int):
+            An integer to control the verbosity of the class.
     """
     def __init__(
         self,
         params_VQT: dict={
             'Fs_sample': 90,
             'Q_lowF': 3,
             'Q_highF': 20,
```

### Comparing `face_rhythm-0.2.4/face_rhythm/util.py` & `face_rhythm-0.2.5/face_rhythm/util.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.2.4/face_rhythm/visualization.py` & `face_rhythm-0.2.5/face_rhythm/visualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Union
 from pathlib import Path
 import copy
+import gc
 
 import numpy as np
 import cv2
 import torch
 # import scipy.sparse
 from tqdm import tqdm
 
@@ -116,15 +117,15 @@
             text_thickness (int or list):
                 OPTIONAL. Can be set during call to visualize_image_with_points.
                 Used as argument for cv2.putText.
                 If int: All text will be this thickness.
                 If list: Each element is a thickness for a different text.
                     Length of list must match the length of text.
         """
-        ## Stor arguments
+        ## Store arguments
         self.point_sizes = point_sizes if point_sizes is not None else None
         self.points_colors = points_colors if points_colors is not None else None
         self.alpha = alpha if alpha is not None else None
         self.text = text if text is not None else None
         self.text_positions = text_positions if text_positions is not None else None
         self.text_color = text_color if text_color is not None else None
         self.text_size = text_size if text_size is not None else None
@@ -411,30 +412,29 @@
         if self.video_writer is not None:
             self.video_writer.write(image_out)
 
         return image_out
 
     def close(self):
         if self.video_writer is not None:
-            self.video_writer.release()
             cv2.destroyWindow(self.handle_cv2Imshow)
+            try:
+                self.video_writer.release()
+            except:
+                pass
 
     def __call__(self, *args, **kwds):
         """
         Calls self.visualize_image_with_points(*args, **kwds).
         See that function for details.
         """
         self.visualize_image_with_points(*args, **kwds)
     def __del__(self):
         self.close()
-    def __exit__(self):
-        self.close()
-    def __enter__(self):
-        return self
-    
+
     def __repr__(self):
         return f'FrameVisualizer(handle_cv2Imshow={self.handle_cv2Imshow}, display={self.display}, video_writer={self.video_writer}, path_video={self.path_save}, frame_rate={self.frame_rate}, frame_height_width={self.frame_height_width})'
 
 
 def play_video_with_points(
         bufferedVideoReader,
         frameVisualizer=None,
@@ -473,23 +473,34 @@
         ## Prep points
         points_int = points.astype(int) if points is not None else None
 
         ## Loop through frames
         ### Set buffered video reader to first frame
         bufferedVideoReader.set_iterator_frame_idx(int(idx_frames[0]))
         ### Iterate through frames
-        for idx_frame in tqdm(idx_frames):
-            frame = bufferedVideoReader[idx_frame][0]
-            frame = frame.numpy() if isinstance(frame, torch.Tensor) else frame
-            p = points_int[idx_frame] if points_int is not None else None
-            frameVisualizer.visualize_image_with_points(
-                image=frame,
-                points=[p],
-            )
-        frameVisualizer.close()
+        ### Use context manager to close frameVisualizer
+        class CM:
+            def __init__(self, frameVisualizer):
+                self.frameVisualizer = frameVisualizer
+            def __enter__(self):
+                return self.frameVisualizer
+            def __exit__(self, exc_type, exc_value, traceback):
+                self.frameVisualizer.close()
+                cv2.destroyWindow(self.frameVisualizer.handle_cv2Imshow)
+                gc.collect()
+        with CM(frameVisualizer) as f:
+            for idx_frame in tqdm(idx_frames):
+                frame = bufferedVideoReader[idx_frame][0]
+                frame = frame.numpy() if isinstance(frame, torch.Tensor) else frame
+                p = points_int[idx_frame] if points_int is not None else None
+                f.visualize_image_with_points(
+                    image=frame,
+                    points=[p],
+                )
+            f.close()
 
 
 # def display_toggle_image_stack(images, clim=None, **kwargs):
 #     """
 #     Display a stack of images using a slider.
 #     REQUIRES use of Jupyter Notebook.
 #     RH 2022
```

### Comparing `face_rhythm-0.2.4/face_rhythm.egg-info/PKG-INFO` & `face_rhythm-0.2.5/face_rhythm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: face_rhythm
-Version: 0.2.4
+Version: 0.2.5
 Summary: A pipeline for analysis of facial behavior using optical flow
 Home-page: https://github.com/RichieHakim/face-rhythm
 Author: Rich Hakim
 License: LICENSE
 Keywords: neuroscience,neuroimaging,machine learning
 Platform: Any
 Classifier: Development Status :: 4 - Beta
@@ -16,15 +16,15 @@
 Provides-Extra: all
 Requires-Dist: numpy==1.26.4; extra == "all"
 Requires-Dist: jupyter; extra == "all"
 Requires-Dist: notebook<7; extra == "all"
 Requires-Dist: tensorly==0.8.1; extra == "all"
 Requires-Dist: opencv_contrib_python==4.9.0.80; extra == "all"
 Requires-Dist: matplotlib; extra == "all"
-Requires-Dist: scikit_learn==1.4.1.post1; extra == "all"
+Requires-Dist: scikit_learn==1.4.2; extra == "all"
 Requires-Dist: scikit_image; extra == "all"
 Requires-Dist: pyyaml; extra == "all"
 Requires-Dist: tqdm; extra == "all"
 Requires-Dist: h5py; extra == "all"
 Requires-Dist: ipywidgets; extra == "all"
 Requires-Dist: Pillow; extra == "all"
 Requires-Dist: eva_decord; extra == "all"
@@ -72,15 +72,15 @@
 Provides-Extra: all-cv2headless
 Requires-Dist: numpy==1.26.4; extra == "all-cv2headless"
 Requires-Dist: jupyter; extra == "all-cv2headless"
 Requires-Dist: notebook<7; extra == "all-cv2headless"
 Requires-Dist: tensorly==0.8.1; extra == "all-cv2headless"
 Requires-Dist: opencv_contrib_python_headless<=4.9.0.80; extra == "all-cv2headless"
 Requires-Dist: matplotlib; extra == "all-cv2headless"
-Requires-Dist: scikit_learn==1.4.1.post1; extra == "all-cv2headless"
+Requires-Dist: scikit_learn==1.4.2; extra == "all-cv2headless"
 Requires-Dist: scikit_image; extra == "all-cv2headless"
 Requires-Dist: pyyaml; extra == "all-cv2headless"
 Requires-Dist: tqdm; extra == "all-cv2headless"
 Requires-Dist: h5py; extra == "all-cv2headless"
 Requires-Dist: ipywidgets; extra == "all-cv2headless"
 Requires-Dist: Pillow; extra == "all-cv2headless"
 Requires-Dist: eva_decord; extra == "all-cv2headless"
@@ -128,15 +128,15 @@
 Provides-Extra: core
 Requires-Dist: numpy==1.26.4; extra == "core"
 Requires-Dist: jupyter; extra == "core"
 Requires-Dist: notebook<7; extra == "core"
 Requires-Dist: tensorly==0.8.1; extra == "core"
 Requires-Dist: opencv_contrib_python==4.9.0.80; extra == "core"
 Requires-Dist: matplotlib; extra == "core"
-Requires-Dist: scikit_learn==1.4.1.post1; extra == "core"
+Requires-Dist: scikit_learn==1.4.2; extra == "core"
 Requires-Dist: scikit_image; extra == "core"
 Requires-Dist: pyyaml; extra == "core"
 Requires-Dist: tqdm; extra == "core"
 Requires-Dist: h5py; extra == "core"
 Requires-Dist: ipywidgets; extra == "core"
 Requires-Dist: Pillow; extra == "core"
 Requires-Dist: eva_decord; extra == "core"
```

### Comparing `face_rhythm-0.2.4/face_rhythm.egg-info/SOURCES.txt` & `face_rhythm-0.2.5/face_rhythm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.2.4/face_rhythm.egg-info/requires.txt` & `face_rhythm-0.2.5/face_rhythm.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [all]
 numpy==1.26.4
 jupyter
 notebook<7
 tensorly==0.8.1
 opencv_contrib_python==4.9.0.80
 matplotlib
-scikit_learn==1.4.1.post1
+scikit_learn==1.4.2
 scikit_image
 pyyaml
 tqdm
 h5py
 ipywidgets
 Pillow
 eva_decord
@@ -31,15 +31,15 @@
 [all_cv2Headless]
 numpy==1.26.4
 jupyter
 notebook<7
 tensorly==0.8.1
 opencv_contrib_python_headless<=4.9.0.80
 matplotlib
-scikit_learn==1.4.1.post1
+scikit_learn==1.4.2
 scikit_image
 pyyaml
 tqdm
 h5py
 ipywidgets
 Pillow
 eva_decord
@@ -118,15 +118,15 @@
 [core]
 numpy==1.26.4
 jupyter
 notebook<7
 tensorly==0.8.1
 opencv_contrib_python==4.9.0.80
 matplotlib
-scikit_learn==1.4.1.post1
+scikit_learn==1.4.2
 scikit_image
 pyyaml
 tqdm
 h5py
 ipywidgets
 Pillow
 eva_decord
```

### Comparing `face_rhythm-0.2.4/setup.py` & `face_rhythm-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.2.4/tests/test_environment.py` & `face_rhythm-0.2.5/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.2.4/tests/test_integration.py` & `face_rhythm-0.2.5/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.2.4/tests/test_unit.py` & `face_rhythm-0.2.5/tests/test_unit.py`

 * *Files identical despite different names*


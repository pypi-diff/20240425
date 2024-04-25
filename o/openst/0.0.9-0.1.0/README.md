# Comparing `tmp/openst-0.0.9.tar.gz` & `tmp/openst-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openst-0.0.9.tar", max compression
+gzip compressed data, was "openst-0.1.0.tar", max compression
```

## Comparing `openst-0.0.9.tar` & `openst-0.1.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0      896 2024-02-14 16:40:20.599326 openst-0.0.9/LICENSE
--rw-r--r--   0        0        0     4235 2024-04-15 10:07:14.979891 openst-0.0.9/README.md
--rw-r--r--   0        0        0       21 2024-02-14 16:40:22.603322 openst-0.0.9/openst/__init__.py
--rw-r--r--   0        0        0      231 2024-04-11 08:32:57.910641 openst-0.0.9/openst/__main__.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.611322 openst-0.0.9/openst/alignment/__init__.py
--rw-r--r--   0        0        0     5878 2024-04-15 14:54:16.746512 openst-0.0.9/openst/alignment/apply_transform.py
--rw-r--r--   0        0        0    11893 2024-02-14 16:40:22.619322 openst-0.0.9/openst/alignment/feature_matching.py
--rw-r--r--   0        0        0     3628 2024-02-14 16:40:22.623322 openst-0.0.9/openst/alignment/fiducial_detection.py
--rw-r--r--   0        0        0    51224 2024-04-15 14:54:16.750512 openst-0.0.9/openst/alignment/manual_pairwise_aligner.py
--rw-r--r--   0        0        0    25638 2024-04-16 05:22:16.053579 openst-0.0.9/openst/alignment/pairwise_aligner.py
--rw-r--r--   0        0        0     5507 2024-04-16 05:18:17.738134 openst-0.0.9/openst/alignment/transcript_assign.py
--rw-r--r--   0        0        0      798 2024-04-15 14:54:16.758512 openst-0.0.9/openst/alignment/transformation.py
--rw-r--r--   0        0        0    47613 2024-04-15 14:54:16.762512 openst-0.0.9/openst/cli.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.655321 openst-0.0.9/openst/metadata/__init__.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.659321 openst-0.0.9/openst/metadata/classes/__init__.py
--rw-r--r--   0        0        0     2906 2024-02-14 16:40:22.663322 openst-0.0.9/openst/metadata/classes/base.py
--rw-r--r--   0        0        0     3406 2024-04-15 14:54:16.762512 openst-0.0.9/openst/metadata/classes/pairwise_alignment.py
--rw-r--r--   0        0        0     1798 2024-02-14 16:40:22.679321 openst-0.0.9/openst/metadata/classes/segmentation.py
--rw-r--r--   0        0        0     3787 2024-02-14 16:40:22.683321 openst-0.0.9/openst/metadata/example_json.json
--rw-r--r--   0        0        0     1450 2024-04-12 13:55:27.459067 openst-0.0.9/openst/metadata/report.py
--rw-r--r--   0        0        0  1187390 2024-02-14 16:40:22.715321 openst-0.0.9/openst/metadata/templates/pairwise_alignment.html
--rw-r--r--   0        0        0     1745 2024-02-14 16:40:22.723321 openst-0.0.9/openst/preprocessing/CUT/README.md
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.723321 openst-0.0.9/openst/preprocessing/CUT/__init__.py
--rw-r--r--   0        0        0     3072 2024-02-14 16:40:22.731321 openst-0.0.9/openst/preprocessing/CUT/models/__init__.py
--rw-r--r--   0        0        0    11223 2024-02-14 16:40:22.735321 openst-0.0.9/openst/preprocessing/CUT/models/base_model.py
--rw-r--r--   0        0        0    10228 2024-02-14 16:40:22.739321 openst-0.0.9/openst/preprocessing/CUT/models/cut_model.py
--rw-r--r--   0        0        0    60639 2024-02-14 16:40:22.747321 openst-0.0.9/openst/preprocessing/CUT/models/networks.py
--rw-r--r--   0        0        0     5953 2024-02-14 16:40:22.751321 openst-0.0.9/openst/preprocessing/CUT/models/template_model.py
--rw-r--r--   0        0        0      136 2024-02-14 16:40:22.755321 openst-0.0.9/openst/preprocessing/CUT/options/__init__.py
--rw-r--r--   0        0        0     9720 2024-02-14 16:40:22.763321 openst-0.0.9/openst/preprocessing/CUT/options/base_options.py
--rw-r--r--   0        0        0      975 2024-02-14 16:40:22.767321 openst-0.0.9/openst/preprocessing/CUT/options/test_options.py
--rw-r--r--   0        0        0      102 2024-02-14 16:40:22.775321 openst-0.0.9/openst/preprocessing/CUT/util/__init__.py
--rw-r--r--   0        0        0     2226 2024-02-14 16:40:22.779321 openst-0.0.9/openst/preprocessing/CUT/util/image_pool.py
--rw-r--r--   0        0        0     5135 2024-02-14 16:40:22.783321 openst-0.0.9/openst/preprocessing/CUT/util/util.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.787321 openst-0.0.9/openst/preprocessing/__init__.py
--rw-r--r--   0        0        0     4005 2024-04-12 13:55:27.459067 openst-0.0.9/openst/preprocessing/barcode_preprocessing.py
--rw-r--r--   0        0        0     2194 2024-04-15 14:53:45.590507 openst-0.0.9/openst/preprocessing/image_preprocess.py
--rw-r--r--   0        0        0     4607 2024-04-15 14:54:16.766512 openst-0.0.9/openst/preprocessing/image_stitch.py
--rw-r--r--   0        0        0      690 2024-02-14 16:40:22.811321 openst-0.0.9/openst/preprocessing/imagej_macros/keyence_stitch.ijm
--rw-r--r--   0        0        0      833 2024-04-12 13:55:27.459067 openst-0.0.9/openst/preprocessing/merge_modalities.py
--rw-r--r--   0        0        0     8996 2024-04-15 14:54:16.766512 openst-0.0.9/openst/preprocessing/spatial_stitch.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.819321 openst-0.0.9/openst/segmentation/__init__.py
--rw-r--r--   0        0        0    14684 2024-04-12 13:55:27.463067 openst-0.0.9/openst/segmentation/segment.py
--rw-r--r--   0        0        0     3842 2024-04-15 14:54:16.770512 openst-0.0.9/openst/segmentation/segment_merge.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.827321 openst-0.0.9/openst/threed/__init__.py
--rw-r--r--   0        0        0     9811 2024-04-12 13:55:27.463067 openst-0.0.9/openst/threed/from_3d_registration.py
--rw-r--r--   0        0        0     2500 2024-04-12 13:55:27.467067 openst-0.0.9/openst/threed/to_3d_registration.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.843321 openst-0.0.9/openst/utils/__init__.py
--rw-r--r--   0        0        0     8010 2024-04-15 14:54:16.778512 openst-0.0.9/openst/utils/file.py
--rw-r--r--   0        0        0    13953 2024-04-15 14:54:16.778512 openst-0.0.9/openst/utils/from_spacemake.py
--rw-r--r--   0        0        0     9651 2024-04-15 14:54:16.782512 openst-0.0.9/openst/utils/pimage.py
--rw-r--r--   0        0        0     3018 2024-02-14 16:40:22.859321 openst-0.0.9/openst/utils/points.py
--rw-r--r--   0        0        0     2419 2024-04-15 14:54:16.786512 openst-0.0.9/openst/utils/preview.py
--rw-r--r--   0        0        0    10068 2024-04-15 14:54:16.786512 openst-0.0.9/openst/utils/pseudoimage.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.867321 openst-0.0.9/openst/utils/scanpy/__init__.py
--rw-r--r--   0        0        0       37 2024-02-14 16:40:22.875321 openst-0.0.9/openst/utils/scanpy/pp/__init__.py
--rw-r--r--   0        0        0    10779 2024-02-14 16:40:22.879321 openst-0.0.9/openst/utils/scanpy/pp/_qc.py
--rw-r--r--   0        0        0     3737 2024-04-16 05:17:10.030292 openst-0.0.9/openst/utils/spacemake.py
--rw-r--r--   0        0        0     1985 2024-04-16 05:07:27.559664 openst-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     6373 1970-01-01 00:00:00.000000 openst-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      896 2024-04-18 14:20:31.331344 openst-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4265 2024-04-25 15:58:08.164649 openst-0.1.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-25 15:58:08.252649 openst-0.1.0/openst/__init__.py
+-rw-r--r--   0        0        0      358 2024-04-25 16:16:49.572600 openst-0.1.0/openst/__main__.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.611322 openst-0.1.0/openst/alignment/__init__.py
+-rw-r--r--   0        0        0     5878 2024-04-18 13:23:51.785039 openst-0.1.0/openst/alignment/apply_transform.py
+-rw-r--r--   0        0        0    12248 2024-04-25 16:16:49.576600 openst-0.1.0/openst/alignment/feature_matching.py
+-rw-r--r--   0        0        0     3628 2024-02-14 16:40:22.623322 openst-0.1.0/openst/alignment/fiducial_detection.py
+-rw-r--r--   0        0        0    50862 2024-04-25 16:16:49.580600 openst-0.1.0/openst/alignment/manual_pairwise_aligner.py
+-rw-r--r--   0        0        0    23898 2024-04-25 16:16:49.580600 openst-0.1.0/openst/alignment/pairwise_aligner.py
+-rw-r--r--   0        0        0     5505 2024-04-25 15:58:08.256649 openst-0.1.0/openst/alignment/transcript_assign.py
+-rw-r--r--   0        0        0      798 2024-04-18 13:23:51.825039 openst-0.1.0/openst/alignment/transformation.py
+-rw-r--r--   0        0        0    47711 2024-04-25 16:16:49.584600 openst-0.1.0/openst/cli.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.655321 openst-0.1.0/openst/metadata/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.659321 openst-0.1.0/openst/metadata/classes/__init__.py
+-rw-r--r--   0        0        0     2899 2024-04-25 16:16:49.588600 openst-0.1.0/openst/metadata/classes/base.py
+-rw-r--r--   0        0        0     3539 2024-04-25 16:16:49.592600 openst-0.1.0/openst/metadata/classes/pairwise_alignment.py
+-rw-r--r--   0        0        0     1798 2024-02-14 16:40:22.679321 openst-0.1.0/openst/metadata/classes/segmentation.py
+-rw-r--r--   0        0        0     3787 2024-02-14 16:40:22.683321 openst-0.1.0/openst/metadata/example_json.json
+-rw-r--r--   0        0        0     1450 2024-04-18 13:23:51.849039 openst-0.1.0/openst/metadata/report.py
+-rw-r--r--   0        0        0  1187390 2024-02-14 16:40:22.715321 openst-0.1.0/openst/metadata/templates/pairwise_alignment.html
+-rw-r--r--   0        0        0     1745 2024-02-14 16:40:22.723321 openst-0.1.0/openst/preprocessing/CUT/README.md
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.723321 openst-0.1.0/openst/preprocessing/CUT/__init__.py
+-rw-r--r--   0        0        0     3157 2024-04-25 15:58:08.256649 openst-0.1.0/openst/preprocessing/CUT/models/__init__.py
+-rw-r--r--   0        0        0    11347 2024-04-25 15:58:08.256649 openst-0.1.0/openst/preprocessing/CUT/models/base_model.py
+-rw-r--r--   0        0        0    10006 2024-04-25 15:58:08.256649 openst-0.1.0/openst/preprocessing/CUT/models/cut_model.py
+-rw-r--r--   0        0        0    59845 2024-04-25 15:58:08.260649 openst-0.1.0/openst/preprocessing/CUT/models/networks.py
+-rw-r--r--   0        0        0     2317 2024-04-25 15:58:08.260649 openst-0.1.0/openst/preprocessing/CUT/models/patchnce.py
+-rw-r--r--   0        0        0     6013 2024-04-25 15:58:08.260649 openst-0.1.0/openst/preprocessing/CUT/models/template_model.py
+-rw-r--r--   0        0        0      136 2024-02-14 16:40:22.755321 openst-0.1.0/openst/preprocessing/CUT/options/__init__.py
+-rw-r--r--   0        0        0     8760 2024-04-25 15:58:08.260649 openst-0.1.0/openst/preprocessing/CUT/options/base_options.py
+-rw-r--r--   0        0        0     1006 2024-04-25 15:58:08.260649 openst-0.1.0/openst/preprocessing/CUT/options/test_options.py
+-rw-r--r--   0        0        0      132 2024-04-25 15:58:08.264649 openst-0.1.0/openst/preprocessing/CUT/util/__init__.py
+-rw-r--r--   0        0        0     5135 2024-02-14 16:40:22.783321 openst-0.1.0/openst/preprocessing/CUT/util/util.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.787321 openst-0.1.0/openst/preprocessing/__init__.py
+-rw-r--r--   0        0        0     4102 2024-04-25 16:16:49.596600 openst-0.1.0/openst/preprocessing/barcode_preprocessing.py
+-rw-r--r--   0        0        0     7323 2024-04-25 15:58:08.264649 openst-0.1.0/openst/preprocessing/image_preprocess.py
+-rw-r--r--   0        0        0     4607 2024-04-18 13:23:51.877039 openst-0.1.0/openst/preprocessing/image_stitch.py
+-rw-r--r--   0        0        0      690 2024-02-14 16:40:22.811321 openst-0.1.0/openst/preprocessing/imagej_macros/keyence_stitch.ijm
+-rw-r--r--   0        0        0      833 2024-04-18 13:23:51.885039 openst-0.1.0/openst/preprocessing/merge_modalities.py
+-rw-r--r--   0        0        0     8996 2024-04-18 13:23:51.893039 openst-0.1.0/openst/preprocessing/spatial_stitch.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.819321 openst-0.1.0/openst/segmentation/__init__.py
+-rw-r--r--   0        0        0    14694 2024-04-25 15:58:08.264649 openst-0.1.0/openst/segmentation/segment.py
+-rw-r--r--   0        0        0     3842 2024-04-18 13:23:51.913039 openst-0.1.0/openst/segmentation/segment_merge.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.827321 openst-0.1.0/openst/threed/__init__.py
+-rw-r--r--   0        0        0     9811 2024-04-18 13:23:51.925039 openst-0.1.0/openst/threed/from_3d_registration.py
+-rw-r--r--   0        0        0     2500 2024-04-18 13:23:51.933039 openst-0.1.0/openst/threed/to_3d_registration.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.843321 openst-0.1.0/openst/utils/__init__.py
+-rw-r--r--   0        0        0     9843 2024-04-25 16:16:49.596600 openst-0.1.0/openst/utils/file.py
+-rw-r--r--   0        0        0    13953 2024-04-18 13:23:51.953039 openst-0.1.0/openst/utils/from_spacemake.py
+-rw-r--r--   0        0        0     9680 2024-04-25 16:16:49.600600 openst-0.1.0/openst/utils/pimage.py
+-rw-r--r--   0        0        0     3018 2024-02-14 16:40:22.859321 openst-0.1.0/openst/utils/points.py
+-rw-r--r--   0        0        0     2419 2024-04-18 13:23:51.969039 openst-0.1.0/openst/utils/preview.py
+-rw-r--r--   0        0        0    10060 2024-04-25 16:16:49.604600 openst-0.1.0/openst/utils/pseudoimage.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.867321 openst-0.1.0/openst/utils/scanpy/__init__.py
+-rw-r--r--   0        0        0       37 2024-02-14 16:40:22.875321 openst-0.1.0/openst/utils/scanpy/pp/__init__.py
+-rw-r--r--   0        0        0    10779 2024-02-14 16:40:22.879321 openst-0.1.0/openst/utils/scanpy/pp/_qc.py
+-rw-r--r--   0        0        0     3737 2024-04-18 13:23:51.997039 openst-0.1.0/openst/utils/spacemake.py
+-rw-r--r--   0        0        0     1991 2024-04-25 16:16:49.608600 openst-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 openst-0.1.0/PKG-INFO
```

### Comparing `openst-0.0.9/LICENSE` & `openst-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openst-0.0.9/README.md` & `openst-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![docs](https://github.com/rajewsky-lab/openst/actions/workflows/docs.yml/badge.svg)](https://github.com/rajewsky-lab/openst/actions/workflows/docs.yml)
+[![Publish Docker image](https://github.com/rajewsky-lab/openst/actions/workflows/docker_hub.yml/badge.svg)](https://github.com/rajewsky-lab/openst/actions/workflows/docker_hub.yml)
 [![Downloads](https://pepy.tech/badge/openst)](https://pepy.tech/project/openst)
 [![PyPI Version](https://img.shields.io/pypi/v/openst.svg)](https://pypi.org/project/openst)
 [![PyPI License](https://img.shields.io/pypi/l/openst.svg)](https://pypi.org/project/openst)
 [![Gitter chat](https://badges.gitter.im/openst/community.png)](https://gitter.im/openst/community)
-[![ci](https://github.com/rajewsky-lab/openst/actions/workflows/docs.yml/badge.svg)](https://github.com/rajewsky-lab/openst/actions/workflows/docs.yml)
 
 <img
   src="https://raw.githubusercontent.com/rajewsky-lab/openst/5617df9d35341778487d4c623eaac53b61000006/docs/static/img/openst_logo_color.png"
   class="dark-light" align="right" width="350" alt="image"
 />
 
 # Open-ST: open-source spatial transcriptomics
```

### Comparing `openst-0.0.9/openst/alignment/apply_transform.py` & `openst-0.1.0/openst/alignment/apply_transform.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.9/openst/alignment/feature_matching.py` & `openst-0.1.0/openst/alignment/feature_matching.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,16 +36,16 @@
             """Optional modules need to be installed to run thi s feature.
                Please run 'pip install kornia'"""
         )
 
     matcher = KF.LoFTR(pretrained=pretrained).to(device)
 
     input_dict = {
-        "image0": torch.tensor(im_0)[None, None].float().to(device),
-        "image1": torch.tensor(im_1)[None, None].float().to(device),
+        "image0": torch.tensor(im_0.copy())[None, None].float().to(device),
+        "image1": torch.tensor(im_1.copy())[None, None].float().to(device),
     }
 
     with torch.inference_mode():
         correspondences = matcher(input_dict)
 
     return correspondences["keypoints0"].cpu().numpy(), correspondences["keypoints1"].cpu().numpy()
 
@@ -267,14 +267,19 @@
             - The best flip of image B (yielding highest A/B matches)
             - The best rotation of image B (yielding highest A/B matches)
     """
     # TODO: check flips list
     # TODO: check rotations list
     # TODO: documentation
 
+    if (isinstance(src, list) and isinstance(src_augmenter, Callable)) \
+        or (isinstance(dst, list) and isinstance(dst_augmenter, Callable)):
+        raise NotImplementedError("Cannot run matching >1 src/dst images and an augmenter\n" +
+                                  "Please choose only one augmentation strategy")
+
     _src, _dst = src, dst
     max_keypoints = 0
     best_flip = flips[0]
     best_rotation = rotations[0]
     _best_mkpts0 = None
     _best_mkpts1 = None
 
@@ -309,16 +314,16 @@
 
                 if inliers.sum() > sum_inliers:
                     sum_inliers = inliers.sum()
                     best_inliers = inliers
         else:
             best_inliers = np.ones(len(mkpts0), dtype=bool)
 
-        if len(mkpts0) > max_keypoints:
-            max_keypoints = len(mkpts0)
+        if best_inliers.sum() > max_keypoints:
+            max_keypoints = best_inliers.sum()
             best_flip = [_flip_x, _flip_y]
             best_rotation = _rotation
 
             _best_mkpts0 = mkpts0[best_inliers.flatten()]
             _best_mkpts1 = mkpts1[best_inliers.flatten()]
 
         logging.info(f"{best_inliers.sum()} inliers (RANSAC)")
```

### Comparing `openst-0.0.9/openst/alignment/fiducial_detection.py` & `openst-0.1.0/openst/alignment/fiducial_detection.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.9/openst/alignment/manual_pairwise_aligner.py` & `openst-0.1.0/openst/alignment/manual_pairwise_aligner.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,61 +281,59 @@
 
         Returns:
             image_pair (dict): Dictionary containing the pseudoimages, cropping and scaling limits, rendering scale.
         """
         image_pair = {}
 
         self.update_text.emit(f"Rendering '{self.layer}'")
-        min_lim, max_lim = in_coords.min(axis=0).astype(int), in_coords.max(axis=0).astype(int)
-        x_all_min, y_all_min = min_lim
-        x_all_max, y_all_max = max_lim
-        
-        # Preparing images and preprocessing routines
-        _i_counts_above_threshold = total_counts > self.threshold_counts
-        sts_coords = in_coords[_i_counts_above_threshold]
-
-        # We keep the limits also when filtering by UMI (avoid issues with offsets)
-        sts_coords = np.concatenate([sts_coords, np.array([[x_all_max, y_all_max],
-                                                           [x_all_min, y_all_min]])])
+        sts_coords = in_coords[:]
+        _t_valid_coords = slice(None)
 
         if not self.recenter_coarse:
             _i_sts_coords_coarse_within_image_bounds = np.where(
-                (sts_coords[:, 0] > 0)
-                & (sts_coords[:, 0] < staining_image.shape[1])
-                & (sts_coords[:, 1] > 0)
-                & (sts_coords[:, 1] < staining_image.shape[0])
+                (sts_coords[:, 0] >= 0)
+                & (sts_coords[:, 0] <= staining_image.shape[1])
+                & (sts_coords[:, 1] >= 0)
+                & (sts_coords[:, 1] <= staining_image.shape[0])
             )
 
             if len(_i_sts_coords_coarse_within_image_bounds[0]) < 10:
                 raise ValueError("There are no spatial coordinates falling inside the image data.\n"+
                                  "Maybe spatial coordinates were never aligned to the image data.\n"+
                                  "Try enabling 'Is unaligned data' under 'Rendering settings' and render again.")
             sts_coords = sts_coords[_i_sts_coords_coarse_within_image_bounds]
+            tile_id = tile_id[_i_sts_coords_coarse_within_image_bounds]
+            total_counts = total_counts[_i_sts_coords_coarse_within_image_bounds]
+            _t_valid_coords = tile_id == int(self.layer) if self.layer != 'all_tiles_coarse' else slice(None)
+
+        min_lim, max_lim = sts_coords[_t_valid_coords].min(axis=0).astype(int), sts_coords[_t_valid_coords].max(axis=0).astype(int)
+        x_all_min, y_all_min = min_lim
+        x_all_max, y_all_max = max_lim
 
-        # if sts_coords.max(axis=0).max() > 10 * staining_image.shape.max():
-        #     raise ValueError("""The spatial coordinates are too large for the selected image\n
-        #                         Please choose a different rescaling factor!""")
+        # Preparing images and preprocessing routines
+        _i_counts_above_threshold = total_counts > self.threshold_counts
+        sts_coords = sts_coords[_i_counts_above_threshold]
+        tile_id = tile_id[_i_counts_above_threshold]
+
+        # We keep the limits also when filtering by UMI (avoid issues with offsets)
+        sts_coords = np.concatenate([sts_coords, np.array([[x_all_max, y_all_max],
+                                                        [x_all_min, y_all_min]])])
+        tile_id = np.concatenate([tile_id, [-1, -1]])
 
         # TODO: instead of this, we plot specific sections...
         if self.layer == "all_tiles_coarse":
             staining_image_rescaled = staining_image[:: self.rescale_factor_coarse, :: self.rescale_factor_coarse]
             sts_pseudoimage = create_paired_pseudoimage(
                 sts_coords[:, ::-1],
                 self.pseudoimg_size,
                 staining_image_rescaled.shape,
                 recenter=self.recenter_coarse,
                 resize_method="cv2",
             )
 
-            #sts_coords_to_transform = sts_pseudoimage["coords_rescaled"] * sts_pseudoimage["rescaling_factor"]
-            #min_lim, max_lim = sts_coords_to_transform.min(axis=0).astype(int), sts_coords_to_transform.max(axis=0).astype(int)
-            # min_lim, max_lim = sts_coords.min(axis=0).astype(int), sts_coords.max(axis=0).astype(int)
-            # x_min, y_min = min_lim
-            # x_max, y_max = max_lim
-
             image_pair = {
                 "imageA": staining_image_rescaled,
                 "imageB": sts_pseudoimage["pseudoimage"],
                 "lims": [0, 0, 0, 0], #[x_min, x_max, y_min, y_max],
                 "factor_rescale": self.rescale_factor_coarse,
                 "rescale_factor": sts_pseudoimage["rescale_factor"],
                 "rescaling_factor": sts_pseudoimage["rescaling_factor"],
@@ -343,17 +341,15 @@
                 "offset_factor": sts_pseudoimage["offset_factor"]
             }
             self.update_text.emit(f"Creating metadata for '{self.layer}'")
         else:
             # Apply scaling to input image again, for fine registration
             staining_image_rescaled = staining_image[:: self.rescale_factor_fine, :: self.rescale_factor_fine]
 
-            _t_valid_coords = tile_id[_i_counts_above_threshold][_i_sts_coords_coarse_within_image_bounds] == int(
-                self.layer
-            )
+            _t_valid_coords = (tile_id == int(self.layer)) | (tile_id == -1)
 
             _t_sts_pseudoimage = create_paired_pseudoimage(
                 sts_coords[:, ::-1],  # we need to flip these coordinates
                 self.pseudoimg_size,
                 staining_image_rescaled.shape,
                 _t_valid_coords,
                 recenter=False,
@@ -368,15 +364,14 @@
             min_lim, max_lim = _t_sts_coords_to_transform[_t_valid_coords].min(axis=0).astype(
                 int
             ), _t_sts_coords_to_transform[_t_valid_coords].max(axis=0).astype(int)
             x_min, y_min = min_lim
             x_max, y_max = max_lim
 
             _pseudoimage = _t_sts_pseudoimage["pseudoimage"][x_min:x_max, y_min:y_max]
-            _pseudoimage = ((_pseudoimage / _pseudoimage.max()) * 255).astype(np.uint8)
 
             self.update_text.emit(f"Creating metadata for '{self.layer}'")
             image_pair = {
                 "imageA": staining_image_rescaled[x_min:x_max, y_min:y_max],
                 "imageB": _pseudoimage,
                 "lims": [x_min, x_max, y_min, y_max],
                 "factor_rescale": self.rescale_factor_fine,
@@ -815,32 +810,32 @@
 
         # we show a dialog to get the name for the new layer
         # TOOD: get dialog
         dialog = InputDialog()
         if dialog.exec():
             spatial_key_out = dialog.getInputs()
         else:
-            QMessageBox.warning(self, "Warning", "Please specify a name to save the coordinates into 'obsm'")
+            QMessageBox.warning(self, "Warning", "Please specify a name to save the coordinates into 'obsm'\n(e.g., 'obsm/spatial_manual_coarse')")
             return
     
         # we apply the transformation using the manual_pairwise_aligner code
         in_coords = self.adata[self.renderer.spatial_path][:]
 
         # TODO: we only do for the whole display layer, we need to adapt for the whole thing...
         tile_id = None
         keypoints = keypoints_json_to_dict(self.generate_point_pairs_dict()['points'])
 
         # Apply transform to all coordinates & retransform back
         sts_coords_coarse = in_coords[..., ::-1].copy()
         sts_transformed = apply_transform_to_coords(sts_coords_coarse, tile_id, keypoints, check_bounds=False)
 
-        if f"obsm/{spatial_key_out}" in self.adata:
-            self.adata[f"obsm/{spatial_key_out}"][...] = sts_transformed[:][..., ::-1]
+        if spatial_key_out in self.adata:
+            self.adata[spatial_key_out][...] = sts_transformed[:][..., ::-1]
         else:
-            self.adata[f"obsm/{spatial_key_out}"] = sts_transformed[:][..., ::-1]
+            self.adata[spatial_key_out] = sts_transformed[:][..., ::-1]
 
         # TODO: display some success feedback
         self.adata_structure = h5_to_dict(self.adata)
 
     def _update_imagerender_params(self):
         if self.adata is None or self.renderer is None:
             QMessageBox.warning(
```

### Comparing `openst-0.0.9/openst/alignment/pairwise_aligner.py` & `openst-0.1.0/openst/alignment/pairwise_aligner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,26 @@
-"""
-Automatic Pairwise Alignment of Spatial Transcriptomics and Imaging Data (Open-ST)
-
-Author: Daniel León-Periñán @ N.Rajewsky Lab (BIMSB)
-Date: April 15, 2024
-Version: 0.2.0
-
-Description:
-This script performs automatic pairwise alignment between spatial transcriptomics data and imaging data.
-It aligns the spatial transcriptomics data onto the imaging data to enable spatial comparison and analysis.
-"""
-
 import logging
 from itertools import product
 
 import cv2
 import numpy as np
 import h5py
 from skimage.color import rgb2gray, rgb2hsv
 from skimage.exposure import equalize_adapthist
 from skimage.filters import gaussian
 from skimage.transform import estimate_transform, rescale, rotate
 from threadpoolctl import threadpool_limits
 
-from openst.alignment import feature_matching, fiducial_detection
+from openst.alignment import feature_matching
 from openst.alignment.transformation import apply_transform
 from openst.metadata.classes.pairwise_alignment import (
     AlignmentResult, PairwiseAlignmentMetadata)
 from openst.utils.file import (check_adata_structure, check_directory_exists,
-                               check_file_exists, load_properties_from_adata)
+                               check_file_exists, load_properties_from_adata,
+                               write_key_to_h5)
 from openst.utils.pimage import mask_tissue as p_mask_tissue
 from openst.utils.pimage import is_grayscale
 from openst.utils.pseudoimage import create_paired_pseudoimage
 
 
 def transform_image(im, flip: list = None, crop: list = None, rotation: int = None):
     _dtype = im.dtype
@@ -41,21 +30,48 @@
     if rotation is not None:
         _im = rotate(_im, rotation, clip=True, preserve_range=True, resize=True)
     if crop is not None:
         _im = _im[crop[0] : crop[1], crop[2] : crop[3]]
 
     return _im.astype(_dtype)
 
+def transform_coords(coords, flip: list = None, rotation: int = 0):
+    def rotate_points(points, angle):
+        angle_rad = np.radians(angle)
+        rotation_matrix = np.array([[np.cos(angle_rad), -np.sin(angle_rad)],
+                                    [np.sin(angle_rad), np.cos(angle_rad)]])
+
+        center = np.mean(points, axis=0)
+
+        translated_points = points - center
+        rotated_points = np.dot(translated_points, rotation_matrix.T)
+        rotated_points += center
+
+        return rotated_points
+
+    _x_flip, _y_flip = coords[:, 0], coords[:, 1]
+
+    if flip[0] == -1:
+        _x_flip = (coords[:, 0]*-1) - ((coords[:, 0]*-1).min() - (coords[:, 0]).min())
+    if flip[1] == -1:
+        _y_flip = (coords[:, 1]*-1) - ((coords[:, 1]*-1).min() - (coords[:, 1]).min())
+    
+    transformed_coords = np.array([_x_flip, _y_flip]).T
+
+    if rotation != 0:
+        transformed_coords = rotate_points(transformed_coords, rotation)
+
+    return transformed_coords
 
 def prepare_image_for_feature_matching(
     image: np.ndarray,
     gaussian_blur: float = 0,
     flip: list = [1, 1],
     rotation: float = 0,
-    crop: list = [9, None, 0, None],
+    crop: list = [0, None, 0, None],
     mask_tissue: bool = False,
     keep_black_background: bool = False,
     mask_gaussian_blur: float = 5,
 ):
     """
     Prepare an image for feature matching by applying a series of image processing steps.
 
@@ -116,15 +132,15 @@
 
 
 def prepare_image_for_feature_matching_grayscale(
     image: np.ndarray,
     gaussian_blur: float = 0,
     flip: list = [1, 1],
     rotation: float = 0,
-    crop: list = [9, None, 0, None],
+    crop: list = [0, None, 0, None],
     mask_tissue: bool = False,
     keep_black_background: bool = False,
     mask_gaussian_blur: float = 5,
 ):
     """
     Prepare an image for feature matching by applying a series of image processing steps.
 
@@ -197,25 +213,25 @@
         - The 'flip' parameter specifies flipping along the x and y axes using a list of factors [x_flip, y_flip].
     """
     # Check if flip argument is a list with two elements
     if not isinstance(flip, list) or len(flip) != 2:
         raise ValueError("The 'flip' argument should be a list with two elements [x_flip, y_flip].")
 
     _image = image.copy() if not invert else ((-image) - ((-image).min()))
-    _image = transform_image(_image, flip, crop=None, rotation=rotation)
+    _image = transform_image(_image, flip, crop=[0, None, 0, None], rotation=rotation)
     return [gaussian(equalize_adapthist(_image), gaussian_blur)[:: flip[0], :: flip[1]]]
 
 
 def run_registration(
     in_coords: np.ndarray,
     total_counts: np.ndarray,
     tile_id: np.ndarray,
     staining_image: np.ndarray,
     args,
-) -> (np.ndarray, np.ndarray, np.ndarray, PairwiseAlignmentMetadata): 
+) -> (np.ndarray, np.ndarray, PairwiseAlignmentMetadata): 
     """
     Perform registration of spatial transcriptomics (STS) data with a staining image.
 
     Args:
         in_coords (np.ndarray): Input STS coordinates.
         total_counts (np.ndarray): Total UMI counts for each STS coordinate.
         tile_id: Identifier for each STS coordinate. During the fine registration,
@@ -224,62 +240,60 @@
         staining_image (np.ndarray): Staining image for registration.
         args: Namespace containing various registration parameters.
 
     Returns:
         tuple: A tuple containing four elements:
             - out_coords_output_coarse (np.ndarray): Registered STS coordinates after coarse registration
             - out_coords_output_fine (np.ndarray): Registered STS coordinates after fine registration
-            - registered_staining_image (np.ndarray): Staining image after registration.
             - metadata (PairwiseAlignmentMetadata)
     """
     # Create output objects
     out_coords_output_fine = np.zeros_like(in_coords)
     metadata = PairwiseAlignmentMetadata(args)
 
     logging.info(f"Coarse registration, {len(in_coords)} coordinates")
 
     # Preparing images and preprocessing routines
     
     logging.info(f"Rescaling input image for coarse registration")
-    # rescaling image
     factors = np.array([args.rescale_factor_coarse, args.rescale_factor_coarse])
     _ker = np.maximum(0, (factors - 1) / 2).astype(int)
     src = cv2.resize(cv2.blur(staining_image, _ker),
                      (np.array(staining_image.shape)[[0, 1]]/args.rescale_factor_coarse).astype(int)[::-1],
                      interpolation=cv2.INTER_NEAREST)
-    # staining_image_rescaled = rescale(
-    #     staining_image, 1 / args.rescale_factor_coarse, preserve_range=True, anti_aliasing=True, channel_axis=-1
-    # ).astype(np.uint8)
-    # src = staining_image_rescaled
 
     _fn_prepare_image_for_feature_matching = prepare_image_for_feature_matching
 
     if is_grayscale(src):
         _fn_prepare_image_for_feature_matching = prepare_image_for_feature_matching_grayscale
 
-    def src_augmenter(x, flip, rotation):
-        return _fn_prepare_image_for_feature_matching(
-            image=x,
+    src_augmented = _fn_prepare_image_for_feature_matching(
+        image=src,
+        mask_tissue=args.mask_tissue,
+        keep_black_background=args.keep_black_background,
+        mask_gaussian_blur=args.mask_gaussian_sigma,
+    )
+    
+    def dst_augmenter(x, flip, rotation):
+        return prepare_pseudoimage_for_feature_matching(
+            x,
             flip=flip,
-            rotation=rotation,
-            mask_tissue=args.mask_tissue,
-            keep_black_background=args.keep_black_background,
-            mask_gaussian_blur=args.tissue_masking_gaussian_sigma,
+            rotation=rotation
         )
 
     sts_coords = in_coords[total_counts > args.threshold_counts_coarse]
     sts_pseudoimage = create_paired_pseudoimage(sts_coords, args.pseudoimage_size_coarse, src.shape, resize_method='cv2')
-    dst = prepare_pseudoimage_for_feature_matching(sts_pseudoimage["pseudoimage"])
+    dst = sts_pseudoimage["pseudoimage"]
 
     # Feature matching
     in_mkpts0, in_mkpts1, _best_flip, _best_rotation = feature_matching.match_images(
-        src,
+        src_augmented,
         dst,
         feature_matcher=args.feature_matcher,
-        src_augmenter=src_augmenter,
+        dst_augmenter=dst_augmenter,
         ransac_min_samples=args.ransac_coarse_min_samples,
         ransac_residual_threshold=args.ransac_coarse_residual_threshold,
         ransac_max_trials=args.ransac_coarse_max_trials,
         device=args.device,
     )
 
     # Estimate and apply transform
@@ -305,49 +319,57 @@
     ) * sts_pseudoimage["rescaling_factor"]
 
     sts_coords_coarse = apply_transform(sts_coords_coarse, tform_points, check_bounds=False)
     sts_coords_coarse = sts_coords_coarse * args.rescale_factor_coarse
     sts_coords_coarse = sts_coords_coarse[:, [0, 1]]
     out_coords_output_coarse = sts_coords_coarse.copy()
 
+    logging.info(f"Coarse registration finished, best configuration: flip={_best_flip}, rotation={_best_rotation}")
+
     # Saving alignment results here
     # TODO: check order of keypoints (in all functions throughout package)
     _align_result = AlignmentResult(
         name="coarse_alignment_whole_section",
-        im_0=transform_image(src, _best_flip, [0, None, 0, None], _best_rotation),
-        im_1=sts_pseudoimage["pseudoimage"],
-        transformation_matrix=tform_points.params,
+        im_0=src,
+        im_1=transform_image(sts_pseudoimage["pseudoimage"], [1, 1], [0, None, 0, None], _best_rotation),
+        transformation_matrix=tform_points.params.tolist(),
         ransac_results=None,
         sift_results=None,
         keypoints0=in_mkpts1,
         keypoints1=in_mkpts0,
     )
     metadata.add_alignment_result(_align_result)
 
+    # Compute similarity matrix and compute point transformation
+    if len(in_mkpts0) < args.min_matches:
+        logging.warning(f"There were not enough matching points ({len(in_mkpts0)}"+
+                        f"out of selected {args.min_matches}). "+
+                        "Will not continue with fine registration" if not args.only_coarse else "")
+        args.only_coarse = True
+
     # Finish here if only coarse registration was selected to run
     if args.only_coarse:
         return (
             out_coords_output_coarse,
             None,
-            transform_image(staining_image, _best_flip, None, _best_rotation).astype(np.uint8),
             metadata,
         )
 
     # STAGE 2: fine registration per tile
     logging.info(f"Fine registration with {_best_flip} flip and {_best_rotation} rotation")
 
     # Collect tile identifiers
     tile_codes = np.unique(tile_id.codes)
 
     # Apply scaling to input image again, for fine registration
     staining_image_rescaled = rescale(
         staining_image, 1 / args.rescale_factor_fine, preserve_range=True, anti_aliasing=True, channel_axis=-1
     ).astype(np.uint8)
     src = staining_image_rescaled.astype(np.uint8)
-    src = transform_image(staining_image_rescaled, _best_flip, None, _best_rotation)
+
 
     for tile_code in tile_codes:
         # Create a pseudoimage
         _t_tile_id = np.isin(tile_id.codes, tile_code)
         _t_valid_coords = np.isin(
             tile_id[(total_counts > args.threshold_counts_coarse)].codes[_i_sts_coords_coarse_within_image_bounds],
             tile_code,
@@ -390,165 +412,125 @@
 
         _fn_prepare_image_for_feature_matching = prepare_image_for_feature_matching
 
         if is_grayscale(src):
             _fn_prepare_image_for_feature_matching = prepare_image_for_feature_matching_grayscale
 
         # Preparing image and pseudoimage modalities for feature detection (imaging modality has optimal flip)
-        def src_preprocessor(x, flip, rotation):
-            return _fn_prepare_image_for_feature_matching(
-                image=x,
-                gaussian_blur=args.fine_registration_gaussian_sigma,
-                crop=[x_min, x_max, y_min, y_max],
-                mask_tissue=args.mask_tissue,
-                keep_black_background=args.keep_black_background,
-                mask_gaussian_blur=args.tissue_masking_gaussian_sigma,
-            )
+        src_augmented  = _fn_prepare_image_for_feature_matching(
+            image=src,
+            gaussian_blur=args.gaussian_sigma_fine,
+            crop=[x_min, x_max, y_min, y_max],
+            mask_tissue=args.mask_tissue,
+            keep_black_background=args.keep_black_background,
+            mask_gaussian_blur=args.mask_gaussian_sigma,
+        )
 
         dst = []
         for pseudoimage, invert in product(
             [_t_sts_pseudoimage["pseudoimage"], _t_sts_pseudoimage_counts["pseudoimage"].astype(int)], [False, True]
         ):
             dst += prepare_pseudoimage_for_feature_matching(
                 pseudoimage[x_min:x_max, y_min:y_max],
-                gaussian_blur=args.fine_registration_gaussian_sigma,
+                gaussian_blur=args.gaussian_sigma_fine,
                 invert=invert,
             )
 
         # Finding matches between modalities
         _t_mkpts0, _t_mkpts1, _, _ = feature_matching.match_images(
-            src,
+            src_augmented,
             dst,
-            flips=[_best_flip],
-            rotations=[_best_rotation],
-            src_augmenter=src_preprocessor,
+            flips=[[1, 1]],
+            rotations=[0],
             ransac_min_samples=args.ransac_fine_min_samples,
             ransac_residual_threshold=args.ransac_fine_residual_threshold,
             ransac_max_trials=args.ransac_fine_max_trials,
             device=args.device,
         )
 
-        # Detect fiducial markers with the YOLO model
-        if args.fiducial_model != "" and check_file_exists(args.fiducial_model, exception=False):
-            raise NotImplementedError("Fiducial marker refinement is not implemented yet")
-            logging.info("Running fiducial marker refinement")
-            fiducial_points_src = fiducial_detection.find_fiducial(
-                transform_image(src, _best_flip, [x_min, x_max, y_min, y_max], _best_rotation), args.fiducial_model
-            )
-            fiducial_points_dst = fiducial_detection.find_fiducial(dst, args.fiducial_model)
-
-            _t_mkpts0_fiducial, _t_mkpts1_fiducial = fiducial_detection.correspondences_fiducials(
-                fiducial_points_src, fiducial_points_dst, distance_threshold=50
-            )
-
-            logging.info(f"{len(_t_mkpts0_fiducial)} fiducial matches")
-            _t_mkpts0 = np.concatenate([_t_mkpts0_fiducial, _t_mkpts0], axis=1)
-            _t_mkpts1 = np.concatenate([_t_mkpts1_fiducial, _t_mkpts1], axis=1)
-
         # Apply the same transformation to the tiles
         _t_sts_coords_fine_to_transform = sts_coords_coarse[_t_tile_id] / args.rescale_factor_fine
         _t_sts_coords_fine_to_transform = (_t_sts_coords_fine_to_transform - np.array([[y_min, x_min]]))[:, ::-1]
 
         # Compute similarity matrix and compute point transformation
-        if len(_t_mkpts0) > args.fine_min_matches:
+        if len(_t_mkpts0) > args.min_matches:
             _t_tform_points = estimate_transform("similarity", _t_mkpts0, _t_mkpts1)
 
             _t_sts_coords_fine_transformed = apply_transform(
                 _t_sts_coords_fine_to_transform, _t_tform_points, check_bounds=True
             )[:, :-1]
 
-            _tform_params = _t_tform_points.params
+            _tform_params = _t_tform_points.params.tolist()
         else:
-            logging.warning(f"There were not enough matching points ({len(_t_mkpts0)} out of selected {args.fine_min_matches})")
+            logging.warning(f"There were not enough matching points ({len(_t_mkpts0)} out of selected {args.min_matches})")
             _t_sts_coords_fine_transformed = _t_sts_coords_fine_to_transform[:, ::-1]
             _tform_params = None
             
 
         # Rescale points to original HE dimensions
         _t_sts_coords_fine_transformed = _t_sts_coords_fine_transformed + np.array([[y_min, x_min]])
         _t_sts_coords_fine_transformed = _t_sts_coords_fine_transformed * args.rescale_factor_fine
 
-        out_coords_output_fine[_t_tile_id] = _t_sts_coords_fine_transformed[:, ::-1]
+        out_coords_output_fine[_t_tile_id] = _t_sts_coords_fine_transformed
 
         # Saving alignment results here (only when passed)
         # TODO: check order of keypoints (in all functions throughout package)
         _align_result = AlignmentResult(
             name=f"fine_alignment_tile_{tile_code}",
             im_0=src[x_min:x_max, y_min:y_max],
             im_1=_t_sts_pseudoimage["pseudoimage"][x_min:x_max, y_min:y_max],
             transformation_matrix=_tform_params,
             ransac_results=None,
             sift_results=None,
-            keypoints0=_t_mkpts1,
-            keypoints1=_t_mkpts0,
+            keypoints0=_t_mkpts1[:, ::-1],
+            keypoints1=_t_mkpts0[:, ::-1],
         )
         metadata.add_alignment_result(_align_result)
 
     return (
         out_coords_output_coarse,
         out_coords_output_fine,
-        transform_image(staining_image, _best_flip, None, _best_rotation).astype(np.uint8),
         metadata,
     )
 
 
 def run_pairwise_aligner(args):
     # Check input and output data
     check_file_exists(args.h5_in)
     check_adata_structure(args.h5_in)
 
-    if args.fiducial_model != "" and check_file_exists(args.fiducial_model, exception=False):
-        raise NotImplementedError("Fiducial marker refinement is not implemented yet")
-
     if args.metadata != "" and not check_directory_exists(args.metadata):
         raise FileNotFoundError("Parent directory for the metadata does not exist")
 
     # Loading the spatial transcriptomics data
     sts = load_properties_from_adata(args.h5_in, properties=["obsm/spatial", "obs/total_counts", "obs/tile_id"])
 
     # Loading image data
     with h5py.File(args.h5_in, 'r') as adata:
         staining_image = adata[args.image_in][:]
 
     # Running registration
-    sts_aligned_coarse, sts_aligned_fine, staining_image_aligned, metadata = run_registration(
+    sts_aligned_coarse, sts_aligned_fine, metadata = run_registration(
         sts["obsm/spatial"],
         sts["obs/total_counts"],
         sts["obs/tile_id"],
         staining_image,
         args,
     )
 
     # Saving the metadata (for QC)
     if args.metadata != "":
         metadata.render()
         metadata.save_json(args.metadata)
 
     logging.info(f"Updating {args.h5_in} in place")
     with h5py.File(args.h5_in, 'r+') as adata:
-        # TODO: to this with a function, instead
-        # TODO: do not save image because we assume it is already there!
-        if "uns/spatial_pairwise_aligned/staining_image" in adata:
-            del adata["uns/spatial_pairwise_aligned/staining_image"]
-        adata["uns/spatial_pairwise_aligned/staining_image"] = staining_image
-
-        if "uns/spatial_pairwise_aligned/staining_image_transformed" in adata:
-            del adata["uns/spatial_pairwise_aligned/staining_image_transformed"]
-        adata["uns/spatial_pairwise_aligned/staining_image_transformed"] = staining_image_aligned
-
-        if "obsm/spatial_pairwise_aligned_coarse" in adata:
-            adata["obsm/spatial_pairwise_aligned_coarse"][:] = sts_aligned_coarse[..., ::-1]
-        else:
-            adata["obsm/spatial_pairwise_aligned_coarse"] = sts_aligned_coarse[..., ::-1]
-        
+        write_key_to_h5(adata, "obsm/spatial_pairwise_aligned_coarse", sts_aligned_coarse[..., ::-1])
         if sts_aligned_fine is not None:
-            if "obsm/spatial_pairwise_aligned_fine" in adata:
-                adata["obsm/spatial_pairwise_aligned_fine"][:] = sts_aligned_fine
-            else:
-                adata["obsm/spatial_pairwise_aligned_fine"] = sts_aligned_fine
+            write_key_to_h5(adata, "obsm/spatial_pairwise_aligned_fine", sts_aligned_fine[..., ::-1])
 
 
 def _run_pairwise_aligner(args):
     with threadpool_limits(limits=args.num_workers):
         run_pairwise_aligner(args)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `openst-0.0.9/openst/alignment/transcript_assign.py` & `openst-0.1.0/openst/alignment/transcript_assign.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,16 +42,16 @@
     return adata_by_cell
 
 
 def subset_adata_to_mask(mask, adata, spatial_key: str = 'spatial'):
     # Subset adata to the valid coordinates from the mask
     adata = adata[(adata.obsm[spatial_key][:, 0] >= 0) & 
                   (adata.obsm[spatial_key][:, 1] >= 0) &
-                  (adata.obsm[spatial_key][:, 0] <= mask.shape[0]) & 
-                  (adata.obsm[spatial_key][:, 1] <= mask.shape[1])].copy()
+                  (adata.obsm[spatial_key][:, 0] < mask.shape[0]) & 
+                  (adata.obsm[spatial_key][:, 1] < mask.shape[1])].copy()
 
     # Subset the labels to those in the mask
     labels = mask[adata.obsm[spatial_key][:, 0].astype(int), adata.obsm[spatial_key][:, 1].astype(int)]
 
     # Assign label as cell_ID
     adata.obs["cell_ID"] = labels
```

### Comparing `openst-0.0.9/openst/alignment/transformation.py` & `openst-0.1.0/openst/alignment/transformation.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.9/openst/cli.py` & `openst-0.1.0/openst/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -676,25 +676,54 @@
 IMAGE_PREPROCESS_HELP = "Restoration of imaging data with CUT model (as in Open-ST paper)"
 def get_image_preprocess_parser():
     parser = argparse.ArgumentParser(
         description=IMAGE_PREPROCESS_HELP,
         allow_abbrev=False,
         add_help=False,
     )
-    parser.add_argument("--input_img", type=str, required=True, help="path to input image")
-    parser.add_argument("--cut_dir", type=str, required=True, help="path to CUT directory (to save patched images)")
-    parser.add_argument("--tile_size_px", type=int, required=True, help="size of the tile in pixels")
+    parser.add_argument(
+        "--h5-in",
+        type=str,
+        default="",
+        help="""If set, image is loaded from the Open-ST h5 object (key in --image-in),
+             and retored image is saved there (to the key --image-out)""",
+    )
+    parser.add_argument(
+        "--image-in",
+        type=str,
+        default="uns/spatial/staining_image",
+        help="Key or path to the input image",
+    )
+    parser.add_argument(
+        "--image-out",
+        type=str,
+        default="uns/spatial/staining_image_restored",
+        help="Key or path where the restored image will be written into",
+    )
+    parser.add_argument(
+        "--tile-size-px",
+        type=int,
+        default=512,
+        help="The input image is split into squared tiles of side `--tile-size-px`, for inference."+ 
+        "Larger values avoid boundary effects, but require more memory.",
+    )
+    parser.add_argument("--model", type=str, default="HE_CUT_rajewsky", help="CUT model used for image restoration")
     parser.add_argument(
         "--device",
         type=str,
         default="cpu",
         choices=["cpu", "cuda"],
-        help="Device used to run feature matching model. Can be ['cpu', 'cuda']",
+        help="Device used to run CUT restoration model. Can be ['cpu', 'cuda']",
+    )
+    parser.add_argument(
+        "--num-workers",
+        type=int,
+        default=-1,
+        help="Number of CPU workers for parallel processing",
     )
-    parser.add_argument("--checkpoints_dir", type=str, default="./checkpoints", help="models are saved here")
 
     return parser
 
 
 def setup_image_preprocess_parser(parent_parser):
     parser = parent_parser.add_parser(
         "image_preprocess",
@@ -1076,49 +1105,35 @@
     )
     coarse_params.add_argument(
         "--ransac-coarse-max-trials",
         type=int,
         default=2,
         help="Times RANSAC will run (x1000 iterations) during coarse registration",
     )
-    coarse_params.add_argument(
-        "--genes-coarse",
-        nargs="+",
-        type=str,
-        default=None,
-        help="Genes used for plotting the pseudoimage during the coarse alignment phase.",
-    )
 
     fine_params = parser.add_argument_group('Fine registration parameters')
     fine_params.add_argument(
         "--rescale-factor-fine",
         type=int,
         default=10,
         help="Rescaling factor for the input image (1:factor), used during fine pairwise alignment",
     )
     fine_params.add_argument(
-        "--tissue-masking-gaussian-sigma",
-        type=int,
-        default=5,
-        help="The gaussian blur sigma used during the isolation of the tissue on the HE (preprocessing)",
-    )
-    fine_params.add_argument(
-        "--fine-registration-gaussian-sigma",
+        "--gaussian-sigma-fine",
         type=int,
         default=2,
         help="Gaussian blur used on all modalities during fine registration",
     )
     fine_params.add_argument(
         "--threshold-counts-fine",
         type=int,
         default=0,
         help="""Only spatial coordinates with counts larger than this number
         will be kept for pseudoimage rendering during fine alignment""",
     )
-    
     fine_params.add_argument(
         "--pseudoimage-size-fine",
         type=int,
         default=2000,
         help="Size (in pixels) of the pseudoimage during fine alignment.",
     )
     
@@ -1137,53 +1152,46 @@
     fine_params.add_argument(
         "--ransac-fine-max-trials",
         type=int,
         default=1,
         help="Times RANSAC will run (x1000 iterations) during fine registration",
     )
     fine_params.add_argument(
-        "--fine-min-matches",
+        "--min-matches",
         type=int,
         default=50,
         help="Minimum number of matching keypoints between modalities during fine alignment",
     )
-    fine_params.add_argument(
-        "--genes-fine",
-        nargs="+",
-        type=str,
-        default=None,
-        help="Genes used for plotting the pseudoimage during the fine alignment phase.",
-    )
 
     image_preproc = parser.add_argument_group('Image preprocessing parameters')
     image_preproc.add_argument(
         "--mask-tissue",
         action="store_true",
         help="Tissue (imaging modality) is masked from the background for the feature detection",
     )
+    fine_params.add_argument(
+        "--mask-gaussian-sigma",
+        type=int,
+        default=5,
+        help="The gaussian blur sigma used during the isolation of the tissue on the HE (preprocessing)",
+    )
     image_preproc.add_argument(
         "--keep-black-background",
         action="store_true",
         help="Whether to set the background of the imaging modalities to white, after tissue masking",
     )
     
     model_params = parser.add_argument_group('Feature model parameters')
     model_params.add_argument(
         "--feature-matcher",
         type=str,
         default="LoFTR",
         choices=["LoFTR", "SIFT", "KeyNet"],
         help="Feature matching algorithm",
     )
-    model_params.add_argument(
-        "--fiducial-model",
-        type=str,
-        default="",
-        help="Path to a object detection model (YOLO) to detect fiducial markers",
-    )
 
     compu_params = parser.add_argument_group('Computational parameters')
     compu_params.add_argument(
         "--num-workers",
         type=int,
         default=1,
         help="Number of CPU workers for parallel processing",
```

### Comparing `openst-0.0.9/openst/metadata/classes/base.py` & `openst-0.1.0/openst/metadata/classes/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import logging
 import sys
 
 import numpy as np
 
 from openst.utils.file import check_directory_exists
 
-
 class BaseMetadata:
     def __init__(self, args):
         self.metadata_type = None
         self.cmdline = " ".join(sys.argv)
         self.args = args
 
     def render(self):
@@ -41,19 +40,19 @@
             for k, v in output_data.items():
                 output_data[k] = self._get_dict_recursive(v)
         elif isinstance(data, list):
             output_data = []
             for m in data:
                 output_data.append(self._get_dict_recursive(m))
         elif isinstance(data, np.ndarray):
-            logging.warn(
+            logging.debug(
                 """'np.ndarray' objects are not represented into a dictionary.
-                         Hint: for large images, write a BaseMetadata.render method.
-                               You can store compressed images as base64 strings. 
-                               Other large datasets must not be stored as plain text."""
+                        Hint: for large images, write a BaseMetadata.render method.
+                            You can store compressed images as base64 strings. 
+                            Other large datasets must not be stored as plain text."""
             )
             output_data = ""
         return output_data
 
     def copy(self):
         """
         Create a deep copy of the current object.
```

### Comparing `openst-0.0.9/openst/metadata/classes/pairwise_alignment.py` & `openst-0.1.0/openst/metadata/classes/pairwise_alignment.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,19 +38,22 @@
         self.keypoints_rendered = None
 
     def visualize_alignment(self, fig=None, axes=None, show=False):
         import matplotlib.pyplot as plt
         from skimage.transform import warp
 
         # Apply the transformation matrix to the image
-        aligned_im_1 = warp(self.im_1, SimilarityTransform(self.transformation_matrix).inverse)
+        if self.transformation_matrix is not None:
+            aligned_im_1 = warp(self.im_1, SimilarityTransform(np.array(self.transformation_matrix)).inverse)
+        else:
+            aligned_im_1 = self.im_1
 
         # Display images before and after alignment
         if axes is None:
-            fig, axes = plt.subplots(1, 2)
+            fig, axes = plt.subplots(1, 2, figsize=(10, 5))
         axes[0].imshow(self.im_0, cmap="gray")
         axes[0].imshow(self.im_1, cmap="Blues_r", alpha=0.5)
         axes[0].set_axis_off()
         axes[0].set_title("Before alignment")
         axes[1].imshow(self.im_0, cmap="gray")
         axes[1].imshow(aligned_im_1, cmap="Blues_r", alpha=0.5)
         axes[1].set_axis_off()
```

### Comparing `openst-0.0.9/openst/metadata/classes/segmentation.py` & `openst-0.1.0/openst/metadata/classes/segmentation.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.9/openst/metadata/example_json.json` & `openst-0.1.0/openst/metadata/example_json.json`

 * *Files identical despite different names*

### Comparing `openst-0.0.9/openst/metadata/report.py` & `openst-0.1.0/openst/metadata/report.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.9/openst/metadata/templates/pairwise_alignment.html` & `openst-0.1.0/openst/metadata/templates/pairwise_alignment.html`

 * *Files identical despite different names*

### Comparing `openst-0.0.9/openst/preprocessing/CUT/README.md` & `openst-0.1.0/openst/preprocessing/CUT/README.md`

 * *Files identical despite different names*

### Comparing `openst-0.0.9/openst/preprocessing/CUT/models/__init__.py` & `openst-0.1.0/openst/preprocessing/CUT/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,25 +15,26 @@
     -- self.optimizers (optimizer list):    define and initialize optimizers. You can define one optimizer for each network. If two networks are updated at the same time, you can use itertools.chain to group them. See cycle_gan_model.py for an usage.
 
 Now you can use the model class by specifying flag '--model dummy'.
 See our template model class 'template_model.py' for more details.
 """
 
 import importlib
-from models.base_model import BaseModel
+import logging
 
+from openst.preprocessing.CUT.models.base_model import BaseModel
 
 def find_model_using_name(model_name):
     """Import the module "models/[model_name]_model.py".
 
     In the file, the class called DatasetNameModel() will
     be instantiated. It has to be a subclass of BaseModel,
     and it is case-insensitive.
     """
-    model_filename = "models." + model_name + "_model"
+    model_filename = "openst.preprocessing.CUT.models." + model_name + "_model"
     modellib = importlib.import_module(model_filename)
     model = None
     target_model_name = model_name.replace('_', '') + 'model'
     for name, cls in modellib.__dict__.items():
         if name.lower() == target_model_name.lower() \
            and issubclass(cls, BaseModel):
             model = cls
@@ -59,9 +60,9 @@
 
     Example:
         >>> from models import create_model
         >>> model = create_model(opt)
     """
     model = find_model_using_name(opt.model)
     instance = model(opt)
-    print("model [%s] was created" % type(instance).__name__)
+    logging.info("Model architecture `%s` was created" % type(instance).__name__)
     return instance
```

### Comparing `openst-0.0.9/openst/preprocessing/CUT/models/base_model.py` & `openst-0.1.0/openst/preprocessing/CUT/models/base_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import torch
+import logging
 from collections import OrderedDict
 from abc import ABC, abstractmethod
-from . import networks
+
+from openst.preprocessing.CUT.models import networks
 
 
 class BaseModel(ABC):
     """This class is an abstract base class (ABC) for models.
     To create a subclass, you need to implement the following five functions:
         -- <__init__>:                      initialize the class; first call BaseModel.__init__(self, opt).
         -- <set_input>:                     unpack data from dataset and apply preprocessing.
@@ -207,15 +209,15 @@
                 else:
                     load_dir = self.save_dir
 
                 load_path = os.path.join(load_dir, load_filename)
                 net = getattr(self, 'net' + name)
                 if isinstance(net, torch.nn.DataParallel):
                     net = net.module
-                print('loading the model from %s' % load_path)
+                logging.info(f'Loading model weights from {load_path}')
                 # if you are using PyTorch newer than 0.4 (e.g., built from
                 # GitHub source), you can remove str() on self.device
                 state_dict = torch.load(load_path, map_location=str(self.device))
                 if hasattr(state_dict, '_metadata'):
                     del state_dict._metadata
 
                 # patch InstanceNorm checkpoints prior to 0.4
@@ -225,25 +227,26 @@
 
     def print_networks(self, verbose):
         """Print the total number of parameters in the network and (if verbose) network architecture
 
         Parameters:
             verbose (bool) -- if verbose: print the network architecture
         """
-        print('---------- Networks initialized -------------')
+        message = '---------- (Start) Networks initialized -------------\n'
         for name in self.model_names:
             if isinstance(name, str):
                 net = getattr(self, 'net' + name)
                 num_params = 0
                 for param in net.parameters():
                     num_params += param.numel()
                 if verbose:
-                    print(net)
-                print('[Network %s] Total number of parameters : %.3f M' % (name, num_params / 1e6))
-        print('-----------------------------------------------')
+                    message += f"{net}\n"
+                message += '[Network %s] Total number of parameters : %.3f M\n' % (name, num_params / 1e6)
+        message += '---------- (End) Networks initialized -------------'
+        logging.debug(message)
 
     def set_requires_grad(self, nets, requires_grad=False):
         """Set requies_grad=Fasle for all the networks to avoid unnecessary computations
         Parameters:
             nets (network list)   -- a list of networks
             requires_grad (bool)  -- whether the networks require gradients or not
         """
```

### Comparing `openst-0.0.9/openst/preprocessing/CUT/models/cut_model.py` & `openst-0.1.0/openst/preprocessing/CUT/models/cut_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import torch
-from .base_model import BaseModel
-from . import networks
-from .patchnce import PatchNCELoss
-import util.util as util
 
+from openst.preprocessing.CUT.models.base_model import BaseModel
+from openst.preprocessing.CUT.models import networks
+from openst.preprocessing.CUT.models.patchnce import PatchNCELoss
+from openst.preprocessing.CUT.util import util
 
 class CUTModel(BaseModel):
     """ This class implements CUT and FastCUT model, described in the paper
     Contrastive Learning for Unpaired Image-to-Image Translation
     Taesung Park, Alexei A. Efros, Richard Zhang, Jun-Yan Zhu
     ECCV, 2020
 
@@ -94,18 +94,18 @@
     def data_dependent_initialize(self, data):
         """
         The feature network netF is defined in terms of the shape of the intermediate, extracted
         features of the encoder portion of netG. Because of this, the weights of netF are
         initialized at the first feedforward pass with some input images.
         Please also see PatchSampleF.create_mlp(), which is called at the first forward() call.
         """
-        bs_per_gpu = data["A"].size(0) // max(len(self.opt.gpu_ids), 1)
+        bs_per_gpu = self.opt.batch_size
         self.set_input(data)
         self.real_A = self.real_A[:bs_per_gpu]
-        self.real_B = self.real_B[:bs_per_gpu]
+        self.real_B = None
         self.forward()                     # compute fake images: G(A)
         if self.opt.isTrain:
             self.compute_D_loss().backward()                  # calculate gradients for D
             self.compute_G_loss().backward()                   # calculate graidents for G
             if self.opt.lambda_NCE > 0.0:
                 self.optimizer_F = torch.optim.Adam(self.netF.parameters(), lr=self.opt.lr, betas=(self.opt.beta1, self.opt.beta2))
                 self.optimizers.append(self.optimizer_F)
@@ -134,22 +134,19 @@
 
     def set_input(self, input):
         """Unpack input data from the dataloader and perform necessary pre-processing steps.
         Parameters:
             input (dict): include the data itself and its metadata information.
         The option 'direction' can be used to swap domain A and domain B.
         """
-        AtoB = self.opt.direction == 'AtoB'
-        self.real_A = input['A' if AtoB else 'B'].to(self.device)
-        self.real_B = input['B' if AtoB else 'A'].to(self.device)
-        self.image_paths = input['A_paths' if AtoB else 'B_paths']
+        self.real_A = input['A'].to(self.device)
 
     def forward(self):
         """Run forward pass; called by both functions <optimize_parameters> and <test>."""
-        self.real = torch.cat((self.real_A, self.real_B), dim=0) if self.opt.nce_idt and self.opt.isTrain else self.real_A
+        self.real = self.real_A
         if self.opt.flip_equivariance:
             self.flipped_for_equivariance = self.opt.isTrain and (np.random.random() < 0.5)
             if self.flipped_for_equivariance:
                 self.real = torch.flip(self.real, [3])
 
         self.fake = self.netG(self.real)
         self.fake_B = self.fake[:self.real_A.size(0)]
```

### Comparing `openst-0.0.9/openst/preprocessing/CUT/models/networks.py` & `openst-0.1.0/openst/preprocessing/CUT/models/networks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.nn import init
 import functools
 from torch.optim import lr_scheduler
 import numpy as np
-from .stylegan_networks import StyleGAN2Discriminator, StyleGAN2Generator, TileStyleGAN2Discriminator
-
-###############################################################################
-# Helper Functions
-###############################################################################
-
 
 def get_filter(filt_size=3):
     if(filt_size == 1):
         a = np.array([1., ])
     elif(filt_size == 2):
         a = np.array([1., 1.])
     elif(filt_size == 3):
@@ -252,18 +246,14 @@
         net = ResnetGenerator(input_nc, output_nc, ngf, norm_layer=norm_layer, use_dropout=use_dropout, no_antialias=no_antialias, no_antialias_up=no_antialias_up, n_blocks=6, opt=opt)
     elif netG == 'resnet_4blocks':
         net = ResnetGenerator(input_nc, output_nc, ngf, norm_layer=norm_layer, use_dropout=use_dropout, no_antialias=no_antialias, no_antialias_up=no_antialias_up, n_blocks=4, opt=opt)
     elif netG == 'unet_128':
         net = UnetGenerator(input_nc, output_nc, 7, ngf, norm_layer=norm_layer, use_dropout=use_dropout)
     elif netG == 'unet_256':
         net = UnetGenerator(input_nc, output_nc, 8, ngf, norm_layer=norm_layer, use_dropout=use_dropout)
-    elif netG == 'stylegan2':
-        net = StyleGAN2Generator(input_nc, output_nc, ngf, use_dropout=use_dropout, opt=opt)
-    elif netG == 'smallstylegan2':
-        net = StyleGAN2Generator(input_nc, output_nc, ngf, use_dropout=use_dropout, n_blocks=2, opt=opt)
     elif netG == 'resnet_cat':
         n_blocks = 8
         net = G_Resnet(input_nc, output_nc, opt.nz, num_downs=2, n_res=n_blocks - 4, ngf=ngf, norm='inst', nl_layer='relu')
     else:
         raise NotImplementedError('Generator model name [%s] is not recognized' % netG)
     return init_net(net, init_type, init_gain, gpu_ids, initialize_weights=('stylegan2' not in netG))
 
@@ -319,16 +309,14 @@
 
     if netD == 'basic':  # default PatchGAN classifier
         net = NLayerDiscriminator(input_nc, ndf, n_layers=3, norm_layer=norm_layer, no_antialias=no_antialias,)
     elif netD == 'n_layers':  # more options
         net = NLayerDiscriminator(input_nc, ndf, n_layers_D, norm_layer=norm_layer, no_antialias=no_antialias,)
     elif netD == 'pixel':     # classify if each pixel is real or fake
         net = PixelDiscriminator(input_nc, ndf, norm_layer=norm_layer)
-    elif 'stylegan2' in netD:
-        net = StyleGAN2Discriminator(input_nc, ndf, n_layers_D, no_antialias=no_antialias, opt=opt)
     else:
         raise NotImplementedError('Discriminator model name [%s] is not recognized' % netD)
     return init_net(net, init_type, init_gain, gpu_ids,
                     initialize_weights=('stylegan2' not in netD))
 
 
 ##############################################################################
@@ -1210,16 +1198,14 @@
     def forward(self, input):
         """Standard forward"""
         return self.model(input)
 
 
 class UnetSkipConnectionBlock(nn.Module):
     """Defines the Unet submodule with skip connection.
-        X -------------------identity----------------------
-        |-- downsampling -- |submodule| -- upsampling --|
     """
 
     def __init__(self, outer_nc, inner_nc, input_nc=None,
                  submodule=None, outermost=False, innermost=False, norm_layer=nn.BatchNorm2d, use_dropout=False):
         """Construct a Unet submodule with skip connections.
 
         Parameters:
```

### Comparing `openst-0.0.9/openst/preprocessing/CUT/models/template_model.py` & `openst-0.1.0/openst/preprocessing/CUT/models/template_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 The class name should be consistent with both the filename and its model option.
 The filename should be <model>_dataset.py
 The class name should be <Model>Dataset.py
 It implements a simple image-to-image translation baseline based on regression loss.
 Given input-output pairs (data_A, data_B), it learns a network netG that can minimize the following L1 loss:
     min_<netG> ||netG(data_A) - data_B||_1
 You need to implement the following functions:
-    <modify_commandline_options>:　Add model-specific options and rewrite default values for existing options.
+    <modify_commandline_options>: Add model-specific options and rewrite default values for existing options.
     <__init__>: Initialize this model class.
     <set_input>: Unpack input data and perform data pre-processing.
     <forward>: Run forward pass. This will be called by both <optimize_parameters> and <test>.
     <optimize_parameters>: Update network weights; it will be called in every training iteration.
 """
 import torch
-from .base_model import BaseModel
-from . import networks
+
+from openst.preprocessing.CUT.models.base_model import BaseModel
+from openst.preprocessing.CUT.models import networks
 
 
 class TemplateModel(BaseModel):
     @staticmethod
     def modify_commandline_options(parser, is_train=True):
         """Add new model-specific options and rewrite default values for existing options.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `openst-0.0.9/openst/preprocessing/CUT/options/base_options.py` & `openst-0.1.0/openst/preprocessing/CUT/options/base_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import argparse
-import os
-from util import util
+import logging
 import torch
-import models
-import data
 
+import openst.preprocessing.CUT.models as models
+import openst.preprocessing.CUT.util as util
 
 class BaseOptions():
     """This class defines options used during both training and test time.
 
     It also implements several helper functions such as parsing, printing, and saving the options.
     It also gathers additional options defined in <modify_commandline_options> functions in both dataset class and model class.
     """
@@ -30,16 +29,16 @@
         parser.add_argument('--checkpoints_dir', type=str, default='./checkpoints', help='models are saved here')
         # model parameters
         parser.add_argument('--model', type=str, default='cut', help='chooses which model to use.')
         parser.add_argument('--input_nc', type=int, default=3, help='# of input image channels: 3 for RGB and 1 for grayscale')
         parser.add_argument('--output_nc', type=int, default=3, help='# of output image channels: 3 for RGB and 1 for grayscale')
         parser.add_argument('--ngf', type=int, default=64, help='# of gen filters in the last conv layer')
         parser.add_argument('--ndf', type=int, default=64, help='# of discrim filters in the first conv layer')
-        parser.add_argument('--netD', type=str, default='basic', choices=['basic', 'n_layers', 'pixel', 'patch', 'tilestylegan2', 'stylegan2'], help='specify discriminator architecture. The basic model is a 70x70 PatchGAN. n_layers allows you to specify the layers in the discriminator')
-        parser.add_argument('--netG', type=str, default='resnet_9blocks', choices=['resnet_9blocks', 'resnet_6blocks', 'unet_256', 'unet_128', 'stylegan2', 'smallstylegan2', 'resnet_cat'], help='specify generator architecture')
+        parser.add_argument('--netD', type=str, default='basic', choices=['basic', 'n_layers', 'pixel', 'patch'], help='specify discriminator architecture. The basic model is a 70x70 PatchGAN. n_layers allows you to specify the layers in the discriminator')
+        parser.add_argument('--netG', type=str, default='resnet_9blocks', choices=['resnet_9blocks', 'resnet_6blocks', 'unet_256', 'unet_128', 'resnet_cat'], help='specify generator architecture')
         parser.add_argument('--n_layers_D', type=int, default=3, help='only used if netD==n_layers')
         parser.add_argument('--normG', type=str, default='instance', choices=['instance', 'batch', 'none'], help='instance normalization or batch normalization for G')
         parser.add_argument('--normD', type=str, default='instance', choices=['instance', 'batch', 'none'], help='instance normalization or batch normalization for D')
         parser.add_argument('--init_type', type=str, default='xavier', choices=['normal', 'xavier', 'kaiming', 'orthogonal'], help='network initialization')
         parser.add_argument('--init_gain', type=float, default=0.02, help='scaling factor for normal, xavier and orthogonal.')
         parser.add_argument('--no_dropout', type=util.str2bool, nargs='?', const=True, default=True,
                             help='no dropout for the generator')
@@ -60,19 +59,14 @@
         parser.add_argument('--random_scale_max', type=float, default=3.0,
                             help='(used for single image translation) Randomly scale the image by the specified factor as data augmentation.')
         # additional parameters
         parser.add_argument('--epoch', type=str, default='latest', help='which epoch to load? set to latest to use latest cached model')
         parser.add_argument('--verbose', action='store_true', help='if specified, print more debugging information')
         parser.add_argument('--suffix', default='', type=str, help='customized suffix: opt.name = opt.name + suffix: e.g., {model}_{netG}_size{load_size}')
 
-        # parameters related to StyleGAN2-based networks
-        parser.add_argument('--stylegan2_G_num_downsampling',
-                            default=1, type=int,
-                            help='Number of downsampling layers used by StyleGAN2Generator')
-
         self.initialized = True
         return parser
 
     def gather_options(self):
         """Initialize our parser with basic options(only once).
         Add additional model-specific and dataset-specific options.
         These options are defined in the <modify_commandline_options> function
@@ -93,54 +87,36 @@
         model_option_setter = models.get_option_setter(model_name)
         parser = model_option_setter(parser, self.isTrain)
         if self.cmd_line is None:
             opt, _ = parser.parse_known_args()  # parse again with new defaults
         else:
             opt, _ = parser.parse_known_args(self.cmd_line)  # parse again with new defaults
 
-        # modify dataset-related parser options
-        dataset_name = opt.dataset_mode
-        dataset_option_setter = data.get_option_setter(dataset_name)
-        parser = dataset_option_setter(parser, self.isTrain)
-
         # save and return the parser
         self.parser = parser
         if self.cmd_line is None:
             return parser.parse_args()
         else:
             return parser.parse_args(self.cmd_line)
 
     def print_options(self, opt):
         """Print and save options
 
         It will print both current options and default values(if different).
-        It will save options into a text file / [checkpoints_dir] / opt.txt
         """
         message = ''
-        message += '----------------- Options ---------------\n'
+        message += '----------------- (Start) CUT restoration options ---------------\n'
         for k, v in sorted(vars(opt).items()):
             comment = ''
             default = self.parser.get_default(k)
             if v != default:
                 comment = '\t[default: %s]' % str(default)
             message += '{:>25}: {:<30}{}\n'.format(str(k), str(v), comment)
-        message += '----------------- End -------------------'
-        print(message)
-
-        # save to the disk
-        expr_dir = os.path.join(opt.checkpoints_dir, opt.name)
-        util.mkdirs(expr_dir)
-        file_name = os.path.join(expr_dir, '{}_opt.txt'.format(opt.phase))
-        try:
-            with open(file_name, 'wt') as opt_file:
-                opt_file.write(message)
-                opt_file.write('\n')
-        except PermissionError as error:
-            print("permission error {}".format(error))
-            pass
+        message += '----------------- (End) CUT restoration options -------------------'
+        logging.debug(message)
 
     def parse(self):
         """Parse our options, create checkpoints directory suffix, and set up gpu device."""
         opt = self.gather_options()
         opt.isTrain = self.isTrain   # train or test
 
         # process opt.suffix
```

### Comparing `openst-0.0.9/openst/preprocessing/CUT/options/test_options.py` & `openst-0.1.0/openst/preprocessing/CUT/options/test_options.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from .base_options import BaseOptions
-
+from openst.preprocessing.CUT.options.base_options import BaseOptions
 
 class TestOptions(BaseOptions):
     """This class includes test options.
 
     It also includes shared options defined in BaseOptions.
     """
```

### Comparing `openst-0.0.9/openst/preprocessing/CUT/util/util.py` & `openst-0.1.0/openst/preprocessing/CUT/util/util.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.9/openst/preprocessing/barcode_preprocessing.py` & `openst-0.1.0/openst/preprocessing/barcode_preprocessing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import gzip
 import os
 import time
 
 import pandas as pd
 
+import logging
+
 
 tab = str.maketrans("ACTG", "TGAC")
 
 
 def reverse_complement_table(seq):
     return seq.translate(tab)[::-1]
 
@@ -27,15 +29,15 @@
         for line in f:
             if idx % 4 == 0:
                 tile_number, xcoord, ycoord = get_tile_number_and_coordinates(line.strip())
                 if current_tile_number is None:
                     current_tile_number = tile_number
 
                 if tile_number != current_tile_number:
-                    print(f"Writing {len(sequences):,} barcodes of file {current_tile_number} to disk")
+                    logging.info(f"Writing {len(sequences):,} barcodes of file {current_tile_number} to disk")
                     df = pd.DataFrame({"cell_bc": sequences, "xcoord": xcoords, "ycoord": ycoords})
                     df.to_csv(
                         os.path.join(
                             out_path,
                             out_prefix + current_tile_number + out_suffix,
                         ),
                         index=False,
@@ -91,20 +93,21 @@
 
     if not args.single_tile and not args.unsorted:
         process_multiple_tiles(args.fastq_in, args.tilecoords_out, args.out_prefix, args.out_suffix, sequence_preprocessor)
     elif not args.single_tile and args.unsorted:
         raise NotImplementedError("We don't support multi-tile files with unsorted tiles yet!")
     else:
         df = process_single_tile(args.fastq_in, sequence_preprocessor)
-        print(f"Writing {len(df):,} barcodes to {os.path.join(args.tilecoords_out, args.out_prefix + args.out_suffix)}")
+        logging.info(f"Writing {len(df):,} barcodes to {os.path.join(args.tilecoords_out, args.out_prefix + args.out_suffix)}")
         df.to_csv(
             os.path.join(args.tilecoords_out, args.out_prefix + args.out_suffix),
             index=False,
             sep="\t",
         )
 
-    print(f"Finished in {round(time.time()-start_time, 2)} sec")
+    logging.info(f"Finished in {round(time.time()-start_time, 2)} sec")
 
 
 if __name__ == "__main__":
+    from openst.cli import get_barcode_preprocessing_parser
     args = get_barcode_preprocessing_parser().parse_args()
     _run_barcode_preprocessing(args)
```

### Comparing `openst-0.0.9/openst/preprocessing/image_stitch.py` & `openst-0.1.0/openst/preprocessing/image_stitch.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.9/openst/preprocessing/imagej_macros/keyence_stitch.ijm` & `openst-0.1.0/openst/preprocessing/imagej_macros/keyence_stitch.ijm`

 * *Files identical despite different names*

### Comparing `openst-0.0.9/openst/preprocessing/merge_modalities.py` & `openst-0.1.0/openst/preprocessing/merge_modalities.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.9/openst/preprocessing/spatial_stitch.py` & `openst-0.1.0/openst/preprocessing/spatial_stitch.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.9/openst/segmentation/segment.py` & `openst-0.1.0/openst/segmentation/segment.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 # Models pretrained by the Rajewsky lab
 OPENST_MODEL_NAMES = [
     "HE_cellpose_rajewsky"
 ]
 
 # adapted from cellpose
-MODEL_DIR = pathlib.Path.home().joinpath(".cellpose", "models")
+MODEL_DIR = pathlib.Path.home().joinpath(".openst", "cellpose", "models")
 _MODEL_URL = "http://bimsbstatic.mdc-berlin.de/rajewsky/openst-public-data/models"
 
 def cache_model_path(basename):
     MODEL_DIR.mkdir(parents=True, exist_ok=True)
     url = f"{_MODEL_URL}/{basename}"
     cached_file = os.fspath(MODEL_DIR.joinpath(basename))
     if not os.path.exists(cached_file):
```

### Comparing `openst-0.0.9/openst/segmentation/segment_merge.py` & `openst-0.1.0/openst/segmentation/segment_merge.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.9/openst/threed/from_3d_registration.py` & `openst-0.1.0/openst/threed/from_3d_registration.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.9/openst/threed/to_3d_registration.py` & `openst-0.1.0/openst/threed/to_3d_registration.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.9/openst/utils/file.py` & `openst-0.1.0/openst/utils/file.py`

 * *Files 16% similar despite different names*

```diff
@@ -242,8 +242,61 @@
     for key, value in adata.items():
         if isinstance(value, h5py.Group):
             result[key] = h5_to_dict(value)
         else:
             dataset_type = str(type(value))
             dataset_shape = value.shape if hasattr(value, 'shape') else None
             result[key] = f"{dataset_type}_{dataset_shape}"
-    return result
+    return result
+
+def write_key_to_h5(adata, key, data, delete_before=False):
+    if key in adata and not delete_before:
+        adata[key][:] = data
+    elif key in adata and delete_before:
+        del adata[key]
+    else:
+        adata[key] = data
+
+def download_url_to_file(url, dst, progress=True):
+    r"""Download object at the given URL to a local path.
+            Thanks to torch & cellpose
+    Args:
+        url (string): URL of the object to download
+        dst (string): Full path where object will be saved, e.g. `/tmp/temporary_file`
+        progress (bool, optional): whether or not to display a progress bar to stderr
+            Default: True
+    """
+
+    from urllib.request import urlopen
+    import tempfile
+    from tqdm import tqdm
+
+    file_size = None
+    import ssl
+    ssl._create_default_https_context = ssl._create_unverified_context
+    u = urlopen(url)
+    meta = u.info()
+    if hasattr(meta, "getheaders"):
+        content_length = meta.getheaders("Content-Length")
+    else:
+        content_length = meta.get_all("Content-Length")
+    if content_length is not None and len(content_length) > 0:
+        file_size = int(content_length[0])
+    # We deliberately save it in a temp file and move it after
+    dst = os.path.expanduser(dst)
+    dst_dir = os.path.dirname(dst)
+    f = tempfile.NamedTemporaryFile(delete=False, dir=dst_dir)
+    try:
+        with tqdm(total=file_size, disable=not progress, unit="B", unit_scale=True,
+                  unit_divisor=1024) as pbar:
+            while True:
+                buffer = u.read(8192)
+                if len(buffer) == 0:
+                    break
+                f.write(buffer)
+                pbar.update(len(buffer))
+        f.close()
+        shutil.move(f.name, dst)
+    finally:
+        f.close()
+        if os.path.exists(f.name):
+            os.remove(f.name)
```

### Comparing `openst-0.0.9/openst/utils/from_spacemake.py` & `openst-0.1.0/openst/utils/from_spacemake.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.9/openst/utils/pimage.py` & `openst-0.1.0/openst/utils/pimage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import dask
 import numpy as np
+import logging
 
 from dask_image.ndmorph import binary_dilation as dask_binary_dilation
 from dask_image.ndfilters import gaussian as dask_gaussian
 from scipy.ndimage import binary_dilation as scipy_binary_dilation
 from skimage.filters import threshold_otsu
 from skimage.filters import gaussian as skimage_gaussian
 from skimage.color import rgb2hsv as skimage_rgb2hsv
@@ -80,15 +81,15 @@
 
     Notes:
         Adapted from skimage; the bin calculation is different, but suffices for this purpose
         Please only use with dask!
 
     """
     if image is not None and image.ndim > 2 and image.shape[-1] in (3, 4):
-        print(f'threshold_otsu is expected to work correctly only for '
+        logging.warn(f'threshold_otsu is expected to work correctly only for '
              f'grayscale images; image shape {image.shape} looks like '
              f'that of an RGB image.')
 
     # Check if the image has more than one intensity value; if not, return that
     # value
     if image is not None:
         first_pixel = image.ravel()[0]
@@ -169,15 +170,15 @@
 
     out.compute_chunk_sizes()
     arr.compute_chunk_sizes()
     delta.compute_chunk_sizes()
 
     if type(rgb) is dask.array.Array:
         out_h = np.zeros_like(out_s)
-        print("Hue channel not implemented when using dask array")
+        logging.warn("Hue channel not implemented when using dask array")
     else:
         # -- H channel
         # red is max
         idx = (arr[..., 0] == out_v)
         out[idx, 0] = (arr[idx, 1] - arr[idx, 2]) / delta[idx]
 
         # green is max
```

### Comparing `openst-0.0.9/openst/utils/points.py` & `openst-0.1.0/openst/utils/points.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.9/openst/utils/preview.py` & `openst-0.1.0/openst/utils/preview.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.9/openst/utils/pseudoimage.py` & `openst-0.1.0/openst/utils/pseudoimage.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
     if values is None:
         values = 1
     
     # new version to generate the pseudoimage
     # np.add.at(_sts_pseudoimage, (coords_rescaled_int[:, 0], coords_rescaled_int[:, 1]), values)
     _sts_pseudoimage, _, _ = np.histogram2d(coords_rescaled_int[:, 0], coords_rescaled_int[:, 1],
-                                   bins=(dim_1 + 1, dim_2 + 1),
+                                   bins=(dim_1, dim_2),
                                    range=[[0, dim_1], [0, dim_2]])
     #_sts_pseudoimage[coords_rescaled_int[:, 0], coords_rescaled_int[:, 1]] += values
 
     if resize_method == 'scikit-image':
         sts_pseudoimage = resize(_sts_pseudoimage, target_size[:2], anti_aliasing=True)
     elif resize_method == 'cv2':
         _ker = 2
```

### Comparing `openst-0.0.9/openst/utils/scanpy/pp/_qc.py` & `openst-0.1.0/openst/utils/scanpy/pp/_qc.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.9/openst/utils/spacemake.py` & `openst-0.1.0/openst/utils/spacemake.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.9/pyproject.toml` & `openst-0.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "openst"
-version = "0.0.9"
+version = "0.1.0"
 description = "The computational pipeline for the Open-ST method."
 license = "GPL-2.0"
 authors = [
     "Daniel León-Periñán <daniel.leonperinan@mdc-berlin.de>",
     "Nikolaos Karaiskos <nikolaos.karaiskos@mdc-berlin.de>",
 ]
 maintainers = [
@@ -32,15 +32,15 @@
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Topic :: Scientific/Engineering :: Visualization",
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">3.8,<3.12"
 anndata = ">=0.7.4"
 numpy = ">=1.17.0"
 matplotlib = ">=3.4"
 pandas = ">=1.0"
 scipy = ">=1.4"
 h5py = ">=3"
 tqdm = "*"
```

### Comparing `openst-0.0.9/PKG-INFO` & `openst-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: openst
-Version: 0.0.9
+Version: 0.1.0
 Summary: The computational pipeline for the Open-ST method.
 License: GPL-2.0
 Author: Daniel León-Periñán
 Author-email: daniel.leonperinan@mdc-berlin.de
 Maintainer: Daniel León-Periñán
 Maintainer-email: daniel.leonperinan@mdc-berlin.de
-Requires-Python: >=3.8,<4.0
+Requires-Python: >3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Dist: anndata (>=0.7.4)
 Requires-Dist: cellpose (>=2.2.3)
 Requires-Dist: dask-image
 Requires-Dist: dask[array]
 Requires-Dist: h5py (>=3)
@@ -49,19 +48,19 @@
 Project-URL: Documentation, https://rajewsky-lab.github.io/openst/
 Project-URL: Home-page, https://rajewsky-lab.github.io/openst
 Project-URL: Source, https://github.com/rajewsky-lab/openst
 Project-URL: Twitter, https://twitter.com/open_sts
 Description-Content-Type: text/markdown
 
 [![docs](https://github.com/rajewsky-lab/openst/actions/workflows/docs.yml/badge.svg)](https://github.com/rajewsky-lab/openst/actions/workflows/docs.yml)
+[![Publish Docker image](https://github.com/rajewsky-lab/openst/actions/workflows/docker_hub.yml/badge.svg)](https://github.com/rajewsky-lab/openst/actions/workflows/docker_hub.yml)
 [![Downloads](https://pepy.tech/badge/openst)](https://pepy.tech/project/openst)
 [![PyPI Version](https://img.shields.io/pypi/v/openst.svg)](https://pypi.org/project/openst)
 [![PyPI License](https://img.shields.io/pypi/l/openst.svg)](https://pypi.org/project/openst)
 [![Gitter chat](https://badges.gitter.im/openst/community.png)](https://gitter.im/openst/community)
-[![ci](https://github.com/rajewsky-lab/openst/actions/workflows/docs.yml/badge.svg)](https://github.com/rajewsky-lab/openst/actions/workflows/docs.yml)
 
 <img
   src="https://raw.githubusercontent.com/rajewsky-lab/openst/5617df9d35341778487d4c623eaac53b61000006/docs/static/img/openst_logo_color.png"
   class="dark-light" align="right" width="350" alt="image"
 />
 
 # Open-ST: open-source spatial transcriptomics
```


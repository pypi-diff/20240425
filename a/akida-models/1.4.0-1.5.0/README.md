# Comparing `tmp/akida_models-1.4.0.tar.gz` & `tmp/akida_models-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akida_models-1.4.0.tar", last modified: Wed Feb 21 15:45:46 2024, max compression
+gzip compressed data, was "akida_models-1.5.0.tar", last modified: Thu Apr 25 12:31:04 2024, max compression
```

## Comparing `akida_models-1.4.0.tar` & `akida_models-1.5.0.tar`

### file list

```diff
@@ -1,105 +1,113 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 15:45:46.728488 akida_models-1.4.0/
--rw-r--r--   0 root         (0) root         (0)    11358 2024-02-21 15:45:43.000000 akida_models-1.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2635 2024-02-21 15:45:43.000000 akida_models-1.4.0/LICENSE.3rdparty
--rw-r--r--   0 root         (0) root         (0)       41 2024-02-21 15:45:43.000000 akida_models-1.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      640 2024-02-21 15:45:46.728488 akida_models-1.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      147 2024-02-21 15:45:43.000000 akida_models-1.4.0/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 15:45:46.720488 akida_models-1.4.0/akida_models/
--rw-r--r--   0 root         (0) root         (0)     1571 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 15:45:46.720488 akida_models-1.4.0/akida_models/casia_webface/
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/casia_webface/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5129 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/casia_webface/preprocessing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 15:45:46.720488 akida_models-1.4.0/akida_models/centernet/
--rw-r--r--   0 root         (0) root         (0)       97 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/centernet/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6804 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/centernet/centernet_loss.py
--rw-r--r--   0 root         (0) root         (0)     3868 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/centernet/centernet_processing.py
--rw-r--r--   0 root         (0) root         (0)     9324 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/centernet/centernet_train.py
--rw-r--r--   0 root         (0) root         (0)    12373 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/centernet/centernet_utils.py
--rw-r--r--   0 root         (0) root         (0)     5823 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/centernet/model_centernet.py
--rw-r--r--   0 root         (0) root         (0)    18526 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/cli.py
--rw-r--r--   0 root         (0) root         (0)     6994 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/cyclic_lr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 15:45:46.724488 akida_models-1.4.0/akida_models/detection/
--rw-r--r--   0 root         (0) root         (0)      164 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/detection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6706 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/detection/box_utils.py
--rw-r--r--   0 root         (0) root         (0)     9022 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/detection/data_augmentation.py
--rw-r--r--   0 root         (0) root         (0)     2021 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/detection/data_utils.py
--rw-r--r--   0 root         (0) root         (0)     4700 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/detection/generate_anchors.py
--rw-r--r--   0 root         (0) root         (0)    11946 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/detection/map_evaluation.py
--rw-r--r--   0 root         (0) root         (0)     7622 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/detection/model_yolo.py
--rw-r--r--   0 root         (0) root         (0)     6047 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/detection/preprocess_data.py
--rw-r--r--   0 root         (0) root         (0)    10746 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/detection/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 15:45:46.724488 akida_models-1.4.0/akida_models/detection/voc/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/detection/voc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5650 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/detection/voc/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 15:45:46.724488 akida_models-1.4.0/akida_models/detection/widerface/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/detection/widerface/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3509 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/detection/widerface/data.py
--rw-r--r--   0 root         (0) root         (0)     6762 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/detection/yolo_loss.py
--rw-r--r--   0 root         (0) root         (0)    13824 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/detection/yolo_train.py
--rw-r--r--   0 root         (0) root         (0)    11195 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/distiller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 15:45:46.724488 akida_models-1.4.0/akida_models/dvs/
--rw-r--r--   0 root         (0) root         (0)      132 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/dvs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18531 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/dvs/dvs_generator.py
--rw-r--r--   0 root         (0) root         (0)     6470 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/dvs/dvs_train.py
--rw-r--r--   0 root         (0) root         (0)     6327 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/dvs/model_convtiny_gesture.py
--rw-r--r--   0 root         (0) root         (0)     6743 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/dvs/model_convtiny_handy.py
--rw-r--r--   0 root         (0) root         (0)    14518 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/dvs/preprocessing.py
--rw-r--r--   0 root         (0) root         (0)     1838 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/extract.py
--rw-r--r--   0 root         (0) root         (0)     3040 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/gamma_constraint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 15:45:46.724488 akida_models-1.4.0/akida_models/imagenet/
--rw-r--r--   0 root         (0) root         (0)      215 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/imagenet/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33671 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/imagenet/imagenet_labels2names.py
--rw-r--r--   0 root         (0) root         (0)    24770 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/imagenet/imagenet_train.py
--rw-r--r--   0 root         (0) root         (0)     3119 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/imagenet/imagenet_utils.py
--rw-r--r--   0 root         (0) root         (0)     4057 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/imagenet/load_samples.py
--rw-r--r--   0 root         (0) root         (0)    19259 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/imagenet/model_akidanet.py
--rw-r--r--   0 root         (0) root         (0)     8468 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/imagenet/model_akidanet18.py
--rw-r--r--   0 root         (0) root         (0)     7648 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/imagenet/model_akidanet_edge.py
--rw-r--r--   0 root         (0) root         (0)    16418 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/imagenet/model_mobilenet.py
--rw-r--r--   0 root         (0) root         (0)     6140 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/imagenet/preprocessing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 15:45:46.728488 akida_models-1.4.0/akida_models/kws/
--rw-r--r--   0 root         (0) root         (0)       57 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/kws/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5101 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/kws/kws_train.py
--rw-r--r--   0 root         (0) root         (0)     6934 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/kws/model_ds_cnn.py
--rw-r--r--   0 root         (0) root         (0)    29734 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/kws/preprocessing.py
--rw-r--r--   0 root         (0) root         (0)    32119 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/layer_blocks.py
--rw-r--r--   0 root         (0) root         (0)     2425 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/macs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 15:45:46.728488 akida_models-1.4.0/akida_models/mnist/
--rw-r--r--   0 root         (0) root         (0)       27 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/mnist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3621 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/mnist/mnist_train.py
--rw-r--r--   0 root         (0) root         (0)     4207 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/mnist/model_gxnor.py
--rw-r--r--   0 root         (0) root         (0)     4775 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/model_io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 15:45:46.728488 akida_models-1.4.0/akida_models/modelnet40/
--rw-r--r--   0 root         (0) root         (0)       94 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/modelnet40/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8939 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/modelnet40/model_pointnet_plus.py
--rw-r--r--   0 root         (0) root         (0)     5251 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/modelnet40/modelnet40_train.py
--rw-r--r--   0 root         (0) root         (0)     6513 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/modelnet40/pointnet_utils.py
--rw-r--r--   0 root         (0) root         (0)     8320 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/modelnet40/preprocessing.py
--rw-r--r--   0 root         (0) root         (0)    10740 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/optimizers.py
--rw-r--r--   0 root         (0) root         (0)     8177 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/param_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 15:45:46.728488 akida_models-1.4.0/akida_models/portrait128/
--rw-r--r--   0 root         (0) root         (0)       32 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/portrait128/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7126 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/portrait128/model_akida_unet.py
--rw-r--r--   0 root         (0) root         (0)     9028 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/portrait128/portrait128_train.py
--rw-r--r--   0 root         (0) root         (0)    13688 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/training.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 15:45:46.728488 akida_models-1.4.0/akida_models/transformers/
--rw-r--r--   0 root         (0) root         (0)       51 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/transformers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12770 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/transformers/model_deit.py
--rw-r--r--   0 root         (0) root         (0)    17044 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/transformers/model_vit.py
--rw-r--r--   0 root         (0) root         (0)    12195 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/unfuse_sepconv_layers.py
--rw-r--r--   0 root         (0) root         (0)     8084 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 15:45:46.728488 akida_models-1.4.0/akida_models/utk_face/
--rw-r--r--   0 root         (0) root         (0)       54 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/utk_face/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5636 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/utk_face/model_vgg.py
--rw-r--r--   0 root         (0) root         (0)     2404 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/utk_face/preprocessing.py
--rw-r--r--   0 root         (0) root         (0)     3795 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/utk_face/utk_face_train.py
--rw-r--r--   0 root         (0) root         (0)      104 2024-02-21 15:45:43.000000 akida_models-1.4.0/akida_models/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 15:45:46.728488 akida_models-1.4.0/akida_models.egg-info/
--rw-r--r--   0 root         (0) root         (0)      640 2024-02-21 15:45:46.000000 akida_models-1.4.0/akida_models.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3029 2024-02-21 15:45:46.000000 akida_models-1.4.0/akida_models.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-21 15:45:46.000000 akida_models-1.4.0/akida_models.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      558 2024-02-21 15:45:46.000000 akida_models-1.4.0/akida_models.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       74 2024-02-21 15:45:46.000000 akida_models-1.4.0/akida_models.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-02-21 15:45:46.000000 akida_models-1.4.0/akida_models.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-21 15:45:46.728488 akida_models-1.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1577 2024-02-21 15:45:42.000000 akida_models-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:31:04.004337 akida_models-1.5.0/
+-rw-r--r--   0 root         (0) root         (0)    11358 2024-04-25 12:31:00.000000 akida_models-1.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2635 2024-04-25 12:31:00.000000 akida_models-1.5.0/LICENSE.3rdparty
+-rw-r--r--   0 root         (0) root         (0)       41 2024-04-25 12:31:00.000000 akida_models-1.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      663 2024-04-25 12:31:04.004337 akida_models-1.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      147 2024-04-25 12:31:00.000000 akida_models-1.5.0/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:31:03.996337 akida_models-1.5.0/akida_models/
+-rw-r--r--   0 root         (0) root         (0)     1575 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:31:03.996337 akida_models-1.5.0/akida_models/casia_webface/
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/casia_webface/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5129 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/casia_webface/preprocessing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:31:03.996337 akida_models-1.5.0/akida_models/centernet/
+-rw-r--r--   0 root         (0) root         (0)       97 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/centernet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6804 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/centernet/centernet_loss.py
+-rw-r--r--   0 root         (0) root         (0)     3868 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/centernet/centernet_processing.py
+-rw-r--r--   0 root         (0) root         (0)     9324 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/centernet/centernet_train.py
+-rw-r--r--   0 root         (0) root         (0)    12370 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/centernet/centernet_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5823 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/centernet/model_centernet.py
+-rw-r--r--   0 root         (0) root         (0)    19474 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/cli.py
+-rw-r--r--   0 root         (0) root         (0)     6994 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/cyclic_lr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:31:04.000337 akida_models-1.5.0/akida_models/detection/
+-rw-r--r--   0 root         (0) root         (0)      164 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/detection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6706 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/detection/box_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:31:04.000337 akida_models-1.5.0/akida_models/detection/coco/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/detection/coco/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2118 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/detection/coco/data.py
+-rw-r--r--   0 root         (0) root         (0)     3707 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/detection/data.py
+-rw-r--r--   0 root         (0) root         (0)     9019 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/detection/data_augmentation.py
+-rw-r--r--   0 root         (0) root         (0)     2021 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/detection/data_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4700 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/detection/generate_anchors.py
+-rw-r--r--   0 root         (0) root         (0)    13580 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/detection/map_evaluation.py
+-rw-r--r--   0 root         (0) root         (0)     7625 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/detection/model_yolo.py
+-rw-r--r--   0 root         (0) root         (0)     6408 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/detection/preprocess_data.py
+-rw-r--r--   0 root         (0) root         (0)    10781 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/detection/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:31:04.000337 akida_models-1.5.0/akida_models/detection/voc/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/detection/voc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5650 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/detection/voc/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:31:04.000337 akida_models-1.5.0/akida_models/detection/widerface/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/detection/widerface/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3497 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/detection/widerface/data.py
+-rw-r--r--   0 root         (0) root         (0)     6762 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/detection/yolo_loss.py
+-rw-r--r--   0 root         (0) root         (0)    11994 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/detection/yolo_train.py
+-rw-r--r--   0 root         (0) root         (0)    11195 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/distiller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:31:04.000337 akida_models-1.5.0/akida_models/dvs/
+-rw-r--r--   0 root         (0) root         (0)       88 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/dvs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18531 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/dvs/dvs_generator.py
+-rw-r--r--   0 root         (0) root         (0)     6470 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/dvs/dvs_train.py
+-rw-r--r--   0 root         (0) root         (0)     7838 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/dvs/model_convtiny.py
+-rw-r--r--   0 root         (0) root         (0)    14518 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/dvs/preprocessing.py
+-rw-r--r--   0 root         (0) root         (0)     1838 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/extract.py
+-rw-r--r--   0 root         (0) root         (0)     3040 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/gamma_constraint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:31:04.000337 akida_models-1.5.0/akida_models/imagenet/
+-rw-r--r--   0 root         (0) root         (0)      215 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/imagenet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33671 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/imagenet/imagenet_labels2names.py
+-rw-r--r--   0 root         (0) root         (0)    24770 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/imagenet/imagenet_train.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/imagenet/imagenet_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4057 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/imagenet/load_samples.py
+-rw-r--r--   0 root         (0) root         (0)    19259 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/imagenet/model_akidanet.py
+-rw-r--r--   0 root         (0) root         (0)     8468 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/imagenet/model_akidanet18.py
+-rw-r--r--   0 root         (0) root         (0)     7648 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/imagenet/model_akidanet_edge.py
+-rw-r--r--   0 root         (0) root         (0)    16418 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/imagenet/model_mobilenet.py
+-rw-r--r--   0 root         (0) root         (0)     6140 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/imagenet/preprocessing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:31:04.004337 akida_models-1.5.0/akida_models/kws/
+-rw-r--r--   0 root         (0) root         (0)       57 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/kws/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5101 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/kws/kws_train.py
+-rw-r--r--   0 root         (0) root         (0)     6901 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/kws/model_ds_cnn.py
+-rw-r--r--   0 root         (0) root         (0)    29734 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/kws/preprocessing.py
+-rw-r--r--   0 root         (0) root         (0)    32119 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/layer_blocks.py
+-rw-r--r--   0 root         (0) root         (0)     2425 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/macs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:31:04.004337 akida_models-1.5.0/akida_models/mnist/
+-rw-r--r--   0 root         (0) root         (0)       27 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/mnist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3621 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/mnist/mnist_train.py
+-rw-r--r--   0 root         (0) root         (0)     4207 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/mnist/model_gxnor.py
+-rw-r--r--   0 root         (0) root         (0)     5044 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/model_io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:31:04.004337 akida_models-1.5.0/akida_models/modelnet40/
+-rw-r--r--   0 root         (0) root         (0)       94 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/modelnet40/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8939 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/modelnet40/model_pointnet_plus.py
+-rw-r--r--   0 root         (0) root         (0)     5251 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/modelnet40/modelnet40_train.py
+-rw-r--r--   0 root         (0) root         (0)     6513 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/modelnet40/pointnet_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8320 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/modelnet40/preprocessing.py
+-rw-r--r--   0 root         (0) root         (0)    10740 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/optimizers.py
+-rw-r--r--   0 root         (0) root         (0)     8177 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/param_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:31:04.004337 akida_models-1.5.0/akida_models/portrait128/
+-rw-r--r--   0 root         (0) root         (0)       32 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/portrait128/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7126 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/portrait128/model_akida_unet.py
+-rw-r--r--   0 root         (0) root         (0)     9028 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/portrait128/portrait128_train.py
+-rw-r--r--   0 root         (0) root         (0)    13688 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/training.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:31:04.004337 akida_models-1.5.0/akida_models/transformers/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/transformers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12770 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/transformers/model_deit.py
+-rw-r--r--   0 root         (0) root         (0)    17044 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/transformers/model_vit.py
+-rw-r--r--   0 root         (0) root         (0)    12195 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/unfuse_sepconv_layers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:31:04.004337 akida_models-1.5.0/akida_models/urbansound/
+-rw-r--r--   0 root         (0) root         (0)       36 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/urbansound/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1998 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/urbansound/model_vit_urbansound.py
+-rw-r--r--   0 root         (0) root         (0)     4386 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/urbansound/preprocessing.py
+-rw-r--r--   0 root         (0) root         (0)     7937 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/urbansound/urbansound_train.py
+-rw-r--r--   0 root         (0) root         (0)     7669 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:31:04.004337 akida_models-1.5.0/akida_models/utk_face/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/utk_face/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5636 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/utk_face/model_vgg.py
+-rw-r--r--   0 root         (0) root         (0)     2404 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/utk_face/preprocessing.py
+-rw-r--r--   0 root         (0) root         (0)     3795 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/utk_face/utk_face_train.py
+-rw-r--r--   0 root         (0) root         (0)      104 2024-04-25 12:31:00.000000 akida_models-1.5.0/akida_models/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:31:04.004337 akida_models-1.5.0/akida_models.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      663 2024-04-25 12:31:03.000000 akida_models-1.5.0/akida_models.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3256 2024-04-25 12:31:03.000000 akida_models-1.5.0/akida_models.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 12:31:03.000000 akida_models-1.5.0/akida_models.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      623 2024-04-25 12:31:03.000000 akida_models-1.5.0/akida_models.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2024-04-25 12:31:03.000000 akida_models-1.5.0/akida_models.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-25 12:31:03.000000 akida_models-1.5.0/akida_models.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 12:31:04.008337 akida_models-1.5.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1668 2024-04-25 12:31:00.000000 akida_models-1.5.0/setup.py
```

### Comparing `akida_models-1.4.0/LICENSE` & `akida_models-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/LICENSE.3rdparty` & `akida_models-1.5.0/LICENSE.3rdparty`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/PKG-INFO` & `akida_models-1.5.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: akida_models
-Version: 1.4.0
+Version: 1.5.0
 Summary: Akida Models
 Home-page: https://doc.brainchipinc.com
 Author: Kevin Tsiknos
 Author-email: ktsiknos@brainchip.com
 License: Apache 2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.3rdparty
-Requires-Dist: cnn2snn~=2.7.0
+Requires-Dist: cnn2snn~=2.7.2
 Requires-Dist: quantizeml~=0.8.1
 Requires-Dist: scipy
 Requires-Dist: opencv-python
 Requires-Dist: mtcnn
 Requires-Dist: imgaug
 Requires-Dist: trimesh
+Requires-Dist: librosa
 
 # Akida models
 
 This package contains a zoo of TensorFlow/Keras defined models that can be
 quantized and that are compatible for Akida conversion.
```

### Comparing `akida_models-1.4.0/akida_models/__init__.py` & `akida_models-1.5.0/akida_models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Imports models.
 """
 
 from .version import __version__
 
-from .dvs import (convtiny_dvs_gesture, convtiny_gesture_pretrained, convtiny_dvs_handy,
-                  convtiny_handy_samsung_pretrained)
+from .dvs import (convtiny_dvs, convtiny_gesture_pretrained, convtiny_handy_samsung_pretrained)
 from .imagenet import (mobilenet_imagenet, mobilenet_imagenet_pretrained, akidanet_imagenet,
                        akidanet_imagenet_pretrained, akidanet_faceidentification_pretrained,
                        akidanet_plantvillage_pretrained, akidanet_vww_pretrained,
                        akidanet_edge_imagenet, akidanet_edge_imagenet_pretrained,
                        akidanet_faceidentification_edge_pretrained, akidanet18_imagenet,
                        akidanet18_imagenet_pretrained)
 from .kws import ds_cnn_kws, ds_cnn_kws_pretrained
@@ -19,10 +18,11 @@
 from .centernet import centernet_base, centernet_voc_pretrained
 from .mnist import gxnor_mnist, gxnor_mnist_pretrained
 from .transformers import (vit_imagenet, vit_ti16, bc_vit_ti16,  bc_vit_ti16_imagenet_pretrained,
                            vit_s16, vit_s32, vit_b16, vit_b32, vit_l16, vit_l32, deit_imagenet,
                            deit_ti16, bc_deit_ti16, bc_deit_dist_ti16_imagenet_pretrained, deit_s16,
                            deit_b16)
 from .portrait128 import akida_unet_portrait128, akida_unet_portrait128_pretrained
+from .urbansound import vit_urbansound_pretrained
 
 from .utils import fetch_file
 from .model_io import load_model
```

### Comparing `akida_models-1.4.0/akida_models/casia_webface/preprocessing.py` & `akida_models-1.5.0/akida_models/casia_webface/preprocessing.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/centernet/centernet_loss.py` & `akida_models-1.5.0/akida_models/centernet/centernet_loss.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/centernet/centernet_processing.py` & `akida_models-1.5.0/akida_models/centernet/centernet_processing.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/centernet/centernet_train.py` & `akida_models-1.5.0/akida_models/centernet/centernet_train.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/centernet/centernet_utils.py` & `akida_models-1.5.0/akida_models/centernet/centernet_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,16 +214,16 @@
     sq3 = tf.sqrt(b3**2 - 4 * a3 * c3)
     r3 = (b3 + sq3) / (2 * a3)
 
     return tf.reduce_min([r1, r2, r3])
 
 
 def build_centernet_aug_pipeline():
-    """ Define a sequence of augmentation steps for Centernet training
-        that will be applied to every image.
+    """ Defines a sequence of augmentation steps for Centernet training
+    that will be applied to every image.
 
     Returns:
         iaa.Sequential: sequence of augmentation.
     """
     # augmentors by https://github.com/aleju/imgaug
     def sometimes(aug): return iaa.Sometimes(0.5, aug)
```

### Comparing `akida_models-1.4.0/akida_models/centernet/model_centernet.py` & `akida_models-1.5.0/akida_models/centernet/model_centernet.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/cli.py` & `akida_models-1.5.0/akida_models/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,33 +20,34 @@
 This package entry-point allows Keras models of Akida model zoo to be instantiated and saved at a
 specified location.
 
 """
 
 import argparse
 import os
+import sys
 
 from .utk_face.model_vgg import vgg_utk_face
 from .kws.model_ds_cnn import ds_cnn_kws
 from .modelnet40.model_pointnet_plus import pointnet_plus_modelnet40
 from .imagenet.model_mobilenet import mobilenet_imagenet
 from .imagenet.model_akidanet import akidanet_imagenet
 from .imagenet.model_akidanet_edge import akidanet_edge_imagenet
 from .imagenet.model_akidanet18 import akidanet18_imagenet
 from .detection.model_yolo import yolo_base
-from .dvs.model_convtiny_handy import convtiny_dvs_handy
-from .dvs.model_convtiny_gesture import convtiny_dvs_gesture
+from .dvs.model_convtiny import convtiny_dvs
 from .mnist.model_gxnor import gxnor_mnist
 from .transformers.model_vit import vit_ti16, bc_vit_ti16
 from .transformers.model_deit import deit_ti16, bc_deit_ti16
 from .portrait128.model_akida_unet import akida_unet_portrait128
 from .centernet.model_centernet import centernet_base
 from .macs import display_macs
 from .model_io import load_weights, save_weights, load_model
 from .unfuse_sepconv_layers import unfuse_sepconv2d
+import onnx
 
 
 def save_model_weights(model_path, weights_path):
     """ CLI entry point to save the model weights in an npz file.
 
     Args:
         model_path (str): Path to the model to extract the weights from.
@@ -138,14 +139,27 @@
                             help="The width of the model, by default %(default)s.")
 
     if bw_required is not None:
         parser.add_argument("-bw", "--base_weights", type=str, required=bw_required,
                             help="The base weights to load on model.")
 
 
+def summary_model(model_path):
+    """ CLI entry point to display a model architecture from h5/onnx/fbz file.
+
+    Args:
+        model_path (str): Path to the model.
+    """
+    model = load_model(model_path)
+    if isinstance(model, onnx.ModelProto):
+        print(onnx.helper.printable_graph(model.graph), file=sys.stdout)
+    else:
+        model.summary()
+
+
 def main():
     """ CLI entry point.
 
     Contains an argument parser with specific arguments depending on the model
     to be created. Complete arguments lists available using the -h or --help
     argument.
 
@@ -244,14 +258,16 @@
     bc_deit_parser = csp.add_parser("bc_deit_ti16", help="A DeiT, brainchip customized model")
     add_transformers_args(bc_deit_parser)
     bc_deit_parser.add_argument("-d", "--dist", action="store_true",
                                 help="Use the model with a distilled token")
     bc_deit_parser.add_argument("-b", "--blocks", type=int, default=12,
                                 help="Number of transformer blocks")
 
+    csp.add_parser("vit_urbansound", help="An audio ViT, brainchip customized model")
+
     macs_parser = sp.add_parser("macs", help="Get MACS for a Keras model")
     macs_parser.add_argument("-m", "--model", type=str)
     macs_parser.add_argument("-v", "--verbose", action="store_true")
 
     unfuse_parser = sp.add_parser(
         "unfuse", help="Unfuse SeparableConv2D layers of a Keras model")
     unfuse_parser.add_argument("-m", "--model", type=str, required=True, help="Model to unfuse.")
@@ -267,24 +283,28 @@
     # Load weights arguments
     w_parser = sp.add_parser(
         "load_weights", help="Apply weights to a model from an npz file.")
     w_parser.add_argument("-m", "--model", type=str, required=True,
                           help="Model to apply the weights.")
     w_parser.add_argument("-w", "--weights_path", type=str, required=True,
                           help="Npz file that contains the weights to apply.")
-
+    # summary model
+    sum_parser = sp.add_parser(
+        "summary",
+        help="Display a model architecture from h5/onnx/fbz file.")
+    sum_parser.add_argument("-m", "--model", type=str, required=True, help="Model to display.")
     args = parser.parse_args()
     if args.action == "create":
         # Instantiate the wished model
         if args.model == "vgg_utk_face":
             model = vgg_utk_face()
         elif args.model == "convtiny_dvs_handy":
-            model = convtiny_dvs_handy(classes=args.classes)
+            model = convtiny_dvs(input_shape=(120, 160, 2), classes=args.classes)
         elif args.model == "convtiny_dvs_gesture":
-            model = convtiny_dvs_gesture(classes=args.classes)
+            model = convtiny_dvs(input_shape=(64, 64, 10), classes=args.classes)
         elif args.model == "ds_cnn_kws":
             model = ds_cnn_kws()
         elif args.model == "pointnet_plus_modelnet40":
             model = pointnet_plus_modelnet40(alpha=args.alpha,
                                              classes=args.classes)
         elif args.model == "mobilenet_imagenet":
             input_shape = (args.image_size, args.image_size, 3)
@@ -316,14 +336,17 @@
                 model.load_weights(args.base_weights, by_name=True)
         elif args.model == "gxnor_mnist":
             model = gxnor_mnist()
         elif args.model == "akida_unet_portrait128":
             model = akida_unet_portrait128()
             if args.base_weights is not None:
                 model.load_weights(args.base_weights, by_name=True)
+        elif args.model == "vit_urbansound":
+            # Create a base ViT model with 10 classes and 1 transformer block
+            model = bc_vit_ti16(input_shape=(224, 224, 1), classes=10, num_blocks=1)
         else:
             # Handle transformer models
             if args.model == "vit_ti16":
                 input_shape = (args.image_size, args.image_size, 3)
                 model = vit_ti16(input_shape=input_shape,
                                  classes=args.classes,
                                  norm=args.norm,
@@ -378,7 +401,9 @@
         # strip file extension from model path
         model_path = os.path.splitext(args.model)[0]
         # Write new path for unfused model
         model_path += "_unfused.h5"
         # Save unfused model
         unfused_model.save(model_path, include_optimizer=False)
         print(f"{model.name} has been unfused and saved under {model_path}.")
+    elif args.action == "summary":
+        summary_model(args.model)
```

### Comparing `akida_models-1.4.0/akida_models/cyclic_lr.py` & `akida_models-1.5.0/akida_models/cyclic_lr.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/detection/box_utils.py` & `akida_models-1.5.0/akida_models/detection/box_utils.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/detection/data_augmentation.py` & `akida_models-1.5.0/akida_models/detection/data_augmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,16 +202,16 @@
 
     objects['bbox'] = boxes
 
     return objects
 
 
 def build_yolo_aug_pipeline():
-    """ Define a sequence of augmentation steps for Yolo training
-        that will be applied to every image.
+    """ Defines a sequence of augmentation steps for Yolo training
+    that will be applied to every image.
 
     Returns:
         iaa.Sequential: sequence of augmentation.
     """
     # augmentors by https://github.com/aleju/imgaug
     def sometimes(aug): return iaa.Sometimes(0.5, aug)
```

### Comparing `akida_models-1.4.0/akida_models/detection/data_utils.py` & `akida_models-1.5.0/akida_models/detection/data_utils.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/detection/generate_anchors.py` & `akida_models-1.5.0/akida_models/detection/generate_anchors.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/detection/map_evaluation.py` & `akida_models-1.5.0/akida_models/detection/map_evaluation.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,23 +19,26 @@
 """
 
 __all__ = ["MapEvaluation"]
 
 import keras
 import numpy as np
 
+from collections import defaultdict
 from keras.utils import io_utils
 from .processing import preprocess_image, decode_output
 from .box_utils import compute_overlap
 from .data_utils import Coord
 
 
 class MapEvaluation(keras.callbacks.Callback):
     """ Evaluate a given dataset using a given model.
         Code originally from https://github.com/fizyr/keras-retinanet.
+        Note that mAP is computed for IoU thresholds from 0.5 to 0.95
+        with a step size of 0.05.
 
         Args:
             model (keras.Model): model to evaluate.
             val_data (dict): dictionary containing validation data as obtained
              using `preprocess_widerface.py` module
             num_valid (int): the length of the validation dataset
             labels (list): list of labels as strings
@@ -92,54 +95,66 @@
                 result keys are prefixed with val. For training epoch, the
                 values of the Model’s metrics are returned.
                 Example: {‘loss’: 0.2, ‘acc’: 0.7}. Defaults to None.
         """
         epoch += 1
         if self._period != 0 and (epoch % self._period == 0 or
                                   epoch == self.params.get('epochs', -1)):
-            _map, average_precisions = self.evaluate_map()
+            _map_dict, average_precisions = self.evaluate_map()
+            mean_map = sum(_map_dict.values()) / len(_map_dict)
             io_utils.print_msg("")
+            io_utils.print_msg('mAP 50: {:.4f}'.format(_map_dict[0.5]))
+            io_utils.print_msg('mAP 75: {:.4f}\n'.format(_map_dict[0.75]))
             for label, average_precision in average_precisions.items():
                 io_utils.print_msg(self._labels[label] + ' {:.4f}'.format(average_precision))
-            io_utils.print_msg('mAP: {:.4f}\n'.format(_map))
-            logs.update({'map': _map})
+            io_utils.print_msg('mAP: {:.4f}\n'.format(mean_map))
+            logs.update({'map': mean_map})
 
     def evaluate_map(self):
-        """ Evaluates current mAP score on the model.
+        """ Evaluates current mAP score on the model. mAP is computed for IoU
+        thresholds from 0.5 to 0.95 with a step size of 0.05
 
         Returns:
-            tuple: global mAP score and dictionnary of label and mAP for each
-            class.
+            tuple: a dictionnary containing mAP for each threshold and a dictionnary of label
+            containing mAP for each class.
         """
-        average_precisions = self._calc_avg_precisions()
-        _map = sum(average_precisions.values()) / len(average_precisions)
+        all_detections, all_annotations = self._get_predictions()
+        all_overlaps = self._compute_all_overlaps(all_detections, all_annotations)
 
-        return _map, average_precisions
+        # Thresholds from 0.5 to 0.95 with a step size of 0.05
+        iou_thresholds = np.linspace(0.5, 0.95, num=10)
+        total_iterations = len(iou_thresholds)
+        mean_avgs = defaultdict(float)
+        map_dict = {}
+
+        for th in iou_thresholds:
+            average_precisions = self._calc_avg_precisions(all_detections, all_annotations,
+                                                           all_overlaps, th)
+            _map = sum(average_precisions.values()) / len(average_precisions)
+            map_dict[th] = _map
+
+            for label, ap in average_precisions.items():
+                mean_avgs[label] += ap / total_iterations
+
+        return map_dict, mean_avgs
 
     def _load_annotations(self, data):
-        annots = []
         objects = data['objects']
         h, w, _ = data['image'].shape
-        num_objects = objects['label'].numpy().shape[0]
-
-        for idx in range(num_objects):
-            bbox = objects['bbox'][idx].numpy()
-            annot = [
-                int(bbox[Coord.x1] * w),
-                int(bbox[Coord.y1] * h),
-                int(bbox[Coord.x2] * w),
-                int(bbox[Coord.y2] * h),
-                objects['label'].numpy()[idx]
-            ]
-            annots += [annot]
+        bbox = objects['bbox'].numpy()
+        labels = objects['label'].numpy()
 
-        return np.array(annots)
+        x1 = (bbox[:, Coord.x1] * w).astype(int)
+        y1 = (bbox[:, Coord.y1] * h).astype(int)
+        x2 = (bbox[:, Coord.x2] * w).astype(int)
+        y2 = (bbox[:, Coord.y2] * h).astype(int)
 
-    def _calc_avg_precisions(self):
+        return np.column_stack([x1, y1, x2, y2, labels])
 
+    def _get_predictions(self):
         # gather all detections and annotations
         all_detections = [[None
                            for _ in range(self._num_classes)]
                           for _ in range(self._data_len)]
         all_annotations = [[None
                             for _ in range(self._num_classes)]
                            for _ in range(self._data_len)]
@@ -198,43 +213,57 @@
             annotations = self._load_annotations(data)
 
             # copy ground truth to all_annotations
             for label in range(self._num_classes):
                 all_annotations[i][label] = annotations[annotations[:, 4] ==
                                                         label, :4].copy()
 
+        return all_detections, all_annotations
+
+    def _compute_all_overlaps(self, all_detections, all_annotations):
+        all_overlaps = {}
+        for label in range(self._num_classes):
+            for i in range(self._data_len):
+                detections = all_detections[i][label]
+                annotations = all_annotations[i][label]
+                overlaps = compute_overlap(detections, annotations,
+                                           mode="outer_product", box_format="xyxy")
+                all_overlaps[(i, label)] = overlaps
+        return all_overlaps
+
+    def _calc_avg_precisions(self, all_detections, all_annotations, all_overlaps, iou_threshold):
         # compute mAP by comparing all detections and all annotations
         average_precisions = {}
 
         for label in range(self._num_classes):
             false_positives = np.zeros((0,))
             true_positives = np.zeros((0,))
             scores = np.zeros((0,))
             num_annotations = 0.0
 
             for i in range(self._data_len):
                 detections = all_detections[i][label]
                 annotations = all_annotations[i][label]
                 num_annotations += annotations.shape[0]
+                overlaps = all_overlaps[(i, label)]
                 detected_annotations = []
 
-                for d in detections:
+                for idx, d in enumerate(detections):
                     scores = np.append(scores, d[4])
 
                     if annotations.shape[0] == 0:
                         false_positives = np.append(false_positives, 1)
                         true_positives = np.append(true_positives, 0)
                         continue
 
-                    overlaps = compute_overlap(np.expand_dims(d, axis=0), annotations,
-                                               mode="outer_product", box_format="xyxy")
-                    assigned_annotation = np.argmax(overlaps, axis=1)
-                    max_overlap = overlaps[0, assigned_annotation]
+                    assigned_annotation = np.argmax(overlaps, axis=1)[idx]
+                    max_overlap = overlaps[idx, assigned_annotation]
 
-                    if max_overlap >= 0.5 and assigned_annotation not in detected_annotations:
+                    if (max_overlap >= iou_threshold and
+                            assigned_annotation not in detected_annotations):
                         false_positives = np.append(false_positives, 0)
                         true_positives = np.append(true_positives, 1)
                         detected_annotations.append(assigned_annotation)
                     else:
                         false_positives = np.append(false_positives, 1)
                         true_positives = np.append(true_positives, 0)
```

### Comparing `akida_models-1.4.0/akida_models/detection/model_yolo.py` & `akida_models-1.5.0/akida_models/detection/model_yolo.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,33 +153,33 @@
         quantized (bool, optional): a boolean indicating whether the model should be loaded
             quantized or not. Defaults to True.
 
     Returns:
         keras.Model, list: a Keras Model instance and a list of anchors.
 
     """
-    anchors_name = 'voc_anchors.pkl'
+    anchors_name = 'coco_anchors.pkl'
     anchors_path = fetch_file(
-        'https://data.brainchip.com/dataset-mirror/voc/' + anchors_name,
+        'https://data.brainchip.com/dataset-mirror/coco/' + anchors_name,
         fname=anchors_name,
-        file_hash='b1fe1ed12691e100646cf52b1320f05abd17b2f546d3e12cdee87758cc9ed0ba',
-        cache_subdir='datasets/voc')
+        file_hash='36993699182495dd843158583515bd8d1412da978c55286ba0fefa88f5a8cace',
+        cache_subdir='datasets/coco')
     with open(anchors_path, 'rb') as handle:
         anchors = pickle.load(handle)
 
     if quantized:
         model_name_v1 = 'yolo_akidanet_voc_iq8_wq4_aq4.h5'
         file_hash_v1 = 'e65b0b6bd4b08c2796c3bbea89343748195e29e240ce28e70489c53d06ca69d9'
         model_name_v2 = 'yolo_akidanet_voc_i8_w4_a4.h5'
-        file_hash_v2 = 'e56873191274ed945b0d41db23cc46209e9800be053fef2fd8bedbea23c857c2'
+        file_hash_v2 = '60e6fbfac6dabe8509df5109d72462e21b53eae53741c619bbe89104fe4c7c4f'
     else:
         model_name_v1 = 'yolo_akidanet_voc.h5'
         file_hash_v1 = '5dff1dd3afafd512e105fa416b444431ca5f816ccc42d9efb49cfa34bd13e91d'
         model_name_v2 = 'yolo_akidanet_voc.h5'
-        file_hash_v2 = '14ad71294894f36eef2095284ef307fad81c61feb5d4577e4185c0a2c9e128be'
+        file_hash_v2 = 'e680e43a136ed3ba23580f4f4bf02be01fdf53d2675fec9c51116e9e79c083ae'
 
     model_path, model_name, file_hash = get_model_path("yolo", model_name_v1, file_hash_v1,
                                                        model_name_v2, file_hash_v2)
     model_path = fetch_file(model_path,
                             fname=model_name,
                             file_hash=file_hash,
                             cache_subdir='models')
```

### Comparing `akida_models-1.4.0/akida_models/detection/preprocess_data.py` & `akida_models-1.5.0/akida_models/detection/preprocess_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,21 @@
 
     h, w, _ = image.shape
     # Transform bbox coordinates to absolute so they are compatible with imgaug
     objects['bbox'] = _to_absolute_coord(objects['bbox'], h, w)
     flip, scale, offx, offy = init_random_vars(h, w)
 
     if training:
-        image, objects = augment_sample(image, objects, aug_pipe, labels, flip, scale, offx, offy)
+        augmented_image, augmented_objects = augment_sample(image, objects, aug_pipe, labels,
+                                                            flip, scale, offx, offy)
+        # Due to some transformation, some bboxes get deleted which throws an error in the next
+        # steps. A quick fix is to not augment these images.
+        if len(augmented_objects['bbox']) != 0:
+            image = augmented_image
+            objects = augmented_objects
 
     image = resize_image(image, input_shape)
     objects = fix_obj_position_and_size(
         objects, h, w, input_shape, scale, offx, offy, training, flip)
 
     # Transform bbox coordinates back to relative
     objects['bbox'] = _to_relative_coord(objects['bbox'], input_shape[0], input_shape[1])
```

### Comparing `akida_models-1.4.0/akida_models/detection/processing.py` & `akida_models-1.5.0/akida_models/detection/processing.py`

 * *Files 9% similar despite different names*

```diff
@@ -210,27 +210,23 @@
                 targets = _update_bbox_target(box, grid_y, grid_x, best_anchor, targets)
                 targets = _update_confidence_target(grid_y, grid_x, best_anchor, targets)
                 targets = _update_class_target(grid_y, grid_x, best_anchor, obj_indx, targets)
 
     return targets
 
 
-def decode_output(output,
-                  anchors,
-                  nb_classes,
-                  obj_threshold=0.5,
-                  nms_threshold=0.5):
+def decode_output(output, anchors, nb_classes, obj_threshold=0.5, nms_threshold=0.5):
     """ Decodes a YOLO model output.
 
     Args:
         output (tf.Tensor): model output to decode
         anchors (list): list of anchors boxes
         nb_classes (int): number of classes
-        obj_threshold (float): confidence threshold for a box
-        nms_threshold (float): non-maximal supression threshold
+        obj_threshold (float, optional): confidence threshold for a box. Defaults to 0.5.
+        nms_threshold (float, optional): non-maximal supression threshold. Defaults to 0.5.
 
     Returns:
         List of `BoundingBox` objects
     """
 
     def _sigmoid(x):
         return 1. / (1. + np.exp(-x))
@@ -247,56 +243,57 @@
 
     grid_h, grid_w, nb_box = output.shape[:3]
 
     boxes = []
 
     # decode the output by the network
     output[..., 4] = _sigmoid(output[..., 4])
-    output[...,
-           5:] = output[..., 4][..., np.newaxis] * _softmax(output[..., 5:])
+    output[..., 5:] = output[..., 4][..., np.newaxis] * _softmax(output[..., 5:])
     output[..., 5:] *= output[..., 5:] > obj_threshold
 
-    for row in range(grid_h):
-        for col in range(grid_w):
-            for b in range(nb_box):
-                # from 5th element onwards are class classes
-                classes = output[row, col, b, 5:]
-
-                if np.sum(classes) > 0:
-                    # first 4 elements are x, y, w, and h
-                    x, y, w, h = output[row, col, b, :4]
-
-                    x = (col + _sigmoid(x)
-                         ) / grid_w  # center position, unit: image width
-                    y = (row + _sigmoid(y)
-                         ) / grid_h  # center position, unit: image height
-                    w = anchors[b][0] * np.exp(w) / grid_w  # unit: image width
-                    h = anchors[b][1] * np.exp(h) / grid_h  # unit: image height
-
-                    confidence = output[row, col, b, 4]
-
-                    x1 = max(x - w / 2, 0)
-                    y1 = max(y - h / 2, 0)
-                    x2 = min(x + w / 2, grid_w)
-                    y2 = min(y + h / 2, grid_h)
+    col, row, _ = np.meshgrid(np.arange(grid_w), np.arange(grid_h), np.arange(nb_box))
 
-                    box = BoundingBox(x1, y1, x2, y2, confidence, classes)
+    x = (col + _sigmoid(output[..., 0])) / grid_w
+    y = (row + _sigmoid(output[..., 1])) / grid_h
+    w = np.array(anchors)[:, 0] * np.exp(output[..., 2]) / grid_w
+    h = np.array(anchors)[:, 1] * np.exp(output[..., 3]) / grid_h
+
+    x1 = np.maximum(x - w / 2, 0)
+    y1 = np.maximum(y - h / 2, 0)
+    x2 = np.minimum(x + w / 2, grid_w)
+    y2 = np.minimum(y + h / 2, grid_h)
+
+    confidence = output[..., 4]
+    classes = output[..., 5:]
+    mask = np.sum(classes, axis=-1) > 0
+    indices = np.where(mask)
+
+    for i in range(len(indices[0])):
+        row_idx, col_idx, box_idx = indices[0][i], indices[1][i], indices[2][i]
+
+        box = BoundingBox(x1[row_idx, col_idx, box_idx],
+                          y1[row_idx, col_idx, box_idx],
+                          x2[row_idx, col_idx, box_idx],
+                          y2[row_idx, col_idx, box_idx],
+                          confidence[row_idx, col_idx, box_idx],
+                          classes[row_idx, col_idx, box_idx])
 
-                    boxes.append(box)
+        boxes.append(box)
 
     # suppress non-maximal boxes
     for c in range(nb_classes):
-        sorted_indices = list(
-            reversed(np.argsort([box.classes[c] for box in boxes])))
+        sorted_indices = np.argsort([box.classes[c] for box in boxes])[::-1]
         for ind, index_i in enumerate(sorted_indices):
-            if boxes[index_i].classes[c] == 0:
+            if boxes[index_i].score == 0 or boxes[index_i].classes[c] == 0:
                 continue
 
             for j in range(ind + 1, len(sorted_indices)):
                 index_j = sorted_indices[j]
+                if boxes[index_j].score == 0:
+                    continue
 
                 # filter out redundant boxes (same class and overlapping too
                 # much)
                 if (boxes[index_i].iou(boxes[index_j]) >= nms_threshold) and (
                         c == boxes[index_i].get_label()) and (
                             c == boxes[index_j].get_label()):
                     boxes[index_j].score = 0
```

### Comparing `akida_models-1.4.0/akida_models/detection/voc/data.py` & `akida_models-1.5.0/akida_models/detection/voc/data.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/detection/widerface/data.py` & `akida_models-1.5.0/akida_models/detection/widerface/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,15 @@
 
     Args:
         data_path (str): path to the folder containing widerface tfrecords.
         training (bool, optional): True to retrieve training data,
             False for validation. Defaults to False.
 
     Returns:
-        tf.dataset, int: the requested dataset (train or validation)
-            and the dataset size.
+        tf.dataset, int: the requested dataset (train or validation) and the dataset size.
     """
 
     assert tfds is not None, "To load wider_face dataset, tensorflow-datasets module must\
         be installed."
 
     write_dir = os.path.join(data_path, 'tfds')
     download_and_prepare_kwargs = {
```

### Comparing `akida_models-1.4.0/akida_models/detection/yolo_loss.py` & `akida_models-1.5.0/akida_models/detection/yolo_loss.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/distiller.py` & `akida_models-1.5.0/akida_models/distiller.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/dvs/dvs_generator.py` & `akida_models-1.5.0/akida_models/dvs/dvs_generator.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/dvs/dvs_train.py` & `akida_models-1.5.0/akida_models/dvs/dvs_train.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/dvs/model_convtiny_gesture.py` & `akida_models-1.5.0/akida_models/kws/model_ds_cnn.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,160 +11,159 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ******************************************************************************
 """
-Convtiny model definition for DVS gesture classification.
+DS-CNN model definition for KWS classification.
 """
 
-__all__ = ["convtiny_dvs_gesture", "convtiny_gesture_pretrained"]
+__all__ = ["ds_cnn_kws", "ds_cnn_kws_pretrained"]
 
 from keras import Model
-from keras.layers import Input, Reshape, Dropout, Activation
+from keras.layers import Input, Reshape, Activation, Rescaling
 
 from ..layer_blocks import conv_block, separable_conv_block, dense_block
 from ..utils import fetch_file, get_params_by_version
 from ..model_io import load_model, get_model_path
 
-# Locally fixed config options
-# The number of neurons in the penultimate dense layer
-# This layer has binary output spikes, and could be a bottleneck
-# if care isn't taken to ensure enough info capacity
-NUM_SPIKING_NEURONS = 256
 
+def ds_cnn_kws(input_shape=(49, 10, 1), classes=33, include_top=True, input_scaling=(255, 0)):
+    """Instantiates a MobileNet-like model for the "Keyword Spotting" example.
 
-def convtiny_dvs_gesture(input_shape=(64, 64, 10), classes=10):
-    """Instantiates a CNN for the "IBM DVS Gesture" example.
+    This model is based on the MobileNet architecture, mainly with fewer layers.
+    The weights and activations are quantized such that it can be converted into
+    an Akida model.
+
+    This architecture is originated from https://arxiv.org/pdf/1711.07128.pdf
+    and was created for the "Keyword Spotting" (KWS) or "Speech Commands"
+    dataset.
+
+    Note: input preprocessing is included as part of the model (as a Rescaling layer). This model
+    expects inputs to be float tensors of pixels with values in the [0, 255] range.
 
     Args:
-        input_shape (tuple, optional): input shape tuple of the model. Defaults to (64, 64, 10).
-        classes (int, optional): number of classes to classify images into. Defaults to 10.
+        input_shape (tuple, optional): input shape tuple of the model. Defaults to (49, 10, 1).
+        classes (int, optional): optional number of classes to classify words into, only
+            be specified if `include_top` is True. Defaults to 33.
+        include_top (bool, optional): whether to include the classification layer at the top of the
+            model. Defaults to True.
+        input_scaling (tuple, optional): scale factor and offset to apply to
+            inputs. Defaults to (255, 0). Note that following Akida convention,
+            the scale factor is an integer used as a divisor.
 
     Returns:
-        keras.Model: a Keras convolutional model for DVS Gesture.
+        keras.Model: a Keras model for MobileNet/KWS
     """
+    if include_top and not classes:
+        raise ValueError("If 'include_top' is True, 'classes' must be set.")
+
     # Model version management
     fused, post_relu_gap, relu_activation = get_params_by_version()
 
-    img_input = Input(input_shape, name="input")
-
-    x = conv_block(img_input,
-                   filters=16,
-                   kernel_size=(3, 3),
-                   name='conv_01',
-                   use_bias=False,
-                   add_batchnorm=True,
-                   padding='same',
-                   pooling='max',
-                   pool_size=(2, 2),
-                   relu_activation=relu_activation,
-                   strides=(1, 1))
-
-    x = conv_block(x,
-                   filters=16,
-                   kernel_size=(3, 3),
-                   name='conv_02',
-                   use_bias=False,
-                   add_batchnorm=True,
-                   padding='same',
-                   pooling='max',
-                   pool_size=(2, 2),
-                   relu_activation=relu_activation,
-                   strides=(1, 1))
+    img_input = Input(shape=input_shape, name="input")
 
-    x = conv_block(x,
-                   filters=32,
-                   kernel_size=(3, 3),
-                   name='conv_03',
-                   use_bias=False,
-                   add_batchnorm=True,
-                   padding='same',
-                   pooling='max',
-                   pool_size=(2, 2),
-                   relu_activation=relu_activation,
-                   strides=(1, 1))
+    if input_scaling is None:
+        x = img_input
+    else:
+        scale, offset = input_scaling
+        x = Rescaling(1. / scale, offset, name="rescaling")(img_input)
 
     x = conv_block(x,
                    filters=64,
-                   kernel_size=(3, 3),
-                   name='conv_04',
-                   use_bias=False,
-                   add_batchnorm=True,
+                   kernel_size=(5, 5),
                    padding='same',
-                   pooling='max',
-                   pool_size=(2, 2),
-                   relu_activation=relu_activation,
-                   strides=(1, 1))
-
-    x = conv_block(x,
-                   filters=128,
-                   kernel_size=(3, 3),
-                   name='conv_05',
+                   strides=(2, 2),
                    use_bias=False,
+                   name='conv_0',
                    add_batchnorm=True,
-                   padding='same',
-                   pooling='global_avg',
-                   relu_activation=relu_activation,
-                   post_relu_gap=post_relu_gap,
-                   strides=(1, 1))
+                   relu_activation=relu_activation)
 
-    bm_outshape = (1, 1, 128)
+    x = separable_conv_block(x,
+                             filters=64,
+                             kernel_size=(3, 3),
+                             padding='same',
+                             use_bias=False,
+                             name='separable_1',
+                             add_batchnorm=True,
+                             fused=fused,
+                             relu_activation=relu_activation)
 
-    x = Reshape(bm_outshape, name='reshape_1')(x)
-    x = Dropout(1e-3, name='dropout')(x)
+    x = separable_conv_block(x,
+                             filters=64,
+                             kernel_size=(3, 3),
+                             padding='same',
+                             use_bias=False,
+                             name='separable_2',
+                             add_batchnorm=True,
+                             fused=fused,
+                             relu_activation=relu_activation)
 
     x = separable_conv_block(x,
-                             filters=NUM_SPIKING_NEURONS,
+                             filters=64,
                              kernel_size=(3, 3),
+                             padding='same',
                              use_bias=False,
+                             name='separable_3',
+                             add_batchnorm=True,
+                             fused=fused,
+                             relu_activation=relu_activation)
+
+    x = separable_conv_block(x,
+                             filters=64,
+                             kernel_size=(3, 3),
                              padding='same',
-                             name='spiking_layer',
+                             use_bias=False,
+                             name='separable_4',
+                             pooling='global_avg',
                              add_batchnorm=True,
-                             pooling=None,
-                             relu_activation=relu_activation,
-                             fused=fused)
-
-    x = dense_block(x,
-                    units=classes,
-                    name='dense',
-                    add_batchnorm=False,
-                    relu_activation=False,
-                    use_bias=False)
-    act_function = 'softmax' if classes > 1 else 'sigmoid'
-    x = Activation(act_function, name=f'act_{act_function}')(x)
-    x = Reshape((classes,), name='reshape_2')(x)
-
-    return Model(inputs=img_input, outputs=x, name='dvs_network')
-
-
-def convtiny_gesture_pretrained(quantized=True):
-    """ Helper method to retrieve a `convtiny_dvs_gesture` model that was
-    trained on IBM DVS Gesture dataset.
+                             fused=fused,
+                             post_relu_gap=post_relu_gap,
+                             relu_activation=relu_activation)
+
+    if include_top:
+        x = dense_block(x,
+                        units=classes,
+                        name='dense_5',
+                        use_bias=True,
+                        relu_activation=False)
+        act_function = 'softmax' if classes > 1 else 'sigmoid'
+        x = Activation(act_function, name=f'act_{act_function}')(x)
+    else:
+        shape = (1, 1, int(64))
+        x = Reshape(shape, name='reshape_1')(x)
+
+    return Model(img_input, x, name='ds_cnn_kws')
+
+
+def ds_cnn_kws_pretrained(quantized=True):
+    """
+    Helper method to retrieve a `ds_cnn_kws` model that was trained on
+    KWS dataset.
 
     Args:
         quantized (bool, optional): a boolean indicating whether the model should be loaded
             quantized or not. Defaults to True.
 
     Returns:
         keras.Model: a Keras Model instance.
 
     """
     if quantized:
-        model_name_v1 = 'convtiny_dvs_gesture_iq4_wq4_aq4.h5'
-        file_hash_v1 = 'ad1a0a2ee13092921a914f25a6159dcb788540239d10ea96d3ff5fefec359281'
-        model_name_v2 = 'convtiny_dvs_gesture_i4_w4_a4.h5'
-        file_hash_v2 = '2921c29c04c0fda278000df18bb63d77c1e8a2d3bc23e32963f92072d26c2771'
+        model_name_v1 = 'ds_cnn_kws_iq8_wq4_aq4_laq1.h5'
+        file_hash_v1 = '2ba6220bb9545857c99a327ec14d2d777420c7848cb6a9b17d87e5a01951fe6f'
+        model_name_v2 = 'ds_cnn_kws_edge_i8_w4_a4.h5'
+        file_hash_v2 = '30e514563be67251a89705c296a137bd79b15918bdb8d6ca7daa02a05506775b'
     else:
-        model_name_v1 = None
-        file_hash_v1 = None
-        model_name_v2 = 'convtiny_dvs_gesture.h5'
-        file_hash_v2 = 'aa576ec4981796643e55d877ddac36c545832d6b1f449a01624fd178baffc587'
+        model_name_v1 = 'ds_cnn_kws.h5'
+        file_hash_v1 = '95a51677b340ee2420015a8576a8aaf41e84138ac0334cd42080b60499b4f146'
+        model_name_v2 = 'ds_cnn_kws.h5'
+        file_hash_v2 = 'e897da2760206aad1328179c2b6861bae4f0e56a9380c78cf1287d18929a2143'
 
-    model_path, model_name, file_hash = get_model_path("convtiny", model_name_v1, file_hash_v1,
+    model_path, model_name, file_hash = get_model_path("ds_cnn", model_name_v1, file_hash_v1,
                                                        model_name_v2, file_hash_v2)
     model_path = fetch_file(model_path,
                             fname=model_name,
                             file_hash=file_hash,
                             cache_subdir='models')
     return load_model(model_path)
```

### Comparing `akida_models-1.4.0/akida_models/dvs/model_convtiny_handy.py` & `akida_models-1.5.0/akida_models/portrait128/model_akida_unet.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,183 +1,153 @@
 #!/usr/bin/env python
 # ******************************************************************************
-# Copyright 2020 Brainchip Holdings Ltd.
+# Copyright 2022 Brainchip Holdings Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ******************************************************************************
 """
-Convtiny model definition for DVS handy classification.
+Akida U-Net model definition for semantic segmentation.
 """
 
-__all__ = ["convtiny_dvs_handy", "convtiny_handy_samsung_pretrained"]
+__all__ = ["akida_unet_portrait128", "akida_unet_portrait128_pretrained"]
 
-from keras import Model
-from keras.layers import Input, Reshape, Dropout, Activation
+from keras import Model, regularizers
+from keras.layers import Dropout, Activation
 
-from ..layer_blocks import conv_block, separable_conv_block, dense_block
-from ..utils import fetch_file, get_params_by_version
-from ..model_io import load_model, get_model_path
+from cnn2snn import set_akida_version, AkidaVersion
 
-# Locally fixed config options
-# The number of neurons in the penultimate dense layer
-# This layer has binary output spikes, and could be a bottleneck
-# if care isn't taken to ensure enough info capacity
-NUM_SPIKING_NEURONS = 256
+from ..layer_blocks import sepconv_transpose_block, conv_block
+from ..imagenet.model_akidanet import akidanet_imagenet
+from ..utils import fetch_file
+from ..model_io import load_model, get_model_path
 
 
-def convtiny_dvs_handy(input_shape=(120, 160, 2), classes=9):
-    """Instantiates a CNN for "Brainchip dvs_handy" example.
+def akida_unet_portrait128(input_shape=(128, 128, 3),
+                           alpha=0.5,
+                           input_scaling=(128, -1)):
+    """Instantiates an Akida U-Net architecture.
+
+    It is composed of an AkidaNet-ImageNet encoder followed by a succession of Conv2DTranspose
+    layers for the decoder part.
+    It does not contain any skip connection (concatenation) between the encoder and the decoder
+    branches.
 
     Args:
-        input_shape (tuple, optional): input shape tuple of the model. Defaults to (120, 160, 2).
-        classes (int, optional): number of classes to classify images into. Defaults to 9.
+        input_shape (tuple, optional): input shape tuple. Defaults to (128, 128, 3).
+        alpha (float, optional): controls the width (number of filters) of the model. Defaults to
+            0.5.
+        input_scaling (tuple, optional): scale factor and offset to apply to inputs. Defaults to
+            (128, -1). Note that following Akida convention, the scale factor is a number used as a
+            divisor.
 
     Returns:
-        keras.Model: a Keras convolutional model for DVS Gesture.
+        keras.Model: a Keras Model instance.
     """
+    # This model is only available for akida 2.0
+    with set_akida_version(AkidaVersion.v2):
+        # Define weight regularization, will apply to pointwise weights of sepconv transposed layers
+        weight_regularizer = regularizers.l2(4e-5)
+
+        # Create an AkidaNet network without top layers
+        encoder = akidanet_imagenet(input_shape=input_shape,
+                                    alpha=alpha,
+                                    include_top=False,
+                                    input_scaling=input_scaling)
+
+        # Add the decoder layers
+        x = encoder.layers[-1].output
+        x = sepconv_transpose_block(x,
+                                    filters=int(512 * alpha),
+                                    kernel_size=(3, 3),
+                                    strides=2,
+                                    padding='same',
+                                    kernel_initializer='he_normal',
+                                    add_batchnorm=True,
+                                    relu_activation='ReLU7.5',
+                                    name='sepconv_t_0',
+                                    pointwise_regularizer=weight_regularizer)
+        x = Dropout(0.5)(x)
+        x = sepconv_transpose_block(x,
+                                    filters=int(256 * alpha),
+                                    kernel_size=(3, 3),
+                                    strides=2,
+                                    padding='same',
+                                    kernel_initializer='he_normal',
+                                    add_batchnorm=True,
+                                    relu_activation='ReLU7.5',
+                                    name='sepconv_t_1',
+                                    pointwise_regularizer=weight_regularizer)
+        x = Dropout(0.5)(x)
+        x = sepconv_transpose_block(x,
+                                    filters=int(128 * alpha),
+                                    kernel_size=(3, 3),
+                                    strides=2,
+                                    padding='same',
+                                    kernel_initializer='he_normal',
+                                    add_batchnorm=True,
+                                    relu_activation='ReLU7.5',
+                                    name='sepconv_t_2',
+                                    pointwise_regularizer=weight_regularizer)
+        x = Dropout(0.5)(x)
+        x = sepconv_transpose_block(x,
+                                    filters=int(64 * alpha),
+                                    kernel_size=(3, 3),
+                                    strides=2,
+                                    padding='same',
+                                    kernel_initializer='he_normal',
+                                    add_batchnorm=True,
+                                    relu_activation='ReLU7.5',
+                                    name='sepconv_t_3',
+                                    pointwise_regularizer=weight_regularizer)
+        x = Dropout(0.5)(x)
+        x = sepconv_transpose_block(x,
+                                    filters=int(32 * alpha),
+                                    kernel_size=(3, 3),
+                                    strides=2,
+                                    padding='same',
+                                    kernel_initializer='he_normal',
+                                    add_batchnorm=True,
+                                    relu_activation='ReLU7.5',
+                                    name='sepconv_t_4',
+                                    pointwise_regularizer=weight_regularizer)
+        x = Dropout(0.5)(x)
+        x = conv_block(x, filters=1, kernel_size=(1, 1), relu_activation=False, name='head')
+        x = Activation('sigmoid', name="sigmoid_act")(x)
 
-    img_input = Input(input_shape, name="input")
+    # Build the whole model: encoder followed by decoder
+    return Model(inputs=encoder.input, outputs=x, name='akida_unet')
 
-    # Model version management
-    fused, post_relu_gap, relu_activation = get_params_by_version()
 
-    x = conv_block(img_input,
-                   filters=16,
-                   kernel_size=(3, 3),
-                   name='conv_0',
-                   use_bias=False,
-                   add_batchnorm=True,
-                   padding='same',
-                   pooling='max',
-                   pool_size=(2, 2),
-                   relu_activation=relu_activation,
-                   strides=(1, 1))
-
-    x = conv_block(x,
-                   filters=32,
-                   kernel_size=(3, 3),
-                   name='conv_1',
-                   use_bias=False,
-                   add_batchnorm=True,
-                   padding='same',
-                   pooling='max',
-                   pool_size=(2, 2),
-                   relu_activation=relu_activation,
-                   strides=(1, 1))
-
-    x = conv_block(x,
-                   filters=64,
-                   kernel_size=(3, 3),
-                   name='conv_2',
-                   use_bias=False,
-                   add_batchnorm=True,
-                   padding='same',
-                   pooling='max',
-                   pool_size=(2, 2),
-                   relu_activation=relu_activation,
-                   strides=(1, 1))
-
-    x = conv_block(x,
-                   filters=128,
-                   kernel_size=(3, 3),
-                   name='conv_3',
-                   use_bias=False,
-                   add_batchnorm=True,
-                   padding='same',
-                   pooling='max',
-                   pool_size=(2, 2),
-                   relu_activation=relu_activation,
-                   strides=(1, 1))
-
-    x = conv_block(x,
-                   filters=256,
-                   kernel_size=(3, 3),
-                   name='conv_4',
-                   use_bias=False,
-                   add_batchnorm=True,
-                   padding='same',
-                   pooling='max',
-                   pool_size=(2, 2),
-                   relu_activation=relu_activation,
-                   strides=(1, 1))
-
-    x = conv_block(x,
-                   filters=512,
-                   kernel_size=(3, 3),
-                   name='conv_5',
-                   use_bias=False,
-                   add_batchnorm=True,
-                   padding='same',
-                   pooling='global_avg',
-                   relu_activation=relu_activation,
-                   post_relu_gap=post_relu_gap,
-                   strides=(1, 1))
-
-    bm_outshape = (1, 1, 512)
-
-    x = Reshape(bm_outshape, name='reshape_1')(x)
-    x = Dropout(1e-3, name='dropout')(x)
-
-    x = separable_conv_block(x,
-                             filters=NUM_SPIKING_NEURONS,
-                             kernel_size=(3, 3),
-                             use_bias=False,
-                             padding='same',
-                             name='spiking_layer',
-                             add_batchnorm=True,
-                             pooling=None,
-                             relu_activation=relu_activation,
-                             fused=fused)
-
-    x = dense_block(x,
-                    units=classes,
-                    name='dense',
-                    add_batchnorm=False,
-                    relu_activation=False,
-                    use_bias=False)
-
-    act_function = 'softmax' if classes > 1 else 'sigmoid'
-    x = Activation(act_function, name=f'act_{act_function}')(x)
-    x = Reshape((classes,), name='reshape_2')(x)
-
-    return Model(inputs=img_input, outputs=x, name='dvs_network')
-
-
-def convtiny_handy_samsung_pretrained(quantized=True):
-    """ Helper method to retrieve a `convtiny_dvs_handy` model that was trained
-    on samsung_handy dataset.
+def akida_unet_portrait128_pretrained(quantized=True):
+    """
+    Helper method to retrieve an `akida_unet` model that was trained on portrait128 dataset.
 
     Args:
         quantized (bool, optional): a boolean indicating whether the model should be loaded
-                quantized or not. Defaults to True.
+            quantized or not. Defaults to True.
+
     Returns:
         keras.Model: a Keras Model instance.
 
     """
     if quantized:
-        model_name_v1 = 'convtiny_dvs_handy_samsung_iq4_wq4_aq4.h5'
-        file_hash_v1 = 'ac5dbf1420fbedc402da4394bb22cf94ff5cff73adb428cca741d6550f663c71'
-        model_name_v2 = 'convtiny_dvs_handy_samsung_i4_w4_a4.h5'
-        file_hash_v2 = '29cd8beabcb0576312e8673e8bf7cc41b92f6be82685357f848dfae39a172076'
+        model_name_v2 = 'akida_unet_portrait128_i8_w8_a8.h5'
+        file_hash_v2 = 'cf5b2eff3b272e3bf3070b36f9e6ca903ac2694b976557053498a72643899a59'
     else:
-        model_name_v1 = None
-        file_hash_v1 = None
-        model_name_v2 = 'convtiny_dvs_handy_samsung.h5'
-        file_hash_v2 = '6cfb0e120f51dbad4961eb9ebdec32449f7113ddc55f864c0374f72fc77ae664'
-
-    model_path, model_name, file_hash = get_model_path("convtiny", model_name_v1, file_hash_v1,
-                                                       model_name_v2, file_hash_v2)
-    model_path = fetch_file(model_path,
-                            fname=model_name,
-                            file_hash=file_hash,
+        model_name_v2 = 'akida_unet_portrait128.h5'
+        file_hash_v2 = '2274a375c02c104a5078b11f64d6986e1ca45c0da7ef5eacce8b2c71e1c35037'
+
+    model_path, model_name, file_hash = get_model_path("akida_unet", model_name_v2=model_name_v2,
+                                                       file_hash_v2=file_hash_v2)
+    model_path = fetch_file(model_path, fname=model_name, file_hash=file_hash,
                             cache_subdir='models')
     return load_model(model_path)
```

### Comparing `akida_models-1.4.0/akida_models/dvs/preprocessing.py` & `akida_models-1.5.0/akida_models/dvs/preprocessing.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/extract.py` & `akida_models-1.5.0/akida_models/extract.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/gamma_constraint.py` & `akida_models-1.5.0/akida_models/gamma_constraint.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/imagenet/imagenet_labels2names.py` & `akida_models-1.5.0/akida_models/imagenet/imagenet_labels2names.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/imagenet/imagenet_train.py` & `akida_models-1.5.0/akida_models/imagenet/imagenet_train.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/imagenet/imagenet_utils.py` & `akida_models-1.5.0/akida_models/imagenet/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/imagenet/load_samples.py` & `akida_models-1.5.0/akida_models/imagenet/load_samples.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/imagenet/model_akidanet.py` & `akida_models-1.5.0/akida_models/imagenet/model_akidanet.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/imagenet/model_akidanet18.py` & `akida_models-1.5.0/akida_models/imagenet/model_akidanet18.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/imagenet/model_akidanet_edge.py` & `akida_models-1.5.0/akida_models/imagenet/model_akidanet_edge.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/imagenet/model_mobilenet.py` & `akida_models-1.5.0/akida_models/imagenet/model_mobilenet.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/imagenet/preprocessing.py` & `akida_models-1.5.0/akida_models/imagenet/preprocessing.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/kws/kws_train.py` & `akida_models-1.5.0/akida_models/kws/kws_train.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/kws/model_ds_cnn.py` & `akida_models-1.5.0/akida_models/dvs/model_convtiny.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,160 +11,193 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ******************************************************************************
 """
-DS-CNN model definition for KWS classification.
+Convtiny model definition for DVS Gesture or DVS Handy classification.
 """
 
-__all__ = ["ds_cnn_kws", "ds_cnn_kws_pretrained"]
+__all__ = ["convtiny_dvs", "convtiny_gesture_pretrained", "convtiny_handy_samsung_pretrained"]
 
 from keras import Model
-from keras.layers import (Input, Reshape, Activation, Flatten, Rescaling)
+from keras.layers import Input, Reshape, Dropout, Activation
 
 from ..layer_blocks import conv_block, separable_conv_block, dense_block
 from ..utils import fetch_file, get_params_by_version
 from ..model_io import load_model, get_model_path
 
+# Locally fixed config options
+# The number of neurons in the penultimate dense layer
+# This layer has binary output spikes, and could be a bottleneck
+# if care isn't taken to ensure enough info capacity
+NUM_SPIKING_NEURONS = 256
 
-def ds_cnn_kws(input_shape=(49, 10, 1), classes=33, include_top=True, input_scaling=(255, 0)):
-    """Instantiates a MobileNet-like model for the "Keyword Spotting" example.
 
-    This model is based on the MobileNet architecture, mainly with fewer layers.
-    The weights and activations are quantized such that it can be converted into
-    an Akida model.
-
-    This architecture is originated from https://arxiv.org/pdf/1711.07128.pdf
-    and was created for the "Keyword Spotting" (KWS) or "Speech Commands"
-    dataset.
-
-    Note: input preprocessing is included as part of the model (as a Rescaling layer). This model
-    expects inputs to be float tensors of pixels with values in the [0, 255] range.
+def convtiny_dvs(input_shape=(64, 64, 10), classes=10):
+    """Instantiates a CNN for the "IBM DVS Gesture" or "Brainchip dvs_handy" examples.
 
     Args:
-        input_shape (tuple, optional): input shape tuple of the model. Defaults to (49, 10, 1).
-        classes (int, optional): optional number of classes to classify words into, only
-            be specified if `include_top` is True. Defaults to 33.
-        include_top (bool, optional): whether to include the classification layer at the top of the
-            model. Defaults to True.
-        input_scaling (tuple, optional): scale factor and offset to apply to
-            inputs. Defaults to (255, 0). Note that following Akida convention,
-            the scale factor is an integer used as a divisor.
+        input_shape (tuple, optional): input shape tuple of the model. Defaults to (64, 64, 10).
+        classes (int, optional): number of classes to classify images into. Defaults to 10.
 
     Returns:
-        keras.Model: a Keras model for MobileNet/KWS
+        keras.Model: a Keras convolutional model for DVS Gesture or DVS Handy.
     """
-    if include_top and not classes:
-        raise ValueError("If 'include_top' is True, 'classes' must be set.")
-
     # Model version management
     fused, post_relu_gap, relu_activation = get_params_by_version()
 
-    img_input = Input(shape=input_shape, name="input")
+    img_input = Input(input_shape, name="input")
 
-    if input_scaling is None:
-        x = img_input
-    else:
-        scale, offset = input_scaling
-        x = Rescaling(1. / scale, offset, name="rescaling")(img_input)
+    x = conv_block(img_input,
+                   filters=16,
+                   kernel_size=(3, 3),
+                   name='conv_01',
+                   use_bias=False,
+                   add_batchnorm=True,
+                   padding='same',
+                   pooling='max',
+                   pool_size=(2, 2),
+                   relu_activation=relu_activation,
+                   strides=(1, 1))
+
+    x = conv_block(x,
+                   filters=16,
+                   kernel_size=(3, 3),
+                   name='conv_02',
+                   use_bias=False,
+                   add_batchnorm=True,
+                   padding='same',
+                   pooling='max',
+                   pool_size=(2, 2),
+                   relu_activation=relu_activation,
+                   strides=(1, 1))
+
+    x = conv_block(x,
+                   filters=32,
+                   kernel_size=(3, 3),
+                   name='conv_03',
+                   use_bias=False,
+                   add_batchnorm=True,
+                   padding='same',
+                   pooling='max',
+                   pool_size=(2, 2),
+                   relu_activation=relu_activation,
+                   strides=(1, 1))
 
     x = conv_block(x,
                    filters=64,
-                   kernel_size=(5, 5),
+                   kernel_size=(3, 3),
+                   name='conv_04',
+                   use_bias=False,
+                   add_batchnorm=True,
                    padding='same',
-                   strides=(2, 2),
+                   pooling='max',
+                   pool_size=(2, 2),
+                   relu_activation=relu_activation,
+                   strides=(1, 1))
+
+    x = conv_block(x,
+                   filters=128,
+                   kernel_size=(3, 3),
+                   name='conv_05',
                    use_bias=False,
-                   name='conv_0',
                    add_batchnorm=True,
-                   relu_activation=relu_activation)
+                   padding='same',
+                   pooling='global_avg',
+                   relu_activation=relu_activation,
+                   post_relu_gap=post_relu_gap,
+                   strides=(1, 1))
 
-    x = separable_conv_block(x,
-                             filters=64,
-                             kernel_size=(3, 3),
-                             padding='same',
-                             use_bias=False,
-                             name='separable_1',
-                             add_batchnorm=True,
-                             fused=fused,
-                             relu_activation=relu_activation)
+    bm_outshape = (1, 1, 128)
 
-    x = separable_conv_block(x,
-                             filters=64,
-                             kernel_size=(3, 3),
-                             padding='same',
-                             use_bias=False,
-                             name='separable_2',
-                             add_batchnorm=True,
-                             fused=fused,
-                             relu_activation=relu_activation)
+    x = Reshape(bm_outshape, name='reshape_1')(x)
+    x = Dropout(1e-3, name='dropout')(x)
 
     x = separable_conv_block(x,
-                             filters=64,
+                             filters=NUM_SPIKING_NEURONS,
                              kernel_size=(3, 3),
-                             padding='same',
                              use_bias=False,
-                             name='separable_3',
-                             add_batchnorm=True,
-                             fused=fused,
-                             relu_activation=relu_activation)
-
-    x = separable_conv_block(x,
-                             filters=64,
-                             kernel_size=(3, 3),
                              padding='same',
-                             use_bias=False,
-                             name='separable_4',
-                             pooling='global_avg',
+                             name='spiking_layer',
                              add_batchnorm=True,
-                             fused=fused,
-                             post_relu_gap=post_relu_gap,
-                             relu_activation=relu_activation)
-
-    shape = (1, 1, int(64))
-    x = Reshape(shape, name='reshape_1')(x)
-
-    if include_top:
-        x = Flatten(name="flatten")(x)
-        x = dense_block(x,
-                        units=classes,
-                        name='dense_5',
-                        use_bias=True,
-                        relu_activation=False)
-        act_function = 'softmax' if classes > 1 else 'sigmoid'
-        x = Activation(act_function, name=f'act_{act_function}')(x)
+                             pooling=None,
+                             relu_activation=relu_activation,
+                             fused=fused)
+
+    x = dense_block(x,
+                    units=classes,
+                    name='dense',
+                    add_batchnorm=False,
+                    relu_activation=False,
+                    use_bias=False)
+    act_function = 'softmax' if classes > 1 else 'sigmoid'
+    x = Activation(act_function, name=f'act_{act_function}')(x)
+    x = Reshape((classes,), name='reshape_2')(x)
+
+    return Model(inputs=img_input, outputs=x, name='dvs_network')
+
+
+def convtiny_gesture_pretrained(quantized=True):
+    """ Helper method to retrieve a `convtiny_dvs_gesture` model that was
+    trained on IBM DVS Gesture dataset.
 
-    return Model(img_input, x, name='ds_cnn_kws')
+    Args:
+        quantized (bool, optional): a boolean indicating whether the model should be loaded
+            quantized or not. Defaults to True.
 
+    Returns:
+        keras.Model: a Keras Model instance.
 
-def ds_cnn_kws_pretrained(quantized=True):
     """
-    Helper method to retrieve a `ds_cnn_kws` model that was trained on
-    KWS dataset.
+    if quantized:
+        model_name_v1 = 'convtiny_dvs_gesture_iq4_wq4_aq4.h5'
+        file_hash_v1 = 'ad1a0a2ee13092921a914f25a6159dcb788540239d10ea96d3ff5fefec359281'
+        model_name_v2 = 'convtiny_dvs_gesture_i4_w4_a4.h5'
+        file_hash_v2 = '2921c29c04c0fda278000df18bb63d77c1e8a2d3bc23e32963f92072d26c2771'
+    else:
+        model_name_v1 = None
+        file_hash_v1 = None
+        model_name_v2 = 'convtiny_dvs_gesture.h5'
+        file_hash_v2 = 'aa576ec4981796643e55d877ddac36c545832d6b1f449a01624fd178baffc587'
+
+    model_path, model_name, file_hash = get_model_path("convtiny", model_name_v1, file_hash_v1,
+                                                       model_name_v2, file_hash_v2)
+    model_path = fetch_file(model_path,
+                            fname=model_name,
+                            file_hash=file_hash,
+                            cache_subdir='models')
+    return load_model(model_path)
+
+
+def convtiny_handy_samsung_pretrained(quantized=True):
+    """ Helper method to retrieve a `convtiny_dvs_handy` model that was trained
+    on samsung_handy dataset.
+    Note that V1 models use different architecture and they are not aligned
+    with DVS Gesture model.
 
     Args:
         quantized (bool, optional): a boolean indicating whether the model should be loaded
-            quantized or not. Defaults to True.
-
+                quantized or not. Defaults to True.
     Returns:
         keras.Model: a Keras Model instance.
 
     """
     if quantized:
-        model_name_v1 = 'ds_cnn_kws_iq8_wq4_aq4_laq1.h5'
-        file_hash_v1 = '2ba6220bb9545857c99a327ec14d2d777420c7848cb6a9b17d87e5a01951fe6f'
-        model_name_v2 = 'ds_cnn_kws_edge_i8_w4_a4.h5'
-        file_hash_v2 = '02a6b5c5496e8ef8fb576ee7b2833427ebdd7a70df26cc87db5e416f756042d5'
+        model_name_v1 = 'convtiny_dvs_handy_samsung_iq4_wq4_aq4.h5'
+        file_hash_v1 = 'ac5dbf1420fbedc402da4394bb22cf94ff5cff73adb428cca741d6550f663c71'
+        model_name_v2 = 'convtiny_dvs_handy_samsung_i4_w4_a4.h5'
+        file_hash_v2 = '07b5c77e534e59af66aaeee3769658c4c00404ceb1a66f43fcc9d64ec53dbca7'
     else:
-        model_name_v1 = 'ds_cnn_kws.h5'
-        file_hash_v1 = '95a51677b340ee2420015a8576a8aaf41e84138ac0334cd42080b60499b4f146'
-        model_name_v2 = 'ds_cnn_kws.h5'
-        file_hash_v2 = '54a4071833ef2f0a2da4fd300c2d1534acf211ee7e2838c7f55df5135cf4a8c4'
+        model_name_v1 = None
+        file_hash_v1 = None
+        model_name_v2 = 'convtiny_dvs_handy_samsung.h5'
+        file_hash_v2 = '141044f5c8a1a3f0a01de2e9751dfb2ea7738f05df2485a108f744bde6f1131d'
 
-    model_path, model_name, file_hash = get_model_path("ds_cnn", model_name_v1, file_hash_v1,
+    model_path, model_name, file_hash = get_model_path("convtiny", model_name_v1, file_hash_v1,
                                                        model_name_v2, file_hash_v2)
     model_path = fetch_file(model_path,
                             fname=model_name,
                             file_hash=file_hash,
                             cache_subdir='models')
     return load_model(model_path)
```

### Comparing `akida_models-1.4.0/akida_models/kws/preprocessing.py` & `akida_models-1.5.0/akida_models/kws/preprocessing.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/layer_blocks.py` & `akida_models-1.5.0/akida_models/layer_blocks.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/macs.py` & `akida_models-1.5.0/akida_models/macs.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/mnist/mnist_train.py` & `akida_models-1.5.0/akida_models/mnist/mnist_train.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/mnist/model_gxnor.py` & `akida_models-1.5.0/akida_models/mnist/model_gxnor.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/model_io.py` & `akida_models-1.5.0/akida_models/model_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,34 +22,42 @@
 import numpy as np
 from pathlib import Path
 from posixpath import join as urljoin
 
 from cnn2snn import load_quantized_model, get_akida_version, AkidaVersion
 from quantizeml.models import load_model as qml_load_model
 from quantizeml.models.utils import apply_weights_to_model
-
 from .layer_blocks import GELU
+import akida
+import onnx
 
 
 def load_model(model_path):
-    """Combine the cnn2snn.load_quantized_model and quantizeml.load_model
+    """Combine the cnn2snn.load_quantized_model, quantizeml.load_model,
+        akida.load_model and onnx.load
 
     Args:
         model_path (str): model path
 
     Returns:
         keras.Model: the load model
     """
     try:
         model = load_quantized_model(model_path)
     except Exception:
         try:
             model = qml_load_model(model_path, custom_layers={'GELU': GELU})
-        except Exception as e:
-            raise e.__class__('Cannot load provided model.')
+        except Exception:
+            try:
+                model = onnx.load(model_path)
+            except Exception:
+                try:
+                    model = akida.Model(model_path)
+                except Exception as e:
+                    raise e.__class__('Cannot load provided model.')
     return model
 
 
 def load_weights(model, weights_path):
     """Loads weights from a npz file and apply it to a model.
 
     Go through the dictionary of weights of the npz file, find the
```

### Comparing `akida_models-1.4.0/akida_models/modelnet40/model_pointnet_plus.py` & `akida_models-1.5.0/akida_models/modelnet40/model_pointnet_plus.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/modelnet40/modelnet40_train.py` & `akida_models-1.5.0/akida_models/modelnet40/modelnet40_train.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/modelnet40/pointnet_utils.py` & `akida_models-1.5.0/akida_models/modelnet40/pointnet_utils.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/modelnet40/preprocessing.py` & `akida_models-1.5.0/akida_models/modelnet40/preprocessing.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/optimizers.py` & `akida_models-1.5.0/akida_models/optimizers.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/param_scheduler.py` & `akida_models-1.5.0/akida_models/param_scheduler.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/portrait128/portrait128_train.py` & `akida_models-1.5.0/akida_models/portrait128/portrait128_train.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/training.py` & `akida_models-1.5.0/akida_models/training.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/transformers/model_deit.py` & `akida_models-1.5.0/akida_models/transformers/model_deit.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,15 @@
             quantized or not. Defaults to True.
 
     Returns:
         keras.Model: a Keras Model instance
     """
     if quantized:
         model_name_v2 = 'bc_deit_dist_ti16_224_i8_w8_a8.h5'
-        file_hash_v2 = '4e40e36beb56a926b18cab4c5880aa3cbe768e0e40c9c91abca6063a72763044'
+        file_hash_v2 = '02dbb25e365324e9ede4a8c71058a91f4064e6ff231bda6f8f79ead6aae0700c'
     else:
         model_name_v2 = 'bc_deit_dist_ti16_224.h5'
         file_hash_v2 = '40618ba14d894fc308ef149c1eb17ff601ad54a8bc0ad329dc6f7dba5ff86260'
 
     model_path, model_name, file_hash = get_model_path("deit", model_name_v2=model_name_v2,
                                                        file_hash_v2=file_hash_v2)
     model_path = fetch_file(model_path,
```

### Comparing `akida_models-1.4.0/akida_models/transformers/model_vit.py` & `akida_models-1.5.0/akida_models/transformers/model_vit.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,15 +308,15 @@
             quantized or not. Defaults to True.
 
     Returns:
         keras.Model: a Keras Model instance
     """
     if quantized:
         model_name_v2 = 'bc_vit_ti16_224_i8_w8_a8.h5'
-        file_hash_v2 = '15ee27991b18f3cb7f38a1ea8e0ed10168b7ca7924baba4fe08593a8caf29a35'
+        file_hash_v2 = '0f9819faa56cad83eec83244c63a540d7bbda0c71574539067bb8460663200e1'
     else:
         model_name_v2 = 'bc_vit_ti16_224.h5'
         file_hash_v2 = '7ae299f698abc545e21338b129dfbc0ff97ee9b994319e53e8605d34e3ee1f82'
 
     model_path, model_name, file_hash = get_model_path("vit", model_name_v2=model_name_v2,
                                                        file_hash_v2=file_hash_v2)
     model_path = fetch_file(model_path,
```

### Comparing `akida_models-1.4.0/akida_models/unfuse_sepconv_layers.py` & `akida_models-1.5.0/akida_models/unfuse_sepconv_layers.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/utils.py` & `akida_models-1.5.0/akida_models/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -105,41 +105,31 @@
                 current = block_num * block_size
                 if current < total_size:
                     self.progbar.update(current)
                 elif not self.finished:
                     self.progbar.update(self.progbar.target)
                     self.finished = True
 
-        error_msg = "URL fetch failure on {}: {} -- {}"
+        error_msg = "URL fetch failure on {} (attempt number {}). \nReason: {}"
         tries = 3
         try:
             for attempt in range(tries):
                 try:
                     urllib.request.urlretrieve(origin, fpath, DLProgbar())
-                except urllib.error.HTTPError as e:
+                except (urllib.error.HTTPError, urllib.error.URLError, ConnectionResetError) as e:
                     if attempt < tries - 1:
-                        print(f"Error downloading data from {origin} to {fpath} \
-                             (HTTPError), retrying...")
+                        io_utils.print_msg(f"Error downloading data from {origin} to {fpath}, "
+                                           "retrying...")
                         continue
-                    else:
-                        raise Exception(error_msg.format(origin, e.code, e.msg))
-                except urllib.error.URLError as e:
-                    if attempt < tries - 1:
-                        print(f"Error downloading data from {origin} to {fpath} \
-                             (URLError), retrying...")
-                        continue
-                    else:
-                        raise Exception(error_msg.format(origin, e.errno, e.reason))
-                except ConnectionResetError:
-                    if attempt < tries - 1:
-                        print(f"Error downloading data from {origin} to {fpath} \
-                             (ConnectionResetError), retrying...")
-                        continue
-                    else:
-                        raise
+                    raise Exception(error_msg.format(origin, attempt+1, str(e)))
+                else:
+                    io_utils.print_msg("Download complete.")
+                finally:
+                    if attempt != 0:
+                        io_utils.print_msg(f"Download failed {attempt} time(s).")
                 break
         except (Exception, KeyboardInterrupt):
             if os.path.exists(fpath):
                 os.remove(fpath)
             raise
 
     if extract:
```

### Comparing `akida_models-1.4.0/akida_models/utk_face/model_vgg.py` & `akida_models-1.5.0/akida_models/utk_face/model_vgg.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/utk_face/preprocessing.py` & `akida_models-1.5.0/akida_models/utk_face/preprocessing.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models/utk_face/utk_face_train.py` & `akida_models-1.5.0/akida_models/utk_face/utk_face_train.py`

 * *Files identical despite different names*

### Comparing `akida_models-1.4.0/akida_models.egg-info/PKG-INFO` & `akida_models-1.5.0/akida_models.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: akida_models
-Version: 1.4.0
+Version: 1.5.0
 Summary: Akida Models
 Home-page: https://doc.brainchipinc.com
 Author: Kevin Tsiknos
 Author-email: ktsiknos@brainchip.com
 License: Apache 2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.3rdparty
-Requires-Dist: cnn2snn~=2.7.0
+Requires-Dist: cnn2snn~=2.7.2
 Requires-Dist: quantizeml~=0.8.1
 Requires-Dist: scipy
 Requires-Dist: opencv-python
 Requires-Dist: mtcnn
 Requires-Dist: imgaug
 Requires-Dist: trimesh
+Requires-Dist: librosa
 
 # Akida models
 
 This package contains a zoo of TensorFlow/Keras defined models that can be
 quantized and that are compatible for Akida conversion.
```

### Comparing `akida_models-1.4.0/akida_models.egg-info/SOURCES.txt` & `akida_models-1.5.0/akida_models.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,32 +30,34 @@
 akida_models/centernet/centernet_loss.py
 akida_models/centernet/centernet_processing.py
 akida_models/centernet/centernet_train.py
 akida_models/centernet/centernet_utils.py
 akida_models/centernet/model_centernet.py
 akida_models/detection/__init__.py
 akida_models/detection/box_utils.py
+akida_models/detection/data.py
 akida_models/detection/data_augmentation.py
 akida_models/detection/data_utils.py
 akida_models/detection/generate_anchors.py
 akida_models/detection/map_evaluation.py
 akida_models/detection/model_yolo.py
 akida_models/detection/preprocess_data.py
 akida_models/detection/processing.py
 akida_models/detection/yolo_loss.py
 akida_models/detection/yolo_train.py
+akida_models/detection/coco/__init__.py
+akida_models/detection/coco/data.py
 akida_models/detection/voc/__init__.py
 akida_models/detection/voc/data.py
 akida_models/detection/widerface/__init__.py
 akida_models/detection/widerface/data.py
 akida_models/dvs/__init__.py
 akida_models/dvs/dvs_generator.py
 akida_models/dvs/dvs_train.py
-akida_models/dvs/model_convtiny_gesture.py
-akida_models/dvs/model_convtiny_handy.py
+akida_models/dvs/model_convtiny.py
 akida_models/dvs/preprocessing.py
 akida_models/imagenet/__init__.py
 akida_models/imagenet/imagenet_labels2names.py
 akida_models/imagenet/imagenet_train.py
 akida_models/imagenet/imagenet_utils.py
 akida_models/imagenet/load_samples.py
 akida_models/imagenet/model_akidanet.py
@@ -77,11 +79,15 @@
 akida_models/modelnet40/preprocessing.py
 akida_models/portrait128/__init__.py
 akida_models/portrait128/model_akida_unet.py
 akida_models/portrait128/portrait128_train.py
 akida_models/transformers/__init__.py
 akida_models/transformers/model_deit.py
 akida_models/transformers/model_vit.py
+akida_models/urbansound/__init__.py
+akida_models/urbansound/model_vit_urbansound.py
+akida_models/urbansound/preprocessing.py
+akida_models/urbansound/urbansound_train.py
 akida_models/utk_face/__init__.py
 akida_models/utk_face/model_vgg.py
 akida_models/utk_face/preprocessing.py
 akida_models/utk_face/utk_face_train.py
```

### Comparing `akida_models-1.4.0/akida_models.egg-info/entry_points.txt` & `akida_models-1.5.0/akida_models.egg-info/entry_points.txt`

 * *Files 18% similar despite different names*

```diff
@@ -3,9 +3,10 @@
 centernet_train = akida_models.centernet.centernet_train:main
 dvs_train = akida_models.dvs.dvs_train:main
 imagenet_train = akida_models.imagenet.imagenet_train:main
 kws_train = akida_models.kws.kws_train:main
 mnist_train = akida_models.mnist.mnist_train:main
 modelnet40_train = akida_models.modelnet40.modelnet40_train:main
 portrait128_train = akida_models.portrait128.portrait128_train:main
+urbansound_train = akida_models.urbansound.urbansound_train:main
 utk_face_train = akida_models.utk_face.utk_face_train:main
 yolo_train = akida_models.detection.yolo_train:main
```

### Comparing `akida_models-1.4.0/setup.py` & `akida_models-1.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of the README file
 directory = path.abspath(path.dirname(__file__))
 with open(path.join(directory, 'README'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='akida_models',
-      version='1.4.0',
+      version='1.5.0',
       description='Akida Models',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Kevin Tsiknos',
       author_email='ktsiknos@brainchip.com',
       url='https://doc.brainchipinc.com',
       license='Apache 2.0',
@@ -24,13 +24,14 @@
             'kws_train = akida_models.kws.kws_train:main',
             'modelnet40_train = akida_models.modelnet40.modelnet40_train:main',
             'yolo_train = akida_models.detection.yolo_train:main',
             'dvs_train = akida_models.dvs.dvs_train:main',
             'mnist_train = akida_models.mnist.mnist_train:main',
             'imagenet_train = akida_models.imagenet.imagenet_train:main',
             'portrait128_train = akida_models.portrait128.portrait128_train:main',
-            'centernet_train = akida_models.centernet.centernet_train:main'
+            'centernet_train = akida_models.centernet.centernet_train:main',
+            'urbansound_train = akida_models.urbansound.urbansound_train:main'
         ]
       },
-      install_requires=['cnn2snn~=2.7.0', 'quantizeml~=0.8.1', 'scipy', 'opencv-python', 'mtcnn',
-        'imgaug', 'trimesh'],
+      install_requires=['cnn2snn~=2.7.2', 'quantizeml~=0.8.1', 'scipy', 'opencv-python', 'mtcnn',
+        'imgaug', 'trimesh', 'librosa'],
       python_requires='>=3.7')
```


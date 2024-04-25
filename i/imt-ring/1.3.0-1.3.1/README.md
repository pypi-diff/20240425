# Comparing `tmp/imt_ring-1.3.0.tar.gz` & `tmp/imt_ring-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imt_ring-1.3.0.tar", last modified: Wed Apr 24 11:18:18 2024, max compression
+gzip compressed data, was "imt_ring-1.3.1.tar", last modified: Wed Apr 24 21:10:22 2024, max compression
```

## Comparing `imt_ring-1.3.0.tar` & `imt_ring-1.3.1.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.610648 imt_ring-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-24 11:18:18.610648 imt_ring-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-24 11:18:07.000000 imt_ring-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-24 11:18:07.000000 imt_ring-1.3.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-24 11:18:18.610648 imt_ring-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.578647 imt_ring-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.610648 imt_ring-1.3.0/src/imt_ring.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-24 11:18:18.000000 imt_ring-1.3.0/src/imt_ring.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-24 11:18:18.000000 imt_ring-1.3.0/src/imt_ring.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:18:18.000000 imt_ring-1.3.0/src/imt_ring.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-24 11:18:18.000000 imt_ring-1.3.0/src/imt_ring.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 11:18:18.000000 imt_ring-1.3.0/src/imt_ring.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.582647 imt_ring-1.3.0/src/ring/
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algebra.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.582647 imt_ring-1.3.0/src/ring/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13340 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/_random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.586647 imt_ring-1.3.0/src/ring/algorithms/custom_joints/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/custom_joints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/custom_joints/rr_imp_joint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/custom_joints/rr_joint.py
--rw-r--r--   0 runner    (1001) docker     (127)    13680 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/custom_joints/suntay.py
--rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/dynamics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.586647 imt_ring-1.3.0/src/ring/algorithms/generator/
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14952 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/generator/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/generator/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/generator/motion_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/generator/pd_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/generator/randomize.py
--rw-r--r--   0 runner    (1001) docker     (127)    12782 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/generator/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/generator/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    28213 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/jcalc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)    18005 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)    33566 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.586647 imt_ring-1.3.0/src/ring/io/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.590648 imt_ring-1.3.0/src/ring/io/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/branched.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.590648 imt_ring-1.3.0/src/ring/io/examples/exclude/
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/exclude/knee_trans_dof.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/exclude/standard_sys.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/exclude/standard_sys_rr_imp.xml
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/inv_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/knee_flexible_imus.xml
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/spherical_stiff.xml
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/symmetric.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/test_all_1.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/test_all_2.xml
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/test_ang0_pos0.xml
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/test_control.xml
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/test_double_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/test_free.xml
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/test_kinematics.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.590648 imt_ring-1.3.0/src/ring/io/examples/test_morph_system/
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/test_morph_system/four_seg_seg1.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/test_morph_system/four_seg_seg3.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/test_randomize_position.xml
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/test_sensors.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/test_three_seg_seg2.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/test_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.590648 imt_ring-1.3.0/src/ring/io/xml/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/xml/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/xml/from_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/xml/test_from_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/xml/test_to_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/xml/to_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)    12193 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/maths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.590648 imt_ring-1.3.0/src/ring/ml/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/ml/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/ml/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/ml/ml_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/ml/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.590648 imt_ring-1.3.0/src/ring/ml/params/
--rw-r--r--   0 runner    (1001) docker     (127)  9355838 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/ml/params/0x13e3518065c21cd8.pickle
--rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/ml/ringnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/ml/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/ml/training_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.602648 imt_ring-1.3.0/src/ring/rendering/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/rendering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/rendering/base_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/rendering/mujoco_render.py
--rw-r--r--   0 runner    (1001) docker     (127)    10260 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/rendering/vispy_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/rendering/vispy_visuals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.606648 imt_ring-1.3.0/src/ring/sim2real/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/sim2real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/sim2real/sim2real.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/spatial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.606648 imt_ring-1.3.0/src/ring/sys_composer/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/sys_composer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/sys_composer/delete_sys.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/sys_composer/inject_sys.py
--rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/sys_composer/morph_sys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.606648 imt_ring-1.3.0/src/ring/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/utils/batchsize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/utils/colab.py
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/utils/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/utils/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.610648 imt_ring-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_custom_joints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_jcalc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_jit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_maths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_ml_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_motion_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_pd_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_randomize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_rcmg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_sim2real.py
--rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_sys_composer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_train.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:10:22.775596 imt_ring-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-24 21:10:22.775596 imt_ring-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-24 21:10:18.000000 imt_ring-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-24 21:10:18.000000 imt_ring-1.3.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-24 21:10:22.779596 imt_ring-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:10:22.743596 imt_ring-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:10:22.775596 imt_ring-1.3.1/src/imt_ring.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-24 21:10:22.000000 imt_ring-1.3.1/src/imt_ring.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-24 21:10:22.000000 imt_ring-1.3.1/src/imt_ring.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 21:10:22.000000 imt_ring-1.3.1/src/imt_ring.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-24 21:10:22.000000 imt_ring-1.3.1/src/imt_ring.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 21:10:22.000000 imt_ring-1.3.1/src/imt_ring.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:10:22.747596 imt_ring-1.3.1/src/ring/
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/algebra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:10:22.751596 imt_ring-1.3.1/src/ring/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13340 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/algorithms/_random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:10:22.751596 imt_ring-1.3.1/src/ring/algorithms/custom_joints/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/algorithms/custom_joints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/algorithms/custom_joints/rr_imp_joint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/algorithms/custom_joints/rr_joint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13680 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/algorithms/custom_joints/suntay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/algorithms/dynamics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:10:22.751596 imt_ring-1.3.1/src/ring/algorithms/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/algorithms/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14771 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/algorithms/generator/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/algorithms/generator/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/algorithms/generator/motion_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/algorithms/generator/pd_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/algorithms/generator/randomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12782 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/algorithms/generator/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/algorithms/generator/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28213 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/algorithms/jcalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/algorithms/kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18005 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/algorithms/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33530 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:10:22.751596 imt_ring-1.3.1/src/ring/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:10:22.755596 imt_ring-1.3.1/src/ring/io/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/examples/branched.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:10:22.755596 imt_ring-1.3.1/src/ring/io/examples/exclude/
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/examples/exclude/knee_trans_dof.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/examples/exclude/standard_sys.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/examples/exclude/standard_sys_rr_imp.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/examples/inv_pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/examples/knee_flexible_imus.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/examples/spherical_stiff.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/examples/symmetric.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/examples/test_all_1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/examples/test_all_2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/examples/test_ang0_pos0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/examples/test_control.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/examples/test_double_pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/examples/test_free.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/examples/test_kinematics.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:10:22.755596 imt_ring-1.3.1/src/ring/io/examples/test_morph_system/
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/examples/test_morph_system/four_seg_seg1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/examples/test_morph_system/four_seg_seg3.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/examples/test_randomize_position.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/examples/test_sensors.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/examples/test_three_seg_seg2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:10:22.755596 imt_ring-1.3.1/src/ring/io/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/xml/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/xml/from_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/xml/test_from_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/xml/test_to_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/io/xml/to_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12193 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/maths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:10:22.759596 imt_ring-1.3.1/src/ring/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/ml/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/ml/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/ml/ml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/ml/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:10:22.759596 imt_ring-1.3.1/src/ring/ml/params/
+-rw-r--r--   0 runner    (1001) docker     (127)  9355838 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/ml/params/0x13e3518065c21cd8.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/ml/ringnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/ml/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/ml/training_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:10:22.771596 imt_ring-1.3.1/src/ring/rendering/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/rendering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/rendering/base_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/rendering/mujoco_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10260 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/rendering/vispy_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/rendering/vispy_visuals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:10:22.771596 imt_ring-1.3.1/src/ring/sim2real/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/sim2real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/sim2real/sim2real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/spatial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:10:22.771596 imt_ring-1.3.1/src/ring/sys_composer/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/sys_composer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/sys_composer/delete_sys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/sys_composer/inject_sys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/sys_composer/morph_sys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:10:22.771596 imt_ring-1.3.1/src/ring/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/utils/batchsize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/utils/colab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/utils/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/utils/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-04-24 21:10:18.000000 imt_ring-1.3.1/src/ring/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:10:22.775596 imt_ring-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-04-24 21:10:18.000000 imt_ring-1.3.1/tests/test_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-24 21:10:18.000000 imt_ring-1.3.1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-24 21:10:18.000000 imt_ring-1.3.1/tests/test_custom_joints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-24 21:10:18.000000 imt_ring-1.3.1/tests/test_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-04-24 21:10:18.000000 imt_ring-1.3.1/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-24 21:10:18.000000 imt_ring-1.3.1/tests/test_jcalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-24 21:10:18.000000 imt_ring-1.3.1/tests/test_jit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-04-24 21:10:18.000000 imt_ring-1.3.1/tests/test_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-24 21:10:18.000000 imt_ring-1.3.1/tests/test_maths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-24 21:10:18.000000 imt_ring-1.3.1/tests/test_ml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-24 21:10:18.000000 imt_ring-1.3.1/tests/test_motion_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-24 21:10:18.000000 imt_ring-1.3.1/tests/test_pd_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-24 21:10:18.000000 imt_ring-1.3.1/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-24 21:10:18.000000 imt_ring-1.3.1/tests/test_randomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-24 21:10:18.000000 imt_ring-1.3.1/tests/test_rcmg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-24 21:10:18.000000 imt_ring-1.3.1/tests/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-24 21:10:18.000000 imt_ring-1.3.1/tests/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-24 21:10:18.000000 imt_ring-1.3.1/tests/test_sim2real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-24 21:10:18.000000 imt_ring-1.3.1/tests/test_sys_composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-24 21:10:18.000000 imt_ring-1.3.1/tests/test_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-24 21:10:18.000000 imt_ring-1.3.1/tests/test_utils.py
```

### Comparing `imt_ring-1.3.0/PKG-INFO` & `imt_ring-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imt-ring
-Version: 1.3.0
+Version: 1.3.1
 Summary: RING: Recurrent Inertial Graph-based Estimator
 Author-email: Simon Bachhuber <simon.bachhuber@fau.de>
 Project-URL: Homepage, https://github.com/SimiPixel/ring
 Project-URL: Issues, https://github.com/SimiPixel/ring/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `imt_ring-1.3.0/pyproject.toml` & `imt_ring-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "imt-ring"
-version = "1.3.0"
+version = "1.3.1"
 authors = [
   { name="Simon Bachhuber", email="simon.bachhuber@fau.de" },
 ]
 description = "RING: Recurrent Inertial Graph-based Estimator"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `imt_ring-1.3.0/readme.md` & `imt_ring-1.3.1/readme.md`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/imt_ring.egg-info/PKG-INFO` & `imt_ring-1.3.1/src/imt_ring.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imt-ring
-Version: 1.3.0
+Version: 1.3.1
 Summary: RING: Recurrent Inertial Graph-based Estimator
 Author-email: Simon Bachhuber <simon.bachhuber@fau.de>
 Project-URL: Homepage, https://github.com/SimiPixel/ring
 Project-URL: Issues, https://github.com/SimiPixel/ring/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `imt_ring-1.3.0/src/imt_ring.egg-info/SOURCES.txt` & `imt_ring-1.3.1/src/imt_ring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/__init__.py` & `imt_ring-1.3.1/src/ring/__init__.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/algebra.py` & `imt_ring-1.3.1/src/ring/algebra.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/algorithms/__init__.py` & `imt_ring-1.3.1/src/ring/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/algorithms/_random.py` & `imt_ring-1.3.1/src/ring/algorithms/_random.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/algorithms/custom_joints/rr_imp_joint.py` & `imt_ring-1.3.1/src/ring/algorithms/custom_joints/rr_imp_joint.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/algorithms/custom_joints/rr_joint.py` & `imt_ring-1.3.1/src/ring/algorithms/custom_joints/rr_joint.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/algorithms/custom_joints/suntay.py` & `imt_ring-1.3.1/src/ring/algorithms/custom_joints/suntay.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/algorithms/dynamics.py` & `imt_ring-1.3.1/src/ring/algorithms/dynamics.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/algorithms/generator/__init__.py` & `imt_ring-1.3.1/src/ring/algorithms/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/algorithms/generator/base.py` & `imt_ring-1.3.1/src/ring/algorithms/generator/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from functools import partial
 from typing import Callable, Optional, Sequence
 import warnings
 
 import jax
 import jax.numpy as jnp
+import tree_utils
+
 from ring import base
 from ring import utils
 from ring.algorithms import jcalc
 from ring.algorithms import kinematics
 from ring.algorithms.generator import batch
 from ring.algorithms.generator import motion_artifacts
 from ring.algorithms.generator import randomize
 from ring.algorithms.generator import transforms
 from ring.algorithms.generator import types
-import tree_utils
 
 
 class RCMG:
     def __init__(
         self,
         sys: base.System | list[base.System],
         config: jcalc.MotionConfig | list[jcalc.MotionConfig] = jcalc.MotionConfig(),
@@ -104,54 +105,47 @@
         else:
             for _sys in sys:
                 for _config in config:
                     self.gens.append(
                         partial_build_gen(sys=_sys, config=_config, sys_ml=sys_ml)
                     )
 
-    def _to_data(self, sizes, seed, jit):
-        return batch.batch_generators_eager_to_list(
-            self.gens, sizes, seed=seed, jit=jit
-        )
+    def _to_data(self, sizes, seed):
+        return batch.batch_generators_eager_to_list(self.gens, sizes, seed=seed)
 
-    def to_list(self, sizes: int | list[int] = 1, seed: int = 1, jit: bool = False):
-        return self._to_data(sizes, seed, jit)
+    def to_list(self, sizes: int | list[int] = 1, seed: int = 1):
+        return self._to_data(sizes, seed)
 
     def to_pickle(
         self,
         path: str,
         sizes: int | list[int] = 1,
         seed: int = 1,
-        jit: bool = False,
         overwrite: bool = True,
     ) -> None:
-        data = tree_utils.tree_batch(self._to_data(sizes, seed, jit))
+        data = tree_utils.tree_batch(self._to_data(sizes, seed))
         utils.pickle_save(data, path, overwrite=overwrite)
 
     def to_hdf5(
         self,
         path: str,
         sizes: int | list[int] = 1,
         seed: int = 1,
-        jit: bool = False,
         overwrite: bool = True,
     ) -> None:
-        data = tree_utils.tree_batch(self._to_data(sizes, seed, jit))
+        data = tree_utils.tree_batch(self._to_data(sizes, seed))
         utils.hdf5_save(path, data, overwrite=overwrite)
 
     def to_eager_gen(
         self,
         batchsize: int = 1,
         sizes: int | list[int] = 1,
         seed: int = 1,
-        jit: bool = False,
     ) -> types.BatchedGenerator:
-        return batch.batch_generators_eager(
-            self.gens, sizes, batchsize, seed=seed, jit=jit
-        )
+        return batch.batch_generators_eager(self.gens, sizes, batchsize, seed=seed)
 
     def to_lazy_gen(
         self, sizes: int | list[int] = 1, jit: bool = True
     ) -> types.BatchedGenerator:
         return batch.batch_generators_lazy(self.gens, sizes, jit=jit)
 
     @staticmethod
```

### Comparing `imt_ring-1.3.0/src/ring/algorithms/generator/batch.py` & `imt_ring-1.3.1/src/ring/algorithms/generator/batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 import random
 from typing import Optional
 import warnings
 
 import jax
 import jax.numpy as jnp
 import numpy as np
-from ring import utils
-from ring.algorithms.generator import types
 from tqdm import tqdm
 import tree_utils
 from tree_utils import tree_batch
 
+from ring import utils
+from ring.algorithms.generator import types
+
 
 def _build_batch_matrix(batchsizes: list[int]) -> jax.Array:
     arr = []
     for i, l in enumerate(batchsizes):
         arr += [i] * l
     return jnp.array(arr)
 
@@ -57,31 +58,53 @@
         # merge pmap and vmap axis
         data = utils.merge_batchsize(data, pmap, vmap)
         return data
 
     return generator
 
 
+def _number_of_executions_required(size: int) -> int:
+    vmap_threshold = 128
+    _, vmap = utils.distribute_batchsize(size)
+
+    primes = iter(utils.primes(vmap))
+    n_calls = 1
+    while vmap > vmap_threshold:
+        prime = next(primes)
+        n_calls *= prime
+        vmap /= prime
+
+    return n_calls
+
+
 def batch_generators_eager_to_list(
     generators: types.Generator | list[types.Generator],
     sizes: int | list[int],
     seed: int = 1,
-    jit: bool = True,
 ) -> list[tree_utils.PyTree]:
     "Returns list of unbatched sequences as numpy arrays."
     generators, sizes = _process_sizes_batchsizes_generators(generators, sizes)
 
     key = jax.random.PRNGKey(seed)
     data = []
     for gen, size in tqdm(zip(generators, sizes), desc="eager data generation"):
-        key, consume = jax.random.split(key)
-        sample = batch_generators_lazy(gen, size, jit=jit)(consume)
-        # converts also to numpy
-        sample = jax.device_get(sample)
-        data.extend([jax.tree_map(lambda a: a[i], sample) for i in range(size)])
+
+        n_calls = _number_of_executions_required(size)
+        # decrease size by n_calls times
+        size = int(size / n_calls)
+        jit = True if n_calls > 1 else False
+        gen_jit = batch_generators_lazy(gen, size, jit=jit)
+
+        for _ in range(n_calls):
+            key, consume = jax.random.split(key)
+            sample = gen_jit(consume)
+            # converts also to numpy
+            sample = jax.device_get(sample)
+            data.extend([jax.tree_map(lambda a: a[i], sample) for i in range(size)])
+
     return data
 
 
 def _is_nan(ele: tree_utils.PyTree, i: int, verbose: bool = False):
     isnan = np.any([np.any(np.isnan(arr)) for arr in jax.tree_util.tree_leaves(ele)])
     if isnan:
         X, y = ele
@@ -239,20 +262,19 @@
 def batch_generators_eager(
     generators: types.Generator | list[types.Generator],
     sizes: int | list[int],
     batchsize: int,
     shuffle: bool = True,
     drop_last: bool = True,
     seed: int = 1,
-    jit: bool = True,
 ) -> types.BatchedGenerator:
     """Eagerly create a large precomputed generator by calling multiple generators
     and stacking their output."""
 
-    data = batch_generators_eager_to_list(generators, sizes, seed=seed, jit=jit)
+    data = batch_generators_eager_to_list(generators, sizes, seed=seed)
     return batched_generator_from_list(data, batchsize, shuffle, drop_last)
 
 
 def _process_sizes_batchsizes_generators(
     generators: types.Generator | list[types.Generator],
     batchsizes_or_sizes: int | list[int],
 ) -> tuple[list, list]:
@@ -266,15 +288,15 @@
         list_sizes = len(generators) * [batchsizes_or_sizes // len(generators)]
     else:
         list_sizes = batchsizes_or_sizes
         assert 0 not in list_sizes
 
     assert len(generators) == len(list_sizes)
 
-    _WARN_SIZE = 4096
+    _WARN_SIZE = 1e6  # disable this warning
     for size in list_sizes:
         if size >= _WARN_SIZE:
             warnings.warn(
                 f"A generator will be called with a large batchsize of {size} "
                 f"(warn limit is {_WARN_SIZE}). The generator sizes are {list_sizes}."
             )
             break
```

### Comparing `imt_ring-1.3.0/src/ring/algorithms/generator/motion_artifacts.py` & `imt_ring-1.3.1/src/ring/algorithms/generator/motion_artifacts.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/algorithms/generator/pd_control.py` & `imt_ring-1.3.1/src/ring/algorithms/generator/pd_control.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/algorithms/generator/randomize.py` & `imt_ring-1.3.1/src/ring/algorithms/generator/randomize.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/algorithms/generator/transforms.py` & `imt_ring-1.3.1/src/ring/algorithms/generator/transforms.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/algorithms/generator/types.py` & `imt_ring-1.3.1/src/ring/algorithms/generator/types.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/algorithms/jcalc.py` & `imt_ring-1.3.1/src/ring/algorithms/jcalc.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/algorithms/kinematics.py` & `imt_ring-1.3.1/src/ring/algorithms/kinematics.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/algorithms/sensors.py` & `imt_ring-1.3.1/src/ring/algorithms/sensors.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/base.py` & `imt_ring-1.3.1/src/ring/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,23 +95,23 @@
 
     def repeat(self, repeats, axis=0):
         return tree_map(lambda x: jnp.repeat(x, repeats, axis), self)
 
     def ndim(self):
         return tu.tree_ndim(self)
 
-    def shape(self, axis=0) -> int:
-        return tu.tree_shape(self, axis)
-
-    def __len__(self) -> int:
-        Bs = tree_map(lambda arr: arr.shape[0], self)
+    def shape(self, axis: int = 0) -> int:
+        Bs = tree_map(lambda arr: arr.shape[axis], self)
         Bs = set(jax.tree_util.tree_flatten(Bs)[0])
         assert len(Bs) == 1
         return list(Bs)[0]
 
+    def __len__(self) -> int:
+        return self.shape(axis=0)
+
 
 @struct.dataclass
 class Transform(_Base):
     """Represents the Transformation from Plücker A to Plücker B,
     where B is located relative to A at `pos` in frame A and `rot` is the
     relative quaternion from A to B."""
 
@@ -681,22 +681,21 @@
             self, xs, camera, show_pbar, backend, render_every_nth, **scene_kwargs
         )
 
     def render_prediction(
         self,
         xs: Transform | list[Transform],
         yhat: dict | jax.Array | np.ndarray,
-        stepframe: int = 1,
         # by default we don't predict the global rotation
         transparent_segment_to_root: bool = True,
         **kwargs,
     ):
         "`xs` matches `sys`. `yhat` matches `sys_noimu`. `yhat` are child-to-parent."
         return ring.rendering.render_prediction(
-            self, xs, yhat, stepframe, transparent_segment_to_root, **kwargs
+            self, xs, yhat, transparent_segment_to_root, **kwargs
         )
 
     def delete_system(self, link_name: str | list[str], strict: bool = True):
         "Cut subsystem starting at `link_name` (inclusive) from tree."
         return ring.sys_composer.delete_subsystem(self, link_name, strict)
 
     def make_sys_noimu(self, imu_link_names: Optional[list[str]] = None):
```

### Comparing `imt_ring-1.3.0/src/ring/io/examples/branched.xml` & `imt_ring-1.3.1/src/ring/io/examples/branched.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/io/examples/exclude/knee_trans_dof.xml` & `imt_ring-1.3.1/src/ring/io/examples/exclude/knee_trans_dof.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/io/examples/exclude/standard_sys.xml` & `imt_ring-1.3.1/src/ring/io/examples/exclude/standard_sys.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/io/examples/exclude/standard_sys_rr_imp.xml` & `imt_ring-1.3.1/src/ring/io/examples/exclude/standard_sys_rr_imp.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/io/examples/inv_pendulum.xml` & `imt_ring-1.3.1/src/ring/io/examples/inv_pendulum.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/io/examples/knee_flexible_imus.xml` & `imt_ring-1.3.1/src/ring/io/examples/knee_flexible_imus.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/io/examples/test_all_1.xml` & `imt_ring-1.3.1/src/ring/io/examples/test_all_1.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/io/examples/test_all_2.xml` & `imt_ring-1.3.1/src/ring/io/examples/test_all_2.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/io/examples/test_control.xml` & `imt_ring-1.3.1/src/ring/io/examples/test_control.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/io/examples/test_double_pendulum.xml` & `imt_ring-1.3.1/src/ring/io/examples/test_double_pendulum.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/io/examples/test_kinematics.xml` & `imt_ring-1.3.1/src/ring/io/examples/test_kinematics.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/io/examples/test_morph_system/four_seg_seg1.xml` & `imt_ring-1.3.1/src/ring/io/examples/test_morph_system/four_seg_seg1.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/io/examples/test_morph_system/four_seg_seg3.xml` & `imt_ring-1.3.1/src/ring/io/examples/test_morph_system/four_seg_seg3.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/io/examples/test_randomize_position.xml` & `imt_ring-1.3.1/src/ring/io/examples/test_randomize_position.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/io/examples/test_three_seg_seg2.xml` & `imt_ring-1.3.1/src/ring/io/examples/test_three_seg_seg2.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/io/examples.py` & `imt_ring-1.3.1/src/ring/io/examples.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/io/xml/abstract.py` & `imt_ring-1.3.1/src/ring/io/xml/abstract.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/io/xml/from_xml.py` & `imt_ring-1.3.1/src/ring/io/xml/from_xml.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/io/xml/test_from_xml.py` & `imt_ring-1.3.1/src/ring/io/xml/test_from_xml.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/io/xml/test_to_xml.py` & `imt_ring-1.3.1/src/ring/io/xml/test_to_xml.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/io/xml/to_xml.py` & `imt_ring-1.3.1/src/ring/io/xml/to_xml.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/maths.py` & `imt_ring-1.3.1/src/ring/maths.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/ml/__init__.py` & `imt_ring-1.3.1/src/ring/ml/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from .base import AbstractFilter
 from .ml_utils import on_cluster
 from .ml_utils import unique_id
 from .optimizer import make_optimizer
 from .ringnet import RING
 from .train import train_fn
 
+_lpf_cutoff_freq = 10.0
+
 
 def RING_ICML24(params=None, eval: bool = True, **kwargs):
     """Create the RING network used in the icml24 paper.
 
     X[..., :3]  = acc
     X[..., 3:6] = gyr
     X[..., 6:9] = jointaxis
@@ -25,15 +27,15 @@
 
     if params is None:
         params = Path(__file__).parent.joinpath("params/0x13e3518065c21cd8.pickle")
 
     ringnet = RING(params=params, **kwargs)  # noqa: F811
     ringnet = base.ScaleX_FilterWrapper(ringnet)
     if eval:
-        ringnet = base.LPF_FilterWrapper(ringnet, 10.0, samp_freq=None)
+        ringnet = base.LPF_FilterWrapper(ringnet, _lpf_cutoff_freq, samp_freq=None)
     ringnet = base.GroundTruthHeading_FilterWrapper(ringnet)
     return ringnet
 
 
 def RNNO(
     output_dim: int,
     return_quats: bool = False,
@@ -51,11 +53,11 @@
         link_output_normalize=False,
         link_output_dim=output_dim,
         **kwargs,
     )
     ringnet = base.NoGraph_FilterWrapper(ringnet, quat_normalize=return_quats)
     ringnet = base.ScaleX_FilterWrapper(ringnet)
     if eval and return_quats:
-        ringnet = base.LPF_FilterWrapper(ringnet, 10.0, samp_freq=None)
+        ringnet = base.LPF_FilterWrapper(ringnet, _lpf_cutoff_freq, samp_freq=None)
     if return_quats:
         ringnet = base.GroundTruthHeading_FilterWrapper(ringnet)
     return ringnet
```

### Comparing `imt_ring-1.3.0/src/ring/ml/base.py` & `imt_ring-1.3.1/src/ring/ml/base.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/ml/callbacks.py` & `imt_ring-1.3.1/src/ring/ml/callbacks.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/ml/ml_utils.py` & `imt_ring-1.3.1/src/ring/ml/ml_utils.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/ml/optimizer.py` & `imt_ring-1.3.1/src/ring/ml/optimizer.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/ml/params/0x13e3518065c21cd8.pickle` & `imt_ring-1.3.1/src/ring/ml/params/0x13e3518065c21cd8.pickle`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/ml/ringnet.py` & `imt_ring-1.3.1/src/ring/ml/ringnet.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/ml/train.py` & `imt_ring-1.3.1/src/ring/ml/train.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/ml/training_loop.py` & `imt_ring-1.3.1/src/ring/ml/training_loop.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/rendering/base_render.py` & `imt_ring-1.3.1/src/ring/rendering/base_render.py`

 * *Files 6% similar despite different names*

```diff
@@ -132,20 +132,23 @@
     return frames
 
 
 def render_prediction(
     sys: base.System,
     xs: base.Transform | list[base.Transform],
     yhat: dict | jax.Array | np.ndarray,
-    stepframe: int = 1,
     # by default we don't predict the global rotation
     transparent_segment_to_root: bool = True,
     **kwargs,
 ):
     "`xs` matches `sys`. `yhat` matches `sys_noimu`. `yhat` are child-to-parent."
+
+    offset_truth = kwargs.pop("offset_truth", [0, 0, 0])
+    offset_pred = kwargs.pop("offset_pred", [0, 0, 0])
+
     if isinstance(xs, list):
         # list -> batched Transform
         xs = xs[0].batch(*xs[1:])
 
     sys_noimu, _ = sys.make_sys_noimu()
 
     if isinstance(yhat, (np.ndarray, jax.Array)):
@@ -176,41 +179,43 @@
     # after transpose shape is (n_timesteps, n_links, ...)
     transform2hat = transform2hat[0].batch(*transform2hat[1:]).transpose((1, 0, 2))
 
     xshat = sim2real.zip_xs(sys_noimu, transform1, transform2hat)
 
     # swap time axis, and link axis
     xs, xshat = xs.transpose((1, 0, 2)), xshat.transpose((1, 0, 2))
+
+    add_offset = lambda x, offset: algebra.transform_mul(
+        x, base.Transform.create(pos=jnp.array(offset, dtype=jnp.float32))
+    )
+
     # create mapping from `name` -> Transform
     xs_dict = dict(
         zip(
             ["hat_" + name for name in sys_noimu.link_names],
-            [xshat[i] for i in range(sys_noimu.num_links())],
+            [add_offset(xshat[i], offset_pred) for i in range(sys_noimu.num_links())],
         )
     )
     xs_dict.update(
         dict(
             zip(
                 sys.link_names,
-                [xs[i] for i in range(sys.num_links())],
+                [add_offset(xs[i], offset_truth) for i in range(sys.num_links())],
             )
         )
     )
 
     sys_render = _sys_render(sys, transparent_segment_to_root)
     xs_render = []
     for name in sys_render.link_names:
         xs_render.append(xs_dict[name])
     xs_render = xs_render[0].batch(*xs_render[1:])
     xs_render = xs_render.transpose((1, 0, 2))
-    N = xs_render.shape()
-    xs_render = [xs_render[t] for t in range(0, N, stepframe)]
 
     frames = render(sys_render, xs_render, **kwargs)
-
     return frames
 
 
 def _color_to_rgba(geom: base.Geometry) -> base.Geometry:
     if geom.color is None:
         new_color = _rgbas["self"]
     elif isinstance(geom.color, tuple):
```

### Comparing `imt_ring-1.3.0/src/ring/rendering/mujoco_render.py` & `imt_ring-1.3.1/src/ring/rendering/mujoco_render.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/rendering/vispy_render.py` & `imt_ring-1.3.1/src/ring/rendering/vispy_render.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/rendering/vispy_visuals.py` & `imt_ring-1.3.1/src/ring/rendering/vispy_visuals.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/sim2real/sim2real.py` & `imt_ring-1.3.1/src/ring/sim2real/sim2real.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/spatial.py` & `imt_ring-1.3.1/src/ring/spatial.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/sys_composer/delete_sys.py` & `imt_ring-1.3.1/src/ring/sys_composer/delete_sys.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/sys_composer/inject_sys.py` & `imt_ring-1.3.1/src/ring/sys_composer/inject_sys.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/sys_composer/morph_sys.py` & `imt_ring-1.3.1/src/ring/sys_composer/morph_sys.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/utils/__init__.py` & `imt_ring-1.3.1/src/ring/utils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,11 +11,12 @@
 from .normalizer import Normalizer
 from .path import parse_path
 from .utils import dict_to_nested
 from .utils import dict_union
 from .utils import import_lib
 from .utils import pickle_load
 from .utils import pickle_save
+from .utils import primes
 from .utils import pytree_deepcopy
 from .utils import sys_compare
 from .utils import to_list
 from .utils import tree_equal
```

### Comparing `imt_ring-1.3.0/src/ring/utils/batchsize.py` & `imt_ring-1.3.1/src/ring/utils/batchsize.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/utils/colab.py` & `imt_ring-1.3.1/src/ring/utils/colab.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/utils/hdf5.py` & `imt_ring-1.3.1/src/ring/utils/hdf5.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/utils/normalizer.py` & `imt_ring-1.3.1/src/ring/utils/normalizer.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/utils/path.py` & `imt_ring-1.3.1/src/ring/utils/path.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/src/ring/utils/utils.py` & `imt_ring-1.3.1/src/ring/utils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -155,7 +155,21 @@
 def pickle_load(
     path,
 ):
     path = parse_path(path, extension="pickle", require_is_file=True)
     with open(path, "rb") as file:
         obj = pickle.load(file)
     return obj
+
+
+def primes(n: int) -> list[int]:
+    "Primefactor decomposition in ascending order."
+    primfac = []
+    d = 2
+    while d * d <= n:
+        while (n % d) == 0:
+            primfac.append(d)  # supposing you want multiple factors repeated
+            n //= d
+        d += 1
+    if n > 1:
+        primfac.append(n)
+    return primfac
```

### Comparing `imt_ring-1.3.0/tests/test_algebra.py` & `imt_ring-1.3.1/tests/test_algebra.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/tests/test_base.py` & `imt_ring-1.3.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/tests/test_custom_joints.py` & `imt_ring-1.3.1/tests/test_custom_joints.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/tests/test_dynamics.py` & `imt_ring-1.3.1/tests/test_dynamics.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/tests/test_generator.py` & `imt_ring-1.3.1/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/tests/test_jcalc.py` & `imt_ring-1.3.1/tests/test_jcalc.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/tests/test_jit.py` & `imt_ring-1.3.1/tests/test_jit.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/tests/test_kinematics.py` & `imt_ring-1.3.1/tests/test_kinematics.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/tests/test_maths.py` & `imt_ring-1.3.1/tests/test_maths.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/tests/test_ml_utils.py` & `imt_ring-1.3.1/tests/test_ml_utils.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/tests/test_motion_artifacts.py` & `imt_ring-1.3.1/tests/test_motion_artifacts.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/tests/test_pd_control.py` & `imt_ring-1.3.1/tests/test_pd_control.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/tests/test_random.py` & `imt_ring-1.3.1/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/tests/test_randomize.py` & `imt_ring-1.3.1/tests/test_randomize.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/tests/test_rcmg.py` & `imt_ring-1.3.1/tests/test_rcmg.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/tests/test_render.py` & `imt_ring-1.3.1/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/tests/test_sensors.py` & `imt_ring-1.3.1/tests/test_sensors.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/tests/test_sim2real.py` & `imt_ring-1.3.1/tests/test_sim2real.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/tests/test_sys_composer.py` & `imt_ring-1.3.1/tests/test_sys_composer.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/tests/test_train.py` & `imt_ring-1.3.1/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.0/tests/test_utils.py` & `imt_ring-1.3.1/tests/test_utils.py`

 * *Files identical despite different names*


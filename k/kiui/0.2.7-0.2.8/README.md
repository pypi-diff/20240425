# Comparing `tmp/kiui-0.2.7.tar.gz` & `tmp/kiui-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiui-0.2.7.tar", last modified: Thu Mar 28 13:02:37 2024, max compression
+gzip compressed data, was "kiui-0.2.8.tar", last modified: Thu Apr 25 08:30:13 2024, max compression
```

## Comparing `kiui-0.2.7.tar` & `kiui-0.2.8.tar`

### file list

```diff
@@ -1,91 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:37.474652 kiui-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-28 13:02:33.000000 kiui-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-28 13:02:33.000000 kiui-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-03-28 13:02:37.474652 kiui-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-03-28 13:02:33.000000 kiui-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:37.462652 kiui-0.2.7/kiui/
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:37.458652 kiui-0.2.7/kiui/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:37.466652 kiui-0.2.7/kiui/assets/blender_lights/
--rw-r--r--   0 runner    (1001) docker     (127)   213545 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/assets/blender_lights/city.exr
--rw-r--r--   0 runner    (1001) docker     (127)   270418 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/assets/blender_lights/courtyard.exr
--rw-r--r--   0 runner    (1001) docker     (127)   513764 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/assets/blender_lights/forest.exr
--rw-r--r--   0 runner    (1001) docker     (127)   202262 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/assets/blender_lights/interior.exr
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/assets/blender_lights/license.txt
--rw-r--r--   0 runner    (1001) docker     (127)   148071 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/assets/blender_lights/night.exr
--rw-r--r--   0 runner    (1001) docker     (127)    97867 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/assets/blender_lights/studio.exr
--rw-r--r--   0 runner    (1001) docker     (127)   260454 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/assets/blender_lights/sunrise.exr
--rw-r--r--   0 runner    (1001) docker     (127)   170385 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/assets/blender_lights/sunset.exr
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:37.466652 kiui-0.2.7/kiui/assets/lights/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/assets/lights/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   524288 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/assets/lights/bsdf_256_256.bin
--rw-r--r--   0 runner    (1001) docker     (127)  1109840 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/assets/lights/mud_road_puresky_1k.hdr
--rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/cam.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:37.470652 kiui-0.2.7/kiui/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/cli/aes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/cli/bg.py
--rw-r--r--   0 runner    (1001) docker     (127)    14965 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/cli/blender_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/cli/blip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/cli/clip_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/cli/clip_sim_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/cli/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/cli/depth_midas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/cli/depth_zoe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/cli/dircmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/cli/hed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/cli/lock_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:37.470652 kiui-0.2.7/kiui/cli/openpose/
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/cli/openpose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13140 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/cli/openpose/body.py
--rw-r--r--   0 runner    (1001) docker     (127)    13806 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/cli/openpose/face.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/cli/openpose/hand.py
--rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/cli/openpose/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/cli/openpose/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/cli/pose.py
--rw-r--r--   0 runner    (1001) docker     (127)    28442 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/cli/remesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/cli/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/env.py
--rw-r--r--   0 runner    (1001) docker     (127)    12478 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/grid_put.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:37.474652 kiui-0.2.7/kiui/gridencoder/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/gridencoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/gridencoder/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     9414 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/gridencoder/grid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:37.474652 kiui-0.2.7/kiui/gridencoder/src/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/gridencoder/src/bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    27116 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/gridencoder/src/gridencoder.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/gridencoder/src/gridencoder.h
--rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/lpips.py
--rw-r--r--   0 runner    (1001) docker     (127)    35463 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     9885 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/mesh_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:37.474652 kiui-0.2.7/kiui/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/nn/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/nn/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/nn/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/nn/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/nn/unet_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    16719 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/nn/unet_2d_cond.py
--rw-r--r--   0 runner    (1001) docker     (127)    16735 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/nn/unet_3d_cond.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/nn/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14104 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/nn/vae_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/nn/vae_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/op.py
--rw-r--r--   0 runner    (1001) docker     (127)    35293 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/poser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (127)    20465 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/render.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/render_viser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/sh.py
--rw-r--r--   0 runner    (1001) docker     (127)    21178 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/sr.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-03-28 13:02:33.000000 kiui-0.2.7/kiui/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:37.462652 kiui-0.2.7/kiui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-03-28 13:02:37.000000 kiui-0.2.7/kiui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-28 13:02:37.000000 kiui-0.2.7/kiui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 13:02:37.000000 kiui-0.2.7/kiui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-28 13:02:37.000000 kiui-0.2.7/kiui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-28 13:02:37.000000 kiui-0.2.7/kiui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-28 13:02:37.000000 kiui-0.2.7/kiui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 13:02:37.474652 kiui-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-28 13:02:33.000000 kiui-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:30:13.574327 kiui-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 08:30:09.000000 kiui-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-25 08:30:09.000000 kiui-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-25 08:30:13.574327 kiui-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-25 08:30:09.000000 kiui-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:30:13.558327 kiui-0.2.8/kiui/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:30:13.554327 kiui-0.2.8/kiui/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:30:13.562327 kiui-0.2.8/kiui/assets/blender_lights/
+-rw-r--r--   0 runner    (1001) docker     (127)   213545 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/assets/blender_lights/city.exr
+-rw-r--r--   0 runner    (1001) docker     (127)   270418 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/assets/blender_lights/courtyard.exr
+-rw-r--r--   0 runner    (1001) docker     (127)   513764 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/assets/blender_lights/forest.exr
+-rw-r--r--   0 runner    (1001) docker     (127)   202262 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/assets/blender_lights/interior.exr
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/assets/blender_lights/license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   148071 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/assets/blender_lights/night.exr
+-rw-r--r--   0 runner    (1001) docker     (127)    97867 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/assets/blender_lights/studio.exr
+-rw-r--r--   0 runner    (1001) docker     (127)   260454 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/assets/blender_lights/sunrise.exr
+-rw-r--r--   0 runner    (1001) docker     (127)   170385 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/assets/blender_lights/sunset.exr
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:30:13.566327 kiui-0.2.8/kiui/assets/lights/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/assets/lights/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   524288 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/assets/lights/bsdf_256_256.bin
+-rw-r--r--   0 runner    (1001) docker     (127)  1109840 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/assets/lights/mud_road_puresky_1k.hdr
+-rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cam.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:30:13.570327 kiui-0.2.8/kiui/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cli/aes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cli/bg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cli/blender_qremesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15121 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cli/blender_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cli/blip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cli/clip_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cli/clip_sim_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cli/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cli/convert_fp16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cli/depth_midas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cli/depth_zoe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cli/dircmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cli/hed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cli/lock_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:30:13.570327 kiui-0.2.8/kiui/cli/openpose/
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cli/openpose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13140 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cli/openpose/body.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13806 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cli/openpose/face.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cli/openpose/hand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cli/openpose/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cli/openpose/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cli/pose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28522 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cli/remesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/cli/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12478 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/grid_put.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:30:13.570327 kiui-0.2.8/kiui/gridencoder/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/gridencoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/gridencoder/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9414 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/gridencoder/grid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:30:13.570327 kiui-0.2.8/kiui/gridencoder/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/gridencoder/src/bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    27116 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/gridencoder/src/gridencoder.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/gridencoder/src/gridencoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/lpips.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35877 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9885 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/mesh_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:30:13.574327 kiui-0.2.8/kiui/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/nn/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/nn/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/nn/perciever.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/nn/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/nn/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/nn/unet_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16719 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/nn/unet_2d_cond.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16735 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/nn/unet_3d_cond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/nn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14105 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/nn/vae_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/nn/vae_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/op.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35293 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/poser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20781 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/render_viser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/sh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21178 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/sr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-04-25 08:30:09.000000 kiui-0.2.8/kiui/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:30:13.558327 kiui-0.2.8/kiui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-25 08:30:13.000000 kiui-0.2.8/kiui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-25 08:30:13.000000 kiui-0.2.8/kiui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:30:13.000000 kiui-0.2.8/kiui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-25 08:30:13.000000 kiui-0.2.8/kiui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-25 08:30:13.000000 kiui-0.2.8/kiui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 08:30:13.000000 kiui-0.2.8/kiui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 08:30:13.574327 kiui-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-25 08:30:09.000000 kiui-0.2.8/setup.py
```

### Comparing `kiui-0.2.7/LICENSE` & `kiui-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/PKG-INFO` & `kiui-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiui
-Version: 0.2.7
+Version: 0.2.8
 Summary: A toolkit for 3D vision
 Home-page: https://github.com/ashawkey/kiuikit
 Author: kiui
 Author-email: ashawkey1999@gmail.com
 Keywords: utility
 Classifier: Programming Language :: Python :: 3 
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kiui Version: 0.2.7 Summary: A toolkit for 3D
+Metadata-Version: 2.1 Name: kiui Version: 0.2.8 Summary: A toolkit for 3D
 vision Home-page: https://github.com/ashawkey/kiuikit Author: kiui Author-
 email: ashawkey1999@gmail.com Keywords: utility Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
 full License-File: LICENSE
           [kiuikit_logo]KKiiuuiikkiitt pip install kiui   •   _D_o_c_u_m_e_n_t_a_t_i_o_n
 A toolkit for computer vision (especially 3D vision) tasks. **Features**: *
 Collection of *maintained, reusable and trustworthy* code snippets. * Always
```

### Comparing `kiui-0.2.7/README.md` & `kiui-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/__init__.py` & `kiui-0.2.8/kiui/__init__.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/assets/blender_lights/city.exr` & `kiui-0.2.8/kiui/assets/blender_lights/city.exr`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/assets/blender_lights/courtyard.exr` & `kiui-0.2.8/kiui/assets/blender_lights/courtyard.exr`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/assets/blender_lights/forest.exr` & `kiui-0.2.8/kiui/assets/blender_lights/forest.exr`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/assets/blender_lights/interior.exr` & `kiui-0.2.8/kiui/assets/blender_lights/interior.exr`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/assets/blender_lights/night.exr` & `kiui-0.2.8/kiui/assets/blender_lights/night.exr`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/assets/blender_lights/studio.exr` & `kiui-0.2.8/kiui/assets/blender_lights/studio.exr`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/assets/blender_lights/sunrise.exr` & `kiui-0.2.8/kiui/assets/blender_lights/sunrise.exr`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/assets/blender_lights/sunset.exr` & `kiui-0.2.8/kiui/assets/blender_lights/sunset.exr`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/assets/lights/bsdf_256_256.bin` & `kiui-0.2.8/kiui/assets/lights/bsdf_256_256.bin`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/assets/lights/mud_road_puresky_1k.hdr` & `kiui-0.2.8/kiui/assets/lights/mud_road_puresky_1k.hdr`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/cam.py` & `kiui-0.2.8/kiui/cam.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/cli/aes.py` & `kiui-0.2.8/kiui/cli/aes.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/cli/bg.py` & `kiui-0.2.8/kiui/cli/bg.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/cli/blender_render.py` & `kiui-0.2.8/kiui/cli/blender_render.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     render_layers = nodes.new("CompositorNodeRLayers")
 
     ## depth
     if args.depth:
         bpy.context.view_layer.use_pass_z = True
         node_depth = nodes.new(type="CompositorNodeOutputFile")
         node_depth.label = "Depth Output"
-        node_depth.base_path = ""
+        node_depth.base_path = "/" # use absolute save path
         node_depth.file_slots[0].use_node_format = True
         node_depth.format.file_format = "OPEN_EXR"
         node_depth.format.color_depth = "16"
         links.new(render_layers.outputs["Depth"], node_depth.inputs[0])
 
         refs['node_depth'] = node_depth
 
@@ -124,15 +124,15 @@
         links.new(render_layers.outputs["Normal"], node_normal_scale.inputs[1])
         node_normal_bias = nodes.new(type="CompositorNodeMixRGB")
         node_normal_bias.blend_type = "ADD"
         node_normal_bias.inputs[2].default_value = (0.5, 0.5, 0.5, 0)
         links.new(node_normal_scale.outputs[0], node_normal_bias.inputs[1])
         node_normal = nodes.new(type="CompositorNodeOutputFile")
         node_normal.label = "Normal Output"
-        node_normal.base_path = ""
+        node_normal.base_path = "/"
         node_normal.file_slots[0].use_node_format = True
         node_normal.format.file_format = "PNG"
         node_normal.format.color_mode = "RGBA"
         links.new(node_normal_bias.outputs[0], node_normal.inputs[0])
 
         refs['node_normal'] = node_normal
 
@@ -140,15 +140,15 @@
     if args.albedo:
         bpy.context.view_layer.use_pass_diffuse_color = True
         node_albedo_alpha = nodes.new(type="CompositorNodeSetAlpha")
         links.new(render_layers.outputs["DiffCol"], node_albedo_alpha.inputs["Image"])
         links.new(render_layers.outputs["Alpha"], node_albedo_alpha.inputs["Alpha"])
         node_albedo = nodes.new(type="CompositorNodeOutputFile")
         node_albedo.label = "Albedo Output"
-        node_albedo.base_path = ""
+        node_albedo.base_path = "/"
         node_albedo.file_slots[0].use_node_format = True
         node_albedo.format.file_format = "PNG"
         node_albedo.format.color_mode = "RGBA"
         links.new(node_albedo_alpha.outputs["Image"], node_albedo.inputs[0])
 
         refs['node_albedo'] = node_albedo
 
@@ -293,15 +293,15 @@
 
     # load the object
     name = os.path.basename(args.mesh).split(".")[0]
     os.makedirs(os.path.join(args.outdir, name), exist_ok=True)
     load_object(args.mesh)
 
     # clever clean scene
-    clean_scene_meshes()
+    # clean_scene_meshes()
 
     # normalize objects to [-b, b]^3
     clear_animation()
     normalize_scene(bound=args.bound)
 
     # load random hdri
     hdri_paths = glob.glob(os.path.join(os.path.dirname(os.path.abspath(__file__)), '../assets/blender_lights/*.exr'))
@@ -345,14 +345,15 @@
         c2w_opengl[1] *= -1
         c2w_opengl[[1, 2]] = c2w_opengl[[2, 1]]
 
         cam_poses.append(c2w_opengl)
 
         # render image
         render_file_path = os.path.join(args.outdir, name, f"{i:03d}")
+        render_file_path = os.path.abspath(render_file_path) # relative path leads to problems for depth/normal/albedo nodes...
         bpy.context.scene.render.filepath = render_file_path
 
         if args.depth:
             refs['node_depth'].file_slots[0].path = render_file_path + "_depth"
         if args.normal:
             refs['node_normal'].file_slots[0].path = render_file_path + "_normal"
         if args.albedo:
@@ -395,13 +396,13 @@
     parser.add_argument('--normal', action='store_true')
     parser.add_argument('--albedo', action='store_true')
     parser.add_argument('--overwrite', action='store_true')
 
     # rendering parameters
     parser.add_argument("--resolution", type=int, default=512)
     parser.add_argument("--bound", type=float, default=0.9)
-    parser.add_argument("--radius", type=float, default=2.5)
-    parser.add_argument("--fovy", type=float, default=49.1)
+    parser.add_argument("--radius", type=float, default=4.5)
+    parser.add_argument("--fovy", type=float, default=30)
 
     args = parser.parse_args()
 
     main(args)
```

### Comparing `kiui-0.2.7/kiui/cli/blip.py` & `kiui-0.2.8/kiui/cli/blip.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/cli/clip_sim.py` & `kiui-0.2.8/kiui/cli/clip_sim.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     parser.add_argument('mesh', type=str, help="path to mesh (obj, glb, ...)")
     parser.add_argument('--pbr', action='store_true', help="enable PBR material")
     parser.add_argument('--envmap', type=str, default=None, help="hdr env map path for pbr")
     parser.add_argument('--front_dir', type=str, default='+z', help="mesh front-facing dir")
     parser.add_argument('--mode', default='albedo', type=str, choices=['lambertian', 'albedo', 'normal', 'depth', 'pbr'], help="rendering mode")
     parser.add_argument('--W', type=int, default=800, help="GUI width")
     parser.add_argument('--H', type=int, default=800, help="GUI height")
+    parser.add_argument('--ssaa', type=float, default=1, help="super-sampling anti-aliasing ratio")
     parser.add_argument('--radius', type=float, default=3, help="default GUI camera radius from center")
     parser.add_argument('--fovy', type=float, default=50, help="default GUI camera fovy")
     parser.add_argument("--force_cuda_rast", action='store_true', help="force to use RasterizeCudaContext.")
     parser.add_argument('--elevation', type=int, default=0, help="rendering elevation")
     parser.add_argument('--num_azimuth', type=int, default=8, help="number of images to render from different azimuths")
     
     opt = parser.parse_args()
@@ -92,8 +93,8 @@
             similarity = (ref_features * cur_features).sum(dim=-1).mean().item()
 
             results.append(similarity)
     
     avg_similarity = np.mean(results)
     print(avg_similarity)
 
-            
+
```

### Comparing `kiui-0.2.7/kiui/cli/clip_sim_text.py` & `kiui-0.2.8/kiui/cli/clip_sim_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     parser.add_argument('mesh', type=str, help="path to mesh (obj, glb, ...)")
     parser.add_argument('--pbr', action='store_true', help="enable PBR material")
     parser.add_argument('--envmap', type=str, default=None, help="hdr env map path for pbr")
     parser.add_argument('--front_dir', type=str, default='+z', help="mesh front-facing dir")
     parser.add_argument('--mode', default='albedo', type=str, choices=['lambertian', 'albedo', 'normal', 'depth', 'pbr'], help="rendering mode")
     parser.add_argument('--W', type=int, default=800, help="GUI width")
     parser.add_argument('--H', type=int, default=800, help="GUI height")
+    parser.add_argument('--ssaa', type=float, default=1, help="super-sampling anti-aliasing ratio")
     parser.add_argument('--radius', type=float, default=3, help="default GUI camera radius from center")
     parser.add_argument('--fovy', type=float, default=50, help="default GUI camera fovy")
     parser.add_argument("--force_cuda_rast", action='store_true', help="force to use RasterizeCudaContext.")
     parser.add_argument('--elevation', type=int, default=0, help="rendering elevation")
     parser.add_argument('--num_azimuth', type=int, default=8, help="number of images to render from different azimuths")
     
     opt = parser.parse_args()
@@ -86,8 +87,8 @@
             similarity = (ref_features * cur_features).sum(dim=-1).mean().item()
 
             results.append(similarity)
     
     avg_similarity = np.mean(results)
     print(avg_similarity)
 
-            
+
```

### Comparing `kiui-0.2.7/kiui/cli/convert.py` & `kiui-0.2.8/kiui/cli/convert.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/cli/depth_midas.py` & `kiui-0.2.8/kiui/cli/depth_midas.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/cli/depth_zoe.py` & `kiui-0.2.8/kiui/cli/depth_zoe.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/cli/dircmp.py` & `kiui-0.2.8/kiui/cli/dircmp.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/cli/hed.py` & `kiui-0.2.8/kiui/cli/hed.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/cli/lock_version.py` & `kiui-0.2.8/kiui/cli/lock_version.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/cli/openpose/__init__.py` & `kiui-0.2.8/kiui/cli/openpose/__init__.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/cli/openpose/body.py` & `kiui-0.2.8/kiui/cli/openpose/body.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/cli/openpose/face.py` & `kiui-0.2.8/kiui/cli/openpose/face.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/cli/openpose/hand.py` & `kiui-0.2.8/kiui/cli/openpose/hand.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/cli/openpose/model.py` & `kiui-0.2.8/kiui/cli/openpose/model.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/cli/openpose/util.py` & `kiui-0.2.8/kiui/cli/openpose/util.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/cli/pose.py` & `kiui-0.2.8/kiui/cli/pose.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/cli/remesh.py` & `kiui-0.2.8/kiui/cli/remesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -521,24 +521,24 @@
     resolution: int = 512
     # nvdiffrast context
     force_cuda_rast: bool = False
     # use fixed 16 cameras and cache gt renders, faster
     fix_cameras: bool = True 
 
     ## params for remeshing
+    # smallest and largest allowed reference edge length (controls final triangle sizes!)
+    edge_len_lims: Tuple[float, ...] = (0.01, 0.15) 
     # learning rate
     lr: float = 0.3 
     # betas[0:2] are the same as in Adam, betas[2] may be used to time-smooth the relative velocity nu
     betas: Tuple[float, ...] = (0.8, 0.8, 0) 
     # optional spatial smoothing for m1,m2,nu, values between 0 (no smoothing) and 1 (max. smoothing)
     gammas: Tuple[float, ...] = (0, 0, 0) 
     # reference velocity for edge length controller
     nu_ref: float = 0.3 
-    # smallest and largest allowed reference edge length
-    edge_len_lims: Tuple[float, ...] = (0.01, 0.15) 
     # edge length tolerance for split and collapse
     edge_len_tol: float = 0.5 
     # gain value for edge length controller
     gain: float = 0.2 
     # for laplacian smoothing/regularization
     laplacian_weight: float = 0.02 
     # learning rate ramp, actual ramp width is ramp/(1-betas[0])
@@ -559,15 +559,15 @@
         self.with_gammas = any(g != 0 for g in self.opt.gammas)
         self.step = 0
 
         # only support cuda
         self.device = torch.device("cuda")
 
         # load input mesh
-        self.mesh = Mesh.load(opt.mesh, bound=0.9, device=self.device)
+        self.mesh = Mesh.load(opt.mesh, bound=0.9, wotex=True, device=self.device)
 
         # init primitive (icosphere now)
         vertices, self.faces = self.init_primitives(level=2, bound=0.5)
         V = vertices.shape[0]
 
         # fixed persp
         self.proj = torch.from_numpy(get_perspective(opt.fovy)).float().to(self.device)
@@ -734,23 +734,23 @@
         poses = torch.from_numpy(poses.astype(np.float32)).to(self.device)
 
         return poses
 
     def fit(self, iters=300):
 
         if self.opt.fix_cameras:
-            # ca.optche gt renders
+            # cache gt renders
             poses = self.get_cameras()
             images_gt = self.render_gt(poses, self.opt.resolution)
 
         pbar = tqdm.trange(iters)
         for i in pbar:
 
             if not self.opt.fix_cameras:
-                # ra.optndom orbital camera pose
+                # random orbital camera pose
                 poses = self.get_cameras()
                 images_gt = self.render_gt(poses, self.opt.resolution)
 
             images = self.render(poses, self.opt.resolution)
 
             # loss
             loss = F.l1_loss(images, images_gt)
@@ -761,15 +761,15 @@
 
             # remesh
             self.remesh()
 
             # zero grad
             self.vertices.grad = None
 
-            pbar.set_description(f"loss = {loss.item():.6f}")
+            pbar.set_description(f"loss={loss.item():.6f} v={self.vertices.shape} f={self.faces.shape}")
 
     def export(self, path):
         mesh = Mesh(v=self.vertices, f=self.faces)
         mesh.write(path)
 
 
 if __name__ == "__main__":
```

### Comparing `kiui-0.2.7/kiui/cli/timer.py` & `kiui-0.2.8/kiui/cli/timer.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/env.py` & `kiui-0.2.8/kiui/env.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/grid_put.py` & `kiui-0.2.8/kiui/grid_put.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/gridencoder/backend.py` & `kiui-0.2.8/kiui/gridencoder/backend.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/gridencoder/grid.py` & `kiui-0.2.8/kiui/gridencoder/grid.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/gridencoder/src/gridencoder.cu` & `kiui-0.2.8/kiui/gridencoder/src/gridencoder.cu`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/gridencoder/src/gridencoder.h` & `kiui-0.2.8/kiui/gridencoder/src/gridencoder.h`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/lpips.py` & `kiui-0.2.8/kiui/lpips.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/mesh.py` & `kiui-0.2.8/kiui/mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,25 +103,28 @@
             from kiui.mesh_utils import clean_mesh
             vertices = mesh.v.detach().cpu().numpy()
             triangles = mesh.f.detach().cpu().numpy()
             vertices, triangles = clean_mesh(vertices, triangles, remesh=False)
             mesh.v = torch.from_numpy(vertices).contiguous().float().to(mesh.device)
             mesh.f = torch.from_numpy(triangles).contiguous().int().to(mesh.device)
 
-        print(f"[INFO] load mesh, v: {mesh.v.shape}, f: {mesh.f.shape}")
         # auto-normalize
         if resize:
             mesh.auto_size(bound=bound)
+        print(f"[INFO] load mesh, v: {mesh.v.shape}, f: {mesh.f.shape}")
+        
         # auto-fix normal
         if renormal or mesh.vn is None:
             mesh.auto_normal()
-            print(f"[INFO] load mesh, vn: {mesh.vn.shape}, fn: {mesh.fn.shape}")
+        print(f"[INFO] load mesh, vn: {mesh.vn.shape}, fn: {mesh.fn.shape}")
+
         # auto-fix texcoords
-        if retex or (mesh.albedo is not None and mesh.vt is None):
+        if retex:
             mesh.auto_uv(cache_path=path)
+        if mesh.vt is not None:
             print(f"[INFO] load mesh, vt: {mesh.vt.shape}, ft: {mesh.ft.shape}")
 
         # rotate front dir to +z
         if front_dir != "+z":
             # axis switch
             if "-z" in front_dir:
                 T = torch.tensor([[1, 0, 0], [0, 1, 0], [0, 0, -1]], device=mesh.device, dtype=torch.float32)
@@ -369,30 +372,37 @@
         if not wotex:
             if _mesh.visual.kind == 'vertex':
                 vertex_colors = _mesh.visual.vertex_colors
                 vertex_colors = np.array(vertex_colors[..., :3]).astype(np.float32) / 255
                 mesh.vc = torch.tensor(vertex_colors, dtype=torch.float32, device=device)
                 print(f"[INFO] load trimesh: use vertex color: {mesh.vc.shape}")
             elif _mesh.visual.kind == 'texture':
-                _material = _mesh.visual.material
-                if isinstance(_material, trimesh.visual.material.PBRMaterial):
-                    texture = np.array(_material.baseColorTexture).astype(np.float32) / 255
-                    # load metallicRoughness if present
-                    if _material.metallicRoughnessTexture is not None:
-                        metallicRoughness = np.array(_material.metallicRoughnessTexture).astype(np.float32) / 255
-                        # NOTE: fix a bug in trimesh that loads metallicRoughness in wrong channels: https://github.com/mikedh/trimesh/issues/2195
-                        if version.parse(trimesh.__version__) < version.parse('4.2.2'):
-                            metallicRoughness = metallicRoughness[..., [2, 1, 0]]
-                        mesh.metallicRoughness = torch.tensor(metallicRoughness, dtype=torch.float32, device=device).contiguous()
-                elif isinstance(_material, trimesh.visual.material.SimpleMaterial):
-                    texture = np.array(_material.to_pbr().baseColorTexture).astype(np.float32) / 255
-                else:
-                    raise NotImplementedError(f"material type {type(_material)} not supported!")
-                mesh.albedo = torch.tensor(texture[..., :3], dtype=torch.float32, device=device).contiguous()
-                print(f"[INFO] load trimesh: load texture: {texture.shape}")
+                try:
+                    _material = _mesh.visual.material
+                    if isinstance(_material, trimesh.visual.material.PBRMaterial):
+                        texture = np.array(_material.baseColorTexture).astype(np.float32) / 255
+                        # load metallicRoughness if present
+                        if _material.metallicRoughnessTexture is not None:
+                            metallicRoughness = np.array(_material.metallicRoughnessTexture).astype(np.float32) / 255
+                            # NOTE: fix a bug in trimesh that loads metallicRoughness in wrong channels: https://github.com/mikedh/trimesh/issues/2195
+                            if version.parse(trimesh.__version__) < version.parse('4.2.2'):
+                                metallicRoughness = metallicRoughness[..., [2, 1, 0]]
+                            mesh.metallicRoughness = torch.tensor(metallicRoughness, dtype=torch.float32, device=device).contiguous()
+                    elif isinstance(_material, trimesh.visual.material.SimpleMaterial):
+                        texture = np.array(_material.to_pbr().baseColorTexture).astype(np.float32) / 255
+                    else:
+                        raise NotImplementedError(f"material type {type(_material)} not supported!")
+                    if len(texture.shape) == 2:
+                        texture = texture[..., None].repeat(3, axis=-1)
+                    mesh.albedo = torch.tensor(texture[..., :3], dtype=torch.float32, device=device).contiguous()
+                    print(f"[INFO] load trimesh: load texture: {texture.shape}")
+                # there really can be lots of mysterious errors...
+                except Exception as e:
+                    mesh.albedo = None
+                    print(f"[INFO] load trimesh: failed to load texture.")
             else:
                 mesh.albedo = None
                 print(f"[INFO] load trimesh: failed to load texture.")
 
         vertices = _mesh.vertices
 
         try:
```

### Comparing `kiui-0.2.7/kiui/mesh_utils.py` & `kiui-0.2.8/kiui/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/nn/__init__.py` & `kiui-0.2.8/kiui/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/nn/attention.py` & `kiui-0.2.8/kiui/nn/attention.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/nn/encoder.py` & `kiui-0.2.8/kiui/nn/encoder.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/nn/sparse.py` & `kiui-0.2.8/kiui/nn/sparse.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/nn/transformer.py` & `kiui-0.2.8/kiui/nn/transformer.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/nn/unet_2d.py` & `kiui-0.2.8/kiui/nn/unet_2d.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/nn/unet_2d_cond.py` & `kiui-0.2.8/kiui/nn/unet_2d_cond.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/nn/unet_3d_cond.py` & `kiui-0.2.8/kiui/nn/unet_3d_cond.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/nn/utils.py` & `kiui-0.2.8/kiui/nn/utils.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/nn/vae_2d.py` & `kiui-0.2.8/kiui/nn/vae_2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.utils.checkpoint import checkpoint
 
 from kiui.typing import *
 from kiui.nn.attention import MemEffAttention
 
-
 class ImageAttention(nn.Module):
     def __init__(
         self, 
         dim: int,
         num_heads: int = 8,
         qkv_bias: bool = False,
         proj_bias: bool = True,
@@ -66,17 +65,17 @@
         return x
 
     def kl(self, other=None, dims=[1, 2, 3]):
         if self.deterministic:
             return torch.Tensor([0.0])
         else:
             if other is None:
-                return 0.5 * torch.sum(torch.pow(self.mean, 2) + self.var - 1.0 - self.logvar, dim=dims)
+                return 0.5 * torch.mean(torch.pow(self.mean, 2) + self.var - 1.0 - self.logvar, dim=dims)
             else:
-                return 0.5 * torch.sum(
+                return 0.5 * torch.mean(
                     torch.pow(self.mean - other.mean, 2) / other.var
                     + self.var / other.var
                     - 1.0
                     - self.logvar
                     + other.logvar,
                     dim=dims,
                 )
@@ -465,11 +464,11 @@
         kiui.lo(y)
         kiui.lo(p.mean)
 
         mem_free, mem_total = torch.cuda.mem_get_info()
         print(f'[INFO] mem forward: {(mem_total-mem_free)/1024**3:.2f}/{mem_total/1024**3:.2f}G')
 
         # test backward
-        loss = y.mean() + 1e-6 * p.kl().mean()
+        loss = y.mean() + 1e-3 * p.kl().mean()
         loss.backward()
         mem_free, mem_total = torch.cuda.mem_get_info()
         print(f'[INFO] mem backward: {(mem_total-mem_free)/1024**3:.2f}/{mem_total/1024**3:.2f}G')
```

### Comparing `kiui-0.2.7/kiui/nn/vae_3d.py` & `kiui-0.2.8/kiui/nn/vae_3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
         x = x.reshape(B, H, W, D, C).permute(0, 4, 1, 2, 3).reshape(B, C, H, W, D)
 
         if self.residual:
             x = (x + res) * self.skip_scale
             
         return x
 
-
 class DiagonalGaussianDistribution:
     def __init__(self, parameters, deterministic=False):
         # parameters: [B, 2C, ...]
         self.parameters = parameters
         self.mean, self.logvar = torch.chunk(parameters, 2, dim=1)
         self.logvar = torch.clamp(self.logvar, -30.0, 20.0)
         self.deterministic = deterministic
@@ -66,17 +65,17 @@
         return x
 
     def kl(self, other=None, dims=[1, 2, 3, 4]):
         if self.deterministic:
             return torch.Tensor([0.0])
         else:
             if other is None:
-                return 0.5 * torch.sum(torch.pow(self.mean, 2) + self.var - 1.0 - self.logvar, dim=dims)
+                return 0.5 * torch.mean(torch.pow(self.mean, 2) + self.var - 1.0 - self.logvar, dim=dims)
             else:
-                return 0.5 * torch.sum(
+                return 0.5 * torch.mean(
                     torch.pow(self.mean - other.mean, 2) / other.var
                     + self.var / other.var
                     - 1.0
                     - self.logvar
                     + other.logvar,
                     dim=dims,
                 )
@@ -457,30 +456,42 @@
 
 if __name__ == '__main__':
     import kiui
     from kiui.nn.utils import count_parameters
     
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
-    model = VAE(gradient_checkpointing=True).to(device)
+    # model = VAE(gradient_checkpointing=True).to(device)
+    model = VAE(
+        in_channels = 6,
+        latent_channels = 128,
+        out_channels = 6,
+        down_channels = (32, 128, 512),
+        mid_attention = True,
+        up_channels = (512, 128, 32),
+        layers_per_block = 2,
+        skip_scale = np.sqrt(0.5),
+        gradient_checkpointing = True,
+    ).to(device)
     print(model)
     
     total, trainable = count_parameters(model)
     print(f'[INFO] param total: {total/1024**2:.2f}M, trainable: {trainable/1024**2:.2f}M')
 
     # test forward
-    x = torch.randn(1, 1, 512, 512, 512, device=device, dtype=torch.float16)
+    # x = torch.randn(1, 1, 512, 512, 512, device=device, dtype=torch.float16)
+    x = torch.randn(2048, 6, 8, 8, 8, device=device, dtype=torch.float16)
     kiui.lo(x)
     
     with torch.autocast(device_type='cuda', dtype=torch.float16):
         y, p = model(x)
         kiui.lo(y)
         kiui.lo(p.mean)
         
         mem_free, mem_total = torch.cuda.mem_get_info()
         print(f'[INFO] mem forward: {(mem_total-mem_free)/1024**3:.2f}/{mem_total/1024**3:.2f}G')
 
         # test backward
-        loss = y.mean() + 1e-6 * p.kl().mean()
+        loss = y.mean() + 1e-3 * p.kl().mean()
         loss.backward()
         mem_free, mem_total = torch.cuda.mem_get_info()
         print(f'[INFO] mem backward: {(mem_total-mem_free)/1024**3:.2f}/{mem_total/1024**3:.2f}G')
```

### Comparing `kiui-0.2.7/kiui/op.py` & `kiui-0.2.8/kiui/op.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/poser.py` & `kiui-0.2.8/kiui/poser.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/quaternion.py` & `kiui-0.2.8/kiui/quaternion.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/render.py` & `kiui-0.2.8/kiui/render.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class GUI:
     def __init__(self, opt):
         self.opt = opt
         self.W = opt.W
         self.H = opt.H
         if not GUI_AVAILABLE and not opt.wogui:
-            print(f'[WARN] cannot import dearpygui, assume without --wogui')
+            print(f'[WARN] cannot import dearpygui, assume running with --wogui')
         self.wogui = not GUI_AVAILABLE or opt.wogui # disable gui and run in cmd
         self.cam = OrbitCamera(opt.W, opt.H, r=opt.radius, fovy=opt.fovy)
         self.bg_color = torch.ones(3, dtype=torch.float32).cuda() # default white bg
         # self.bg_color = torch.zeros(3, dtype=torch.float32).cuda() # black bg
 
         self.render_buffer = np.zeros((self.W, self.H, 3), dtype=np.float32)
         self.need_update = True # camera moved, should reset accumulation
@@ -98,15 +98,16 @@
         # do MVP for vertices
         pose = torch.from_numpy(self.cam.pose.astype(np.float32)).cuda()
         proj = torch.from_numpy(self.cam.perspective.astype(np.float32)).cuda()
         
         v_cam = torch.matmul(F.pad(self.mesh.v, pad=(0, 1), mode='constant', value=1.0), torch.inverse(pose).T).float().unsqueeze(0)
         v_clip = v_cam @ proj.T
 
-        rast, rast_db = dr.rasterize(self.glctx, v_clip, self.mesh.f, (self.H, self.W))
+        H, W = int(self.opt.ssaa * self.H), int(self.opt.ssaa * self.W)
+        rast, rast_db = dr.rasterize(self.glctx, v_clip, self.mesh.f, (H, W))
 
         alpha = (rast[..., 3:] > 0).float()
         alpha = dr.antialias(alpha, rast, v_clip, self.mesh.f).squeeze(0).clamp(0, 1) # [H, W, 3]
         
         if self.mode == 'depth':
             depth, _ = dr.interpolate(-v_cam[..., [2]], rast, self.mesh.f) # [1, H, W, 1]
             depth = (depth - depth.min()) / (depth.max() - depth.min() + 1e-20)
@@ -168,15 +169,15 @@
 
                     fg_uv = torch.cat([n_dot_v, roughness], -1).clamp(0, 1) # [H, W, 2]
                     fg = dr.texture(
                         self.FG_LUT,
                         fg_uv.reshape(1, -1, 1, 2).contiguous(),
                         filter_mode="linear",
                         boundary_mode="clamp",
-                    ).reshape(1, self.H, self.W, 2)
+                    ).reshape(1, H, W, 2)
                     F0 = (1 - metallic) * 0.04 + metallic * albedo
                     specular_albedo = F0 * fg[..., 0:1] + fg[..., 1:2]
 
                     diffuse_light = self.light(normal)
                     specular_light = self.light(reflective, roughness)
 
                     color = diffuse_albedo * diffuse_light + specular_albedo * specular_light # [H, W, 3]
@@ -187,14 +188,18 @@
         if self.show_wire:
             u = rast[..., 0] # [1, h, w]
             v = rast[..., 1] # [1, h, w]
             w = 1 - u - v
             mask = rast[..., 2]
             near_edge = (((w < 0.01) | (u < 0.01) | (v < 0.01)) & (mask > 0))[0].detach().cpu().numpy() # [h, w]
             buffer[near_edge] = np.array([0, 0, 0], dtype=np.float32) # black wire
+        
+        # ssaa rescale
+        if H != self.H or W != self.W:
+            buffer = cv2.resize(buffer, (self.H, self.W), interpolation=cv2.INTER_AREA)
 
         ender.record()
         torch.cuda.synchronize()
         t = starter.elapsed_time(ender)
 
         self.render_buffer = buffer
         self.need_update = False
@@ -407,14 +412,15 @@
     parser.add_argument('mesh', type=str, help="path to mesh (obj, ply, glb, ...)")
     parser.add_argument('--pbr', action='store_true', help="enable PBR material")
     parser.add_argument('--envmap', type=str, default=None, help="hdr env map path for pbr")
     parser.add_argument('--front_dir', type=str, default='+z', help="mesh front-facing dir")
     parser.add_argument('--mode', default='albedo', type=str, choices=['lambertian', 'albedo', 'normal', 'depth', 'pbr'], help="rendering mode")
     parser.add_argument('--W', type=int, default=800, help="GUI width")
     parser.add_argument('--H', type=int, default=800, help="GUI height")
+    parser.add_argument('--ssaa', type=float, default=1, help="super-sampling anti-aliasing ratio")
     parser.add_argument('--radius', type=float, default=3, help="default GUI camera radius from center")
     parser.add_argument('--fovy', type=float, default=50, help="default GUI camera fovy")
     parser.add_argument("--wogui", action='store_true', help="disable all dpg GUI")
     parser.add_argument("--force_cuda_rast", action='store_true', help="force to use RasterizeCudaContext.")
     parser.add_argument('--save', type=str, default=None, help="path to save example rendered images")
     parser.add_argument('--elevation', type=int, default=0, help="rendering elevation")
     parser.add_argument('--num_azimuth', type=int, default=8, help="number of images to render from different azimuths")
```

### Comparing `kiui-0.2.7/kiui/render_viser.py` & `kiui-0.2.8/kiui/render_viser.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/sh.py` & `kiui-0.2.8/kiui/sh.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/sr.py` & `kiui-0.2.8/kiui/sr.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/utils.py` & `kiui-0.2.8/kiui/utils.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui/vis.py` & `kiui-0.2.8/kiui/vis.py`

 * *Files identical despite different names*

### Comparing `kiui-0.2.7/kiui.egg-info/PKG-INFO` & `kiui-0.2.8/kiui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiui
-Version: 0.2.7
+Version: 0.2.8
 Summary: A toolkit for 3D vision
 Home-page: https://github.com/ashawkey/kiuikit
 Author: kiui
 Author-email: ashawkey1999@gmail.com
 Keywords: utility
 Classifier: Programming Language :: Python :: 3 
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kiui Version: 0.2.7 Summary: A toolkit for 3D
+Metadata-Version: 2.1 Name: kiui Version: 0.2.8 Summary: A toolkit for 3D
 vision Home-page: https://github.com/ashawkey/kiuikit Author: kiui Author-
 email: ashawkey1999@gmail.com Keywords: utility Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
 full License-File: LICENSE
           [kiuikit_logo]KKiiuuiikkiitt pip install kiui   •   _D_o_c_u_m_e_n_t_a_t_i_o_n
 A toolkit for computer vision (especially 3D vision) tasks. **Features**: *
 Collection of *maintained, reusable and trustworthy* code snippets. * Always
```

### Comparing `kiui-0.2.7/kiui.egg-info/SOURCES.txt` & `kiui-0.2.8/kiui.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -36,19 +36,21 @@
 kiui/assets/blender_lights/sunset.exr
 kiui/assets/lights/LICENSE.txt
 kiui/assets/lights/bsdf_256_256.bin
 kiui/assets/lights/mud_road_puresky_1k.hdr
 kiui/cli/__init__.py
 kiui/cli/aes.py
 kiui/cli/bg.py
+kiui/cli/blender_qremesh.py
 kiui/cli/blender_render.py
 kiui/cli/blip.py
 kiui/cli/clip_sim.py
 kiui/cli/clip_sim_text.py
 kiui/cli/convert.py
+kiui/cli/convert_fp16.py
 kiui/cli/depth_midas.py
 kiui/cli/depth_zoe.py
 kiui/cli/dircmp.py
 kiui/cli/hed.py
 kiui/cli/lock_version.py
 kiui/cli/pose.py
 kiui/cli/remesh.py
@@ -64,14 +66,15 @@
 kiui/gridencoder/grid.py
 kiui/gridencoder/src/bindings.cpp
 kiui/gridencoder/src/gridencoder.cu
 kiui/gridencoder/src/gridencoder.h
 kiui/nn/__init__.py
 kiui/nn/attention.py
 kiui/nn/encoder.py
+kiui/nn/perciever.py
 kiui/nn/sparse.py
 kiui/nn/transformer.py
 kiui/nn/unet_2d.py
 kiui/nn/unet_2d_cond.py
 kiui/nn/unet_3d_cond.py
 kiui/nn/utils.py
 kiui/nn/vae_2d.py
```

### Comparing `kiui-0.2.7/setup.py` & `kiui-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 if __name__ == "__main__":
     setup(
         name="kiui",
-        version="0.2.7",
+        version="0.2.8",
         description="A toolkit for 3D vision",
         long_description=open("README.md", encoding="utf-8").read(),
         long_description_content_type="text/markdown",
         url="https://github.com/ashawkey/kiuikit",
         author="kiui",
         author_email="ashawkey1999@gmail.com",
         packages=find_packages(),
```


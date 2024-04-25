# Comparing `tmp/ajc27_freemocap_blender_addon-2023.10.1016.tar.gz` & `tmp/ajc27_freemocap_blender_addon-2023.10.1017.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ajc27_freemocap_blender_addon-2023.10.1016.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ajc27_freemocap_blender_addon-2023.10.1017.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ajc27_freemocap_blender_addon-2023.10.1016.tar` & `ajc27_freemocap_blender_addon-2023.10.1017.tar`

### file list

```diff
@@ -1,111 +1,146 @@
--rw-r--r--   0        0        0     1114 2023-12-12 01:50:57.296159 ajc27_freemocap_blender_addon-2023.10.1016/.github/workflows/flit_publish_to_pypi.yml
--rw-r--r--   0        0        0     1113 2023-12-12 01:50:57.296159 ajc27_freemocap_blender_addon-2023.10.1016/.github/workflows/publish_to_pypi_on_version_bump.yml
--rw-r--r--   0        0        0     1871 2023-12-12 01:50:57.296159 ajc27_freemocap_blender_addon-2023.10.1016/.gitignore
--rw-r--r--   0        0        0    34523 2023-12-12 01:50:57.296159 ajc27_freemocap_blender_addon-2023.10.1016/LICENSE
--rw-r--r--   0        0        0      693 2023-12-12 01:50:57.296159 ajc27_freemocap_blender_addon-2023.10.1016/README.md
--rw-r--r--   0        0        0     2852 2023-12-12 01:50:57.296159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/__init__.py
--rw-r--r--   0        0        0   705884 2023-12-12 01:50:57.300159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/assets/skelly_lowpoly_mesh.fbx
--rw-r--r--   0        0        0      500 2023-12-12 01:50:57.300159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/__init__.py
--rw-r--r--   0        0        0     8000 2023-12-12 01:50:57.300159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/main_view3d_panel.py
--rw-r--r--   0        0        0     1701 2023-12-12 01:50:57.300159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/operators/__init__.py
--rw-r--r--   0        0        0     2452 2023-12-12 01:50:57.300159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/operators/_add_body_mesh.py
--rw-r--r--   0        0        0     2636 2023-12-12 01:50:57.300159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/operators/_add_rig.py
--rw-r--r--   0        0        0      332 2023-12-12 01:50:57.300159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/operators/_clear_scene.py
--rw-r--r--   0        0        0      426 2023-12-12 01:50:57.300159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/operators/_download_sample_data.py
--rw-r--r--   0        0        0     1095 2023-12-12 01:50:57.300159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/operators/_export_fbx.py
--rw-r--r--   0        0        0     2023 2023-12-12 01:50:57.300159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/operators/_load_freemocap_data.py
--rw-r--r--   0        0        0      669 2023-12-12 01:50:57.300159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/operators/_load_videos.py
--rw-r--r--   0        0        0     1578 2023-12-12 01:50:57.300159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/operators/_reduce_bone_length_dispersion.py
--rw-r--r--   0        0        0      972 2023-12-12 01:50:57.300159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/operators/_reduce_shakiness.py
--rw-r--r--   0        0        0     2297 2023-12-12 01:50:57.300159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/operators/_reorient_empties.py
--rw-r--r--   0        0        0     1417 2023-12-12 01:50:57.300159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/operators/_run_all.py
--rw-r--r--   0        0        0     1517 2023-12-12 01:50:57.300159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/operators/_save_out_data.py
--rw-r--r--   0        0        0     5935 2023-12-12 01:50:57.300159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/properties.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/sub_panels/__init__.py
--rw-r--r--   0        0        0       67 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/__init__.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/bones/__init__.py
--rw-r--r--   0        0        0     2987 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/bones/calculate_body_dimensions.py
--rw-r--r--   0        0        0     2120 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/bones/calculate_bone_length_statistics.py
--rw-r--r--   0        0        0     5751 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/bones/enforce_rigid_bones.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/empties/__init__.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/empties/creation/__init__.py
--rw-r--r--   0        0        0     2068 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/empties/creation/create_empty_from_trajectory.py
--rw-r--r--   0        0        0     2262 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/empties/creation/create_freemocap_empties.py
--rw-r--r--   0        0        0     4183 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/empties/creation/create_virtual_trajectories.py
--rw-r--r--   0        0        0     4801 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/empties/hands.py
--rw-r--r--   0        0        0     3578 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/empties/reduce_shakiness.py
--rw-r--r--   0        0        0     9042 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/empties/reorient_empties.py
--rw-r--r--   0        0        0     1705 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/empties/translate_empty_and_its_children.py
--rw-r--r--   0        0        0     3887 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/empties/update_empty_positions.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/fbx_export/__init__.py
--rw-r--r--   0        0        0    29618 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/fbx_export/fbx.py
--rw-r--r--   0        0        0     1900 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/fbx_export/get_io_scene_fbx_addon.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/freemocap_data_handler/__init__.py
--rw-r--r--   0        0        0    26817 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/freemocap_data_handler/handler.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/freemocap_data_handler/helpers/__init__.py
--rw-r--r--   0        0        0      579 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/freemocap_data_handler/helpers/get_or_create_freemocap_data_handler.py
--rw-r--r--   0        0        0    11109 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/freemocap_data_handler/helpers/saver.py
--rw-r--r--   0        0        0     9330 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/freemocap_data_handler/helpers/transformer.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/freemocap_data_handler/operations/__init__.py
--rw-r--r--   0        0        0     3604 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/freemocap_data_handler/operations/estimate_good_frame.py
--rw-r--r--   0        0        0     6146 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/freemocap_data_handler/operations/fix_hand_data.py
--rw-r--r--   0        0        0      209 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/freemocap_data_handler/operations/freemocap_empties_from_parent_object.py
--rw-r--r--   0        0        0     5614 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/freemocap_data_handler/operations/put_skeleton_on_ground.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/load_data/__init__.py
--rw-r--r--   0        0        0      732 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/load_data/load_freemocap_data.py
--rw-r--r--   0        0        0     3122 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/load_data/load_videos.py
--rw-r--r--   0        0        0    13612 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/main_controller.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/__init__.py
--rw-r--r--   0        0        0    13248 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/attach_mesh_to_rig.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/center_of_mass/__init__.py
--rw-r--r--   0        0        0     1265 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/center_of_mass/center_of_mass_material.py
--rw-r--r--   0        0        0      847 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/center_of_mass/center_of_mass_mesh.py
--rw-r--r--   0        0        0     4860 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/center_of_mass/center_of_mass_trails.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/__init__.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/__init__.py
--rw-r--r--   0        0        0      942 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/create_bone_stick.py
--rw-r--r--   0        0        0     6136 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/create_material.py
--rw-r--r--   0        0        0      690 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/get_edit_bones.py
--rw-r--r--   0        0        0     4998 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/make_bone_mesh.py
--rw-r--r--   0        0        0      877 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/parent_mesh_to_rig.py
--rw-r--r--   0        0        0     5205 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/put_meshes_on_empties.py
--rw-r--r--   0        0        0     1427 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/put_sphere_at_location.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/skelly_mesh/__init__.py
--rw-r--r--   0        0        0     3486 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/skelly_mesh/attach_skelly_mesh.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/rig/__init__.py
--rw-r--r--   0        0        0    41882 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/rig/add_rig.py
--rw-r--r--   0        0        0     5590 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/rig/save_bone_and_joint_angles_from_rig.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/setup_scene/__init__.py
--rw-r--r--   0        0        0      528 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/setup_scene/clear_scene.py
--rw-r--r--   0        0        0     1248 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/setup_scene/get_path_to_sample_data.py
--rw-r--r--   0        0        0      594 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/setup_scene/make_parent_empties.py
--rw-r--r--   0        0        0      344 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/setup_scene/set_start_end_frame.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/video_output/__init__.py
--rw-r--r--   0        0        0       66 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/video_output/create_video_output.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/__init__.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/bones/__init__.py
--rw-r--r--   0        0        0    14652 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/bones/bone_constraints.py
--rw-r--r--   0        0        0    10402 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/bones/bone_definitions.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/freemocap_data/__init__.py
--rw-r--r--   0        0        0     9950 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/freemocap_data/freemocap_data_model.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/__init__.py
--rw-r--r--   0        0        0     1179 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/freemocap_component_data.py
--rw-r--r--   0        0        0     1901 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/freemocap_data_paths.py
--rw-r--r--   0        0        0     2201 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/freemocap_data_stats.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/mediapipe_names/__init__.py
--rw-r--r--   0        0        0     5533 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/mediapipe_names/mediapipe_heirarchy.py
--rw-r--r--   0        0        0     4434 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/mediapipe_names/mediapipe_trajectory_names.py
--rw-r--r--   0        0        0      828 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/mediapipe_names/virtual_trajectories.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.304159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/parameter_models/__init__.py
--rw-r--r--   0        0        0      652 2023-12-12 01:50:57.308159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/parameter_models/default_parameters.json
--rw-r--r--   0        0        0     1132 2023-12-12 01:50:57.308159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/parameter_models/load_parameters_config.py
--rw-r--r--   0        0        0     1197 2023-12-12 01:50:57.308159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/parameter_models/parameter_models.py
--rw-r--r--   0        0        0     2423 2023-12-12 01:50:57.308159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/run_as_main.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.308159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/system/__init__.py
--rw-r--r--   0        0        0        0 2023-12-12 01:50:57.308159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/system/configure_logging/__init__.py
--rw-r--r--   0        0        0     6838 2023-12-12 01:50:57.308159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/system/configure_logging/configure_logging.py
--rw-r--r--   0        0        0     1115 2023-12-12 01:50:57.308159 ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/system/configure_logging/utilities.py
--rw-r--r--   0        0        0   235277 2023-12-12 01:50:57.308159 ajc27_freemocap_blender_addon-2023.10.1016/body_mesh.ply
--rw-r--r--   0        0        0      241 2023-12-12 01:50:57.308159 ajc27_freemocap_blender_addon-2023.10.1016/poetry.lock
--rw-r--r--   0        0        0      931 2023-12-12 01:50:57.308159 ajc27_freemocap_blender_addon-2023.10.1016/pyproject.toml
--rw-r--r--   0        0        0     1176 1970-01-01 00:00:00.000000 ajc27_freemocap_blender_addon-2023.10.1016/PKG-INFO
+-rw-r--r--   0        0        0     1114 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/.github/workflows/flit_publish_to_pypi.yml
+-rw-r--r--   0        0        0     1113 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/.github/workflows/publish_to_pypi_on_version_bump.yml
+-rw-r--r--   0        0        0     1871 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/.gitignore
+-rw-r--r--   0        0        0    34523 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/LICENSE
+-rw-r--r--   0        0        0      693 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/README.md
+-rw-r--r--   0        0        0      176 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/.idea/.gitignore
+-rw-r--r--   0        0        0      441 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/.idea/ajc27_freemocap_blender_addon.iml
+-rw-r--r--   0        0        0      174 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      278 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/.idea/misc.xml
+-rw-r--r--   0        0        0      310 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/.idea/modules.xml
+-rw-r--r--   0        0        0      183 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/.idea/vcs.xml
+-rw-r--r--   0        0        0     2870 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/__init__.py
+-rw-r--r--   0        0        0   235277 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/assets/body_mesh.ply
+-rw-r--r--   0        0        0    44734 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/assets/charuco_board.png
+-rw-r--r--   0        0        0    44729 2024-04-25 16:27:55.573934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/assets/freemocap_logo_white_outline.png
+-rw-r--r--   0        0        0   705884 2024-04-25 16:27:55.577934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/assets/skelly_lowpoly_mesh.fbx
+-rw-r--r--   0        0        0      511 2024-04-25 16:27:55.577934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/__init__.py
+-rw-r--r--   0        0        0     7989 2024-04-25 16:27:55.577934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/main_view3d_panel.py
+-rw-r--r--   0        0        0     1742 2024-04-25 16:27:55.577934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/__init__.py
+-rw-r--r--   0        0        0     2532 2024-04-25 16:27:55.577934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_add_body_mesh.py
+-rw-r--r--   0        0        0     2675 2024-04-25 16:27:55.577934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_add_rig.py
+-rw-r--r--   0        0        0      359 2024-04-25 16:27:55.577934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_clear_scene.py
+-rw-r--r--   0        0        0      849 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_create_video.py
+-rw-r--r--   0        0        0      398 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_download_sample_data.py
+-rw-r--r--   0        0        0     1094 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_export_fbx.py
+-rw-r--r--   0        0        0     2027 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_load_freemocap_data.py
+-rw-r--r--   0        0        0      670 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_load_videos.py
+-rw-r--r--   0        0        0     1615 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_reduce_bone_length_dispersion.py
+-rw-r--r--   0        0        0      954 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_reduce_shakiness.py
+-rw-r--r--   0        0        0     2320 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_reorient_empties.py
+-rw-r--r--   0        0        0     1388 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_run_all.py
+-rw-r--r--   0        0        0     1463 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_save_out_data.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/properties/__init__.py
+-rw-r--r--   0        0        0     6418 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/properties/properties.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/sub_panels/__init__.py
+-rw-r--r--   0        0        0      881 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/sub_panels/video_export_panel.py
+-rw-r--r--   0        0        0       67 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/__init__.py
+-rw-r--r--   0        0        0     1263 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/create_video.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/__init__.py
+-rw-r--r--   0        0        0     1390 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/add_render_background.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/__init__.py
+-rw-r--r--   0        0        0      303 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/frame_information_dataclass.py
+-rw-r--r--   0        0        0     1240 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/frame_number_overlay.py
+-rw-r--r--   0        0        0     3029 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/image_overlays.py
+-rw-r--r--   0        0        0     3542 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/json_table_overlays.py
+-rw-r--r--   0        0        0    18216 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/overlay_components/matplotlib_plot_overlays.py
+-rw-r--r--   0        0        0      941 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/rearrange_background_videos.py
+-rw-r--r--   0        0        0     2657 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/create_video/helpers/save_video.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/creation/__init__.py
+-rw-r--r--   0        0        0     2041 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/creation/create_empty_from_trajectory.py
+-rw-r--r--   0        0        0     2272 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/creation/create_freemocap_empties.py
+-rw-r--r--   0        0        0     4187 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/creation/create_virtual_trajectories.py
+-rw-r--r--   0        0        0     4801 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/hands.py
+-rw-r--r--   0        0        0     3578 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/reduce_shakiness.py
+-rw-r--r--   0        0        0     9042 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/reorient_empties.py
+-rw-r--r--   0        0        0     1704 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/translate_empty_and_its_children.py
+-rw-r--r--   0        0        0     3860 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/update_empty_positions.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/fbx_export/__init__.py
+-rw-r--r--   0        0        0    29592 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/fbx_export/fbx.py
+-rw-r--r--   0        0        0     1873 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/fbx_export/get_io_scene_fbx_addon.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/load_videos/__init__.py
+-rw-r--r--   0        0        0     3094 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/load_videos/load_videos.py
+-rw-r--r--   0        0        0      905 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/load_videos/rearrange_background_videos.py
+-rw-r--r--   0        0        0    14085 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/main_controller.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/materials/__init__.py
+-rw-r--r--   0        0        0     3319 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/materials/create_checkerboard_material.py
+-rw-r--r--   0        0        0     6136 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/materials/create_material.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/__init__.py
+-rw-r--r--   0        0        0    13248 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/attach_mesh_to_rig.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/center_of_mass/__init__.py
+-rw-r--r--   0        0        0     1379 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/center_of_mass/center_of_mass_mesh.py
+-rw-r--r--   0        0        0     4739 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/center_of_mass/center_of_mass_trails.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/__init__.py
+-rw-r--r--   0        0        0      942 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/create_bone_stick.py
+-rw-r--r--   0        0        0      690 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/get_edit_bones.py
+-rw-r--r--   0        0        0     5051 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/make_bone_mesh.py
+-rw-r--r--   0        0        0      853 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/parent_mesh_to_rig.py
+-rw-r--r--   0        0        0     5222 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/put_meshes_on_empties.py
+-rw-r--r--   0        0        0     1460 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/put_sphere_at_location.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/skelly_mesh/__init__.py
+-rw-r--r--   0        0        0     3448 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/skelly_mesh/attach_skelly_mesh.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/rig/__init__.py
+-rw-r--r--   0        0        0    42581 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/rig/add_rig.py
+-rw-r--r--   0        0        0     5589 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/rig/save_bone_and_joint_angles_from_rig.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/__init__.py
+-rw-r--r--   0        0        0      528 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/clear_scene.py
+-rw-r--r--   0        0        0     1221 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/get_path_to_sample_data.py
+-rw-r--r--   0        0        0      594 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/make_parent_empties.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/cameras/__init__.py
+-rw-r--r--   0        0        0     4046 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/cameras/create_cameras.py
+-rw-r--r--   0        0        0      951 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/create_scene_objects.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/ground_plane/__init__.py
+-rw-r--r--   0        0        0     1553 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/ground_plane/create_ground_plane.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/lights/__init__.py
+-rw-r--r--   0        0        0      894 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/scene_objects/lights/create_lights.py
+-rw-r--r--   0        0        0      316 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/set_start_end_frame.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.581934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/bones/__init__.py
+-rw-r--r--   0        0        0    14652 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/bones/bone_constraints.py
+-rw-r--r--   0        0        0    10402 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/bones/bone_definitions.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/freemocap_data/__init__.py
+-rw-r--r--   0        0        0     9923 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/freemocap_data/freemocap_data_model.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/__init__.py
+-rw-r--r--   0        0        0     1179 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/freemocap_component_data.py
+-rw-r--r--   0        0        0     1874 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/freemocap_data_paths.py
+-rw-r--r--   0        0        0     2201 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/freemocap_data_stats.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/mediapipe_names/__init__.py
+-rw-r--r--   0        0        0     5533 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/mediapipe_names/mediapipe_heirarchy.py
+-rw-r--r--   0        0        0     4434 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/mediapipe_names/mediapipe_trajectory_names.py
+-rw-r--r--   0        0        0      828 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/mediapipe_names/virtual_trajectories.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/parameter_models/__init__.py
+-rw-r--r--   0        0        0      652 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/parameter_models/default_parameters.json
+-rw-r--r--   0        0        0     1132 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/parameter_models/load_parameters_config.py
+-rw-r--r--   0        0        0     1197 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/parameter_models/parameter_models.py
+-rw-r--r--   0        0        0     5284 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/parameter_models/video_config.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/__init__.py
+-rw-r--r--   0        0        0    26905 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/handler.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/helpers/__init__.py
+-rw-r--r--   0        0        0    11082 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/helpers/saver.py
+-rw-r--r--   0        0        0     9328 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/helpers/transformer.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/enforce_rigid_bones/__init__.py
+-rw-r--r--   0        0        0     2987 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/enforce_rigid_bones/calculate_body_dimensions.py
+-rw-r--r--   0        0        0     2093 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/enforce_rigid_bones/calculate_bone_length_statistics.py
+-rw-r--r--   0        0        0     5759 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/enforce_rigid_bones/enforce_rigid_bones.py
+-rw-r--r--   0        0        0     3604 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/estimate_good_frame.py
+-rw-r--r--   0        0        0     6119 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/fix_hand_data.py
+-rw-r--r--   0        0        0      209 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/freemocap_empties_from_parent_object.py
+-rw-r--r--   0        0        0     5587 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/put_skeleton_on_ground.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/utilities/__init__.py
+-rw-r--r--   0        0        0      630 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/utilities/get_or_create_freemocap_data_handler.py
+-rw-r--r--   0        0        0      762 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/utilities/load_data.py
+-rw-r--r--   0        0        0     2424 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/main.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/system/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/system/configure_logging/__init__.py
+-rw-r--r--   0        0        0     6838 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/system/configure_logging/configure_logging.py
+-rw-r--r--   0        0        0     1115 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/system/configure_logging/utilities.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/utilities/__init__.py
+-rw-r--r--   0        0        0     1567 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/utilities/install_dependencies.py
+-rw-r--r--   0        0        0      241 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/poetry.lock
+-rw-r--r--   0        0        0      931 2024-04-25 16:27:55.585934 ajc27_freemocap_blender_addon-2023.10.1017/pyproject.toml
+-rw-r--r--   0        0        0     1176 1970-01-01 00:00:00.000000 ajc27_freemocap_blender_addon-2023.10.1017/PKG-INFO
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/.github/workflows/flit_publish_to_pypi.yml` & `ajc27_freemocap_blender_addon-2023.10.1017/.github/workflows/flit_publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/.github/workflows/publish_to_pypi_on_version_bump.yml` & `ajc27_freemocap_blender_addon-2023.10.1017/.github/workflows/publish_to_pypi_on_version_bump.yml`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/.gitignore` & `ajc27_freemocap_blender_addon-2023.10.1017/.gitignore`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/LICENSE` & `ajc27_freemocap_blender_addon-2023.10.1017/LICENSE`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/README.md` & `ajc27_freemocap_blender_addon-2023.10.1017/README.md`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/__init__.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __author__ = """Skelly FreeMoCap"""
 __email__ = "info@freemocap.org"
-__version__ = "v2023.10.1016"
+__version__ = "v2023.10.1017"
 
 #######################################################################
 ### Add-on to adapt the Freemocap Blender output. It can adjust the
 ### empties position, add a rig and a body mesh. The resulting rig
 ### and animation can be imported in platforms like Unreal Engine.
 ### The rig has a TPose as rest pose for easier retargeting.
 ### For best results, when the script is ran the empties should be
@@ -62,20 +62,20 @@
         bpy.utils.register_class(cls)
 
     print("Registering property group FMC_ADAPTER_PROPERTIES")
 
     from .blender_interface import FMC_ADAPTER_PROPERTIES
     bpy.types.Scene.fmc_adapter_properties = bpy.props.PointerProperty(type=FMC_ADAPTER_PROPERTIES)
 
-    try:
-        from .core_functions.fbx_export.get_io_scene_fbx_addon import get_io_scene_fbx_addon
-        get_io_scene_fbx_addon()
-    except Exception as e:
-        print(f"Error loading io_scene_fbx addon: {str(e)}")
-        raise
+    # try:
+    #     from ajc27_freemocap_blender_addon.core_functions.fbx_export import get_io_scene_fbx_addon
+    #     get_io_scene_fbx_addon()
+    # except Exception as e:
+    #     print(f"Error loading io_scene_fbx addon: {str(e)}")
+    #     raise
 
     print(f"Finished registering {__file__} as add-on!")
 
 
 if __name__ == "__main__":
     print(f"Running {__file__} as main file ")
     register()
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/assets/skelly_lowpoly_mesh.fbx` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/assets/skelly_lowpoly_mesh.fbx`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/main_view3d_panel.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/main_view3d_panel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import logging
 
 from bpy.types import Panel
 
-
-
-import sys
 logger = logging.getLogger(__name__)
 
 
 class VIEW3D_PT_freemocap_adapter(Panel):
     bl_space_type = "VIEW_3D"
     bl_region_type = "UI"
     bl_category = "Freemocap Adapter"
@@ -62,15 +59,15 @@
         box.operator('fmc_adapter._run_all', text='RUN ALL')
 
     def _save_data_to_disk_panel(self, fmc_adapter_tool, layout):
         box = layout.box()
         box.prop(fmc_adapter_tool,
                  "data_parent_empty",
                  text="Data Parent Empty")
-        box.operator('fmc_adapter._save_data_to_disk', text='Save Data to Disk')
+        # box.operator('fmc_adapter._save_data_to_disk', text='Save Data to Disk')
 
     def _fbx_export_panel(self, layout):
         # FBX Export
         fbx_export_box = layout.box()
         fbx_export_box.operator('fmc_adapter._export_fbx', text='5. Export FBX')
 
     def _add_body_mesh_panel(self, fmc_adapter_tool, layout):
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/operators/__init__.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-from ajc27_freemocap_blender_addon.blender_interface.operators._add_body_mesh import FMC_ADAPTER_OT_add_body_mesh
-from ajc27_freemocap_blender_addon.blender_interface.operators._add_rig import FMC_ADAPTER_OT_add_rig
 from ajc27_freemocap_blender_addon.blender_interface.operators._clear_scene import FMC_ADAPTER_clear_scene
-from ajc27_freemocap_blender_addon.blender_interface.operators._export_fbx import FMC_ADAPTER_OT_export_fbx
-from ajc27_freemocap_blender_addon.blender_interface.operators._load_freemocap_data import FMC_ADAPTER_load_freemocap_data
-from ajc27_freemocap_blender_addon.blender_interface.operators._load_videos import FMC_ADAPTER_load_videos
-from ajc27_freemocap_blender_addon.blender_interface.operators._reduce_bone_length_dispersion import \
-    FMC_ADAPTER_OT_reduce_bone_length_dispersion
-from ajc27_freemocap_blender_addon.blender_interface.operators._reduce_shakiness import FMC_ADAPTER_OT_reduce_shakiness
-from ajc27_freemocap_blender_addon.blender_interface.operators._reorient_empties import FMC_ADAPTER_OT_reorient_empties
 from ajc27_freemocap_blender_addon.blender_interface.operators._run_all import FMC_ADAPTER_run_all
-from ajc27_freemocap_blender_addon.blender_interface.operators._save_out_data import FMC_ADAPTER_save_data_to_disk
+
+#
+# from ajc27_freemocap_blender_addon.blender_interface.operators._add_body_mesh import FMC_ADAPTER_OT_add_body_mesh
+# from ajc27_freemocap_blender_addon.blender_interface.operators._add_rig import FMC_ADAPTER_OT_add_rig
+# from ajc27_freemocap_blender_addon.blender_interface.operators._export_fbx import FMC_ADAPTER_OT_export_fbx
+# from ajc27_freemocap_blender_addon.blender_interface.operators._load_freemocap_data import FMC_ADAPTER_load_freemocap_data
+# from ajc27_freemocap_blender_addon.blender_interface.operators._load_videos import FMC_ADAPTER_load_videos
+# from ajc27_freemocap_blender_addon.blender_interface.operators._reduce_bone_length_dispersion import \
+#     FMC_ADAPTER_OT_reduce_bone_length_dispersion
+# from ajc27_freemocap_blender_addon.blender_interface.operators._reduce_shakiness import FMC_ADAPTER_OT_reduce_shakiness
+# from ajc27_freemocap_blender_addon.blender_interface.operators._reorient_empties import FMC_ADAPTER_OT_reorient_empties
+# from ajc27_freemocap_blender_addon.blender_interface.operators._save_out_data import FMC_ADAPTER_save_data_to_disk
 
 BLENDER_OPERATORS = [  # FMC_ADAPTER_download_sample_data,
     FMC_ADAPTER_clear_scene,
     FMC_ADAPTER_run_all,
-    FMC_ADAPTER_save_data_to_disk,
-    FMC_ADAPTER_load_videos,
-    FMC_ADAPTER_load_freemocap_data,
-    FMC_ADAPTER_OT_reorient_empties,
-    FMC_ADAPTER_OT_reduce_bone_length_dispersion,
-    FMC_ADAPTER_OT_reduce_shakiness,
-    FMC_ADAPTER_OT_add_rig,
-    FMC_ADAPTER_OT_add_body_mesh,
-    FMC_ADAPTER_OT_export_fbx,
+    # FMC_ADAPTER_save_data_to_disk,
+    # FMC_ADAPTER_load_videos,
+    # FMC_ADAPTER_load_freemocap_data,
+    # FMC_ADAPTER_OT_reorient_empties,
+    # FMC_ADAPTER_OT_reduce_bone_length_dispersion,
+    # FMC_ADAPTER_OT_reduce_shakiness,
+    # FMC_ADAPTER_OT_add_rig,
+    # FMC_ADAPTER_OT_add_body_mesh,
+    # FMC_ADAPTER_OT_export_fbx,
 ]
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/operators/_add_body_mesh.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_add_body_mesh.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import math as m
 import time
 
 import bpy
+from ajc27_freemocap_blender_addon.core_functions.empties.reorient_empties import reorient_empties
+from ajc27_freemocap_blender_addon.core_functions.meshes.attach_mesh_to_rig import attach_mesh_to_rig
+from ajc27_freemocap_blender_addon.core_functions.rig.add_rig import add_rig
 from bpy.types import Operator
 
-from ...core_functions.meshes.attach_mesh_to_rig import attach_mesh_to_rig
-from ...core_functions.empties.reorient_empties import reorient_empties
-from ...core_functions.rig.add_rig import add_rig
-
 REORIENT_EMPTIES_EXECUTED = True
 
 import logging
 logger = logging.getLogger(__name__)
 
 class FMC_ADAPTER_OT_add_body_mesh(Operator):
     bl_idname = 'fmc_adapter._add_body_mesh'
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/operators/_add_rig.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_add_rig.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging
 import math as m
 import time
 
+from ajc27_freemocap_blender_addon.core_functions.empties.reorient_empties import reorient_empties
+from ajc27_freemocap_blender_addon.core_functions.rig.add_rig import add_rig
 from bpy.types import Operator
 
 from ...blender_interface.operators._add_body_mesh import REORIENT_EMPTIES_EXECUTED
-from ...core_functions.empties.reorient_empties import reorient_empties
-from ...core_functions.freemocap_data_handler.operations.freemocap_empties_from_parent_object import \
+from ...freemocap_data_handler.operations.freemocap_empties_from_parent_object import \
     freemocap_empties_from_parent_object
-from ...core_functions.rig.add_rig import add_rig
 
 logger = logging.getLogger(__name__)
 
 
 class FMC_ADAPTER_OT_add_rig(Operator):
     bl_idname = 'fmc_adapter._add_rig'
     bl_label = 'Freemocap Adapter - Add Rig'
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/operators/_export_fbx.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_export_fbx.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-import logging
 import math as m
 import time
 
+from ajc27_freemocap_blender_addon.core_functions.fbx_export.fbx import export_fbx
 from bpy.types import Operator
 
-from ...core_functions.fbx_export.fbx import export_fbx
-
-import sys
-
 
 class FMC_ADAPTER_OT_export_fbx(Operator):
     bl_idname = 'fmc_adapter._export_fbx'
     bl_label = 'Freemocap Adapter - Export FBX'
     bl_description = 'Exports a FBX file containing the rig, the mesh and the baked animation'
     bl_options = {'REGISTER', 'UNDO_GROUPED'}
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/operators/_load_freemocap_data.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_load_freemocap_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-import logging
 from pathlib import Path
 
-from ...core_functions.empties.creation.create_freemocap_empties import create_freemocap_empties
-from ...core_functions.load_data.load_freemocap_data import load_freemocap_data
-from ...core_functions.setup_scene.make_parent_empties import create_parent_empty
-from ...core_functions.setup_scene.set_start_end_frame import set_start_end_frame
-
-import sys
-
 import bpy
+from ajc27_freemocap_blender_addon.core_functions.empties import create_freemocap_empties
+from ajc27_freemocap_blender_addon.core_functions.setup_scene import create_parent_empty
+from ajc27_freemocap_blender_addon.core_functions.setup_scene import set_start_end_frame
+from ajc27_freemocap_blender_addon.freemocap_data_handler.utilities.load_data import load_freemocap_data
 
 
 class FMC_ADAPTER_load_freemocap_data(bpy.types.Operator):  # , bpy_extras.io_utils.ImportHelper):
     bl_idname = 'fmc_adapter._freemocap_data_operations'
     bl_label = "Load FreeMoCap Data"
     bl_options = {'REGISTER', 'UNDO_GROUPED'}
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/operators/_load_videos.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_load_videos.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-import logging
-
 import bpy
 
-import sys
-
-from ...core_functions.load_data.load_videos import load_videos
+from ajc27_freemocap_blender_addon.core_functions.load_videos.load_videos import load_videos
 
 
 class FMC_ADAPTER_load_videos(bpy.types.Operator):
     bl_idname = 'fmc_adapter._load_videos'
     bl_label = "Load Videos as planes"
     bl_options = {'REGISTER', 'UNDO_GROUPED'}
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/operators/_reduce_bone_length_dispersion.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_reduce_bone_length_dispersion.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-import logging
 import math as m
 import time
 
+from ajc27_freemocap_blender_addon.freemocap_data_handler.operations.enforce_rigid_bones import enforce_rigid_bones
+from ajc27_freemocap_blender_addon.freemocap_data_handler.utilities.load_data import load_freemocap_data
 from bpy.types import Operator
 
-from ...core_functions.bones.enforce_rigid_bones import enforce_rigid_bones
-from ...core_functions.load_data.load_freemocap_data import load_freemocap_data
-
-import sys
-
 
 class FMC_ADAPTER_OT_reduce_bone_length_dispersion(Operator):
     bl_idname = 'fmc_adapter._reduce_bone_length_dispersion'
     bl_label = 'Freemocap Adapter - Reduce Bone Length Dispersion'
     bl_description = 'Reduce the bone length dispersion by moving the tail empty and its children along the bone projection so the bone new length is within the interval'
     bl_options = {'REGISTER', 'UNDO_GROUPED'}
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/operators/_reduce_shakiness.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_reduce_shakiness.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-import logging
 import math as m
 import time
 
+from ajc27_freemocap_blender_addon.core_functions.empties import reduce_shakiness
 from bpy.types import Operator
 
-from ...core_functions.empties.reduce_shakiness import reduce_shakiness
-
-import sys
-
 
 class FMC_ADAPTER_OT_reduce_shakiness(Operator):
     bl_idname = 'fmc_adapter._reduce_shakiness'
     bl_label = 'Freemocap Adapter - Reduce Shakiness'
     bl_description = 'Reduce the shakiness of the capture empties by restricting their acceleration to a defined threshold'
     bl_options = {'REGISTER', 'UNDO_GROUPED'}
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/operators/_reorient_empties.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_reorient_empties.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-import logging
 import math as m
 import time
 
-from bpy.types import Operator
-
-from ...core_functions.empties.reorient_empties import reorient_empties
-from ...core_functions.freemocap_data_handler.operations import \
+from ajc27_freemocap_blender_addon.core_functions.empties.reorient_empties import reorient_empties
+from ajc27_freemocap_blender_addon.freemocap_data_handler.operations import \
     freemocap_empties_from_parent_object
+from bpy.types import Operator
 
 
 class FMC_ADAPTER_OT_reorient_empties(Operator):
     bl_idname = 'fmc_adapter._reorient_empties'
     bl_label = 'Freemocap Adapter - Re-orient Empties'
     bl_description = "Change the position of the freemocap_origin_axes empty to so it is placed in an imaginary ground plane of the capture between the actor's feet"
     bl_options = {'REGISTER', 'UNDO_GROUPED'}
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/operators/_run_all.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_run_all.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-import logging
-from pathlib import Path
 import traceback
+from pathlib import Path
 
 import bpy
 
 
-
-import sys
-
-
 class FMC_ADAPTER_run_all(bpy.types.Operator):
     bl_idname = 'fmc_adapter._run_all'
     bl_label = "Run All"
     bl_options = {'REGISTER', 'UNDO_GROUPED'}
 
     def execute(self, context):
         from ...core_functions.main_controller import MainController
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/operators/_save_out_data.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/operators/_save_out_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-import logging
-
 import bpy
 
-from ...core_functions.freemocap_data_handler.operations.freemocap_empties_from_parent_object import \
+from ajc27_freemocap_blender_addon.freemocap_data_handler.operations import \
     freemocap_empties_from_parent_object
 
 
-import sys
-
-
 class FMC_ADAPTER_save_data_to_disk(bpy.types.Operator):
     bl_idname = 'fmc_adapter._save_data_to_disk'
     bl_label = "Save Data to Disk"
     bl_options = {'REGISTER', 'UNDO_GROUPED'}
 
     def execute(self, context):
         from ...core_functions.main_controller import MainController
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/blender_interface/properties.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/blender_interface/properties/properties.py`

 * *Files 3% similar despite different names*

```diff
@@ -156,7 +156,24 @@
     # Add Body Mesh Options
     body_mesh_mode: bpy.props.EnumProperty(
         name='',
         description='Mode (source) for adding the mesh to the rig',
         items=[('custom', 'custom', ''),
                ('file', 'file', '')]
     )
+
+
+class FMC_VIDEO_EXPORT_PROPERTIES(bpy.types.PropertyGroup):
+    export_profile: bpy.props.EnumProperty(
+        name='',
+        description='Profile of the export video',
+        items=[('debug', 'Debug', ''),
+               ('showcase', 'Showcase', ''),
+               ('scientific', 'Scientific', ''),
+               ],
+    )
+
+    ground_contact_threshold: bpy.props.FloatProperty(
+        name='',
+        default=0.05,
+        description='Ground contact threshold (m)'
+    )
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/bones/calculate_body_dimensions.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/enforce_rigid_bones/calculate_body_dimensions.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/bones/calculate_bone_length_statistics.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/enforce_rigid_bones/calculate_bone_length_statistics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-import logging
 import math
 import statistics
 from typing import Dict, Any
 
 import numpy as np
 
-import sys
-
 
 def calculate_bone_length_statistics(trajectories: Dict[str, np.ndarray],
                                      bones: Dict[str, Dict[str, Any]]):
     print('Calculating bone length statistics...')
 
     # Reset the lengths list for every virtual bone
     for bone in bones:
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/bones/enforce_rigid_bones.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/enforce_rigid_bones/enforce_rigid_bones.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-import logging
 from copy import deepcopy
-from typing import Dict, Any, Tuple
+from typing import Dict, Any
 
 import numpy as np
+from ajc27_freemocap_blender_addon.data_models.bones.bone_definitions import BONE_DEFINITIONS
+from ajc27_freemocap_blender_addon.data_models.mediapipe_names.mediapipe_heirarchy import MEDIAPIPE_HIERARCHY
 
 from .calculate_body_dimensions import calculate_body_dimensions
-from ..bones.calculate_bone_length_statistics import calculate_bone_length_statistics
-from ..freemocap_data_handler.handler import     FreemocapDataHandler
-from ...data_models.bones.bone_definitions import BONE_DEFINITIONS
-from ...data_models.mediapipe_names.mediapipe_heirarchy import MEDIAPIPE_HIERARCHY
-
-import sys
+from ..enforce_rigid_bones.calculate_bone_length_statistics import calculate_bone_length_statistics
+from ...handler import FreemocapDataHandler
 
 
 def enforce_rigid_bones(handler: FreemocapDataHandler,
                         bones: Dict[str, Dict[str, Any]] = BONE_DEFINITIONS) -> FreemocapDataHandler:
     print('Enforcing rigid bones - altering bone lengths to ensure they are the same length on each frame...')
     original_trajectories = handler.trajectories
     updated_trajectories = deepcopy(original_trajectories)
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/empties/creation/create_empty_from_trajectory.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/creation/create_empty_from_trajectory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-import logging
 from typing import List, Union, Dict
 
 import bpy
 import numpy as np
 
-import sys
-
 
 def create_empties(trajectory_frame_marker_xyz: np.ndarray,
                    names_list: Union[List[str], str],
                    empty_scale: float,
                    empty_type: str,
                    parent_object: bpy.types.Object,
                    ) -> Dict[str, bpy.types.Object]:
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/empties/creation/create_freemocap_empties.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/creation/create_freemocap_empties.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-import logging
-
 import bpy
-
+from ajc27_freemocap_blender_addon.freemocap_data_handler.handler import FreemocapDataHandler
 
 from .create_empty_from_trajectory import create_empties
-from ...freemocap_data_handler.handler import FreemocapDataHandler
 
 BODY_EMPTY_SCALE = 0.03
 
 
 def create_freemocap_empties(handler: FreemocapDataHandler,
                              parent_object: bpy.types.Object,
                              center_of_mass_data_parent: bpy.types.Object,
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/empties/creation/create_virtual_trajectories.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/creation/create_virtual_trajectories.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-import logging
 from typing import List, Dict
 
 import numpy as np
-
-from ....data_models.mediapipe_names.virtual_trajectories import MEDIAPIPE_VIRTUAL_TRAJECTORY_DEFINITIONS
-
-import sys
+from ajc27_freemocap_blender_addon.data_models.mediapipe_names.virtual_trajectories import \
+    MEDIAPIPE_VIRTUAL_TRAJECTORY_DEFINITIONS
 
 
 def validate_marker_definitions(virtual_marker_definitions: dict):
     """
     Validate the virtual marker definitions dictionary to ensure that there are the same number of marker names and weights, and that the weights sum to 1
     """
     for virtual_marker_name, virtual_marker_definition in virtual_marker_definitions.items():
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/empties/hands.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/hands.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/empties/reduce_shakiness.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/reduce_shakiness.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/empties/reorient_empties.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/reorient_empties.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/empties/translate_empty_and_its_children.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/translate_empty_and_its_children.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-import logging
 from typing import Tuple, List, Union
 
 import bpy
 import numpy as np
-
-from ...data_models.mediapipe_names.mediapipe_heirarchy import MEDIAPIPE_HIERARCHY
-
-import sys
+from ajc27_freemocap_blender_addon.data_models.mediapipe_names.mediapipe_heirarchy import MEDIAPIPE_HIERARCHY
 
 
 def translate_empty_and_its_children(empty_name: str,
                                      frame_index: int,
                                      delta: Union[List[float], Tuple[float, float, float], np.ndarray]):
     if isinstance(delta, np.ndarray) or isinstance(delta, tuple):
         delta = list(delta)
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/empties/update_empty_positions.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/empties/update_empty_positions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-import logging
 import math as m
 from typing import Dict, Any
 
 import bpy
 
-import sys
-
 EMPTY_VELOCITIES = {}
 EMPTY_POSITIONS = {}
 
 
 def get_empty_positions(empties: Dict[str, bpy.types.Object], ) -> dict[str, dict[str, list[Any]]]:
     print('Updating Empty Positions Dictionary...')
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/fbx_export/fbx.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/fbx_export/fbx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-import logging
 from pathlib import Path
 
 import bpy
 import mathutils
 
-import sys
-
 
 def export_fbx(recording_path: str, ):
     print("Exporting recording to FBX...")
     try:
         # Deselect all
         bpy.ops.object.select_all(action='DESELECT')
 
@@ -450,15 +447,15 @@
             #         object_world_location = current_object.matrix_world.to_translation()
             #         loc = mathutils.Vector((
             #             (object_world_location[0] - asset_world_location[0]) * SCALE_FACTOR,
             #             (object_world_location[1] - asset_world_location[1]) * SCALE_FACTOR,
             #             (object_world_location[2] - asset_world_location[2]) * SCALE_FACTOR
             #         ))
 
-            #         if bpy.context.scene.send2ue.extensions.instance_assets.place_in_active_level:
+            #         if bpy.context.scene.send2ue.extensions.instance_assets.create_in_active_level:
             #             # clear rotation and scale only if spawning actor
             #             # https://github.com/EpicGames/BlenderTools/issues/610
             #             rot = (0, 0, 0)
             #             scale = (1.0 * SCALE_FACTOR, 1.0 * SCALE_FACTOR, 1.0 * SCALE_FACTOR)
             #     else:
             #         loc = mathutils.Vector((0, 0, 0))
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/fbx_export/get_io_scene_fbx_addon.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/fbx_export/get_io_scene_fbx_addon.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-import logging
 import os
 import zipfile
 from importlib.machinery import SourceFileLoader
 from pathlib import Path
 
 import addon_utils
 import bpy
 
-import sys
-
 
 def get_io_scene_fbx_addon():
     print("Checking for io_scene_fbx addon...")
 
     # Your addon name and github repo lik
     addon_name = 'io_scene_fbx'
     github_url = 'https://github.com/Taremin/io_scene_fbx/archive/main.zip'
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/freemocap_data_handler/handler.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import logging
 from copy import deepcopy
 from typing import List, Union, Dict, Any
 
 import numpy as np
+from ajc27_freemocap_blender_addon.core_functions.empties.creation.create_virtual_trajectories import \
+    calculate_virtual_trajectories
+from ajc27_freemocap_blender_addon.data_models.freemocap_data.freemocap_data_model import FreemocapData, \
+    FREEMOCAP_DATA_COMPONENT_TYPES
+from ajc27_freemocap_blender_addon.data_models.freemocap_data.helpers.freemocap_component_data import \
+    FreemocapComponentData
 
 from .operations.estimate_good_frame import estimate_good_frame
-from ..empties.creation.create_virtual_trajectories import calculate_virtual_trajectories
 from ..freemocap_data_handler.helpers.saver import FreemocapDataSaver
 from ..freemocap_data_handler.helpers.transformer import FreemocapDataTransformer
-from ...data_models.freemocap_data.freemocap_data_model import FreemocapData, FREEMOCAP_DATA_COMPONENT_TYPES
-from ...data_models.freemocap_data.helpers.freemocap_component_data import FreemocapComponentData
-
-import sys
 
 
 class FreemocapDataHandler:
     def __init__(self,
                  freemocap_data: FreemocapData):
 
         self.freemocap_data = freemocap_data
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/freemocap_data_handler/helpers/get_or_create_freemocap_data_handler.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/utilities/get_or_create_freemocap_data_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from ..handler import FreemocapDataHandler
+from ajc27_freemocap_blender_addon.freemocap_data_handler.handler import FreemocapDataHandler
 
 FREEMOCAP_DATA_HANDLER = None
 
 
 def get_or_create_freemocap_data_handler(recording_path: str):
     global FREEMOCAP_DATA_HANDLER
     if FREEMOCAP_DATA_HANDLER is None:
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/freemocap_data_handler/helpers/saver.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/helpers/saver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import json
-import logging
 import pickle
 from pathlib import Path
 from typing import Union, TYPE_CHECKING
 
 import numpy as np
 
-import sys
-
 # this allows us to import the `FreemocapDataHandler` class for type hinting without causing a circular import
 if TYPE_CHECKING:
     from ..handler import FreemocapDataHandler
 
 
 class FreemocapDataSaver:
     def __init__(self, handler: "FreemocapDataHandler"):
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/freemocap_data_handler/helpers/transformer.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/helpers/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-import logging
 from typing import List, Union
 from typing import TYPE_CHECKING
 
 import numpy as np
-
-from ....data_models.freemocap_data.freemocap_data_model import (
+from ajc27_freemocap_blender_addon.data_models.freemocap_data.freemocap_data_model import (
     FREEMOCAP_DATA_COMPONENT_TYPES,
 )
 
-import sys
-
 # this allows us to import the `FreemocapDataHandler` class for type hinting without causing a circular import
 if TYPE_CHECKING:
     from ..handler import FreemocapDataHandler
 
 
 class FreemocapDataTransformer:
     def __init__(self, handler: "FreemocapDataHandler"):
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/freemocap_data_handler/operations/estimate_good_frame.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/estimate_good_frame.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/freemocap_data_handler/operations/fix_hand_data.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/fix_hand_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-import logging
 from typing import List, TYPE_CHECKING
 
 import numpy as np
 from numpy import dot
 
 if TYPE_CHECKING:
     from ..handler import FreemocapDataHandler
 
-import sys
-
 
 def fix_hand_data(handler: 'FreemocapDataHandler'):
     """
     fix hand data by...
 
     On each frame:
     1. translate hand data so "right/left_hand_wrist" trajectory (hand data) is on top of the "right/left_wrist" trajectory (body data)
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/freemocap_data_handler/operations/put_skeleton_on_ground.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/operations/put_skeleton_on_ground.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-import logging
 from typing import Dict, TYPE_CHECKING
 
 import numpy as np
 
 from .estimate_good_frame import estimate_good_frame
 
-import sys
-
 if TYPE_CHECKING:
     from ..handler import FreemocapDataHandler
 
 
 def put_skeleton_on_ground(handler: 'FreemocapDataHandler'):
     print(f"Putting freemocap data in inertial reference frame...")
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/load_data/load_freemocap_data.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/freemocap_data_handler/utilities/load_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-import logging
-
-from ..freemocap_data_handler.handler import FreemocapDataHandler
-from ..freemocap_data_handler.helpers.get_or_create_freemocap_data_handler import create_freemocap_data_handler
-
-import sys
+from ajc27_freemocap_blender_addon.freemocap_data_handler.handler import FreemocapDataHandler
+from ajc27_freemocap_blender_addon.freemocap_data_handler.utilities.get_or_create_freemocap_data_handler import create_freemocap_data_handler
 
 
 def load_freemocap_data(
         recording_path: str,
 ) -> FreemocapDataHandler:
     print(f"Loading freemocap_data from {recording_path}....")
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/load_data/load_videos.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/load_videos/load_videos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-import logging
 from pathlib import Path
 from typing import Union
 
 import addon_utils
 import bpy
 import numpy as np
 
 
-import sys
-
-
 def get_video_paths(path_to_video_folder: Path) -> list:
     """Search the folder for 'mp4' files (case insensitive) and return them as a list"""
     print(f"Searching for videos in {path_to_video_folder}")
     list_of_video_paths = list(Path(path_to_video_folder).glob("*.mp4")) + list(
         Path(path_to_video_folder).glob("*.MP4")
     )
     unique_list_of_video_paths = list(set(list_of_video_paths))
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/main_controller.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/main_controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,34 @@
 import traceback
 from pathlib import Path
 from typing import List
 
 import numpy as np
+from ajc27_freemocap_blender_addon.core_functions.load_videos.load_videos import load_videos
+from ajc27_freemocap_blender_addon.core_functions.meshes.attach_mesh_to_rig import attach_mesh_to_rig
+from ajc27_freemocap_blender_addon.core_functions.rig.add_rig import add_rig
+from ajc27_freemocap_blender_addon.freemocap_data_handler.utilities.get_or_create_freemocap_data_handler import (
+    get_or_create_freemocap_data_handler,
+)
+from ajc27_freemocap_blender_addon.freemocap_data_handler.utilities.load_data import load_freemocap_data
 
+from .create_video.create_video import create_video
+from .empties.creation.create_freemocap_empties import create_freemocap_empties
 from .meshes.center_of_mass.center_of_mass_mesh import create_center_of_mass_mesh
 from .meshes.center_of_mass.center_of_mass_trails import create_center_of_mass_trails
 from .meshes.skelly_mesh.attach_skelly_mesh import attach_skelly_mesh_to_rig
 from .rig.save_bone_and_joint_angles_from_rig import save_bone_and_joint_angles_from_rig
-from .video_output.create_video_output import create_video_output
-from ..core_functions.bones.enforce_rigid_bones import enforce_rigid_bones
-from ..core_functions.empties.creation.create_freemocap_empties import (
-    create_freemocap_empties,
-)
-from ..core_functions.freemocap_data_handler.helpers.get_or_create_freemocap_data_handler import (
-    get_or_create_freemocap_data_handler,
-)
-from ..core_functions.freemocap_data_handler.helpers.saver import FreemocapDataSaver
-from ..core_functions.freemocap_data_handler.operations.fix_hand_data import (
-    fix_hand_data,
-)
-from ..core_functions.freemocap_data_handler.operations.put_skeleton_on_ground import (
-    put_skeleton_on_ground,
-)
-from ..core_functions.load_data.load_freemocap_data import load_freemocap_data
-from ..core_functions.load_data.load_videos import load_videos
-from ..core_functions.meshes.attach_mesh_to_rig import attach_mesh_to_rig
-from ..core_functions.rig.add_rig import add_rig
-from ..core_functions.setup_scene.make_parent_empties import (
-    create_parent_empty,
-)
-from ..core_functions.setup_scene.set_start_end_frame import set_start_end_frame
+from .setup_scene.make_parent_empties import create_parent_empty
+from .setup_scene.scene_objects.create_scene_objects import create_scene_objects
+from .setup_scene.set_start_end_frame import set_start_end_frame
 from ..data_models.parameter_models.parameter_models import Config
+from ..freemocap_data_handler.helpers.saver import FreemocapDataSaver
+from ..freemocap_data_handler.operations.enforce_rigid_bones.enforce_rigid_bones import enforce_rigid_bones
+from ..freemocap_data_handler.operations.fix_hand_data import fix_hand_data
+from ..freemocap_data_handler.operations.put_skeleton_on_ground import put_skeleton_on_ground
 
 
 class MainController:
     """
     This class is used to run the program as a main script.
     """
 
@@ -329,18 +322,31 @@
 
         # self.data_parent_object.hide_set(True)
         self._empty_parent_object.hide_set(True)
         self._rigid_body_meshes_parent_object.hide_set(True)
         self._video_parent_object.hide_set(True)
         self._center_of_mass_parent_object.hide_set(True)
 
+        # remove default cube
+        if "Cube" in bpy.data.objects:
+            bpy.data.objects.remove(bpy.data.objects["Cube"])
+
+        # create_scene_objects(scene=bpy.context.scene)
 
-    def create_video_output(self):
+
+    def create_video(self):
+        print("Creating export video...")
         import bpy
-        create_video_output(video_save_path=self.blend_file_path, )
+        create_video(
+            scene=bpy.context.scene,
+            recording_folder=self.recording_path,
+            start_frame=bpy.context.scene.frame_start,
+            end_frame=bpy.context.scene.frame_end,
+        )
+
 
     def save_blender_file(self):
         print("Saving blender file...")
         import bpy
 
         bpy.ops.wm.save_as_mainfile(filepath=str(self.blend_file_path))
         print(f"Saved .blend file to: {self.blend_file_path}")
@@ -362,11 +368,11 @@
         self.save_bone_and_joint_data_from_rig()
         self.attach_rigid_body_mesh_to_rig()
         self.attach_skelly_mesh_to_rig()
         self.create_center_of_mass_mesh()
         # self.create_center_of_mass_trails()
         self.add_videos()
         self.setup_scene()
-        self.create_video_output()
+        # self.create_video()
         self.save_blender_file()
-        # export_fbx(recording_path=recording_path, )
+        # export_fbx(recording_path=recording_path)
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/attach_mesh_to_rig.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/attach_mesh_to_rig.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/center_of_mass/center_of_mass_trails.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/center_of_mass/center_of_mass_trails.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # from typing import Tuple
 from typing import Tuple
 
 import bpy
 import numpy as np
-
 from ajc27_freemocap_blender_addon.core_functions.empties.creation.create_empty_from_trajectory import \
     create_keyframed_empty_from_3d_trajectory_data
-from ajc27_freemocap_blender_addon.core_functions.meshes.rigid_body_meshes.helpers.make_bone_mesh import make_bone_mesh
 
 
 def create_trail_empties(trajectory: np.ndarray,
                          parent_object: bpy.types.Object,
                          tail_past_frames: int,
                          trail_future_frames: int):
     """
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/create_bone_stick.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/create_bone_stick.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/create_material.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/materials/create_material.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/get_edit_bones.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/get_edit_bones.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/make_bone_mesh.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/make_bone_mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import List, Tuple, Union
 
 import bmesh
 import bpy
 import numpy as np
-
-from .create_material import create_material
+from ajc27_freemocap_blender_addon.core_functions.materials.create_material import create_material
 
 
 def make_cone_mesh(name: str = "cone_mesh",
                    color: str = "#00FFFF",
                    emission_strength: float = 1.0,
                    transmittance: float = 0.0,
                    vertices: int = 8,
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/parent_mesh_to_rig.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/parent_mesh_to_rig.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import logging
 import bpy
-import sys
+
+
 def parent_mesh_to_rig(meshes, rig):
     print("Parenting mesh to rig...")
     try:
         meshes[0].name = "mesh"
         # Deselect all
         bpy.ops.object.select_all(action='DESELECT')
         # Select all body meshes
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/put_meshes_on_empties.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/put_meshes_on_empties.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict, Tuple
 
 import bpy
+from ajc27_freemocap_blender_addon.data_models.mediapipe_names.mediapipe_heirarchy import MEDIAPIPE_HIERARCHY
 
-from .make_bone_mesh import     make_bone_mesh
+from .make_bone_mesh import make_bone_mesh
 from .put_sphere_at_location import put_sphere_mesh_at_location
-from .....data_models.mediapipe_names.mediapipe_heirarchy import     MEDIAPIPE_HIERARCHY
 
 
 def create_skeleton_segment_object(child_name: str,
                                    child_empty: bpy.types.Object,
                                    parent_empty: bpy.types.Object,
                                    parent_name: str):
     pass
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/put_sphere_at_location.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/rigid_body_meshes/helpers/put_sphere_at_location.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from typing import Union, List
 
-import numpy as np
-
-from .create_material import create_material
-
 import bpy
+from ajc27_freemocap_blender_addon.core_functions.materials.create_material import create_material
 
 
 def put_sphere_mesh_at_location(
     name: str,
     location: List[float],
     sphere_scale: float = 0.02,
     material: Union[bpy.types.Material, str] = None,
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/meshes/skelly_mesh/attach_skelly_mesh.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/meshes/skelly_mesh/attach_skelly_mesh.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-import math
-from pathlib import Path
 import traceback
+from pathlib import Path
 from typing import Dict
 
 import bpy
-
 from ajc27_freemocap_blender_addon import PACKAGE_ROOT_PATH
-from pathlib import Path
 
 SKELLY_MESH_PATH = str(Path(PACKAGE_ROOT_PATH) / "assets" / "skelly_lowpoly_mesh.fbx")
 
 def attach_skelly_mesh_to_rig(rig: bpy.types.Object,
                               body_dimensions: Dict[str, float],
                               empties: Dict[str, bpy.types.Object],
                               skelly_mesh_path: str = SKELLY_MESH_PATH
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/rig/add_rig.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/rig/add_rig.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import logging
 import math as m
 import re
 from typing import Dict, List
 
 import bpy
 import mathutils
+import addon_utils
 
-from ...data_models.bones.bone_constraints import ALL_BONES_CONSTRAINT_DEFINITIONS
-
-import sys
+from ajc27_freemocap_blender_addon.data_models.bones.bone_constraints import ALL_BONES_CONSTRAINT_DEFINITIONS
 
 
 def add_rig(empty_names: List[str],
             bone_data: Dict[str, Dict[str, float]],
             rig_name: str,
             parent_object: bpy.types.Object,
             keep_symmetry: bool = False,
@@ -20,16 +19,21 @@
             use_limit_rotation: bool = False,
             ) -> bpy.types.Object:
     try:
         # Deselect all objects
         for object in bpy.data.objects:
             object.select_set(False)
 
-        # Add normal human armature
-        bpy.ops.object.armature_human_metarig_add()
+        ensure_rigify()
+
+        try:
+            bpy.ops.object.armature_human_metarig_add()
+        except Exception as e:
+            raise e
+
         # Rename metarig armature to rig_name
         bpy.data.armatures[0].name = rig_name
         # Get reference to armature
         rig = bpy.data.objects['metarig']
         # Rename the rig object to root
         rig.name = rig_name
         rig.data.display_type = 'STICK'
@@ -777,14 +781,30 @@
         bpy.ops.object.select_all(action='DESELECT')
     except Exception as e:
         logging.error(f'{e.__class__} Error while creating the rig: {e}')
         print(e)
         raise e
     return rig
 
+def ensure_rigify():
+    _, rigify_enabled = addon_utils.check("rigify")
+
+    if not rigify_enabled:
+        try:
+            print("Rigify not found - enabling Rigify addon...")
+            addon_utils.enable("rigify", default_set=True, persistent=True, handle_error=print)
+        except Exception as e:
+            print(f"Error enabling Rigify addon - \n\n{e}")
+            raise e
+        
+    _, rigify_enabled = addon_utils.check("rigify")
+
+    if not rigify_enabled:
+        raise Exception("Rigify not enabled, please enable it in your blender preferences and then close blender before retrying")
+
 def get_appended_number(rig_name):
     pattern = r"\.0[0-9]{2}$"
     match = re.search(pattern, rig_name)
     return match.group() if match else None
 
 
 def get_actual_empty_target_name(empty_names:List[str],
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/rig/save_bone_and_joint_angles_from_rig.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/rig/save_bone_and_joint_angles_from_rig.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import csv
 from pathlib import Path
 from typing import Dict
 
 import bpy
-
 from ajc27_freemocap_blender_addon.data_models.bones.bone_constraints import ALL_BONES_CONSTRAINT_DEFINITIONS
 
 
 def save_bone_and_joint_angles_from_rig(rig: bpy.types.Object,
                                         csv_save_path: str,
                                         start_frame: int,
                                         end_frame: int):
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/setup_scene/clear_scene.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/clear_scene.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/setup_scene/get_path_to_sample_data.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/get_path_to_sample_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-import logging
 from pathlib import Path
 
-import sys
-
 
 def get_path_to_sample_data():
     sample_data_path = Path().home() / "freemocap_data" / "recording_sessions" / "freemocap_sample_data"
     sample_data_path = sample_data_path.resolve()
     if not sample_data_path.exists():
         print(
             "Sample data not found. To download sample data, in the main FreeMoCap Gui:"
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/core_functions/setup_scene/make_parent_empties.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/core_functions/setup_scene/make_parent_empties.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/bones/bone_constraints.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/bones/bone_constraints.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/bones/bone_definitions.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/bones/bone_definitions.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/freemocap_data/freemocap_data_model.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/freemocap_data/freemocap_data_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-import logging
 from dataclasses import dataclass
 from typing import Any, Dict, Optional, Union, Literal
 
 import numpy as np
-
 from ajc27_freemocap_blender_addon.core_functions.setup_scene.get_path_to_sample_data import get_path_to_sample_data
+
 from .helpers.freemocap_component_data import FreemocapComponentData
 from .helpers.freemocap_data_paths import FreemocapDataPaths
 from .helpers.freemocap_data_stats import FreemocapDataStats
 from ..mediapipe_names.mediapipe_trajectory_names import MediapipeTrajectoryNames, \
     HumanTrajectoryNames
 
-import sys
-
 FREEMOCAP_DATA_COMPONENT_TYPES = Literal["body", "right_hand", "left_hand", "face", "other"]
 
 
 @dataclass
 class FreemocapData:
     body: FreemocapComponentData
     hands: Dict[str, FreemocapComponentData]
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/freemocap_component_data.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/freemocap_component_data.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/freemocap_data_paths.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/freemocap_data_paths.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-import logging
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Union
 
-import sys
-
 
 @dataclass
 class FreemocapDataPaths:
     body_npy: str
     right_hand_npy: str
     left_hand_npy: str
     face_npy: str
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/freemocap_data_stats.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/freemocap_data/helpers/freemocap_data_stats.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/mediapipe_names/mediapipe_heirarchy.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/mediapipe_names/mediapipe_heirarchy.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/mediapipe_names/mediapipe_trajectory_names.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/mediapipe_names/mediapipe_trajectory_names.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/mediapipe_names/virtual_trajectories.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/mediapipe_names/virtual_trajectories.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/parameter_models/default_parameters.json` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/parameter_models/default_parameters.json`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/parameter_models/load_parameters_config.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/parameter_models/load_parameters_config.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/data_models/parameter_models/parameter_models.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/data_models/parameter_models/parameter_models.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/run_as_main.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,7 +50,8 @@
             blender_file_save_path_input = recording_path_input / (recording_path_input.stem + ".blend")
 
         print(f"Running {__file__} with recording_path={recording_path_input}")
         ajc27_run_as_main_function(recording_path=str(recording_path_input),
                                    blend_file_path=str(blender_file_save_path_input))
     except Exception as e:
         print(f"ERROR RUNNING {__file__}: \n\n GOT ERROR \n\n {str(e)}")
+
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/system/configure_logging/configure_logging.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/system/configure_logging/configure_logging.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/ajc27_freemocap_blender_addon/system/configure_logging/utilities.py` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/system/configure_logging/utilities.py`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/body_mesh.ply` & `ajc27_freemocap_blender_addon-2023.10.1017/ajc27_freemocap_blender_addon/assets/body_mesh.ply`

 * *Files identical despite different names*

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/pyproject.toml` & `ajc27_freemocap_blender_addon-2023.10.1017/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 [project.urls]
 Homepage = "https://freemocap.org"
 Documentation = "https://freemocap.github.io/documentation/"
 Github = "https://github.com/freemocap/ajc27_freemocap_blender_addon"
 
 
 [tool.bumpver]
-current_version = "v2023.10.1016"
+current_version = "v2023.10.1017"
 
 version_pattern = "vMAJOR.MINOR.PATCH[-TAG]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = true
 [tool.bumpver.file_patterns]
```

### Comparing `ajc27_freemocap_blender_addon-2023.10.1016/PKG-INFO` & `ajc27_freemocap_blender_addon-2023.10.1017/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ajc27_freemocap_blender_addon
-Version: 2023.10.1016
+Version: 2023.10.1017
 Summary: A Blender Add-on for working with Freemocap Data (based on @ajc27's addon)
 Author-email: Skelly FreeMoCap <info@freemocap.org>
 Requires-Python: >=3.9,<3.12
 Description-Content-Type: text/markdown
 Project-URL: Documentation, https://freemocap.github.io/documentation/
 Project-URL: Github, https://github.com/freemocap/ajc27_freemocap_blender_addon
 Project-URL: Homepage, https://freemocap.org
```


# Comparing `tmp/orchid_python_api-5.24.0.tar.gz` & `tmp/orchid_python_api-5.24.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchid_python_api-5.24.0.tar", max compression
+gzip compressed data, was "orchid_python_api-5.24.1.tar", max compression
```

## Comparing `orchid_python_api-5.24.0.tar` & `orchid_python_api-5.24.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0     3351 2024-01-15 16:16:25.475075 orchid_python_api-5.24.0/copy_orchid_examples.py
--rw-r--r--   0        0        0     3569 2024-01-15 16:16:25.403712 orchid_python_api-5.24.0/copy_orchid_low_level_examples.py
--rw-r--r--   0        0        0     3551 2024-01-15 16:16:25.436495 orchid_python_api-5.24.0/copy_orchid_manual_examples.py
--rw-r--r--   0        0        0     3375 2024-01-15 16:16:25.462061 orchid_python_api-5.24.0/copy_orchid_tutorials.py
--rw-r--r--   0        0        0    10316 2023-03-30 13:38:52.087989 orchid_python_api-5.24.0/LICENSE
--rw-r--r--   0        0        0     1534 2024-01-15 16:10:51.465929 orchid_python_api-5.24.0/orchid/__init__.py
--rw-r--r--   0        0        0      701 2024-01-15 16:10:51.338615 orchid_python_api-5.24.0/orchid/__version__.py
--rw-r--r--   0        0        0     1046 2024-01-15 16:16:25.478587 orchid_python_api-5.24.0/orchid/base.py
--rw-r--r--   0        0        0     3737 2024-01-15 16:16:25.400712 orchid_python_api-5.24.0/orchid/base_time_series_adapter.py
--rw-r--r--   0        0        0     6788 2024-01-15 16:10:51.718410 orchid_python_api-5.24.0/orchid/configuration.py
--rw-r--r--   0        0        0     1796 2024-01-15 16:16:25.093921 orchid_python_api-5.24.0/orchid/convert.py
--rw-r--r--   0        0        0     6507 2024-01-15 16:10:51.143950 orchid_python_api-5.24.0/orchid/core.py
--rw-r--r--   0        0        0     1151 2024-01-15 16:16:25.346947 orchid_python_api-5.24.0/orchid/dom_project_object.py
--rw-r--r--   0        0        0     2394 2024-01-15 16:10:51.106281 orchid_python_api-5.24.0/orchid/dot_net.py
--rw-r--r--   0        0        0     2126 2024-01-15 16:16:25.293795 orchid_python_api-5.24.0/orchid/dot_net_disposable.py
--rw-r--r--   0        0        0    10259 2024-01-15 16:10:51.382652 orchid_python_api-5.24.0/orchid/dot_net_dom_access.py
--rw-r--r--   0        0        0     1386 2024-01-15 16:16:25.447538 orchid_python_api-5.24.0/orchid/measurement.py
--rw-r--r--   0        0        0     8393 2024-01-15 16:16:25.308825 orchid_python_api-5.24.0/orchid/native_data_frame_adapter.py
--rw-r--r--   0        0        0     2771 2024-01-15 16:16:25.250092 orchid_python_api-5.24.0/orchid/native_monitor_adapter.py
--rw-r--r--   0        0        0     6190 2024-01-15 16:10:51.422672 orchid_python_api-5.24.0/orchid/native_project_user_data_adapter.py
--rw-r--r--   0        0        0    30491 2024-01-15 16:10:51.152458 orchid_python_api-5.24.0/orchid/native_stage_adapter.py
--rw-r--r--   0        0        0     2064 2024-01-15 16:10:51.227810 orchid_python_api-5.24.0/orchid/native_stage_part_adapter.py
--rw-r--r--   0        0        0     2593 2024-01-15 16:16:25.298309 orchid_python_api-5.24.0/orchid/native_subsurface_point.py
--rw-r--r--   0        0        0     2068 2024-01-15 16:10:51.741950 orchid_python_api-5.24.0/orchid/native_time_series_adapter.py
--rw-r--r--   0        0        0    10583 2024-01-15 16:10:51.267749 orchid_python_api-5.24.0/orchid/native_trajectory_adapter.py
--rw-r--r--   0        0        0     7435 2024-01-15 16:16:25.285147 orchid_python_api-5.24.0/orchid/native_treatment_calculations.py
--rw-r--r--   0        0        0     2496 2024-01-15 16:10:51.417641 orchid_python_api-5.24.0/orchid/native_treatment_curve_adapter.py
--rw-r--r--   0        0        0     5404 2024-01-15 16:10:51.278857 orchid_python_api-5.24.0/orchid/native_well_adapter.py
--rw-r--r--   0        0        0    10765 2024-01-15 16:16:25.197417 orchid_python_api-5.24.0/orchid/net_date_time.py
--rw-r--r--   0        0        0     2285 2024-01-15 16:16:25.491608 orchid_python_api-5.24.0/orchid/net_enumerable.py
--rw-r--r--   0        0        0     2091 2024-01-15 16:16:25.016332 orchid_python_api-5.24.0/orchid/net_fracture_diagnostics_factory.py
--rw-r--r--   0        0        0    27111 2024-01-15 16:10:51.121385 orchid_python_api-5.24.0/orchid/net_quantity.py
--rw-r--r--   0        0        0     2411 2024-01-15 16:10:51.180294 orchid_python_api-5.24.0/orchid/net_stage_qc.py
--rw-r--r--   0        0        0     1146 2024-01-15 16:16:25.424274 orchid_python_api-5.24.0/orchid/physical_quantity.py
--rw-r--r--   0        0        0     7029 2024-01-15 16:10:51.252393 orchid_python_api-5.24.0/orchid/project.py
--rw-r--r--   0        0        0    12458 2024-01-15 16:10:51.304350 orchid_python_api-5.24.0/orchid/project_store.py
--rw-r--r--   0        0        0     1417 2024-01-15 16:16:25.389178 orchid_python_api-5.24.0/orchid/reference_origins.py
--rw-r--r--   0        0        0     2931 2024-01-15 16:16:25.103434 orchid_python_api-5.24.0/orchid/script_adapter_context.py
--rw-r--r--   0        0        0     1718 2024-01-15 16:16:25.219838 orchid_python_api-5.24.0/orchid/searchable_data_frames.py
--rw-r--r--   0        0        0     7520 2024-01-15 16:16:25.452548 orchid_python_api-5.24.0/orchid/searchable_project_objects.py
--rw-r--r--   0        0        0     2592 2024-01-15 16:16:25.209036 orchid_python_api-5.24.0/orchid/searchable_stage_parts.py
--rw-r--r--   0        0        0     1191 2024-01-15 16:16:25.030649 orchid_python_api-5.24.0/orchid/searchable_stages.py
--rw-r--r--   0        0        0     6514 2024-01-15 16:16:25.246093 orchid_python_api-5.24.0/orchid/unit_system.py
--rw-r--r--   0        0        0     1769 2024-01-15 16:10:51.745936 orchid_python_api-5.24.0/orchid/validation.py
--rw-r--r--   0        0        0        6 2024-01-15 15:49:21.997643 orchid_python_api-5.24.0/orchid/VERSION
--rw-r--r--   0        0        0     1076 2024-01-15 16:10:51.346617 orchid_python_api-5.24.0/orchid/version.py
--rw-r--r--   0        0        0      787 2024-01-15 16:16:25.276163 orchid_python_api-5.24.0/orchid_python_api/__init__.py
--rw-r--r--   0        0        0     6452 2024-01-15 16:10:51.103276 orchid_python_api-5.24.0/orchid_python_api/examples/add_stages.py
--rw-r--r--   0        0        0     4365 2024-01-15 16:16:25.242040 orchid_python_api-5.24.0/orchid_python_api/examples/change_stage_times.py
--rw-r--r--   0        0        0    28645 2024-01-15 16:16:24.995242 orchid_python_api-5.24.0/orchid_python_api/examples/completion_analysis.ipynb
--rw-r--r--   0        0        0    16982 2024-01-15 16:16:25.066607 orchid_python_api-5.24.0/orchid_python_api/examples/completion_analysis.py
--rw-r--r--   0        0        0    11561 2024-01-15 16:16:25.353451 orchid_python_api-5.24.0/orchid_python_api/examples/low_level/add_stages_low.py
--rw-r--r--   0        0        0    31996 2024-01-15 16:16:25.342436 orchid_python_api-5.24.0/orchid_python_api/examples/low_level/auto_pick.ipynb
--rw-r--r--   0        0        0    15869 2024-01-15 16:16:25.204982 orchid_python_api-5.24.0/orchid_python_api/examples/low_level/auto_pick.py
--rw-r--r--   0        0        0    18521 2024-01-15 16:16:25.012302 orchid_python_api-5.24.0/orchid_python_api/examples/low_level/auto_pick_and_create_stage_attribute.py
--rw-r--r--   0        0        0    16083 2024-01-15 16:16:25.411223 orchid_python_api-5.24.0/orchid_python_api/examples/low_level/auto_pick_iterate_example.py
--rw-r--r--   0        0        0     2411 2024-01-15 16:16:25.043671 orchid_python_api-5.24.0/orchid_python_api/examples/low_level/monitor_time_series.py
--rw-r--r--   0        0        0    10060 2024-01-15 16:16:25.062686 orchid_python_api-5.24.0/orchid_python_api/examples/low_level/multi_picking_events.py
--rw-r--r--   0        0        0    21605 2024-01-15 16:16:25.470572 orchid_python_api-5.24.0/orchid_python_api/examples/manual/data_frame_with_guid.ipynb
--rw-r--r--   0        0        0     1338 2024-01-15 16:16:25.053177 orchid_python_api-5.24.0/orchid_python_api/examples/manual/data_frame_with_guid.py
--rw-r--r--   0        0        0     8216 2024-01-15 16:16:25.358978 orchid_python_api-5.24.0/orchid_python_api/examples/plot_time_series.ipynb
--rw-r--r--   0        0        0     4368 2024-01-15 16:16:25.088916 orchid_python_api-5.24.0/orchid_python_api/examples/plot_time_series.py
--rw-r--r--   0        0        0     6962 2024-01-15 16:16:25.048176 orchid_python_api-5.24.0/orchid_python_api/examples/plot_trajectories.ipynb
--rw-r--r--   0        0        0     3064 2024-01-15 16:16:25.379125 orchid_python_api-5.24.0/orchid_python_api/examples/plot_trajectories.py
--rw-r--r--   0        0        0     7212 2024-01-15 16:16:25.443503 orchid_python_api-5.24.0/orchid_python_api/examples/plot_treatment.ipynb
--rw-r--r--   0        0        0     3765 2024-01-15 16:16:25.235036 orchid_python_api-5.24.0/orchid_python_api/examples/plot_treatment.py
--rw-r--r--   0        0        0      561 2023-03-30 13:38:52.090988 orchid_python_api-5.24.0/orchid_python_api/examples/python_api.yaml.example
--rw-r--r--   0        0        0    30834 2023-10-13 16:42:45.415979 orchid_python_api-5.24.0/orchid_python_api/examples/pythonnet3/internal_tests.ipynb
--rw-r--r--   0        0        0    18697 2024-01-15 16:16:25.303309 orchid_python_api-5.24.0/orchid_python_api/examples/pythonnet3/internal_tests.py
--rw-r--r--   0        0        0    19486 2023-10-13 16:42:45.329657 orchid_python_api-5.24.0/orchid_python_api/examples/pythonnet3/low_level.ipynb
--rw-r--r--   0        0        0    14296 2024-01-15 16:16:25.386176 orchid_python_api-5.24.0/orchid_python_api/examples/pythonnet3/low_level.py
--rw-r--r--   0        0        0    13201 2024-01-15 16:16:25.003255 orchid_python_api-5.24.0/orchid_python_api/examples/search_data_frames.ipynb
--rw-r--r--   0        0        0     5928 2024-01-15 16:16:25.393198 orchid_python_api-5.24.0/orchid_python_api/examples/search_data_frames.py
--rw-r--r--   0        0        0     8578 2024-01-15 16:16:25.215330 orchid_python_api-5.24.0/orchid_python_api/examples/stage_qc_results.py
--rw-r--r--   0        0        0    12843 2024-01-15 16:16:25.231529 orchid_python_api-5.24.0/orchid_python_api/examples/volume_2_first_response.ipynb
--rw-r--r--   0        0        0     8513 2024-01-15 16:16:25.313826 orchid_python_api-5.24.0/orchid_python_api/examples/volume_2_first_response.py
--rw-r--r--   0        0        0    24046 2024-01-15 16:16:25.080299 orchid_python_api-5.24.0/orchid_python_api/tutorials/dom_navigation_tutorial.ipynb
--rw-r--r--   0        0        0    19127 2024-01-15 16:16:25.257602 orchid_python_api-5.24.0/orchid_python_api/tutorials/dom_navigation_tutorial.py
--rw-r--r--   0        0        0     3645 2024-01-15 16:16:25.349947 orchid_python_api-5.24.0/pyproject.toml
--rw-r--r--   0        0        0    32834 2024-01-15 16:16:25.419276 orchid_python_api-5.24.0/README.md
--rw-r--r--   0        0        0    21404 2024-01-15 15:47:44.048867 orchid_python_api-5.24.0/ReleaseNotes.md
--rw-r--r--   0        0        0    34404 1970-01-01 00:00:00.000000 orchid_python_api-5.24.0/PKG-INFO
+-rw-r--r--   0        0        0     3351 2024-03-07 20:21:22.362733 orchid_python_api-5.24.1/copy_orchid_examples.py
+-rw-r--r--   0        0        0     3569 2024-03-07 20:21:22.361733 orchid_python_api-5.24.1/copy_orchid_low_level_examples.py
+-rw-r--r--   0        0        0     3551 2024-03-07 20:21:22.361733 orchid_python_api-5.24.1/copy_orchid_manual_examples.py
+-rw-r--r--   0        0        0     3375 2024-03-07 20:21:22.361733 orchid_python_api-5.24.1/copy_orchid_tutorials.py
+-rw-r--r--   0        0        0    10316 2023-03-30 13:38:52.087989 orchid_python_api-5.24.1/LICENSE
+-rw-r--r--   0        0        0     1534 2024-03-07 20:21:22.374733 orchid_python_api-5.24.1/orchid/__init__.py
+-rw-r--r--   0        0        0      701 2024-03-07 20:21:22.371733 orchid_python_api-5.24.1/orchid/__version__.py
+-rw-r--r--   0        0        0     1046 2024-03-07 20:21:22.372732 orchid_python_api-5.24.1/orchid/base.py
+-rw-r--r--   0        0        0     3737 2024-03-07 20:21:22.372732 orchid_python_api-5.24.1/orchid/base_time_series_adapter.py
+-rw-r--r--   0        0        0     6788 2024-03-07 20:21:22.372732 orchid_python_api-5.24.1/orchid/configuration.py
+-rw-r--r--   0        0        0     1796 2024-03-07 20:21:22.372732 orchid_python_api-5.24.1/orchid/convert.py
+-rw-r--r--   0        0        0     6507 2024-03-07 20:21:22.372732 orchid_python_api-5.24.1/orchid/core.py
+-rw-r--r--   0        0        0     1151 2024-03-07 20:21:22.373732 orchid_python_api-5.24.1/orchid/dom_project_object.py
+-rw-r--r--   0        0        0     2394 2024-03-07 20:21:22.373732 orchid_python_api-5.24.1/orchid/dot_net.py
+-rw-r--r--   0        0        0     2126 2024-03-07 20:21:22.373732 orchid_python_api-5.24.1/orchid/dot_net_disposable.py
+-rw-r--r--   0        0        0    10259 2024-03-07 20:21:22.373732 orchid_python_api-5.24.1/orchid/dot_net_dom_access.py
+-rw-r--r--   0        0        0     1386 2024-03-07 20:21:22.373732 orchid_python_api-5.24.1/orchid/measurement.py
+-rw-r--r--   0        0        0     8393 2024-03-07 20:21:22.374733 orchid_python_api-5.24.1/orchid/native_data_frame_adapter.py
+-rw-r--r--   0        0        0     2820 2024-03-07 20:21:22.374733 orchid_python_api-5.24.1/orchid/native_monitor_adapter.py
+-rw-r--r--   0        0        0     6190 2024-03-07 20:21:22.375733 orchid_python_api-5.24.1/orchid/native_project_user_data_adapter.py
+-rw-r--r--   0        0        0    30491 2024-03-07 20:21:22.378733 orchid_python_api-5.24.1/orchid/native_stage_adapter.py
+-rw-r--r--   0        0        0     2064 2024-03-07 20:21:22.375733 orchid_python_api-5.24.1/orchid/native_stage_part_adapter.py
+-rw-r--r--   0        0        0     2593 2024-03-07 20:21:22.376733 orchid_python_api-5.24.1/orchid/native_subsurface_point.py
+-rw-r--r--   0        0        0     2068 2024-03-07 20:21:22.376733 orchid_python_api-5.24.1/orchid/native_time_series_adapter.py
+-rw-r--r--   0        0        0    10583 2024-03-07 20:21:22.376733 orchid_python_api-5.24.1/orchid/native_trajectory_adapter.py
+-rw-r--r--   0        0        0     7435 2024-03-07 20:21:22.377734 orchid_python_api-5.24.1/orchid/native_treatment_calculations.py
+-rw-r--r--   0        0        0     2496 2024-03-07 20:21:22.378733 orchid_python_api-5.24.1/orchid/native_treatment_curve_adapter.py
+-rw-r--r--   0        0        0     5404 2024-03-07 20:21:22.378733 orchid_python_api-5.24.1/orchid/native_well_adapter.py
+-rw-r--r--   0        0        0    10765 2024-03-07 20:21:22.378733 orchid_python_api-5.24.1/orchid/net_date_time.py
+-rw-r--r--   0        0        0     2285 2024-03-07 20:21:22.378733 orchid_python_api-5.24.1/orchid/net_enumerable.py
+-rw-r--r--   0        0        0     2091 2024-03-07 20:21:22.378733 orchid_python_api-5.24.1/orchid/net_fracture_diagnostics_factory.py
+-rw-r--r--   0        0        0    27111 2024-03-07 20:21:22.378733 orchid_python_api-5.24.1/orchid/net_quantity.py
+-rw-r--r--   0        0        0     2411 2024-03-07 20:21:22.382733 orchid_python_api-5.24.1/orchid/net_stage_qc.py
+-rw-r--r--   0        0        0     1146 2024-03-07 20:21:22.379733 orchid_python_api-5.24.1/orchid/physical_quantity.py
+-rw-r--r--   0        0        0     7029 2024-03-07 20:21:22.379733 orchid_python_api-5.24.1/orchid/project.py
+-rw-r--r--   0        0        0    12458 2024-03-07 20:21:22.379733 orchid_python_api-5.24.1/orchid/project_store.py
+-rw-r--r--   0        0        0     1417 2024-03-07 20:21:22.379733 orchid_python_api-5.24.1/orchid/reference_origins.py
+-rw-r--r--   0        0        0     2931 2024-03-07 20:21:22.380733 orchid_python_api-5.24.1/orchid/script_adapter_context.py
+-rw-r--r--   0        0        0     1718 2024-03-07 20:21:22.380733 orchid_python_api-5.24.1/orchid/searchable_data_frames.py
+-rw-r--r--   0        0        0     7520 2024-03-07 20:21:22.383733 orchid_python_api-5.24.1/orchid/searchable_project_objects.py
+-rw-r--r--   0        0        0     2592 2024-03-07 20:21:22.380733 orchid_python_api-5.24.1/orchid/searchable_stage_parts.py
+-rw-r--r--   0        0        0     1191 2024-03-07 20:21:22.380733 orchid_python_api-5.24.1/orchid/searchable_stages.py
+-rw-r--r--   0        0        0     6514 2024-03-07 20:21:22.380733 orchid_python_api-5.24.1/orchid/unit_system.py
+-rw-r--r--   0        0        0     1769 2024-03-07 20:21:22.379733 orchid_python_api-5.24.1/orchid/validation.py
+-rw-r--r--   0        0        0        6 2024-04-24 15:04:18.738278 orchid_python_api-5.24.1/orchid/VERSION
+-rw-r--r--   0        0        0     1076 2024-03-07 20:21:22.383733 orchid_python_api-5.24.1/orchid/version.py
+-rw-r--r--   0        0        0      787 2024-03-07 20:21:22.383733 orchid_python_api-5.24.1/orchid_python_api/__init__.py
+-rw-r--r--   0        0        0     6452 2024-03-07 20:21:22.383733 orchid_python_api-5.24.1/orchid_python_api/examples/add_stages.py
+-rw-r--r--   0        0        0     4365 2024-03-07 20:21:22.384734 orchid_python_api-5.24.1/orchid_python_api/examples/change_stage_times.py
+-rw-r--r--   0        0        0    28645 2024-03-07 20:21:22.384734 orchid_python_api-5.24.1/orchid_python_api/examples/completion_analysis.ipynb
+-rw-r--r--   0        0        0    16982 2024-03-07 20:21:22.384734 orchid_python_api-5.24.1/orchid_python_api/examples/completion_analysis.py
+-rw-r--r--   0        0        0    11561 2024-03-07 20:21:22.385734 orchid_python_api-5.24.1/orchid_python_api/examples/low_level/add_stages_low.py
+-rw-r--r--   0        0        0    32026 2024-03-07 20:21:22.385734 orchid_python_api-5.24.1/orchid_python_api/examples/low_level/auto_pick.ipynb
+-rw-r--r--   0        0        0    15899 2024-03-07 20:21:22.385734 orchid_python_api-5.24.1/orchid_python_api/examples/low_level/auto_pick.py
+-rw-r--r--   0        0        0    18561 2024-03-07 20:21:22.385734 orchid_python_api-5.24.1/orchid_python_api/examples/low_level/auto_pick_and_create_stage_attribute.py
+-rw-r--r--   0        0        0    16123 2024-03-07 20:21:22.385734 orchid_python_api-5.24.1/orchid_python_api/examples/low_level/auto_pick_iterate_example.py
+-rw-r--r--   0        0        0     2411 2024-03-07 20:21:22.385734 orchid_python_api-5.24.1/orchid_python_api/examples/low_level/monitor_time_series.py
+-rw-r--r--   0        0        0    10080 2024-03-07 20:21:22.385734 orchid_python_api-5.24.1/orchid_python_api/examples/low_level/multi_picking_events.py
+-rw-r--r--   0        0        0    21605 2024-03-07 20:21:22.386733 orchid_python_api-5.24.1/orchid_python_api/examples/manual/data_frame_with_guid.ipynb
+-rw-r--r--   0        0        0     1338 2024-03-07 20:21:22.386733 orchid_python_api-5.24.1/orchid_python_api/examples/manual/data_frame_with_guid.py
+-rw-r--r--   0        0        0     8216 2024-03-07 20:21:22.386733 orchid_python_api-5.24.1/orchid_python_api/examples/plot_time_series.ipynb
+-rw-r--r--   0        0        0     4368 2024-03-07 20:21:22.387733 orchid_python_api-5.24.1/orchid_python_api/examples/plot_time_series.py
+-rw-r--r--   0        0        0     6962 2024-03-07 20:21:22.387733 orchid_python_api-5.24.1/orchid_python_api/examples/plot_trajectories.ipynb
+-rw-r--r--   0        0        0     3064 2024-03-07 20:21:22.387733 orchid_python_api-5.24.1/orchid_python_api/examples/plot_trajectories.py
+-rw-r--r--   0        0        0     7212 2024-03-07 20:21:22.387733 orchid_python_api-5.24.1/orchid_python_api/examples/plot_treatment.ipynb
+-rw-r--r--   0        0        0     3765 2024-03-07 20:21:22.387733 orchid_python_api-5.24.1/orchid_python_api/examples/plot_treatment.py
+-rw-r--r--   0        0        0      561 2023-03-30 13:38:52.090988 orchid_python_api-5.24.1/orchid_python_api/examples/python_api.yaml.example
+-rw-r--r--   0        0        0    30834 2024-03-07 20:21:22.390734 orchid_python_api-5.24.1/orchid_python_api/examples/pythonnet3/internal_tests.ipynb
+-rw-r--r--   0        0        0    18697 2024-03-07 20:21:22.391734 orchid_python_api-5.24.1/orchid_python_api/examples/pythonnet3/internal_tests.py
+-rw-r--r--   0        0        0    19486 2024-03-07 20:21:22.391734 orchid_python_api-5.24.1/orchid_python_api/examples/pythonnet3/low_level.ipynb
+-rw-r--r--   0        0        0    14296 2024-03-07 20:21:22.391734 orchid_python_api-5.24.1/orchid_python_api/examples/pythonnet3/low_level.py
+-rw-r--r--   0        0        0    13201 2024-03-07 20:21:22.391734 orchid_python_api-5.24.1/orchid_python_api/examples/search_data_frames.ipynb
+-rw-r--r--   0        0        0     5928 2024-03-07 20:21:22.392733 orchid_python_api-5.24.1/orchid_python_api/examples/search_data_frames.py
+-rw-r--r--   0        0        0     8578 2024-03-07 20:21:22.392733 orchid_python_api-5.24.1/orchid_python_api/examples/stage_qc_results.py
+-rw-r--r--   0        0        0    12843 2024-03-07 20:21:22.392733 orchid_python_api-5.24.1/orchid_python_api/examples/volume_2_first_response.ipynb
+-rw-r--r--   0        0        0     8513 2024-03-07 20:21:22.393734 orchid_python_api-5.24.1/orchid_python_api/examples/volume_2_first_response.py
+-rw-r--r--   0        0        0    24046 2024-03-07 20:21:22.393734 orchid_python_api-5.24.1/orchid_python_api/tutorials/dom_navigation_tutorial.ipynb
+-rw-r--r--   0        0        0    19127 2024-03-07 20:21:22.396733 orchid_python_api-5.24.1/orchid_python_api/tutorials/dom_navigation_tutorial.py
+-rw-r--r--   0        0        0     3645 2024-04-24 15:04:18.667123 orchid_python_api-5.24.1/pyproject.toml
+-rw-r--r--   0        0        0    32834 2024-03-07 20:21:22.397734 orchid_python_api-5.24.1/README.md
+-rw-r--r--   0        0        0    22029 2024-04-24 14:29:32.931781 orchid_python_api-5.24.1/ReleaseNotes.md
+-rw-r--r--   0        0        0    34404 1970-01-01 00:00:00.000000 orchid_python_api-5.24.1/PKG-INFO
```

### Comparing `orchid_python_api-5.24.0/copy_orchid_examples.py` & `orchid_python_api-5.24.1/copy_orchid_examples.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/copy_orchid_low_level_examples.py` & `orchid_python_api-5.24.1/copy_orchid_low_level_examples.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/copy_orchid_manual_examples.py` & `orchid_python_api-5.24.1/copy_orchid_manual_examples.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/copy_orchid_tutorials.py` & `orchid_python_api-5.24.1/copy_orchid_tutorials.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/LICENSE` & `orchid_python_api-5.24.1/LICENSE`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/__init__.py` & `orchid_python_api-5.24.1/orchid/__init__.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/__version__.py` & `orchid_python_api-5.24.1/orchid/__version__.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/base.py` & `orchid_python_api-5.24.1/orchid/base.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/base_time_series_adapter.py` & `orchid_python_api-5.24.1/orchid/base_time_series_adapter.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/configuration.py` & `orchid_python_api-5.24.1/orchid/configuration.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/convert.py` & `orchid_python_api-5.24.1/orchid/convert.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/core.py` & `orchid_python_api-5.24.1/orchid/core.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/dom_project_object.py` & `orchid_python_api-5.24.1/orchid/dom_project_object.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/dot_net.py` & `orchid_python_api-5.24.1/orchid/dot_net.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/dot_net_disposable.py` & `orchid_python_api-5.24.1/orchid/dot_net_disposable.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/dot_net_dom_access.py` & `orchid_python_api-5.24.1/orchid/dot_net_dom_access.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/measurement.py` & `orchid_python_api-5.24.1/orchid/measurement.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/native_data_frame_adapter.py` & `orchid_python_api-5.24.1/orchid/native_data_frame_adapter.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/native_monitor_adapter.py` & `orchid_python_api-5.24.1/orchid/native_monitor_adapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,22 +19,22 @@
     dot_net_dom_access as dna,
     dom_project_object as dpo,
     native_time_series_adapter as tsa,
     net_date_time as ndt,
 )
 
 # noinspection PyUnresolvedReferences
-from Orchid.FractureDiagnostics import IMonitor
+from Orchid.FractureDiagnostics.Monitors import ITimeSeriesMonitor
 
 
 class NativeMonitorAdapter(dpo.DomProjectObject):
-    """Adapts a native IMonitor to python."""
-    def __init__(self, net_monitor: IMonitor):
+    """Adapts a native ITimeSeriesMonitor to python."""
+    def __init__(self, net_monitor: ITimeSeriesMonitor):
         """
-        Constructs an instance adapting a .NET IMonitor.
+        Constructs an instance adapting a .NET ITimeSeriesMonitor.
 
         Args:
             net_monitor: The .NET monitor to be adapted.
         """
         super().__init__(net_monitor, orchid.base.constantly(net_monitor.Project))
 
     start_time = dna.transformed_dom_property('start_time', 'The start time of this monitor.',
```

### Comparing `orchid_python_api-5.24.0/orchid/native_project_user_data_adapter.py` & `orchid_python_api-5.24.1/orchid/native_project_user_data_adapter.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/native_stage_adapter.py` & `orchid_python_api-5.24.1/orchid/native_stage_adapter.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/native_stage_part_adapter.py` & `orchid_python_api-5.24.1/orchid/native_stage_part_adapter.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/native_subsurface_point.py` & `orchid_python_api-5.24.1/orchid/native_subsurface_point.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/native_time_series_adapter.py` & `orchid_python_api-5.24.1/orchid/native_time_series_adapter.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/native_trajectory_adapter.py` & `orchid_python_api-5.24.1/orchid/native_trajectory_adapter.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/native_treatment_calculations.py` & `orchid_python_api-5.24.1/orchid/native_treatment_calculations.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/native_treatment_curve_adapter.py` & `orchid_python_api-5.24.1/orchid/native_treatment_curve_adapter.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/native_well_adapter.py` & `orchid_python_api-5.24.1/orchid/native_well_adapter.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/net_date_time.py` & `orchid_python_api-5.24.1/orchid/net_date_time.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/net_enumerable.py` & `orchid_python_api-5.24.1/orchid/net_enumerable.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/net_fracture_diagnostics_factory.py` & `orchid_python_api-5.24.1/orchid/net_fracture_diagnostics_factory.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/net_quantity.py` & `orchid_python_api-5.24.1/orchid/net_quantity.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/net_stage_qc.py` & `orchid_python_api-5.24.1/orchid/net_stage_qc.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/physical_quantity.py` & `orchid_python_api-5.24.1/orchid/physical_quantity.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/project.py` & `orchid_python_api-5.24.1/orchid/project.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/project_store.py` & `orchid_python_api-5.24.1/orchid/project_store.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/reference_origins.py` & `orchid_python_api-5.24.1/orchid/reference_origins.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/script_adapter_context.py` & `orchid_python_api-5.24.1/orchid/script_adapter_context.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/searchable_data_frames.py` & `orchid_python_api-5.24.1/orchid/searchable_data_frames.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/searchable_project_objects.py` & `orchid_python_api-5.24.1/orchid/searchable_project_objects.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/searchable_stage_parts.py` & `orchid_python_api-5.24.1/orchid/searchable_stage_parts.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/searchable_stages.py` & `orchid_python_api-5.24.1/orchid/searchable_stages.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/unit_system.py` & `orchid_python_api-5.24.1/orchid/unit_system.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/validation.py` & `orchid_python_api-5.24.1/orchid/validation.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid/version.py` & `orchid_python_api-5.24.1/orchid/version.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/__init__.py` & `orchid_python_api-5.24.1/orchid_python_api/__init__.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/add_stages.py` & `orchid_python_api-5.24.1/orchid_python_api/examples/add_stages.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/change_stage_times.py` & `orchid_python_api-5.24.1/orchid_python_api/examples/change_stage_times.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/completion_analysis.ipynb` & `orchid_python_api-5.24.1/orchid_python_api/examples/completion_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/completion_analysis.py` & `orchid_python_api-5.24.1/orchid_python_api/examples/completion_analysis.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/low_level/add_stages_low.py` & `orchid_python_api-5.24.1/orchid_python_api/examples/low_level/add_stages_low.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/low_level/auto_pick.ipynb` & `orchid_python_api-5.24.1/orchid_python_api/examples/low_level/auto_pick.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999022777214334%*

 * *Differences: {"'cells'": "{18: {'source': {insert: [(5, '        native_monitor: The .NET `ITimeSeriesMonitor` "*

 * *            "object recording pressures.\\n')], delete: [5]}}, 21: {'source': {insert: [(6, "*

 * *            "'        native_monitor: The .NET `ITimeSeriesMonitor` for this observation.\\n')], "*

 * *            "delete: [6]}}, 22: {'source': {insert: [(5, '        native_monitor: The "*

 * *            "`ITimeSeriesMonitor` whose observations we automatically pick.\\n')], delete: [5]}}}"}*

```diff
@@ -321,15 +321,15 @@
             "outputs": [],
             "source": [
                 "def calculate_stage_part_pressure_samples(native_monitor, stage_part):\n",
                 "    \"\"\"\n",
                 "    Calculate the pressure samples from the monitor for the `stage_part`.\n",
                 "\n",
                 "    Args:\n",
-                "        native_monitor: The .NET `IMonitor` object recording pressures.\n",
+                "        native_monitor: The .NET `ITimeSeriesMonitor` object recording pressures.\n",
                 "        stage_part: The .NET `IStagePart` limiting the monitor times to the stage treatment times.\n",
                 "\n",
                 "    Returns:\n",
                 "        The pressure samples from `native_monitor` for the `stage_part`.\n",
                 "    \"\"\"\n",
                 "    time_range = object_factory.CreateDateTimeOffsetRange(stage_part.StartTime.AddDays(-1),\n",
                 "                                                          stage_part.StopTime.AddDays(1))\n",
@@ -392,15 +392,15 @@
             "source": [
                 "def auto_pick_observation_details(unpicked_observation, native_monitor, stage_part):\n",
                 "    \"\"\"\n",
                 "    Change `unpicked_observation` by adding details to make it a picked observation.\n",
                 "\n",
                 "    Args:\n",
                 "        unpicked_observation: The unpicked observation.\n",
-                "        native_monitor: The .NET `IMonitor` for this observation.\n",
+                "        native_monitor: The .NET `ITimeSeriesMonitor` for this observation.\n",
                 "        stage_part: The .NET `IStagePart` observed by `native_monitor`.\n",
                 "\n",
                 "    Returns:\n",
                 "        The \"picked\" observation with the appropriate details filled in.\n",
                 "    \"\"\"\n",
                 "    # Auto pick observation details to be set\n",
                 "    # - Leak off curve type\n",
@@ -451,15 +451,15 @@
             "outputs": [],
             "source": [
                 "def auto_pick_observations(native_project, native_monitor):\n",
                 "    \"\"\"\n",
                 "        Automatically pick observations for each treatment stage of `native_project` observed by `native_monitor`.\n",
                 "    Args:\n",
                 "        native_project: The `IProject` whose observations are sought.\n",
-                "        native_monitor: The `IMonitor` whose observations we automatically pick.\n",
+                "        native_monitor: The `ITimeSeriesMonitor` whose observations we automatically pick.\n",
                 "\n",
                 "    Returns:\n",
                 "\n",
                 "    \"\"\"\n",
                 "    stage_parts = MonitorExtensions.FindPossiblyVisibleStageParts(native_monitor,\n",
                 "                                                                  native_project.Wells.Items)\n",
                 "\n",
```

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/low_level/auto_pick.py` & `orchid_python_api-5.24.1/orchid_python_api/examples/low_level/auto_pick.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 
 
 def calculate_stage_part_pressure_samples(native_monitor, stage_part):
     """
     Calculate the pressure samples from the monitor for the `stage_part`.
 
     Args:
-        native_monitor: The .NET `IMonitor` object recording pressures.
+        native_monitor: The .NET `ITimeSeriesMonitor` object recording pressures.
         stage_part: The .NET `IStagePart` limiting the monitor times to the stage treatment times.
 
     Returns:
         The pressure samples from `native_monitor` for the `stage_part`.
     """
     time_range = object_factory.CreateDateTimeOffsetRange(stage_part.StartTime.AddDays(-1),
                                                           stage_part.StopTime.AddDays(1))
@@ -202,15 +202,15 @@
 
 def auto_pick_observation_details(unpicked_observation, native_monitor, stage_part):
     """
     Change `unpicked_observation` by adding details to make it a picked observation.
 
     Args:
         unpicked_observation: The unpicked observation.
-        native_monitor: The .NET `IMonitor` for this observation.
+        native_monitor: The .NET `ITimeSeriesMonitor` for this observation.
         stage_part: The .NET `IStagePart` observed by `native_monitor`.
 
     Returns:
         The "picked" observation with the appropriate details filled in.
     """
     # Auto pick observation details to be set
     # - Leak off curve type
@@ -253,15 +253,15 @@
 
 
 def auto_pick_observations(native_project, native_monitor):
     """
         Automatically pick observations for each treatment stage of `native_project` observed by `native_monitor`.
     Args:
         native_project: The `IProject` whose observations are sought.
-        native_monitor: The `IMonitor` whose observations we automatically pick.
+        native_monitor: The `ITimeSeriesMonitor` whose observations we automatically pick.
 
     Returns:
 
     """
     stage_parts = MonitorExtensions.FindPossiblyVisibleStageParts(native_monitor,
                                                                   native_project.Wells.Items)
```

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/low_level/auto_pick_and_create_stage_attribute.py` & `orchid_python_api-5.24.1/orchid_python_api/examples/low_level/auto_pick_and_create_stage_attribute.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 
 
 def calculate_stage_part_pressure_samples(native_monitor, stage_part):
     """
     Calculate the pressure samples from the monitor for the `stage_part`.
 
     Args:
-        native_monitor: The .NET `IMonitor` object recording pressures.
+        native_monitor: The .NET `ITimeSeriesMonitor` object recording pressures.
         stage_part: The .NET `IStagePart` limiting the monitor times to the stage treatment times.
 
     Returns:
         The pressure samples from `native_monitor` for the `stage_part`.
     """
     time_range = object_factory.CreateDateTimeOffsetRange(stage_part.StartTime.AddDays(-1),
                                                           stage_part.StopTime.AddDays(1))
@@ -199,15 +199,15 @@
 
 def auto_pick_observation_details(unpicked_observation, native_monitor, stage_part):
     """
     Change `unpicked_observation` by adding details to make it a picked observation.
 
     Args:
         unpicked_observation: The unpicked observation.
-        native_monitor: The .NET `IMonitor` for this observation.
+        native_monitor: The .NET `ITimeSeriesMonitor` for this observation.
         stage_part: The .NET `IStagePart` observed by `native_monitor`.
 
     Returns:
         The "picked" observation with the appropriate details filled in.
     """
     # Auto pick observation details to be set
     # - Leak off curve type
@@ -254,15 +254,15 @@
 
 
 def auto_pick_observations(native_project, native_monitor):
     """
         Automatically pick observations for each treatment stage of `native_project` observed by `native_monitor`.
     Args:
         native_project: The `IProject` whose observations are sought.
-        native_monitor: The `IMonitor` whose observations we automatically pick.
+        native_monitor: The `ITimeSeriesMonitor` whose observations we automatically pick.
 
     Returns:
 
     """
     observation_set = object_factory.CreateObservationSet(native_project, 'Auto-picked Observation Set3')
 
     wells = native_project.Wells.Items
@@ -326,15 +326,15 @@
 
 
 def is_stage_visible_to_monitor(native_monitor, stage):
     """
     Determine if the stage treatment is visible to the specified monitor.
 
     Args:
-        native_monitor: The .NET `IMonitor` that may "see" the stage treatment.
+        native_monitor: The .NET `ITimeSeriesMonitor` that may "see" the stage treatment.
         stage: The stage of interest.
 
     Returns:
         True if the stage is being treated while the monitor is actively monitoring pressures.
     """
     return stage.StartTime.Ticks > native_monitor.StartTime.Ticks and stage.StopTime.Ticks < native_monitor.StopTime.Ticks
```

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/low_level/auto_pick_iterate_example.py` & `orchid_python_api-5.24.1/orchid_python_api/examples/low_level/auto_pick_iterate_example.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 
 
 def calculate_stage_part_pressure_samples(native_monitor, stage_part):
     """
     Calculate the pressure samples from the monitor for the `stage_part`.
 
     Args:
-        native_monitor: The .NET `IMonitor` object recording pressures.
+        native_monitor: The .NET `ITimeSeriesMonitor` object recording pressures.
         stage_part: The .NET `IStagePart` limiting the monitor times to the stage treatment times.
 
     Returns:
         The pressure samples from `native_monitor` for the `stage_part`.
     """
     time_range = object_factory.CreateDateTimeOffsetRange(stage_part.StartTime.AddDays(-1),
                                                           stage_part.StopTime.AddDays(1))
@@ -195,15 +195,15 @@
 
 def auto_pick_observation_details(unpicked_observation, native_monitor, stage_part):
     """
     Change `unpicked_observation` by adding details to make it a picked observation.
 
     Args:
         unpicked_observation: The unpicked observation.
-        native_monitor: The .NET `IMonitor` for this observation.
+        native_monitor: The .NET `ITimeSeriesMonitor` for this observation.
         stage_part: The .NET `IStagePart` observed by `native_monitor`.
 
     Returns:
         The "picked" observation with the appropriate details filled in.
     """
     # Auto pick observation details to be set
     # - Leak off curve type
@@ -246,15 +246,15 @@
 
 
 def auto_pick_observations(native_project, native_monitor):
     """
         Automatically pick observations for each treatment stage of `native_project` observed by `native_monitor`.
     Args:
         native_project: The `IProject` whose observations are sought.
-        native_monitor: The `IMonitor` whose observations we automatically pick.
+        native_monitor: The `ITimeSeriesMonitor` whose observations we automatically pick.
 
     Returns:
 
     """
     observation_set = object_factory.CreateObservationSet(native_project, 'Auto-picked Observation Set3')
 
     wells = native_project.Wells.Items
@@ -287,15 +287,15 @@
 
 
 def is_stage_visible_to_monitor(native_monitor, stage):
     """
     Determine if the stage treatment is visible to the specified monitor.
 
     Args:
-        native_monitor: The .NET `IMonitor` that may "see" the stage treatment.
+        native_monitor: The .NET `ITimeSeriesMonitor` that may "see" the stage treatment.
         stage: The stage of interest.
 
     Returns:
         True if the stage is being treated while the monitor is actively monitoring pressures.
     """
     return stage.StartTime.Ticks > native_monitor.StartTime.Ticks and stage.StopTime.Ticks < native_monitor.StopTime.Ticks
```

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/low_level/monitor_time_series.py` & `orchid_python_api-5.24.1/orchid_python_api/examples/low_level/monitor_time_series.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/low_level/multi_picking_events.py` & `orchid_python_api-5.24.1/orchid_python_api/examples/low_level/multi_picking_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 
 def multi_pick_observations(native_project, native_monitor):
     """
         Multi-pick observations for each treatment stage of `native_project` observed by `native_monitor`.
     Args:
         native_project: The `IProject` whose observations are sought.
-        native_monitor: The `IMonitor` whose observations we automatically pick.
+        native_monitor: The `ITimeSeriesMonitor` whose observations we automatically pick.
 
     Returns:
 
     """
     observation_set = object_factory.CreateObservationSet(native_project, 'Multi-pick Observation Set')
 
     # Arbitrarily select well, 'Demo_1H'
@@ -128,15 +128,15 @@
 # - `auto_pick_and_create_attributes.py`
 # - `auto_pick_iterate_example.py`
 def is_stage_visible_to_monitor(native_monitor, stage):
     """
     Determine if the stage treatment is visible to the specified monitor.
 
     Args:
-        native_monitor: The .NET `IMonitor` that may "see" the stage treatment.
+        native_monitor: The .NET `ITimeSeriesMonitor` that may "see" the stage treatment.
         stage: The stage of interest.
 
     Returns:
         True if the stage is being treated while the monitor is actively monitoring pressures.
     """
     return (stage.StartTime.Ticks > native_monitor.StartTime.Ticks and
             stage.StopTime.Ticks < native_monitor.StopTime.Ticks)
```

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/manual/data_frame_with_guid.ipynb` & `orchid_python_api-5.24.1/orchid_python_api/examples/manual/data_frame_with_guid.ipynb`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/manual/data_frame_with_guid.py` & `orchid_python_api-5.24.1/orchid_python_api/examples/manual/data_frame_with_guid.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/plot_time_series.ipynb` & `orchid_python_api-5.24.1/orchid_python_api/examples/plot_time_series.ipynb`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/plot_time_series.py` & `orchid_python_api-5.24.1/orchid_python_api/examples/plot_time_series.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/plot_trajectories.ipynb` & `orchid_python_api-5.24.1/orchid_python_api/examples/plot_trajectories.ipynb`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/plot_trajectories.py` & `orchid_python_api-5.24.1/orchid_python_api/examples/plot_trajectories.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/plot_treatment.ipynb` & `orchid_python_api-5.24.1/orchid_python_api/examples/plot_treatment.ipynb`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/plot_treatment.py` & `orchid_python_api-5.24.1/orchid_python_api/examples/plot_treatment.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/python_api.yaml.example` & `orchid_python_api-5.24.1/orchid_python_api/examples/python_api.yaml.example`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/pythonnet3/internal_tests.ipynb` & `orchid_python_api-5.24.1/orchid_python_api/examples/pythonnet3/internal_tests.ipynb`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/pythonnet3/internal_tests.py` & `orchid_python_api-5.24.1/orchid_python_api/examples/pythonnet3/internal_tests.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/pythonnet3/low_level.ipynb` & `orchid_python_api-5.24.1/orchid_python_api/examples/pythonnet3/low_level.ipynb`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/pythonnet3/low_level.py` & `orchid_python_api-5.24.1/orchid_python_api/examples/pythonnet3/low_level.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/search_data_frames.ipynb` & `orchid_python_api-5.24.1/orchid_python_api/examples/search_data_frames.ipynb`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/search_data_frames.py` & `orchid_python_api-5.24.1/orchid_python_api/examples/search_data_frames.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/stage_qc_results.py` & `orchid_python_api-5.24.1/orchid_python_api/examples/stage_qc_results.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/volume_2_first_response.ipynb` & `orchid_python_api-5.24.1/orchid_python_api/examples/volume_2_first_response.ipynb`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/examples/volume_2_first_response.py` & `orchid_python_api-5.24.1/orchid_python_api/examples/volume_2_first_response.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/tutorials/dom_navigation_tutorial.ipynb` & `orchid_python_api-5.24.1/orchid_python_api/tutorials/dom_navigation_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/orchid_python_api/tutorials/dom_navigation_tutorial.py` & `orchid_python_api-5.24.1/orchid_python_api/tutorials/dom_navigation_tutorial.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/pyproject.toml` & `orchid_python_api-5.24.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry>=0.12",]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "orchid-python-api"
-version = "5.24.0"
+version = "5.24.1"
 description = "Defines and implements the Python API for Orchid*. (*Orchid is a mark of KAPPA.)"
 authors = [ "KAPPA. <support@reveal-energy.com>",]
 maintainers = [ "KAPPA. <support@reveal-energy.com>",]
 license = "Apache-2.0"
 readme = "README.md"
 homepage="https://github.com/Reveal-Energy-Services/orchid-python-api"
 repository="https://github.com/Reveal-Energy-Services/orchid-python-api"
```

### Comparing `orchid_python_api-5.24.0/README.md` & `orchid_python_api-5.24.1/README.md`

 * *Files identical despite different names*

### Comparing `orchid_python_api-5.24.0/ReleaseNotes.md` & `orchid_python_api-5.24.1/ReleaseNotes.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,48 @@
 - [ReleaseNotes.md](./ReleaseNotes.md) - The release notes for this project.
 
 Although one can read this document in any text editor since it is simply a text file, consider installing
 the [Python grip utility](https://pypi.org/project/grip/). This application allows one to "render local readme
 files before sending off to GitHub". Although you need not send any of these file to `GitHub`, by using `grip` 
 to render the file, you can much more easily navigate the document links.
 
+### Release notes for 5.24.1
+
+This release is the production release of the Orchid Python API corresponding to Orchid 5.24.1. We have made the necessary
+updates to the Python API to remain compatible with the .NET API.
+
+On the .NET side, we renamed IMonitor to ITimeSeriesMonitor. The necessary updates have been made on the Python API side.
+Additionally, the Shmin property was moved from IWell to IStage. As such, some tests have been updated to accommodate that change.
+
+#### Possible breaking .NET API changes
+
+- None
+
+#### Resolved Issues
+
+- None
+
+#### Features
+
+- None
+
+#### Known Issues
+
+- None
+
 ### Release notes for 5.24.0
 
-This release is the production release of the Orchid Python API corresponding to Orchid 5.24.320. We have made the necessary
+This release is the production release of the Orchid Python API corresponding to Orchid 5.24.0. We have made the necessary
 updates to the Python API to remain compatible with the .NET API.
 
 In addition, we have updated the project to be netcore (semantically, in practice it is just called .NET) compatible. .NET Core is Microsoft's cross platform library.  Everything should behave
 the same way as before, as pythonnet fully supports netcore (albeit with a few workarounds which have been implemented in this release),
 but you may need to install .NET if it's not done already. As a user of Orchid, you should have these libraries pre-installed, but,
 if not, you can find .NET 8 here (https://dotnet.microsoft.com/en-us/download). The latest version of .NET 6 (6.0.26) should be
-fine, but we recommend moving to .NET 8 is possible.
+fine, but we recommend moving to .NET 8 if possible.
 
 #### Possible breaking .NET API changes
 
 - None
 
 #### Resolved Issues
```

### Comparing `orchid_python_api-5.24.0/PKG-INFO` & `orchid_python_api-5.24.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchid-python-api
-Version: 5.24.0
+Version: 5.24.1
 Summary: Defines and implements the Python API for Orchid*. (*Orchid is a mark of KAPPA.)
 Home-page: https://github.com/Reveal-Energy-Services/orchid-python-api
 License: Apache-2.0
 Keywords: Orchid Integration,Fracture Diagnostics
 Author: KAPPA.
 Author-email: support@reveal-energy.com
 Maintainer: KAPPA.
```


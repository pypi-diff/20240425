# Comparing `tmp/rips-2024.3.2.2.tar.gz` & `tmp/rips-2024.3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rips-2024.3.2.2.tar", last modified: Mon Apr 22 09:12:35 2024, max compression
+gzip compressed data, was "rips-2024.3.3.2.tar", last modified: Thu Apr 25 08:32:17 2024, max compression
```

## Comparing `rips-2024.3.2.2.tar` & `rips-2024.3.3.2.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:12:35.393531 rips-2024.3.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-22 08:36:51.000000 rips-2024.3.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-22 08:36:51.000000 rips-2024.3.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-22 09:12:35.393531 rips-2024.3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-22 08:36:51.000000 rips-2024.3.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-22 08:36:51.000000 rips-2024.3.2.2/autoformat_pep8.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-22 08:36:51.000000 rips-2024.3.2.2/create_pip_package.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-22 08:36:51.000000 rips-2024.3.2.2/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-22 08:36:51.000000 rips-2024.3.2.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:12:35.385531 rips-2024.3.2.2/rips/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:12:35.389531 rips-2024.3.2.2/rips/PythonExamples/
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/all_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/all_simulation_wells.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/all_wells.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/alter_wbs_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/case_grid_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/case_grid_group_generated_results.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/case_info_streaming_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/cell_result_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/command_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/create_and_export_stim_plan_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/create_intersection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/create_surface_from_thermal_fracture.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/create_wbs_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/export_contour_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/export_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/export_snapshots.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/export_well_path_completions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/generate_ensemble_of_well_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/generate_ensemble_surface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/generate_ensemble_surface_optimized.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/grid_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/headless_plot_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/import_case_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/import_fractures_on_well.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/import_thermal_fracture_on_well.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/import_well_paths_and_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/input_prop_test_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/input_prop_test_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/instance_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/launch_load_case_snapshot_exit.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/launch_with_commandline_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/load_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/modeled_well_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/modeled_well_path_lateral.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/new_summary_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/open_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/replace_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/save_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/selected_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/selected_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/set_cell_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/set_flow_diagnostics_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/set_grid_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/soil_average_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/soil_average_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/soil_porv_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/soil_porv_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/summary_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/summary_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/surface_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/PythonExamples/view_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44480 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/contour_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:12:35.393531 rips-2024.3.2.2/rips/generated/
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-22 08:43:31.000000 rips-2024.3.2.2/rips/generated/App_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-04-22 08:43:31.000000 rips-2024.3.2.2/rips/generated/App_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-22 08:43:31.000000 rips-2024.3.2.2/rips/generated/Case_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    19104 2024-04-22 08:43:31.000000 rips-2024.3.2.2/rips/generated/Case_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    20675 2024-04-22 08:43:31.000000 rips-2024.3.2.2/rips/generated/Commands_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-22 08:43:31.000000 rips-2024.3.2.2/rips/generated/Commands_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-22 08:43:31.000000 rips-2024.3.2.2/rips/generated/Definitions_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-22 08:43:31.000000 rips-2024.3.2.2/rips/generated/Definitions_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-22 08:43:31.000000 rips-2024.3.2.2/rips/generated/Grid_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-04-22 08:43:31.000000 rips-2024.3.2.2/rips/generated/Grid_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-22 08:43:31.000000 rips-2024.3.2.2/rips/generated/NNCProperties_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-22 08:43:31.000000 rips-2024.3.2.2/rips/generated/NNCProperties_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-22 08:43:31.000000 rips-2024.3.2.2/rips/generated/PdmObject_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15439 2024-04-22 08:43:31.000000 rips-2024.3.2.2/rips/generated/PdmObject_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-22 08:43:31.000000 rips-2024.3.2.2/rips/generated/Project_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-04-22 08:43:31.000000 rips-2024.3.2.2/rips/generated/Project_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-22 08:43:31.000000 rips-2024.3.2.2/rips/generated/Properties_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10631 2024-04-22 08:43:31.000000 rips-2024.3.2.2/rips/generated/Properties_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-22 08:40:18.000000 rips-2024.3.2.2/rips/generated/RiaVersionInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-22 08:43:31.000000 rips-2024.3.2.2/rips/generated/SimulationWell_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-22 08:43:31.000000 rips-2024.3.2.2/rips/generated/SimulationWell_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)   101175 2024-04-22 09:12:27.000000 rips-2024.3.2.2/rips/generated/generated_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/gridcasegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/grpc_retry_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (127)    14943 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    19331 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/pdmobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    11783 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/project.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/resinsight_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/retry_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/simulation_well.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:12:35.393531 rips-2024.3.2.2/rips/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/tests/dataroot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/tests/test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/tests/test_create_well_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/tests/test_grids.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/tests/test_launch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/tests/test_nnc_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/tests/test_object_lifetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/tests/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/tests/test_simulation_wells.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/tests/test_summary_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/tests/test_surfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/tests/test_well_log_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/tests/test_wells.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/tests/test_wells_path_completions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-22 08:36:51.000000 rips-2024.3.2.2/rips/well_log_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:12:35.385531 rips-2024.3.2.2/rips.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-22 09:12:35.000000 rips-2024.3.2.2/rips.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-04-22 09:12:35.000000 rips-2024.3.2.2/rips.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 09:12:35.000000 rips-2024.3.2.2/rips.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 09:12:35.000000 rips-2024.3.2.2/rips.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 09:12:35.000000 rips-2024.3.2.2/rips.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 09:12:35.393531 rips-2024.3.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-22 08:40:18.000000 rips-2024.3.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:32:17.261403 rips-2024.3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-25 07:52:11.000000 rips-2024.3.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-25 07:52:11.000000 rips-2024.3.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-25 08:32:17.261403 rips-2024.3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-25 07:52:11.000000 rips-2024.3.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-25 07:52:11.000000 rips-2024.3.3.2/autoformat_pep8.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-25 07:52:11.000000 rips-2024.3.3.2/create_pip_package.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-25 07:52:11.000000 rips-2024.3.3.2/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 07:52:11.000000 rips-2024.3.3.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:32:17.253403 rips-2024.3.3.2/rips/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:32:17.257403 rips-2024.3.3.2/rips/PythonExamples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/all_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/all_simulation_wells.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/all_wells.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/alter_wbs_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/case_grid_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/case_grid_group_generated_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/case_info_streaming_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/cell_result_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/command_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/create_and_export_stim_plan_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/create_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/create_surface_from_thermal_fracture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/create_wbs_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/export_contour_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/export_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/export_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/export_well_path_completions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/generate_ensemble_of_well_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/generate_ensemble_surface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/generate_ensemble_surface_optimized.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/grid_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/headless_plot_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/import_case_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/import_fractures_on_well.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/import_thermal_fracture_on_well.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/import_well_paths_and_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/input_prop_test_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/input_prop_test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/instance_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/launch_load_case_snapshot_exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/launch_with_commandline_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/load_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/modeled_well_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/modeled_well_path_lateral.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/new_summary_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/open_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/replace_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/save_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/selected_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/selected_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/set_cell_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/set_flow_diagnostics_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/set_grid_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/soil_average_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/soil_average_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/soil_porv_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/soil_porv_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/summary_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/summary_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/surface_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/PythonExamples/view_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44480 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/contour_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:32:17.261403 rips-2024.3.3.2/rips/generated/
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-25 08:03:17.000000 rips-2024.3.3.2/rips/generated/App_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-04-25 08:03:17.000000 rips-2024.3.3.2/rips/generated/App_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-25 08:03:17.000000 rips-2024.3.3.2/rips/generated/Case_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19104 2024-04-25 08:03:17.000000 rips-2024.3.3.2/rips/generated/Case_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20675 2024-04-25 08:03:17.000000 rips-2024.3.3.2/rips/generated/Commands_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-25 08:03:17.000000 rips-2024.3.3.2/rips/generated/Commands_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-25 08:03:17.000000 rips-2024.3.3.2/rips/generated/Definitions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 08:03:17.000000 rips-2024.3.3.2/rips/generated/Definitions_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-25 08:03:17.000000 rips-2024.3.3.2/rips/generated/Grid_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-04-25 08:03:17.000000 rips-2024.3.3.2/rips/generated/Grid_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-25 08:03:17.000000 rips-2024.3.3.2/rips/generated/NNCProperties_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-25 08:03:17.000000 rips-2024.3.3.2/rips/generated/NNCProperties_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-25 08:03:17.000000 rips-2024.3.3.2/rips/generated/PdmObject_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15439 2024-04-25 08:03:17.000000 rips-2024.3.3.2/rips/generated/PdmObject_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-25 08:03:17.000000 rips-2024.3.3.2/rips/generated/Project_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-04-25 08:03:17.000000 rips-2024.3.3.2/rips/generated/Project_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-25 08:03:17.000000 rips-2024.3.3.2/rips/generated/Properties_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10631 2024-04-25 08:03:17.000000 rips-2024.3.3.2/rips/generated/Properties_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-25 08:00:06.000000 rips-2024.3.3.2/rips/generated/RiaVersionInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-25 08:03:18.000000 rips-2024.3.3.2/rips/generated/SimulationWell_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-25 08:03:18.000000 rips-2024.3.3.2/rips/generated/SimulationWell_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101175 2024-04-25 08:32:11.000000 rips-2024.3.3.2/rips/generated/generated_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/gridcasegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/grpc_retry_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14943 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19331 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/pdmobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11783 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/resinsight_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/retry_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/simulation_well.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:32:17.261403 rips-2024.3.3.2/rips/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/tests/dataroot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/tests/test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/tests/test_create_well_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/tests/test_grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/tests/test_launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/tests/test_nnc_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/tests/test_object_lifetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/tests/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/tests/test_simulation_wells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/tests/test_summary_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/tests/test_surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/tests/test_well_log_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/tests/test_wells.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/tests/test_wells_path_completions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-25 07:52:11.000000 rips-2024.3.3.2/rips/well_log_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:32:17.253403 rips-2024.3.3.2/rips.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-25 08:32:17.000000 rips-2024.3.3.2/rips.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-04-25 08:32:17.000000 rips-2024.3.3.2/rips.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:32:17.000000 rips-2024.3.3.2/rips.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 08:32:17.000000 rips-2024.3.3.2/rips.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 08:32:17.000000 rips-2024.3.3.2/rips.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 08:32:17.261403 rips-2024.3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-25 08:00:06.000000 rips-2024.3.3.2/setup.py
```

### Comparing `rips-2024.3.2.2/LICENSE` & `rips-2024.3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/PKG-INFO` & `rips-2024.3.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rips
-Version: 2024.3.2.2
+Version: 2024.3.3.2
 Summary: Python Interface for ResInsight
 Home-page: http://www.resinsight.org
 Author: Ceetron Solutions
 Author-email: info@ceetronsolutions.com
 License: Copyright (C) 2019-     Equinor ASA
         
         ResInsight is free software: you can redistribute it andor modify
```

### Comparing `rips-2024.3.2.2/create_pip_package.txt` & `rips-2024.3.3.2/create_pip_package.txt`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/all_cases.py` & `rips-2024.3.3.2/rips/PythonExamples/all_cases.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/all_simulation_wells.py` & `rips-2024.3.3.2/rips/PythonExamples/all_simulation_wells.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/all_wells.py` & `rips-2024.3.3.2/rips/PythonExamples/all_wells.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/alter_wbs_plot.py` & `rips-2024.3.3.2/rips/PythonExamples/alter_wbs_plot.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/case_grid_group.py` & `rips-2024.3.3.2/rips/PythonExamples/case_grid_group.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/case_grid_group_generated_results.py` & `rips-2024.3.3.2/rips/PythonExamples/case_grid_group_generated_results.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/case_info_streaming_example.py` & `rips-2024.3.3.2/rips/PythonExamples/case_info_streaming_example.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/command_example.py` & `rips-2024.3.3.2/rips/PythonExamples/command_example.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/create_and_export_stim_plan_model.py` & `rips-2024.3.3.2/rips/PythonExamples/create_and_export_stim_plan_model.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/create_intersection.py` & `rips-2024.3.3.2/rips/PythonExamples/create_intersection.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/create_surface_from_thermal_fracture.py` & `rips-2024.3.3.2/rips/PythonExamples/create_surface_from_thermal_fracture.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/create_wbs_plot.py` & `rips-2024.3.3.2/rips/PythonExamples/create_wbs_plot.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/error_handling.py` & `rips-2024.3.3.2/rips/PythonExamples/error_handling.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/export_contour_maps.py` & `rips-2024.3.3.2/rips/PythonExamples/export_contour_maps.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/export_plots.py` & `rips-2024.3.3.2/rips/PythonExamples/export_plots.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/export_snapshots.py` & `rips-2024.3.3.2/rips/PythonExamples/export_snapshots.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/export_well_path_completions.py` & `rips-2024.3.3.2/rips/PythonExamples/export_well_path_completions.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/generate_ensemble_of_well_logs.py` & `rips-2024.3.3.2/rips/PythonExamples/generate_ensemble_of_well_logs.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/generate_ensemble_surface.py` & `rips-2024.3.3.2/rips/PythonExamples/generate_ensemble_surface.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/generate_ensemble_surface_optimized.py` & `rips-2024.3.3.2/rips/PythonExamples/generate_ensemble_surface_optimized.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/grid_information.py` & `rips-2024.3.3.2/rips/PythonExamples/grid_information.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/headless_plot_export.py` & `rips-2024.3.3.2/rips/PythonExamples/headless_plot_export.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/import_case_properties.py` & `rips-2024.3.3.2/rips/PythonExamples/import_case_properties.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/import_fractures_on_well.py` & `rips-2024.3.3.2/rips/PythonExamples/import_fractures_on_well.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/import_thermal_fracture_on_well.py` & `rips-2024.3.3.2/rips/PythonExamples/import_thermal_fracture_on_well.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/import_well_paths_and_logs.py` & `rips-2024.3.3.2/rips/PythonExamples/import_well_paths_and_logs.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/input_prop_test_async.py` & `rips-2024.3.3.2/rips/PythonExamples/input_prop_test_async.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/input_prop_test_sync.py` & `rips-2024.3.3.2/rips/PythonExamples/input_prop_test_sync.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/launch_load_case_snapshot_exit.py` & `rips-2024.3.3.2/rips/PythonExamples/launch_load_case_snapshot_exit.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/load_case.py` & `rips-2024.3.3.2/rips/PythonExamples/load_case.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/modeled_well_path.py` & `rips-2024.3.3.2/rips/PythonExamples/modeled_well_path.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/modeled_well_path_lateral.py` & `rips-2024.3.3.2/rips/PythonExamples/modeled_well_path_lateral.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/open_project.py` & `rips-2024.3.3.2/rips/PythonExamples/open_project.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/save_project.py` & `rips-2024.3.3.2/rips/PythonExamples/save_project.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/selected_cases.py` & `rips-2024.3.3.2/rips/PythonExamples/selected_cases.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/selected_cells.py` & `rips-2024.3.3.2/rips/PythonExamples/selected_cells.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/set_flow_diagnostics_result.py` & `rips-2024.3.3.2/rips/PythonExamples/set_flow_diagnostics_result.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/set_grid_properties.py` & `rips-2024.3.3.2/rips/PythonExamples/set_grid_properties.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/soil_average_async.py` & `rips-2024.3.3.2/rips/PythonExamples/soil_average_async.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/soil_average_sync.py` & `rips-2024.3.3.2/rips/PythonExamples/soil_average_sync.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/soil_porv_async.py` & `rips-2024.3.3.2/rips/PythonExamples/soil_porv_async.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/soil_porv_sync.py` & `rips-2024.3.3.2/rips/PythonExamples/soil_porv_sync.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/summary_vectors.py` & `rips-2024.3.3.2/rips/PythonExamples/summary_vectors.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/surface_import.py` & `rips-2024.3.3.2/rips/PythonExamples/surface_import.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/PythonExamples/view_example.py` & `rips-2024.3.3.2/rips/PythonExamples/view_example.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/__init__.py` & `rips-2024.3.3.2/rips/__init__.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/case.py` & `rips-2024.3.3.2/rips/case.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/contour_map.py` & `rips-2024.3.3.2/rips/contour_map.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/generated/App_pb2.py` & `rips-2024.3.3.2/rips/generated/App_pb2.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/generated/App_pb2_grpc.py` & `rips-2024.3.3.2/rips/generated/App_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/generated/Case_pb2.py` & `rips-2024.3.3.2/rips/generated/Case_pb2.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/generated/Case_pb2_grpc.py` & `rips-2024.3.3.2/rips/generated/Case_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/generated/Commands_pb2.py` & `rips-2024.3.3.2/rips/generated/Commands_pb2.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/generated/Commands_pb2_grpc.py` & `rips-2024.3.3.2/rips/generated/Commands_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/generated/Definitions_pb2.py` & `rips-2024.3.3.2/rips/generated/Definitions_pb2.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/generated/Grid_pb2.py` & `rips-2024.3.3.2/rips/generated/Grid_pb2.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/generated/Grid_pb2_grpc.py` & `rips-2024.3.3.2/rips/generated/Grid_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/generated/NNCProperties_pb2.py` & `rips-2024.3.3.2/rips/generated/NNCProperties_pb2.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/generated/NNCProperties_pb2_grpc.py` & `rips-2024.3.3.2/rips/generated/NNCProperties_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/generated/PdmObject_pb2.py` & `rips-2024.3.3.2/rips/generated/PdmObject_pb2.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/generated/PdmObject_pb2_grpc.py` & `rips-2024.3.3.2/rips/generated/PdmObject_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/generated/Project_pb2.py` & `rips-2024.3.3.2/rips/generated/Project_pb2.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/generated/Project_pb2_grpc.py` & `rips-2024.3.3.2/rips/generated/Project_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/generated/Properties_pb2.py` & `rips-2024.3.3.2/rips/generated/Properties_pb2.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/generated/Properties_pb2_grpc.py` & `rips-2024.3.3.2/rips/generated/Properties_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/generated/RiaVersionInfo.py` & `rips-2024.3.3.2/rips/generated/RiaVersionInfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 #  for more details.
 #
 #  Python version of RiaVersionInfo.h
 #  Just sets version constants
 
 RESINSIGHT_MAJOR_VERSION : str = "2024"
 RESINSIGHT_MINOR_VERSION : str = "03"
-RESINSIGHT_PATCH_VERSION : str = "2"
+RESINSIGHT_PATCH_VERSION : str = "3"
 
 PYTHON_GRPC_PROTOC_VERSION : str = "libprotoc 25.1"
```

### Comparing `rips-2024.3.2.2/rips/generated/SimulationWell_pb2.py` & `rips-2024.3.3.2/rips/generated/SimulationWell_pb2.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/generated/SimulationWell_pb2_grpc.py` & `rips-2024.3.3.2/rips/generated/SimulationWell_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/generated/generated_classes.py` & `rips-2024.3.3.2/rips/generated/generated_classes.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/grid.py` & `rips-2024.3.3.2/rips/grid.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/gridcasegroup.py` & `rips-2024.3.3.2/rips/gridcasegroup.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/grpc_retry_interceptor.py` & `rips-2024.3.3.2/rips/grpc_retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/instance.py` & `rips-2024.3.3.2/rips/instance.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/pdmobject.py` & `rips-2024.3.3.2/rips/pdmobject.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/plot.py` & `rips-2024.3.3.2/rips/plot.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/project.py` & `rips-2024.3.3.2/rips/project.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/retry_policy.py` & `rips-2024.3.3.2/rips/retry_policy.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/simulation_well.py` & `rips-2024.3.3.2/rips/simulation_well.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/tests/conftest.py` & `rips-2024.3.3.2/rips/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/tests/test_cases.py` & `rips-2024.3.3.2/rips/tests/test_cases.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/tests/test_commands.py` & `rips-2024.3.3.2/rips/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/tests/test_create_well_path.py` & `rips-2024.3.3.2/rips/tests/test_create_well_path.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/tests/test_grids.py` & `rips-2024.3.3.2/rips/tests/test_grids.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/tests/test_launch.py` & `rips-2024.3.3.2/rips/tests/test_launch.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/tests/test_nnc_properties.py` & `rips-2024.3.3.2/rips/tests/test_nnc_properties.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/tests/test_object_lifetime.py` & `rips-2024.3.3.2/rips/tests/test_object_lifetime.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/tests/test_project.py` & `rips-2024.3.3.2/rips/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/tests/test_properties.py` & `rips-2024.3.3.2/rips/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/tests/test_simulation_wells.py` & `rips-2024.3.3.2/rips/tests/test_simulation_wells.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/tests/test_summary_cases.py` & `rips-2024.3.3.2/rips/tests/test_summary_cases.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/tests/test_surfaces.py` & `rips-2024.3.3.2/rips/tests/test_surfaces.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/tests/test_well_log_extraction.py` & `rips-2024.3.3.2/rips/tests/test_well_log_extraction.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/tests/test_wells.py` & `rips-2024.3.3.2/rips/tests/test_wells.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/tests/test_wells_path_completions.py` & `rips-2024.3.3.2/rips/tests/test_wells_path_completions.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/view.py` & `rips-2024.3.3.2/rips/view.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips/well_log_plot.py` & `rips-2024.3.3.2/rips/well_log_plot.py`

 * *Files identical despite different names*

### Comparing `rips-2024.3.2.2/rips.egg-info/PKG-INFO` & `rips-2024.3.3.2/rips.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rips
-Version: 2024.3.2.2
+Version: 2024.3.3.2
 Summary: Python Interface for ResInsight
 Home-page: http://www.resinsight.org
 Author: Ceetron Solutions
 Author-email: info@ceetronsolutions.com
 License: Copyright (C) 2019-     Equinor ASA
         
         ResInsight is free software: you can redistribute it andor modify
```

### Comparing `rips-2024.3.2.2/rips.egg-info/SOURCES.txt` & `rips-2024.3.3.2/rips.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/pyedb-0.8.0.tar.gz` & `tmp/pyedb-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyedb-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyedb-0.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyedb-0.8.0.tar` & `pyedb-0.8.1.tar`

### file list

```diff
@@ -1,137 +1,137 @@
--rw-r--r--   0        0        0     1089 2024-04-19 14:58:42.239572 pyedb-0.8.0/LICENSE
--rw-r--r--   0        0        0     5476 2024-04-19 14:58:42.239572 pyedb-0.8.0/README.md
--rw-r--r--   0        0        0     4506 2024-04-19 14:58:42.299572 pyedb-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1520 2024-04-19 14:58:42.299572 pyedb-0.8.0/src/pyedb/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 14:58:42.299572 pyedb-0.8.0/src/pyedb/dotnet/__init__.py
--rw-r--r--   0        0        0    79042 2024-04-19 14:58:42.299572 pyedb-0.8.0/src/pyedb/dotnet/application/Variables.py
--rw-r--r--   0        0        0        0 2024-04-19 14:58:42.299572 pyedb-0.8.0/src/pyedb/dotnet/application/__init__.py
--rw-r--r--   0        0        0     3406 2024-04-19 14:58:42.299572 pyedb-0.8.0/src/pyedb/dotnet/clr_module.py
--rw-r--r--   0        0        0   169971 2024-04-19 14:58:42.299572 pyedb-0.8.0/src/pyedb/dotnet/edb.py
--rw-r--r--   0        0        0       52 2024-04-19 14:58:42.299572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 14:58:42.299572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/cell/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 14:58:42.299572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/cell/hierarchy/__init__.py
--rw-r--r--   0        0        0     3309 2024-04-19 14:58:42.299572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/cell/hierarchy/model.py
--rw-r--r--   0        0        0   103173 2024-04-19 14:58:42.299572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/components.py
--rw-r--r--   0        0        0    33626 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/configuration.py
--rw-r--r--   0        0        0        0 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/definition/__init__.py
--rw-r--r--   0        0        0     6743 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/definition/component_def.py
--rw-r--r--   0        0        0     2029 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/definition/component_model.py
--rw-r--r--   0        0        0     1550 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/definition/definition_obj.py
--rw-r--r--   0        0        0     2476 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/definition/definitions.py
--rw-r--r--   0        0        0     5967 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/definition/package_def.py
--rw-r--r--   0        0        0        0 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/dotnet/__init__.py
--rw-r--r--   0        0        0    37653 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/dotnet/database.py
--rw-r--r--   0        0        0     8904 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/dotnet/layout.py
--rw-r--r--   0        0        0    48320 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/dotnet/primitive.py
--rw-r--r--   0        0        0        0 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/__init__.py
--rw-r--r--   0        0        0    37225 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/components_data.py
--rw-r--r--   0        0        0     4256 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/connectable.py
--rw-r--r--   0        0        0    48425 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/control_file.py
--rw-r--r--   0        0        0     2057 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/design_options.py
--rw-r--r--   0        0        0     1977 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/edbvalue.py
--rw-r--r--   0        0        0    13190 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/hfss_extent_info.py
--rw-r--r--   0        0        0    48944 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/hfss_simulation_setup_data.py
--rw-r--r--   0        0        0    21945 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/layer_data.py
--rw-r--r--   0        0        0     9933 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/nets_data.py
--rw-r--r--   0        0        0    78754 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/padstacks_data.py
--rw-r--r--   0        0        0     9223 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/ports.py
--rw-r--r--   0        0        0    48155 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/primitives_data.py
--rw-r--r--   0        0        0    99967 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/simulation_configuration.py
--rw-r--r--   0        0        0    42354 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/siwave_simulation_setup_data.py
--rw-r--r--   0        0        0    15342 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/sources.py
--rw-r--r--   0        0        0    25287 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/terminals.py
--rw-r--r--   0        0        0     4928 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/utilities.py
--rw-r--r--   0        0        0     3501 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/variables.py
--rw-r--r--   0        0        0     4726 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/general.py
--rw-r--r--   0        0        0        0 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/geometry/__init__.py
--rw-r--r--   0        0        0     1590 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/geometry/point_data.py
--rw-r--r--   0        0        0     2990 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/geometry/polygon_data.py
--rw-r--r--   0        0        0    68343 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/hfss.py
--rw-r--r--   0        0        0    50907 2024-04-19 14:58:42.303572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/layout.py
--rw-r--r--   0        0        0    11798 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/layout_validation.py
--rw-r--r--   0        0        0    44463 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/materials.py
--rw-r--r--   0        0        0    11857 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/net_class.py
--rw-r--r--   0        0        0    43882 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/nets.py
--rw-r--r--   0        0        0     3312 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/obj_base.py
--rw-r--r--   0        0        0    54540 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/padstack.py
--rw-r--r--   0        0        0    61077 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/siwave.py
--rw-r--r--   0        0        0   115375 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/stackup.py
--rw-r--r--   0        0        0       58 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/utilities/__init__.py
--rw-r--r--   0        0        0     2220 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/utilities/heatsink.py
--rw-r--r--   0        0        0    23967 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/dotnet/edb_core/utilities/simulation_setup.py
--rw-r--r--   0        0        0     1931 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/dotnet/sim_setup_data/data/siw_dc_ir_settings.py
--rw-r--r--   0        0        0    14950 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/edb_logger.py
--rw-r--r--   0        0        0      111 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/generic/__init__.py
--rw-r--r--   0        0        0    28956 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/generic/constants.py
--rw-r--r--   0        0        0     7137 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/generic/data_handlers.py
--rw-r--r--   0        0        0     4354 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/generic/design_types.py
--rw-r--r--   0        0        0     3941 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/generic/filesystem.py
--rw-r--r--   0        0        0    43608 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/generic/general_methods.py
--rw-r--r--   0        0        0     4901 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/generic/plot.py
--rw-r--r--   0        0        0    11206 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/generic/process.py
--rw-r--r--   0        0        0     9235 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/generic/settings.py
--rw-r--r--   0        0        0        0 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/bom/__init__.py
--rw-r--r--   0        0        0     1853 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/bom/bom.py
--rw-r--r--   0        0        0     2394 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/bom/bom_item.py
--rw-r--r--   0        0        0     3329 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/bom/characteristics.py
--rw-r--r--   0        0        0     1661 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/bom/refdes.py
--rw-r--r--   0        0        0        0 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/content/__init__.py
--rw-r--r--   0        0        0     1883 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/content/color.py
--rw-r--r--   0        0        0     3187 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/content/content.py
--rw-r--r--   0        0        0     2052 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/content/dictionary_color.py
--rw-r--r--   0        0        0     2026 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/content/dictionary_fill.py
--rw-r--r--   0        0        0     2142 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/content/dictionary_line.py
--rw-r--r--   0        0        0     1546 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/content/entry_color.py
--rw-r--r--   0        0        0     1687 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/content/entry_line.py
--rw-r--r--   0        0        0     1651 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/content/fill.py
--rw-r--r--   0        0        0     1427 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/content/layer_ref.py
--rw-r--r--   0        0        0     3931 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/content/standard_geometries_dictionary.py
--rw-r--r--   0        0        0        0 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/__init__.py
--rw-r--r--   0        0        0     2300 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/assembly_drawing.py
--rw-r--r--   0        0        0     2405 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/cad_data.py
--rw-r--r--   0        0        0     2628 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/component.py
--rw-r--r--   0        0        0     2083 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/drill.py
--rw-r--r--   0        0        0     3023 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/feature.py
--rw-r--r--   0        0        0     2270 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/layer.py
--rw-r--r--   0        0        0     8586 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/layer_feature.py
--rw-r--r--   0        0        0     2042 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/logical_net.py
--rw-r--r--   0        0        0     2197 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/outline.py
--rw-r--r--   0        0        0     5598 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/package.py
--rw-r--r--   0        0        0     2535 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/padstack_def.py
--rw-r--r--   0        0        0     2004 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/padstack_hole_def.py
--rw-r--r--   0        0        0     3866 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/padstack_instance.py
--rw-r--r--   0        0        0     2014 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/padstack_pad_def.py
--rw-r--r--   0        0        0     5044 2024-04-19 14:58:42.307572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/path.py
--rw-r--r--   0        0        0     3640 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/phy_net.py
--rw-r--r--   0        0        0     2124 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/pin.py
--rw-r--r--   0        0        0     8945 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/polygon.py
--rw-r--r--   0        0        0     2781 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/profile.py
--rw-r--r--   0        0        0     2274 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/stackup.py
--rw-r--r--   0        0        0     2717 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/stackup_group.py
--rw-r--r--   0        0        0     1970 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/stackup_layer.py
--rw-r--r--   0        0        0    12590 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/step.py
--rw-r--r--   0        0        0     2143 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_header.py
--rw-r--r--   0        0        0     1797 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/ecad.py
--rw-r--r--   0        0        0     3115 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/ipc2581/ecad/spec.py
--rw-r--r--   0        0        0     2739 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/ipc2581/history_record.py
--rw-r--r--   0        0        0    22685 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/ipc2581/ipc2581.py
--rw-r--r--   0        0        0     2092 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/ipc2581/logistic_header.py
--rw-r--r--   0        0        0        0 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/misc/__init__.py
--rw-r--r--   0        0        0     1759 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/misc/aedtlib_personalib_install.py
--rw-r--r--   0        0        0    12223 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/misc/downloads.py
--rw-r--r--   0        0        0     3315 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/misc/misc.py
--rw-r--r--   0        0        0      301 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/misc/pyedb.runtimeconfig.json
--rw-r--r--   0        0        0        0 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/misc/siw_feature_config/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/misc/siw_feature_config/emc/__init__.py
--rw-r--r--   0        0        0     1560 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/misc/siw_feature_config/emc/component_tags.py
--rw-r--r--   0        0        0     1184 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/misc/siw_feature_config/emc/net_tags.py
--rw-r--r--   0        0        0     1557 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/misc/siw_feature_config/emc/tag_library.py
--rw-r--r--   0        0        0     2521 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/misc/siw_feature_config/emc/xml_generic.py
--rw-r--r--   0        0        0     7389 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/misc/siw_feature_config/emc_rule_checker_settings.py
--rw-r--r--   0        0        0      465 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/misc/utilities.py
--rw-r--r--   0        0        0    66820 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/modeler/geometry_operators.py
--rw-r--r--   0        0        0    11576 2024-04-19 14:58:42.311572 pyedb-0.8.0/src/pyedb/siwave.py
--rw-r--r--   0        0        0     8320 1970-01-01 00:00:00.000000 pyedb-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-25 07:42:45.492631 pyedb-0.8.1/LICENSE
+-rw-r--r--   0        0        0     5476 2024-04-25 07:42:45.492631 pyedb-0.8.1/README.md
+-rw-r--r--   0        0        0     4506 2024-04-25 07:42:45.556630 pyedb-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1520 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/__init__.py
+-rw-r--r--   0        0        0    79042 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/application/Variables.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/application/__init__.py
+-rw-r--r--   0        0        0     3406 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/clr_module.py
+-rw-r--r--   0        0        0   169971 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb.py
+-rw-r--r--   0        0        0       52 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/cell/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/cell/hierarchy/__init__.py
+-rw-r--r--   0        0        0     3309 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/cell/hierarchy/model.py
+-rw-r--r--   0        0        0   102985 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/components.py
+-rw-r--r--   0        0        0    33626 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/configuration.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/definition/__init__.py
+-rw-r--r--   0        0        0     6743 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/definition/component_def.py
+-rw-r--r--   0        0        0     2029 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/definition/component_model.py
+-rw-r--r--   0        0        0     1550 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/definition/definition_obj.py
+-rw-r--r--   0        0        0     2476 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/definition/definitions.py
+-rw-r--r--   0        0        0     5967 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/definition/package_def.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/dotnet/__init__.py
+-rw-r--r--   0        0        0    37653 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/dotnet/database.py
+-rw-r--r--   0        0        0     8904 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/dotnet/layout.py
+-rw-r--r--   0        0        0    48320 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/dotnet/primitive.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/__init__.py
+-rw-r--r--   0        0        0    37225 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/components_data.py
+-rw-r--r--   0        0        0     4256 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/connectable.py
+-rw-r--r--   0        0        0    48425 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/control_file.py
+-rw-r--r--   0        0        0     2057 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/design_options.py
+-rw-r--r--   0        0        0     1977 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/edbvalue.py
+-rw-r--r--   0        0        0    13190 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/hfss_extent_info.py
+-rw-r--r--   0        0        0    48944 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/hfss_simulation_setup_data.py
+-rw-r--r--   0        0        0    21945 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/layer_data.py
+-rw-r--r--   0        0        0     9933 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/nets_data.py
+-rw-r--r--   0        0        0    78754 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/padstacks_data.py
+-rw-r--r--   0        0        0     9223 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/ports.py
+-rw-r--r--   0        0        0    48155 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/primitives_data.py
+-rw-r--r--   0        0        0    99967 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/simulation_configuration.py
+-rw-r--r--   0        0        0    42354 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/siwave_simulation_setup_data.py
+-rw-r--r--   0        0        0    15342 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/sources.py
+-rw-r--r--   0        0        0    25287 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/terminals.py
+-rw-r--r--   0        0        0     4928 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/utilities.py
+-rw-r--r--   0        0        0     3501 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/variables.py
+-rw-r--r--   0        0        0     4726 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/general.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/geometry/__init__.py
+-rw-r--r--   0        0        0     1590 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/geometry/point_data.py
+-rw-r--r--   0        0        0     2990 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/geometry/polygon_data.py
+-rw-r--r--   0        0        0    68343 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/hfss.py
+-rw-r--r--   0        0        0    50907 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/layout.py
+-rw-r--r--   0        0        0    11798 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/layout_validation.py
+-rw-r--r--   0        0        0    44463 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/materials.py
+-rw-r--r--   0        0        0    11857 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/net_class.py
+-rw-r--r--   0        0        0    43882 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/nets.py
+-rw-r--r--   0        0        0     3312 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/obj_base.py
+-rw-r--r--   0        0        0    54540 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/padstack.py
+-rw-r--r--   0        0        0    62356 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/siwave.py
+-rw-r--r--   0        0        0   115372 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/stackup.py
+-rw-r--r--   0        0        0       58 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/utilities/__init__.py
+-rw-r--r--   0        0        0     2220 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/utilities/heatsink.py
+-rw-r--r--   0        0        0    23967 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/utilities/simulation_setup.py
+-rw-r--r--   0        0        0     1931 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/dotnet/sim_setup_data/data/siw_dc_ir_settings.py
+-rw-r--r--   0        0        0    14950 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/edb_logger.py
+-rw-r--r--   0        0        0      111 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/generic/__init__.py
+-rw-r--r--   0        0        0    28956 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/generic/constants.py
+-rw-r--r--   0        0        0     7137 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/generic/data_handlers.py
+-rw-r--r--   0        0        0     4354 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/generic/design_types.py
+-rw-r--r--   0        0        0     3941 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/generic/filesystem.py
+-rw-r--r--   0        0        0    43608 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/generic/general_methods.py
+-rw-r--r--   0        0        0     4901 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/generic/plot.py
+-rw-r--r--   0        0        0    11206 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/generic/process.py
+-rw-r--r--   0        0        0     9220 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/generic/settings.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/bom/__init__.py
+-rw-r--r--   0        0        0     1853 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/bom/bom.py
+-rw-r--r--   0        0        0     2394 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/bom/bom_item.py
+-rw-r--r--   0        0        0     3329 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/bom/characteristics.py
+-rw-r--r--   0        0        0     1661 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/bom/refdes.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/content/__init__.py
+-rw-r--r--   0        0        0     1883 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/content/color.py
+-rw-r--r--   0        0        0     3187 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/content/content.py
+-rw-r--r--   0        0        0     2052 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/content/dictionary_color.py
+-rw-r--r--   0        0        0     2026 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/content/dictionary_fill.py
+-rw-r--r--   0        0        0     2142 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/content/dictionary_line.py
+-rw-r--r--   0        0        0     1546 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/content/entry_color.py
+-rw-r--r--   0        0        0     1687 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/content/entry_line.py
+-rw-r--r--   0        0        0     1651 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/content/fill.py
+-rw-r--r--   0        0        0     1427 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/content/layer_ref.py
+-rw-r--r--   0        0        0     3931 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/content/standard_geometries_dictionary.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/__init__.py
+-rw-r--r--   0        0        0     2300 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/assembly_drawing.py
+-rw-r--r--   0        0        0     2405 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/cad_data.py
+-rw-r--r--   0        0        0     2628 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/component.py
+-rw-r--r--   0        0        0     2083 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/drill.py
+-rw-r--r--   0        0        0     3023 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/feature.py
+-rw-r--r--   0        0        0     2270 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/layer.py
+-rw-r--r--   0        0        0     8586 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/layer_feature.py
+-rw-r--r--   0        0        0     2042 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/logical_net.py
+-rw-r--r--   0        0        0     2197 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/outline.py
+-rw-r--r--   0        0        0     5598 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/package.py
+-rw-r--r--   0        0        0     2535 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/padstack_def.py
+-rw-r--r--   0        0        0     2004 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/padstack_hole_def.py
+-rw-r--r--   0        0        0     3866 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/padstack_instance.py
+-rw-r--r--   0        0        0     2014 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/padstack_pad_def.py
+-rw-r--r--   0        0        0     5044 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/path.py
+-rw-r--r--   0        0        0     3640 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/phy_net.py
+-rw-r--r--   0        0        0     2124 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/pin.py
+-rw-r--r--   0        0        0     8945 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/polygon.py
+-rw-r--r--   0        0        0     2781 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/profile.py
+-rw-r--r--   0        0        0     2274 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/stackup.py
+-rw-r--r--   0        0        0     2717 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/stackup_group.py
+-rw-r--r--   0        0        0     1970 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/stackup_layer.py
+-rw-r--r--   0        0        0    12590 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/step.py
+-rw-r--r--   0        0        0     2143 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_header.py
+-rw-r--r--   0        0        0     1797 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/ecad.py
+-rw-r--r--   0        0        0     3115 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/spec.py
+-rw-r--r--   0        0        0     2739 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/history_record.py
+-rw-r--r--   0        0        0    22685 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ipc2581.py
+-rw-r--r--   0        0        0     2092 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/logistic_header.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/misc/__init__.py
+-rw-r--r--   0        0        0     1759 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/misc/aedtlib_personalib_install.py
+-rw-r--r--   0        0        0    12223 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/misc/downloads.py
+-rw-r--r--   0        0        0     3315 2024-04-25 07:42:45.568630 pyedb-0.8.1/src/pyedb/misc/misc.py
+-rw-r--r--   0        0        0      301 2024-04-25 07:42:45.568630 pyedb-0.8.1/src/pyedb/misc/pyedb.runtimeconfig.json
+-rw-r--r--   0        0        0        0 2024-04-25 07:42:45.568630 pyedb-0.8.1/src/pyedb/misc/siw_feature_config/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:42:45.568630 pyedb-0.8.1/src/pyedb/misc/siw_feature_config/emc/__init__.py
+-rw-r--r--   0        0        0     1560 2024-04-25 07:42:45.568630 pyedb-0.8.1/src/pyedb/misc/siw_feature_config/emc/component_tags.py
+-rw-r--r--   0        0        0     1184 2024-04-25 07:42:45.568630 pyedb-0.8.1/src/pyedb/misc/siw_feature_config/emc/net_tags.py
+-rw-r--r--   0        0        0     1557 2024-04-25 07:42:45.568630 pyedb-0.8.1/src/pyedb/misc/siw_feature_config/emc/tag_library.py
+-rw-r--r--   0        0        0     2521 2024-04-25 07:42:45.568630 pyedb-0.8.1/src/pyedb/misc/siw_feature_config/emc/xml_generic.py
+-rw-r--r--   0        0        0     7389 2024-04-25 07:42:45.568630 pyedb-0.8.1/src/pyedb/misc/siw_feature_config/emc_rule_checker_settings.py
+-rw-r--r--   0        0        0      465 2024-04-25 07:42:45.568630 pyedb-0.8.1/src/pyedb/misc/utilities.py
+-rw-r--r--   0        0        0    66820 2024-04-25 07:42:45.568630 pyedb-0.8.1/src/pyedb/modeler/geometry_operators.py
+-rw-r--r--   0        0        0    11576 2024-04-25 07:42:45.568630 pyedb-0.8.1/src/pyedb/siwave.py
+-rw-r--r--   0        0        0     8320 1970-01-01 00:00:00.000000 pyedb-0.8.1/PKG-INFO
```

### Comparing `pyedb-0.8.0/LICENSE` & `pyedb-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/README.md` & `pyedb-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/pyproject.toml` & `pyedb-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/__init__.py` & `pyedb-0.8.1/src/pyedb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,13 +40,13 @@
 
 
 deprecation_warning()
 
 #
 
 pyedb_path = os.path.dirname(__file__)
-__version__ = "0.8.0"
+__version__ = "0.8.1"
 version = __version__
 
 #
 
 from pyedb.generic.design_types import Edb, Siwave
```

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/application/Variables.py` & `pyedb-0.8.1/src/pyedb/dotnet/application/Variables.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/clr_module.py` & `pyedb-0.8.1/src/pyedb/dotnet/clr_module.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/cell/hierarchy/model.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/cell/hierarchy/model.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/components.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -875,15 +875,15 @@
         net_list : str or list of string.
             List of nets where ports must be created on the component.
             If the net is not part of the component, this parameter is skipped.
         port_type : SourceType enumerator, CoaxPort or CircuitPort
             Type of port to create. ``CoaxPort`` generates solder balls.
             ``CircuitPort`` generates circuit ports on pins belonging to the net list.
         do_pingroup : bool
-            True activate pingroup during port creation (only used with combination of CoaxPort),
+            True activate pingroup during port creation (only used with combination of CircPort),
             False will take the closest reference pin and generate one port per signal pin.
         refnet : string or list of string.
             list of the reference net.
         port_name : str
             Port name for overwriting the default port-naming convention,
             which is ``[component][net][pin]``. The port name must be unique.
             If a port with the specified name already exists, the
@@ -1012,25 +1012,18 @@
                                 return False
                             pin_group_term = self._create_pin_group_terminal(pin_group)
                             if pin_group_term:
                                 pin_group_term.SetReferenceTerminal(ref_pin_group_term)
                     else:
                         self._logger.info("No pins found on component {} for the net {}".format(component, net))
             else:
-                ref_pin_group = self.create_pingroup_from_pins(ref_pins)
-                if not ref_pin_group:
-                    self._logger.warning("failed to create reference pin group")
-                    return False
-                ref_pin_group_term = self._create_pin_group_terminal(ref_pin_group, isref=True)
                 for net in net_list:
                     pins = [pin for pin in cmp_pins if pin.GetNet().GetName() == net]
                     for pin in pins:
-                        pin_group = self.create_pingroup_from_pins([pin])
-                        pin_group_term = self._create_pin_group_terminal(pin_group, isref=False)
-                        pin_group_term.SetReferenceTerminal(ref_pin_group_term)
+                        self.create_port_on_pins(component, pin, ref_pins)
         return True
 
     @pyedb_function_handler()
     def _create_terminal(self, pin, term_name=None):
         """Create terminal on component pin.
 
         Parameters
@@ -1331,39 +1324,46 @@
                 rlc.C = self._edb.utility.value(rlc_values[2])
             rlc.is_parallel = component.is_parallel_rlc
             pos_pin_term.SetRlcBoundaryParameters(rlc)
             self._logger.info("Component {} has been replaced by port".format(component.refdes))
             return True
 
     @pyedb_function_handler()
-    def _create_pin_group_terminal(self, pingroup, isref=False, term_name=None):
+    def _create_pin_group_terminal(self, pingroup, isref=False, term_name=None, term_type="circuit"):
         """Creates an EDB pin group terminal from a given EDB pin group.
 
         Parameters
         ----------
         pingroup : Edb pin group.
 
         isref : bool
+        Specify if this terminal a reference terminal.
 
         term_name : Terminal name (Optional). If not provided default name is Component name, Pin name, Net name.
             str.
 
+        term_type: Type of terminal, gap, circuit or auto.
+        str.
         Returns
         -------
         Edb pin group terminal.
         """
         pin = list(pingroup.GetPins())[0]
         if term_name is None:
             term_name = "{}.{}.{}".format(pin.GetComponent().GetName(), pin.GetName(), pin.GetNet().GetName())
         for t in list(self._pedb.active_layout.Terminals):
             if t.GetName() == term_name:
                 return t
         pingroup_term = self._edb.cell.terminal.PinGroupTerminal.Create(
             self._active_layout, pingroup.GetNet(), term_name, pingroup, isref
         )
+        if term_type == "circuit":
+            pingroup_term.SetIsCircuitPort(True)
+        elif term_type == "auto":
+            pingroup_term.SetIsAutoPort(True)
         return pingroup_term
 
     @pyedb_function_handler()
     def _is_top_component(self, cmp):
         """Test the component placement layer.
 
         Parameters
@@ -2291,15 +2291,15 @@
         ----------
         component : str or EDB component
             Name of the component or the EDB component object.
         netName : str, optional
             Filter on the net name as an alternative to
             ``pinName``. The default is ``None``.
         pinName : str, optional
-            Filter on the pin name an an alternative to
+            Filter on the pin name an alternative to
             ``netName``. The default is ``None``.
 
         Returns
         -------
         list
             List of pins when the component is found or ``[]`` otherwise.
```

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/configuration.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/configuration.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/definition/component_def.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/definition/component_def.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/definition/component_model.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/definition/component_model.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/definition/definition_obj.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/definition/definition_obj.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/definition/definitions.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/definition/definitions.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/definition/package_def.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/definition/package_def.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/dotnet/database.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/dotnet/database.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/dotnet/layout.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/dotnet/layout.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/dotnet/primitive.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/dotnet/primitive.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/components_data.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/components_data.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/connectable.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/connectable.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/control_file.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/control_file.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/design_options.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/design_options.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/edbvalue.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/edbvalue.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/hfss_extent_info.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/hfss_extent_info.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/hfss_simulation_setup_data.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/hfss_simulation_setup_data.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/layer_data.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/layer_data.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/nets_data.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/nets_data.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/padstacks_data.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/padstacks_data.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/ports.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/ports.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/primitives_data.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/primitives_data.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/simulation_configuration.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/simulation_configuration.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/siwave_simulation_setup_data.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/siwave_simulation_setup_data.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/sources.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/sources.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/terminals.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/terminals.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/utilities.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/utilities.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/edb_data/variables.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/variables.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/general.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/general.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/geometry/point_data.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/geometry/point_data.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/geometry/polygon_data.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/geometry/polygon_data.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/hfss.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/hfss.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/layout.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/layout.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/layout_validation.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/layout_validation.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/materials.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/materials.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/net_class.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/net_class.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/nets.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/nets.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/obj_base.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/obj_base.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/padstack.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/padstack.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/siwave.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/siwave.py`

 * *Files 1% similar despite different names*

```diff
@@ -1450,7 +1450,38 @@
             Location of the negative terminal.
         negative_layer : str
             Layer of the negative terminal.
         """
         p_terminal = self._pedb.get_point_terminal(name, positive_net_name, positive_location, positive_layer)
         n_terminal = self._pedb.get_point_terminal(name + "_ref", negative_net_name, negative_location, negative_layer)
         return self._pedb.create_voltage_probe(p_terminal, n_terminal)
+
+    @property
+    def icepak_use_minimal_comp_defaults(self):
+        """Icepak default setting. If "True", only resistor are active in Icepak simulation.
+        The power dissipation of the resistors are calculated from DC results.
+        """
+        siwave_id = self._pedb.edb_api.ProductId.SIWave
+        cell = self._pedb.active_cell._active_cell
+        _, value = cell.GetProductProperty(siwave_id, 422, "")
+        return bool(value)
+
+    @icepak_use_minimal_comp_defaults.setter
+    def icepak_use_minimal_comp_defaults(self, value):
+        value = "True" if bool(value) else ""
+        siwave_id = self._pedb.edb_api.ProductId.SIWave
+        cell = self._pedb.active_cell._active_cell
+        cell.SetProductProperty(siwave_id, 422, value)
+
+    @property
+    def icepak_component_file(self):
+        """Icepak component file path."""
+        siwave_id = self._pedb.edb_api.ProductId.SIWave
+        cell = self._pedb.active_cell._active_cell
+        _, value = cell.GetProductProperty(siwave_id, 420, "")
+        return value
+
+    @icepak_component_file.setter
+    def icepak_component_file(self, value):
+        siwave_id = self._pedb.edb_api.ProductId.SIWave
+        cell = self._pedb.active_cell._active_cell
+        cell.SetProductProperty(siwave_id, 420, value)
```

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/stackup.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/stackup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5840,1372 +5840,1372 @@
 00016cf0: 6220 3d20 4564 6228 290a 2020 2020 2020  b = Edb().      
 00016d00: 2020 3e3e 3e20 6564 622e 7374 6163 6b75    >>> edb.stacku
 00016d10: 702e 696d 706f 7274 5f73 7461 636b 7570  p.import_stackup
 00016d20: 2822 7374 6163 6b75 702e 786d 6c22 290a  ("stackup.xml").
 00016d30: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
 00016d40: 2020 2020 2073 656c 662e 5f6c 6f67 6765       self._logge
 00016d50: 722e 7761 726e 696e 6728 224d 6574 686f  r.warning("Metho
-00016d60: 6420 6578 706f 7274 5f73 7461 636b 7570  d export_stackup
+00016d60: 6420 696d 706f 7274 5f73 7461 636b 7570  d import_stackup
 00016d70: 2069 7320 6465 7072 6563 6174 6564 2e20   is deprecated. 
-00016d80: 5573 6520 2e65 7870 6f72 742e 2229 0a20  Use .export."). 
-00016d90: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00016da0: 6c66 2e6c 6f61 6428 6669 6c65 5f70 6174  lf.load(file_pat
-00016db0: 6829 0a0a 2020 2020 4070 7965 6462 5f66  h)..    @pyedb_f
-00016dc0: 756e 6374 696f 6e5f 6861 6e64 6c65 7228  unction_handler(
-00016dd0: 290a 2020 2020 6465 6620 706c 6f74 280a  ).    def plot(.
-00016de0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00016df0: 2020 2020 2020 7361 7665 5f70 6c6f 743d        save_plot=
-00016e00: 4e6f 6e65 2c0a 2020 2020 2020 2020 7369  None,.        si
-00016e10: 7a65 3d28 3230 3030 2c20 3135 3030 292c  ze=(2000, 1500),
-00016e20: 0a20 2020 2020 2020 2070 6c6f 745f 6465  .        plot_de
-00016e30: 6669 6e69 7469 6f6e 733d 4e6f 6e65 2c0a  finitions=None,.
-00016e40: 2020 2020 2020 2020 6669 7273 745f 6c61          first_la
-00016e50: 7965 723d 4e6f 6e65 2c0a 2020 2020 2020  yer=None,.      
-00016e60: 2020 6c61 7374 5f6c 6179 6572 3d4e 6f6e    last_layer=Non
-00016e70: 652c 0a20 2020 2020 2020 2073 6361 6c65  e,.        scale
-00016e80: 5f65 6c65 7661 7469 6f6e 3d54 7275 652c  _elevation=True,
-00016e90: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-00016ea0: 2222 2250 6c6f 7420 6375 7272 656e 7420  """Plot current 
-00016eb0: 7374 6163 6b75 7020 616e 642c 206f 7074  stackup and, opt
-00016ec0: 696f 6e61 6c6c 792c 206f 7665 726c 6170  ionally, overlap
-00016ed0: 2070 6164 7374 6163 6b20 6465 6669 6e69   padstack defini
-00016ee0: 7469 6f6e 732e 0a20 2020 2020 2020 2050  tions..        P
-00016ef0: 6c6f 7420 7375 7070 6f72 7473 206f 6e6c  lot supports onl
-00016f00: 7920 274c 616d 696e 6174 6527 2061 6e64  y 'Laminate' and
-00016f10: 2027 4f76 6572 6c61 7070 696e 6727 2073   'Overlapping' s
-00016f20: 7461 636b 7570 2074 7970 6573 2e0a 0a20  tackup types... 
-00016f30: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00016f40: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00016f50: 2d2d 2d2d 0a20 2020 2020 2020 2073 6176  ----.        sav
-00016f60: 655f 706c 6f74 203a 2073 7472 2c20 6f70  e_plot : str, op
-00016f70: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
-00016f80: 2020 2049 6620 6060 4e6f 6e65 6060 2074     If ``None`` t
-00016f90: 6865 2070 6c6f 7420 7769 6c6c 2062 6520  he plot will be 
-00016fa0: 7368 6f77 6e2e 0a20 2020 2020 2020 2020  shown..         
-00016fb0: 2020 2049 6620 6120 6669 6c65 2070 6174     If a file pat
-00016fc0: 6820 6973 2073 7065 6369 6669 6564 2074  h is specified t
-00016fd0: 6865 2070 6c6f 7420 7769 6c6c 2062 6520  he plot will be 
-00016fe0: 7361 7665 6420 746f 2073 7563 6820 6669  saved to such fi
-00016ff0: 6c65 2e0a 2020 2020 2020 2020 7369 7a65  le..        size
-00017000: 203a 2074 7570 6c65 2c20 6f70 7469 6f6e   : tuple, option
-00017010: 616c 0a20 2020 2020 2020 2020 2020 2049  al.            I
-00017020: 6d61 6765 2073 697a 6520 696e 2070 6978  mage size in pix
-00017030: 656c 2028 7769 6474 682c 2068 6569 6768  el (width, heigh
-00017040: 7429 2e20 4465 6661 756c 7420 7661 6c75  t). Default valu
-00017050: 6520 6973 2060 6028 3230 3030 2c20 3135  e is ``(2000, 15
-00017060: 3030 2960 600a 2020 2020 2020 2020 706c  00)``.        pl
-00017070: 6f74 5f64 6566 696e 6974 696f 6e73 203a  ot_definitions :
-00017080: 2073 7472 2c20 6c69 7374 2c20 6f70 7469   str, list, opti
-00017090: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
-000170a0: 204c 6973 7420 6f66 2070 6164 7374 6163   List of padstac
-000170b0: 6b20 6465 6669 6e69 7469 6f6e 7320 746f  k definitions to
-000170c0: 2070 6c6f 7420 6f6e 2074 6865 2073 7461   plot on the sta
-000170d0: 636b 7570 2e0a 2020 2020 2020 2020 2020  ckup..          
-000170e0: 2020 4974 2069 7320 7375 7070 6f72 7465    It is supporte
-000170f0: 6420 6f6e 6c79 2066 6f72 204c 616d 696e  d only for Lamin
-00017100: 6174 6520 6d6f 6465 2e0a 2020 2020 2020  ate mode..      
-00017110: 2020 6669 7273 745f 6c61 7965 7220 3a20    first_layer : 
-00017120: 7374 7220 6f72 203a 636c 6173 733a 6070  str or :class:`p
-00017130: 7965 6462 2e64 6f74 6e65 742e 6564 625f  yedb.dotnet.edb_
-00017140: 636f 7265 2e65 6462 5f64 6174 612e 6c61  core.edb_data.la
-00017150: 7965 725f 6461 7461 2e4c 6179 6572 4564  yer_data.LayerEd
-00017160: 6243 6c61 7373 600a 2020 2020 2020 2020  bClass`.        
-00017170: 2020 2020 4669 7273 7420 6c61 7965 7220      First layer 
-00017180: 746f 2070 6c6f 7420 6672 6f6d 2074 6865  to plot from the
-00017190: 2062 6f74 746f 6d2e 2044 6566 6175 6c74   bottom. Default
-000171a0: 2069 7320 604e 6f6e 6560 2074 6f20 7374   is `None` to st
-000171b0: 6172 7420 706c 6f74 7469 6e67 2066 726f  art plotting fro
-000171c0: 6d20 626f 7474 6f6d 2e0a 2020 2020 2020  m bottom..      
-000171d0: 2020 6c61 7374 5f6c 6179 6572 203a 2073    last_layer : s
-000171e0: 7472 206f 7220 3a63 6c61 7373 3a60 7079  tr or :class:`py
-000171f0: 6564 622e 646f 746e 6574 2e65 6462 5f63  edb.dotnet.edb_c
-00017200: 6f72 652e 6564 625f 6461 7461 2e6c 6179  ore.edb_data.lay
-00017210: 6572 5f64 6174 612e 4c61 7965 7245 6462  er_data.LayerEdb
-00017220: 436c 6173 7360 0a20 2020 2020 2020 2020  Class`.         
-00017230: 2020 204c 6173 7420 6c61 7965 7220 746f     Last layer to
-00017240: 2070 6c6f 7420 6672 6f6d 2074 6865 2062   plot from the b
-00017250: 6f74 746f 6d2e 2044 6566 6175 6c74 2069  ottom. Default i
-00017260: 7320 604e 6f6e 6560 2074 6f20 706c 6f74  s `None` to plot
-00017270: 2075 7020 746f 2074 6f70 206c 6179 6572   up to top layer
-00017280: 2e0a 2020 2020 2020 2020 7363 616c 655f  ..        scale_
-00017290: 656c 6576 6174 696f 6e20 3a20 626f 6f6c  elevation : bool
-000172a0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-000172b0: 2020 2020 2020 2054 6865 2072 6561 6c20         The real 
-000172c0: 6c61 7965 7220 7468 6963 6b6e 6573 7320  layer thickness 
-000172d0: 6973 2073 6361 6c65 6420 736f 2074 6861  is scaled so tha
-000172e0: 7420 6d61 785f 7468 6963 6b6e 6573 7320  t max_thickness 
-000172f0: 3d20 3320 2a20 6d69 6e5f 7468 6963 6b6e  = 3 * min_thickn
-00017300: 6573 732e 0a20 2020 2020 2020 2020 2020  ess..           
-00017310: 2044 6566 6175 6c74 2069 7320 6054 7275   Default is `Tru
-00017320: 6560 2e0a 0a20 2020 2020 2020 2052 6574  e`...        Ret
-00017330: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-00017340: 2d2d 2d2d 0a20 2020 2020 2020 203a 636c  ----.        :cl
-00017350: 6173 733a 606d 6174 706c 6f74 6c69 622e  ass:`matplotlib.
-00017360: 706c 7460 0a20 2020 2020 2020 2022 2222  plt`.        """
-00017370: 0a20 2020 2020 2020 2069 6620 6973 5f69  .        if is_i
-00017380: 726f 6e70 7974 686f 6e3a 0a20 2020 2020  ronpython:.     
-00017390: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-000173a0: 6c73 650a 2020 2020 2020 2020 6672 6f6d  lse.        from
-000173b0: 2070 7965 6462 2e67 656e 6572 6963 2e63   pyedb.generic.c
-000173c0: 6f6e 7374 616e 7473 2069 6d70 6f72 7420  onstants import 
-000173d0: 4353 5334 5f43 4f4c 4f52 530a 2020 2020  CSS4_COLORS.    
-000173e0: 2020 2020 6672 6f6d 2070 7965 6462 2e67      from pyedb.g
-000173f0: 656e 6572 6963 2e70 6c6f 7420 696d 706f  eneric.plot impo
-00017400: 7274 2070 6c6f 745f 6d61 7470 6c6f 746c  rt plot_matplotl
-00017410: 6962 0a0a 2020 2020 2020 2020 6c61 7965  ib..        laye
-00017420: 725f 6e61 6d65 7320 3d20 6c69 7374 2873  r_names = list(s
-00017430: 656c 662e 7374 6163 6b75 705f 6c61 7965  elf.stackup_laye
-00017440: 7273 2e6b 6579 7328 2929 0a20 2020 2020  rs.keys()).     
-00017450: 2020 2069 6620 6669 7273 745f 6c61 7965     if first_laye
-00017460: 7220 6973 204e 6f6e 6520 6f72 2066 6972  r is None or fir
-00017470: 7374 5f6c 6179 6572 206e 6f74 2069 6e20  st_layer not in 
-00017480: 6c61 7965 725f 6e61 6d65 733a 0a20 2020  layer_names:.   
-00017490: 2020 2020 2020 2020 2062 6f74 746f 6d5f           bottom_
-000174a0: 6c61 7965 7220 3d20 6c61 7965 725f 6e61  layer = layer_na
-000174b0: 6d65 735b 2d31 5d0a 2020 2020 2020 2020  mes[-1].        
-000174c0: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
-000174d0: 6669 7273 745f 6c61 7965 722c 2073 7472  first_layer, str
-000174e0: 293a 0a20 2020 2020 2020 2020 2020 2062  ):.            b
-000174f0: 6f74 746f 6d5f 6c61 7965 7220 3d20 6669  ottom_layer = fi
-00017500: 7273 745f 6c61 7965 720a 2020 2020 2020  rst_layer.      
-00017510: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
-00017520: 6528 6669 7273 745f 6c61 7965 722c 204c  e(first_layer, L
-00017530: 6179 6572 4564 6243 6c61 7373 293a 0a20  ayerEdbClass):. 
-00017540: 2020 2020 2020 2020 2020 2062 6f74 746f             botto
-00017550: 6d5f 6c61 7965 7220 3d20 6669 7273 745f  m_layer = first_
-00017560: 6c61 7965 722e 6e61 6d65 0a20 2020 2020  layer.name.     
-00017570: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00017580: 2020 2020 2072 6169 7365 2041 7474 7269       raise Attri
-00017590: 6275 7465 4572 726f 7228 2266 6972 7374  buteError("first
-000175a0: 5f6c 6179 6572 206d 7573 7420 6265 2073  _layer must be s
-000175b0: 7472 206f 7220 636c 6173 7320 6064 6f74  tr or class `dot
-000175c0: 6e65 742e 6564 625f 636f 7265 2e65 6462  net.edb_core.edb
-000175d0: 5f64 6174 612e 6c61 7965 725f 6461 7461  _data.layer_data
-000175e0: 2e4c 6179 6572 4564 6243 6c61 7373 6022  .LayerEdbClass`"
-000175f0: 290a 2020 2020 2020 2020 6966 206c 6173  ).        if las
-00017600: 745f 6c61 7965 7220 6973 204e 6f6e 6520  t_layer is None 
-00017610: 6f72 206c 6173 745f 6c61 7965 7220 6e6f  or last_layer no
-00017620: 7420 696e 206c 6179 6572 5f6e 616d 6573  t in layer_names
-00017630: 3a0a 2020 2020 2020 2020 2020 2020 746f  :.            to
-00017640: 705f 6c61 7965 7220 3d20 6c61 7965 725f  p_layer = layer_
-00017650: 6e61 6d65 735b 305d 0a20 2020 2020 2020  names[0].       
-00017660: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
-00017670: 286c 6173 745f 6c61 7965 722c 2073 7472  (last_layer, str
-00017680: 293a 0a20 2020 2020 2020 2020 2020 2074  ):.            t
-00017690: 6f70 5f6c 6179 6572 203d 206c 6173 745f  op_layer = last_
-000176a0: 6c61 7965 720a 2020 2020 2020 2020 656c  layer.        el
-000176b0: 6966 2069 7369 6e73 7461 6e63 6528 6c61  if isinstance(la
-000176c0: 7374 5f6c 6179 6572 2c20 4c61 7965 7245  st_layer, LayerE
-000176d0: 6462 436c 6173 7329 3a0a 2020 2020 2020  dbClass):.      
-000176e0: 2020 2020 2020 746f 705f 6c61 7965 7220        top_layer 
-000176f0: 3d20 6c61 7374 5f6c 6179 6572 2e6e 616d  = last_layer.nam
-00017700: 650a 2020 2020 2020 2020 656c 7365 3a0a  e.        else:.
-00017710: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00017720: 6520 4174 7472 6962 7574 6545 7272 6f72  e AttributeError
-00017730: 2822 6c61 7374 5f6c 6179 6572 206d 7573  ("last_layer mus
-00017740: 7420 6265 2073 7472 206f 7220 636c 6173  t be str or clas
-00017750: 7320 6064 6f74 6e65 742e 6564 625f 636f  s `dotnet.edb_co
-00017760: 7265 2e65 6462 5f64 6174 612e 6c61 7965  re.edb_data.laye
-00017770: 725f 6461 7461 2e4c 6179 6572 4564 6243  r_data.LayerEdbC
-00017780: 6c61 7373 6022 290a 0a20 2020 2020 2020  lass`")..       
-00017790: 2073 7461 636b 7570 5f6d 6f64 6520 3d20   stackup_mode = 
-000177a0: 7365 6c66 2e73 7461 636b 7570 5f6d 6f64  self.stackup_mod
-000177b0: 650a 2020 2020 2020 2020 6966 2073 7461  e.        if sta
-000177c0: 636b 7570 5f6d 6f64 6520 6e6f 7420 696e  ckup_mode not in
-000177d0: 205b 224c 616d 696e 6174 6522 2c20 224f   ["Laminate", "O
-000177e0: 7665 726c 6170 7069 6e67 225d 3a0a 2020  verlapping"]:.  
-000177f0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00017800: 4174 7472 6962 7574 6545 7272 6f72 2822  AttributeError("
-00017810: 7374 6163 6b75 7020 706c 6f74 2073 7570  stackup plot sup
-00017820: 706f 7274 7320 6f6e 6c79 2027 4c61 6d69  ports only 'Lami
-00017830: 6e61 7465 2720 616e 6420 274f 7665 726c  nate' and 'Overl
-00017840: 6170 7069 6e67 2720 7374 6163 6b75 7020  apping' stackup 
-00017850: 7479 7065 732e 2229 0a0a 2020 2020 2020  types.")..      
-00017860: 2020 2320 6275 696c 6420 7468 6520 6c61    # build the la
-00017870: 7965 7273 2064 6174 610a 2020 2020 2020  yers data.      
-00017880: 2020 6c61 7965 7273 5f64 6174 6120 3d20    layers_data = 
-00017890: 5b5d 0a20 2020 2020 2020 2073 6b69 705f  [].        skip_
-000178a0: 666c 6167 203d 2054 7275 650a 2020 2020  flag = True.    
-000178b0: 2020 2020 666f 7220 6c61 7965 7220 696e      for layer in
-000178c0: 2073 656c 662e 7374 6163 6b75 705f 6c61   self.stackup_la
-000178d0: 7965 7273 2e76 616c 7565 7328 293a 2020  yers.values():  
-000178e0: 2320 7374 6172 7420 6672 6f6d 2074 6f70  # start from top
-000178f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00017900: 6c61 7965 722e 6e61 6d65 2021 3d20 746f  layer.name != to
-00017910: 705f 6c61 7965 7220 616e 6420 736b 6970  p_layer and skip
-00017920: 5f66 6c61 673a 0a20 2020 2020 2020 2020  _flag:.         
-00017930: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
-00017940: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00017950: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00017960: 2020 736b 6970 5f66 6c61 6720 3d20 4661    skip_flag = Fa
-00017970: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
-00017980: 6c61 7965 7273 5f64 6174 612e 6170 7065  layers_data.appe
-00017990: 6e64 285b 6c61 7965 722c 206c 6179 6572  nd([layer, layer
-000179a0: 2e6c 6f77 6572 5f65 6c65 7661 7469 6f6e  .lower_elevation
-000179b0: 2c20 6c61 7965 722e 7570 7065 725f 656c  , layer.upper_el
-000179c0: 6576 6174 696f 6e2c 206c 6179 6572 2e74  evation, layer.t
-000179d0: 6869 636b 6e65 7373 5d29 0a20 2020 2020  hickness]).     
-000179e0: 2020 2020 2020 2069 6620 6c61 7965 722e         if layer.
-000179f0: 6e61 6d65 203d 3d20 626f 7474 6f6d 5f6c  name == bottom_l
-00017a00: 6179 6572 3a0a 2020 2020 2020 2020 2020  ayer:.          
-00017a10: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
-00017a20: 2020 2020 6c61 7965 7273 5f64 6174 612e      layers_data.
-00017a30: 7265 7665 7273 6528 2920 2023 206c 6574  reverse()  # let
-00017a40: 2773 2073 7461 7274 2066 726f 6d20 7468  's start from th
-00017a50: 6520 626f 7474 6f6d 0a0a 2020 2020 2020  e bottom..      
-00017a60: 2020 2320 7365 7061 7261 7465 2064 6965    # separate die
-00017a70: 6c65 6374 7269 6320 616e 6420 7369 676e  lectric and sign
-00017a80: 616c 2069 6620 6f76 6572 6c61 7070 696e  al if overlappin
-00017a90: 6720 7374 6163 6b75 700a 2020 2020 2020  g stackup.      
-00017aa0: 2020 6966 2073 7461 636b 7570 5f6d 6f64    if stackup_mod
-00017ab0: 6520 3d3d 2022 4f76 6572 6c61 7070 696e  e == "Overlappin
-00017ac0: 6722 3a0a 2020 2020 2020 2020 2020 2020  g":.            
-00017ad0: 6469 656c 6563 7472 6963 5f6c 6179 6572  dielectric_layer
-00017ae0: 7320 3d20 5b6c 2066 6f72 206c 2069 6e20  s = [l for l in 
-00017af0: 6c61 7965 7273 5f64 6174 6120 6966 206c  layers_data if l
-00017b00: 5b30 5d2e 7479 7065 203d 3d20 2264 6965  [0].type == "die
-00017b10: 6c65 6374 7269 6322 5d0a 2020 2020 2020  lectric"].      
-00017b20: 2020 2020 2020 7369 676e 616c 5f6c 6179        signal_lay
-00017b30: 6572 7320 3d20 5b6c 2066 6f72 206c 2069  ers = [l for l i
-00017b40: 6e20 6c61 7965 7273 5f64 6174 6120 6966  n layers_data if
-00017b50: 206c 5b30 5d2e 7479 7065 203d 3d20 2273   l[0].type == "s
-00017b60: 6967 6e61 6c22 5d0a 0a20 2020 2020 2020  ignal"]..       
-00017b70: 2023 2063 6f6d 7072 6573 7320 7468 6520   # compress the 
-00017b80: 7468 6963 6b6e 6573 7365 7320 6966 2072  thicknesses if r
-00017b90: 6571 7569 7265 640a 2020 2020 2020 2020  equired.        
-00017ba0: 6966 2073 6361 6c65 5f65 6c65 7661 7469  if scale_elevati
-00017bb0: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
-00017bc0: 6d69 6e5f 7468 6963 6b6e 6573 7320 3d20  min_thickness = 
-00017bd0: 6d69 6e28 5b69 5b33 5d20 666f 7220 6920  min([i[3] for i 
-00017be0: 696e 206c 6179 6572 735f 6461 7461 2069  in layers_data i
-00017bf0: 6620 695b 335d 2021 3d20 305d 290a 2020  f i[3] != 0]).  
-00017c00: 2020 2020 2020 2020 2020 6d61 785f 7468            max_th
-00017c10: 6963 6b6e 6573 7320 3d20 6d61 7828 5b69  ickness = max([i
-00017c20: 5b33 5d20 666f 7220 6920 696e 206c 6179  [3] for i in lay
-00017c30: 6572 735f 6461 7461 5d29 0a20 2020 2020  ers_data]).     
-00017c40: 2020 2020 2020 2063 203d 2033 2020 2320         c = 3  # 
-00017c50: 6d61 785f 7468 6963 6b6e 6573 7320 3d20  max_thickness = 
-00017c60: 6320 2a20 6d69 6e5f 7468 6963 6b6e 6573  c * min_thicknes
-00017c70: 730a 0a20 2020 2020 2020 2020 2020 2064  s..            d
-00017c80: 6566 205f 636f 6d70 7265 7373 5f74 2879  ef _compress_t(y
-00017c90: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00017ca0: 2020 206d 203d 206d 696e 5f74 6869 636b     m = min_thick
-00017cb0: 6e65 7373 0a20 2020 2020 2020 2020 2020  ness.           
-00017cc0: 2020 2020 204d 203d 206d 6178 5f74 6869       M = max_thi
-00017cd0: 636b 6e65 7373 0a20 2020 2020 2020 2020  ckness.         
-00017ce0: 2020 2020 2020 206b 203d 2028 6320 2d20         k = (c - 
-00017cf0: 3129 202a 206d 202f 2028 4d20 2d20 6d29  1) * m / (M - m)
-00017d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017d10: 2069 6620 7920 3e20 303a 0a20 2020 2020   if y > 0:.     
-00017d20: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00017d30: 6574 7572 6e20 2879 202d 206d 2920 2a20  eturn (y - m) * 
-00017d40: 6b20 2b20 6d0a 2020 2020 2020 2020 2020  k + m.          
-00017d50: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00017d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d70: 7265 7475 726e 2030 2e30 0a0a 2020 2020  return 0.0..    
-00017d80: 2020 2020 2020 2020 6966 2073 7461 636b          if stack
-00017d90: 7570 5f6d 6f64 6520 3d3d 2022 4c61 6d69  up_mode == "Lami
-00017da0: 6e61 7465 223a 0a20 2020 2020 2020 2020  nate":.         
-00017db0: 2020 2020 2020 206c 3020 3d20 6c61 7965         l0 = laye
-00017dc0: 7273 5f64 6174 615b 305d 0a20 2020 2020  rs_data[0].     
-00017dd0: 2020 2020 2020 2020 2020 2063 6f6d 7072             compr
-00017de0: 6573 7365 645f 6c61 7965 7273 5f64 6174  essed_layers_dat
-00017df0: 6120 3d20 5b5b 6c30 5b30 5d2c 206c 305b  a = [[l0[0], l0[
-00017e00: 315d 2c20 5f63 6f6d 7072 6573 735f 7428  1], _compress_t(
-00017e10: 6c30 5b33 5d29 2c20 5f63 6f6d 7072 6573  l0[3]), _compres
-00017e20: 735f 7428 6c30 5b33 5d29 5d5d 2020 2320  s_t(l0[3])]]  # 
-00017e30: 7468 6520 6669 7273 7420 726f 770a 2020  the first row.  
-00017e40: 2020 2020 2020 2020 2020 2020 2020 6c70                lp
-00017e50: 203d 2063 6f6d 7072 6573 7365 645f 6c61   = compressed_la
-00017e60: 7965 7273 5f64 6174 615b 305d 0a20 2020  yers_data[0].   
-00017e70: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00017e80: 206c 6920 696e 206c 6179 6572 735f 6461   li in layers_da
-00017e90: 7461 5b31 3a5d 3a20 2023 2074 6865 206f  ta[1:]:  # the o
-00017ea0: 7468 6572 2072 6f77 730a 2020 2020 2020  ther rows.      
-00017eb0: 2020 2020 2020 2020 2020 2020 2020 6374                ct
-00017ec0: 203d 205f 636f 6d70 7265 7373 5f74 286c   = _compress_t(l
-00017ed0: 695b 335d 290a 2020 2020 2020 2020 2020  i[3]).          
-00017ee0: 2020 2020 2020 2020 2020 636f 6d70 7265            compre
-00017ef0: 7373 6564 5f6c 6179 6572 735f 6461 7461  ssed_layers_data
-00017f00: 2e61 7070 656e 6428 5b6c 695b 305d 2c20  .append([li[0], 
-00017f10: 6c70 5b32 5d2c 206c 705b 325d 202b 2063  lp[2], lp[2] + c
-00017f20: 742c 2063 745d 290a 2020 2020 2020 2020  t, ct]).        
-00017f30: 2020 2020 2020 2020 2020 2020 6c70 203d              lp =
-00017f40: 2063 6f6d 7072 6573 7365 645f 6c61 7965   compressed_laye
-00017f50: 7273 5f64 6174 615b 2d31 5d0a 2020 2020  rs_data[-1].    
-00017f60: 2020 2020 2020 2020 2020 2020 6c61 7965              laye
-00017f70: 7273 5f64 6174 6120 3d20 636f 6d70 7265  rs_data = compre
-00017f80: 7373 6564 5f6c 6179 6572 735f 6461 7461  ssed_layers_data
-00017f90: 0a0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-00017fa0: 6966 2073 7461 636b 7570 5f6d 6f64 6520  if stackup_mode 
-00017fb0: 3d3d 2022 4f76 6572 6c61 7070 696e 6722  == "Overlapping"
-00017fc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00017fd0: 2020 636f 6d70 7265 7373 6564 5f64 6965    compressed_die
-00017fe0: 6c73 203d 205b 5d0a 2020 2020 2020 2020  ls = [].        
-00017ff0: 2020 2020 2020 2020 6669 7273 745f 6469          first_di
-00018000: 656c 203d 2054 7275 650a 2020 2020 2020  el = True.      
-00018010: 2020 2020 2020 2020 2020 666f 7220 6c69            for li
-00018020: 2069 6e20 6469 656c 6563 7472 6963 5f6c   in dielectric_l
-00018030: 6179 6572 733a 0a20 2020 2020 2020 2020  ayers:.         
-00018040: 2020 2020 2020 2020 2020 2063 7420 3d20             ct = 
-00018050: 5f63 6f6d 7072 6573 735f 7428 6c69 5b33  _compress_t(li[3
-00018060: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-00018070: 2020 2020 2020 2069 6620 6669 7273 745f         if first_
-00018080: 6469 656c 3a0a 2020 2020 2020 2020 2020  diel:.          
-00018090: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000180a0: 206c 695b 315d 203e 2030 3a0a 2020 2020   li[1] > 0:.    
+00016d80: 5573 6520 2e6c 6f61 6422 290a 2020 2020  Use .load").    
+00016d90: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00016da0: 6c6f 6164 2866 696c 655f 7061 7468 290a  load(file_path).
+00016db0: 0a20 2020 2040 7079 6564 625f 6675 6e63  .    @pyedb_func
+00016dc0: 7469 6f6e 5f68 616e 646c 6572 2829 0a20  tion_handler(). 
+00016dd0: 2020 2064 6566 2070 6c6f 7428 0a20 2020     def plot(.   
+00016de0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00016df0: 2020 2073 6176 655f 706c 6f74 3d4e 6f6e     save_plot=Non
+00016e00: 652c 0a20 2020 2020 2020 2073 697a 653d  e,.        size=
+00016e10: 2832 3030 302c 2031 3530 3029 2c0a 2020  (2000, 1500),.  
+00016e20: 2020 2020 2020 706c 6f74 5f64 6566 696e        plot_defin
+00016e30: 6974 696f 6e73 3d4e 6f6e 652c 0a20 2020  itions=None,.   
+00016e40: 2020 2020 2066 6972 7374 5f6c 6179 6572       first_layer
+00016e50: 3d4e 6f6e 652c 0a20 2020 2020 2020 206c  =None,.        l
+00016e60: 6173 745f 6c61 7965 723d 4e6f 6e65 2c0a  ast_layer=None,.
+00016e70: 2020 2020 2020 2020 7363 616c 655f 656c          scale_el
+00016e80: 6576 6174 696f 6e3d 5472 7565 2c0a 2020  evation=True,.  
+00016e90: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
+00016ea0: 506c 6f74 2063 7572 7265 6e74 2073 7461  Plot current sta
+00016eb0: 636b 7570 2061 6e64 2c20 6f70 7469 6f6e  ckup and, option
+00016ec0: 616c 6c79 2c20 6f76 6572 6c61 7020 7061  ally, overlap pa
+00016ed0: 6473 7461 636b 2064 6566 696e 6974 696f  dstack definitio
+00016ee0: 6e73 2e0a 2020 2020 2020 2020 506c 6f74  ns..        Plot
+00016ef0: 2073 7570 706f 7274 7320 6f6e 6c79 2027   supports only '
+00016f00: 4c61 6d69 6e61 7465 2720 616e 6420 274f  Laminate' and 'O
+00016f10: 7665 726c 6170 7069 6e67 2720 7374 6163  verlapping' stac
+00016f20: 6b75 7020 7479 7065 732e 0a0a 2020 2020  kup types...    
+00016f30: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00016f40: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00016f50: 2d0a 2020 2020 2020 2020 7361 7665 5f70  -.        save_p
+00016f60: 6c6f 7420 3a20 7374 722c 206f 7074 696f  lot : str, optio
+00016f70: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
+00016f80: 4966 2060 604e 6f6e 6560 6020 7468 6520  If ``None`` the 
+00016f90: 706c 6f74 2077 696c 6c20 6265 2073 686f  plot will be sho
+00016fa0: 776e 2e0a 2020 2020 2020 2020 2020 2020  wn..            
+00016fb0: 4966 2061 2066 696c 6520 7061 7468 2069  If a file path i
+00016fc0: 7320 7370 6563 6966 6965 6420 7468 6520  s specified the 
+00016fd0: 706c 6f74 2077 696c 6c20 6265 2073 6176  plot will be sav
+00016fe0: 6564 2074 6f20 7375 6368 2066 696c 652e  ed to such file.
+00016ff0: 0a20 2020 2020 2020 2073 697a 6520 3a20  .        size : 
+00017000: 7475 706c 652c 206f 7074 696f 6e61 6c0a  tuple, optional.
+00017010: 2020 2020 2020 2020 2020 2020 496d 6167              Imag
+00017020: 6520 7369 7a65 2069 6e20 7069 7865 6c20  e size in pixel 
+00017030: 2877 6964 7468 2c20 6865 6967 6874 292e  (width, height).
+00017040: 2044 6566 6175 6c74 2076 616c 7565 2069   Default value i
+00017050: 7320 6060 2832 3030 302c 2031 3530 3029  s ``(2000, 1500)
+00017060: 6060 0a20 2020 2020 2020 2070 6c6f 745f  ``.        plot_
+00017070: 6465 6669 6e69 7469 6f6e 7320 3a20 7374  definitions : st
+00017080: 722c 206c 6973 742c 206f 7074 696f 6e61  r, list, optiona
+00017090: 6c0a 2020 2020 2020 2020 2020 2020 4c69  l.            Li
+000170a0: 7374 206f 6620 7061 6473 7461 636b 2064  st of padstack d
+000170b0: 6566 696e 6974 696f 6e73 2074 6f20 706c  efinitions to pl
+000170c0: 6f74 206f 6e20 7468 6520 7374 6163 6b75  ot on the stacku
+000170d0: 702e 0a20 2020 2020 2020 2020 2020 2049  p..            I
+000170e0: 7420 6973 2073 7570 706f 7274 6564 206f  t is supported o
+000170f0: 6e6c 7920 666f 7220 4c61 6d69 6e61 7465  nly for Laminate
+00017100: 206d 6f64 652e 0a20 2020 2020 2020 2066   mode..        f
+00017110: 6972 7374 5f6c 6179 6572 203a 2073 7472  irst_layer : str
+00017120: 206f 7220 3a63 6c61 7373 3a60 7079 6564   or :class:`pyed
+00017130: 622e 646f 746e 6574 2e65 6462 5f63 6f72  b.dotnet.edb_cor
+00017140: 652e 6564 625f 6461 7461 2e6c 6179 6572  e.edb_data.layer
+00017150: 5f64 6174 612e 4c61 7965 7245 6462 436c  _data.LayerEdbCl
+00017160: 6173 7360 0a20 2020 2020 2020 2020 2020  ass`.           
+00017170: 2046 6972 7374 206c 6179 6572 2074 6f20   First layer to 
+00017180: 706c 6f74 2066 726f 6d20 7468 6520 626f  plot from the bo
+00017190: 7474 6f6d 2e20 4465 6661 756c 7420 6973  ttom. Default is
+000171a0: 2060 4e6f 6e65 6020 746f 2073 7461 7274   `None` to start
+000171b0: 2070 6c6f 7474 696e 6720 6672 6f6d 2062   plotting from b
+000171c0: 6f74 746f 6d2e 0a20 2020 2020 2020 206c  ottom..        l
+000171d0: 6173 745f 6c61 7965 7220 3a20 7374 7220  ast_layer : str 
+000171e0: 6f72 203a 636c 6173 733a 6070 7965 6462  or :class:`pyedb
+000171f0: 2e64 6f74 6e65 742e 6564 625f 636f 7265  .dotnet.edb_core
+00017200: 2e65 6462 5f64 6174 612e 6c61 7965 725f  .edb_data.layer_
+00017210: 6461 7461 2e4c 6179 6572 4564 6243 6c61  data.LayerEdbCla
+00017220: 7373 600a 2020 2020 2020 2020 2020 2020  ss`.            
+00017230: 4c61 7374 206c 6179 6572 2074 6f20 706c  Last layer to pl
+00017240: 6f74 2066 726f 6d20 7468 6520 626f 7474  ot from the bott
+00017250: 6f6d 2e20 4465 6661 756c 7420 6973 2060  om. Default is `
+00017260: 4e6f 6e65 6020 746f 2070 6c6f 7420 7570  None` to plot up
+00017270: 2074 6f20 746f 7020 6c61 7965 722e 0a20   to top layer.. 
+00017280: 2020 2020 2020 2073 6361 6c65 5f65 6c65         scale_ele
+00017290: 7661 7469 6f6e 203a 2062 6f6f 6c2c 206f  vation : bool, o
+000172a0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+000172b0: 2020 2020 5468 6520 7265 616c 206c 6179      The real lay
+000172c0: 6572 2074 6869 636b 6e65 7373 2069 7320  er thickness is 
+000172d0: 7363 616c 6564 2073 6f20 7468 6174 206d  scaled so that m
+000172e0: 6178 5f74 6869 636b 6e65 7373 203d 2033  ax_thickness = 3
+000172f0: 202a 206d 696e 5f74 6869 636b 6e65 7373   * min_thickness
+00017300: 2e0a 2020 2020 2020 2020 2020 2020 4465  ..            De
+00017310: 6661 756c 7420 6973 2060 5472 7565 602e  fault is `True`.
+00017320: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00017330: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00017340: 2d0a 2020 2020 2020 2020 3a63 6c61 7373  -.        :class
+00017350: 3a60 6d61 7470 6c6f 746c 6962 2e70 6c74  :`matplotlib.plt
+00017360: 600a 2020 2020 2020 2020 2222 220a 2020  `.        """.  
+00017370: 2020 2020 2020 6966 2069 735f 6972 6f6e        if is_iron
+00017380: 7079 7468 6f6e 3a0a 2020 2020 2020 2020  python:.        
+00017390: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+000173a0: 0a20 2020 2020 2020 2066 726f 6d20 7079  .        from py
+000173b0: 6564 622e 6765 6e65 7269 632e 636f 6e73  edb.generic.cons
+000173c0: 7461 6e74 7320 696d 706f 7274 2043 5353  tants import CSS
+000173d0: 345f 434f 4c4f 5253 0a20 2020 2020 2020  4_COLORS.       
+000173e0: 2066 726f 6d20 7079 6564 622e 6765 6e65   from pyedb.gene
+000173f0: 7269 632e 706c 6f74 2069 6d70 6f72 7420  ric.plot import 
+00017400: 706c 6f74 5f6d 6174 706c 6f74 6c69 620a  plot_matplotlib.
+00017410: 0a20 2020 2020 2020 206c 6179 6572 5f6e  .        layer_n
+00017420: 616d 6573 203d 206c 6973 7428 7365 6c66  ames = list(self
+00017430: 2e73 7461 636b 7570 5f6c 6179 6572 732e  .stackup_layers.
+00017440: 6b65 7973 2829 290a 2020 2020 2020 2020  keys()).        
+00017450: 6966 2066 6972 7374 5f6c 6179 6572 2069  if first_layer i
+00017460: 7320 4e6f 6e65 206f 7220 6669 7273 745f  s None or first_
+00017470: 6c61 7965 7220 6e6f 7420 696e 206c 6179  layer not in lay
+00017480: 6572 5f6e 616d 6573 3a0a 2020 2020 2020  er_names:.      
+00017490: 2020 2020 2020 626f 7474 6f6d 5f6c 6179        bottom_lay
+000174a0: 6572 203d 206c 6179 6572 5f6e 616d 6573  er = layer_names
+000174b0: 5b2d 315d 0a20 2020 2020 2020 2065 6c69  [-1].        eli
+000174c0: 6620 6973 696e 7374 616e 6365 2866 6972  f isinstance(fir
+000174d0: 7374 5f6c 6179 6572 2c20 7374 7229 3a0a  st_layer, str):.
+000174e0: 2020 2020 2020 2020 2020 2020 626f 7474              bott
+000174f0: 6f6d 5f6c 6179 6572 203d 2066 6972 7374  om_layer = first
+00017500: 5f6c 6179 6572 0a20 2020 2020 2020 2065  _layer.        e
+00017510: 6c69 6620 6973 696e 7374 616e 6365 2866  lif isinstance(f
+00017520: 6972 7374 5f6c 6179 6572 2c20 4c61 7965  irst_layer, Laye
+00017530: 7245 6462 436c 6173 7329 3a0a 2020 2020  rEdbClass):.    
+00017540: 2020 2020 2020 2020 626f 7474 6f6d 5f6c          bottom_l
+00017550: 6179 6572 203d 2066 6972 7374 5f6c 6179  ayer = first_lay
+00017560: 6572 2e6e 616d 650a 2020 2020 2020 2020  er.name.        
+00017570: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00017580: 2020 7261 6973 6520 4174 7472 6962 7574    raise Attribut
+00017590: 6545 7272 6f72 2822 6669 7273 745f 6c61  eError("first_la
+000175a0: 7965 7220 6d75 7374 2062 6520 7374 7220  yer must be str 
+000175b0: 6f72 2063 6c61 7373 2060 646f 746e 6574  or class `dotnet
+000175c0: 2e65 6462 5f63 6f72 652e 6564 625f 6461  .edb_core.edb_da
+000175d0: 7461 2e6c 6179 6572 5f64 6174 612e 4c61  ta.layer_data.La
+000175e0: 7965 7245 6462 436c 6173 7360 2229 0a20  yerEdbClass`"). 
+000175f0: 2020 2020 2020 2069 6620 6c61 7374 5f6c         if last_l
+00017600: 6179 6572 2069 7320 4e6f 6e65 206f 7220  ayer is None or 
+00017610: 6c61 7374 5f6c 6179 6572 206e 6f74 2069  last_layer not i
+00017620: 6e20 6c61 7965 725f 6e61 6d65 733a 0a20  n layer_names:. 
+00017630: 2020 2020 2020 2020 2020 2074 6f70 5f6c             top_l
+00017640: 6179 6572 203d 206c 6179 6572 5f6e 616d  ayer = layer_nam
+00017650: 6573 5b30 5d0a 2020 2020 2020 2020 656c  es[0].        el
+00017660: 6966 2069 7369 6e73 7461 6e63 6528 6c61  if isinstance(la
+00017670: 7374 5f6c 6179 6572 2c20 7374 7229 3a0a  st_layer, str):.
+00017680: 2020 2020 2020 2020 2020 2020 746f 705f              top_
+00017690: 6c61 7965 7220 3d20 6c61 7374 5f6c 6179  layer = last_lay
+000176a0: 6572 0a20 2020 2020 2020 2065 6c69 6620  er.        elif 
+000176b0: 6973 696e 7374 616e 6365 286c 6173 745f  isinstance(last_
+000176c0: 6c61 7965 722c 204c 6179 6572 4564 6243  layer, LayerEdbC
+000176d0: 6c61 7373 293a 0a20 2020 2020 2020 2020  lass):.         
+000176e0: 2020 2074 6f70 5f6c 6179 6572 203d 206c     top_layer = l
+000176f0: 6173 745f 6c61 7965 722e 6e61 6d65 0a20  ast_layer.name. 
+00017700: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00017710: 2020 2020 2020 2020 2072 6169 7365 2041           raise A
+00017720: 7474 7269 6275 7465 4572 726f 7228 226c  ttributeError("l
+00017730: 6173 745f 6c61 7965 7220 6d75 7374 2062  ast_layer must b
+00017740: 6520 7374 7220 6f72 2063 6c61 7373 2060  e str or class `
+00017750: 646f 746e 6574 2e65 6462 5f63 6f72 652e  dotnet.edb_core.
+00017760: 6564 625f 6461 7461 2e6c 6179 6572 5f64  edb_data.layer_d
+00017770: 6174 612e 4c61 7965 7245 6462 436c 6173  ata.LayerEdbClas
+00017780: 7360 2229 0a0a 2020 2020 2020 2020 7374  s`")..        st
+00017790: 6163 6b75 705f 6d6f 6465 203d 2073 656c  ackup_mode = sel
+000177a0: 662e 7374 6163 6b75 705f 6d6f 6465 0a20  f.stackup_mode. 
+000177b0: 2020 2020 2020 2069 6620 7374 6163 6b75         if stacku
+000177c0: 705f 6d6f 6465 206e 6f74 2069 6e20 5b22  p_mode not in ["
+000177d0: 4c61 6d69 6e61 7465 222c 2022 4f76 6572  Laminate", "Over
+000177e0: 6c61 7070 696e 6722 5d3a 0a20 2020 2020  lapping"]:.     
+000177f0: 2020 2020 2020 2072 6169 7365 2041 7474         raise Att
+00017800: 7269 6275 7465 4572 726f 7228 2273 7461  ributeError("sta
+00017810: 636b 7570 2070 6c6f 7420 7375 7070 6f72  ckup plot suppor
+00017820: 7473 206f 6e6c 7920 274c 616d 696e 6174  ts only 'Laminat
+00017830: 6527 2061 6e64 2027 4f76 6572 6c61 7070  e' and 'Overlapp
+00017840: 696e 6727 2073 7461 636b 7570 2074 7970  ing' stackup typ
+00017850: 6573 2e22 290a 0a20 2020 2020 2020 2023  es.")..        #
+00017860: 2062 7569 6c64 2074 6865 206c 6179 6572   build the layer
+00017870: 7320 6461 7461 0a20 2020 2020 2020 206c  s data.        l
+00017880: 6179 6572 735f 6461 7461 203d 205b 5d0a  ayers_data = [].
+00017890: 2020 2020 2020 2020 736b 6970 5f66 6c61          skip_fla
+000178a0: 6720 3d20 5472 7565 0a20 2020 2020 2020  g = True.       
+000178b0: 2066 6f72 206c 6179 6572 2069 6e20 7365   for layer in se
+000178c0: 6c66 2e73 7461 636b 7570 5f6c 6179 6572  lf.stackup_layer
+000178d0: 732e 7661 6c75 6573 2829 3a20 2023 2073  s.values():  # s
+000178e0: 7461 7274 2066 726f 6d20 746f 700a 2020  tart from top.  
+000178f0: 2020 2020 2020 2020 2020 6966 206c 6179            if lay
+00017900: 6572 2e6e 616d 6520 213d 2074 6f70 5f6c  er.name != top_l
+00017910: 6179 6572 2061 6e64 2073 6b69 705f 666c  ayer and skip_fl
+00017920: 6167 3a0a 2020 2020 2020 2020 2020 2020  ag:.            
+00017930: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
+00017940: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00017950: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00017960: 6b69 705f 666c 6167 203d 2046 616c 7365  kip_flag = False
+00017970: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
+00017980: 6572 735f 6461 7461 2e61 7070 656e 6428  ers_data.append(
+00017990: 5b6c 6179 6572 2c20 6c61 7965 722e 6c6f  [layer, layer.lo
+000179a0: 7765 725f 656c 6576 6174 696f 6e2c 206c  wer_elevation, l
+000179b0: 6179 6572 2e75 7070 6572 5f65 6c65 7661  ayer.upper_eleva
+000179c0: 7469 6f6e 2c20 6c61 7965 722e 7468 6963  tion, layer.thic
+000179d0: 6b6e 6573 735d 290a 2020 2020 2020 2020  kness]).        
+000179e0: 2020 2020 6966 206c 6179 6572 2e6e 616d      if layer.nam
+000179f0: 6520 3d3d 2062 6f74 746f 6d5f 6c61 7965  e == bottom_laye
+00017a00: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
+00017a10: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
+00017a20: 206c 6179 6572 735f 6461 7461 2e72 6576   layers_data.rev
+00017a30: 6572 7365 2829 2020 2320 6c65 7427 7320  erse()  # let's 
+00017a40: 7374 6172 7420 6672 6f6d 2074 6865 2062  start from the b
+00017a50: 6f74 746f 6d0a 0a20 2020 2020 2020 2023  ottom..        #
+00017a60: 2073 6570 6172 6174 6520 6469 656c 6563   separate dielec
+00017a70: 7472 6963 2061 6e64 2073 6967 6e61 6c20  tric and signal 
+00017a80: 6966 206f 7665 726c 6170 7069 6e67 2073  if overlapping s
+00017a90: 7461 636b 7570 0a20 2020 2020 2020 2069  tackup.        i
+00017aa0: 6620 7374 6163 6b75 705f 6d6f 6465 203d  f stackup_mode =
+00017ab0: 3d20 224f 7665 726c 6170 7069 6e67 223a  = "Overlapping":
+00017ac0: 0a20 2020 2020 2020 2020 2020 2064 6965  .            die
+00017ad0: 6c65 6374 7269 635f 6c61 7965 7273 203d  lectric_layers =
+00017ae0: 205b 6c20 666f 7220 6c20 696e 206c 6179   [l for l in lay
+00017af0: 6572 735f 6461 7461 2069 6620 6c5b 305d  ers_data if l[0]
+00017b00: 2e74 7970 6520 3d3d 2022 6469 656c 6563  .type == "dielec
+00017b10: 7472 6963 225d 0a20 2020 2020 2020 2020  tric"].         
+00017b20: 2020 2073 6967 6e61 6c5f 6c61 7965 7273     signal_layers
+00017b30: 203d 205b 6c20 666f 7220 6c20 696e 206c   = [l for l in l
+00017b40: 6179 6572 735f 6461 7461 2069 6620 6c5b  ayers_data if l[
+00017b50: 305d 2e74 7970 6520 3d3d 2022 7369 676e  0].type == "sign
+00017b60: 616c 225d 0a0a 2020 2020 2020 2020 2320  al"]..        # 
+00017b70: 636f 6d70 7265 7373 2074 6865 2074 6869  compress the thi
+00017b80: 636b 6e65 7373 6573 2069 6620 7265 7175  cknesses if requ
+00017b90: 6972 6564 0a20 2020 2020 2020 2069 6620  ired.        if 
+00017ba0: 7363 616c 655f 656c 6576 6174 696f 6e3a  scale_elevation:
+00017bb0: 0a20 2020 2020 2020 2020 2020 206d 696e  .            min
+00017bc0: 5f74 6869 636b 6e65 7373 203d 206d 696e  _thickness = min
+00017bd0: 285b 695b 335d 2066 6f72 2069 2069 6e20  ([i[3] for i in 
+00017be0: 6c61 7965 7273 5f64 6174 6120 6966 2069  layers_data if i
+00017bf0: 5b33 5d20 213d 2030 5d29 0a20 2020 2020  [3] != 0]).     
+00017c00: 2020 2020 2020 206d 6178 5f74 6869 636b         max_thick
+00017c10: 6e65 7373 203d 206d 6178 285b 695b 335d  ness = max([i[3]
+00017c20: 2066 6f72 2069 2069 6e20 6c61 7965 7273   for i in layers
+00017c30: 5f64 6174 615d 290a 2020 2020 2020 2020  _data]).        
+00017c40: 2020 2020 6320 3d20 3320 2023 206d 6178      c = 3  # max
+00017c50: 5f74 6869 636b 6e65 7373 203d 2063 202a  _thickness = c *
+00017c60: 206d 696e 5f74 6869 636b 6e65 7373 0a0a   min_thickness..
+00017c70: 2020 2020 2020 2020 2020 2020 6465 6620              def 
+00017c80: 5f63 6f6d 7072 6573 735f 7428 7929 3a0a  _compress_t(y):.
+00017c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ca0: 6d20 3d20 6d69 6e5f 7468 6963 6b6e 6573  m = min_thicknes
+00017cb0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00017cc0: 2020 4d20 3d20 6d61 785f 7468 6963 6b6e    M = max_thickn
+00017cd0: 6573 730a 2020 2020 2020 2020 2020 2020  ess.            
+00017ce0: 2020 2020 6b20 3d20 2863 202d 2031 2920      k = (c - 1) 
+00017cf0: 2a20 6d20 2f20 284d 202d 206d 290a 2020  * m / (M - m).  
+00017d00: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00017d10: 2079 203e 2030 3a0a 2020 2020 2020 2020   y > 0:.        
+00017d20: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00017d30: 726e 2028 7920 2d20 6d29 202a 206b 202b  rn (y - m) * k +
+00017d40: 206d 0a20 2020 2020 2020 2020 2020 2020   m.             
+00017d50: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00017d60: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00017d70: 7572 6e20 302e 300a 0a20 2020 2020 2020  urn 0.0..       
+00017d80: 2020 2020 2069 6620 7374 6163 6b75 705f       if stackup_
+00017d90: 6d6f 6465 203d 3d20 224c 616d 696e 6174  mode == "Laminat
+00017da0: 6522 3a0a 2020 2020 2020 2020 2020 2020  e":.            
+00017db0: 2020 2020 6c30 203d 206c 6179 6572 735f      l0 = layers_
+00017dc0: 6461 7461 5b30 5d0a 2020 2020 2020 2020  data[0].        
+00017dd0: 2020 2020 2020 2020 636f 6d70 7265 7373          compress
+00017de0: 6564 5f6c 6179 6572 735f 6461 7461 203d  ed_layers_data =
+00017df0: 205b 5b6c 305b 305d 2c20 6c30 5b31 5d2c   [[l0[0], l0[1],
+00017e00: 205f 636f 6d70 7265 7373 5f74 286c 305b   _compress_t(l0[
+00017e10: 335d 292c 205f 636f 6d70 7265 7373 5f74  3]), _compress_t
+00017e20: 286c 305b 335d 295d 5d20 2023 2074 6865  (l0[3])]]  # the
+00017e30: 2066 6972 7374 2072 6f77 0a20 2020 2020   first row.     
+00017e40: 2020 2020 2020 2020 2020 206c 7020 3d20             lp = 
+00017e50: 636f 6d70 7265 7373 6564 5f6c 6179 6572  compressed_layer
+00017e60: 735f 6461 7461 5b30 5d0a 2020 2020 2020  s_data[0].      
+00017e70: 2020 2020 2020 2020 2020 666f 7220 6c69            for li
+00017e80: 2069 6e20 6c61 7965 7273 5f64 6174 615b   in layers_data[
+00017e90: 313a 5d3a 2020 2320 7468 6520 6f74 6865  1:]:  # the othe
+00017ea0: 7220 726f 7773 0a20 2020 2020 2020 2020  r rows.         
+00017eb0: 2020 2020 2020 2020 2020 2063 7420 3d20             ct = 
+00017ec0: 5f63 6f6d 7072 6573 735f 7428 6c69 5b33  _compress_t(li[3
+00017ed0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+00017ee0: 2020 2020 2020 2063 6f6d 7072 6573 7365         compresse
+00017ef0: 645f 6c61 7965 7273 5f64 6174 612e 6170  d_layers_data.ap
+00017f00: 7065 6e64 285b 6c69 5b30 5d2c 206c 705b  pend([li[0], lp[
+00017f10: 325d 2c20 6c70 5b32 5d20 2b20 6374 2c20  2], lp[2] + ct, 
+00017f20: 6374 5d29 0a20 2020 2020 2020 2020 2020  ct]).           
+00017f30: 2020 2020 2020 2020 206c 7020 3d20 636f           lp = co
+00017f40: 6d70 7265 7373 6564 5f6c 6179 6572 735f  mpressed_layers_
+00017f50: 6461 7461 5b2d 315d 0a20 2020 2020 2020  data[-1].       
+00017f60: 2020 2020 2020 2020 206c 6179 6572 735f           layers_
+00017f70: 6461 7461 203d 2063 6f6d 7072 6573 7365  data = compresse
+00017f80: 645f 6c61 7965 7273 5f64 6174 610a 0a20  d_layers_data.. 
+00017f90: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00017fa0: 7374 6163 6b75 705f 6d6f 6465 203d 3d20  stackup_mode == 
+00017fb0: 224f 7665 726c 6170 7069 6e67 223a 0a20  "Overlapping":. 
+00017fc0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00017fd0: 6f6d 7072 6573 7365 645f 6469 656c 7320  ompressed_diels 
+00017fe0: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
+00017ff0: 2020 2020 2066 6972 7374 5f64 6965 6c20       first_diel 
+00018000: 3d20 5472 7565 0a20 2020 2020 2020 2020  = True.         
+00018010: 2020 2020 2020 2066 6f72 206c 6920 696e         for li in
+00018020: 2064 6965 6c65 6374 7269 635f 6c61 7965   dielectric_laye
+00018030: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
+00018040: 2020 2020 2020 2020 6374 203d 205f 636f          ct = _co
+00018050: 6d70 7265 7373 5f74 286c 695b 335d 290a  mpress_t(li[3]).
+00018060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018070: 2020 2020 6966 2066 6972 7374 5f64 6965      if first_die
+00018080: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
+00018090: 2020 2020 2020 2020 2020 2069 6620 6c69             if li
+000180a0: 5b31 5d20 3e20 303a 0a20 2020 2020 2020  [1] > 0:.       
 000180b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000180c0: 2020 2020 2020 2020 6c30 6c65 203d 205f          l0le = _
-000180d0: 636f 6d70 7265 7373 5f74 286c 695b 315d  compress_t(li[1]
-000180e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000180f0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+000180c0: 2020 2020 206c 306c 6520 3d20 5f63 6f6d       l0le = _com
+000180d0: 7072 6573 735f 7428 6c69 5b31 5d29 0a20  press_t(li[1]). 
+000180e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000180f0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
 00018100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018110: 2020 2020 2020 2020 2020 2020 6c30 6c65              l0le
-00018120: 203d 206c 695b 315d 0a20 2020 2020 2020   = li[1].       
-00018130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018140: 2063 6f6d 7072 6573 7365 645f 6469 656c   compressed_diel
-00018150: 732e 6170 7065 6e64 285b 6c69 5b30 5d2c  s.append([li[0],
-00018160: 206c 306c 652c 206c 306c 6520 2b20 6374   l0le, l0le + ct
-00018170: 2c20 6374 5d29 0a20 2020 2020 2020 2020  , ct]).         
-00018180: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00018190: 6972 7374 5f64 6965 6c20 3d20 4661 6c73  irst_diel = Fals
-000181a0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-000181b0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00018110: 2020 2020 2020 2020 206c 306c 6520 3d20           l0le = 
+00018120: 6c69 5b31 5d0a 2020 2020 2020 2020 2020  li[1].          
+00018130: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00018140: 6d70 7265 7373 6564 5f64 6965 6c73 2e61  mpressed_diels.a
+00018150: 7070 656e 6428 5b6c 695b 305d 2c20 6c30  ppend([li[0], l0
+00018160: 6c65 2c20 6c30 6c65 202b 2063 742c 2063  le, l0le + ct, c
+00018170: 745d 290a 2020 2020 2020 2020 2020 2020  t]).            
+00018180: 2020 2020 2020 2020 2020 2020 6669 7273              firs
+00018190: 745f 6469 656c 203d 2046 616c 7365 0a20  t_diel = False. 
+000181a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000181b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
 000181c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000181d0: 2020 2020 6c70 203d 2063 6f6d 7072 6573      lp = compres
-000181e0: 7365 645f 6469 656c 735b 2d31 5d0a 2020  sed_diels[-1].  
+000181d0: 206c 7020 3d20 636f 6d70 7265 7373 6564   lp = compressed
+000181e0: 5f64 6965 6c73 5b2d 315d 0a20 2020 2020  _diels[-1].     
 000181f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018200: 2020 2020 2020 636f 6d70 7265 7373 6564        compressed
-00018210: 5f64 6965 6c73 2e61 7070 656e 6428 5b6c  _diels.append([l
-00018220: 695b 305d 2c20 6c70 5b32 5d2c 206c 705b  i[0], lp[2], lp[
-00018230: 325d 202b 2063 742c 2063 745d 290a 0a20  2] + ct, ct]).. 
-00018240: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00018250: 6566 205f 636f 6e76 6572 745f 656c 6576  ef _convert_elev
-00018260: 6174 696f 6e28 656c 293a 0a20 2020 2020  ation(el):.     
-00018270: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00018280: 6e73 6964 6520 3d20 4661 6c73 650a 2020  nside = False.  
-00018290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000182a0: 2020 666f 7220 692c 206c 6920 696e 2065    for i, li in e
-000182b0: 6e75 6d65 7261 7465 2864 6965 6c65 6374  numerate(dielect
-000182c0: 7269 635f 6c61 7965 7273 293a 0a20 2020  ric_layers):.   
+00018200: 2020 2063 6f6d 7072 6573 7365 645f 6469     compressed_di
+00018210: 656c 732e 6170 7065 6e64 285b 6c69 5b30  els.append([li[0
+00018220: 5d2c 206c 705b 325d 2c20 6c70 5b32 5d20  ], lp[2], lp[2] 
+00018230: 2b20 6374 2c20 6374 5d29 0a0a 2020 2020  + ct, ct])..    
+00018240: 2020 2020 2020 2020 2020 2020 6465 6620              def 
+00018250: 5f63 6f6e 7665 7274 5f65 6c65 7661 7469  _convert_elevati
+00018260: 6f6e 2865 6c29 3a0a 2020 2020 2020 2020  on(el):.        
+00018270: 2020 2020 2020 2020 2020 2020 696e 7369              insi
+00018280: 6465 203d 2046 616c 7365 0a20 2020 2020  de = False.     
+00018290: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000182a0: 6f72 2069 2c20 6c69 2069 6e20 656e 756d  or i, li in enum
+000182b0: 6572 6174 6528 6469 656c 6563 7472 6963  erate(dielectric
+000182c0: 5f6c 6179 6572 7329 3a0a 2020 2020 2020  _layers):.      
 000182d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000182e0: 2020 2020 2069 6620 6c69 5b31 5d20 3c3d       if li[1] <=
-000182f0: 2065 6c20 3c3d 206c 695b 325d 3a0a 2020   el <= li[2]:.  
+000182e0: 2020 6966 206c 695b 315d 203c 3d20 656c    if li[1] <= el
+000182f0: 203c 3d20 6c69 5b32 5d3a 0a20 2020 2020   <= li[2]:.     
 00018300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018310: 2020 2020 2020 2020 2020 696e 7369 6465            inside
-00018320: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
+00018310: 2020 2020 2020 2069 6e73 6964 6520 3d20         inside = 
+00018320: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
 00018330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018340: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
-00018350: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00018360: 2069 6e73 6964 653a 0a20 2020 2020 2020   inside:.       
-00018370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018380: 2075 203d 2028 656c 202d 206c 695b 315d   u = (el - li[1]
-00018390: 2920 2f20 286c 695b 325d 202d 206c 695b  ) / (li[2] - li[
-000183a0: 315d 290a 2020 2020 2020 2020 2020 2020  1]).            
-000183b0: 2020 2020 2020 2020 2020 2020 636c 6920              cli 
-000183c0: 3d20 636f 6d70 7265 7373 6564 5f64 6965  = compressed_die
-000183d0: 6c73 5b69 5d0a 2020 2020 2020 2020 2020  ls[i].          
-000183e0: 2020 2020 2020 2020 2020 2020 2020 6365                ce
-000183f0: 6c20 3d20 636c 695b 315d 202b 2075 202a  l = cli[1] + u *
-00018400: 2028 636c 695b 325d 202d 2063 6c69 5b31   (cli[2] - cli[1
-00018410: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-00018420: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00018340: 2062 7265 616b 0a20 2020 2020 2020 2020   break.         
+00018350: 2020 2020 2020 2020 2020 2069 6620 696e             if in
+00018360: 7369 6465 3a0a 2020 2020 2020 2020 2020  side:.          
+00018370: 2020 2020 2020 2020 2020 2020 2020 7520                u 
+00018380: 3d20 2865 6c20 2d20 6c69 5b31 5d29 202f  = (el - li[1]) /
+00018390: 2028 6c69 5b32 5d20 2d20 6c69 5b31 5d29   (li[2] - li[1])
+000183a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000183b0: 2020 2020 2020 2020 2063 6c69 203d 2063           cli = c
+000183c0: 6f6d 7072 6573 7365 645f 6469 656c 735b  ompressed_diels[
+000183d0: 695d 0a20 2020 2020 2020 2020 2020 2020  i].             
+000183e0: 2020 2020 2020 2020 2020 2063 656c 203d             cel =
+000183f0: 2063 6c69 5b31 5d20 2b20 7520 2a20 2863   cli[1] + u * (c
+00018400: 6c69 5b32 5d20 2d20 636c 695b 315d 290a  li[2] - cli[1]).
+00018410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018420: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
 00018430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018440: 2020 2020 2063 656c 203d 2065 6c0a 2020       cel = el.  
-00018450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018460: 2020 7265 7475 726e 2063 656c 0a0a 2020    return cel..  
-00018470: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00018480: 6d70 7265 7373 6564 5f73 6967 6e61 6c73  mpressed_signals
-00018490: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
-000184a0: 2020 2020 2020 666f 7220 6c69 2069 6e20        for li in 
-000184b0: 7369 676e 616c 5f6c 6179 6572 733a 0a20  signal_layers:. 
+00018440: 2020 6365 6c20 3d20 656c 0a20 2020 2020    cel = el.     
+00018450: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00018460: 6574 7572 6e20 6365 6c0a 0a20 2020 2020  eturn cel..     
+00018470: 2020 2020 2020 2020 2020 2063 6f6d 7072             compr
+00018480: 6573 7365 645f 7369 676e 616c 7320 3d20  essed_signals = 
+00018490: 5b5d 0a20 2020 2020 2020 2020 2020 2020  [].             
+000184a0: 2020 2066 6f72 206c 6920 696e 2073 6967     for li in sig
+000184b0: 6e61 6c5f 6c61 7965 7273 3a0a 2020 2020  nal_layers:.    
 000184c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184d0: 2020 2063 6c65 203d 205f 636f 6e76 6572     cle = _conver
-000184e0: 745f 656c 6576 6174 696f 6e28 6c69 5b31  t_elevation(li[1
-000184f0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-00018500: 2020 2020 2020 2063 7565 203d 205f 636f         cue = _co
-00018510: 6e76 6572 745f 656c 6576 6174 696f 6e28  nvert_elevation(
-00018520: 6c69 5b32 5d29 0a20 2020 2020 2020 2020  li[2]).         
-00018530: 2020 2020 2020 2020 2020 2063 7420 3d20             ct = 
-00018540: 6375 6520 2d20 636c 650a 2020 2020 2020  cue - cle.      
-00018550: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00018560: 6d70 7265 7373 6564 5f73 6967 6e61 6c73  mpressed_signals
-00018570: 2e61 7070 656e 6428 5b6c 695b 305d 2c20  .append([li[0], 
-00018580: 636c 652c 2063 7565 2c20 6374 5d29 0a0a  cle, cue, ct])..
-00018590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000185a0: 6469 656c 6563 7472 6963 5f6c 6179 6572  dielectric_layer
-000185b0: 7320 3d20 636f 6d70 7265 7373 6564 5f64  s = compressed_d
-000185c0: 6965 6c73 0a20 2020 2020 2020 2020 2020  iels.           
-000185d0: 2020 2020 2073 6967 6e61 6c5f 6c61 7965       signal_laye
-000185e0: 7273 203d 2063 6f6d 7072 6573 7365 645f  rs = compressed_
-000185f0: 7369 676e 616c 730a 0a20 2020 2020 2020  signals..       
-00018600: 2023 2063 7265 6174 6520 7468 6520 6461   # create the da
-00018610: 7461 2066 6f72 2074 6865 2070 6c6f 740a  ta for the plot.
-00018620: 2020 2020 2020 2020 6469 656c 5f61 6c70          diel_alp
-00018630: 6861 203d 2030 2e34 0a20 2020 2020 2020  ha = 0.4.       
-00018640: 2073 6967 6e61 6c5f 616c 7068 6120 3d20   signal_alpha = 
-00018650: 302e 360a 2020 2020 2020 2020 7a65 726f  0.6.        zero
-00018660: 5f74 6869 636b 6e65 7373 5f61 6c70 6861  _thickness_alpha
-00018670: 203d 2031 2e30 0a20 2020 2020 2020 2061   = 1.0.        a
-00018680: 6e6e 6f74 6174 696f 6e5f 666f 6e74 7369  nnotation_fontsi
-00018690: 7a65 203d 2031 340a 2020 2020 2020 2020  ze = 14.        
-000186a0: 616e 6e6f 7461 7469 6f6e 5f78 5f6d 6172  annotation_x_mar
-000186b0: 6769 6e20 3d20 302e 3031 0a20 2020 2020  gin = 0.01.     
-000186c0: 2020 2061 6e6e 6f74 6174 696f 6e73 203d     annotations =
-000186d0: 205b 5d0a 2020 2020 2020 2020 706c 6f74   [].        plot
-000186e0: 5f64 6174 6120 3d20 5b5d 0a20 2020 2020  _data = [].     
-000186f0: 2020 2069 6620 7374 6163 6b75 705f 6d6f     if stackup_mo
-00018700: 6465 203d 3d20 224c 616d 696e 6174 6522  de == "Laminate"
-00018710: 3a0a 2020 2020 2020 2020 2020 2020 6d69  :.            mi
-00018720: 6e5f 7468 6963 6b6e 6573 7320 3d20 6d69  n_thickness = mi
-00018730: 6e28 5b69 5b33 5d20 666f 7220 6920 696e  n([i[3] for i in
-00018740: 206c 6179 6572 735f 6461 7461 2069 6620   layers_data if 
-00018750: 695b 335d 2021 3d20 305d 290a 2020 2020  i[3] != 0]).    
-00018760: 2020 2020 2020 2020 666f 7220 6c79 2069          for ly i
-00018770: 6e20 6c61 7965 7273 5f64 6174 613a 0a20  n layers_data:. 
-00018780: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00018790: 6179 6572 203d 206c 795b 305d 0a0a 2020  ayer = ly[0]..  
-000187a0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000187b0: 7365 7420 636f 6c6f 7220 616e 6420 6c61  set color and la
-000187c0: 6265 6c0a 2020 2020 2020 2020 2020 2020  bel.            
-000187d0: 2020 2020 636f 6c6f 7220 3d20 5b66 6c6f      color = [flo
-000187e0: 6174 2869 2920 2f20 3235 3620 666f 7220  at(i) / 256 for 
-000187f0: 6920 696e 206c 6179 6572 2e63 6f6c 6f72  i in layer.color
-00018800: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00018810: 2020 6966 2063 6f6c 6f72 203d 3d20 5b31    if color == [1
-00018820: 2e30 2c20 312e 302c 2031 2e30 5d3a 0a20  .0, 1.0, 1.0]:. 
+000184d0: 636c 6520 3d20 5f63 6f6e 7665 7274 5f65  cle = _convert_e
+000184e0: 6c65 7661 7469 6f6e 286c 695b 315d 290a  levation(li[1]).
+000184f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018500: 2020 2020 6375 6520 3d20 5f63 6f6e 7665      cue = _conve
+00018510: 7274 5f65 6c65 7661 7469 6f6e 286c 695b  rt_elevation(li[
+00018520: 325d 290a 2020 2020 2020 2020 2020 2020  2]).            
+00018530: 2020 2020 2020 2020 6374 203d 2063 7565          ct = cue
+00018540: 202d 2063 6c65 0a20 2020 2020 2020 2020   - cle.         
+00018550: 2020 2020 2020 2020 2020 2063 6f6d 7072             compr
+00018560: 6573 7365 645f 7369 676e 616c 732e 6170  essed_signals.ap
+00018570: 7065 6e64 285b 6c69 5b30 5d2c 2063 6c65  pend([li[0], cle
+00018580: 2c20 6375 652c 2063 745d 290a 0a20 2020  , cue, ct])..   
+00018590: 2020 2020 2020 2020 2020 2020 2064 6965               die
+000185a0: 6c65 6374 7269 635f 6c61 7965 7273 203d  lectric_layers =
+000185b0: 2063 6f6d 7072 6573 7365 645f 6469 656c   compressed_diel
+000185c0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+000185d0: 2020 7369 676e 616c 5f6c 6179 6572 7320    signal_layers 
+000185e0: 3d20 636f 6d70 7265 7373 6564 5f73 6967  = compressed_sig
+000185f0: 6e61 6c73 0a0a 2020 2020 2020 2020 2320  nals..        # 
+00018600: 6372 6561 7465 2074 6865 2064 6174 6120  create the data 
+00018610: 666f 7220 7468 6520 706c 6f74 0a20 2020  for the plot.   
+00018620: 2020 2020 2064 6965 6c5f 616c 7068 6120       diel_alpha 
+00018630: 3d20 302e 340a 2020 2020 2020 2020 7369  = 0.4.        si
+00018640: 676e 616c 5f61 6c70 6861 203d 2030 2e36  gnal_alpha = 0.6
+00018650: 0a20 2020 2020 2020 207a 6572 6f5f 7468  .        zero_th
+00018660: 6963 6b6e 6573 735f 616c 7068 6120 3d20  ickness_alpha = 
+00018670: 312e 300a 2020 2020 2020 2020 616e 6e6f  1.0.        anno
+00018680: 7461 7469 6f6e 5f66 6f6e 7473 697a 6520  tation_fontsize 
+00018690: 3d20 3134 0a20 2020 2020 2020 2061 6e6e  = 14.        ann
+000186a0: 6f74 6174 696f 6e5f 785f 6d61 7267 696e  otation_x_margin
+000186b0: 203d 2030 2e30 310a 2020 2020 2020 2020   = 0.01.        
+000186c0: 616e 6e6f 7461 7469 6f6e 7320 3d20 5b5d  annotations = []
+000186d0: 0a20 2020 2020 2020 2070 6c6f 745f 6461  .        plot_da
+000186e0: 7461 203d 205b 5d0a 2020 2020 2020 2020  ta = [].        
+000186f0: 6966 2073 7461 636b 7570 5f6d 6f64 6520  if stackup_mode 
+00018700: 3d3d 2022 4c61 6d69 6e61 7465 223a 0a20  == "Laminate":. 
+00018710: 2020 2020 2020 2020 2020 206d 696e 5f74             min_t
+00018720: 6869 636b 6e65 7373 203d 206d 696e 285b  hickness = min([
+00018730: 695b 335d 2066 6f72 2069 2069 6e20 6c61  i[3] for i in la
+00018740: 7965 7273 5f64 6174 6120 6966 2069 5b33  yers_data if i[3
+00018750: 5d20 213d 2030 5d29 0a20 2020 2020 2020  ] != 0]).       
+00018760: 2020 2020 2066 6f72 206c 7920 696e 206c       for ly in l
+00018770: 6179 6572 735f 6461 7461 3a0a 2020 2020  ayers_data:.    
+00018780: 2020 2020 2020 2020 2020 2020 6c61 7965              laye
+00018790: 7220 3d20 6c79 5b30 5d0a 0a20 2020 2020  r = ly[0]..     
+000187a0: 2020 2020 2020 2020 2020 2023 2073 6574             # set
+000187b0: 2063 6f6c 6f72 2061 6e64 206c 6162 656c   color and label
+000187c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000187d0: 2063 6f6c 6f72 203d 205b 666c 6f61 7428   color = [float(
+000187e0: 6929 202f 2032 3536 2066 6f72 2069 2069  i) / 256 for i i
+000187f0: 6e20 6c61 7965 722e 636f 6c6f 725d 0a20  n layer.color]. 
+00018800: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00018810: 6620 636f 6c6f 7220 3d3d 205b 312e 302c  f color == [1.0,
+00018820: 2031 2e30 2c20 312e 305d 3a0a 2020 2020   1.0, 1.0]:.    
 00018830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018840: 2020 2063 6f6c 6f72 203d 205b 302e 392c     color = [0.9,
-00018850: 2030 2e39 2c20 302e 395d 0a20 2020 2020   0.9, 0.9].     
-00018860: 2020 2020 2020 2020 2020 206c 6162 656c             label
-00018870: 203d 2022 7b7d 2c20 7b7d 2c20 7468 6963   = "{}, {}, thic
-00018880: 6b3a 207b 3a2e 3366 7d75 6d2c 2065 6c65  k: {:.3f}um, ele
-00018890: 763a 207b 3a2e 3366 7d75 6d22 2e66 6f72  v: {:.3f}um".for
-000188a0: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
-000188b0: 2020 2020 2020 2020 206c 6179 6572 2e6e           layer.n
-000188c0: 616d 652c 206c 6179 6572 2e6d 6174 6572  ame, layer.mater
-000188d0: 6961 6c2c 206c 6179 6572 2e74 6869 636b  ial, layer.thick
-000188e0: 6e65 7373 202a 2031 6536 2c20 6c61 7965  ness * 1e6, laye
-000188f0: 722e 6c6f 7765 725f 656c 6576 6174 696f  r.lower_elevatio
-00018900: 6e20 2a20 3165 360a 2020 2020 2020 2020  n * 1e6.        
-00018910: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00018920: 2020 2020 2020 2020 2020 2023 2063 7265             # cre
-00018930: 6174 6520 7061 7463 680a 2020 2020 2020  ate patch.      
-00018940: 2020 2020 2020 2020 2020 7820 3d20 5b30            x = [0
-00018950: 2c20 302c 2031 2c20 315d 0a20 2020 2020  , 0, 1, 1].     
-00018960: 2020 2020 2020 2020 2020 2069 6620 6c79             if ly
-00018970: 5b33 5d20 3e20 303a 0a20 2020 2020 2020  [3] > 0:.       
-00018980: 2020 2020 2020 2020 2020 2020 206c 6f77               low
-00018990: 6572 5f65 6c65 7661 7469 6f6e 203d 206c  er_elevation = l
-000189a0: 795b 315d 0a20 2020 2020 2020 2020 2020  y[1].           
-000189b0: 2020 2020 2020 2020 2075 7070 6572 5f65           upper_e
-000189c0: 6c65 7661 7469 6f6e 203d 206c 795b 325d  levation = ly[2]
-000189d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000189e0: 2020 2020 2079 203d 205b 6c6f 7765 725f       y = [lower_
-000189f0: 656c 6576 6174 696f 6e2c 2075 7070 6572  elevation, upper
-00018a00: 5f65 6c65 7661 7469 6f6e 2c20 7570 7065  _elevation, uppe
-00018a10: 725f 656c 6576 6174 696f 6e2c 206c 6f77  r_elevation, low
-00018a20: 6572 5f65 6c65 7661 7469 6f6e 5d0a 2020  er_elevation].  
-00018a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a40: 2020 706c 6f74 5f64 6174 612e 696e 7365    plot_data.inse
-00018a50: 7274 2830 2c20 5b78 2c20 792c 2063 6f6c  rt(0, [x, y, col
-00018a60: 6f72 2c20 6c61 6265 6c2c 2073 6967 6e61  or, label, signa
-00018a70: 6c5f 616c 7068 612c 2022 6669 6c6c 225d  l_alpha, "fill"]
-00018a80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00018a90: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00018aa0: 2020 2020 2020 2020 2020 2020 6c6f 7765              lowe
-00018ab0: 725f 656c 6576 6174 696f 6e20 3d20 6c79  r_elevation = ly
-00018ac0: 5b31 5d20 2d20 6d69 6e5f 7468 6963 6b6e  [1] - min_thickn
-00018ad0: 6573 7320 2a20 302e 3120 2023 206d 616b  ess * 0.1  # mak
-00018ae0: 6520 7468 6520 7a65 726f 2074 6869 636b  e the zero thick
-00018af0: 6e65 7373 206c 6179 6572 7320 6d6f 7265  ness layers more
-00018b00: 2076 6973 6962 6c65 0a20 2020 2020 2020   visible.       
-00018b10: 2020 2020 2020 2020 2020 2020 2075 7070               upp
-00018b20: 6572 5f65 6c65 7661 7469 6f6e 203d 206c  er_elevation = l
-00018b30: 795b 325d 202b 206d 696e 5f74 6869 636b  y[2] + min_thick
-00018b40: 6e65 7373 202a 2030 2e31 0a20 2020 2020  ness * 0.1.     
-00018b50: 2020 2020 2020 2020 2020 2020 2020 2079                 y
-00018b60: 203d 205b 6c6f 7765 725f 656c 6576 6174   = [lower_elevat
-00018b70: 696f 6e2c 2075 7070 6572 5f65 6c65 7661  ion, upper_eleva
-00018b80: 7469 6f6e 2c20 7570 7065 725f 656c 6576  tion, upper_elev
-00018b90: 6174 696f 6e2c 206c 6f77 6572 5f65 6c65  ation, lower_ele
-00018ba0: 7661 7469 6f6e 5d0a 2020 2020 2020 2020  vation].        
-00018bb0: 2020 2020 2020 2020 2020 2020 2320 7075              # pu
-00018bc0: 7420 7468 6520 7a65 726f 2074 6869 636b  t the zero thick
-00018bd0: 6e65 7373 206c 6179 6572 7320 6f6e 2074  ness layers on t
-00018be0: 6f70 0a20 2020 2020 2020 2020 2020 2020  op.             
-00018bf0: 2020 2020 2020 2070 6c6f 745f 6461 7461         plot_data
-00018c00: 2e61 7070 656e 6428 5b78 2c20 792c 2063  .append([x, y, c
-00018c10: 6f6c 6f72 2c20 6c61 6265 6c2c 207a 6572  olor, label, zer
-00018c20: 6f5f 7468 6963 6b6e 6573 735f 616c 7068  o_thickness_alph
-00018c30: 612c 2022 6669 6c6c 225d 290a 0a20 2020  a, "fill"])..   
-00018c40: 2020 2020 2020 2020 2020 2020 2023 2063               # c
-00018c50: 7265 6174 6520 616e 6e6f 7461 7469 6f6e  reate annotation
-00018c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018c70: 2079 5f70 6f73 203d 2028 6c6f 7765 725f   y_pos = (lower_
-00018c80: 656c 6576 6174 696f 6e20 2b20 7570 7065  elevation + uppe
-00018c90: 725f 656c 6576 6174 696f 6e29 202f 2032  r_elevation) / 2
-00018ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018cb0: 2069 6620 6c61 7965 722e 7479 7065 203d   if layer.type =
-00018cc0: 3d20 2264 6965 6c65 6374 7269 6322 3a0a  = "dielectric":.
+00018840: 636f 6c6f 7220 3d20 5b30 2e39 2c20 302e  color = [0.9, 0.
+00018850: 392c 2030 2e39 5d0a 2020 2020 2020 2020  9, 0.9].        
+00018860: 2020 2020 2020 2020 6c61 6265 6c20 3d20          label = 
+00018870: 227b 7d2c 207b 7d2c 2074 6869 636b 3a20  "{}, {}, thick: 
+00018880: 7b3a 2e33 667d 756d 2c20 656c 6576 3a20  {:.3f}um, elev: 
+00018890: 7b3a 2e33 667d 756d 222e 666f 726d 6174  {:.3f}um".format
+000188a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000188b0: 2020 2020 2020 6c61 7965 722e 6e61 6d65        layer.name
+000188c0: 2c20 6c61 7965 722e 6d61 7465 7269 616c  , layer.material
+000188d0: 2c20 6c61 7965 722e 7468 6963 6b6e 6573  , layer.thicknes
+000188e0: 7320 2a20 3165 362c 206c 6179 6572 2e6c  s * 1e6, layer.l
+000188f0: 6f77 6572 5f65 6c65 7661 7469 6f6e 202a  ower_elevation *
+00018900: 2031 6536 0a20 2020 2020 2020 2020 2020   1e6.           
+00018910: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00018920: 2020 2020 2020 2020 2320 6372 6561 7465          # create
+00018930: 2070 6174 6368 0a20 2020 2020 2020 2020   patch.         
+00018940: 2020 2020 2020 2078 203d 205b 302c 2030         x = [0, 0
+00018950: 2c20 312c 2031 5d0a 2020 2020 2020 2020  , 1, 1].        
+00018960: 2020 2020 2020 2020 6966 206c 795b 335d          if ly[3]
+00018970: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
+00018980: 2020 2020 2020 2020 2020 6c6f 7765 725f            lower_
+00018990: 656c 6576 6174 696f 6e20 3d20 6c79 5b31  elevation = ly[1
+000189a0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+000189b0: 2020 2020 2020 7570 7065 725f 656c 6576        upper_elev
+000189c0: 6174 696f 6e20 3d20 6c79 5b32 5d0a 2020  ation = ly[2].  
+000189d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000189e0: 2020 7920 3d20 5b6c 6f77 6572 5f65 6c65    y = [lower_ele
+000189f0: 7661 7469 6f6e 2c20 7570 7065 725f 656c  vation, upper_el
+00018a00: 6576 6174 696f 6e2c 2075 7070 6572 5f65  evation, upper_e
+00018a10: 6c65 7661 7469 6f6e 2c20 6c6f 7765 725f  levation, lower_
+00018a20: 656c 6576 6174 696f 6e5d 0a20 2020 2020  elevation].     
+00018a30: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00018a40: 6c6f 745f 6461 7461 2e69 6e73 6572 7428  lot_data.insert(
+00018a50: 302c 205b 782c 2079 2c20 636f 6c6f 722c  0, [x, y, color,
+00018a60: 206c 6162 656c 2c20 7369 676e 616c 5f61   label, signal_a
+00018a70: 6c70 6861 2c20 2266 696c 6c22 5d29 0a20  lpha, "fill"]). 
+00018a80: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00018a90: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00018aa0: 2020 2020 2020 2020 206c 6f77 6572 5f65           lower_e
+00018ab0: 6c65 7661 7469 6f6e 203d 206c 795b 315d  levation = ly[1]
+00018ac0: 202d 206d 696e 5f74 6869 636b 6e65 7373   - min_thickness
+00018ad0: 202a 2030 2e31 2020 2320 6d61 6b65 2074   * 0.1  # make t
+00018ae0: 6865 207a 6572 6f20 7468 6963 6b6e 6573  he zero thicknes
+00018af0: 7320 6c61 7965 7273 206d 6f72 6520 7669  s layers more vi
+00018b00: 7369 626c 650a 2020 2020 2020 2020 2020  sible.          
+00018b10: 2020 2020 2020 2020 2020 7570 7065 725f            upper_
+00018b20: 656c 6576 6174 696f 6e20 3d20 6c79 5b32  elevation = ly[2
+00018b30: 5d20 2b20 6d69 6e5f 7468 6963 6b6e 6573  ] + min_thicknes
+00018b40: 7320 2a20 302e 310a 2020 2020 2020 2020  s * 0.1.        
+00018b50: 2020 2020 2020 2020 2020 2020 7920 3d20              y = 
+00018b60: 5b6c 6f77 6572 5f65 6c65 7661 7469 6f6e  [lower_elevation
+00018b70: 2c20 7570 7065 725f 656c 6576 6174 696f  , upper_elevatio
+00018b80: 6e2c 2075 7070 6572 5f65 6c65 7661 7469  n, upper_elevati
+00018b90: 6f6e 2c20 6c6f 7765 725f 656c 6576 6174  on, lower_elevat
+00018ba0: 696f 6e5d 0a20 2020 2020 2020 2020 2020  ion].           
+00018bb0: 2020 2020 2020 2020 2023 2070 7574 2074           # put t
+00018bc0: 6865 207a 6572 6f20 7468 6963 6b6e 6573  he zero thicknes
+00018bd0: 7320 6c61 7965 7273 206f 6e20 746f 700a  s layers on top.
+00018be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018bf0: 2020 2020 706c 6f74 5f64 6174 612e 6170      plot_data.ap
+00018c00: 7065 6e64 285b 782c 2079 2c20 636f 6c6f  pend([x, y, colo
+00018c10: 722c 206c 6162 656c 2c20 7a65 726f 5f74  r, label, zero_t
+00018c20: 6869 636b 6e65 7373 5f61 6c70 6861 2c20  hickness_alpha, 
+00018c30: 2266 696c 6c22 5d29 0a0a 2020 2020 2020  "fill"])..      
+00018c40: 2020 2020 2020 2020 2020 2320 6372 6561            # crea
+00018c50: 7465 2061 6e6e 6f74 6174 696f 6e0a 2020  te annotation.  
+00018c60: 2020 2020 2020 2020 2020 2020 2020 795f                y_
+00018c70: 706f 7320 3d20 286c 6f77 6572 5f65 6c65  pos = (lower_ele
+00018c80: 7661 7469 6f6e 202b 2075 7070 6572 5f65  vation + upper_e
+00018c90: 6c65 7661 7469 6f6e 2920 2f20 320a 2020  levation) / 2.  
+00018ca0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00018cb0: 206c 6179 6572 2e74 7970 6520 3d3d 2022   layer.type == "
+00018cc0: 6469 656c 6563 7472 6963 223a 0a20 2020  dielectric":.   
 00018cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ce0: 2020 2020 785f 706f 7320 3d20 2d61 6e6e      x_pos = -ann
-00018cf0: 6f74 6174 696f 6e5f 785f 6d61 7267 696e  otation_x_margin
-00018d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018d10: 2020 2020 2061 6e6e 6f74 6174 696f 6e73       annotations
-00018d20: 2e61 7070 656e 6428 0a20 2020 2020 2020  .append(.       
-00018d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d40: 205b 785f 706f 732c 2079 5f70 6f73 2c20   [x_pos, y_pos, 
-00018d50: 6c61 7965 722e 6e61 6d65 2c20 7b22 666f  layer.name, {"fo
-00018d60: 6e74 7369 7a65 223a 2061 6e6e 6f74 6174  ntsize": annotat
-00018d70: 696f 6e5f 666f 6e74 7369 7a65 2c20 2268  ion_fontsize, "h
-00018d80: 6f72 697a 6f6e 7461 6c61 6c69 676e 6d65  orizontalalignme
-00018d90: 6e74 223a 2022 7269 6768 7422 7d5d 0a20  nt": "right"}]. 
+00018ce0: 2078 5f70 6f73 203d 202d 616e 6e6f 7461   x_pos = -annota
+00018cf0: 7469 6f6e 5f78 5f6d 6172 6769 6e0a 2020  tion_x_margin.  
+00018d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d10: 2020 616e 6e6f 7461 7469 6f6e 732e 6170    annotations.ap
+00018d20: 7065 6e64 280a 2020 2020 2020 2020 2020  pend(.          
+00018d30: 2020 2020 2020 2020 2020 2020 2020 5b78                [x
+00018d40: 5f70 6f73 2c20 795f 706f 732c 206c 6179  _pos, y_pos, lay
+00018d50: 6572 2e6e 616d 652c 207b 2266 6f6e 7473  er.name, {"fonts
+00018d60: 697a 6522 3a20 616e 6e6f 7461 7469 6f6e  ize": annotation
+00018d70: 5f66 6f6e 7473 697a 652c 2022 686f 7269  _fontsize, "hori
+00018d80: 7a6f 6e74 616c 616c 6967 6e6d 656e 7422  zontalalignment"
+00018d90: 3a20 2272 6967 6874 227d 5d0a 2020 2020  : "right"}].    
 00018da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018db0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00018dc0: 2020 2020 2065 6c69 6620 6c61 7965 722e       elif layer.
-00018dd0: 7479 7065 203d 3d20 2273 6967 6e61 6c22  type == "signal"
-00018de0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00018df0: 2020 2020 2020 785f 706f 7320 3d20 312e        x_pos = 1.
-00018e00: 3020 2b20 616e 6e6f 7461 7469 6f6e 5f78  0 + annotation_x
-00018e10: 5f6d 6172 6769 6e0a 2020 2020 2020 2020  _margin.        
-00018e20: 2020 2020 2020 2020 2020 2020 616e 6e6f              anno
-00018e30: 7461 7469 6f6e 732e 6170 7065 6e64 285b  tations.append([
-00018e40: 785f 706f 732c 2079 5f70 6f73 2c20 6c61  x_pos, y_pos, la
-00018e50: 7965 722e 6e61 6d65 2c20 7b22 666f 6e74  yer.name, {"font
-00018e60: 7369 7a65 223a 2061 6e6e 6f74 6174 696f  size": annotatio
-00018e70: 6e5f 666f 6e74 7369 7a65 7d5d 290a 0a20  n_fontsize}]).. 
-00018e80: 2020 2020 2020 2020 2020 2023 2065 7661             # eva
-00018e90: 6c75 6174 6520 7468 6520 6c65 6765 6e64  luate the legend
-00018ea0: 2072 656f 7264 6572 0a20 2020 2020 2020   reorder.       
-00018eb0: 2020 2020 206c 6567 656e 645f 6f72 6465       legend_orde
-00018ec0: 7220 3d20 5b5d 0a20 2020 2020 2020 2020  r = [].         
-00018ed0: 2020 2066 6f72 206c 7920 696e 206c 6179     for ly in lay
-00018ee0: 6572 735f 6461 7461 3a0a 2020 2020 2020  ers_data:.      
-00018ef0: 2020 2020 2020 2020 2020 6e61 6d65 203d            name =
-00018f00: 206c 795b 305d 2e6e 616d 650a 2020 2020   ly[0].name.    
-00018f10: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00018f20: 692c 2061 2069 6e20 656e 756d 6572 6174  i, a in enumerat
-00018f30: 6528 706c 6f74 5f64 6174 6129 3a0a 2020  e(plot_data):.  
-00018f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f50: 2020 696e 616d 6520 3d20 615b 335d 2e73    iname = a[3].s
-00018f60: 706c 6974 2822 2c22 295b 305d 0a20 2020  plit(",")[0].   
-00018f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f80: 2069 6620 6e61 6d65 203d 3d20 696e 616d   if name == inam
-00018f90: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00018fa0: 2020 2020 2020 2020 2020 206c 6567 656e             legen
-00018fb0: 645f 6f72 6465 722e 6170 7065 6e64 2869  d_order.append(i
-00018fc0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00018fd0: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
-00018fe0: 0a20 2020 2020 2020 2065 6c69 6620 7374  .        elif st
-00018ff0: 6163 6b75 705f 6d6f 6465 203d 3d20 224f  ackup_mode == "O
-00019000: 7665 726c 6170 7069 6e67 223a 0a20 2020  verlapping":.   
-00019010: 2020 2020 2020 2020 206d 696e 5f74 6869           min_thi
-00019020: 636b 6e65 7373 203d 206d 696e 285b 695b  ckness = min([i[
-00019030: 335d 2066 6f72 2069 2069 6e20 7369 676e  3] for i in sign
-00019040: 616c 5f6c 6179 6572 7320 6966 2069 5b33  al_layers if i[3
-00019050: 5d20 213d 2030 5d29 0a20 2020 2020 2020  ] != 0]).       
-00019060: 2020 2020 2063 6f6c 756d 6e73 203d 205b       columns = [
-00019070: 5d20 2023 2066 6972 7374 2063 6f6c 756d  ]  # first colum
-00019080: 6e20 6973 2078 3d5b 302c 315d 2c20 7365  n is x=[0,1], se
-00019090: 636f 6e64 2063 6f6c 756d 6e20 6973 2078  cond column is x
-000190a0: 3d5b 312c 325d 2061 6e64 2073 6f20 6f6e  =[1,2] and so on
-000190b0: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
-000190c0: 666f 7220 6c79 2069 6e20 7369 676e 616c  for ly in signal
-000190d0: 5f6c 6179 6572 733a 0a20 2020 2020 2020  _layers:.       
-000190e0: 2020 2020 2020 2020 206c 6f77 6572 5f65           lower_e
-000190f0: 6c65 7661 7469 6f6e 203d 206c 795b 315d  levation = ly[1]
-00019100: 2020 2320 6c6f 7765 7220 656c 6576 6174    # lower elevat
-00019110: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-00019120: 2020 2020 7420 3d20 6c79 5b33 5d20 2023      t = ly[3]  #
-00019130: 2074 6869 636b 6e65 7373 0a20 2020 2020   thickness.     
-00019140: 2020 2020 2020 2020 2020 2070 7574 5f69             put_i
-00019150: 6e5f 636f 6c75 6d6e 203d 2030 0a20 2020  n_column = 0.   
-00019160: 2020 2020 2020 2020 2020 2020 2063 656c               cel
-00019170: 6c5f 706f 7369 7469 6f6e 203d 2030 0a20  l_position = 0. 
-00019180: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00019190: 6f72 2063 2069 6e20 636f 6c75 6d6e 733a  or c in columns:
-000191a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000191b0: 2020 2020 2075 6570 203d 2063 5b2d 315d       uep = c[-1]
-000191c0: 5b30 5d5b 325d 2020 2320 7570 7065 7220  [0][2]  # upper 
-000191d0: 656c 6576 6174 696f 6e20 6f66 2074 6865  elevation of the
-000191e0: 206c 6173 7420 656e 7472 7920 6f66 2074   last entry of t
-000191f0: 6861 7420 636f 6c75 6d6e 0a20 2020 2020  hat column.     
-00019200: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00019210: 7020 3d20 635b 2d31 5d5b 305d 5b33 5d20  p = c[-1][0][3] 
-00019220: 2023 2074 6869 636b 6e65 7373 206f 6620   # thickness of 
-00019230: 7468 6520 6c61 7374 2065 6e74 7279 206f  the last entry o
-00019240: 6620 7468 6174 2063 6f6c 756d 6e0a 2020  f that column.  
-00019250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019260: 2020 6966 206c 6f77 6572 5f65 6c65 7661    if lower_eleva
-00019270: 7469 6f6e 203c 2075 6570 206f 7220 2861  tion < uep or (a
-00019280: 6273 286c 6f77 6572 5f65 6c65 7661 7469  bs(lower_elevati
-00019290: 6f6e 202d 2075 6570 2920 3c20 3165 2d31  on - uep) < 1e-1
-000192a0: 3520 616e 6420 7470 203d 3d20 3020 616e  5 and tp == 0 an
-000192b0: 6420 7420 3d3d 2030 293a 0a20 2020 2020  d t == 0):.     
+00018db0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00018dc0: 2020 656c 6966 206c 6179 6572 2e74 7970    elif layer.typ
+00018dd0: 6520 3d3d 2022 7369 676e 616c 223a 0a20  e == "signal":. 
+00018de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018df0: 2020 2078 5f70 6f73 203d 2031 2e30 202b     x_pos = 1.0 +
+00018e00: 2061 6e6e 6f74 6174 696f 6e5f 785f 6d61   annotation_x_ma
+00018e10: 7267 696e 0a20 2020 2020 2020 2020 2020  rgin.           
+00018e20: 2020 2020 2020 2020 2061 6e6e 6f74 6174           annotat
+00018e30: 696f 6e73 2e61 7070 656e 6428 5b78 5f70  ions.append([x_p
+00018e40: 6f73 2c20 795f 706f 732c 206c 6179 6572  os, y_pos, layer
+00018e50: 2e6e 616d 652c 207b 2266 6f6e 7473 697a  .name, {"fontsiz
+00018e60: 6522 3a20 616e 6e6f 7461 7469 6f6e 5f66  e": annotation_f
+00018e70: 6f6e 7473 697a 657d 5d29 0a0a 2020 2020  ontsize}])..    
+00018e80: 2020 2020 2020 2020 2320 6576 616c 7561          # evalua
+00018e90: 7465 2074 6865 206c 6567 656e 6420 7265  te the legend re
+00018ea0: 6f72 6465 720a 2020 2020 2020 2020 2020  order.          
+00018eb0: 2020 6c65 6765 6e64 5f6f 7264 6572 203d    legend_order =
+00018ec0: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
+00018ed0: 666f 7220 6c79 2069 6e20 6c61 7965 7273  for ly in layers
+00018ee0: 5f64 6174 613a 0a20 2020 2020 2020 2020  _data:.         
+00018ef0: 2020 2020 2020 206e 616d 6520 3d20 6c79         name = ly
+00018f00: 5b30 5d2e 6e61 6d65 0a20 2020 2020 2020  [0].name.       
+00018f10: 2020 2020 2020 2020 2066 6f72 2069 2c20           for i, 
+00018f20: 6120 696e 2065 6e75 6d65 7261 7465 2870  a in enumerate(p
+00018f30: 6c6f 745f 6461 7461 293a 0a20 2020 2020  lot_data):.     
+00018f40: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00018f50: 6e61 6d65 203d 2061 5b33 5d2e 7370 6c69  name = a[3].spli
+00018f60: 7428 222c 2229 5b30 5d0a 2020 2020 2020  t(",")[0].      
+00018f70: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00018f80: 206e 616d 6520 3d3d 2069 6e61 6d65 3a0a   name == iname:.
+00018f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018fa0: 2020 2020 2020 2020 6c65 6765 6e64 5f6f          legend_o
+00018fb0: 7264 6572 2e61 7070 656e 6428 6929 0a20  rder.append(i). 
+00018fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018fd0: 2020 2020 2020 2062 7265 616b 0a0a 2020         break..  
+00018fe0: 2020 2020 2020 656c 6966 2073 7461 636b        elif stack
+00018ff0: 7570 5f6d 6f64 6520 3d3d 2022 4f76 6572  up_mode == "Over
+00019000: 6c61 7070 696e 6722 3a0a 2020 2020 2020  lapping":.      
+00019010: 2020 2020 2020 6d69 6e5f 7468 6963 6b6e        min_thickn
+00019020: 6573 7320 3d20 6d69 6e28 5b69 5b33 5d20  ess = min([i[3] 
+00019030: 666f 7220 6920 696e 2073 6967 6e61 6c5f  for i in signal_
+00019040: 6c61 7965 7273 2069 6620 695b 335d 2021  layers if i[3] !
+00019050: 3d20 305d 290a 2020 2020 2020 2020 2020  = 0]).          
+00019060: 2020 636f 6c75 6d6e 7320 3d20 5b5d 2020    columns = []  
+00019070: 2320 6669 7273 7420 636f 6c75 6d6e 2069  # first column i
+00019080: 7320 783d 5b30 2c31 5d2c 2073 6563 6f6e  s x=[0,1], secon
+00019090: 6420 636f 6c75 6d6e 2069 7320 783d 5b31  d column is x=[1
+000190a0: 2c32 5d20 616e 6420 736f 206f 6e2e 2e2e  ,2] and so on...
+000190b0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+000190c0: 206c 7920 696e 2073 6967 6e61 6c5f 6c61   ly in signal_la
+000190d0: 7965 7273 3a0a 2020 2020 2020 2020 2020  yers:.          
+000190e0: 2020 2020 2020 6c6f 7765 725f 656c 6576        lower_elev
+000190f0: 6174 696f 6e20 3d20 6c79 5b31 5d20 2023  ation = ly[1]  #
+00019100: 206c 6f77 6572 2065 6c65 7661 7469 6f6e   lower elevation
+00019110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019120: 2074 203d 206c 795b 335d 2020 2320 7468   t = ly[3]  # th
+00019130: 6963 6b6e 6573 730a 2020 2020 2020 2020  ickness.        
+00019140: 2020 2020 2020 2020 7075 745f 696e 5f63          put_in_c
+00019150: 6f6c 756d 6e20 3d20 300a 2020 2020 2020  olumn = 0.      
+00019160: 2020 2020 2020 2020 2020 6365 6c6c 5f70            cell_p
+00019170: 6f73 6974 696f 6e20 3d20 300a 2020 2020  osition = 0.    
+00019180: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00019190: 6320 696e 2063 6f6c 756d 6e73 3a0a 2020  c in columns:.  
+000191a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000191b0: 2020 7565 7020 3d20 635b 2d31 5d5b 305d    uep = c[-1][0]
+000191c0: 5b32 5d20 2023 2075 7070 6572 2065 6c65  [2]  # upper ele
+000191d0: 7661 7469 6f6e 206f 6620 7468 6520 6c61  vation of the la
+000191e0: 7374 2065 6e74 7279 206f 6620 7468 6174  st entry of that
+000191f0: 2063 6f6c 756d 6e0a 2020 2020 2020 2020   column.        
+00019200: 2020 2020 2020 2020 2020 2020 7470 203d              tp =
+00019210: 2063 5b2d 315d 5b30 5d5b 335d 2020 2320   c[-1][0][3]  # 
+00019220: 7468 6963 6b6e 6573 7320 6f66 2074 6865  thickness of the
+00019230: 206c 6173 7420 656e 7472 7920 6f66 2074   last entry of t
+00019240: 6861 7420 636f 6c75 6d6e 0a20 2020 2020  hat column.     
+00019250: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00019260: 6620 6c6f 7765 725f 656c 6576 6174 696f  f lower_elevatio
+00019270: 6e20 3c20 7565 7020 6f72 2028 6162 7328  n < uep or (abs(
+00019280: 6c6f 7765 725f 656c 6576 6174 696f 6e20  lower_elevation 
+00019290: 2d20 7565 7029 203c 2031 652d 3135 2061  - uep) < 1e-15 a
+000192a0: 6e64 2074 7020 3d3d 2030 2061 6e64 2074  nd tp == 0 and t
+000192b0: 203d 3d20 3029 3a0a 2020 2020 2020 2020   == 0):.        
 000192c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000192d0: 2020 2070 7574 5f69 6e5f 636f 6c75 6d6e     put_in_column
-000192e0: 202b 3d20 310a 2020 2020 2020 2020 2020   += 1.          
-000192f0: 2020 2020 2020 2020 2020 2020 2020 6365                ce
-00019300: 6c6c 5f70 6f73 6974 696f 6e20 3d20 6c65  ll_position = le
-00019310: 6e28 6329 0a20 2020 2020 2020 2020 2020  n(c).           
-00019320: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+000192d0: 7075 745f 696e 5f63 6f6c 756d 6e20 2b3d  put_in_column +=
+000192e0: 2031 0a20 2020 2020 2020 2020 2020 2020   1.             
+000192f0: 2020 2020 2020 2020 2020 2063 656c 6c5f             cell_
+00019300: 706f 7369 7469 6f6e 203d 206c 656e 2863  position = len(c
+00019310: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00019320: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
 00019330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019340: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
-00019350: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00019360: 6c65 6e28 636f 6c75 6d6e 7329 203c 2070  len(columns) < p
-00019370: 7574 5f69 6e5f 636f 6c75 6d6e 202b 2031  ut_in_column + 1
-00019380: 3a20 2023 2061 6464 2061 206e 6577 2063  :  # add a new c
-00019390: 6f6c 756d 6e20 6966 2072 6571 7569 7265  olumn if require
-000193a0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-000193b0: 2020 2020 2020 636f 6c75 6d6e 732e 6170        columns.ap
-000193c0: 7065 6e64 285b 5d29 0a20 2020 2020 2020  pend([]).       
-000193d0: 2020 2020 2020 2020 2023 2070 7574 207a           # put z
-000193e0: 6572 6f73 2061 7420 7468 6520 6265 6769  eros at the begi
-000193f0: 6e6e 696e 6720 6f66 2074 6865 2063 6f6c  nning of the col
-00019400: 756d 6e20 756e 7469 6c20 7468 6572 6520  umn until there 
-00019410: 6973 2074 6865 2066 6972 7374 206c 6179  is the first lay
-00019420: 6572 0a20 2020 2020 2020 2020 2020 2020  er.             
-00019430: 2020 2069 6620 6365 6c6c 5f70 6f73 6974     if cell_posit
-00019440: 696f 6e20 213d 2030 3a0a 2020 2020 2020  ion != 0:.      
-00019450: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-00019460: 6c6c 5f63 656c 6c73 203d 2063 656c 6c5f  ll_cells = cell_
-00019470: 706f 7369 7469 6f6e 202d 2031 202d 206c  position - 1 - l
-00019480: 656e 2863 6f6c 756d 6e73 5b70 7574 5f69  en(columns[put_i
-00019490: 6e5f 636f 6c75 6d6e 5d29 0a20 2020 2020  n_column]).     
-000194a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000194b0: 6f72 2069 2069 6e20 7261 6e67 6528 6669  or i in range(fi
-000194c0: 6c6c 5f63 656c 6c73 293a 0a20 2020 2020  ll_cells):.     
+00019340: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
+00019350: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+00019360: 2863 6f6c 756d 6e73 2920 3c20 7075 745f  (columns) < put_
+00019370: 696e 5f63 6f6c 756d 6e20 2b20 313a 2020  in_column + 1:  
+00019380: 2320 6164 6420 6120 6e65 7720 636f 6c75  # add a new colu
+00019390: 6d6e 2069 6620 7265 7175 6972 6564 0a20  mn if required. 
+000193a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000193b0: 2020 2063 6f6c 756d 6e73 2e61 7070 656e     columns.appen
+000193c0: 6428 5b5d 290a 2020 2020 2020 2020 2020  d([]).          
+000193d0: 2020 2020 2020 2320 7075 7420 7a65 726f        # put zero
+000193e0: 7320 6174 2074 6865 2062 6567 696e 6e69  s at the beginni
+000193f0: 6e67 206f 6620 7468 6520 636f 6c75 6d6e  ng of the column
+00019400: 2075 6e74 696c 2074 6865 7265 2069 7320   until there is 
+00019410: 7468 6520 6669 7273 7420 6c61 7965 720a  the first layer.
+00019420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019430: 6966 2063 656c 6c5f 706f 7369 7469 6f6e  if cell_position
+00019440: 2021 3d20 303a 0a20 2020 2020 2020 2020   != 0:.         
+00019450: 2020 2020 2020 2020 2020 2066 696c 6c5f             fill_
+00019460: 6365 6c6c 7320 3d20 6365 6c6c 5f70 6f73  cells = cell_pos
+00019470: 6974 696f 6e20 2d20 3120 2d20 6c65 6e28  ition - 1 - len(
+00019480: 636f 6c75 6d6e 735b 7075 745f 696e 5f63  columns[put_in_c
+00019490: 6f6c 756d 6e5d 290a 2020 2020 2020 2020  olumn]).        
+000194a0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000194b0: 6920 696e 2072 616e 6765 2866 696c 6c5f  i in range(fill_
+000194c0: 6365 6c6c 7329 3a0a 2020 2020 2020 2020  cells):.        
 000194d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000194e0: 2020 2063 6f6c 756d 6e73 5b70 7574 5f69     columns[put_i
-000194f0: 6e5f 636f 6c75 6d6e 5d2e 6170 7065 6e64  n_column].append
-00019500: 2830 290a 2020 2020 2020 2020 2020 2020  (0).            
-00019510: 2020 2020 2320 6170 7065 6e64 2074 6865      # append the
-00019520: 206c 6179 6572 2074 6f20 7468 6520 7072   layer to the pr
-00019530: 6f70 6572 2063 6f6c 756d 6e20 616e 6420  oper column and 
-00019540: 726f 770a 2020 2020 2020 2020 2020 2020  row.            
-00019550: 2020 2020 7820 3d20 5b70 7574 5f69 6e5f      x = [put_in_
-00019560: 636f 6c75 6d6e 202b 2031 2c20 7075 745f  column + 1, put_
-00019570: 696e 5f63 6f6c 756d 6e20 2b20 312c 2070  in_column + 1, p
-00019580: 7574 5f69 6e5f 636f 6c75 6d6e 202b 2032  ut_in_column + 2
-00019590: 2c20 7075 745f 696e 5f63 6f6c 756d 6e20  , put_in_column 
-000195a0: 2b20 325d 0a20 2020 2020 2020 2020 2020  + 2].           
-000195b0: 2020 2020 2063 6f6c 756d 6e73 5b70 7574       columns[put
-000195c0: 5f69 6e5f 636f 6c75 6d6e 5d2e 6170 7065  _in_column].appe
-000195d0: 6e64 285b 6c79 2c20 785d 290a 0a20 2020  nd([ly, x])..   
-000195e0: 2020 2020 2020 2020 2023 2066 696c 6c20           # fill 
-000195f0: 7468 6520 636f 6c75 6d6e 7320 6d61 7472  the columns matr
-00019600: 6978 2077 6974 6820 7a65 726f 7320 6f6e  ix with zeros on
-00019610: 2074 6f70 0a20 2020 2020 2020 2020 2020   top.           
-00019620: 206e 5f72 6f77 7320 3d20 6d61 7828 5b6c   n_rows = max([l
-00019630: 656e 2869 2920 666f 7220 6920 696e 2063  en(i) for i in c
-00019640: 6f6c 756d 6e73 5d29 0a20 2020 2020 2020  olumns]).       
-00019650: 2020 2020 2066 6f72 2063 2069 6e20 636f       for c in co
-00019660: 6c75 6d6e 733a 0a20 2020 2020 2020 2020  lumns:.         
-00019670: 2020 2020 2020 2077 6869 6c65 206c 656e         while len
-00019680: 2863 2920 3c20 6e5f 726f 7773 3a0a 2020  (c) < n_rows:.  
-00019690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196a0: 2020 632e 6170 7065 6e64 2830 290a 2020    c.append(0).  
-000196b0: 2020 2020 2020 2020 2020 2320 6578 7061            # expa
-000196c0: 6e64 2074 6f20 7468 6520 7269 6768 7420  nd to the right 
-000196d0: 7468 6520 6669 6c6c 2066 6f72 2074 6865  the fill for the
-000196e0: 2073 6967 6e61 6c73 2074 6861 7420 6861   signals that ha
-000196f0: 7665 206e 6f20 6f76 6572 6c61 7020 6f6e  ve no overlap on
-00019700: 2074 6865 2072 6967 6874 0a20 2020 2020   the right.     
-00019710: 2020 2020 2020 2077 6964 7468 203d 206c         width = l
-00019720: 656e 2863 6f6c 756d 6e73 2920 2b20 310a  en(columns) + 1.
-00019730: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00019740: 692c 2063 2069 6e20 656e 756d 6572 6174  i, c in enumerat
-00019750: 6528 636f 6c75 6d6e 735b 3a2d 315d 293a  e(columns[:-1]):
-00019760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019770: 2066 6f72 206a 2c20 7220 696e 2065 6e75   for j, r in enu
-00019780: 6d65 7261 7465 2863 293a 0a20 2020 2020  merate(c):.     
-00019790: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000197a0: 6620 7220 213d 2030 3a20 2023 2061 6e64  f r != 0:  # and
-000197b0: 2064 6e61 6d65 203d 3d20 725b 305d 2e6e   dname == r[0].n
-000197c0: 616d 653a 0a20 2020 2020 2020 2020 2020  ame:.           
-000197d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000197e0: 636f 6c75 6d6e 735b 6920 2b20 315d 5b6a  columns[i + 1][j
-000197f0: 5d20 3d3d 2030 3a0a 2020 2020 2020 2020  ] == 0:.        
+000194e0: 636f 6c75 6d6e 735b 7075 745f 696e 5f63  columns[put_in_c
+000194f0: 6f6c 756d 6e5d 2e61 7070 656e 6428 3029  olumn].append(0)
+00019500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019510: 2023 2061 7070 656e 6420 7468 6520 6c61   # append the la
+00019520: 7965 7220 746f 2074 6865 2070 726f 7065  yer to the prope
+00019530: 7220 636f 6c75 6d6e 2061 6e64 2072 6f77  r column and row
+00019540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019550: 2078 203d 205b 7075 745f 696e 5f63 6f6c   x = [put_in_col
+00019560: 756d 6e20 2b20 312c 2070 7574 5f69 6e5f  umn + 1, put_in_
+00019570: 636f 6c75 6d6e 202b 2031 2c20 7075 745f  column + 1, put_
+00019580: 696e 5f63 6f6c 756d 6e20 2b20 322c 2070  in_column + 2, p
+00019590: 7574 5f69 6e5f 636f 6c75 6d6e 202b 2032  ut_in_column + 2
+000195a0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+000195b0: 2020 636f 6c75 6d6e 735b 7075 745f 696e    columns[put_in
+000195c0: 5f63 6f6c 756d 6e5d 2e61 7070 656e 6428  _column].append(
+000195d0: 5b6c 792c 2078 5d29 0a0a 2020 2020 2020  [ly, x])..      
+000195e0: 2020 2020 2020 2320 6669 6c6c 2074 6865        # fill the
+000195f0: 2063 6f6c 756d 6e73 206d 6174 7269 7820   columns matrix 
+00019600: 7769 7468 207a 6572 6f73 206f 6e20 746f  with zeros on to
+00019610: 700a 2020 2020 2020 2020 2020 2020 6e5f  p.            n_
+00019620: 726f 7773 203d 206d 6178 285b 6c65 6e28  rows = max([len(
+00019630: 6929 2066 6f72 2069 2069 6e20 636f 6c75  i) for i in colu
+00019640: 6d6e 735d 290a 2020 2020 2020 2020 2020  mns]).          
+00019650: 2020 666f 7220 6320 696e 2063 6f6c 756d    for c in colum
+00019660: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00019670: 2020 2020 7768 696c 6520 6c65 6e28 6329      while len(c)
+00019680: 203c 206e 5f72 6f77 733a 0a20 2020 2020   < n_rows:.     
+00019690: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000196a0: 2e61 7070 656e 6428 3029 0a20 2020 2020  .append(0).     
+000196b0: 2020 2020 2020 2023 2065 7870 616e 6420         # expand 
+000196c0: 746f 2074 6865 2072 6967 6874 2074 6865  to the right the
+000196d0: 2066 696c 6c20 666f 7220 7468 6520 7369   fill for the si
+000196e0: 676e 616c 7320 7468 6174 2068 6176 6520  gnals that have 
+000196f0: 6e6f 206f 7665 726c 6170 206f 6e20 7468  no overlap on th
+00019700: 6520 7269 6768 740a 2020 2020 2020 2020  e right.        
+00019710: 2020 2020 7769 6474 6820 3d20 6c65 6e28      width = len(
+00019720: 636f 6c75 6d6e 7329 202b 2031 0a20 2020  columns) + 1.   
+00019730: 2020 2020 2020 2020 2066 6f72 2069 2c20           for i, 
+00019740: 6320 696e 2065 6e75 6d65 7261 7465 2863  c in enumerate(c
+00019750: 6f6c 756d 6e73 5b3a 2d31 5d29 3a0a 2020  olumns[:-1]):.  
+00019760: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00019770: 7220 6a2c 2072 2069 6e20 656e 756d 6572  r j, r in enumer
+00019780: 6174 6528 6329 3a0a 2020 2020 2020 2020  ate(c):.        
+00019790: 2020 2020 2020 2020 2020 2020 6966 2072              if r
+000197a0: 2021 3d20 303a 2020 2320 616e 6420 646e   != 0:  # and dn
+000197b0: 616d 6520 3d3d 2072 5b30 5d2e 6e61 6d65  ame == r[0].name
+000197c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000197d0: 2020 2020 2020 2020 2020 6966 2063 6f6c            if col
+000197e0: 756d 6e73 5b69 202b 2031 5d5b 6a5d 203d  umns[i + 1][j] =
+000197f0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
 00019800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019810: 2020 2020 2320 6e6f 7468 696e 6720 6f6e      # nothing on
-00019820: 2074 6865 2072 6967 6874 2c20 736f 2065   the right, so e
-00019830: 7870 616e 6420 7468 6520 6669 6c6c 0a20  xpand the fill. 
+00019810: 2023 206e 6f74 6869 6e67 206f 6e20 7468   # nothing on th
+00019820: 6520 7269 6768 742c 2073 6f20 6578 7061  e right, so expa
+00019830: 6e64 2074 6865 2066 696c 6c0a 2020 2020  nd the fill.    
 00019840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019850: 2020 2020 2020 2020 2020 2078 203d 2072             x = r
-00019860: 5b31 5d0a 2020 2020 2020 2020 2020 2020  [1].            
-00019870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019880: 725b 315d 203d 205b 785b 305d 2c20 785b  r[1] = [x[0], x[
-00019890: 305d 2c20 7769 6474 682c 2077 6964 7468  0], width, width
-000198a0: 5d0a 0a20 2020 2020 2020 2020 2020 2066  ]..            f
-000198b0: 6f72 2063 2069 6e20 636f 6c75 6d6e 733a  or c in columns:
-000198c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000198d0: 2066 6f72 2072 2069 6e20 633a 0a20 2020   for r in c:.   
-000198e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000198f0: 2069 6620 7220 213d 2030 3a0a 2020 2020   if r != 0:.    
+00019850: 2020 2020 2020 2020 7820 3d20 725b 315d          x = r[1]
+00019860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019870: 2020 2020 2020 2020 2020 2020 2072 5b31               r[1
+00019880: 5d20 3d20 5b78 5b30 5d2c 2078 5b30 5d2c  ] = [x[0], x[0],
+00019890: 2077 6964 7468 2c20 7769 6474 685d 0a0a   width, width]..
+000198a0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000198b0: 6320 696e 2063 6f6c 756d 6e73 3a0a 2020  c in columns:.  
+000198c0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000198d0: 7220 7220 696e 2063 3a0a 2020 2020 2020  r r in c:.      
+000198e0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000198f0: 2072 2021 3d20 303a 0a20 2020 2020 2020   r != 0:.       
 00019900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019910: 2020 2020 6c79 203d 2072 5b30 5d0a 2020      ly = r[0].  
+00019910: 206c 7920 3d20 725b 305d 0a20 2020 2020   ly = r[0].     
 00019920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019930: 2020 2020 2020 6c61 7965 7220 3d20 6c79        layer = ly
-00019940: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-00019950: 2020 2020 2020 2020 2020 2020 7820 3d20              x = 
-00019960: 725b 315d 0a0a 2020 2020 2020 2020 2020  r[1]..          
-00019970: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00019980: 7365 7420 636f 6c6f 7220 616e 6420 6c61  set color and la
-00019990: 6265 6c0a 2020 2020 2020 2020 2020 2020  bel.            
-000199a0: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
-000199b0: 7220 3d20 5b66 6c6f 6174 2869 2920 2f20  r = [float(i) / 
-000199c0: 3235 3620 666f 7220 6920 696e 206c 6179  256 for i in lay
-000199d0: 6572 2e63 6f6c 6f72 5d0a 2020 2020 2020  er.color].      
-000199e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000199f0: 2020 6966 2063 6f6c 6f72 203d 3d20 5b31    if color == [1
-00019a00: 2e30 2c20 312e 302c 2031 2e30 5d3a 0a20  .0, 1.0, 1.0]:. 
+00019930: 2020 206c 6179 6572 203d 206c 795b 305d     layer = ly[0]
+00019940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019950: 2020 2020 2020 2020 2078 203d 2072 5b31           x = r[1
+00019960: 5d0a 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00019970: 2020 2020 2020 2020 2020 2023 2073 6574             # set
+00019980: 2063 6f6c 6f72 2061 6e64 206c 6162 656c   color and label
+00019990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000199a0: 2020 2020 2020 2020 2063 6f6c 6f72 203d           color =
+000199b0: 205b 666c 6f61 7428 6929 202f 2032 3536   [float(i) / 256
+000199c0: 2066 6f72 2069 2069 6e20 6c61 7965 722e   for i in layer.
+000199d0: 636f 6c6f 725d 0a20 2020 2020 2020 2020  color].         
+000199e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000199f0: 6620 636f 6c6f 7220 3d3d 205b 312e 302c  f color == [1.0,
+00019a00: 2031 2e30 2c20 312e 305d 3a0a 2020 2020   1.0, 1.0]:.    
 00019a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019a20: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
-00019a30: 203d 205b 302e 392c 2030 2e39 2c20 302e   = [0.9, 0.9, 0.
-00019a40: 395d 0a20 2020 2020 2020 2020 2020 2020  9].             
-00019a50: 2020 2020 2020 2020 2020 206c 6162 656c             label
-00019a60: 203d 2022 7b7d 2c20 7b7d 2c20 7468 6963   = "{}, {}, thic
-00019a70: 6b3a 207b 3a2e 3366 7d75 6d2c 2065 6c65  k: {:.3f}um, ele
-00019a80: 763a 207b 3a2e 3366 7d75 6d22 2e66 6f72  v: {:.3f}um".for
-00019a90: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
-00019aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ab0: 206c 6179 6572 2e6e 616d 652c 206c 6179   layer.name, lay
-00019ac0: 6572 2e6d 6174 6572 6961 6c2c 206c 6179  er.material, lay
-00019ad0: 6572 2e74 6869 636b 6e65 7373 202a 2031  er.thickness * 1
-00019ae0: 6536 2c20 6c61 7965 722e 6c6f 7765 725f  e6, layer.lower_
-00019af0: 656c 6576 6174 696f 6e20 2a20 3165 360a  elevation * 1e6.
+00019a20: 2020 2020 2020 2020 636f 6c6f 7220 3d20          color = 
+00019a30: 5b30 2e39 2c20 302e 392c 2030 2e39 5d0a  [0.9, 0.9, 0.9].
+00019a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a50: 2020 2020 2020 2020 6c61 6265 6c20 3d20          label = 
+00019a60: 227b 7d2c 207b 7d2c 2074 6869 636b 3a20  "{}, {}, thick: 
+00019a70: 7b3a 2e33 667d 756d 2c20 656c 6576 3a20  {:.3f}um, elev: 
+00019a80: 7b3a 2e33 667d 756d 222e 666f 726d 6174  {:.3f}um".format
+00019a90: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00019aa0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+00019ab0: 7965 722e 6e61 6d65 2c20 6c61 7965 722e  yer.name, layer.
+00019ac0: 6d61 7465 7269 616c 2c20 6c61 7965 722e  material, layer.
+00019ad0: 7468 6963 6b6e 6573 7320 2a20 3165 362c  thickness * 1e6,
+00019ae0: 206c 6179 6572 2e6c 6f77 6572 5f65 6c65   layer.lower_ele
+00019af0: 7661 7469 6f6e 202a 2031 6536 0a20 2020  vation * 1e6.   
 00019b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019b10: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00019b10: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
 00019b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019b30: 2020 2069 6620 6c79 5b33 5d20 3e20 303a     if ly[3] > 0:
-00019b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019b50: 2020 2020 2020 2020 2020 2020 206c 6f77               low
-00019b60: 6572 5f65 6c65 7661 7469 6f6e 203d 206c  er_elevation = l
-00019b70: 795b 315d 0a20 2020 2020 2020 2020 2020  y[1].           
-00019b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019b90: 2075 7070 6572 5f65 6c65 7661 7469 6f6e   upper_elevation
-00019ba0: 203d 206c 795b 325d 0a20 2020 2020 2020   = ly[2].       
+00019b30: 6966 206c 795b 335d 203e 2030 3a0a 2020  if ly[3] > 0:.  
+00019b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b50: 2020 2020 2020 2020 2020 6c6f 7765 725f            lower_
+00019b60: 656c 6576 6174 696f 6e20 3d20 6c79 5b31  elevation = ly[1
+00019b70: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00019b80: 2020 2020 2020 2020 2020 2020 2020 7570                up
+00019b90: 7065 725f 656c 6576 6174 696f 6e20 3d20  per_elevation = 
+00019ba0: 6c79 5b32 5d0a 2020 2020 2020 2020 2020  ly[2].          
 00019bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019bc0: 2020 2020 2079 203d 205b 6c6f 7765 725f       y = [lower_
-00019bd0: 656c 6576 6174 696f 6e2c 2075 7070 6572  elevation, upper
-00019be0: 5f65 6c65 7661 7469 6f6e 2c20 7570 7065  _elevation, uppe
-00019bf0: 725f 656c 6576 6174 696f 6e2c 206c 6f77  r_elevation, low
-00019c00: 6572 5f65 6c65 7661 7469 6f6e 5d0a 2020  er_elevation].  
+00019bc0: 2020 7920 3d20 5b6c 6f77 6572 5f65 6c65    y = [lower_ele
+00019bd0: 7661 7469 6f6e 2c20 7570 7065 725f 656c  vation, upper_el
+00019be0: 6576 6174 696f 6e2c 2075 7070 6572 5f65  evation, upper_e
+00019bf0: 6c65 7661 7469 6f6e 2c20 6c6f 7765 725f  levation, lower_
+00019c00: 656c 6576 6174 696f 6e5d 0a20 2020 2020  elevation].     
 00019c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c20: 2020 2020 2020 2020 2020 706c 6f74 5f64            plot_d
-00019c30: 6174 612e 696e 7365 7274 2830 2c20 5b78  ata.insert(0, [x
-00019c40: 2c20 792c 2063 6f6c 6f72 2c20 6c61 6265  , y, color, labe
-00019c50: 6c2c 2073 6967 6e61 6c5f 616c 7068 612c  l, signal_alpha,
-00019c60: 2022 6669 6c6c 225d 290a 2020 2020 2020   "fill"]).      
-00019c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c80: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00019c20: 2020 2020 2020 2070 6c6f 745f 6461 7461         plot_data
+00019c30: 2e69 6e73 6572 7428 302c 205b 782c 2079  .insert(0, [x, y
+00019c40: 2c20 636f 6c6f 722c 206c 6162 656c 2c20  , color, label, 
+00019c50: 7369 676e 616c 5f61 6c70 6861 2c20 2266  signal_alpha, "f
+00019c60: 696c 6c22 5d29 0a20 2020 2020 2020 2020  ill"]).         
+00019c70: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00019c80: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
 00019c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ca0: 2020 2020 6c6f 7765 725f 656c 6576 6174      lower_elevat
-00019cb0: 696f 6e20 3d20 6c79 5b31 5d20 2d20 6d69  ion = ly[1] - mi
-00019cc0: 6e5f 7468 6963 6b6e 6573 7320 2a20 302e  n_thickness * 0.
-00019cd0: 3120 2023 206d 616b 6520 7468 6520 7a65  1  # make the ze
-00019ce0: 726f 2074 6869 636b 6e65 7373 206c 6179  ro thickness lay
-00019cf0: 6572 7320 6d6f 7265 2076 6973 6962 6c65  ers more visible
-00019d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019d10: 2020 2020 2020 2020 2020 2020 2075 7070               upp
-00019d20: 6572 5f65 6c65 7661 7469 6f6e 203d 206c  er_elevation = l
-00019d30: 795b 325d 202b 206d 696e 5f74 6869 636b  y[2] + min_thick
-00019d40: 6e65 7373 202a 2030 2e31 0a20 2020 2020  ness * 0.1.     
+00019ca0: 206c 6f77 6572 5f65 6c65 7661 7469 6f6e   lower_elevation
+00019cb0: 203d 206c 795b 315d 202d 206d 696e 5f74   = ly[1] - min_t
+00019cc0: 6869 636b 6e65 7373 202a 2030 2e31 2020  hickness * 0.1  
+00019cd0: 2320 6d61 6b65 2074 6865 207a 6572 6f20  # make the zero 
+00019ce0: 7468 6963 6b6e 6573 7320 6c61 7965 7273  thickness layers
+00019cf0: 206d 6f72 6520 7669 7369 626c 650a 2020   more visible.  
+00019d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d10: 2020 2020 2020 2020 2020 7570 7065 725f            upper_
+00019d20: 656c 6576 6174 696f 6e20 3d20 6c79 5b32  elevation = ly[2
+00019d30: 5d20 2b20 6d69 6e5f 7468 6963 6b6e 6573  ] + min_thicknes
+00019d40: 7320 2a20 302e 310a 2020 2020 2020 2020  s * 0.1.        
 00019d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019d60: 2020 2020 2020 2079 203d 205b 6c6f 7765         y = [lowe
-00019d70: 725f 656c 6576 6174 696f 6e2c 2075 7070  r_elevation, upp
-00019d80: 6572 5f65 6c65 7661 7469 6f6e 2c20 7570  er_elevation, up
-00019d90: 7065 725f 656c 6576 6174 696f 6e2c 206c  per_elevation, l
-00019da0: 6f77 6572 5f65 6c65 7661 7469 6f6e 5d0a  ower_elevation].
+00019d60: 2020 2020 7920 3d20 5b6c 6f77 6572 5f65      y = [lower_e
+00019d70: 6c65 7661 7469 6f6e 2c20 7570 7065 725f  levation, upper_
+00019d80: 656c 6576 6174 696f 6e2c 2075 7070 6572  elevation, upper
+00019d90: 5f65 6c65 7661 7469 6f6e 2c20 6c6f 7765  _elevation, lowe
+00019da0: 725f 656c 6576 6174 696f 6e5d 0a20 2020  r_elevation].   
 00019db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019dc0: 2020 2020 2020 2020 2020 2020 2320 7075              # pu
-00019dd0: 7420 7468 6520 7a65 726f 2074 6869 636b  t the zero thick
-00019de0: 6e65 7373 206c 6179 6572 7320 6f6e 2074  ness layers on t
-00019df0: 6f70 0a20 2020 2020 2020 2020 2020 2020  op.             
-00019e00: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00019e10: 6c6f 745f 6461 7461 2e61 7070 656e 6428  lot_data.append(
-00019e20: 5b78 2c20 792c 2063 6f6c 6f72 2c20 6c61  [x, y, color, la
-00019e30: 6265 6c2c 207a 6572 6f5f 7468 6963 6b6e  bel, zero_thickn
-00019e40: 6573 735f 616c 7068 612c 2022 6669 6c6c  ess_alpha, "fill
-00019e50: 225d 290a 0a20 2020 2020 2020 2020 2020  "])..           
-00019e60: 2020 2020 2020 2020 2020 2020 2023 2063               # c
-00019e70: 7265 6174 6520 616e 6e6f 7461 7469 6f6e  reate annotation
-00019e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019e90: 2020 2020 2020 2020 2078 5f70 6f73 203d           x_pos =
-00019ea0: 2031 2e30 0a20 2020 2020 2020 2020 2020   1.0.           
-00019eb0: 2020 2020 2020 2020 2020 2020 2079 5f70               y_p
-00019ec0: 6f73 203d 2028 6c6f 7765 725f 656c 6576  os = (lower_elev
-00019ed0: 6174 696f 6e20 2b20 7570 7065 725f 656c  ation + upper_el
-00019ee0: 6576 6174 696f 6e29 202f 2032 0a20 2020  evation) / 2.   
+00019dc0: 2020 2020 2020 2020 2023 2070 7574 2074           # put t
+00019dd0: 6865 207a 6572 6f20 7468 6963 6b6e 6573  he zero thicknes
+00019de0: 7320 6c61 7965 7273 206f 6e20 746f 700a  s layers on top.
+00019df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e00: 2020 2020 2020 2020 2020 2020 706c 6f74              plot
+00019e10: 5f64 6174 612e 6170 7065 6e64 285b 782c  _data.append([x,
+00019e20: 2079 2c20 636f 6c6f 722c 206c 6162 656c   y, color, label
+00019e30: 2c20 7a65 726f 5f74 6869 636b 6e65 7373  , zero_thickness
+00019e40: 5f61 6c70 6861 2c20 2266 696c 6c22 5d29  _alpha, "fill"])
+00019e50: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019e60: 2020 2020 2020 2020 2020 2320 6372 6561            # crea
+00019e70: 7465 2061 6e6e 6f74 6174 696f 6e0a 2020  te annotation.  
+00019e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e90: 2020 2020 2020 785f 706f 7320 3d20 312e        x_pos = 1.
+00019ea0: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
+00019eb0: 2020 2020 2020 2020 2020 795f 706f 7320            y_pos 
+00019ec0: 3d20 286c 6f77 6572 5f65 6c65 7661 7469  = (lower_elevati
+00019ed0: 6f6e 202b 2075 7070 6572 5f65 6c65 7661  on + upper_eleva
+00019ee0: 7469 6f6e 2920 2f20 320a 2020 2020 2020  tion) / 2.      
 00019ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019f00: 2020 2020 2061 6e6e 6f74 6174 696f 6e73       annotations
-00019f10: 2e61 7070 656e 6428 5b78 5f70 6f73 2c20  .append([x_pos, 
-00019f20: 795f 706f 732c 206c 6179 6572 2e6e 616d  y_pos, layer.nam
-00019f30: 652c 207b 2266 6f6e 7473 697a 6522 3a20  e, {"fontsize": 
-00019f40: 616e 6e6f 7461 7469 6f6e 5f66 6f6e 7473  annotation_fonts
-00019f50: 697a 657d 5d29 0a0a 2020 2020 2020 2020  ize}])..        
-00019f60: 2020 2020 2320 6f72 6465 7220 7468 6520      # order the 
-00019f70: 616e 6e6f 7461 7469 6f6e 7320 6261 7365  annotations base
-00019f80: 6420 6f6e 2079 5f70 6f73 2028 6974 2069  d on y_pos (it i
-00019f90: 7320 6e65 6365 7373 6172 7920 6c61 7465  s necessary late
-00019fa0: 7220 746f 206d 6f76 6520 7468 656d 2074  r to move them t
-00019fb0: 6f20 6176 6f69 6420 7465 7874 206f 7665  o avoid text ove
-00019fc0: 726c 6170 7069 6e67 290a 2020 2020 2020  rlapping).      
-00019fd0: 2020 2020 2020 616e 6e6f 7461 7469 6f6e        annotation
-00019fe0: 732e 736f 7274 286b 6579 3d6c 616d 6264  s.sort(key=lambd
-00019ff0: 6120 653a 2065 5b31 5d29 0a20 2020 2020  a e: e[1]).     
-0001a000: 2020 2020 2020 2023 206d 6f76 6520 616c         # move al
-0001a010: 6c20 7468 6520 616e 6e6f 7461 7469 6f6e  l the annotation
-0001a020: 7320 746f 2074 6865 2066 696e 616c 2078  s to the final x
-0001a030: 2028 6974 2063 6f75 6c64 2062 6520 6c61   (it could be la
-0001a040: 7267 6572 2074 6861 6e20 3120 6475 6520  rger than 1 due 
-0001a050: 746f 2061 6464 6974 696f 6e61 6c20 636f  to additional co
-0001a060: 6c75 6d6e 7329 0a20 2020 2020 2020 2020  lumns).         
-0001a070: 2020 2077 6964 7468 203d 206c 656e 2863     width = len(c
-0001a080: 6f6c 756d 6e73 2920 2b20 310a 2020 2020  olumns) + 1.    
-0001a090: 2020 2020 2020 2020 666f 7220 692c 2061          for i, a
-0001a0a0: 2069 6e20 656e 756d 6572 6174 6528 616e   in enumerate(an
-0001a0b0: 6e6f 7461 7469 6f6e 7329 3a0a 2020 2020  notations):.    
-0001a0c0: 2020 2020 2020 2020 2020 2020 615b 305d              a[0]
-0001a0d0: 203d 2077 6964 7468 202b 2061 6e6e 6f74   = width + annot
-0001a0e0: 6174 696f 6e5f 785f 6d61 7267 696e 202a  ation_x_margin *
-0001a0f0: 2077 6964 7468 0a0a 2020 2020 2020 2020   width..        
-0001a100: 2020 2020 666f 7220 6c79 2069 6e20 6469      for ly in di
-0001a110: 656c 6563 7472 6963 5f6c 6179 6572 733a  electric_layers:
-0001a120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a130: 206c 6179 6572 203d 206c 795b 305d 0a20   layer = ly[0]. 
-0001a140: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0001a150: 2073 6574 2063 6f6c 6f72 2061 6e64 206c   set color and l
-0001a160: 6162 656c 0a20 2020 2020 2020 2020 2020  abel.           
-0001a170: 2020 2020 2063 6f6c 6f72 203d 205b 666c       color = [fl
-0001a180: 6f61 7428 6929 202f 2032 3536 2066 6f72  oat(i) / 256 for
-0001a190: 2069 2069 6e20 6c61 7965 722e 636f 6c6f   i in layer.colo
-0001a1a0: 725d 0a20 2020 2020 2020 2020 2020 2020  r].             
-0001a1b0: 2020 2069 6620 636f 6c6f 7220 3d3d 205b     if color == [
-0001a1c0: 312e 302c 2031 2e30 2c20 312e 305d 3a0a  1.0, 1.0, 1.0]:.
+00019f00: 2020 616e 6e6f 7461 7469 6f6e 732e 6170    annotations.ap
+00019f10: 7065 6e64 285b 785f 706f 732c 2079 5f70  pend([x_pos, y_p
+00019f20: 6f73 2c20 6c61 7965 722e 6e61 6d65 2c20  os, layer.name, 
+00019f30: 7b22 666f 6e74 7369 7a65 223a 2061 6e6e  {"fontsize": ann
+00019f40: 6f74 6174 696f 6e5f 666f 6e74 7369 7a65  otation_fontsize
+00019f50: 7d5d 290a 0a20 2020 2020 2020 2020 2020  }])..           
+00019f60: 2023 206f 7264 6572 2074 6865 2061 6e6e   # order the ann
+00019f70: 6f74 6174 696f 6e73 2062 6173 6564 206f  otations based o
+00019f80: 6e20 795f 706f 7320 2869 7420 6973 206e  n y_pos (it is n
+00019f90: 6563 6573 7361 7279 206c 6174 6572 2074  ecessary later t
+00019fa0: 6f20 6d6f 7665 2074 6865 6d20 746f 2061  o move them to a
+00019fb0: 766f 6964 2074 6578 7420 6f76 6572 6c61  void text overla
+00019fc0: 7070 696e 6729 0a20 2020 2020 2020 2020  pping).         
+00019fd0: 2020 2061 6e6e 6f74 6174 696f 6e73 2e73     annotations.s
+00019fe0: 6f72 7428 6b65 793d 6c61 6d62 6461 2065  ort(key=lambda e
+00019ff0: 3a20 655b 315d 290a 2020 2020 2020 2020  : e[1]).        
+0001a000: 2020 2020 2320 6d6f 7665 2061 6c6c 2074      # move all t
+0001a010: 6865 2061 6e6e 6f74 6174 696f 6e73 2074  he annotations t
+0001a020: 6f20 7468 6520 6669 6e61 6c20 7820 2869  o the final x (i
+0001a030: 7420 636f 756c 6420 6265 206c 6172 6765  t could be large
+0001a040: 7220 7468 616e 2031 2064 7565 2074 6f20  r than 1 due to 
+0001a050: 6164 6469 7469 6f6e 616c 2063 6f6c 756d  additional colum
+0001a060: 6e73 290a 2020 2020 2020 2020 2020 2020  ns).            
+0001a070: 7769 6474 6820 3d20 6c65 6e28 636f 6c75  width = len(colu
+0001a080: 6d6e 7329 202b 2031 0a20 2020 2020 2020  mns) + 1.       
+0001a090: 2020 2020 2066 6f72 2069 2c20 6120 696e       for i, a in
+0001a0a0: 2065 6e75 6d65 7261 7465 2861 6e6e 6f74   enumerate(annot
+0001a0b0: 6174 696f 6e73 293a 0a20 2020 2020 2020  ations):.       
+0001a0c0: 2020 2020 2020 2020 2061 5b30 5d20 3d20           a[0] = 
+0001a0d0: 7769 6474 6820 2b20 616e 6e6f 7461 7469  width + annotati
+0001a0e0: 6f6e 5f78 5f6d 6172 6769 6e20 2a20 7769  on_x_margin * wi
+0001a0f0: 6474 680a 0a20 2020 2020 2020 2020 2020  dth..           
+0001a100: 2066 6f72 206c 7920 696e 2064 6965 6c65   for ly in diele
+0001a110: 6374 7269 635f 6c61 7965 7273 3a0a 2020  ctric_layers:.  
+0001a120: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+0001a130: 7965 7220 3d20 6c79 5b30 5d0a 2020 2020  yer = ly[0].    
+0001a140: 2020 2020 2020 2020 2020 2020 2320 7365              # se
+0001a150: 7420 636f 6c6f 7220 616e 6420 6c61 6265  t color and labe
+0001a160: 6c0a 2020 2020 2020 2020 2020 2020 2020  l.              
+0001a170: 2020 636f 6c6f 7220 3d20 5b66 6c6f 6174    color = [float
+0001a180: 2869 2920 2f20 3235 3620 666f 7220 6920  (i) / 256 for i 
+0001a190: 696e 206c 6179 6572 2e63 6f6c 6f72 5d0a  in layer.color].
+0001a1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a1b0: 6966 2063 6f6c 6f72 203d 3d20 5b31 2e30  if color == [1.0
+0001a1c0: 2c20 312e 302c 2031 2e30 5d3a 0a20 2020  , 1.0, 1.0]:.   
 0001a1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a1e0: 2020 2020 636f 6c6f 7220 3d20 5b30 2e39      color = [0.9
-0001a1f0: 2c20 302e 392c 2030 2e39 5d0a 2020 2020  , 0.9, 0.9].    
-0001a200: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
-0001a210: 6c20 3d20 227b 7d2c 207b 7d2c 2074 6869  l = "{}, {}, thi
-0001a220: 636b 3a20 7b3a 2e33 667d 756d 2c20 656c  ck: {:.3f}um, el
-0001a230: 6576 3a20 7b3a 2e33 667d 756d 222e 666f  ev: {:.3f}um".fo
-0001a240: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-0001a250: 2020 2020 2020 2020 2020 6c61 7965 722e            layer.
-0001a260: 6e61 6d65 2c20 6c61 7965 722e 6d61 7465  name, layer.mate
-0001a270: 7269 616c 2c20 6c61 7965 722e 7468 6963  rial, layer.thic
-0001a280: 6b6e 6573 7320 2a20 3165 362c 206c 6179  kness * 1e6, lay
-0001a290: 6572 2e6c 6f77 6572 5f65 6c65 7661 7469  er.lower_elevati
-0001a2a0: 6f6e 202a 2031 6536 0a20 2020 2020 2020  on * 1e6.       
-0001a2b0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0001a2c0: 2020 2020 2020 2020 2020 2023 2063 7265             # cre
-0001a2d0: 6174 6520 7468 6520 7061 7463 680a 2020  ate the patch.  
-0001a2e0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-0001a2f0: 7765 725f 656c 6576 6174 696f 6e20 3d20  wer_elevation = 
-0001a300: 6c79 5b31 5d0a 2020 2020 2020 2020 2020  ly[1].          
-0001a310: 2020 2020 2020 7570 7065 725f 656c 6576        upper_elev
-0001a320: 6174 696f 6e20 3d20 6c79 5b32 5d0a 2020  ation = ly[2].  
-0001a330: 2020 2020 2020 2020 2020 2020 2020 7920                y 
-0001a340: 3d20 5b6c 6f77 6572 5f65 6c65 7661 7469  = [lower_elevati
-0001a350: 6f6e 2c20 7570 7065 725f 656c 6576 6174  on, upper_elevat
-0001a360: 696f 6e2c 2075 7070 6572 5f65 6c65 7661  ion, upper_eleva
-0001a370: 7469 6f6e 2c20 6c6f 7765 725f 656c 6576  tion, lower_elev
-0001a380: 6174 696f 6e5d 0a20 2020 2020 2020 2020  ation].         
-0001a390: 2020 2020 2020 2078 203d 205b 302c 2030         x = [0, 0
-0001a3a0: 2c20 7769 6474 682c 2077 6964 7468 5d0a  , width, width].
-0001a3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a3c0: 706c 6f74 5f64 6174 612e 696e 7365 7274  plot_data.insert
-0001a3d0: 2830 2c20 5b78 2c20 792c 2063 6f6c 6f72  (0, [x, y, color
-0001a3e0: 2c20 6c61 6265 6c2c 2064 6965 6c5f 616c  , label, diel_al
-0001a3f0: 7068 612c 2022 6669 6c6c 225d 290a 0a20  pha, "fill"]).. 
-0001a400: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0001a410: 2063 7265 6174 6520 616e 6e6f 7461 7469   create annotati
-0001a420: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
-0001a430: 2020 2078 5f70 6f73 203d 202d 616e 6e6f     x_pos = -anno
-0001a440: 7461 7469 6f6e 5f78 5f6d 6172 6769 6e20  tation_x_margin 
-0001a450: 2a20 7769 6474 680a 2020 2020 2020 2020  * width.        
-0001a460: 2020 2020 2020 2020 795f 706f 7320 3d20          y_pos = 
-0001a470: 286c 6f77 6572 5f65 6c65 7661 7469 6f6e  (lower_elevation
-0001a480: 202b 2075 7070 6572 5f65 6c65 7661 7469   + upper_elevati
-0001a490: 6f6e 2920 2f20 320a 2020 2020 2020 2020  on) / 2.        
-0001a4a0: 2020 2020 2020 2020 616e 6e6f 7461 7469          annotati
-0001a4b0: 6f6e 732e 6170 7065 6e64 280a 2020 2020  ons.append(.    
-0001a4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a4d0: 5b78 5f70 6f73 2c20 795f 706f 732c 206c  [x_pos, y_pos, l
-0001a4e0: 6179 6572 2e6e 616d 652c 207b 2266 6f6e  ayer.name, {"fon
-0001a4f0: 7473 697a 6522 3a20 616e 6e6f 7461 7469  tsize": annotati
-0001a500: 6f6e 5f66 6f6e 7473 697a 652c 2022 686f  on_fontsize, "ho
-0001a510: 7269 7a6f 6e74 616c 616c 6967 6e6d 656e  rizontalalignmen
-0001a520: 7422 3a20 2272 6967 6874 227d 5d0a 2020  t": "right"}].  
-0001a530: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0001a540: 0a20 2020 2020 2020 2020 2020 2023 2065  .            # e
-0001a550: 7661 6c75 6174 6520 7468 6520 6c65 6765  valuate the lege
-0001a560: 6e64 2072 656f 7264 6572 0a20 2020 2020  nd reorder.     
-0001a570: 2020 2020 2020 206c 6567 656e 645f 6f72         legend_or
-0001a580: 6465 7220 3d20 5b5d 0a20 2020 2020 2020  der = [].       
-0001a590: 2020 2020 2066 6f72 206c 7920 696e 2064       for ly in d
-0001a5a0: 6965 6c65 6374 7269 635f 6c61 7965 7273  ielectric_layers
-0001a5b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001a5c0: 2020 6e61 6d65 203d 206c 795b 305d 2e6e    name = ly[0].n
-0001a5d0: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
-0001a5e0: 2020 2020 666f 7220 692c 2061 2069 6e20      for i, a in 
-0001a5f0: 656e 756d 6572 6174 6528 706c 6f74 5f64  enumerate(plot_d
-0001a600: 6174 6129 3a0a 2020 2020 2020 2020 2020  ata):.          
-0001a610: 2020 2020 2020 2020 2020 696e 616d 6520            iname 
-0001a620: 3d20 615b 335d 2e73 706c 6974 2822 2c22  = a[3].split(","
-0001a630: 295b 305d 0a20 2020 2020 2020 2020 2020  )[0].           
-0001a640: 2020 2020 2020 2020 2069 6620 6e61 6d65           if name
-0001a650: 203d 3d20 696e 616d 653a 0a20 2020 2020   == iname:.     
+0001a1e0: 2063 6f6c 6f72 203d 205b 302e 392c 2030   color = [0.9, 0
+0001a1f0: 2e39 2c20 302e 395d 0a20 2020 2020 2020  .9, 0.9].       
+0001a200: 2020 2020 2020 2020 206c 6162 656c 203d           label =
+0001a210: 2022 7b7d 2c20 7b7d 2c20 7468 6963 6b3a   "{}, {}, thick:
+0001a220: 207b 3a2e 3366 7d75 6d2c 2065 6c65 763a   {:.3f}um, elev:
+0001a230: 207b 3a2e 3366 7d75 6d22 2e66 6f72 6d61   {:.3f}um".forma
+0001a240: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+0001a250: 2020 2020 2020 206c 6179 6572 2e6e 616d         layer.nam
+0001a260: 652c 206c 6179 6572 2e6d 6174 6572 6961  e, layer.materia
+0001a270: 6c2c 206c 6179 6572 2e74 6869 636b 6e65  l, layer.thickne
+0001a280: 7373 202a 2031 6536 2c20 6c61 7965 722e  ss * 1e6, layer.
+0001a290: 6c6f 7765 725f 656c 6576 6174 696f 6e20  lower_elevation 
+0001a2a0: 2a20 3165 360a 2020 2020 2020 2020 2020  * 1e6.          
+0001a2b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001a2c0: 2020 2020 2020 2020 2320 6372 6561 7465          # create
+0001a2d0: 2074 6865 2070 6174 6368 0a20 2020 2020   the patch.     
+0001a2e0: 2020 2020 2020 2020 2020 206c 6f77 6572             lower
+0001a2f0: 5f65 6c65 7661 7469 6f6e 203d 206c 795b  _elevation = ly[
+0001a300: 315d 0a20 2020 2020 2020 2020 2020 2020  1].             
+0001a310: 2020 2075 7070 6572 5f65 6c65 7661 7469     upper_elevati
+0001a320: 6f6e 203d 206c 795b 325d 0a20 2020 2020  on = ly[2].     
+0001a330: 2020 2020 2020 2020 2020 2079 203d 205b             y = [
+0001a340: 6c6f 7765 725f 656c 6576 6174 696f 6e2c  lower_elevation,
+0001a350: 2075 7070 6572 5f65 6c65 7661 7469 6f6e   upper_elevation
+0001a360: 2c20 7570 7065 725f 656c 6576 6174 696f  , upper_elevatio
+0001a370: 6e2c 206c 6f77 6572 5f65 6c65 7661 7469  n, lower_elevati
+0001a380: 6f6e 5d0a 2020 2020 2020 2020 2020 2020  on].            
+0001a390: 2020 2020 7820 3d20 5b30 2c20 302c 2077      x = [0, 0, w
+0001a3a0: 6964 7468 2c20 7769 6474 685d 0a20 2020  idth, width].   
+0001a3b0: 2020 2020 2020 2020 2020 2020 2070 6c6f               plo
+0001a3c0: 745f 6461 7461 2e69 6e73 6572 7428 302c  t_data.insert(0,
+0001a3d0: 205b 782c 2079 2c20 636f 6c6f 722c 206c   [x, y, color, l
+0001a3e0: 6162 656c 2c20 6469 656c 5f61 6c70 6861  abel, diel_alpha
+0001a3f0: 2c20 2266 696c 6c22 5d29 0a0a 2020 2020  , "fill"])..    
+0001a400: 2020 2020 2020 2020 2020 2020 2320 6372              # cr
+0001a410: 6561 7465 2061 6e6e 6f74 6174 696f 6e0a  eate annotation.
+0001a420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a430: 785f 706f 7320 3d20 2d61 6e6e 6f74 6174  x_pos = -annotat
+0001a440: 696f 6e5f 785f 6d61 7267 696e 202a 2077  ion_x_margin * w
+0001a450: 6964 7468 0a20 2020 2020 2020 2020 2020  idth.           
+0001a460: 2020 2020 2079 5f70 6f73 203d 2028 6c6f       y_pos = (lo
+0001a470: 7765 725f 656c 6576 6174 696f 6e20 2b20  wer_elevation + 
+0001a480: 7570 7065 725f 656c 6576 6174 696f 6e29  upper_elevation)
+0001a490: 202f 2032 0a20 2020 2020 2020 2020 2020   / 2.           
+0001a4a0: 2020 2020 2061 6e6e 6f74 6174 696f 6e73       annotations
+0001a4b0: 2e61 7070 656e 6428 0a20 2020 2020 2020  .append(.       
+0001a4c0: 2020 2020 2020 2020 2020 2020 205b 785f               [x_
+0001a4d0: 706f 732c 2079 5f70 6f73 2c20 6c61 7965  pos, y_pos, laye
+0001a4e0: 722e 6e61 6d65 2c20 7b22 666f 6e74 7369  r.name, {"fontsi
+0001a4f0: 7a65 223a 2061 6e6e 6f74 6174 696f 6e5f  ze": annotation_
+0001a500: 666f 6e74 7369 7a65 2c20 2268 6f72 697a  fontsize, "horiz
+0001a510: 6f6e 7461 6c61 6c69 676e 6d65 6e74 223a  ontalalignment":
+0001a520: 2022 7269 6768 7422 7d5d 0a20 2020 2020   "right"}].     
+0001a530: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0001a540: 2020 2020 2020 2020 2020 2320 6576 616c            # eval
+0001a550: 7561 7465 2074 6865 206c 6567 656e 6420  uate the legend 
+0001a560: 7265 6f72 6465 720a 2020 2020 2020 2020  reorder.        
+0001a570: 2020 2020 6c65 6765 6e64 5f6f 7264 6572      legend_order
+0001a580: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
+0001a590: 2020 666f 7220 6c79 2069 6e20 6469 656c    for ly in diel
+0001a5a0: 6563 7472 6963 5f6c 6179 6572 733a 0a20  ectric_layers:. 
+0001a5b0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0001a5c0: 616d 6520 3d20 6c79 5b30 5d2e 6e61 6d65  ame = ly[0].name
+0001a5d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a5e0: 2066 6f72 2069 2c20 6120 696e 2065 6e75   for i, a in enu
+0001a5f0: 6d65 7261 7465 2870 6c6f 745f 6461 7461  merate(plot_data
+0001a600: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0001a610: 2020 2020 2020 2069 6e61 6d65 203d 2061         iname = a
+0001a620: 5b33 5d2e 7370 6c69 7428 222c 2229 5b30  [3].split(",")[0
+0001a630: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0001a640: 2020 2020 2020 6966 206e 616d 6520 3d3d        if name ==
+0001a650: 2069 6e61 6d65 3a0a 2020 2020 2020 2020   iname:.        
 0001a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a670: 2020 206c 6567 656e 645f 6f72 6465 722e     legend_order.
-0001a680: 6170 7065 6e64 2869 290a 2020 2020 2020  append(i).      
-0001a690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a6a0: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
-0001a6b0: 2020 2020 666f 7220 6c79 2069 6e20 7369      for ly in si
-0001a6c0: 676e 616c 5f6c 6179 6572 733a 0a20 2020  gnal_layers:.   
-0001a6d0: 2020 2020 2020 2020 2020 2020 206e 616d               nam
-0001a6e0: 6520 3d20 6c79 5b30 5d2e 6e61 6d65 0a20  e = ly[0].name. 
-0001a6f0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0001a700: 6f72 2069 2c20 6120 696e 2065 6e75 6d65  or i, a in enume
-0001a710: 7261 7465 2870 6c6f 745f 6461 7461 293a  rate(plot_data):
-0001a720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a730: 2020 2020 2069 6e61 6d65 203d 2061 5b33       iname = a[3
-0001a740: 5d2e 7370 6c69 7428 222c 2229 5b30 5d0a  ].split(",")[0].
+0001a670: 6c65 6765 6e64 5f6f 7264 6572 2e61 7070  legend_order.app
+0001a680: 656e 6428 6929 0a20 2020 2020 2020 2020  end(i).         
+0001a690: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0001a6a0: 7265 616b 0a20 2020 2020 2020 2020 2020  reak.           
+0001a6b0: 2066 6f72 206c 7920 696e 2073 6967 6e61   for ly in signa
+0001a6c0: 6c5f 6c61 7965 7273 3a0a 2020 2020 2020  l_layers:.      
+0001a6d0: 2020 2020 2020 2020 2020 6e61 6d65 203d            name =
+0001a6e0: 206c 795b 305d 2e6e 616d 650a 2020 2020   ly[0].name.    
+0001a6f0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0001a700: 692c 2061 2069 6e20 656e 756d 6572 6174  i, a in enumerat
+0001a710: 6528 706c 6f74 5f64 6174 6129 3a0a 2020  e(plot_data):.  
+0001a720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a730: 2020 696e 616d 6520 3d20 615b 335d 2e73    iname = a[3].s
+0001a740: 706c 6974 2822 2c22 295b 305d 0a20 2020  plit(",")[0].   
 0001a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a760: 2020 2020 6966 206e 616d 6520 3d3d 2069      if name == i
-0001a770: 6e61 6d65 3a0a 2020 2020 2020 2020 2020  name:.          
-0001a780: 2020 2020 2020 2020 2020 2020 2020 6c65                le
-0001a790: 6765 6e64 5f6f 7264 6572 2e61 7070 656e  gend_order.appen
-0001a7a0: 6428 6929 0a20 2020 2020 2020 2020 2020  d(i).           
-0001a7b0: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-0001a7c0: 616b 0a0a 2020 2020 2020 2020 2320 6361  ak..        # ca
-0001a7d0: 6c63 756c 6174 6520 7468 6520 6578 7472  lculate the extr
-0001a7e0: 656d 6974 6965 7320 6f66 2074 6865 2070  emities of the p
-0001a7f0: 6c6f 740a 2020 2020 2020 2020 785f 6d69  lot.        x_mi
-0001a800: 6e20 3d20 302e 300a 2020 2020 2020 2020  n = 0.0.        
-0001a810: 785f 6d61 7820 3d20 6d61 7828 5b6d 6178  x_max = max([max
-0001a820: 2869 5b30 5d29 2066 6f72 2069 2069 6e20  (i[0]) for i in 
-0001a830: 706c 6f74 5f64 6174 615d 290a 2020 2020  plot_data]).    
-0001a840: 2020 2020 6966 2073 7461 636b 7570 5f6d      if stackup_m
-0001a850: 6f64 6520 3d3d 2022 4c61 6d69 6e61 7465  ode == "Laminate
-0001a860: 223a 0a20 2020 2020 2020 2020 2020 2079  ":.            y
-0001a870: 5f6d 696e 203d 206c 6179 6572 735f 6461  _min = layers_da
-0001a880: 7461 5b30 5d5b 315d 0a20 2020 2020 2020  ta[0][1].       
-0001a890: 2020 2020 2079 5f6d 6178 203d 206c 6179       y_max = lay
-0001a8a0: 6572 735f 6461 7461 5b2d 315d 5b32 5d0a  ers_data[-1][2].
-0001a8b0: 2020 2020 2020 2020 656c 6966 2073 7461          elif sta
-0001a8c0: 636b 7570 5f6d 6f64 6520 3d3d 2022 4f76  ckup_mode == "Ov
-0001a8d0: 6572 6c61 7070 696e 6722 3a0a 2020 2020  erlapping":.    
-0001a8e0: 2020 2020 2020 2020 795f 6d69 6e20 3d20          y_min = 
-0001a8f0: 6d69 6e28 6469 656c 6563 7472 6963 5f6c  min(dielectric_l
-0001a900: 6179 6572 735b 305d 5b31 5d2c 2073 6967  ayers[0][1], sig
-0001a910: 6e61 6c5f 6c61 7965 7273 5b30 5d5b 315d  nal_layers[0][1]
-0001a920: 290a 2020 2020 2020 2020 2020 2020 795f  ).            y_
-0001a930: 6d61 7820 3d20 6d61 7828 6469 656c 6563  max = max(dielec
-0001a940: 7472 6963 5f6c 6179 6572 735b 2d31 5d5b  tric_layers[-1][
-0001a950: 325d 2c20 7369 676e 616c 5f6c 6179 6572  2], signal_layer
-0001a960: 735b 2d31 5d5b 325d 290a 0a20 2020 2020  s[-1][2])..     
-0001a970: 2020 2023 206d 6f76 6520 7468 6520 616e     # move the an
-0001a980: 6e6f 7461 7469 6f6e 7320 746f 2061 766f  notations to avo
-0001a990: 6964 2074 6578 7420 6f76 6572 6c61 7070  id text overlapp
-0001a9a0: 696e 670a 2020 2020 2020 2020 6e65 775f  ing.        new_
-0001a9b0: 616e 6e6f 7461 7469 6f6e 7320 3d20 5b5d  annotations = []
-0001a9c0: 0a20 2020 2020 2020 2066 6f72 2069 2c20  .        for i, 
-0001a9d0: 6120 696e 2065 6e75 6d65 7261 7465 2861  a in enumerate(a
-0001a9e0: 6e6e 6f74 6174 696f 6e73 293a 0a20 2020  nnotations):.   
-0001a9f0: 2020 2020 2020 2020 2069 6620 6920 3e20           if i > 
-0001aa00: 3020 616e 6420 6162 7328 615b 315d 202d  0 and abs(a[1] -
-0001aa10: 2061 6e6e 6f74 6174 696f 6e73 5b69 202d   annotations[i -
-0001aa20: 2031 5d5b 315d 2920 3c20 2879 5f6d 6178   1][1]) < (y_max
-0001aa30: 202d 2079 5f6d 696e 2920 2f20 3735 3a0a   - y_min) / 75:.
-0001aa40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa50: 6e65 775f 616e 6e6f 7461 7469 6f6e 735b  new_annotations[
-0001aa60: 2d31 5d5b 325d 203d 2073 7472 286e 6577  -1][2] = str(new
-0001aa70: 5f61 6e6e 6f74 6174 696f 6e73 5b2d 315d  _annotations[-1]
-0001aa80: 5b32 5d29 202b 2022 2c20 2220 2b20 7374  [2]) + ", " + st
-0001aa90: 7228 615b 325d 290a 2020 2020 2020 2020  r(a[2]).        
-0001aaa0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0001aab0: 2020 2020 2020 2020 2020 6e65 775f 616e            new_an
-0001aac0: 6e6f 7461 7469 6f6e 732e 6170 7065 6e64  notations.append
-0001aad0: 2861 290a 2020 2020 2020 2020 616e 6e6f  (a).        anno
-0001aae0: 7461 7469 6f6e 7320 3d20 6e65 775f 616e  tations = new_an
-0001aaf0: 6e6f 7461 7469 6f6e 730a 0a20 2020 2020  notations..     
-0001ab00: 2020 2069 6620 706c 6f74 5f64 6566 696e     if plot_defin
-0001ab10: 6974 696f 6e73 3a0a 2020 2020 2020 2020  itions:.        
-0001ab20: 2020 2020 6966 2073 7461 636b 7570 5f6d      if stackup_m
-0001ab30: 6f64 6520 3d3d 2022 4f76 6572 6c61 7070  ode == "Overlapp
-0001ab40: 696e 6722 3a0a 2020 2020 2020 2020 2020  ing":.          
-0001ab50: 2020 2020 2020 7365 6c66 2e5f 6c6f 6767        self._logg
-0001ab60: 6572 2e77 6172 6e69 6e67 2822 506c 6f74  er.warning("Plot
-0001ab70: 206f 6620 7061 6473 7461 636b 7320 6172   of padstacks ar
-0001ab80: 6520 7375 7070 6f72 7465 6420 6f6e 6c79  e supported only
-0001ab90: 2066 6f72 204c 616d 696e 6174 6520 6d6f   for Laminate mo
-0001aba0: 6465 2e22 290a 0a20 2020 2020 2020 2020  de.")..         
-0001abb0: 2020 206d 6178 5f70 6c6f 7473 203d 2031     max_plots = 1
-0001abc0: 300a 0a20 2020 2020 2020 2020 2020 2069  0..            i
-0001abd0: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
-0001abe0: 2870 6c6f 745f 6465 6669 6e69 7469 6f6e  (plot_definition
-0001abf0: 732c 206c 6973 7429 3a0a 2020 2020 2020  s, list):.      
-0001ac00: 2020 2020 2020 2020 2020 706c 6f74 5f64            plot_d
-0001ac10: 6566 696e 6974 696f 6e73 203d 205b 706c  efinitions = [pl
-0001ac20: 6f74 5f64 6566 696e 6974 696f 6e73 5d0a  ot_definitions].
-0001ac30: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
-0001ac40: 725f 696e 6465 7820 3d20 300a 2020 2020  r_index = 0.    
-0001ac50: 2020 2020 2020 2020 636f 6c6f 725f 6b65          color_ke
-0001ac60: 7973 203d 206c 6973 7428 4353 5334 5f43  ys = list(CSS4_C
-0001ac70: 4f4c 4f52 532e 6b65 7973 2829 290a 2020  OLORS.keys()).  
-0001ac80: 2020 2020 2020 2020 2020 6465 6c74 6120            delta 
-0001ac90: 3d20 3120 2f20 286d 6178 5f70 6c6f 7473  = 1 / (max_plots
-0001aca0: 202b 2031 2920 2023 2070 6164 7374 6163   + 1)  # padstac
-0001acb0: 6b20 7370 6163 696e 6720 696e 2070 6c6f  k spacing in plo
-0001acc0: 7420 636f 6f72 6469 6e61 7465 730a 2020  t coordinates.  
-0001acd0: 2020 2020 2020 2020 2020 785f 7374 6172            x_star
-0001ace0: 7420 3d20 6465 6c74 610a 0a20 2020 2020  t = delta..     
-0001acf0: 2020 2020 2020 2023 2066 696e 6420 7468         # find th
-0001ad00: 6520 6d61 7820 7061 6473 7461 636b 2073  e max padstack s
-0001ad10: 697a 6520 746f 2063 616c 6375 6c61 7465  ize to calculate
-0001ad20: 2074 6865 2073 6361 6c69 6e67 2066 6163   the scaling fac
-0001ad30: 746f 720a 2020 2020 2020 2020 2020 2020  tor.            
-0001ad40: 6d61 785f 7061 6473 7461 6b5f 7369 7a65  max_padstak_size
-0001ad50: 203d 2030 0a20 2020 2020 2020 2020 2020   = 0.           
-0001ad60: 2066 6f72 2064 6566 696e 6974 696f 6e20   for definition 
-0001ad70: 696e 2070 6c6f 745f 6465 6669 6e69 7469  in plot_definiti
-0001ad80: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
-0001ad90: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-0001ada0: 6365 2864 6566 696e 6974 696f 6e2c 2073  ce(definition, s
-0001adb0: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-0001adc0: 2020 2020 2020 2020 2064 6566 696e 6974           definit
-0001add0: 696f 6e20 3d20 7365 6c66 2e5f 7065 6462  ion = self._pedb
-0001ade0: 2e70 6164 7374 6163 6b73 2e64 6566 696e  .padstacks.defin
-0001adf0: 6974 696f 6e73 5b64 6566 696e 6974 696f  itions[definitio
-0001ae00: 6e5d 0a20 2020 2020 2020 2020 2020 2020  n].             
-0001ae10: 2020 2066 6f72 206c 6179 6572 2c20 6465     for layer, de
-0001ae20: 6673 2069 6e20 6465 6669 6e69 7469 6f6e  fs in definition
-0001ae30: 2e70 6164 5f62 795f 6c61 7965 722e 6974  .pad_by_layer.it
-0001ae40: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
-0001ae50: 2020 2020 2020 2020 2020 2070 6164 5f73             pad_s
-0001ae60: 6861 7065 203d 2064 6566 732e 6765 6f6d  hape = defs.geom
-0001ae70: 6574 7279 5f74 7970 650a 2020 2020 2020  etry_type.      
-0001ae80: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-0001ae90: 7261 6d73 203d 2064 6566 732e 7061 7261  rams = defs.para
-0001aea0: 6d65 7465 7273 5f76 616c 7565 730a 2020  meters_values.  
-0001aeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aec0: 2020 6966 2070 6164 5f73 6861 7065 2069    if pad_shape i
-0001aed0: 6e20 5b31 2c20 322c 2036 5d3a 0a20 2020  n [1, 2, 6]:.   
+0001a760: 2069 6620 6e61 6d65 203d 3d20 696e 616d   if name == inam
+0001a770: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0001a780: 2020 2020 2020 2020 2020 206c 6567 656e             legen
+0001a790: 645f 6f72 6465 722e 6170 7065 6e64 2869  d_order.append(i
+0001a7a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001a7b0: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
+0001a7c0: 0a20 2020 2020 2020 2023 2063 616c 6375  .        # calcu
+0001a7d0: 6c61 7465 2074 6865 2065 7874 7265 6d69  late the extremi
+0001a7e0: 7469 6573 206f 6620 7468 6520 706c 6f74  ties of the plot
+0001a7f0: 0a20 2020 2020 2020 2078 5f6d 696e 203d  .        x_min =
+0001a800: 2030 2e30 0a20 2020 2020 2020 2078 5f6d   0.0.        x_m
+0001a810: 6178 203d 206d 6178 285b 6d61 7828 695b  ax = max([max(i[
+0001a820: 305d 2920 666f 7220 6920 696e 2070 6c6f  0]) for i in plo
+0001a830: 745f 6461 7461 5d29 0a20 2020 2020 2020  t_data]).       
+0001a840: 2069 6620 7374 6163 6b75 705f 6d6f 6465   if stackup_mode
+0001a850: 203d 3d20 224c 616d 696e 6174 6522 3a0a   == "Laminate":.
+0001a860: 2020 2020 2020 2020 2020 2020 795f 6d69              y_mi
+0001a870: 6e20 3d20 6c61 7965 7273 5f64 6174 615b  n = layers_data[
+0001a880: 305d 5b31 5d0a 2020 2020 2020 2020 2020  0][1].          
+0001a890: 2020 795f 6d61 7820 3d20 6c61 7965 7273    y_max = layers
+0001a8a0: 5f64 6174 615b 2d31 5d5b 325d 0a20 2020  _data[-1][2].   
+0001a8b0: 2020 2020 2065 6c69 6620 7374 6163 6b75       elif stacku
+0001a8c0: 705f 6d6f 6465 203d 3d20 224f 7665 726c  p_mode == "Overl
+0001a8d0: 6170 7069 6e67 223a 0a20 2020 2020 2020  apping":.       
+0001a8e0: 2020 2020 2079 5f6d 696e 203d 206d 696e       y_min = min
+0001a8f0: 2864 6965 6c65 6374 7269 635f 6c61 7965  (dielectric_laye
+0001a900: 7273 5b30 5d5b 315d 2c20 7369 676e 616c  rs[0][1], signal
+0001a910: 5f6c 6179 6572 735b 305d 5b31 5d29 0a20  _layers[0][1]). 
+0001a920: 2020 2020 2020 2020 2020 2079 5f6d 6178             y_max
+0001a930: 203d 206d 6178 2864 6965 6c65 6374 7269   = max(dielectri
+0001a940: 635f 6c61 7965 7273 5b2d 315d 5b32 5d2c  c_layers[-1][2],
+0001a950: 2073 6967 6e61 6c5f 6c61 7965 7273 5b2d   signal_layers[-
+0001a960: 315d 5b32 5d29 0a0a 2020 2020 2020 2020  1][2])..        
+0001a970: 2320 6d6f 7665 2074 6865 2061 6e6e 6f74  # move the annot
+0001a980: 6174 696f 6e73 2074 6f20 6176 6f69 6420  ations to avoid 
+0001a990: 7465 7874 206f 7665 726c 6170 7069 6e67  text overlapping
+0001a9a0: 0a20 2020 2020 2020 206e 6577 5f61 6e6e  .        new_ann
+0001a9b0: 6f74 6174 696f 6e73 203d 205b 5d0a 2020  otations = [].  
+0001a9c0: 2020 2020 2020 666f 7220 692c 2061 2069        for i, a i
+0001a9d0: 6e20 656e 756d 6572 6174 6528 616e 6e6f  n enumerate(anno
+0001a9e0: 7461 7469 6f6e 7329 3a0a 2020 2020 2020  tations):.      
+0001a9f0: 2020 2020 2020 6966 2069 203e 2030 2061        if i > 0 a
+0001aa00: 6e64 2061 6273 2861 5b31 5d20 2d20 616e  nd abs(a[1] - an
+0001aa10: 6e6f 7461 7469 6f6e 735b 6920 2d20 315d  notations[i - 1]
+0001aa20: 5b31 5d29 203c 2028 795f 6d61 7820 2d20  [1]) < (y_max - 
+0001aa30: 795f 6d69 6e29 202f 2037 353a 0a20 2020  y_min) / 75:.   
+0001aa40: 2020 2020 2020 2020 2020 2020 206e 6577               new
+0001aa50: 5f61 6e6e 6f74 6174 696f 6e73 5b2d 315d  _annotations[-1]
+0001aa60: 5b32 5d20 3d20 7374 7228 6e65 775f 616e  [2] = str(new_an
+0001aa70: 6e6f 7461 7469 6f6e 735b 2d31 5d5b 325d  notations[-1][2]
+0001aa80: 2920 2b20 222c 2022 202b 2073 7472 2861  ) + ", " + str(a
+0001aa90: 5b32 5d29 0a20 2020 2020 2020 2020 2020  [2]).           
+0001aaa0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0001aab0: 2020 2020 2020 206e 6577 5f61 6e6e 6f74         new_annot
+0001aac0: 6174 696f 6e73 2e61 7070 656e 6428 6129  ations.append(a)
+0001aad0: 0a20 2020 2020 2020 2061 6e6e 6f74 6174  .        annotat
+0001aae0: 696f 6e73 203d 206e 6577 5f61 6e6e 6f74  ions = new_annot
+0001aaf0: 6174 696f 6e73 0a0a 2020 2020 2020 2020  ations..        
+0001ab00: 6966 2070 6c6f 745f 6465 6669 6e69 7469  if plot_definiti
+0001ab10: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
+0001ab20: 2069 6620 7374 6163 6b75 705f 6d6f 6465   if stackup_mode
+0001ab30: 203d 3d20 224f 7665 726c 6170 7069 6e67   == "Overlapping
+0001ab40: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+0001ab50: 2020 2073 656c 662e 5f6c 6f67 6765 722e     self._logger.
+0001ab60: 7761 726e 696e 6728 2250 6c6f 7420 6f66  warning("Plot of
+0001ab70: 2070 6164 7374 6163 6b73 2061 7265 2073   padstacks are s
+0001ab80: 7570 706f 7274 6564 206f 6e6c 7920 666f  upported only fo
+0001ab90: 7220 4c61 6d69 6e61 7465 206d 6f64 652e  r Laminate mode.
+0001aba0: 2229 0a0a 2020 2020 2020 2020 2020 2020  ")..            
+0001abb0: 6d61 785f 706c 6f74 7320 3d20 3130 0a0a  max_plots = 10..
+0001abc0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0001abd0: 6f74 2069 7369 6e73 7461 6e63 6528 706c  ot isinstance(pl
+0001abe0: 6f74 5f64 6566 696e 6974 696f 6e73 2c20  ot_definitions, 
+0001abf0: 6c69 7374 293a 0a20 2020 2020 2020 2020  list):.         
+0001ac00: 2020 2020 2020 2070 6c6f 745f 6465 6669         plot_defi
+0001ac10: 6e69 7469 6f6e 7320 3d20 5b70 6c6f 745f  nitions = [plot_
+0001ac20: 6465 6669 6e69 7469 6f6e 735d 0a20 2020  definitions].   
+0001ac30: 2020 2020 2020 2020 2063 6f6c 6f72 5f69           color_i
+0001ac40: 6e64 6578 203d 2030 0a20 2020 2020 2020  ndex = 0.       
+0001ac50: 2020 2020 2063 6f6c 6f72 5f6b 6579 7320       color_keys 
+0001ac60: 3d20 6c69 7374 2843 5353 345f 434f 4c4f  = list(CSS4_COLO
+0001ac70: 5253 2e6b 6579 7328 2929 0a20 2020 2020  RS.keys()).     
+0001ac80: 2020 2020 2020 2064 656c 7461 203d 2031         delta = 1
+0001ac90: 202f 2028 6d61 785f 706c 6f74 7320 2b20   / (max_plots + 
+0001aca0: 3129 2020 2320 7061 6473 7461 636b 2073  1)  # padstack s
+0001acb0: 7061 6369 6e67 2069 6e20 706c 6f74 2063  pacing in plot c
+0001acc0: 6f6f 7264 696e 6174 6573 0a20 2020 2020  oordinates.     
+0001acd0: 2020 2020 2020 2078 5f73 7461 7274 203d         x_start =
+0001ace0: 2064 656c 7461 0a0a 2020 2020 2020 2020   delta..        
+0001acf0: 2020 2020 2320 6669 6e64 2074 6865 206d      # find the m
+0001ad00: 6178 2070 6164 7374 6163 6b20 7369 7a65  ax padstack size
+0001ad10: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
+0001ad20: 6520 7363 616c 696e 6720 6661 6374 6f72  e scaling factor
+0001ad30: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
+0001ad40: 5f70 6164 7374 616b 5f73 697a 6520 3d20  _padstak_size = 
+0001ad50: 300a 2020 2020 2020 2020 2020 2020 666f  0.            fo
+0001ad60: 7220 6465 6669 6e69 7469 6f6e 2069 6e20  r definition in 
+0001ad70: 706c 6f74 5f64 6566 696e 6974 696f 6e73  plot_definitions
+0001ad80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001ad90: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+0001ada0: 6465 6669 6e69 7469 6f6e 2c20 7374 7229  definition, str)
+0001adb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001adc0: 2020 2020 2020 6465 6669 6e69 7469 6f6e        definition
+0001add0: 203d 2073 656c 662e 5f70 6564 622e 7061   = self._pedb.pa
+0001ade0: 6473 7461 636b 732e 6465 6669 6e69 7469  dstacks.definiti
+0001adf0: 6f6e 735b 6465 6669 6e69 7469 6f6e 5d0a  ons[definition].
+0001ae00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ae10: 666f 7220 6c61 7965 722c 2064 6566 7320  for layer, defs 
+0001ae20: 696e 2064 6566 696e 6974 696f 6e2e 7061  in definition.pa
+0001ae30: 645f 6279 5f6c 6179 6572 2e69 7465 6d73  d_by_layer.items
+0001ae40: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0001ae50: 2020 2020 2020 2020 7061 645f 7368 6170          pad_shap
+0001ae60: 6520 3d20 6465 6673 2e67 656f 6d65 7472  e = defs.geometr
+0001ae70: 795f 7479 7065 0a20 2020 2020 2020 2020  y_type.         
+0001ae80: 2020 2020 2020 2020 2020 2070 6172 616d             param
+0001ae90: 7320 3d20 6465 6673 2e70 6172 616d 6574  s = defs.paramet
+0001aea0: 6572 735f 7661 6c75 6573 0a20 2020 2020  ers_values.     
+0001aeb0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001aec0: 6620 7061 645f 7368 6170 6520 696e 205b  f pad_shape in [
+0001aed0: 312c 2032 2c20 365d 3a0a 2020 2020 2020  1, 2, 6]:.      
 0001aee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aef0: 2020 2020 2070 6164 5f73 697a 6520 3d20       pad_size = 
-0001af00: 7061 7261 6d73 5b30 5d0a 2020 2020 2020  params[0].      
-0001af10: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0001af20: 6966 2070 6164 5f73 6861 7065 2069 6e20  if pad_shape in 
-0001af30: 5b33 2c20 342c 2035 5d3a 0a20 2020 2020  [3, 4, 5]:.     
+0001aef0: 2020 7061 645f 7369 7a65 203d 2070 6172    pad_size = par
+0001af00: 616d 735b 305d 0a20 2020 2020 2020 2020  ams[0].         
+0001af10: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+0001af20: 7061 645f 7368 6170 6520 696e 205b 332c  pad_shape in [3,
+0001af30: 2034 2c20 355d 3a0a 2020 2020 2020 2020   4, 5]:.        
 0001af40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001af50: 2020 2070 6164 5f73 697a 6520 3d20 6d61     pad_size = ma
-0001af60: 7828 7061 7261 6d73 5b30 5d2c 2070 6172  x(params[0], par
-0001af70: 616d 735b 315d 290a 2020 2020 2020 2020  ams[1]).        
-0001af80: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0001af90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001afa0: 2020 2020 2020 2020 2020 7061 645f 7369            pad_si
-0001afb0: 7a65 203d 2031 652d 340a 2020 2020 2020  ze = 1e-4.      
-0001afc0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-0001afd0: 785f 7061 6473 7461 6b5f 7369 7a65 203d  x_padstak_size =
-0001afe0: 206d 6178 2870 6164 5f73 697a 652c 206d   max(pad_size, m
-0001aff0: 6178 5f70 6164 7374 616b 5f73 697a 6529  ax_padstak_size)
-0001b000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b010: 2069 6620 6465 6669 6e69 7469 6f6e 2e68   if definition.h
-0001b020: 6f6c 655f 7072 6f70 6572 7469 6573 3a0a  ole_properties:.
+0001af50: 7061 645f 7369 7a65 203d 206d 6178 2870  pad_size = max(p
+0001af60: 6172 616d 735b 305d 2c20 7061 7261 6d73  arams[0], params
+0001af70: 5b31 5d29 0a20 2020 2020 2020 2020 2020  [1]).           
+0001af80: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0001af90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001afa0: 2020 2020 2020 2070 6164 5f73 697a 6520         pad_size 
+0001afb0: 3d20 3165 2d34 0a20 2020 2020 2020 2020  = 1e-4.         
+0001afc0: 2020 2020 2020 2020 2020 206d 6178 5f70             max_p
+0001afd0: 6164 7374 616b 5f73 697a 6520 3d20 6d61  adstak_size = ma
+0001afe0: 7828 7061 645f 7369 7a65 2c20 6d61 785f  x(pad_size, max_
+0001aff0: 7061 6473 7461 6b5f 7369 7a65 290a 2020  padstak_size).  
+0001b000: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001b010: 2064 6566 696e 6974 696f 6e2e 686f 6c65   definition.hole
+0001b020: 5f70 726f 7065 7274 6965 733a 0a20 2020  _properties:.   
 0001b030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b040: 2020 2020 686f 6c65 5f64 203d 2064 6566      hole_d = def
-0001b050: 696e 6974 696f 6e2e 686f 6c65 5f70 726f  inition.hole_pro
-0001b060: 7065 7274 6965 735b 305d 0a20 2020 2020  perties[0].     
-0001b070: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0001b080: 6178 5f70 6164 7374 616b 5f73 697a 6520  ax_padstak_size 
-0001b090: 3d20 6d61 7828 686f 6c65 5f64 2c20 6d61  = max(hole_d, ma
-0001b0a0: 785f 7061 6473 7461 6b5f 7369 7a65 290a  x_padstak_size).
-0001b0b0: 2020 2020 2020 2020 2020 2020 7363 616c              scal
-0001b0c0: 696e 675f 665f 7061 6420 3d20 2832 202f  ing_f_pad = (2 /
-0001b0d0: 2028 286d 6178 5f70 6c6f 7473 202b 2031   ((max_plots + 1
-0001b0e0: 2920 2a20 3329 2920 2f20 6d61 785f 7061  ) * 3)) / max_pa
-0001b0f0: 6473 7461 6b5f 7369 7a65 0a0a 2020 2020  dstak_size..    
-0001b100: 2020 2020 2020 2020 666f 7220 6465 6669          for defi
-0001b110: 6e69 7469 6f6e 2069 6e20 706c 6f74 5f64  nition in plot_d
-0001b120: 6566 696e 6974 696f 6e73 3a0a 2020 2020  efinitions:.    
-0001b130: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-0001b140: 7369 6e73 7461 6e63 6528 6465 6669 6e69  sinstance(defini
-0001b150: 7469 6f6e 2c20 7374 7229 3a0a 2020 2020  tion, str):.    
-0001b160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b170: 6465 6669 6e69 7469 6f6e 203d 2073 656c  definition = sel
-0001b180: 662e 5f70 6564 622e 7061 6473 7461 636b  f._pedb.padstack
-0001b190: 732e 6465 6669 6e69 7469 6f6e 735b 6465  s.definitions[de
-0001b1a0: 6669 6e69 7469 6f6e 5d0a 2020 2020 2020  finition].      
-0001b1b0: 2020 2020 2020 2020 2020 6d69 6e5f 6c65            min_le
-0001b1c0: 203d 2031 6531 320a 2020 2020 2020 2020   = 1e12.        
-0001b1d0: 2020 2020 2020 2020 6d61 785f 7565 203d          max_ue =
-0001b1e0: 202d 3165 3132 0a20 2020 2020 2020 2020   -1e12.         
-0001b1f0: 2020 2020 2020 206d 6178 5f78 203d 2030         max_x = 0
-0001b200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b210: 2070 6164 7374 6163 6b5f 6e61 6d65 203d   padstack_name =
-0001b220: 2064 6566 696e 6974 696f 6e2e 6e61 6d65   definition.name
-0001b230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b240: 2061 6e6e 6f74 6174 696f 6e73 2e61 7070   annotations.app
-0001b250: 656e 6428 5b78 5f73 7461 7274 2c20 795f  end([x_start, y_
-0001b260: 6d61 782c 2070 6164 7374 6163 6b5f 6e61  max, padstack_na
-0001b270: 6d65 2c20 7b22 726f 7461 7469 6f6e 223a  me, {"rotation":
-0001b280: 2034 357d 5d29 0a0a 2020 2020 2020 2020   45}])..        
-0001b290: 2020 2020 2020 2020 7669 615f 7374 6172          via_star
-0001b2a0: 745f 6c61 7965 7220 3d20 6465 6669 6e69  t_layer = defini
-0001b2b0: 7469 6f6e 2e76 6961 5f73 7461 7274 5f6c  tion.via_start_l
-0001b2c0: 6179 6572 0a20 2020 2020 2020 2020 2020  ayer.           
-0001b2d0: 2020 2020 2076 6961 5f73 746f 705f 6c61       via_stop_la
-0001b2e0: 7965 7220 3d20 6465 6669 6e69 7469 6f6e  yer = definition
-0001b2f0: 2e76 6961 5f73 746f 705f 6c61 7965 720a  .via_stop_layer.
-0001b300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b310: 2069 6620 7374 6163 6b75 705f 6d6f 6465   if stackup_mode
-0001b320: 203d 3d20 224f 7665 726c 6170 7069 6e67   == "Overlapping
-0001b330: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-0001b340: 2020 2020 2020 2023 2068 6572 6520 7365         # here se
-0001b350: 6172 6368 2074 6865 2063 6f6c 756d 6e20  arch the column 
-0001b360: 7573 696e 6720 7468 6520 6669 7273 7420  using the first 
-0001b370: 616e 6420 6c61 7374 206c 6179 6572 2e20  and last layer. 
-0001b380: 5069 636b 2074 6865 2063 6f6c 756d 6e20  Pick the column 
-0001b390: 7769 7468 206d 6178 2069 6e64 6578 2e0a  with max index..
+0001b040: 2068 6f6c 655f 6420 3d20 6465 6669 6e69   hole_d = defini
+0001b050: 7469 6f6e 2e68 6f6c 655f 7072 6f70 6572  tion.hole_proper
+0001b060: 7469 6573 5b30 5d0a 2020 2020 2020 2020  ties[0].        
+0001b070: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
+0001b080: 7061 6473 7461 6b5f 7369 7a65 203d 206d  padstak_size = m
+0001b090: 6178 2868 6f6c 655f 642c 206d 6178 5f70  ax(hole_d, max_p
+0001b0a0: 6164 7374 616b 5f73 697a 6529 0a20 2020  adstak_size).   
+0001b0b0: 2020 2020 2020 2020 2073 6361 6c69 6e67           scaling
+0001b0c0: 5f66 5f70 6164 203d 2028 3220 2f20 2828  _f_pad = (2 / ((
+0001b0d0: 6d61 785f 706c 6f74 7320 2b20 3129 202a  max_plots + 1) *
+0001b0e0: 2033 2929 202f 206d 6178 5f70 6164 7374   3)) / max_padst
+0001b0f0: 616b 5f73 697a 650a 0a20 2020 2020 2020  ak_size..       
+0001b100: 2020 2020 2066 6f72 2064 6566 696e 6974       for definit
+0001b110: 696f 6e20 696e 2070 6c6f 745f 6465 6669  ion in plot_defi
+0001b120: 6e69 7469 6f6e 733a 0a20 2020 2020 2020  nitions:.       
+0001b130: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+0001b140: 7374 616e 6365 2864 6566 696e 6974 696f  stance(definitio
+0001b150: 6e2c 2073 7472 293a 0a20 2020 2020 2020  n, str):.       
+0001b160: 2020 2020 2020 2020 2020 2020 2064 6566               def
+0001b170: 696e 6974 696f 6e20 3d20 7365 6c66 2e5f  inition = self._
+0001b180: 7065 6462 2e70 6164 7374 6163 6b73 2e64  pedb.padstacks.d
+0001b190: 6566 696e 6974 696f 6e73 5b64 6566 696e  efinitions[defin
+0001b1a0: 6974 696f 6e5d 0a20 2020 2020 2020 2020  ition].         
+0001b1b0: 2020 2020 2020 206d 696e 5f6c 6520 3d20         min_le = 
+0001b1c0: 3165 3132 0a20 2020 2020 2020 2020 2020  1e12.           
+0001b1d0: 2020 2020 206d 6178 5f75 6520 3d20 2d31       max_ue = -1
+0001b1e0: 6531 320a 2020 2020 2020 2020 2020 2020  e12.            
+0001b1f0: 2020 2020 6d61 785f 7820 3d20 300a 2020      max_x = 0.  
+0001b200: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+0001b210: 6473 7461 636b 5f6e 616d 6520 3d20 6465  dstack_name = de
+0001b220: 6669 6e69 7469 6f6e 2e6e 616d 650a 2020  finition.name.  
+0001b230: 2020 2020 2020 2020 2020 2020 2020 616e                an
+0001b240: 6e6f 7461 7469 6f6e 732e 6170 7065 6e64  notations.append
+0001b250: 285b 785f 7374 6172 742c 2079 5f6d 6178  ([x_start, y_max
+0001b260: 2c20 7061 6473 7461 636b 5f6e 616d 652c  , padstack_name,
+0001b270: 207b 2272 6f74 6174 696f 6e22 3a20 3435   {"rotation": 45
+0001b280: 7d5d 290a 0a20 2020 2020 2020 2020 2020  }])..           
+0001b290: 2020 2020 2076 6961 5f73 7461 7274 5f6c       via_start_l
+0001b2a0: 6179 6572 203d 2064 6566 696e 6974 696f  ayer = definitio
+0001b2b0: 6e2e 7669 615f 7374 6172 745f 6c61 7965  n.via_start_laye
+0001b2c0: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+0001b2d0: 2020 7669 615f 7374 6f70 5f6c 6179 6572    via_stop_layer
+0001b2e0: 203d 2064 6566 696e 6974 696f 6e2e 7669   = definition.vi
+0001b2f0: 615f 7374 6f70 5f6c 6179 6572 0a0a 2020  a_stop_layer..  
+0001b300: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001b310: 2073 7461 636b 7570 5f6d 6f64 6520 3d3d   stackup_mode ==
+0001b320: 2022 4f76 6572 6c61 7070 696e 6722 3a0a   "Overlapping":.
+0001b330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b340: 2020 2020 2320 6865 7265 2073 6561 7263      # here searc
+0001b350: 6820 7468 6520 636f 6c75 6d6e 2075 7369  h the column usi
+0001b360: 6e67 2074 6865 2066 6972 7374 2061 6e64  ng the first and
+0001b370: 206c 6173 7420 6c61 7965 722e 2050 6963   last layer. Pic
+0001b380: 6b20 7468 6520 636f 6c75 6d6e 2077 6974  k the column wit
+0001b390: 6820 6d61 7820 696e 6465 782e 0a20 2020  h max index..   
 0001b3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b3b0: 2020 2020 7061 7373 0a0a 2020 2020 2020      pass..      
-0001b3c0: 2020 2020 2020 2020 2020 666f 7220 6c61            for la
-0001b3d0: 7965 722c 2064 6566 7320 696e 2064 6566  yer, defs in def
-0001b3e0: 696e 6974 696f 6e2e 7061 645f 6279 5f6c  inition.pad_by_l
-0001b3f0: 6179 6572 2e69 7465 6d73 2829 3a0a 2020  ayer.items():.  
-0001b400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b410: 2020 7061 645f 7368 6170 6520 3d20 6465    pad_shape = de
-0001b420: 6673 2e67 656f 6d65 7472 795f 7479 7065  fs.geometry_type
-0001b430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b440: 2020 2020 2070 6172 616d 7320 3d20 6465       params = de
-0001b450: 6673 2e70 6172 616d 6574 6572 735f 7661  fs.parameters_va
-0001b460: 6c75 6573 0a20 2020 2020 2020 2020 2020  lues.           
-0001b470: 2020 2020 2020 2020 2069 6620 7061 645f           if pad_
-0001b480: 7368 6170 6520 696e 205b 312c 2032 2c20  shape in [1, 2, 
-0001b490: 365d 3a0a 2020 2020 2020 2020 2020 2020  6]:.            
-0001b4a0: 2020 2020 2020 2020 2020 2020 7061 645f              pad_
-0001b4b0: 7369 7a65 203d 2070 6172 616d 735b 305d  size = params[0]
-0001b4c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b4d0: 2020 2020 2065 6c69 6620 7061 645f 7368       elif pad_sh
-0001b4e0: 6170 6520 696e 205b 332c 2034 2c20 355d  ape in [3, 4, 5]
-0001b4f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001b500: 2020 2020 2020 2020 2020 7061 645f 7369            pad_si
-0001b510: 7a65 203d 206d 6178 2870 6172 616d 735b  ze = max(params[
-0001b520: 305d 2c20 7061 7261 6d73 5b31 5d29 0a20  0], params[1]). 
+0001b3b0: 2070 6173 730a 0a20 2020 2020 2020 2020   pass..         
+0001b3c0: 2020 2020 2020 2066 6f72 206c 6179 6572         for layer
+0001b3d0: 2c20 6465 6673 2069 6e20 6465 6669 6e69  , defs in defini
+0001b3e0: 7469 6f6e 2e70 6164 5f62 795f 6c61 7965  tion.pad_by_laye
+0001b3f0: 722e 6974 656d 7328 293a 0a20 2020 2020  r.items():.     
+0001b400: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0001b410: 6164 5f73 6861 7065 203d 2064 6566 732e  ad_shape = defs.
+0001b420: 6765 6f6d 6574 7279 5f74 7970 650a 2020  geometry_type.  
+0001b430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b440: 2020 7061 7261 6d73 203d 2064 6566 732e    params = defs.
+0001b450: 7061 7261 6d65 7465 7273 5f76 616c 7565  parameters_value
+0001b460: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+0001b470: 2020 2020 2020 6966 2070 6164 5f73 6861        if pad_sha
+0001b480: 7065 2069 6e20 5b31 2c20 322c 2036 5d3a  pe in [1, 2, 6]:
+0001b490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b4a0: 2020 2020 2020 2020 2070 6164 5f73 697a           pad_siz
+0001b4b0: 6520 3d20 7061 7261 6d73 5b30 5d0a 2020  e = params[0].  
+0001b4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b4d0: 2020 656c 6966 2070 6164 5f73 6861 7065    elif pad_shape
+0001b4e0: 2069 6e20 5b33 2c20 342c 2035 5d3a 0a20   in [3, 4, 5]:. 
+0001b4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b500: 2020 2020 2020 2070 6164 5f73 697a 6520         pad_size 
+0001b510: 3d20 6d61 7828 7061 7261 6d73 5b30 5d2c  = max(params[0],
+0001b520: 2070 6172 616d 735b 315d 290a 2020 2020   params[1]).    
 0001b530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b540: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0001b550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b560: 2070 6164 5f73 697a 6520 3d20 3165 2d34   pad_size = 1e-4
-0001b570: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001b580: 2020 2020 2020 6966 2073 7461 636b 7570        if stackup
-0001b590: 5f6d 6f64 6520 3d3d 2022 4c61 6d69 6e61  _mode == "Lamina
-0001b5a0: 7465 223a 0a20 2020 2020 2020 2020 2020  te":.           
-0001b5b0: 2020 2020 2020 2020 2020 2020 2078 203d               x =
-0001b5c0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-0001b5d0: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-0001b5e0: 5f73 7461 7274 202d 2070 6164 5f73 697a  _start - pad_siz
-0001b5f0: 6520 2f20 3220 2a20 7363 616c 696e 675f  e / 2 * scaling_
-0001b600: 665f 7061 642c 0a20 2020 2020 2020 2020  f_pad,.         
+0001b540: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0001b550: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+0001b560: 645f 7369 7a65 203d 2031 652d 340a 0a20  d_size = 1e-4.. 
+0001b570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b580: 2020 2069 6620 7374 6163 6b75 705f 6d6f     if stackup_mo
+0001b590: 6465 203d 3d20 224c 616d 696e 6174 6522  de == "Laminate"
+0001b5a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001b5b0: 2020 2020 2020 2020 2020 7820 3d20 5b0a            x = [.
+0001b5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b5d0: 2020 2020 2020 2020 2020 2020 785f 7374              x_st
+0001b5e0: 6172 7420 2d20 7061 645f 7369 7a65 202f  art - pad_size /
+0001b5f0: 2032 202a 2073 6361 6c69 6e67 5f66 5f70   2 * scaling_f_p
+0001b600: 6164 2c0a 2020 2020 2020 2020 2020 2020  ad,.            
 0001b610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b620: 2020 2078 5f73 7461 7274 202d 2070 6164     x_start - pad
-0001b630: 5f73 697a 6520 2f20 3220 2a20 7363 616c  _size / 2 * scal
-0001b640: 696e 675f 665f 7061 642c 0a20 2020 2020  ing_f_pad,.     
+0001b620: 785f 7374 6172 7420 2d20 7061 645f 7369  x_start - pad_si
+0001b630: 7a65 202f 2032 202a 2073 6361 6c69 6e67  ze / 2 * scaling
+0001b640: 5f66 5f70 6164 2c0a 2020 2020 2020 2020  _f_pad,.        
 0001b650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b660: 2020 2020 2020 2078 5f73 7461 7274 202b         x_start +
-0001b670: 2070 6164 5f73 697a 6520 2f20 3220 2a20   pad_size / 2 * 
-0001b680: 7363 616c 696e 675f 665f 7061 642c 0a20  scaling_f_pad,. 
+0001b660: 2020 2020 785f 7374 6172 7420 2b20 7061      x_start + pa
+0001b670: 645f 7369 7a65 202f 2032 202a 2073 6361  d_size / 2 * sca
+0001b680: 6c69 6e67 5f66 5f70 6164 2c0a 2020 2020  ling_f_pad,.    
 0001b690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b6a0: 2020 2020 2020 2020 2020 2078 5f73 7461             x_sta
-0001b6b0: 7274 202b 2070 6164 5f73 697a 6520 2f20  rt + pad_size / 
-0001b6c0: 3220 2a20 7363 616c 696e 675f 665f 7061  2 * scaling_f_pa
-0001b6d0: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-0001b6e0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+0001b6a0: 2020 2020 2020 2020 785f 7374 6172 7420          x_start 
+0001b6b0: 2b20 7061 645f 7369 7a65 202f 2032 202a  + pad_size / 2 *
+0001b6c0: 2073 6361 6c69 6e67 5f66 5f70 6164 2c0a   scaling_f_pad,.
+0001b6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b6e0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
 0001b6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b700: 2020 2020 206c 6f77 6572 5f65 6c65 7661       lower_eleva
-0001b710: 7469 6f6e 203d 205b 655b 315d 2066 6f72  tion = [e[1] for
-0001b720: 2065 2069 6e20 6c61 7965 7273 5f64 6174   e in layers_dat
-0001b730: 6120 6966 2065 5b30 5d2e 6e61 6d65 203d  a if e[0].name =
-0001b740: 3d20 6c61 7965 7220 6f72 206c 6179 6572  = layer or layer
-0001b750: 203d 3d20 2244 6566 6175 6c74 225d 5b30   == "Default"][0
-0001b760: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0001b770: 2020 2020 2020 2020 2020 7570 7065 725f            upper_
-0001b780: 656c 6576 6174 696f 6e20 3d20 5b65 5b32  elevation = [e[2
-0001b790: 5d20 666f 7220 6520 696e 206c 6179 6572  ] for e in layer
-0001b7a0: 735f 6461 7461 2069 6620 655b 305d 2e6e  s_data if e[0].n
-0001b7b0: 616d 6520 3d3d 206c 6179 6572 206f 7220  ame == layer or 
-0001b7c0: 6c61 7965 7220 3d3d 2022 4465 6661 756c  layer == "Defaul
-0001b7d0: 7422 5d5b 305d 0a20 2020 2020 2020 2020  t"][0].         
-0001b7e0: 2020 2020 2020 2020 2020 2020 2020 2079                 y
-0001b7f0: 203d 205b 6c6f 7765 725f 656c 6576 6174   = [lower_elevat
-0001b800: 696f 6e2c 2075 7070 6572 5f65 6c65 7661  ion, upper_eleva
-0001b810: 7469 6f6e 2c20 7570 7065 725f 656c 6576  tion, upper_elev
-0001b820: 6174 696f 6e2c 206c 6f77 6572 5f65 6c65  ation, lower_ele
-0001b830: 7661 7469 6f6e 5d0a 2020 2020 2020 2020  vation].        
-0001b840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b850: 2320 6372 6561 7465 2074 6865 2070 6174  # create the pat
-0001b860: 6368 2066 6f72 2074 6861 7420 7369 676e  ch for that sign
-0001b870: 616c 206c 6179 6572 0a20 2020 2020 2020  al layer.       
-0001b880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b890: 2070 6c6f 745f 6461 7461 2e61 7070 656e   plot_data.appen
-0001b8a0: 6428 5b78 2c20 792c 2063 6f6c 6f72 5f6b  d([x, y, color_k
-0001b8b0: 6579 735b 636f 6c6f 725f 696e 6465 785d  eys[color_index]
-0001b8c0: 2c20 4e6f 6e65 2c20 312e 302c 2022 6669  , None, 1.0, "fi
-0001b8d0: 6c6c 225d 290a 2020 2020 2020 2020 2020  ll"]).          
-0001b8e0: 2020 2020 2020 2020 2020 656c 6966 2073            elif s
-0001b8f0: 7461 636b 7570 5f6d 6f64 6520 3d3d 2022  tackup_mode == "
-0001b900: 4f76 6572 6c61 7070 696e 6722 3a0a 2020  Overlapping":.  
+0001b700: 2020 6c6f 7765 725f 656c 6576 6174 696f    lower_elevatio
+0001b710: 6e20 3d20 5b65 5b31 5d20 666f 7220 6520  n = [e[1] for e 
+0001b720: 696e 206c 6179 6572 735f 6461 7461 2069  in layers_data i
+0001b730: 6620 655b 305d 2e6e 616d 6520 3d3d 206c  f e[0].name == l
+0001b740: 6179 6572 206f 7220 6c61 7965 7220 3d3d  ayer or layer ==
+0001b750: 2022 4465 6661 756c 7422 5d5b 305d 0a20   "Default"][0]. 
+0001b760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b770: 2020 2020 2020 2075 7070 6572 5f65 6c65         upper_ele
+0001b780: 7661 7469 6f6e 203d 205b 655b 325d 2066  vation = [e[2] f
+0001b790: 6f72 2065 2069 6e20 6c61 7965 7273 5f64  or e in layers_d
+0001b7a0: 6174 6120 6966 2065 5b30 5d2e 6e61 6d65  ata if e[0].name
+0001b7b0: 203d 3d20 6c61 7965 7220 6f72 206c 6179   == layer or lay
+0001b7c0: 6572 203d 3d20 2244 6566 6175 6c74 225d  er == "Default"]
+0001b7d0: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+0001b7e0: 2020 2020 2020 2020 2020 2020 7920 3d20              y = 
+0001b7f0: 5b6c 6f77 6572 5f65 6c65 7661 7469 6f6e  [lower_elevation
+0001b800: 2c20 7570 7065 725f 656c 6576 6174 696f  , upper_elevatio
+0001b810: 6e2c 2075 7070 6572 5f65 6c65 7661 7469  n, upper_elevati
+0001b820: 6f6e 2c20 6c6f 7765 725f 656c 6576 6174  on, lower_elevat
+0001b830: 696f 6e5d 0a20 2020 2020 2020 2020 2020  ion].           
+0001b840: 2020 2020 2020 2020 2020 2020 2023 2063               # c
+0001b850: 7265 6174 6520 7468 6520 7061 7463 6820  reate the patch 
+0001b860: 666f 7220 7468 6174 2073 6967 6e61 6c20  for that signal 
+0001b870: 6c61 7965 720a 2020 2020 2020 2020 2020  layer.          
+0001b880: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+0001b890: 6f74 5f64 6174 612e 6170 7065 6e64 285b  ot_data.append([
+0001b8a0: 782c 2079 2c20 636f 6c6f 725f 6b65 7973  x, y, color_keys
+0001b8b0: 5b63 6f6c 6f72 5f69 6e64 6578 5d2c 204e  [color_index], N
+0001b8c0: 6f6e 652c 2031 2e30 2c20 2266 696c 6c22  one, 1.0, "fill"
+0001b8d0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+0001b8e0: 2020 2020 2020 2065 6c69 6620 7374 6163         elif stac
+0001b8f0: 6b75 705f 6d6f 6465 203d 3d20 224f 7665  kup_mode == "Ove
+0001b900: 726c 6170 7069 6e67 223a 0a20 2020 2020  rlapping":.     
 0001b910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b920: 2020 2020 2020 2320 6865 7265 2065 7661        # here eva
-0001b930: 6c75 6174 6520 7468 6520 7820 6261 7365  luate the x base
-0001b940: 6420 6f6e 2074 6865 2063 6f6c 756d 6e20  d on the column 
-0001b950: 6576 616c 7561 7465 6420 6265 666f 7265  evaluated before
-0001b960: 2061 6e64 2074 6865 2070 6164 2073 697a   and the pad siz
-0001b970: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0001b980: 2020 2020 2020 2020 2020 7061 7373 0a0a            pass..
+0001b920: 2020 2023 2068 6572 6520 6576 616c 7561     # here evalua
+0001b930: 7465 2074 6865 2078 2062 6173 6564 206f  te the x based o
+0001b940: 6e20 7468 6520 636f 6c75 6d6e 2065 7661  n the column eva
+0001b950: 6c75 6174 6564 2062 6566 6f72 6520 616e  luated before an
+0001b960: 6420 7468 6520 7061 6420 7369 7a65 0a20  d the pad size. 
+0001b970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b980: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
 0001b990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b9a0: 2020 2020 6d69 6e5f 6c65 203d 206d 696e      min_le = min
-0001b9b0: 286c 6f77 6572 5f65 6c65 7661 7469 6f6e  (lower_elevation
-0001b9c0: 2c20 6d69 6e5f 6c65 290a 2020 2020 2020  , min_le).      
-0001b9d0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-0001b9e0: 785f 7565 203d 206d 6178 2875 7070 6572  x_ue = max(upper
-0001b9f0: 5f65 6c65 7661 7469 6f6e 2c20 6d61 785f  _elevation, max_
-0001ba00: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
-0001ba10: 2020 2020 6966 2064 6566 696e 6974 696f      if definitio
-0001ba20: 6e2e 686f 6c65 5f70 726f 7065 7274 6965  n.hole_propertie
-0001ba30: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0001ba40: 2020 2020 2020 2023 2063 7265 6174 6520         # create 
-0001ba50: 7061 7463 6820 666f 7220 7468 6520 686f  patch for the ho
-0001ba60: 6c65 0a20 2020 2020 2020 2020 2020 2020  le.             
-0001ba70: 2020 2020 2020 2068 6f6c 655f 7261 6469         hole_radi
-0001ba80: 7573 203d 2064 6566 696e 6974 696f 6e2e  us = definition.
-0001ba90: 686f 6c65 5f70 726f 7065 7274 6965 735b  hole_properties[
-0001baa0: 305d 202f 2032 202a 2073 6361 6c69 6e67  0] / 2 * scaling
-0001bab0: 5f66 5f70 6164 0a20 2020 2020 2020 2020  _f_pad.         
-0001bac0: 2020 2020 2020 2020 2020 2078 203d 205b             x = [
-0001bad0: 785f 7374 6172 7420 2d20 686f 6c65 5f72  x_start - hole_r
-0001bae0: 6164 6975 732c 2078 5f73 7461 7274 202d  adius, x_start -
-0001baf0: 2068 6f6c 655f 7261 6469 7573 2c20 785f   hole_radius, x_
-0001bb00: 7374 6172 7420 2b20 686f 6c65 5f72 6164  start + hole_rad
-0001bb10: 6975 732c 2078 5f73 7461 7274 202b 2068  ius, x_start + h
-0001bb20: 6f6c 655f 7261 6469 7573 5d0a 2020 2020  ole_radius].    
-0001bb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bb40: 7920 3d20 5b6d 696e 5f6c 652c 206d 6178  y = [min_le, max
-0001bb50: 5f75 652c 206d 6178 5f75 652c 206d 696e  _ue, max_ue, min
-0001bb60: 5f6c 655d 0a20 2020 2020 2020 2020 2020  _le].           
-0001bb70: 2020 2020 2020 2020 2070 6c6f 745f 6461           plot_da
-0001bb80: 7461 2e61 7070 656e 6428 5b78 2c20 792c  ta.append([x, y,
-0001bb90: 2063 6f6c 6f72 5f6b 6579 735b 636f 6c6f   color_keys[colo
-0001bba0: 725f 696e 6465 785d 2c20 4e6f 6e65 2c20  r_index], None, 
-0001bbb0: 302e 372c 2022 6669 6c6c 225d 290a 2020  0.7, "fill"]).  
-0001bbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bbd0: 2020 2320 6372 6561 7465 2070 6174 6368    # create patch
-0001bbe0: 2066 6f72 2074 6865 2064 6965 6c65 6374   for the dielect
-0001bbf0: 7269 630a 2020 2020 2020 2020 2020 2020  ric.            
-0001bc00: 2020 2020 2020 2020 6d61 785f 7820 3d20          max_x = 
-0001bc10: 6d61 7828 6d61 785f 782c 2068 6f6c 655f  max(max_x, hole_
-0001bc20: 7261 6469 7573 290a 2020 2020 2020 2020  radius).        
-0001bc30: 2020 2020 2020 2020 2020 2020 7261 6420              rad 
-0001bc40: 3d20 686f 6c65 5f72 6164 6975 7320 2a20  = hole_radius * 
-0001bc50: 2831 3030 202d 2064 6566 696e 6974 696f  (100 - definitio
-0001bc60: 6e2e 686f 6c65 5f70 6c61 7469 6e67 5f72  n.hole_plating_r
-0001bc70: 6174 696f 2920 2f20 3130 300a 2020 2020  atio) / 100.    
-0001bc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bc90: 7820 3d20 5b78 5f73 7461 7274 202d 2072  x = [x_start - r
-0001bca0: 6164 2c20 785f 7374 6172 7420 2d20 7261  ad, x_start - ra
-0001bcb0: 642c 2078 5f73 7461 7274 202b 2072 6164  d, x_start + rad
-0001bcc0: 2c20 785f 7374 6172 7420 2b20 7261 645d  , x_start + rad]
-0001bcd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001bce0: 2020 2020 2070 6c6f 745f 6461 7461 2e61       plot_data.a
-0001bcf0: 7070 656e 6428 5b78 2c20 792c 2063 6f6c  ppend([x, y, col
-0001bd00: 6f72 5f6b 6579 735b 636f 6c6f 725f 696e  or_keys[color_in
-0001bd10: 6465 785d 2c20 4e6f 6e65 2c20 312e 302c  dex], None, 1.0,
-0001bd20: 2022 6669 6c6c 225d 290a 0a20 2020 2020   "fill"])..     
-0001bd30: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
-0001bd40: 5f69 6e64 6578 202b 3d20 310a 2020 2020  _index += 1.    
-0001bd50: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-0001bd60: 6f6c 6f72 5f69 6e64 6578 203d 3d20 6d61  olor_index == ma
-0001bd70: 785f 706c 6f74 733a 0a20 2020 2020 2020  x_plots:.       
-0001bd80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0001bd90: 662e 5f6c 6f67 6765 722e 7761 726e 696e  f._logger.warnin
-0001bda0: 6728 224d 6178 696d 756d 206e 756d 6265  g("Maximum numbe
-0001bdb0: 7220 6f66 2064 6566 696e 6974 696f 6e73  r of definitions
-0001bdc0: 2070 6c6f 7474 6564 2e22 290a 2020 2020   plotted.").    
-0001bdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bde0: 6272 6561 6b0a 2020 2020 2020 2020 2020  break.          
-0001bdf0: 2020 2020 2020 785f 7374 6172 7420 2b3d        x_start +=
-0001be00: 2064 656c 7461 0a0a 2020 2020 2020 2020   delta..        
-0001be10: 2320 706c 6f74 2074 6865 2073 7461 636b  # plot the stack
-0001be20: 7570 0a20 2020 2020 2020 2070 6c74 203d  up.        plt =
-0001be30: 2070 6c6f 745f 6d61 7470 6c6f 746c 6962   plot_matplotlib
-0001be40: 280a 2020 2020 2020 2020 2020 2020 706c  (.            pl
-0001be50: 6f74 5f64 6174 612c 0a20 2020 2020 2020  ot_data,.       
-0001be60: 2020 2020 2073 697a 653d 7369 7a65 2c0a       size=size,.
-0001be70: 2020 2020 2020 2020 2020 2020 7368 6f77              show
-0001be80: 5f6c 6567 656e 643d 4661 6c73 652c 0a20  _legend=False,. 
-0001be90: 2020 2020 2020 2020 2020 2078 6c61 6265             xlabe
-0001bea0: 6c3d 2222 2c0a 2020 2020 2020 2020 2020  l="",.          
-0001beb0: 2020 796c 6162 656c 3d22 222c 0a20 2020    ylabel="",.   
-0001bec0: 2020 2020 2020 2020 2074 6974 6c65 3d22           title="
-0001bed0: 222c 0a20 2020 2020 2020 2020 2020 2073  ",.            s
-0001bee0: 6e61 7073 686f 745f 7061 7468 3d4e 6f6e  napshot_path=Non
-0001bef0: 652c 0a20 2020 2020 2020 2020 2020 2078  e,.            x
-0001bf00: 5f6c 696d 6974 733d 5b78 5f6d 696e 2c20  _limits=[x_min, 
-0001bf10: 785f 6d61 785d 2c0a 2020 2020 2020 2020  x_max],.        
-0001bf20: 2020 2020 795f 6c69 6d69 7473 3d5b 795f      y_limits=[y_
-0001bf30: 6d69 6e2c 2079 5f6d 6178 5d2c 0a20 2020  min, y_max],.   
-0001bf40: 2020 2020 2020 2020 2061 7869 735f 6571           axis_eq
-0001bf50: 7561 6c3d 4661 6c73 652c 0a20 2020 2020  ual=False,.     
-0001bf60: 2020 2020 2020 2061 6e6e 6f74 6174 696f         annotatio
-0001bf70: 6e73 3d61 6e6e 6f74 6174 696f 6e73 2c0a  ns=annotations,.
-0001bf80: 2020 2020 2020 2020 2020 2020 7368 6f77              show
-0001bf90: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-0001bfa0: 290a 2020 2020 2020 2020 2320 7765 2068  ).        # we h
-0001bfb0: 6176 6520 746f 2063 7573 746f 6d69 7a65  ave to customize
-0001bfc0: 2073 6f6d 6520 6465 6661 756c 7473 2c20   some defaults, 
-0001bfd0: 736f 2077 6520 706c 6f74 206f 7220 7361  so we plot or sa
-0001bfe0: 7665 2074 6865 2066 6967 7572 6520 6865  ve the figure he
-0001bff0: 7265 0a20 2020 2020 2020 2070 6c74 2e61  re.        plt.a
-0001c000: 7869 7328 226f 6666 2229 0a20 2020 2020  xis("off").     
-0001c010: 2020 2070 6c74 2e62 6f78 2846 616c 7365     plt.box(False
-0001c020: 290a 2020 2020 2020 2020 706c 742e 7469  ).        plt.ti
-0001c030: 746c 6528 2253 7461 636b 7570 5c6e 2022  tle("Stackup\n "
-0001c040: 2c20 666f 6e74 7369 7a65 3d32 3829 0a20  , fontsize=28). 
-0001c050: 2020 2020 2020 2023 2065 7661 6c75 6174         # evaluat
-0001c060: 6573 2074 6865 206e 756d 6265 7220 6f66  es the number of
-0001c070: 206c 6567 656e 6420 636f 6c75 6d6e 2062   legend column b
-0001c080: 6173 6564 206f 6e20 7468 6520 6c61 7965  ased on the laye
-0001c090: 7220 6e61 6d65 206d 6178 206c 656e 6774  r name max lengt
-0001c0a0: 680a 2020 2020 2020 2020 6e63 6f6c 203d  h.        ncol =
-0001c0b0: 2033 2069 6620 6d61 7828 5b6c 656e 286e   3 if max([len(n
-0001c0c0: 2920 666f 7220 6e20 696e 206c 6179 6572  ) for n in layer
-0001c0d0: 5f6e 616d 6573 5d29 203c 2031 3520 656c  _names]) < 15 el
-0001c0e0: 7365 2032 0a20 2020 2020 2020 2068 616e  se 2.        han
-0001c0f0: 646c 6573 2c20 6c61 6265 6c73 203d 2070  dles, labels = p
-0001c100: 6c74 2e67 6361 2829 2e67 6574 5f6c 6567  lt.gca().get_leg
-0001c110: 656e 645f 6861 6e64 6c65 735f 6c61 6265  end_handles_labe
-0001c120: 6c73 2829 0a20 2020 2020 2020 2070 6c74  ls().        plt
-0001c130: 2e6c 6567 656e 6428 0a20 2020 2020 2020  .legend(.       
-0001c140: 2020 2020 205b 6861 6e64 6c65 735b 6964       [handles[id
-0001c150: 785d 2066 6f72 2069 6478 2069 6e20 6c65  x] for idx in le
-0001c160: 6765 6e64 5f6f 7264 6572 5d2c 0a20 2020  gend_order],.   
-0001c170: 2020 2020 2020 2020 205b 6c61 6265 6c73           [labels
-0001c180: 5b69 6478 5d20 666f 7220 6964 7820 696e  [idx] for idx in
-0001c190: 206c 6567 656e 645f 6f72 6465 725d 2c0a   legend_order],.
-0001c1a0: 2020 2020 2020 2020 2020 2020 6262 6f78              bbox
-0001c1b0: 5f74 6f5f 616e 6368 6f72 3d28 302c 202d  _to_anchor=(0, -
-0001c1c0: 302e 3035 292c 0a20 2020 2020 2020 2020  0.05),.         
-0001c1d0: 2020 206c 6f63 3d22 7570 7065 7220 6c65     loc="upper le
-0001c1e0: 6674 222c 0a20 2020 2020 2020 2020 2020  ft",.           
-0001c1f0: 2062 6f72 6465 7261 7865 7370 6164 3d30   borderaxespad=0
-0001c200: 2c0a 2020 2020 2020 2020 2020 2020 6e63  ,.            nc
-0001c210: 6f6c 3d6e 636f 6c2c 0a20 2020 2020 2020  ol=ncol,.       
-0001c220: 2029 0a20 2020 2020 2020 2070 6c74 2e74   ).        plt.t
-0001c230: 6967 6874 5f6c 6179 6f75 7428 290a 2020  ight_layout().  
-0001c240: 2020 2020 2020 6966 2073 6176 655f 706c        if save_pl
-0001c250: 6f74 3a0a 2020 2020 2020 2020 2020 2020  ot:.            
-0001c260: 706c 742e 7361 7665 6669 6728 7361 7665  plt.savefig(save
-0001c270: 5f70 6c6f 7429 0a20 2020 2020 2020 2065  _plot).        e
-0001c280: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0001c290: 2070 6c74 2e73 686f 7728 290a 2020 2020   plt.show().    
-0001c2a0: 2020 2020 7265 7475 726e 2070 6c74 0a        return plt.
+0001b9a0: 206d 696e 5f6c 6520 3d20 6d69 6e28 6c6f   min_le = min(lo
+0001b9b0: 7765 725f 656c 6576 6174 696f 6e2c 206d  wer_elevation, m
+0001b9c0: 696e 5f6c 6529 0a20 2020 2020 2020 2020  in_le).         
+0001b9d0: 2020 2020 2020 2020 2020 206d 6178 5f75             max_u
+0001b9e0: 6520 3d20 6d61 7828 7570 7065 725f 656c  e = max(upper_el
+0001b9f0: 6576 6174 696f 6e2c 206d 6178 5f75 6529  evation, max_ue)
+0001ba00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ba10: 2069 6620 6465 6669 6e69 7469 6f6e 2e68   if definition.h
+0001ba20: 6f6c 655f 7072 6f70 6572 7469 6573 3a0a  ole_properties:.
+0001ba30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ba40: 2020 2020 2320 6372 6561 7465 2070 6174      # create pat
+0001ba50: 6368 2066 6f72 2074 6865 2068 6f6c 650a  ch for the hole.
+0001ba60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ba70: 2020 2020 686f 6c65 5f72 6164 6975 7320      hole_radius 
+0001ba80: 3d20 6465 6669 6e69 7469 6f6e 2e68 6f6c  = definition.hol
+0001ba90: 655f 7072 6f70 6572 7469 6573 5b30 5d20  e_properties[0] 
+0001baa0: 2f20 3220 2a20 7363 616c 696e 675f 665f  / 2 * scaling_f_
+0001bab0: 7061 640a 2020 2020 2020 2020 2020 2020  pad.            
+0001bac0: 2020 2020 2020 2020 7820 3d20 5b78 5f73          x = [x_s
+0001bad0: 7461 7274 202d 2068 6f6c 655f 7261 6469  tart - hole_radi
+0001bae0: 7573 2c20 785f 7374 6172 7420 2d20 686f  us, x_start - ho
+0001baf0: 6c65 5f72 6164 6975 732c 2078 5f73 7461  le_radius, x_sta
+0001bb00: 7274 202b 2068 6f6c 655f 7261 6469 7573  rt + hole_radius
+0001bb10: 2c20 785f 7374 6172 7420 2b20 686f 6c65  , x_start + hole
+0001bb20: 5f72 6164 6975 735d 0a20 2020 2020 2020  _radius].       
+0001bb30: 2020 2020 2020 2020 2020 2020 2079 203d               y =
+0001bb40: 205b 6d69 6e5f 6c65 2c20 6d61 785f 7565   [min_le, max_ue
+0001bb50: 2c20 6d61 785f 7565 2c20 6d69 6e5f 6c65  , max_ue, min_le
+0001bb60: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0001bb70: 2020 2020 2020 706c 6f74 5f64 6174 612e        plot_data.
+0001bb80: 6170 7065 6e64 285b 782c 2079 2c20 636f  append([x, y, co
+0001bb90: 6c6f 725f 6b65 7973 5b63 6f6c 6f72 5f69  lor_keys[color_i
+0001bba0: 6e64 6578 5d2c 204e 6f6e 652c 2030 2e37  ndex], None, 0.7
+0001bbb0: 2c20 2266 696c 6c22 5d29 0a20 2020 2020  , "fill"]).     
+0001bbc0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0001bbd0: 2063 7265 6174 6520 7061 7463 6820 666f   create patch fo
+0001bbe0: 7220 7468 6520 6469 656c 6563 7472 6963  r the dielectric
+0001bbf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001bc00: 2020 2020 206d 6178 5f78 203d 206d 6178       max_x = max
+0001bc10: 286d 6178 5f78 2c20 686f 6c65 5f72 6164  (max_x, hole_rad
+0001bc20: 6975 7329 0a20 2020 2020 2020 2020 2020  ius).           
+0001bc30: 2020 2020 2020 2020 2072 6164 203d 2068           rad = h
+0001bc40: 6f6c 655f 7261 6469 7573 202a 2028 3130  ole_radius * (10
+0001bc50: 3020 2d20 6465 6669 6e69 7469 6f6e 2e68  0 - definition.h
+0001bc60: 6f6c 655f 706c 6174 696e 675f 7261 7469  ole_plating_rati
+0001bc70: 6f29 202f 2031 3030 0a20 2020 2020 2020  o) / 100.       
+0001bc80: 2020 2020 2020 2020 2020 2020 2078 203d               x =
+0001bc90: 205b 785f 7374 6172 7420 2d20 7261 642c   [x_start - rad,
+0001bca0: 2078 5f73 7461 7274 202d 2072 6164 2c20   x_start - rad, 
+0001bcb0: 785f 7374 6172 7420 2b20 7261 642c 2078  x_start + rad, x
+0001bcc0: 5f73 7461 7274 202b 2072 6164 5d0a 2020  _start + rad].  
+0001bcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bce0: 2020 706c 6f74 5f64 6174 612e 6170 7065    plot_data.appe
+0001bcf0: 6e64 285b 782c 2079 2c20 636f 6c6f 725f  nd([x, y, color_
+0001bd00: 6b65 7973 5b63 6f6c 6f72 5f69 6e64 6578  keys[color_index
+0001bd10: 5d2c 204e 6f6e 652c 2031 2e30 2c20 2266  ], None, 1.0, "f
+0001bd20: 696c 6c22 5d29 0a0a 2020 2020 2020 2020  ill"])..        
+0001bd30: 2020 2020 2020 2020 636f 6c6f 725f 696e          color_in
+0001bd40: 6465 7820 2b3d 2031 0a20 2020 2020 2020  dex += 1.       
+0001bd50: 2020 2020 2020 2020 2069 6620 636f 6c6f           if colo
+0001bd60: 725f 696e 6465 7820 3d3d 206d 6178 5f70  r_index == max_p
+0001bd70: 6c6f 7473 3a0a 2020 2020 2020 2020 2020  lots:.          
+0001bd80: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0001bd90: 6c6f 6767 6572 2e77 6172 6e69 6e67 2822  logger.warning("
+0001bda0: 4d61 7869 6d75 6d20 6e75 6d62 6572 206f  Maximum number o
+0001bdb0: 6620 6465 6669 6e69 7469 6f6e 7320 706c  f definitions pl
+0001bdc0: 6f74 7465 642e 2229 0a20 2020 2020 2020  otted.").       
+0001bdd0: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+0001bde0: 616b 0a20 2020 2020 2020 2020 2020 2020  ak.             
+0001bdf0: 2020 2078 5f73 7461 7274 202b 3d20 6465     x_start += de
+0001be00: 6c74 610a 0a20 2020 2020 2020 2023 2070  lta..        # p
+0001be10: 6c6f 7420 7468 6520 7374 6163 6b75 700a  lot the stackup.
+0001be20: 2020 2020 2020 2020 706c 7420 3d20 706c          plt = pl
+0001be30: 6f74 5f6d 6174 706c 6f74 6c69 6228 0a20  ot_matplotlib(. 
+0001be40: 2020 2020 2020 2020 2020 2070 6c6f 745f             plot_
+0001be50: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
+0001be60: 2020 7369 7a65 3d73 697a 652c 0a20 2020    size=size,.   
+0001be70: 2020 2020 2020 2020 2073 686f 775f 6c65           show_le
+0001be80: 6765 6e64 3d46 616c 7365 2c0a 2020 2020  gend=False,.    
+0001be90: 2020 2020 2020 2020 786c 6162 656c 3d22          xlabel="
+0001bea0: 222c 0a20 2020 2020 2020 2020 2020 2079  ",.            y
+0001beb0: 6c61 6265 6c3d 2222 2c0a 2020 2020 2020  label="",.      
+0001bec0: 2020 2020 2020 7469 746c 653d 2222 2c0a        title="",.
+0001bed0: 2020 2020 2020 2020 2020 2020 736e 6170              snap
+0001bee0: 7368 6f74 5f70 6174 683d 4e6f 6e65 2c0a  shot_path=None,.
+0001bef0: 2020 2020 2020 2020 2020 2020 785f 6c69              x_li
+0001bf00: 6d69 7473 3d5b 785f 6d69 6e2c 2078 5f6d  mits=[x_min, x_m
+0001bf10: 6178 5d2c 0a20 2020 2020 2020 2020 2020  ax],.           
+0001bf20: 2079 5f6c 696d 6974 733d 5b79 5f6d 696e   y_limits=[y_min
+0001bf30: 2c20 795f 6d61 785d 2c0a 2020 2020 2020  , y_max],.      
+0001bf40: 2020 2020 2020 6178 6973 5f65 7175 616c        axis_equal
+0001bf50: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+0001bf60: 2020 2020 616e 6e6f 7461 7469 6f6e 733d      annotations=
+0001bf70: 616e 6e6f 7461 7469 6f6e 732c 0a20 2020  annotations,.   
+0001bf80: 2020 2020 2020 2020 2073 686f 773d 4661           show=Fa
+0001bf90: 6c73 652c 0a20 2020 2020 2020 2029 0a20  lse,.        ). 
+0001bfa0: 2020 2020 2020 2023 2077 6520 6861 7665         # we have
+0001bfb0: 2074 6f20 6375 7374 6f6d 697a 6520 736f   to customize so
+0001bfc0: 6d65 2064 6566 6175 6c74 732c 2073 6f20  me defaults, so 
+0001bfd0: 7765 2070 6c6f 7420 6f72 2073 6176 6520  we plot or save 
+0001bfe0: 7468 6520 6669 6775 7265 2068 6572 650a  the figure here.
+0001bff0: 2020 2020 2020 2020 706c 742e 6178 6973          plt.axis
+0001c000: 2822 6f66 6622 290a 2020 2020 2020 2020  ("off").        
+0001c010: 706c 742e 626f 7828 4661 6c73 6529 0a20  plt.box(False). 
+0001c020: 2020 2020 2020 2070 6c74 2e74 6974 6c65         plt.title
+0001c030: 2822 5374 6163 6b75 705c 6e20 222c 2066  ("Stackup\n ", f
+0001c040: 6f6e 7473 697a 653d 3238 290a 2020 2020  ontsize=28).    
+0001c050: 2020 2020 2320 6576 616c 7561 7465 7320      # evaluates 
+0001c060: 7468 6520 6e75 6d62 6572 206f 6620 6c65  the number of le
+0001c070: 6765 6e64 2063 6f6c 756d 6e20 6261 7365  gend column base
+0001c080: 6420 6f6e 2074 6865 206c 6179 6572 206e  d on the layer n
+0001c090: 616d 6520 6d61 7820 6c65 6e67 7468 0a20  ame max length. 
+0001c0a0: 2020 2020 2020 206e 636f 6c20 3d20 3320         ncol = 3 
+0001c0b0: 6966 206d 6178 285b 6c65 6e28 6e29 2066  if max([len(n) f
+0001c0c0: 6f72 206e 2069 6e20 6c61 7965 725f 6e61  or n in layer_na
+0001c0d0: 6d65 735d 2920 3c20 3135 2065 6c73 6520  mes]) < 15 else 
+0001c0e0: 320a 2020 2020 2020 2020 6861 6e64 6c65  2.        handle
+0001c0f0: 732c 206c 6162 656c 7320 3d20 706c 742e  s, labels = plt.
+0001c100: 6763 6128 292e 6765 745f 6c65 6765 6e64  gca().get_legend
+0001c110: 5f68 616e 646c 6573 5f6c 6162 656c 7328  _handles_labels(
+0001c120: 290a 2020 2020 2020 2020 706c 742e 6c65  ).        plt.le
+0001c130: 6765 6e64 280a 2020 2020 2020 2020 2020  gend(.          
+0001c140: 2020 5b68 616e 646c 6573 5b69 6478 5d20    [handles[idx] 
+0001c150: 666f 7220 6964 7820 696e 206c 6567 656e  for idx in legen
+0001c160: 645f 6f72 6465 725d 2c0a 2020 2020 2020  d_order],.      
+0001c170: 2020 2020 2020 5b6c 6162 656c 735b 6964        [labels[id
+0001c180: 785d 2066 6f72 2069 6478 2069 6e20 6c65  x] for idx in le
+0001c190: 6765 6e64 5f6f 7264 6572 5d2c 0a20 2020  gend_order],.   
+0001c1a0: 2020 2020 2020 2020 2062 626f 785f 746f           bbox_to
+0001c1b0: 5f61 6e63 686f 723d 2830 2c20 2d30 2e30  _anchor=(0, -0.0
+0001c1c0: 3529 2c0a 2020 2020 2020 2020 2020 2020  5),.            
+0001c1d0: 6c6f 633d 2275 7070 6572 206c 6566 7422  loc="upper left"
+0001c1e0: 2c0a 2020 2020 2020 2020 2020 2020 626f  ,.            bo
+0001c1f0: 7264 6572 6178 6573 7061 643d 302c 0a20  rderaxespad=0,. 
+0001c200: 2020 2020 2020 2020 2020 206e 636f 6c3d             ncol=
+0001c210: 6e63 6f6c 2c0a 2020 2020 2020 2020 290a  ncol,.        ).
+0001c220: 2020 2020 2020 2020 706c 742e 7469 6768          plt.tigh
+0001c230: 745f 6c61 796f 7574 2829 0a20 2020 2020  t_layout().     
+0001c240: 2020 2069 6620 7361 7665 5f70 6c6f 743a     if save_plot:
+0001c250: 0a20 2020 2020 2020 2020 2020 2070 6c74  .            plt
+0001c260: 2e73 6176 6566 6967 2873 6176 655f 706c  .savefig(save_pl
+0001c270: 6f74 290a 2020 2020 2020 2020 656c 7365  ot).        else
+0001c280: 3a0a 2020 2020 2020 2020 2020 2020 706c  :.            pl
+0001c290: 742e 7368 6f77 2829 0a20 2020 2020 2020  t.show().       
+0001c2a0: 2072 6574 7572 6e20 706c 740a             return plt.
```

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/utilities/heatsink.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/utilities/heatsink.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/edb_core/utilities/simulation_setup.py` & `pyedb-0.8.1/src/pyedb/dotnet/edb_core/utilities/simulation_setup.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/dotnet/sim_setup_data/data/siw_dc_ir_settings.py` & `pyedb-0.8.1/src/pyedb/dotnet/sim_setup_data/data/siw_dc_ir_settings.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/edb_logger.py` & `pyedb-0.8.1/src/pyedb/edb_logger.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/generic/constants.py` & `pyedb-0.8.1/src/pyedb/generic/constants.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/generic/data_handlers.py` & `pyedb-0.8.1/src/pyedb/generic/data_handlers.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/generic/design_types.py` & `pyedb-0.8.1/src/pyedb/generic/design_types.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/generic/filesystem.py` & `pyedb-0.8.1/src/pyedb/generic/filesystem.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/generic/general_methods.py` & `pyedb-0.8.1/src/pyedb/generic/general_methods.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/generic/plot.py` & `pyedb-0.8.1/src/pyedb/generic/plot.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/generic/process.py` & `pyedb-0.8.1/src/pyedb/generic/process.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/generic/settings.py` & `pyedb-0.8.1/src/pyedb/generic/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import logging
 import os
 import time
 
 
 class Settings(object):
     """Manages all PyEDB environment variables and global settings."""
```

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/bom/bom.py` & `pyedb-0.8.1/src/pyedb/ipc2581/bom/bom.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/bom/bom_item.py` & `pyedb-0.8.1/src/pyedb/ipc2581/bom/bom_item.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/bom/characteristics.py` & `pyedb-0.8.1/src/pyedb/ipc2581/bom/characteristics.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/bom/refdes.py` & `pyedb-0.8.1/src/pyedb/ipc2581/bom/refdes.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/content/color.py` & `pyedb-0.8.1/src/pyedb/ipc2581/content/color.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/content/content.py` & `pyedb-0.8.1/src/pyedb/ipc2581/content/content.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/content/dictionary_color.py` & `pyedb-0.8.1/src/pyedb/ipc2581/content/dictionary_color.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/content/dictionary_fill.py` & `pyedb-0.8.1/src/pyedb/ipc2581/content/dictionary_fill.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/content/dictionary_line.py` & `pyedb-0.8.1/src/pyedb/ipc2581/content/dictionary_line.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/content/entry_color.py` & `pyedb-0.8.1/src/pyedb/ipc2581/content/entry_color.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/content/entry_line.py` & `pyedb-0.8.1/src/pyedb/ipc2581/content/entry_line.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/content/fill.py` & `pyedb-0.8.1/src/pyedb/ipc2581/content/fill.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/content/layer_ref.py` & `pyedb-0.8.1/src/pyedb/ipc2581/content/layer_ref.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/content/standard_geometries_dictionary.py` & `pyedb-0.8.1/src/pyedb/ipc2581/content/standard_geometries_dictionary.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/assembly_drawing.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/assembly_drawing.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/cad_data.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/cad_data.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/component.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/component.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/drill.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/drill.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/feature.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/feature.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/layer.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/layer.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/layer_feature.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/layer_feature.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/logical_net.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/logical_net.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/outline.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/outline.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/package.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/package.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/padstack_def.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/padstack_def.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/padstack_hole_def.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/padstack_hole_def.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/padstack_instance.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/padstack_instance.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/padstack_pad_def.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/padstack_pad_def.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/path.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/path.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/phy_net.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/phy_net.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/pin.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/pin.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/polygon.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/polygon.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/profile.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/profile.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/stackup.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/stackup.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/stackup_group.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/stackup_group.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/stackup_layer.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/stackup_layer.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_data/step.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/step.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/cad_header.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_header.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/ecad.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/ecad.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ecad/spec.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ecad/spec.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/history_record.py` & `pyedb-0.8.1/src/pyedb/ipc2581/history_record.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/ipc2581.py` & `pyedb-0.8.1/src/pyedb/ipc2581/ipc2581.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/ipc2581/logistic_header.py` & `pyedb-0.8.1/src/pyedb/ipc2581/logistic_header.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/misc/aedtlib_personalib_install.py` & `pyedb-0.8.1/src/pyedb/misc/aedtlib_personalib_install.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/misc/downloads.py` & `pyedb-0.8.1/src/pyedb/misc/downloads.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/misc/misc.py` & `pyedb-0.8.1/src/pyedb/misc/misc.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/misc/siw_feature_config/emc/component_tags.py` & `pyedb-0.8.1/src/pyedb/misc/siw_feature_config/emc/component_tags.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/misc/siw_feature_config/emc/net_tags.py` & `pyedb-0.8.1/src/pyedb/misc/siw_feature_config/emc/net_tags.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/misc/siw_feature_config/emc/tag_library.py` & `pyedb-0.8.1/src/pyedb/misc/siw_feature_config/emc/tag_library.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/misc/siw_feature_config/emc/xml_generic.py` & `pyedb-0.8.1/src/pyedb/misc/siw_feature_config/emc/xml_generic.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/misc/siw_feature_config/emc_rule_checker_settings.py` & `pyedb-0.8.1/src/pyedb/misc/siw_feature_config/emc_rule_checker_settings.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/modeler/geometry_operators.py` & `pyedb-0.8.1/src/pyedb/modeler/geometry_operators.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/src/pyedb/siwave.py` & `pyedb-0.8.1/src/pyedb/siwave.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.0/PKG-INFO` & `pyedb-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyedb
-Version: 0.8.0
+Version: 0.8.1
 Summary: Higher-Level Pythonic Ansys Electronics Data Base
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyEDB developers <simon.vandenbrouck@ansys.com>
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```


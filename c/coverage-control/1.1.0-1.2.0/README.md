# Comparing `tmp/coverage_control-1.1.0.tar.gz` & `tmp/coverage_control-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coverage_control-1.1.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "coverage_control-1.2.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `coverage_control-1.1.0.tar` & `coverage_control-1.2.0.tar`

### file list

```diff
@@ -1,230 +1,229 @@
--rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 coverage_control-1.1.0/.git_archival.txt
--rw-r--r--   0        0        0       61 2022-11-09 12:37:21.000000 coverage_control-1.1.0/.gitattributes
--rw-r--r--   0        0        0     1333 2022-11-09 12:37:21.000000 coverage_control-1.1.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 coverage_control-1.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1635 2022-11-09 12:37:21.000000 coverage_control-1.1.0/.github/docker-base-action/action.yml
--rw-r--r--   0        0        0      668 2022-11-09 12:37:21.000000 coverage_control-1.1.0/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1253 2022-11-09 12:37:21.000000 coverage_control-1.1.0/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1714 2022-11-09 12:37:21.000000 coverage_control-1.1.0/.github/workflows/cd_wheels.yml
--rw-r--r--   0        0        0      561 2022-11-09 12:37:21.000000 coverage_control-1.1.0/.github/workflows/ghaction-doxygen-ghpages.yml
--rw-r--r--   0        0        0     2379 2022-11-09 12:37:21.000000 coverage_control-1.1.0/.gitignore
--rw-r--r--   0        0        0     2870 2022-11-09 12:37:21.000000 coverage_control-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        4 2022-11-09 12:37:21.000000 coverage_control-1.1.0/.prettierignore
--rw-r--r--   0        0        0     1757 2022-11-09 12:37:21.000000 coverage_control-1.1.0/CMakeLists.txt
--rw-r--r--   0        0        0    35149 2022-11-09 12:37:21.000000 coverage_control-1.1.0/LICENSE
--rw-r--r--   0        0        0     3418 2022-11-09 12:37:21.000000 coverage_control-1.1.0/README.md
--rw-r--r--   0        0        0     6438 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/CMakeLists.txt
--rw-r--r--   0        0        0      642 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/cmake/CoverageControlConfig.cmake.in
--rw-r--r--   0        0        0      443 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/cmake/CoverageControlConfig.h.in
--rw-r--r--   0        0        0     2140 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/abstract_controller.h
--rw-r--r--   0        0        0     4644 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/centralized_cvt.h
--rw-r--r--   0        0        0     4444 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/clairvoyant_cvt.h
--rw-r--r--   0        0        0     6907 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/decentralized_cvt.h
--rw-r--r--   0        0        0     4216 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/near_optimal_cvt.h
--rw-r--r--   0        0        0     6247 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/near_optimal_cvt_algorithm.h
--rw-r--r--   0        0        0    14125 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/oracle_bang_explore_exploit.h
--rw-r--r--   0        0        0     6826 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/oracle_explore_exploit.h
--rw-r--r--   0        0        0    15316 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/simul_explore_exploit.h
--rw-r--r--   0        0        0     6530 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/bivariate_normal_distribution.h
--rw-r--r--   0        0        0     2477 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/cgal/config.h
--rw-r--r--   0        0        0     2220 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/cgal/polygon_utils.h
--rw-r--r--   0        0        0     3752 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/cgal/utilities.h
--rw-r--r--   0        0        0     2219 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/constants.h
--rw-r--r--   0        0        0    22208 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/coverage_system.h
--rw-r--r--   0        0        0     3320 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/cuda/geometry_utils.cuh
--rw-r--r--   0        0        0     5159 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/cuda_utils.h
--rw-r--r--   0        0        0    27792 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/cuda_helpers/helper_cuda.h
--rw-r--r--   0        0        0    14875 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/cuda_helpers/helper_string.h
--rw-r--r--   0        0        0    90448 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/gnuplot/gnuplot-iostream.h
--rw-r--r--   0        0        0   914638 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/json/json.hpp
--rw-r--r--   0        0        0     2157 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/lsap/Hungarian.h
--rw-r--r--   0        0        0     1291 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/lsap/LICENSE
--rw-r--r--   0        0        0      555 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/lsap/README.txt
--rw-r--r--   0        0        0   485931 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/tomlplusplus/toml.hpp
--rw-r--r--   0        0        0     2769 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/generate_world_map.h
--rw-r--r--   0        0        0     2321 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/geographiclib_wrapper.h
--rw-r--r--   0        0        0     5141 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/map_utils.h
--rw-r--r--   0        0        0     5246 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/parameters.h
--rw-r--r--   0        0        0     5085 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/plotter.h
--rw-r--r--   0        0        0    15301 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/robot_model.h
--rw-r--r--   0        0        0     2859 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/typedefs.h
--rw-r--r--   0        0        0     3999 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/vec2d.h
--rw-r--r--   0        0        0     6529 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/voronoi.h
--rw-r--r--   0        0        0    11924 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/world_idf.h
--rw-r--r--   0        0        0    25544 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/src/coverage_system.cpp
--rw-r--r--   0        0        0     8168 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/src/cuda/cuda_utils.cu
--rw-r--r--   0        0        0    11364 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/src/cuda/generate_world_map.cu
--rw-r--r--   0        0        0     1349 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/src/cuda_utils.cpp
--rw-r--r--   0        0        0    12642 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/src/extern/Hungarian.cpp
--rw-r--r--   0        0        0    10949 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/src/parameters.cpp
--rw-r--r--   0        0        0    10722 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/src/plotter.cpp
--rw-r--r--   0        0        0     3994 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/src/polygon_utils.cpp
--rw-r--r--   0        0        0     9358 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/src/voronoi.cpp
--rw-r--r--   0        0        0     4659 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/src/world_idf.cpp
--rw-r--r--   0        0        0     1878 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/main/CMakeLists.txt
--rw-r--r--   0        0        0     4301 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/main/coverage_algorithm.cpp
--rw-r--r--   0        0        0     2079 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/main/torch/data_generation.cpp
--rw-r--r--   0        0        0     4464 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/main/torch/eval_dist_gnn.cpp
--rw-r--r--   0        0        0     3885 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/main/torch/eval_gnn.cpp
--rw-r--r--   0        0        0     3764 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/main/torch/test_cnn.cpp
--rw-r--r--   0        0        0     1217 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/main/torch/train_cnn.cpp
--rw-r--r--   0        0        0     1210 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/main/torch/train_gnn.cpp
--rw-r--r--   0        0        0     2100 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/main/world_idf.cpp
--rw-r--r--   0        0        0    19463 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/python_bindings/core_binds.h
--rw-r--r--   0        0        0     1513 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/python_bindings/python_binds.cpp
--rwxr-xr-x   0        0        0     4319 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/setup.sh
--rw-r--r--   0        0        0     3261 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/tests/CMakeLists.txt
--rw-r--r--   0        0        0     2056 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/tests/geo_transforms.cpp
--rw-r--r--   0        0        0     2658 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/tests/map_generation.cpp
--rw-r--r--   0        0        0     3234 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/tests/simultaneous_explore_exploit.cpp
--rw-r--r--   0        0        0     2597 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/tests/torch/torch_data_loader.cpp
--rw-r--r--   0        0        0     2749 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/tests/torch/torch_map_conversion.cpp
--rw-r--r--   0        0        0     1288 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/tests/torch/torch_normalization.cpp
--rw-r--r--   0        0        0     6003 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/tests/torch/torch_scripting.cpp
--rw-r--r--   0        0        0     1011 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/tests/torch/torch_test.cpp
--rw-r--r--   0        0        0     3585 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/CMakeLists.txt
--rw-r--r--   0        0        0      764 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/cmake/CoverageControlTorchConfig.cmake.in
--rw-r--r--   0        0        0      242 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/cmake/CoverageControlTorchConfig.h.in
--rw-r--r--   0        0        0     1057 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/base.h
--rw-r--r--   0        0        0     3104 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/cnn_backbone.h
--rw-r--r--   0        0        0     2961 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/cnn_module.h
--rw-r--r--   0        0        0    23777 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/coverage_system.h
--rw-r--r--   0        0        0     4278 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/edge_wts_comm_map_generator.h
--rw-r--r--   0        0        0   485931 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/extern/tomlplusplus/toml.hpp
--rw-r--r--   0        0        0    16536 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/generate_dataset.h
--rw-r--r--   0        0        0     3380 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/gnn_backbone.h
--rw-r--r--   0        0        0     5512 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/mlp.h
--rw-r--r--   0        0        0     7754 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/train_cnn.h
--rw-r--r--   0        0        0     2925 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/type_conversions.h
--rw-r--r--   0        0        0     1214 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/python_bindings/CMakeLists.txt
--rw-r--r--   0        0        0      405 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/python_bindings/pyproject.toml
--rw-r--r--   0        0        0     6075 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/python_bindings/src/coverage_control_torch_extension.cpp
--rw-r--r--   0        0        0     1379 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/src/base.cpp
--rw-r--r--   0        0        0     5111 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/src/coverage_system.cpp
--rw-r--r--   0        0        0     1228 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/Doxyfile
--rw-r--r--   0        0        0     4824 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/bash-filter.py
--rw-r--r--   0        0        0   127483 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/BaseDoxyfile
--rw-r--r--   0        0        0     6808 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/DoxygenLayout.xml
--rw-r--r--   0        0        0     2957 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/custom.css
--rw-r--r--   0        0        0     8469 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/doxygen-awesome-darkmode-toggle.js
--rw-r--r--   0        0        0     4042 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/doxygen-awesome-fragment-copy-button.js
--rw-r--r--   0        0        0     3177 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/doxygen-awesome-interactive-toc.js
--rw-r--r--   0        0        0     2447 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/doxygen-awesome-paragraph-link.js
--rw-r--r--   0        0        0     1474 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/doxygen-awesome-sidebar-only-darkmode-toggle.css
--rw-r--r--   0        0        0     3287 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/doxygen-awesome-sidebar-only.css
--rw-r--r--   0        0        0     3797 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/doxygen-awesome-tabs.js
--rw-r--r--   0        0        0    67222 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/doxygen-awesome.css
--rw-r--r--   0        0        0     5455 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/header.html
--rw-r--r--   0        0        0    15889 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/navtree-hacks.js
--rw-r--r--   0        0        0  6603024 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/graphics/LPAC.gif
--rw-r--r--   0        0        0  1443985 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/graphics/SearchRescue.png
--rw-r--r--   0        0        0   831774 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/graphics/coveragecontrol_global.png
--rw-r--r--   0        0        0  1111552 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/graphics/learnable_pac.png
--rw-r--r--   0        0        0       12 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/manual/CUDA-installation-troubleshooting.md
--rw-r--r--   0        0        0     3629 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/manual/README.md
--rw-r--r--   0        0        0     6274 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/manual/algorithms.md
--rw-r--r--   0        0        0     7513 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/manual/coverage-control.md
--rw-r--r--   0        0        0     2671 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/manual/docker.md
--rw-r--r--   0        0        0     5747 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/manual/installation.md
--rw-r--r--   0        0        0     3082 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/manual/lpac.md
--rw-r--r--   0        0        0     5038 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/manual/quick_start.md
--rw-r--r--   0        0        0      721 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/manual/ref_manual.txt
--rwxr-xr-x   0        0        0       34 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/py-filter.sh
--rw-r--r--   0        0        0     2578 2022-11-09 12:37:21.000000 coverage_control-1.1.0/params/coverage_control_params.toml
--rw-r--r--   0        0        0     1155 2022-11-09 12:37:21.000000 coverage_control-1.1.0/params/data_params.toml
--rw-r--r--   0        0        0      900 2022-11-09 12:37:21.000000 coverage_control-1.1.0/params/eval.toml
--rw-r--r--   0        0        0     1074 2022-11-09 12:37:21.000000 coverage_control-1.1.0/params/eval_single.toml
--rw-r--r--   0        0        0      837 2022-11-09 12:37:21.000000 coverage_control-1.1.0/params/learning_params.toml
--rw-r--r--   0        0        0     3876 2022-11-09 12:37:21.000000 coverage_control-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      457 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/__init__.py
--rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/_version.py
--rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/_version.pyi
--rw-r--r--   0        0        0      268 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/algorithms/__init__.py
--rw-r--r--   0        0        0      656 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/core/__init__.py
--rw-r--r--   0        0        0     3572 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/io_utils.py
--rw-r--r--   0        0        0      446 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/__init__.py
--rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/data_loaders/__init__.py
--rw-r--r--   0        0        0    14354 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/data_loaders/coverage_env_utils.py
--rw-r--r--   0        0        0     7690 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/data_loaders/data_loader_utils.py
--rw-r--r--   0        0        0     8753 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/data_loaders/loaders.py
--rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/models/__init__.py
--rw-r--r--   0        0        0     2610 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/models/cnn.py
--rw-r--r--   0        0        0     3374 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/models/cnn_backbone.py
--rw-r--r--   0        0        0     2560 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/models/config_parser.py
--rw-r--r--   0        0        0     2282 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/models/gnn_backbone.py
--rw-r--r--   0        0        0     3922 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/models/lpac.py
--rw-r--r--   0        0        0      129 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/trainers/__init__.py
--rw-r--r--   0        0        0     8195 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/trainers/trainer.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/py.typed
--rw-r--r--   0        0        0     2808 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/coverage_env/coverage_class.py
--rw-r--r--   0        0        0     2018 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/coverage_env/coverage_simple.py
--rw-r--r--   0        0        0     1283 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/coverage_env/world_idf.py
--rw-r--r--   0        0        0     2480 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/coverage_env/world_map_numpy.py
--rw-r--r--   0        0        0    16013 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/data_generation/data_generation.py
--rwxr-xr-x   0        0        0      150 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/data_generation/gen.sh
--rw-r--r--   0        0        0    11910 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/data_generation/simple_data_generation.py
--rw-r--r--   0        0        0     5359 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/evaluators/controller.py
--rw-r--r--   0        0        0     1284 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/evaluators/deprecated/eval_multi.py
--rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/evaluators/deprecated/eval_rf_exp.py
--rw-r--r--   0        0        0     7617 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/evaluators/deprecated/eval_semantic_video.py
--rw-r--r--   0        0        0     9535 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/evaluators/deprecated/eval_video.py
--rw-r--r--   0        0        0    10152 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/evaluators/deprecated/semantic_eval.py
--rw-r--r--   0        0        0     6547 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/evaluators/eval.py
--rw-r--r--   0        0        0     5705 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/evaluators/eval_single_env.py
--rw-r--r--   0        0        0     3468 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/training/train_cnn.py
--rw-r--r--   0        0        0     4049 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/training/train_lpac.py
--rw-r--r--   0        0        0     5830 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/data_generators/cnn_data_generation.py
--rw-r--r--   0        0        0     6652 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/data_generators/cnn_data_generation_NoCommsMap.py
--rw-r--r--   0        0        0     7866 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/data_generators/dense_gnn_NoCommMaps_data_generation.py
--rw-r--r--   0        0        0     6804 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/data_generators/dense_gnn_data_generation.py
--rw-r--r--   0        0        0     6111 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/data_generators/gnn_NoCNNmaps_data_generation.py
--rw-r--r--   0        0        0     7892 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/data_generators/sparse_gnn_NoCommsMap_data_generation.py
--rw-r--r--   0        0        0     7140 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/data_generators/sparse_gnn_data_generation.py
--rw-r--r--   0        0        0     3562 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/gnn.py
--rw-r--r--   0        0        0     4851 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/gnn_dist.py
--rw-r--r--   0        0        0     2948 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/mlp_test.py
--rw-r--r--   0        0        0      361 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/plot_edge_weights.py
--rw-r--r--   0        0        0     3574 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/test_cnn.py
--rw-r--r--   0        0        0      350 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/test_jit_tensor.py
--rw-r--r--   0        0        0     6115 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/test_library_objects.py
--rw-r--r--   0        0        0     3977 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/test_lpac_coverage.py
--rw-r--r--   0        0        0     2840 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/testplot.py
--rw-r--r--   0        0        0     2861 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/torch_compat.py
--rw-r--r--   0        0        0     3870 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/test_coverage.py
--rw-r--r--   0        0        0     9921 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/test_coverage_env_utils.py
--rw-r--r--   0        0        0     1859 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/test_env_io.py
--rw-r--r--   0        0        0     2042 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/test_map_generation.py
--rw-r--r--   0        0        0     3583 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/test_models.py
--rw-r--r--   0        0        0     1083 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/test_package.py
--rw-r--r--   0        0        0     2242 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/test_parameters.py
--rw-r--r--   0        0        0     2200 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/test_parity.py
--rw-r--r--   0        0        0    27669 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/ts_jit/TorchVisionResize_32.pt
--rw-r--r--   0        0        0     1552 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/ts_jit/gnn_backbone.py
--rw-r--r--   0        0        0      581 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/ts_jit/torchvision_resize.py
--rw-r--r--   0        0        0     5928 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/utils/dataset_utils.py
--rw-r--r--   0        0        0     1146 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/utils/generate_video.py
--rw-r--r--   0        0        0      304 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/utils/process_data.sh
--rw-r--r--   0        0        0     2941 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/utils/save_gnn_params.py
--rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/utils/save_state_dict.py
--rwxr-xr-x   0        0        0     2993 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup.sh
--rwxr-xr-x   0        0        0     1163 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/check_headers.sh
--rw-r--r--   0        0        0      468 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/docker/Dockerfile
--rwxr-xr-x   0        0        0     4196 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/docker/base_images/.bashrc
--rwxr-xr-x   0        0        0     4514 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/docker/base_images/.ros.bashrc
--rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/docker/base_images/build_all_images.sh
--rw-r--r--   0        0        0      297 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/docker/base_images/requirements.txt
--rw-r--r--   0        0        0      345 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/docker/base_images/requirements_cpu.txt
--rw-r--r--   0        0        0     3410 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/docker/base_images/ubuntu22.04-cuda-ros2.Dockerfile
--rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/docker/base_images/ubuntu22.04-cuda.Dockerfile
--rw-r--r--   0        0        0     3382 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/docker/base_images/ubuntu22.04-ros2.Dockerfile
--rw-r--r--   0        0        0     2576 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/docker/base_images/ubuntu22.04.Dockerfile
--rwxr-xr-x   0        0        0     1436 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/docker/create_container.sh
--rwxr-xr-x   0        0        0       68 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/docker/entrypoint.sh
--rw-r--r--   0        0        0      198 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/helpers.sh
--rwxr-xr-x   0        0        0    10447 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/install_dependencies.sh
--rwxr-xr-x   0        0        0      911 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/install_libtorch.sh
--rwxr-xr-x   0        0        0      633 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/manylinux_2_28_before-all.sh
--rw-r--r--   0        0        0     1659 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/noxfile.py
--rw-r--r--   0        0        0      312 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/requirements.txt
--rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/requirements_cpu.txt
--rw-r--r--   0        0        0    45505 2022-11-09 12:37:21.000000 coverage_control-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 coverage_control-1.2.0/.git_archival.txt
+-rw-r--r--   0        0        0       61 2022-11-09 12:37:21.000000 coverage_control-1.2.0/.gitattributes
+-rw-r--r--   0        0        0     1333 2022-11-09 12:37:21.000000 coverage_control-1.2.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 coverage_control-1.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1635 2022-11-09 12:37:21.000000 coverage_control-1.2.0/.github/docker-base-action/action.yml
+-rw-r--r--   0        0        0      668 2022-11-09 12:37:21.000000 coverage_control-1.2.0/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     2858 2022-11-09 12:37:21.000000 coverage_control-1.2.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0      525 2022-11-09 12:37:21.000000 coverage_control-1.2.0/.github/workflows/ghaction-doxygen-ghpages.yml
+-rw-r--r--   0        0        0     2379 2022-11-09 12:37:21.000000 coverage_control-1.2.0/.gitignore
+-rw-r--r--   0        0        0     2870 2022-11-09 12:37:21.000000 coverage_control-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        4 2022-11-09 12:37:21.000000 coverage_control-1.2.0/.prettierignore
+-rw-r--r--   0        0        0     1757 2022-11-09 12:37:21.000000 coverage_control-1.2.0/CMakeLists.txt
+-rw-r--r--   0        0        0    35149 2022-11-09 12:37:21.000000 coverage_control-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3343 2022-11-09 12:37:21.000000 coverage_control-1.2.0/README.md
+-rw-r--r--   0        0        0     6633 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/CMakeLists.txt
+-rw-r--r--   0        0        0      642 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/cmake/CoverageControlConfig.cmake.in
+-rw-r--r--   0        0        0      443 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/cmake/CoverageControlConfig.h.in
+-rw-r--r--   0        0        0     2140 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/algorithms/abstract_controller.h
+-rw-r--r--   0        0        0     4644 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/algorithms/centralized_cvt.h
+-rw-r--r--   0        0        0     4583 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/algorithms/clairvoyant_cvt.h
+-rw-r--r--   0        0        0     6907 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/algorithms/decentralized_cvt.h
+-rw-r--r--   0        0        0     4216 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/algorithms/near_optimal_cvt.h
+-rw-r--r--   0        0        0     6247 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/algorithms/near_optimal_cvt_algorithm.h
+-rw-r--r--   0        0        0    14125 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/algorithms/oracle_bang_explore_exploit.h
+-rw-r--r--   0        0        0     6826 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/algorithms/oracle_explore_exploit.h
+-rw-r--r--   0        0        0    15316 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/algorithms/simul_explore_exploit.h
+-rw-r--r--   0        0        0     6530 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/bivariate_normal_distribution.h
+-rw-r--r--   0        0        0     2477 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/cgal/config.h
+-rw-r--r--   0        0        0     2220 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/cgal/polygon_utils.h
+-rw-r--r--   0        0        0     3752 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/cgal/utilities.h
+-rw-r--r--   0        0        0     2219 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/constants.h
+-rw-r--r--   0        0        0    22533 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/coverage_system.h
+-rw-r--r--   0        0        0     3320 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/cuda/geometry_utils.cuh
+-rw-r--r--   0        0        0     5159 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/cuda_utils.h
+-rw-r--r--   0        0        0    27792 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/extern/cuda_helpers/helper_cuda.h
+-rw-r--r--   0        0        0    14875 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/extern/cuda_helpers/helper_string.h
+-rw-r--r--   0        0        0    90448 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/extern/gnuplot/gnuplot-iostream.h
+-rw-r--r--   0        0        0   914638 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/extern/json/json.hpp
+-rw-r--r--   0        0        0     2157 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/extern/lsap/Hungarian.h
+-rw-r--r--   0        0        0     1291 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/extern/lsap/LICENSE
+-rw-r--r--   0        0        0      555 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/extern/lsap/README.txt
+-rw-r--r--   0        0        0   485931 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/extern/tomlplusplus/toml.hpp
+-rw-r--r--   0        0        0     2769 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/generate_world_map.h
+-rw-r--r--   0        0        0     2321 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/geographiclib_wrapper.h
+-rw-r--r--   0        0        0     5141 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/map_utils.h
+-rw-r--r--   0        0        0     5511 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/parameters.h
+-rw-r--r--   0        0        0     5085 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/plotter.h
+-rw-r--r--   0        0        0    15353 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/robot_model.h
+-rw-r--r--   0        0        0     2859 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/typedefs.h
+-rw-r--r--   0        0        0     3999 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/vec2d.h
+-rw-r--r--   0        0        0     6529 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/voronoi.h
+-rw-r--r--   0        0        0    11924 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/include/CoverageControl/world_idf.h
+-rw-r--r--   0        0        0    25731 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/src/coverage_system.cpp
+-rw-r--r--   0        0        0     8168 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/src/cuda/cuda_utils.cu
+-rw-r--r--   0        0        0    11364 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/src/cuda/generate_world_map.cu
+-rw-r--r--   0        0        0     1349 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/src/cuda_utils.cpp
+-rw-r--r--   0        0        0    12642 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/src/extern/Hungarian.cpp
+-rw-r--r--   0        0        0    11473 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/src/parameters.cpp
+-rw-r--r--   0        0        0    10980 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/src/plotter.cpp
+-rw-r--r--   0        0        0     3994 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/src/polygon_utils.cpp
+-rw-r--r--   0        0        0     9358 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/src/voronoi.cpp
+-rw-r--r--   0        0        0     4659 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/core/src/world_idf.cpp
+-rw-r--r--   0        0        0     1878 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/main/CMakeLists.txt
+-rw-r--r--   0        0        0     3359 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/main/coverage_algorithm.cpp
+-rw-r--r--   0        0        0     2079 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/main/torch/data_generation.cpp
+-rw-r--r--   0        0        0     4464 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/main/torch/eval_dist_gnn.cpp
+-rw-r--r--   0        0        0     3885 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/main/torch/eval_gnn.cpp
+-rw-r--r--   0        0        0     3764 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/main/torch/test_cnn.cpp
+-rw-r--r--   0        0        0     1217 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/main/torch/train_cnn.cpp
+-rw-r--r--   0        0        0     1210 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/main/torch/train_gnn.cpp
+-rw-r--r--   0        0        0     1158 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/main/world_idf.cpp
+-rw-r--r--   0        0        0    19905 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/python_bindings/core_binds.h
+-rw-r--r--   0        0        0     1513 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/python_bindings/python_binds.cpp
+-rwxr-xr-x   0        0        0     4319 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/setup.sh
+-rw-r--r--   0        0        0     3261 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/tests/CMakeLists.txt
+-rw-r--r--   0        0        0     2056 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/tests/geo_transforms.cpp
+-rw-r--r--   0        0        0     2658 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/tests/map_generation.cpp
+-rw-r--r--   0        0        0     3234 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/tests/simultaneous_explore_exploit.cpp
+-rw-r--r--   0        0        0     2597 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/tests/torch/torch_data_loader.cpp
+-rw-r--r--   0        0        0     2749 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/tests/torch/torch_map_conversion.cpp
+-rw-r--r--   0        0        0     1288 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/tests/torch/torch_normalization.cpp
+-rw-r--r--   0        0        0     6003 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/tests/torch/torch_scripting.cpp
+-rw-r--r--   0        0        0     1011 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/tests/torch/torch_test.cpp
+-rw-r--r--   0        0        0     3585 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/torch/CMakeLists.txt
+-rw-r--r--   0        0        0      764 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/torch/cmake/CoverageControlTorchConfig.cmake.in
+-rw-r--r--   0        0        0      242 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/torch/cmake/CoverageControlTorchConfig.h.in
+-rw-r--r--   0        0        0     1057 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/torch/include/CoverageControlTorch/base.h
+-rw-r--r--   0        0        0     3104 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/torch/include/CoverageControlTorch/cnn_backbone.h
+-rw-r--r--   0        0        0     2961 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/torch/include/CoverageControlTorch/cnn_module.h
+-rw-r--r--   0        0        0    23777 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/torch/include/CoverageControlTorch/coverage_system.h
+-rw-r--r--   0        0        0     4278 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/torch/include/CoverageControlTorch/edge_wts_comm_map_generator.h
+-rw-r--r--   0        0        0   485931 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/torch/include/CoverageControlTorch/extern/tomlplusplus/toml.hpp
+-rw-r--r--   0        0        0    16536 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/torch/include/CoverageControlTorch/generate_dataset.h
+-rw-r--r--   0        0        0     3380 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/torch/include/CoverageControlTorch/gnn_backbone.h
+-rw-r--r--   0        0        0     5512 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/torch/include/CoverageControlTorch/mlp.h
+-rw-r--r--   0        0        0     7754 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/torch/include/CoverageControlTorch/train_cnn.h
+-rw-r--r--   0        0        0     2925 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/torch/include/CoverageControlTorch/type_conversions.h
+-rw-r--r--   0        0        0     1214 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/torch/python_bindings/CMakeLists.txt
+-rw-r--r--   0        0        0      405 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/torch/python_bindings/pyproject.toml
+-rw-r--r--   0        0        0     6075 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/torch/python_bindings/src/coverage_control_torch_extension.cpp
+-rw-r--r--   0        0        0     1379 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/torch/src/base.cpp
+-rw-r--r--   0        0        0     5111 2022-11-09 12:37:21.000000 coverage_control-1.2.0/cppsrc/torch/src/coverage_system.cpp
+-rw-r--r--   0        0        0     1284 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/Doxyfile
+-rw-r--r--   0        0        0     4824 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/bash-filter.py
+-rw-r--r--   0        0        0   127483 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/config/BaseDoxyfile
+-rw-r--r--   0        0        0     6808 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/config/DoxygenLayout.xml
+-rw-r--r--   0        0        0     2957 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/config/custom.css
+-rw-r--r--   0        0        0     8469 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/config/doxygen-awesome-darkmode-toggle.js
+-rw-r--r--   0        0        0     4042 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/config/doxygen-awesome-fragment-copy-button.js
+-rw-r--r--   0        0        0     3177 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/config/doxygen-awesome-interactive-toc.js
+-rw-r--r--   0        0        0     2447 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/config/doxygen-awesome-paragraph-link.js
+-rw-r--r--   0        0        0     1474 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/config/doxygen-awesome-sidebar-only-darkmode-toggle.css
+-rw-r--r--   0        0        0     3287 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/config/doxygen-awesome-sidebar-only.css
+-rw-r--r--   0        0        0     3797 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/config/doxygen-awesome-tabs.js
+-rw-r--r--   0        0        0    67222 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/config/doxygen-awesome.css
+-rw-r--r--   0        0        0     5455 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/config/header.html
+-rw-r--r--   0        0        0    15889 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/config/navtree-hacks.js
+-rw-r--r--   0        0        0  6603024 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/graphics/LPAC.gif
+-rw-r--r--   0        0        0  1443985 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/graphics/SearchRescue.png
+-rw-r--r--   0        0        0   831774 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/graphics/coveragecontrol_global.png
+-rw-r--r--   0        0        0  1111552 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/graphics/learnable_pac.png
+-rw-r--r--   0        0        0       12 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/manual/CUDA-installation-troubleshooting.md
+-rw-r--r--   0        0        0     3577 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/manual/README.md
+-rw-r--r--   0        0        0     6274 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/manual/algorithms.md
+-rw-r--r--   0        0        0     7513 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/manual/coverage-control.md
+-rw-r--r--   0        0        0     2671 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/manual/docker.md
+-rw-r--r--   0        0        0     5809 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/manual/installation.md
+-rw-r--r--   0        0        0     3137 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/manual/lpac.md
+-rw-r--r--   0        0        0     5038 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/manual/quick_start.md
+-rw-r--r--   0        0        0      721 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/manual/ref_manual.txt
+-rwxr-xr-x   0        0        0       34 2022-11-09 12:37:21.000000 coverage_control-1.2.0/doc/py-filter.sh
+-rw-r--r--   0        0        0     2764 2022-11-09 12:37:21.000000 coverage_control-1.2.0/params/coverage_control_params.toml
+-rw-r--r--   0        0        0     1155 2022-11-09 12:37:21.000000 coverage_control-1.2.0/params/data_params.toml
+-rw-r--r--   0        0        0      900 2022-11-09 12:37:21.000000 coverage_control-1.2.0/params/eval.toml
+-rw-r--r--   0        0        0     1074 2022-11-09 12:37:21.000000 coverage_control-1.2.0/params/eval_single.toml
+-rw-r--r--   0        0        0      837 2022-11-09 12:37:21.000000 coverage_control-1.2.0/params/learning_params.toml
+-rw-r--r--   0        0        0     3876 2022-11-09 12:37:21.000000 coverage_control-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      457 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/coverage_control/__init__.py
+-rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/coverage_control/_version.py
+-rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/coverage_control/_version.pyi
+-rw-r--r--   0        0        0      354 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/coverage_control/algorithms/__init__.py
+-rw-r--r--   0        0        0     5419 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/coverage_control/algorithms/controllers.py
+-rw-r--r--   0        0        0      656 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/coverage_control/core/__init__.py
+-rw-r--r--   0        0        0     3572 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/coverage_control/io_utils.py
+-rw-r--r--   0        0        0      446 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/coverage_control/nn/__init__.py
+-rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/coverage_control/nn/data_loaders/__init__.py
+-rw-r--r--   0        0        0    14354 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/coverage_control/nn/data_loaders/coverage_env_utils.py
+-rw-r--r--   0        0        0     7690 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/coverage_control/nn/data_loaders/data_loader_utils.py
+-rw-r--r--   0        0        0     8753 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/coverage_control/nn/data_loaders/loaders.py
+-rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/coverage_control/nn/models/__init__.py
+-rw-r--r--   0        0        0     2610 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/coverage_control/nn/models/cnn.py
+-rw-r--r--   0        0        0     3374 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/coverage_control/nn/models/cnn_backbone.py
+-rw-r--r--   0        0        0     2560 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/coverage_control/nn/models/config_parser.py
+-rw-r--r--   0        0        0     2282 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/coverage_control/nn/models/gnn_backbone.py
+-rw-r--r--   0        0        0     3922 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/coverage_control/nn/models/lpac.py
+-rw-r--r--   0        0        0      129 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/coverage_control/nn/trainers/__init__.py
+-rw-r--r--   0        0        0     8195 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/coverage_control/nn/trainers/trainer.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/coverage_control/py.typed
+-rw-r--r--   0        0        0     1905 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/scripts/coverage_env/coverage_class.py
+-rw-r--r--   0        0        0     1089 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/scripts/coverage_env/coverage_simple.py
+-rw-r--r--   0        0        0      335 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/scripts/coverage_env/world_idf.py
+-rw-r--r--   0        0        0     1551 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/scripts/coverage_env/world_map_numpy.py
+-rw-r--r--   0        0        0    15107 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/scripts/data_generation/data_generation.py
+-rwxr-xr-x   0        0        0      150 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/scripts/data_generation/gen.sh
+-rw-r--r--   0        0        0    12076 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/scripts/data_generation/simple_data_generation.py
+-rw-r--r--   0        0        0     1284 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/scripts/evaluators/deprecated/eval_multi.py
+-rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/scripts/evaluators/deprecated/eval_rf_exp.py
+-rw-r--r--   0        0        0     7617 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/scripts/evaluators/deprecated/eval_semantic_video.py
+-rw-r--r--   0        0        0     9535 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/scripts/evaluators/deprecated/eval_video.py
+-rw-r--r--   0        0        0    10152 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/scripts/evaluators/deprecated/semantic_eval.py
+-rw-r--r--   0        0        0     5760 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/scripts/evaluators/eval.py
+-rw-r--r--   0        0        0     5858 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/scripts/evaluators/eval_single_env.py
+-rw-r--r--   0        0        0     2577 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/scripts/training/train_cnn.py
+-rw-r--r--   0        0        0     3180 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/scripts/training/train_lpac.py
+-rw-r--r--   0        0        0     5830 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/deprecated/data_generators/cnn_data_generation.py
+-rw-r--r--   0        0        0     6652 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/deprecated/data_generators/cnn_data_generation_NoCommsMap.py
+-rw-r--r--   0        0        0     7866 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/deprecated/data_generators/dense_gnn_NoCommMaps_data_generation.py
+-rw-r--r--   0        0        0     6804 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/deprecated/data_generators/dense_gnn_data_generation.py
+-rw-r--r--   0        0        0     6111 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/deprecated/data_generators/gnn_NoCNNmaps_data_generation.py
+-rw-r--r--   0        0        0     7892 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/deprecated/data_generators/sparse_gnn_NoCommsMap_data_generation.py
+-rw-r--r--   0        0        0     7140 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/deprecated/data_generators/sparse_gnn_data_generation.py
+-rw-r--r--   0        0        0     3562 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/deprecated/gnn.py
+-rw-r--r--   0        0        0     4851 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/deprecated/gnn_dist.py
+-rw-r--r--   0        0        0     2948 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/deprecated/mlp_test.py
+-rw-r--r--   0        0        0      361 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/deprecated/plot_edge_weights.py
+-rw-r--r--   0        0        0     3574 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/deprecated/test_cnn.py
+-rw-r--r--   0        0        0      350 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/deprecated/test_jit_tensor.py
+-rw-r--r--   0        0        0     6115 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/deprecated/test_library_objects.py
+-rw-r--r--   0        0        0     3977 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/deprecated/test_lpac_coverage.py
+-rw-r--r--   0        0        0     2840 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/deprecated/testplot.py
+-rw-r--r--   0        0        0     2861 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/deprecated/torch_compat.py
+-rw-r--r--   0        0        0     3870 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/test_coverage.py
+-rw-r--r--   0        0        0     9921 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/test_coverage_env_utils.py
+-rw-r--r--   0        0        0     1859 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/test_env_io.py
+-rw-r--r--   0        0        0     2042 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/test_map_generation.py
+-rw-r--r--   0        0        0     3583 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/test_models.py
+-rw-r--r--   0        0        0     1083 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/test_package.py
+-rw-r--r--   0        0        0     2242 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/test_parameters.py
+-rw-r--r--   0        0        0     2200 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/tests/test_parity.py
+-rw-r--r--   0        0        0    27669 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/ts_jit/TorchVisionResize_32.pt
+-rw-r--r--   0        0        0     1552 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/ts_jit/gnn_backbone.py
+-rw-r--r--   0        0        0      581 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/ts_jit/torchvision_resize.py
+-rw-r--r--   0        0        0     5928 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/utils/dataset_utils.py
+-rw-r--r--   0        0        0     1146 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/utils/generate_video.py
+-rw-r--r--   0        0        0      304 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/utils/process_data.sh
+-rw-r--r--   0        0        0     2941 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/utils/save_gnn_params.py
+-rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 coverage_control-1.2.0/python/utils/save_state_dict.py
+-rwxr-xr-x   0        0        0     2993 2022-11-09 12:37:21.000000 coverage_control-1.2.0/setup.sh
+-rwxr-xr-x   0        0        0     1163 2022-11-09 12:37:21.000000 coverage_control-1.2.0/setup_utils/check_headers.sh
+-rw-r--r--   0        0        0      548 2022-11-09 12:37:21.000000 coverage_control-1.2.0/setup_utils/docker/Dockerfile
+-rwxr-xr-x   0        0        0     4196 2022-11-09 12:37:21.000000 coverage_control-1.2.0/setup_utils/docker/base_images/.bashrc
+-rwxr-xr-x   0        0        0     4514 2022-11-09 12:37:21.000000 coverage_control-1.2.0/setup_utils/docker/base_images/.ros.bashrc
+-rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 coverage_control-1.2.0/setup_utils/docker/base_images/build_all_images.sh
+-rw-r--r--   0        0        0      297 2022-11-09 12:37:21.000000 coverage_control-1.2.0/setup_utils/docker/base_images/requirements.txt
+-rw-r--r--   0        0        0      345 2022-11-09 12:37:21.000000 coverage_control-1.2.0/setup_utils/docker/base_images/requirements_cpu.txt
+-rw-r--r--   0        0        0     3410 2022-11-09 12:37:21.000000 coverage_control-1.2.0/setup_utils/docker/base_images/ubuntu22.04-cuda-ros2.Dockerfile
+-rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 coverage_control-1.2.0/setup_utils/docker/base_images/ubuntu22.04-cuda.Dockerfile
+-rw-r--r--   0        0        0     3382 2022-11-09 12:37:21.000000 coverage_control-1.2.0/setup_utils/docker/base_images/ubuntu22.04-ros2.Dockerfile
+-rw-r--r--   0        0        0     2576 2022-11-09 12:37:21.000000 coverage_control-1.2.0/setup_utils/docker/base_images/ubuntu22.04.Dockerfile
+-rwxr-xr-x   0        0        0     1436 2022-11-09 12:37:21.000000 coverage_control-1.2.0/setup_utils/docker/create_container.sh
+-rwxr-xr-x   0        0        0       70 2022-11-09 12:37:21.000000 coverage_control-1.2.0/setup_utils/docker/entrypoint.sh
+-rw-r--r--   0        0        0      198 2022-11-09 12:37:21.000000 coverage_control-1.2.0/setup_utils/helpers.sh
+-rwxr-xr-x   0        0        0    10447 2022-11-09 12:37:21.000000 coverage_control-1.2.0/setup_utils/install_dependencies.sh
+-rwxr-xr-x   0        0        0      911 2022-11-09 12:37:21.000000 coverage_control-1.2.0/setup_utils/install_libtorch.sh
+-rwxr-xr-x   0        0        0      633 2022-11-09 12:37:21.000000 coverage_control-1.2.0/setup_utils/manylinux_2_28_before-all.sh
+-rw-r--r--   0        0        0     1659 2022-11-09 12:37:21.000000 coverage_control-1.2.0/setup_utils/noxfile.py
+-rw-r--r--   0        0        0      312 2022-11-09 12:37:21.000000 coverage_control-1.2.0/setup_utils/requirements.txt
+-rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 coverage_control-1.2.0/setup_utils/requirements_cpu.txt
+-rw-r--r--   0        0        0    45430 2022-11-09 12:37:21.000000 coverage_control-1.2.0/PKG-INFO
```

### Comparing `coverage_control-1.1.0/.github/CONTRIBUTING.md` & `coverage_control-1.2.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/.github/docker-base-action/action.yml` & `coverage_control-1.2.0/.github/docker-base-action/action.yml`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/.github/matchers/pylint.json` & `coverage_control-1.2.0/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/.github/workflows/cd_wheels.yml` & `coverage_control-1.2.0/.github/workflows/cd.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-name: wheels
-
+name: docker-deploy
 on:
   workflow_dispatch:
   release:
-    types:
-      - published
+    types: [published]
 
 env:
   FORCE_COLOR: 3
 
 jobs:
   make_sdist:
     name: Make SDist
@@ -68,7 +66,41 @@
           merge-multiple: true
 
       - uses: pypa/gh-action-pypi-publish@release/v1
         # with:
           # Remember to tell (test-)pypi about this repo before publishing
           # Remove this line to publish to PyPI
           # repository-url: https://test.pypi.org/legacy/
+  docker-deploy:
+    permissions: write-all
+    runs-on: ubuntu-latest
+    steps:
+      - name: Checkout
+        uses: actions/checkout@v4
+      - name: Free Disk Space (Ubuntu)
+        uses: jlumbroso/free-disk-space@v1.3.1
+      - name: 'CI docker base'
+        uses: ./.github/docker-base-action
+        with:
+          base_tag: pytorch2.2.2-cuda12.2.2-ros2humble
+          github_token: ${{ secrets.GITHUB_TOKEN }}
+      - name: cleanup
+        run: docker system prune -a -f
+      - name: 'CI docker base'
+        uses: ./.github/docker-base-action
+        with:
+          base_tag: pytorch2.2.2-ros2humble
+          github_token: ${{ secrets.GITHUB_TOKEN }}
+      - name: cleanup
+        run: docker system prune -a -f
+      - name: 'CI docker base'
+        uses: ./.github/docker-base-action
+        with:
+          base_tag: pytorch2.2.2-cuda12.2.2
+          github_token: ${{ secrets.GITHUB_TOKEN }}
+      - name: cleanup
+        run: docker system prune -a -f
+      - name: 'CI docker base'
+        uses: ./.github/docker-base-action
+        with:
+          base_tag: pytorch2.2.2
+          github_token: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `coverage_control-1.1.0/.github/workflows/ghaction-doxygen-ghpages.yml` & `coverage_control-1.2.0/.github/workflows/ghaction-doxygen-ghpages.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 name: doxygen-ghpages
 on:
   workflow_dispatch:
   release:
     types: [published]
-  push:
-    paths:
-      - 'doc/**'
 permissions:
   contents: write
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
```

### Comparing `coverage_control-1.1.0/.gitignore` & `coverage_control-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/.pre-commit-config.yaml` & `coverage_control-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/CMakeLists.txt` & `coverage_control-1.2.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/LICENSE` & `coverage_control-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/README.md` & `coverage_control-1.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 See full documentation at [https://KumarRobotics.github.io/CoverageControl/](https://KumarRobotics.github.io/CoverageControl/)
 
 ## Introduction
 
 Coverage control is the problem of navigating a robot swarm to collaboratively monitor features or a phenomenon of interest not known _a priori_.
 The library provides a simulation environment, algorithms, and GNN-based architectures for the coverage control problem.  
-<img align="right" width="300" src="https://github.com/KumarRobotics/CoverageControl/raw/main/doc/graphics/LPAC.gif">
+<img align="right" width="300" src="https://kumarrobotics.github.io/CoverageControl/LPAC.gif">
 
 **Key features:**  
 - The core library is written in `C++` and `CUDA` to handle large-scale simulations
 - There are `python` bindings that interface with the core library
 - Several Centroidal Voronoi Tessellation (CVT)-based algorithms (aka Lloyd's algorithms)
 - Learnable Perception-Action-Communication (LPAC) architecture for the coverage control problem is implemented in `PyTorch` and `PyTorch Geometric`
-- GPU and CPU parallelization using `CUDA` and `OpenMP`
 
 ---
-## Quick Start
+## Getting Started
 The library is available as a `pip` package. To install the package, run the following command:
 ```bash
 pip install coverage_control
 ```
 
 See [Installation](https://kumarrobotics.github.io/CoverageControl/installation.html) for more details on installation.
```

### Comparing `coverage_control-1.1.0/cppsrc/core/CMakeLists.txt` & `coverage_control-1.2.0/cppsrc/core/CMakeLists.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,179 +1,191 @@
 cmake_minimum_required(VERSION 3.16)
 
-include(FetchContent)
-FetchContent_Declare(CMakeExtraUtils
-        GIT_REPOSITORY https://github.com/LecrisUT/CMakeExtraUtils
-        GIT_TAG v0.4.1)
-FetchContent_MakeAvailable(CMakeExtraUtils)
-
-include(DynamicVersion)
-dynamic_version(PROJECT_PREFIX "CoverageControl_" GIT_ARCHIVAL_FILE "${CMAKE_CURRENT_SOURCE_DIR}/../../.git_archival.txt"
-  FALLBACK_VERSION 0.0.1)
+if(DEFINED SKBUILD_PROJECT_VERSION)
+  set(PROJECT_VERSION ${SKBUILD_PROJECT_VERSION})
+else()
+  include(FetchContent)
+  FetchContent_Declare(CMakeExtraUtils
+    GIT_REPOSITORY https://github.com/LecrisUT/CMakeExtraUtils
+    GIT_TAG v0.4.1)
+  FetchContent_MakeAvailable(CMakeExtraUtils)
+
+  include(DynamicVersion)
+  dynamic_version(
+    PROJECT_PREFIX "CoverageControl_"
+    GIT_ARCHIVAL_FILE "${CMAKE_CURRENT_SOURCE_DIR}/../../.git_archival.txt"
+    FALLBACK_VERSION 0.0.1
+  )
+endif()
 
 project(CoverageControl VERSION ${PROJECT_VERSION} LANGUAGES CXX)
 
 if(NOT CMAKE_BUILD_TYPE)
-	set(CMAKE_BUILD_TYPE Release)
+  set(CMAKE_BUILD_TYPE Release)
 endif()
 
 option(COVERAGECONTROL_WITH_CUDA "Enable CUDA support" ON)
 
-if (COVERAGECONTROL_WITH_CUDA)
-	cmake_minimum_required(VERSION 3.24)
-	include(CheckLanguage)
-	check_language(CUDA)
-	if(NOT CMAKE_CUDA_COMPILER)
-		message(WARNING "No CUDA compiler found, disabling CUDA support")
-		set(COVERAGECONTROL_WITH_CUDA OFF)
-	else()
-		enable_language(CUDA)
-	endif()
+if(COVERAGECONTROL_WITH_CUDA)
+  cmake_minimum_required(VERSION 3.24)
+  include(CheckLanguage)
+  check_language(CUDA)
+  if(NOT CMAKE_CUDA_COMPILER)
+    message(WARNING "No CUDA compiler found, disabling CUDA support")
+    set(COVERAGECONTROL_WITH_CUDA OFF)
+  else()
+    enable_language(CUDA)
+  endif()
 endif()
 
 set(CMAKE_CXX_STANDARD 17)
 set(CMAKE_CXX_STANDARD_REQUIRED True)
 set(CMAKE_COLOR_DIAGNOSTICS ON)
 
 include(CheckCXXCompilerFlag)
 include(GNUInstallDirs)
 
-if (NOT CMAKE_LIBRARY_OUTPUT_DIRECTORY)
-	if(UNIX)
-		set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_INSTALL_LIBDIR})
-	else()
-		set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_INSTALL_BINDIR})
-	endif()
-endif()
-if (NOT CMAKE_ARCHIVE_OUTPUT_DIRECTORY)
-	if(UNIX)
-		set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_INSTALL_LIBDIR})
-	else()
-		set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_INSTALL_BINDIR})
-	endif()
-endif()
-if (NOT CMAKE_RUNTIME_OUTPUT_DIRECTORY)
-	set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_INSTALL_BINDIR})
+if(NOT CMAKE_LIBRARY_OUTPUT_DIRECTORY)
+  if(UNIX)
+    set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_INSTALL_LIBDIR})
+  else()
+    set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_INSTALL_BINDIR})
+  endif()
+endif()
+if(NOT CMAKE_ARCHIVE_OUTPUT_DIRECTORY)
+  if(UNIX)
+    set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_INSTALL_LIBDIR})
+  else()
+    set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_INSTALL_BINDIR})
+  endif()
+endif()
+if(NOT CMAKE_RUNTIME_OUTPUT_DIRECTORY)
+  set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_INSTALL_BINDIR})
 endif()
-if (NOT CMAKE_INCLUDE_OUTPUT_DIRECTORY)
-	set(CMAKE_INCLUDE_OUTPUT_DIRECTORY ${CMAKE_INSTALL_INCLUDEDIR})
+if(NOT CMAKE_INCLUDE_OUTPUT_DIRECTORY)
+  set(CMAKE_INCLUDE_OUTPUT_DIRECTORY ${CMAKE_INSTALL_INCLUDEDIR})
 endif()
 
-set(CMAKEPACKAGE_INSTALL_DIR "${CMAKE_LIBRARY_OUTPUT_DIRECTORY}/cmake/${PROJECT_NAME}")
+set(CMAKEPACKAGE_INSTALL_DIR
+  "${CMAKE_LIBRARY_OUTPUT_DIRECTORY}/cmake/${PROJECT_NAME}"
+)
 
 
 find_package(OpenMP REQUIRED)
 
 ###########################
 #### Eigen3 dependency ####
 ###########################
 find_package(Eigen3 3.4 QUIET)
-if (NOT Eigen3_FOUND OR Eigen3_VERSION VERSION_LESS 3.4)
-	message(STATUS "Eigen3 3.4 not found, fetching it")
-	include(FetchContent)
-	FetchContent_Declare(Eigen3
-		URL https://gitlab.com/libeigen/eigen/-/archive/3.4.0/eigen-3.4.0.tar.gz
-	)
-	set(FETCHCONTENT_QUIET FALSE) # show progress dialog
-	FetchContent_Populate(Eigen3)   # finish fetching and unpacking before continuing
-	add_subdirectory(${FETCHCONTENT_BASE_DIR}/eigen3-src ${CMAKE_CURRENT_BINARY_DIR}/eigen3)
+if(NOT Eigen3_FOUND OR Eigen3_VERSION VERSION_LESS 3.4)
+  message(STATUS "Eigen3 3.4 not found, fetching it")
+  include(FetchContent)
+  FetchContent_Declare(Eigen3
+    URL https://gitlab.com/libeigen/eigen/-/archive/3.4.0/eigen-3.4.0.tar.gz
+  )
+  set(FETCHCONTENT_QUIET FALSE) # show progress dialog
+  FetchContent_Populate(Eigen3)   # finish fetching and unpacking before continuing
+  add_subdirectory(${FETCHCONTENT_BASE_DIR}/eigen3-src ${CMAKE_CURRENT_BINARY_DIR}/eigen3)
 endif()
 
 ###########################
 #### CGAL dependency ####
 ###########################
 find_package(CGAL 5.6.1 QUIET)
-if (NOT CGAL_FOUND OR CGAL_VERSION VERSION_LESS 5.6.1)
-	message(STATUS "CGAL 5.6.1 not found, fetching it")
-	include(FetchContent)
-	FetchContent_Declare(CGAL
-		URL https://github.com/CGAL/cgal/releases/download/v5.6.1/CGAL-5.6.1.tar.xz
-		URL_HASH SHA256=cdb15e7ee31e0663589d3107a79988a37b7b1719df3d24f2058545d1bcdd5837
-	)
-	set(FETCHCONTENT_QUIET FALSE) # show progress dialog
-	FetchContent_Populate(CGAL)   # finish fetching and unpacking before continuing
-	set(CGAL_DIR "${FETCHCONTENT_BASE_DIR}/cgal-src")
-	find_package(CGAL 5.6 REQUIRED)
+if(NOT CGAL_FOUND OR CGAL_VERSION VERSION_LESS 5.6.1)
+  message(STATUS "CGAL 5.6.1 not found, fetching it")
+  include(FetchContent)
+  FetchContent_Declare(CGAL
+    URL https://github.com/CGAL/cgal/releases/download/v5.6.1/CGAL-5.6.1.tar.xz
+    URL_HASH SHA256=cdb15e7ee31e0663589d3107a79988a37b7b1719df3d24f2058545d1bcdd5837
+  )
+  set(FETCHCONTENT_QUIET FALSE) # show progress dialog
+  FetchContent_Populate(CGAL)   # finish fetching and unpacking before continuing
+  set(CGAL_DIR "${FETCHCONTENT_BASE_DIR}/cgal-src")
+  find_package(CGAL 5.6 REQUIRED)
 endif()
 ###########################
 
 set(Boost_USE_STATIC_LIBS ON)
 find_package(Boost REQUIRED COMPONENTS iostreams)
 
-configure_file(${CMAKE_CURRENT_SOURCE_DIR}/cmake/${PROJECT_NAME}Config.h.in ${PROJECT_NAME}/Config.h)
+configure_file(
+  ${CMAKE_CURRENT_SOURCE_DIR}/cmake/${PROJECT_NAME}Config.h.in
+  ${PROJECT_NAME}/Config.h
+)
 
 add_library(compiler_flags INTERFACE)
 target_compile_features(compiler_flags INTERFACE cxx_std_17)
 
 set(gcc_like_cxx "$<COMPILE_LANG_AND_ID:CXX,ARMClang,AppleClang,Clang,GNU,LCC>")
 set(msvc_cxx "$<COMPILE_LANG_AND_ID:CXX,MSVC>")
 target_compile_options(compiler_flags INTERFACE
-	"$<${gcc_like_cxx}:$<BUILD_INTERFACE:-Wall;-Wextra;-Wshadow;-Wformat=2;-Wunused;-pedantic>>"
-	"$<${msvc_cxx}:$<BUILD_INTERFACE:-W3>>"
+  "$<${gcc_like_cxx}:$<BUILD_INTERFACE:-Wall;-Wextra;-Wshadow;-Wformat=2;-Wunused;-pedantic>>"
+  "$<${msvc_cxx}:$<BUILD_INTERFACE:-W3>>"
 )
 #################################
 ## CoverageControl library ##
 #################################
 
 set(sources_list
-	polygon_utils.cpp
-	parameters.cpp
-	voronoi.cpp
+  polygon_utils.cpp
+  parameters.cpp
+  voronoi.cpp
   world_idf.cpp
-	coverage_system.cpp
-	plotter.cpp
-	cuda_utils.cpp
-	extern/Hungarian.cpp)
-
-if (COVERAGECONTROL_WITH_CUDA)
-	list(APPEND sources_list
-		cuda/generate_world_map.cu
-		cuda/cuda_utils.cu)
+  coverage_system.cpp
+  plotter.cpp
+  cuda_utils.cpp
+  extern/Hungarian.cpp)
+
+if(COVERAGECONTROL_WITH_CUDA)
+  list(APPEND sources_list
+    cuda/generate_world_map.cu
+    cuda/cuda_utils.cu)
 endif()
 list(TRANSFORM sources_list PREPEND "${CMAKE_CURRENT_SOURCE_DIR}/src/")
 
 set(dependencies_list Eigen3::Eigen OpenMP::OpenMP_CXX)
 
 add_library(${PROJECT_NAME} SHARED ${sources_list})
 target_include_directories(${PROJECT_NAME} PRIVATE "${PROJECT_BINARY_DIR}")
 target_include_directories(${PROJECT_NAME} PRIVATE "${CMAKE_INSTALL_INCLUDEDIR}")
 target_include_directories(${PROJECT_NAME} PRIVATE "${CMAKE_CURRENT_SOURCE_DIR}/include")
 target_link_libraries(${PROJECT_NAME} PRIVATE compiler_flags CGAL::CGAL Boost::boost Boost::iostreams)
 target_link_libraries(${PROJECT_NAME} PUBLIC ${dependencies_list})
 set_target_properties(${PROJECT_NAME} PROPERTIES INSTALL_RPATH "${CMAKE_LIBRARY_OUTPUT_DIRECTORY}")
 
-if (COVERAGECONTROL_WITH_CUDA)
-	set_target_properties(${PROJECT_NAME} PROPERTIES CUDA_ARCHITECTURES all POSITION_INDEPENDENT_CODE ON)
+if(COVERAGECONTROL_WITH_CUDA)
+  set_target_properties(${PROJECT_NAME} PROPERTIES CUDA_ARCHITECTURES all POSITION_INDEPENDENT_CODE ON)
 else()
-	set_target_properties(${PROJECT_NAME} PROPERTIES POSITION_INDEPENDENT_CODE ON)
+  set_target_properties(${PROJECT_NAME} PROPERTIES POSITION_INDEPENDENT_CODE ON)
 endif()
 
 target_include_directories(${PROJECT_NAME} INTERFACE
-	"$<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>"
-	"$<INSTALL_INTERFACE:${CMAKE_INCLUDE_OUTPUT_DIRECTORY}>")
+  "$<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>"
+  "$<INSTALL_INTERFACE:${CMAKE_INCLUDE_OUTPUT_DIRECTORY}>")
 
 install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/include/ DESTINATION ${CMAKE_INCLUDE_OUTPUT_DIRECTORY})
 install(TARGETS ${PROJECT_NAME} EXPORT ${PROJECT_NAME}Targets LIBRARY DESTINATION ${CMAKE_LIBRARY_OUTPUT_DIRECTORY} ARCHIVE DESTINATION ${CMAKE_ARCHIVE_OUTPUT_DIRECTORY})
 install(FILES "${PROJECT_BINARY_DIR}/${PROJECT_NAME}/Config.h" DESTINATION ${CMAKE_INCLUDE_OUTPUT_DIRECTORY}/${PROJECT_NAME})
 
 include(CMakePackageConfigHelpers)
 # generate the config file that includes the exports
 configure_package_config_file(${CMAKE_CURRENT_SOURCE_DIR}/cmake/${PROJECT_NAME}Config.cmake.in
-	"${CMAKE_CURRENT_BINARY_DIR}/${PROJECT_NAME}Config.cmake"
-	INSTALL_DESTINATION "${CMAKEPACKAGE_INSTALL_DIR}")
+  "${CMAKE_CURRENT_BINARY_DIR}/${PROJECT_NAME}Config.cmake"
+  INSTALL_DESTINATION "${CMAKEPACKAGE_INSTALL_DIR}")
 
 write_basic_package_version_file(
-	"${CMAKE_CURRENT_BINARY_DIR}/${PROJECT_NAME}ConfigVersion.cmake"
-	VERSION "${${PROJECT_NAME}_VERSION_MAJOR}.${${PROJECT_NAME}_VERSION_MINOR}.${${PROJECT_NAME}_VERSION_PATCH}"
-	COMPATIBILITY AnyNewerVersion)
+  "${CMAKE_CURRENT_BINARY_DIR}/${PROJECT_NAME}ConfigVersion.cmake"
+  VERSION "${${PROJECT_NAME}_VERSION_MAJOR}.${${PROJECT_NAME}_VERSION_MINOR}.${${PROJECT_NAME}_VERSION_PATCH}"
+  COMPATIBILITY AnyNewerVersion)
 
-export (PACKAGE ${PROJECT_NAME})
+export(PACKAGE ${PROJECT_NAME})
 
 install(FILES
-	${CMAKE_CURRENT_BINARY_DIR}/${PROJECT_NAME}Config.cmake
-	${CMAKE_CURRENT_BINARY_DIR}/${PROJECT_NAME}ConfigVersion.cmake
-	DESTINATION ${CMAKEPACKAGE_INSTALL_DIR})
+  ${CMAKE_CURRENT_BINARY_DIR}/${PROJECT_NAME}Config.cmake
+  ${CMAKE_CURRENT_BINARY_DIR}/${PROJECT_NAME}ConfigVersion.cmake
+  DESTINATION ${CMAKEPACKAGE_INSTALL_DIR})
 
 install(EXPORT ${PROJECT_NAME}Targets
-	FILE ${PROJECT_NAME}Targets.cmake
-	NAMESPACE CoverageControl::
-	DESTINATION ${CMAKEPACKAGE_INSTALL_DIR})
+  FILE ${PROJECT_NAME}Targets.cmake
+  NAMESPACE CoverageControl::
+  DESTINATION ${CMAKEPACKAGE_INSTALL_DIR})
```

### Comparing `coverage_control-1.1.0/cppsrc/core/cmake/CoverageControlConfig.cmake.in` & `coverage_control-1.2.0/cppsrc/core/cmake/CoverageControlConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/abstract_controller.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/algorithms/abstract_controller.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/centralized_cvt.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/algorithms/centralized_cvt.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/clairvoyant_cvt.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/algorithms/clairvoyant_cvt.h`

 * *Files 11% similar despite different names*

```diff
@@ -89,15 +89,17 @@
   PointVector GetActions() { return actions_; }
 
   auto GetGoals() { return goals_; }
 
   auto &GetVoronoi() { return voronoi_; }
 
   void ComputeGoals() {
-    voronoi_.UpdateSites(robot_global_positions_);
+    voronoi_ = Voronoi(robot_global_positions_, env_.GetWorldMap(),
+                       Point2(params_.pWorldMapSize, params_.pWorldMapSize),
+                       params_.pResolution);
     auto voronoi_cells = voronoi_.GetVoronoiCells();
     for (size_t iRobot = 0; iRobot < num_robots_; ++iRobot) {
       goals_[iRobot] = voronoi_cells[iRobot].centroid();
       voronoi_mass_[iRobot] = voronoi_cells[iRobot].mass();
     }
   }
```

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/decentralized_cvt.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/algorithms/decentralized_cvt.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/near_optimal_cvt.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/algorithms/near_optimal_cvt.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/near_optimal_cvt_algorithm.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/algorithms/near_optimal_cvt_algorithm.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/oracle_bang_explore_exploit.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/algorithms/oracle_bang_explore_exploit.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/oracle_explore_exploit.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/algorithms/oracle_explore_exploit.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/simul_explore_exploit.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/algorithms/simul_explore_exploit.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/bivariate_normal_distribution.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/bivariate_normal_distribution.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/cgal/config.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/cgal/config.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/cgal/polygon_utils.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/cgal/polygon_utils.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/cgal/utilities.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/cgal/utilities.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/constants.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/constants.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/coverage_system.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/coverage_system.h`

 * *Files 2% similar despite different names*

```diff
@@ -327,14 +327,17 @@
   //! Add noise to the given point and ensure within bounds
   Point2 AddNoise(Point2 const pt) const;
 
   //! Check if the robot is oscillating about its current position
   //! \warning This function is dependent on the size of the robot positions
   //! history
   bool CheckOscillation(size_t const robot_id) const {
+    if (params_.pCheckOscillations == false) {
+      return false;
+    }
     if (robot_positions_history_[robot_id].size() < 2) {
       return false;
     }
     auto const &history = robot_positions_history_[robot_id];
     Point2 const last_pos = history.back();
     auto it_end = std::next(history.crbegin(),
                             std::max(6, static_cast<int>(history.size()) - 1));
@@ -381,14 +384,26 @@
    * Step all robots towards given goals
    *
    * \param goals Vector of goals for the robots
    * \param actions Vector of actions for the robots
    * \return True if any robot is still moving
    */
   bool StepRobotsToGoals(PointVector const &goals, PointVector &actions);
+
+  void ClearRobotMaps() {
+    for (size_t i = 0; i < num_robots_; ++i) {
+      robots_[i].ClearRobotMap();
+    }
+  }
+
+  void ClearExploredIDF() {
+    explored_idf_map_ =
+        MapType::Constant(params_.pWorldMapSize, params_.pWorldMapSize, 0);
+  }
+
   //! @}
 
   //! \name I/O
   //! @{
   int WriteRobotPositions(std::string const &file_name) const;
   int WriteRobotPositions(std::string const &file_name,
                           PointVector const &positions) const;
```

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/cuda/geometry_utils.cuh` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/cuda/geometry_utils.cuh`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/cuda_utils.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/cuda_utils.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/cuda_helpers/helper_cuda.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/extern/cuda_helpers/helper_cuda.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/cuda_helpers/helper_string.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/extern/cuda_helpers/helper_string.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/gnuplot/gnuplot-iostream.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/extern/gnuplot/gnuplot-iostream.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/json/json.hpp` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/extern/json/json.hpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/lsap/Hungarian.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/extern/lsap/Hungarian.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/lsap/LICENSE` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/extern/lsap/LICENSE`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/lsap/README.txt` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/extern/lsap/README.txt`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/tomlplusplus/toml.hpp` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/extern/tomlplusplus/toml.hpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/generate_world_map.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/generate_world_map.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/geographiclib_wrapper.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/geographiclib_wrapper.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/map_utils.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/map_utils.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/parameters.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/parameters.h`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,23 @@
    */
   int pNumRobots = 32;    //!< Number of robots
   int pNumFeatures = 32;  //!< Number of features
   int pNumPolygons = 0;   //!< Number of polygonal features
   int pMaxVertices = 10;  //!< Maximum number of vertices in a polygon
   double pPolygonRadius = 64;
 
+  /*! \name IO Parameters
+   * @{
+   */
+  //! Determines the quality of the plot and videos
+  //! > 1: High quality (takes more time to plot)
+  //! < 1: Low quality (takes less time to plot)
+  double pPlotScale = 1.0;
+  /*! @} */
+
   /*! \name Map Parameters
    * @{
    */
   //! Assuming same resolution in both the directions in meters. Pixel area =
   //! pResolution^2
   double pResolution = 1.0;
 
@@ -140,14 +149,15 @@
   /*! @} */
 
   /*! \name Algorithm Parameters
    * @{
    */
 
   int pEpisodeSteps = 2000;  // Total time is pEpisodeSteps * pTimeStep
+  bool pCheckOscillations = true;
 
   /*! \name Global-CVT
    * @{
    */
   int pLloydMaxIterations = 100;
   int pLloydNumTries = 10;
   /*! @} */
```

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/plotter.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/plotter.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/robot_model.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/robot_model.h`

 * *Files 2% similar despite different names*

```diff
@@ -133,50 +133,55 @@
     world_idf_ = std::make_shared<const WorldIDF>(world_idf);
     normalization_factor_ = world_idf_->GetNormalizationFactor();
     global_current_position_ = global_start_position_;
 
     sensor_view_ = MapType::Zero(params_.pSensorSize, params_.pSensorSize);
     local_map_ = MapType::Zero(params_.pLocalMapSize, params_.pLocalMapSize);
     obstacle_map_ = MapType::Zero(params_.pLocalMapSize, params_.pLocalMapSize);
-    if (params_.pRobotMapUseUnknownImportance == true) {
-      robot_map_ =
-          MapType::Constant(params_.pRobotMapSize, params_.pRobotMapSize,
-                            params_.pUnknownImportance * params_.pNorm);
-    } else {
-      robot_map_ = MapType::Zero(params_.pRobotMapSize, params_.pRobotMapSize);
-    }
 
     local_start_position_ = Point2{0, 0};
     local_current_position_ = local_start_position_;
 
+    ClearRobotMap();
+
     if (params_.pUpdateExplorationMap == true) {
       exploration_map_ =
           MapType::Constant(params_.pRobotMapSize, params_.pRobotMapSize, 1);
       local_exploration_map_ =
           MapType::Constant(params_.pRobotMapSize, params_.pRobotMapSize, 1);
       UpdateExplorationMap();
     } else {
       exploration_map_ =
           MapType::Constant(params_.pRobotMapSize, params_.pRobotMapSize, 0);
       local_exploration_map_ =
           MapType::Constant(params_.pRobotMapSize, params_.pRobotMapSize, 0);
     }
 
+    time_step_dist_ =
+        params_.pMaxRobotSpeed * params_.pTimeStep * params_.pResolution;
+    sensor_area_ = params_.pSensorSize * params_.pSensorSize;
+  }
+
+  void ClearRobotMap() {
+    if (params_.pRobotMapUseUnknownImportance == true) {
+      robot_map_ =
+          MapType::Constant(params_.pRobotMapSize, params_.pRobotMapSize,
+                            params_.pUnknownImportance * params_.pNorm);
+    } else {
+      robot_map_ = MapType::Zero(params_.pRobotMapSize, params_.pRobotMapSize);
+    }
+
     if (params_.pUpdateSensorView == true) {
       UpdateSensorView();
     }
     if (params_.pUpdateRobotMap == false) {
       robot_map_ = world_idf_->GetWorldMap();
     } else {
       UpdateRobotMap();
     }
-
-    time_step_dist_ =
-        params_.pMaxRobotSpeed * params_.pTimeStep * params_.pResolution;
-    sensor_area_ = params_.pSensorSize * params_.pSensorSize;
   }
 
   //! \note Time step robot with the given control direction and speed.
   //! \note Direction cannot be zero-vector is speed is not zero.
   //! \note Speed needs to be positive
   int StepControl(Point2 const &direction, double const &speed) {
     auto dir = direction;
```

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/typedefs.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/typedefs.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/vec2d.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/vec2d.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/voronoi.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/voronoi.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/world_idf.h` & `coverage_control-1.2.0/cppsrc/core/include/CoverageControl/world_idf.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/src/coverage_system.cpp` & `coverage_control-1.2.0/cppsrc/core/src/coverage_system.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -376,19 +376,19 @@
 
 void CoverageSystem::RenderRecordedMap(std::string const &dir_name,
                                        std::string const &video_name) const {
   std::string frame_dir = dir_name + "/frames/";
   std::filesystem::create_directory(frame_dir);
   Plotter plotter(frame_dir, params_.pWorldMapSize * params_.pResolution,
                   params_.pResolution);
-  plotter.SetScale(2);
+  plotter.SetScale(params_.pPlotScale);
   Plotter plotter_voronoi(frame_dir,
                           params_.pWorldMapSize * params_.pResolution,
                           params_.pResolution);
-  plotter_voronoi.SetScale(2);
+  plotter_voronoi.SetScale(params_.pPlotScale);
 #pragma omp parallel for
   for (size_t i = 0; i < plotter_data_.size(); ++i) {
     auto iPlotter = plotter;
     iPlotter.SetPlotName("map", i);
     /* iPlotter.PlotMap(plotter_data_[i].map, plotter_data_[i].positions,
      * plotter_data_[i].positions_history, plotter_data_[i].robot_status); */
     iPlotter.PlotMap(plotter_data_[i].map, plotter_data_[i].positions,
@@ -446,86 +446,86 @@
   plotter_data_.push_back(data);
 }
 
 void CoverageSystem::PlotSystemMap(std::string const &filename) const {
   std::vector<int> robot_status(num_robots_, 0);
   Plotter plotter("./", params_.pWorldMapSize * params_.pResolution,
                   params_.pResolution);
-  plotter.SetScale(2);
+  plotter.SetScale(params_.pPlotScale);
   plotter.SetPlotName(filename);
   plotter.PlotMap(system_map_, robot_global_positions_,
                   robot_positions_history_, robot_status,
                   params_.pCommunicationRange);
 }
 
 void CoverageSystem::PlotSystemMap(std::string const &dir_name, int const &step,
                                    std::vector<int> const &robot_status) const {
   Plotter plotter(dir_name, params_.pWorldMapSize * params_.pResolution,
                   params_.pResolution);
-  plotter.SetScale(1);
+  plotter.SetScale(params_.pPlotScale);
   plotter.SetPlotName("map", step);
   plotter.PlotMap(system_map_, robot_global_positions_,
                   robot_positions_history_, robot_status);
 }
 
 void CoverageSystem::PlotWorldMapRobots(std::string const &dir_name,
                                         std::string const &map_name) const {
   Plotter plotter(dir_name, params_.pWorldMapSize * params_.pResolution,
                   params_.pResolution);
-  plotter.SetScale(1);
+  plotter.SetScale(params_.pPlotScale);
   plotter.SetPlotName(map_name);
   std::vector<int> robot_status(num_robots_, 0);
   plotter.PlotMap(GetWorldMap(), robot_global_positions_,
                   robot_positions_history_, robot_status);
 }
 
 void CoverageSystem::PlotWorldMap(std::string const &dir_name,
                                   std::string const &map_name) const {
   Plotter plotter(dir_name, params_.pWorldMapSize * params_.pResolution,
                   params_.pResolution);
-  plotter.SetScale(1);
+  plotter.SetScale(params_.pPlotScale);
   plotter.SetPlotName(map_name);
   plotter.PlotMap(GetWorldMap());
 }
 
 void CoverageSystem::PlotInitMap(std::string const &dir_name,
                                  std::string const &map_name) const {
   Plotter plotter(dir_name, params_.pWorldMapSize * params_.pResolution,
                   params_.pResolution);
-  plotter.SetScale(2);
+  plotter.SetScale(params_.pPlotScale);
   plotter.SetPlotName(map_name);
   plotter.PlotMap(GetWorldMap(), robot_global_positions_);
 }
 
 void CoverageSystem::PlotMapVoronoi(std::string const &dir_name,
                                     int const &step) {
   ComputeVoronoiCells();
   Plotter plotter(dir_name, params_.pWorldMapSize * params_.pResolution,
                   params_.pResolution);
-  plotter.SetScale(2);
+  plotter.SetScale(params_.pPlotScale);
   plotter.SetPlotName("voronoi_map", step);
   plotter.PlotMap(GetWorldMap(), robot_global_positions_, voronoi_,
                   robot_positions_history_);
 }
 
 void CoverageSystem::PlotMapVoronoi(std::string const &dir_name,
                                     int const &step, Voronoi const &voronoi,
                                     PointVector const &goals) const {
   Plotter plotter(dir_name, params_.pWorldMapSize * params_.pResolution,
                   params_.pResolution);
-  plotter.SetScale(2);
+  plotter.SetScale(params_.pPlotScale);
   plotter.SetPlotName("map", step);
   plotter.PlotMap(GetWorldMap(), robot_global_positions_, goals, voronoi);
 }
 
 void CoverageSystem::PlotFrontiers(std::string const &dir_name, int const &step,
                                    PointVector const &frontiers) const {
   Plotter plotter(dir_name, params_.pWorldMapSize * params_.pResolution,
                   params_.pResolution);
-  plotter.SetScale(2);
+  plotter.SetScale(params_.pPlotScale);
   plotter.SetPlotName("map", step);
   plotter.PlotMap(system_map_, robot_global_positions_,
                   robot_positions_history_, frontiers);
 }
 
 void CoverageSystem::PlotRobotSystemMap(std::string const &dir_name,
                                         int const &robot_id, int const &step) {
@@ -540,15 +540,15 @@
   plotter.PlotMap(GetRobotSystemMap(robot_id), neighbours_positions);
 }
 
 void CoverageSystem::PlotRobotIDFMap(std::string const &dir_name,
                                      int const &robot_id, int const &step) {
   Plotter plotter(dir_name, params_.pLocalMapSize * params_.pResolution,
                   params_.pResolution);
-  plotter.SetScale(4);
+  plotter.SetScale(params_.pPlotScale);
   plotter.SetPlotName("robot_" + std::to_string(robot_id) + "_", step);
   plotter.PlotMap(GetRobotLocalMap(robot_id));
 }
 
 void CoverageSystem::PlotRobotExplorationMap(std::string const &dir_name,
                                              int const &robot_id,
                                              int const &step) {
```

### Comparing `coverage_control-1.1.0/cppsrc/core/src/cuda/cuda_utils.cu` & `coverage_control-1.2.0/cppsrc/core/src/cuda/cuda_utils.cu`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/src/cuda/generate_world_map.cu` & `coverage_control-1.2.0/cppsrc/core/src/cuda/generate_world_map.cu`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/src/cuda_utils.cpp` & `coverage_control-1.2.0/cppsrc/core/src/cuda_utils.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/src/extern/Hungarian.cpp` & `coverage_control-1.2.0/cppsrc/core/src/extern/Hungarian.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/src/parameters.cpp` & `coverage_control-1.2.0/cppsrc/core/src/parameters.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,21 @@
 
   if (toml_config["PolygonRadius"].value<double>()) {
     pPolygonRadius = toml_config["PolygonRadius"].value<double>().value();
   } else {
     std::cout << "PolygonRadius (default): " << pPolygonRadius << std::endl;
   }
 
+  auto toml_IO = toml_config["IO"];
+  if (toml_IO["PlotScale"].value<double>()) {
+    pPlotScale = toml_IO["PlotScale"].value<double>().value();
+  } else {
+    std::cout << "PlotScale (default): " << pPlotScale << std::endl;
+  }
+
   auto toml_EnvironmentMaps = toml_config["Environment.Maps"];
 
   if (toml_EnvironmentMaps) {
     auto toml_Resolution = toml_EnvironmentMaps["Resolution"].value<double>();
     auto toml_WorldMapSize = toml_EnvironmentMaps["WorldMapSize"].value<int>();
     auto toml_RobotMapSize = toml_EnvironmentMaps["RobotMapSize"].value<int>();
     auto toml_LocalMapSize = toml_EnvironmentMaps["LocalMapSize"].value<int>();
@@ -222,14 +229,18 @@
   auto toml_Algorithm = toml_config["Algorithm"];
 
   if (toml_Algorithm) {
     auto toml_EpisodeSteps = toml_Algorithm["EpisodeSteps"].value<int>();
     if (toml_EpisodeSteps) {
       pEpisodeSteps = toml_EpisodeSteps.value();
     }
+    if (toml_Algorithm["CheckOscillations"].value<bool>()) {
+      pCheckOscillations =
+          toml_Algorithm["CheckOscillations"].value<bool>().value();
+    }
 
     auto toml_LloydMaxIterations =
         toml_Algorithm["Global-CVT.LloydMaxIterations"].value<int>();
     auto toml_LloydNumTries =
         toml_Algorithm["Global-CVT.LloydNumTries"].value<int>();
     if (toml_LloydMaxIterations) {
       pLloydMaxIterations = toml_LloydMaxIterations.value();
@@ -249,14 +260,16 @@
 void Parameters::PrintParameters() {
   std::cout << "NumRobots: " << pNumRobots << std::endl;
   std::cout << "NumFeatures: " << pNumFeatures << std::endl;
   std::cout << "NumPolygons: " << pNumPolygons << std::endl;
   std::cout << "MaxVertices: " << pMaxVertices << std::endl;
   std::cout << "PolygonRadius" << pPolygonRadius << std::endl;
 
+  std::cout << "PlotScale: " << pPlotScale << std::endl;
+
   std::cout << "Resolution: " << pResolution << std::endl;
   std::cout << "WorldMapSize: " << pWorldMapSize << std::endl;
   std::cout << "RobotMapSize: " << pRobotMapSize << std::endl;
   std::cout << "LocalMapSize: " << pLocalMapSize << std::endl;
 
   std::cout << "UpdateRobotMap: " << pUpdateRobotMap << std::endl;
   std::cout << "UpdateSensorView: " << pUpdateSensorView << std::endl;
@@ -281,12 +294,13 @@
   std::cout << "RobotPosHistorySize: " << pRobotPosHistorySize << std::endl;
   std::cout << "TimeStep: " << pTimeStep << std::endl;
 
   std::cout << "AddNoisePositions: " << pAddNoisePositions << std::endl;
   std::cout << "PositionsNoiseSigma: " << pPositionsNoiseSigma << std::endl;
 
   std::cout << "EpisodeSteps: " << pEpisodeSteps << std::endl;
+  std::cout << "CheckOscillations: " << pCheckOscillations << std::endl;
   std::cout << "LloydMaxIterations: " << pLloydMaxIterations << std::endl;
   std::cout << "LloydNumTries: " << pLloydNumTries << std::endl;
   std::cout << "NumFrontiers: " << pNumFrontiers << std::endl;
 }
 } /* namespace CoverageControl */
```

### Comparing `coverage_control-1.1.0/cppsrc/core/src/plotter.cpp` & `coverage_control-1.2.0/cppsrc/core/src/plotter.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -44,26 +44,27 @@
      << image_sz << "," << image_sz << "\n";
   gp << "set palette defined (-5 'black', -1 '" << color_unknown
      << "', 0 'white', 1 '" << color_idf << "')\n";
   gp << "set cbrange [-5:1]\n";
   gp << "set size ratio -1\n";
   gp << "set xrange [0:" << range_max << "]\n";
   gp << "set yrange [0:" << range_max << "]\n";
+  gp << "set border linewidth 1.5\n";
   if (unset_colorbox) gp << "unset colorbox\n";
   return 0;
 }
 
 void Plotter::StreamMap(Gnuplot &gp, MapType const &map) {
   for (int i = 0; i < map.rows(); ++i) {
     for (int j = 0; j < map.cols(); ++j) {
       gp << map(i, j) << " ";
     }
     gp << "\n";
   }
-  gp << "e\n";
+  gp << "e" << std::endl;
 }
 
 void Plotter::PlotMap(Gnuplot &gp, bool begin) {
   if (begin == true)
     gp << "plot ";
   else
     gp << ", ";
@@ -113,15 +114,15 @@
   gp << "\n";
 
   StreamMap(gp, map);
 
   for (auto const &pos : positions) {
     gp << pos[0] << " " << pos[1] << std::endl;
   }
-  gp << "e\n";
+  gp << "e" << std::endl;
 }
 
 void Plotter::PlotMap(MapType const &map, PointVector const &positions,
                       std::vector<std::list<Point2>> const &trajectories,
                       std::vector<int> const &robot_status) {
   Gnuplot gp;
   if (GnuplotCommands(gp)) {
@@ -147,20 +148,20 @@
   gp << "\n";
 
   StreamMap(gp, map);
   for (auto const &trajectory : trajectories) {
     for (auto const &pos : trajectory) {
       gp << pos[0] << " " << pos[1] << std::endl;
     }
-    gp << "e\n";
+    gp << "e" << std::endl;
   }
 
   for (auto const &pos : positions) {
     gp << pos[0] << " " << pos[1] << std::endl;
-    gp << "e\n";
+    gp << "e" << std::endl;
   }
 }
 
 void Plotter::PlotMap(MapType const &map, PointVector const &positions,
                       std::vector<std::list<Point2>> const &trajectories,
                       std::vector<int> const &robot_status,
                       double const &communication_range) {
@@ -189,30 +190,30 @@
   gp << "\n";
 
   StreamMap(gp, map);
   for (auto const &trajectory : trajectories) {
     for (auto const &pos : trajectory) {
       gp << pos[0] << " " << pos[1] << std::endl;
     }
-    gp << "e\n";
+    gp << "e" << std::endl;
   }
 
   for (size_t i = 0; i < positions.size(); ++i) {
     for (size_t j = i + 1; j < positions.size(); ++j) {
       if ((positions[i] - positions[j]).norm() < communication_range) {
         gp << positions[i][0] << " " << positions[i][1] << "\n";
         gp << positions[j][0] << " " << positions[j][1] << "\n";
         gp << "\n";
       }
     }
   }
-  gp << "e\n";
+  gp << "e" << std::endl;
   for (auto const &pos : positions) {
     gp << pos[0] << " " << pos[1] << std::endl;
-    gp << "e\n";
+    gp << "e" << std::endl;
   }
 }
 
 void Plotter::PlotMap(MapType const &map, PointVector const &positions,
                       std::vector<std::list<Point2>> const &voronoi,
                       std::vector<std::list<Point2>> const &trajectories) {
   Gnuplot gp;
@@ -231,28 +232,28 @@
 
   for (auto const &trajectory : trajectories) {
     for (auto const &pos : trajectory) {
       gp << pos[0] << " " << pos[1] << "\n";
     }
     gp << "\n";
   }
-  gp << "e\n";
+  gp << "e" << std::endl;
 
   for (auto const &vcell : voronoi) {
     for (auto const &pos : vcell) {
       gp << pos[0] << " " << pos[1] << "\n";
     }
     gp << "\n";
   }
-  gp << "e\n";
+  gp << "e" << std::endl;
 
   for (auto const &pos : positions) {
     gp << pos[0] << " " << pos[1] << "\n";
   }
-  gp << "e\n";
+  gp << "e" << std::endl;
 }
 
 void Plotter::PlotMap(MapType const &map, PointVector const &positions,
                       Voronoi const &voronoi,
                       std::vector<std::list<Point2>> const &trajectories) {
   Gnuplot gp;
   if (GnuplotCommands(gp)) {
@@ -270,31 +271,31 @@
 
   for (auto const &trajectory : trajectories) {
     for (auto const &pos : trajectory) {
       gp << pos[0] << " " << pos[1] << "\n";
     }
     gp << "\n";
   }
-  gp << "e\n";
+  gp << "e" << std::endl;
 
   auto voronoi_cells = voronoi.GetVoronoiCells();
   for (auto const &vcell : voronoi_cells) {
     for (auto const &pos : vcell.cell) {
       gp << pos[0] << " " << pos[1] << "\n";
     }
     auto const &pos = vcell.cell.front();
     gp << pos[0] << " " << pos[1] << "\n";
     gp << "\n";
   }
-  gp << "e\n";
+  gp << "e" << std::endl;
 
   for (auto const &pos : positions) {
     gp << pos[0] << " " << pos[1] << "\n";
   }
-  gp << "e\n";
+  gp << "e" << std::endl;
 }
 
 void Plotter::PlotMap(MapType const &map, PointVector const &positions,
                       PointVector const &goals, Voronoi const &voronoi) {
   Gnuplot gp;
   if (GnuplotCommands(gp)) {
     std::cerr << "Error in GnuplotCommands" << std::endl;
@@ -315,34 +316,34 @@
     for (auto const &pos : vcell.cell) {
       gp << pos[0] << " " << pos[1] << std::endl;
     }
     auto const &pos = vcell.cell.front();
     gp << pos[0] << " " << pos[1] << std::endl;
     gp << "\n";
   }
-  gp << "e\n";
+  gp << "e" << std::endl;
 
   for (size_t i = 0; i < positions.size(); ++i) {
     auto const &pos = positions[i];
     auto const &goal = goals[i];
     gp << pos[0] << " " << pos[1] << std::endl;
     gp << goal[0] << " " << goal[1] << std::endl;
     gp << "\n";
   }
-  gp << "e\n";
+  gp << "e" << std::endl;
 
   for (auto const &pos : goals) {
     gp << pos[0] << " " << pos[1] << std::endl;
   }
-  gp << "e\n";
+  gp << "e" << std::endl;
 
   for (auto const &pos : positions) {
     gp << pos[0] << " " << pos[1] << std::endl;
   }
-  gp << "e\n";
+  gp << "e" << std::endl;
 }
 
 void Plotter::PlotMap(MapType const &map, PointVector const &positions,
                       std::vector<std::list<Point2>> const &trajectories,
                       PointVector const &frontiers) {
   Gnuplot gp;
   if (GnuplotCommands(gp)) {
@@ -360,21 +361,21 @@
   StreamMap(gp, map);
   for (auto const &trajectory : trajectories) {
     for (auto const &pos : trajectory) {
       gp << pos[0] << " " << pos[1] << std::endl;
     }
     gp << "\n";
   }
-  gp << "e\n";
+  gp << "e" << std::endl;
 
   for (auto const &pos : positions) {
     gp << pos[0] << " " << pos[1] << std::endl;
   }
-  gp << "e\n";
+  gp << "e" << std::endl;
 
   for (auto const &pos : frontiers) {
     gp << pos[0] << " " << pos[1] << std::endl;
   }
-  gp << "e\n";
+  gp << "e" << std::endl;
 }
 
 }  // namespace CoverageControl
```

### Comparing `coverage_control-1.1.0/cppsrc/core/src/polygon_utils.cpp` & `coverage_control-1.2.0/cppsrc/core/src/polygon_utils.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/src/voronoi.cpp` & `coverage_control-1.2.0/cppsrc/core/src/voronoi.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/core/src/world_idf.cpp` & `coverage_control-1.2.0/cppsrc/core/src/world_idf.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/main/CMakeLists.txt` & `coverage_control-1.2.0/cppsrc/main/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/main/coverage_algorithm.cpp` & `coverage_control-1.2.0/doc/manual/quick_start.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,118 +1,200 @@
-/*
- * This file is part of the CoverageControl library
- *
- * Author: Saurav Agarwal
- * Contact: sauravag@seas.upenn.edu, agr.saurav1@gmail.com
- * Repository: https://github.com/KumarRobotics/CoverageControl
- *
- * Copyright (c) 2024, Saurav Agarwal
- *
- * The CoverageControl library is free software: you can redistribute it and/or
- * modify it under the terms of the GNU General Public License as published by
- * the Free Software Foundation, either version 3 of the License, or (at your
- * option) any later version.
- *
- * The CoverageControl library is distributed in the hope that it will be
- * useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
- * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General
- * Public License for more details.
- *
- * You should have received a copy of the GNU General Public License along with
- * CoverageControl library. If not, see <https://www.gnu.org/licenses/>.
- */
-
-/*!
- * \file coverage_algorithm.cpp
- * \brief Program to test the CVT-based (Lloyd's) coverage control algorithms
- *
- * This program is used to execute CVT-based (Lloyd's) coverage control
- * algorithms. The environment can be initialized with default parameters. The
- * program can also take in a parameter file, a position file and an IDF file.
- * The position file contains the initial positions of the robots and the IDF
- * file contains the location of the features of interest. The program then runs
- * the coverage control algorithm and outputs the final objective value.
- * ```bash
- * ./coverage_algorithm [parameter_file] [<position_file> <idf_file>]
- * ```
- *
- */
+\page quick_start Quick Start
+\tableofcontents
 
-#include <CoverageControl/algorithms/clairvoyant_cvt.h>
-#include <CoverageControl/coverage_system.h>
+# Parameters
+The library uses `toml` files to specify the configuration parameters for the environment and the robot models.  
+The class `CoverageControl::Parameters` is used to load the configuration file and access the parameters.
+
+```python
+params = CoverageControl.Parameters("params/coverage_control_params.toml")
+```
+See \ref params/coverage_control_params.toml for an example configuration file.
+
+# Python Interface
+
+Import the `coverage_control` library and the `ClairvoyantCVT` algorithm.
+```python
+import coverage_control as cc
+from coverage_control import ClairvoyantCVT as CoverageAlgorithm
+```
+
+You can choose one of the following algorithms instead of `ClairvoyantCVT`:
+- `ClairvoyantCVT`
+- `CentralizedCVT`
+- `DecentralizedCVT`
+- `NearOptimalCVT`
+
+Create a `CoverageControl::Parameters` object and load the configuration file:
+```python
+params = cc.Parameters() # for default parameters
+```
+
+Create a simulation environment:
+```python
+env = cc.CoverageSystem(params)
+```
+
+Plot the initial environment (needs `gnuplot` installed):
+```python
+env.PlotInitMap("init_map");
+```
+
+Print the initial coverage cost:
+```python
+init_cost = env.GetObjectiveValue()
+print(f"Initial Coverage cost: {init_cost:.2e}")
+```
+
+Create a controller using the `CoverageAlgorithm` and the environment:
+```python
+controller = CoverageAlgorithm(params, env)
+```
+
+Execute the algorithm:
+```python
+for i in range(0, params.pEpisodeSteps):
+    # Compute actions to be taken by the robots
+    controller.ComputeActions();
+    # Get actions from the controller
+    actions = controller.GetActions()
+
+    # Send actions to the environment
+    if env.StepActions(actions):
+        print(f"Error in step {i}")
+        break
+
+    if controller.IsConverged():
+        print(f"Converged in step {i}")
+        break
+
+```
+
+Print improvement in cost:
+```python
+current_cost = env.GetObjectiveValue()
+print(f"Improvement %: {100 * (init_cost - current_cost)/init_cost:.2f}")
+```
+
+Plot the final state of the environment:
+```cpp
+env.PlotSystemMap("final_map");
+```
+
+
+See \ref python/scripts/coverage_env/coverage_simple.py and \ref python/scripts/coverage_env/coverage_class.py for complete examples.
+
+---
+
+# C++ Interface
+
+\note The C++ interface is not available in the pip package. You need to build the library from source. See the [Installation](https://kumarrobotics.github.io/CoverageControl/installation.html#installation-from-source) guide for instructions.
+
+
+Include the `CoverageControl` library, algorithms, and other necessary headers:
+```cpp
 #include <CoverageControl/parameters.h>
 #include <CoverageControl/typedefs.h>
 #include <CoverageControl/world_idf.h>
-/* #include <CoverageControl/algorithms/centralized_cvt.h> */
-/* #include <CoverageControl/algorithms/decentralized_cvt.h> */
-/* #include <CoverageControl/algorithms/near_optimal_cvt.h> */
-/* #include <CoverageControl/algorithms/simul_explore_exploit.h> */
-/* #include <CoverageControl/bivariate_normal_distribution.h> */
+#include <CoverageControl/coverage_system.h>
+
+#include <CoverageControl/algorithms/clairvoyant_cvt.h>
 
 #include <iostream>
 #include <memory>
 #include <string>
+```
 
+Typedefs and using statements for easier access to the library classes:
+```cpp
 typedef CoverageControl::ClairvoyantCVT CoverageAlgorithm;
-/* typedef CoverageControl::CentralizedCVT CoverageAlgorithm; */
-/* typedef CoverageControl::DecentralizedCVT CoverageAlgorithm; */
-/* typedef CoverageControl::DecentralizedCVT CoverageAlgorithm; */
-/* typedef CoverageControl::NearOptimalCVT CoverageAlgorithm; */
 
-using CoverageControl::CoverageSystem;
-using CoverageControl::Parameters;
 using CoverageControl::Point2;
 using CoverageControl::PointVector;
+using CoverageControl::Parameters;
 using CoverageControl::WorldIDF;
+using CoverageControl::CoverageSystem;
+```
 
-int main(int argc, char** argv) {
-  CoverageControl::CudaUtils::SetUseCuda(false);
-  Parameters params;
-  /* params.pSensorSize = 16; */
-  if (argc >= 2) {
-    std::string parameter_file = argv[1];
-    params = Parameters(parameter_file);
-  }
-
-  std::unique_ptr<CoverageSystem> env;
-
-  if (argc == 3) {
-    std::cerr << "Please provide both position and IDF files" << std::endl;
-    std::cerr << "Usage: ./coverage_algorithm [parameter_file] "
-                 "[<position_file> <idf_file>]"
-              << std::endl;
-    return 1;
-  } else if (argc == 4) {
-    std::string pos_file = argv[2];
-    std::string idf_file = argv[3];
-    WorldIDF world_idf(params, idf_file);
-    env = std::make_unique<CoverageSystem>(params, world_idf, pos_file);
-  } else {
-    env = std::make_unique<CoverageSystem>(params);
-  }
-
-  auto init_objective = env->GetObjectiveValue();
-  std::cout << "Initial objective: " << init_objective << std::endl;
-
-  CoverageAlgorithm algorithm(params, *env);
-  auto goals = algorithm.GetGoals();
-
-  for (int ii = 0; ii < params.pEpisodeSteps; ++ii) {
+Inside the `main` function, create a `Parameters` object:
+```cpp
+Parameters params;
+```
+
+Create coverage system environment:
+```cpp
+CoverageSystem env(params);
+auto init_objective = env.GetObjectiveValue();
+std::cout << "Initial objective: " << init_objective << std::endl;
+```
+
+Plot the initial environment:
+```cpp
+env.PlotInitMap("init_map"); // Creates "init_map.png"
+```
+
+Create a controller using the `CoverageAlgorithm` and the environment:
+```cpp
+CoverageAlgorithm algorithm(params, env);
+```
+
+Execute the algorithm:
+```cpp
+for (int i = 0; i < params.pEpisodeSteps; ++i) {
     algorithm.ComputeActions();
     auto actions = algorithm.GetActions();
-    if (env->StepActions(actions)) {
-      std::cout << "Invalid action" << std::endl;
-      break;
-    }
-    if (ii % 100 == 0) {
-      std::cout << "Step: " << ii << std::endl;
+    if (env.StepActions(actions)) {
+        std::cout << "Invalid action" << std::endl;
+        break;
     }
     if (algorithm.IsConverged()) {
-      break;
+        break;
     }
-  }
-  auto final_objective = env->GetObjectiveValue();
-  std::cout << "Improvement %: "
-            << (init_objective - final_objective) / init_objective * 100
-            << std::endl;
-  return 0;
 }
+```
+
+Print improvement in cost:
+```cpp
+auto final_objective = env.GetObjectiveValue();
+std::cout << "Improvement %: "
+          << (init_objective - final_objective) / init_objective * 100
+          << std::endl;
+```
+
+Plot the final state of the environment:
+```cpp
+env.PlotSystemMap("final_map"); // Creates "final_map.png"
+```
+
+See \ref cppsrc/main/coverage_algorithm.cpp for a complete example.
+
+## Compile and Run
+
+Create a `CMakeLists.txt` file with the following content:
+```python
+cmake_minimum_required(VERSION 3.16)
+project(coveragecontrol)
+
+set(CMAKE_BUILD_TYPE Release)
+set(CMAKE_CXX_STANDARD 17)
+set(CMAKE_CXX_STANDARD_REQUIRED True)
+
+find_package(CoverageControl REQUIRED)
+
+add_executable(coveragecontrol coveragecontrol.cpp) # Replace with your source file
+target_link_libraries(coveragecontrol PRIVATE CoverageControl::CoverageControl)
+install(TARGETS coveragecontrol DESTINATION ${CMAKE_INSTALL_BINDIR})
+```
+
+Build the program:
+```bash
+mkdir build
+cd build
+cmake ..
+make
+```
+
+Run the program:
+```bash
+./coveragecontrol
+```
+
```

### Comparing `coverage_control-1.1.0/cppsrc/main/torch/data_generation.cpp` & `coverage_control-1.2.0/cppsrc/main/torch/data_generation.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/main/torch/eval_dist_gnn.cpp` & `coverage_control-1.2.0/cppsrc/main/torch/eval_dist_gnn.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/main/torch/eval_gnn.cpp` & `coverage_control-1.2.0/cppsrc/main/torch/eval_gnn.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/main/torch/test_cnn.cpp` & `coverage_control-1.2.0/cppsrc/main/torch/test_cnn.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/main/torch/train_cnn.cpp` & `coverage_control-1.2.0/cppsrc/main/torch/train_cnn.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/main/torch/train_gnn.cpp` & `coverage_control-1.2.0/cppsrc/main/torch/train_gnn.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/main/world_idf.cpp` & `coverage_control-1.2.0/cppsrc/python_bindings/python_binds.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -18,53 +18,29 @@
  * Public License for more details.
  *
  * You should have received a copy of the GNU General Public License along with
  * CoverageControl library. If not, see <https://www.gnu.org/licenses/>.
  */
 
 /*!
- * \file world_idf.cpp
- * \brief Program to test generation of IDF
- *
- * ```bash
- * ./world_idf
- * ```
- *
+ * \file python_binds.cpp
+ * \brief Python bindings for the CoverageControl library using pybind11 (\ref
+ * core_binds.h)
  */
 
-#include <CoverageControl/coverage_system.h>
-#include <CoverageControl/parameters.h>
-#include <CoverageControl/typedefs.h>
-#include <CoverageControl/world_idf.h>
-
-#include <iostream>
-#include <memory>
-#include <string>
-
-using CoverageControl::CoverageSystem;
-using CoverageControl::Parameters;
-using CoverageControl::Point2;
-using CoverageControl::PointVector;
-using CoverageControl::WorldIDF;
-
-int main(int argc, char** argv) {
-  CoverageControl::CudaUtils::SetUseCuda(false);
-  Parameters params;
-  params.pNumRobots = 1;
-  params.pNumFeatures = 2;
-  params.pNumPolygons = 20;
-  params.pWorldMapSize = 1024;
-  params.pMaxVertices = 7;
-  params.pPolygonRadius = 128;
-
-  CoverageSystem env(params);
-  env.WriteEnvironment("pos", "env");
-  env.PlotInitMap("init_map");
-  CoverageControl::MapType map = env.GetWorldMap();
-  CoverageControl::CudaUtils::SetUseCuda(true);
-  WorldIDF world_idf(params, "env");
-  CoverageSystem env1(params, world_idf, "pos");
-  env1.WriteEnvironment("pos1", "env1");
-  env1.PlotInitMap("init_map1");
-
-  return 0;
+#include <pybind11/eigen.h>
+#include <pybind11/pybind11.h>
+#include <pybind11/stl_bind.h>
+
+#include "core_binds.h"
+
+PYBIND11_MODULE(_core, m) {
+  CoverageControl::pyCoverageControl_core(m);
+  CoverageControl::pyCoverageControl_core_coverage_system(m);
+  CoverageControl::pyCoverageControl_core_cuda_utils(m);
+
+#ifdef CoverageControl_VERSION
+  m.attr("__version__") = CoverageControl_VERSION;
+#else
+  m.attr("__version__") = "dev";
+#endif
 }
```

### Comparing `coverage_control-1.1.0/cppsrc/python_bindings/core_binds.h` & `coverage_control-1.2.0/cppsrc/python_bindings/core_binds.h`

 * *Files 1% similar despite different names*

```diff
@@ -226,32 +226,35 @@
       .def("GetVoronoiCells", &OracleBangExploreExploit::GetVoronoiCells,
            py::return_value_policy::copy);
 
   py::class_<Parameters>(m, "Parameters")
       .def(py::init<>())
       .def(py::init<std::string const &>())
       .def("SetConfig", &Parameters::SetConfig)
+      .def("PrintParameters", &Parameters::PrintParameters)
       .def_readwrite("pNumRobots", &Parameters::pNumRobots)
       .def_readwrite("pNumFeatures", &Parameters::pNumFeatures)
       .def_readwrite("pNumPolygons", &Parameters::pNumPolygons)
       .def_readwrite("pMaxVertices", &Parameters::pMaxVertices)
       .def_readwrite("pPolygonRadius", &Parameters::pPolygonRadius)
+      .def_readwrite("pPlotScale", &Parameters::pPlotScale)
       .def_readwrite("pResolution", &Parameters::pResolution)
       .def_readwrite("pWorldMapSize", &Parameters::pWorldMapSize)
       .def_readwrite("pRobotMapSize", &Parameters::pRobotMapSize)
       .def_readwrite("pUnknownImportance", &Parameters::pUnknownImportance)
       .def_readwrite("pLocalMapSize", &Parameters::pLocalMapSize)
       .def_readwrite("pCommunicationRange", &Parameters::pCommunicationRange)
       .def_readwrite("pRobotInitDist", &Parameters::pRobotInitDist)
       .def_readwrite("pUpdateRobotMap", &Parameters::pUpdateRobotMap)
       .def_readwrite("pUpdateSensorView", &Parameters::pUpdateSensorView)
       .def_readwrite("pSensorSize", &Parameters::pSensorSize)
       .def_readwrite("pTimeStep", &Parameters::pTimeStep)
       .def_readwrite("pMaxRobotSpeed", &Parameters::pMaxRobotSpeed)
       .def_readwrite("pEpisodeSteps", &Parameters::pEpisodeSteps)
+      .def_readwrite("pCheckOscillations", &Parameters::pCheckOscillations)
       .def_readwrite("pTruncationBND", &Parameters::pTruncationBND)
       .def_readwrite("pNorm", &Parameters::pNorm)
       .def_readwrite("pMinSigma", &Parameters::pMinSigma)
       .def_readwrite("pMaxSigma", &Parameters::pMaxSigma)
       .def_readwrite("pMinPeak", &Parameters::pMinPeak)
       .def_readwrite("pMaxPeak", &Parameters::pMaxPeak)
       .def_readwrite("pLloydNumTries", &Parameters::pLloydNumTries)
@@ -278,14 +281,16 @@
                     PointVector const &>())
       .def("GetWorldMap", &CoverageSystem::GetWorldMap,
            py::return_value_policy::reference_internal)
       .def("GetWorldMapMutable", &CoverageSystem::GetWorldMapMutable,
            py::return_value_policy::reference_internal)
       .def("GetWorldIDFObject", &CoverageSystem::GetWorldIDFObject,
            py::return_value_policy::reference_internal)
+      .def("GetWorldIDF", &CoverageSystem::GetWorldIDFObject,
+           py::return_value_policy::reference_internal)
       .def("StepControl", &CoverageSystem::StepControl)
       .def("StepAction", &CoverageSystem::StepAction)
       .def("StepActions", &CoverageSystem::StepActions)
       .def("SetLocalRobotPositions", &CoverageSystem::SetLocalRobotPositions)
       .def("SetLocalRobotPosition", &CoverageSystem::SetLocalRobotPosition)
       .def("SetGlobalRobotPosition", &CoverageSystem::SetGlobalRobotPosition)
       .def("GetRelativePositonsNeighbors",
@@ -364,15 +369,17 @@
            &CoverageSystem::GetWeightedExplorationRatio)
       .def("RecordPlotData",
            py::overload_cast<>(&CoverageSystem::RecordPlotData))
       .def("RecordPlotData", py::overload_cast<std::string const &>(
                                  &CoverageSystem::RecordPlotData))
       .def("RenderRecordedMap", &CoverageSystem::RenderRecordedMap)
       .def("WriteEnvironment", &CoverageSystem::WriteEnvironment)
-      .def("GetNumRobots", &CoverageSystem::GetNumRobots);
+      .def("GetNumRobots", &CoverageSystem::GetNumRobots)
+      .def("ClearRobotMaps", &CoverageSystem::ClearRobotMaps)
+      .def("ClearExploredIDF", &CoverageSystem::ClearExploredIDF);
 }
 
 // CudaUtils
 void pyCoverageControl_core_cuda_utils(py::module &m) {
   py::class_<CudaUtils>(m, "CudaUtils")
       .def_static("UseCuda", &CudaUtils::UseCuda)
       .def_static("SetUseCuda", &CudaUtils::SetUseCuda)
```

### Comparing `coverage_control-1.1.0/cppsrc/python_bindings/python_binds.cpp` & `coverage_control-1.2.0/cppsrc/tests/torch/torch_test.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,21 @@
 /*
  * This file is part of the CoverageControl library
  *
  * Author: Saurav Agarwal
  * Contact: sauravag@seas.upenn.edu, agr.saurav1@gmail.com
  * Repository: https://github.com/KumarRobotics/CoverageControl
  *
- * Copyright (c) 2024, Saurav Agarwal
+ * The CoverageControl library is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
  *
- * The CoverageControl library is free software: you can redistribute it and/or
- * modify it under the terms of the GNU General Public License as published by
- * the Free Software Foundation, either version 3 of the License, or (at your
- * option) any later version.
+ * The CoverageControl library is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
  *
- * The CoverageControl library is distributed in the hope that it will be
- * useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
- * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General
- * Public License for more details.
- *
- * You should have received a copy of the GNU General Public License along with
- * CoverageControl library. If not, see <https://www.gnu.org/licenses/>.
- */
-
-/*!
- * \file python_binds.cpp
- * \brief Python bindings for the CoverageControl library using pybind11 (\ref
- * core_binds.h)
+ * You should have received a copy of the GNU General Public License along with CoverageControl library. If not, see <https://www.gnu.org/licenses/>.
  */
 
-#include <pybind11/eigen.h>
-#include <pybind11/pybind11.h>
-#include <pybind11/stl_bind.h>
-
-#include "core_binds.h"
-
-PYBIND11_MODULE(_core, m) {
-  CoverageControl::pyCoverageControl_core(m);
-  CoverageControl::pyCoverageControl_core_coverage_system(m);
-  CoverageControl::pyCoverageControl_core_cuda_utils(m);
+#include <torch/torch.h>
+#include <iostream>
+#include <CoverageControlTorch/base.h>
 
-#ifdef CoverageControl_VERSION
-  m.attr("__version__") = CoverageControl_VERSION;
-#else
-  m.attr("__version__") = "dev";
-#endif
+int main() {
+	CoverageControlTorch::base();
 }
```

### Comparing `coverage_control-1.1.0/cppsrc/setup.sh` & `coverage_control-1.2.0/cppsrc/setup.sh`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/tests/CMakeLists.txt` & `coverage_control-1.2.0/cppsrc/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/tests/geo_transforms.cpp` & `coverage_control-1.2.0/cppsrc/tests/geo_transforms.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/tests/map_generation.cpp` & `coverage_control-1.2.0/cppsrc/tests/map_generation.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/tests/simultaneous_explore_exploit.cpp` & `coverage_control-1.2.0/cppsrc/tests/simultaneous_explore_exploit.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/tests/torch/torch_data_loader.cpp` & `coverage_control-1.2.0/cppsrc/tests/torch/torch_data_loader.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/tests/torch/torch_map_conversion.cpp` & `coverage_control-1.2.0/cppsrc/tests/torch/torch_map_conversion.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/tests/torch/torch_normalization.cpp` & `coverage_control-1.2.0/cppsrc/tests/torch/torch_normalization.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/tests/torch/torch_scripting.cpp` & `coverage_control-1.2.0/cppsrc/tests/torch/torch_scripting.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/tests/torch/torch_test.cpp` & `coverage_control-1.2.0/cppsrc/torch/include/CoverageControlTorch/base.h`

 * *Files 13% similar despite different names*

```diff
@@ -10,12 +10,13 @@
  * The CoverageControl library is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
  *
  * You should have received a copy of the GNU General Public License along with CoverageControl library. If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <torch/torch.h>
 #include <iostream>
-#include <CoverageControlTorch/base.h>
+#include <CoverageControl/coverage_system.h>
 
-int main() {
-	CoverageControlTorch::base();
-}
+
+namespace CoverageControlTorch {
+	int base();
+} /* namespace CoverageControlTorch */
```

### Comparing `coverage_control-1.1.0/cppsrc/torch/CMakeLists.txt` & `coverage_control-1.2.0/cppsrc/torch/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/torch/cmake/CoverageControlTorchConfig.cmake.in` & `coverage_control-1.2.0/cppsrc/torch/cmake/CoverageControlTorchConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/base.h` & `coverage_control-1.2.0/python/tests/test_package.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,28 @@
-/*
- * This file is part of the CoverageControl library
- *
- * Author: Saurav Agarwal
- * Contact: sauravag@seas.upenn.edu, agr.saurav1@gmail.com
- * Repository: https://github.com/KumarRobotics/CoverageControl
- *
- * The CoverageControl library is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
- *
- * The CoverageControl library is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License along with CoverageControl library. If not, see <https://www.gnu.org/licenses/>.
- */
+#  This file is part of the CoverageControl library
+#
+#  Author: Saurav Agarwal
+#  Contact: sauravag@seas.upenn.edu, agr.saurav1@gmail.com
+#  Repository: https://github.com/KumarRobotics/CoverageControl
+#
+#  Copyright (c) 2024, Saurav Agarwal
+#
+#  The CoverageControl library is free software: you can redistribute it and/or
+#  modify it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 3 of the License, or (at your
+#  option) any later version.
+#
+#  The CoverageControl library is distributed in the hope that it will be
+#  useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General
+#  Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License along with
+#  CoverageControl library. If not, see <https://www.gnu.org/licenses/>.
 
-#include <torch/torch.h>
-#include <iostream>
-#include <CoverageControl/coverage_system.h>
+import importlib.metadata
 
+import coverage_control as m
 
-namespace CoverageControlTorch {
-	int base();
-} /* namespace CoverageControlTorch */
+
+def test_version():
+    assert importlib.metadata.version("coverage_control") == m.__version__
```

### Comparing `coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/cnn_backbone.h` & `coverage_control-1.2.0/cppsrc/torch/include/CoverageControlTorch/cnn_backbone.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/cnn_module.h` & `coverage_control-1.2.0/cppsrc/torch/include/CoverageControlTorch/cnn_module.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/coverage_system.h` & `coverage_control-1.2.0/cppsrc/torch/include/CoverageControlTorch/coverage_system.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/edge_wts_comm_map_generator.h` & `coverage_control-1.2.0/cppsrc/torch/include/CoverageControlTorch/edge_wts_comm_map_generator.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/extern/tomlplusplus/toml.hpp` & `coverage_control-1.2.0/cppsrc/torch/include/CoverageControlTorch/extern/tomlplusplus/toml.hpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/generate_dataset.h` & `coverage_control-1.2.0/cppsrc/torch/include/CoverageControlTorch/generate_dataset.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/gnn_backbone.h` & `coverage_control-1.2.0/cppsrc/torch/include/CoverageControlTorch/gnn_backbone.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/mlp.h` & `coverage_control-1.2.0/cppsrc/torch/include/CoverageControlTorch/mlp.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/train_cnn.h` & `coverage_control-1.2.0/cppsrc/torch/include/CoverageControlTorch/train_cnn.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/type_conversions.h` & `coverage_control-1.2.0/cppsrc/torch/include/CoverageControlTorch/type_conversions.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/torch/python_bindings/CMakeLists.txt` & `coverage_control-1.2.0/cppsrc/torch/python_bindings/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/torch/python_bindings/src/coverage_control_torch_extension.cpp` & `coverage_control-1.2.0/cppsrc/torch/python_bindings/src/coverage_control_torch_extension.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/torch/src/base.cpp` & `coverage_control-1.2.0/cppsrc/torch/src/base.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/cppsrc/torch/src/coverage_system.cpp` & `coverage_control-1.2.0/cppsrc/torch/src/coverage_system.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/doc/Doxyfile` & `coverage_control-1.2.0/doc/Doxyfile`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 												 doc/manual/lpac.md \
 												 doc/manual/coverage-control.md \
 												 cppsrc/core \
 												 params \
 												 cppsrc/main/coverage_algorithm.cpp \
                          python/coverage_control \
                          python/scripts \
-                         python/utils
+                         python/utils \
+                         python/utils/process_data.sh
 EXCLUDE                = doc/cppsrc/torch doc/cppsrc/main/torch
 OUTPUT_DIRECTORY       = doc/
 LAYOUT_FILE            = doc/config/DoxygenLayout.xml
 HIDE_SCOPE_NAMES       = YES
 IMAGE_PATH             = doc/graphics
 HTML_EXTRA_FILES			+= doc/graphics/LPAC.gif doc/graphics/coveragecontrol_global.png doc/graphics/learnable_pac.png
 FILTER_PATTERNS        = "*.md=python doc/bash-filter.py" *.py=doc/py-filter.sh
```

### Comparing `coverage_control-1.1.0/doc/bash-filter.py` & `coverage_control-1.2.0/doc/bash-filter.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/doc/config/BaseDoxyfile` & `coverage_control-1.2.0/doc/config/BaseDoxyfile`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/doc/config/DoxygenLayout.xml` & `coverage_control-1.2.0/doc/config/DoxygenLayout.xml`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/doc/config/custom.css` & `coverage_control-1.2.0/doc/config/custom.css`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/doc/config/doxygen-awesome-darkmode-toggle.js` & `coverage_control-1.2.0/doc/config/doxygen-awesome-darkmode-toggle.js`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/doc/config/doxygen-awesome-fragment-copy-button.js` & `coverage_control-1.2.0/doc/config/doxygen-awesome-fragment-copy-button.js`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/doc/config/doxygen-awesome-interactive-toc.js` & `coverage_control-1.2.0/doc/config/doxygen-awesome-interactive-toc.js`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/doc/config/doxygen-awesome-paragraph-link.js` & `coverage_control-1.2.0/doc/config/doxygen-awesome-paragraph-link.js`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/doc/config/doxygen-awesome-sidebar-only-darkmode-toggle.css` & `coverage_control-1.2.0/doc/config/doxygen-awesome-sidebar-only-darkmode-toggle.css`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/doc/config/doxygen-awesome-sidebar-only.css` & `coverage_control-1.2.0/doc/config/doxygen-awesome-sidebar-only.css`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/doc/config/doxygen-awesome-tabs.js` & `coverage_control-1.2.0/doc/config/doxygen-awesome-tabs.js`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/doc/config/doxygen-awesome.css` & `coverage_control-1.2.0/doc/config/doxygen-awesome.css`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/doc/config/header.html` & `coverage_control-1.2.0/doc/config/header.html`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/doc/config/navtree-hacks.js` & `coverage_control-1.2.0/doc/config/navtree-hacks.js`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/doc/graphics/LPAC.gif` & `coverage_control-1.2.0/doc/graphics/LPAC.gif`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/doc/graphics/SearchRescue.png` & `coverage_control-1.2.0/doc/graphics/SearchRescue.png`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/doc/graphics/coveragecontrol_global.png` & `coverage_control-1.2.0/doc/graphics/coveragecontrol_global.png`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/doc/graphics/learnable_pac.png` & `coverage_control-1.2.0/doc/graphics/learnable_pac.png`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/doc/manual/README.md` & `coverage_control-1.2.0/doc/manual/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -11,19 +11,18 @@
 The library provides a simulation environment, algorithms, and GNN-based architectures for the coverage control problem.  
 
 **Key features:**  
 - The core library is written in `C++` and `CUDA` to handle large-scale simulations
 - There are `python` bindings that interface with the core library
 - Several Centroidal Voronoi Tessellation (CVT)-based algorithms (aka Lloyd's algorithms)
 - Learnable Perception-Action-Communication (LPAC) architecture for the coverage control problem is implemented in `PyTorch` and `PyTorch Geometric`
-- GPU and CPU parallelization using `CUDA` and `OpenMP`
 
 ---
 
-## Quick Start
+## Getting Started
 The library is available as a `pip` package. To install the package, run the following command:
 ```bash
 pip install coverage_control
 ```
 
 See [Installation](https://kumarrobotics.github.io/CoverageControl/installation.html) for more details on installation.
```

### Comparing `coverage_control-1.1.0/doc/manual/algorithms.md` & `coverage_control-1.2.0/doc/manual/algorithms.md`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/doc/manual/coverage-control.md` & `coverage_control-1.2.0/doc/manual/coverage-control.md`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/doc/manual/docker.md` & `coverage_control-1.2.0/doc/manual/docker.md`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/doc/manual/installation.md` & `coverage_control-1.2.0/doc/manual/installation.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 ```bash
 pip install coverage_control
 ```
 
 The package depends on the following packages
 - [PyTorch](https://pytorch.org/)
 - [PyTorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/)
+
 ```bash
 pip install torch torchvision torch-geometric
 ```
 
 \note PyTorch and PyTorch Geometric have CPU and CUDA-specific versions. The command installs the default version (latest CUDA).
 
 We need the following optional packages for visualization and video generation:
@@ -77,15 +78,15 @@
 
 The base image is `ghcr.io/\repo_owner_lower/coveragecontrol` with different tags for different versions and configurations.
 
 |Tags Suffix | Flags|
 |--- | ---|
 |`python2.2.2-cuda12.2.2-ros2humble` | `--with-ros --with-cuda`|
 |`python2.2.2-cuda12.2.2` | `--with-cuda`|
-|`python2.2.1-ros2humble` | `--with-ros`|
+|`python2.2.2-ros2humble` | `--with-ros`|
 |`python2.2.2` | None|
 
 The library is already built and installed in the container.
 However, if you want to build it again, you can do so following the [Installation from Source](#installation-from-source) instructions (except for the prerequisites).
 
 --------
 
@@ -118,15 +119,15 @@
 
 ```bash
 pip install .
 ```
 
 Testing the installation (from the root of the repository):
 
-Download the file `pytest_data.tar.gz` from the repository's release page and extract it to `python/tests/`.
+Download the file `pytest_data.tar.gz` from the repository's [release page](https://github.com/KumarRobotics/CoverageControl/releases) and extract it to `python/tests/`.
 This will create a directory `python/tests/data`.
 
 Then run the following commands:
 ```bash
 pip install pytest
 pytest
 ```
```

### Comparing `coverage_control-1.1.0/doc/manual/lpac.md` & `coverage_control-1.2.0/doc/manual/lpac.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 \page lpac LPAC Neural Network
 \tableofcontents
 
 # Preliminaries
 We will organize files in a **workspace** directory: `${CoverageControl_ws}` (e.g., ~/CoverageControl\_ws).
 
 Download and extract the file `lpac_CoverageControl.tar.gz` to the workspace directory.
-The file can be downloaded from the repository's release page.
+The file can be downloaded from the repository [releases](https://github.com/KumarRobotics/CoverageControl/releases).
 ```bash
 tar -xvzf lpac_CoverageControl.tar.gz -C ${CoverageControl_ws}
 ```
 This will create a directory `lpac` in the workspace directory.
 The directory structure is as follows:
 ```bash
 ${CoverageControl_ws}/
```

### Comparing `coverage_control-1.1.0/doc/manual/ref_manual.txt` & `coverage_control-1.2.0/doc/manual/ref_manual.txt`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/params/coverage_control_params.toml` & `coverage_control-1.2.0/params/coverage_control_params.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 NumRobots = 32
 NumFeatures = 32
 
 NumPolygons = 0
 MaxVertices = 10
 PolygonRadius = 64
 
+[IO]
+# Determines the quality of the plot and videos
+# > 1: High quality (takes more time to plot)
+# < 1: Low quality (takes less time to plot)
+PlotScale = 1.0
+
 # Parameters for the environment
 [Environment]
 
 [Environment.Maps]
 # Assuming same resolution in both the directions. Pixel area = Resolution^2
 Resolution = 1
 
@@ -77,14 +83,15 @@
 PositionsNoiseSigma = 0.1
 
 # Parameters for the standard baseline coverage control algorithms
 [Algorithm]
 
 # Number of steps in an episode
 EpisodeSteps = 2100
+CheckOscillations = true
 
 [Algorithm.Global-CVT]
 # Settings for Global-CVT algorithm
 LloydMaxIterations = 1000
 LloydNumTries = 20
 
 [Algorithm.Exploration]
```

### Comparing `coverage_control-1.1.0/params/data_params.toml` & `coverage_control-1.2.0/params/data_params.toml`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/params/eval.toml` & `coverage_control-1.2.0/params/eval.toml`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/params/eval_single.toml` & `coverage_control-1.2.0/params/eval_single.toml`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/params/learning_params.toml` & `coverage_control-1.2.0/params/learning_params.toml`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/pyproject.toml` & `coverage_control-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 repair-wheel-command = ""
 
 # test-command=""
 # before-test=""
 test-command = "pytest -ra --showlocals --ignore={project}/python/tests/deprecated {project}/python/tests/test_coverage_env_utils.py {project}/python/tests/test_coverage.py {project}/python/tests/test_env_io.py {project}/python/tests/test_map_generation.py {project}/python/tests/test_models.py {project}/python/tests/test_package.py {project}/python/tests/test_parameters.py {project}/python/tests/test_parity.py"
 
-before-test = "pip install pytest torch torchvision torch_geometric && wget https://github.com/KumarRobotics/CoverageControl/releases/download/v1.1.0/pytest_data.tar.gz && tar -xvf pytest_data.tar.gz -C python/tests/ && rm pytest_data.tar.gz"
+before-test = "pip install pytest torch torchvision torch_geometric && wget https://github.com/KumarRobotics/CoverageControl/releases/download/v1.2.0/pytest_data.tar.gz && tar -xvf pytest_data.tar.gz -C python/tests/ && rm pytest_data.tar.gz"
 test-requires = []
 test-extras = []
 
 container-engine = "docker"
 
 manylinux-x86_64-image = "manylinux_2_28"
 manylinux-aarch64-image = "manylinux_2_28"
```

### Comparing `coverage_control-1.1.0/python/coverage_control/core/__init__.py` & `coverage_control-1.2.0/python/coverage_control/core/__init__.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/coverage_control/io_utils.py` & `coverage_control-1.2.0/python/coverage_control/io_utils.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/coverage_control/nn/data_loaders/coverage_env_utils.py` & `coverage_control-1.2.0/python/coverage_control/nn/data_loaders/coverage_env_utils.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/coverage_control/nn/data_loaders/data_loader_utils.py` & `coverage_control-1.2.0/python/coverage_control/nn/data_loaders/data_loader_utils.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/coverage_control/nn/data_loaders/loaders.py` & `coverage_control-1.2.0/python/coverage_control/nn/data_loaders/loaders.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/coverage_control/nn/models/cnn.py` & `coverage_control-1.2.0/python/coverage_control/nn/models/cnn.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/coverage_control/nn/models/cnn_backbone.py` & `coverage_control-1.2.0/python/coverage_control/nn/models/cnn_backbone.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/coverage_control/nn/models/config_parser.py` & `coverage_control-1.2.0/python/coverage_control/nn/models/config_parser.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/coverage_control/nn/models/gnn_backbone.py` & `coverage_control-1.2.0/python/coverage_control/nn/models/gnn_backbone.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/coverage_control/nn/models/lpac.py` & `coverage_control-1.2.0/python/coverage_control/nn/models/lpac.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/coverage_control/nn/trainers/trainer.py` & `coverage_control-1.2.0/python/coverage_control/nn/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/scripts/data_generation/data_generation.py` & `coverage_control-1.2.0/python/scripts/data_generation/data_generation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,10 @@
-#  This file is part of the CoverageControl library
-#
-#  Author: Saurav Agarwal
-#  Contact: sauravag@seas.upenn.edu, agr.saurav1@gmail.com
-#  Repository: https://github.com/KumarRobotics/CoverageControl
-#
-#  Copyright (c) 2024, Saurav Agarwal
-#
-#  The CoverageControl library is free software: you can redistribute it and/or
-#  modify it under the terms of the GNU General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or (at your
-#  option) any later version.
-#
-#  The CoverageControl library is distributed in the hope that it will be
-#  useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General
-#  Public License for more details.
-#
-#  You should have received a copy of the GNU General Public License along with
-#  CoverageControl library. If not, see <https://www.gnu.org/licenses/>.
-
 # @file data_generation.py
 # This file contains the code to generate a dataset for learning
 #
-
 # DataDir =  "${CoverageControl_ws}/datasets/lpac" # Absolute location
 # EnvironmentConfig = "${CoverageControl_ws}/datasets/lpac/coverage_control_params.toml" # Absolute location
 #
 # NumDataset = 1000
 #
 # # Number of steps to take before data is stores
 # # This helps in creating a more diverse dataset
@@ -44,38 +22,38 @@
 # SaveAsSparseQ = true
 # NormalizeQ = true
 #
 # [DataSetSplit]
 # TrainRatio = 0.7
 # ValRatio =  0.2
 # TestRatio = 0.1
-
-## @file data_generation.py
+# @file data_generation.py
 #  @brief Class to generate CoverageControl dataset for LPAC architecture
-
-import os
-import sys
-import pathlib
 import datetime
 import math
+import os
+import pathlib
+import sys
 
 import coverage_control
 import torch
-from coverage_control import CoverageSystem, IOUtils
+from coverage_control import CoverageSystem
+from coverage_control import IOUtils
 from coverage_control.algorithms import ClairvoyantCVT as CoverageAlgorithm
 from coverage_control.nn import CoverageEnvUtils
 
-## @ingroup python_api
+# @ingroup python_api
+
+
 class DatasetGenerator:
     """
     Class to generate CoverageControl dataset for LPAC architecture
     """
 
     def __init__(self, config_file, append_dir=None):
-
         self.config = IOUtils.load_toml(config_file)
         self.data_dir = IOUtils.sanitize_path(self.config["DataDir"])
         self.dataset_dir = self.data_dir + "/data/"
 
         if append_dir is not None:
             self.dataset_dir += append_dir
```

### Comparing `coverage_control-1.1.0/python/scripts/data_generation/simple_data_generation.py` & `coverage_control-1.2.0/python/scripts/data_generation/simple_data_generation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,10 @@
-#  This file is part of the CoverageControl library
-#
-#  Author: Saurav Agarwal
-#  Contact: sauravag@seas.upenn.edu, agr.saurav1@gmail.com
-#  Repository: https://github.com/KumarRobotics/CoverageControl
-#
-#  Copyright (c) 2024, Saurav Agarwal
-#
-#  The CoverageControl library is free software: you can redistribute it and/or
-#  modify it under the terms of the GNU General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or (at your
-#  option) any later version.
-#
-#  The CoverageControl library is distributed in the hope that it will be
-#  useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General
-#  Public License for more details.
-#
-#  You should have received a copy of the GNU General Public License along with
-#  CoverageControl library. If not, see <https://www.gnu.org/licenses/>.
-
 # @file simple_data_generation.py
 # This file contains the code to generate a dataset for learning
 #
-
 # Uses the following configuration given in a toml file:
 # DataDir =  "${CoverageControl_ws}/datasets/lpac" # Absolute location
 # EnvironmentConfig = "${CoverageControl_ws}/datasets/lpac/coverage_control_params.toml" # Absolute location
 #
 # NumDataset = 1000
 #
 # # Number of steps to take before data is stores
@@ -38,61 +16,64 @@
 # ConvergedDataRatio = 0.02
 #
 # # Resizing of maps and Sparsification of tensors are triggered every TriggerPostProcessing dataset
 # # This should be set based on RAM resources available on the system
 # TriggerPostProcessing = 100
 #
 # CNNMapSize = 32
-
-## @file simple_data_generation.py
+# @file simple_data_generation.py
 #  @brief Generates a dataset for coverage control learning
-
-import os
-import sys
-import torch
 import math
+import os
 import pathlib
+import sys
 
 import coverage_control
-from coverage_control import IOUtils
+import torch
 from coverage_control import CoverageSystem
+from coverage_control import IOUtils
 from coverage_control.algorithms import ClairvoyantCVT as CoverageAlgorithm
 from coverage_control.nn import CoverageEnvUtils
 
-## @ingroup python_api
-class SimpleDatasetGenerator():
+# @ingroup python_api
+
+
+class SimpleDatasetGenerator:
     """
     Class for generating dataset for learning
     """
+
     def __init__(self, config_file: str, append_dir: str = None):
         """
         Constructor for the class
 
         Args:
             config_file (str): Configuration file in toml format
             append_dir (str): Name of the directory to append to the dataset directory
         """
 
         self.config = IOUtils.load_toml(config_file)
-        self.data_dir = IOUtils.sanitize_path(self.config['DataDir'])
-        self.dataset_dir = self.data_dir + '/data/'
+        self.data_dir = IOUtils.sanitize_path(self.config["DataDir"])
+        self.dataset_dir = self.data_dir + "/data/"
+
         if append_dir is not None:
             self.dataset_dir += append_dir
 
         if not pathlib.Path(self.data_dir).exists():
-            print(f'{self.data_dir} does not exist')
+            print(f"{self.data_dir} does not exist")
             exit()
 
         if not pathlib.Path(self.dataset_dir).exists():
             os.makedirs(self.dataset_dir)
 
         env_config_file = IOUtils.sanitize_path(self.config["EnvironmentConfig"])
         env_config_file = pathlib.Path(env_config_file)
+
         if not env_config_file.exists():
-            print(f'{env_config_file} does not exist')
+            print(f"{env_config_file} does not exist")
             exit()
 
         self.env_params = coverage_control.Parameters(env_config_file.as_posix())
 
         # Initialize variables
         self.dataset_count = 0
         self.env_count = 0
@@ -103,157 +84,255 @@
         self.num_robots = self.env_params.pNumRobots
         self.comm_range = self.env_params.pCommunicationRange
         self.resolution = self.env_params.pResolution
         self.cnn_map_size = self.config["CNNMapSize"]
         self.every_num_step = self.config["EveryNumSteps"]
         self.trigger_size = self.config["TriggerPostProcessing"]
         self.converged_data_ratio = self.config["ConvergedDataRatio"]
+
         if self.trigger_size == 0 or self.trigger_size > self.num_dataset:
             self.trigger_size = self.num_dataset
 
         if torch.cuda.is_available():
             self.device = torch.device("cuda")
         else:
             self.device = torch.device("cpu")
 
         # Initialize tensors
         self.actions = torch.zeros((self.num_dataset, self.num_robots, 2))
         self.robot_positions = torch.zeros((self.num_dataset, self.num_robots, 2))
-        self.raw_local_maps = torch.zeros((self.trigger_size, self.num_robots, self.env_params.pLocalMapSize, self.env_params.pLocalMapSize))
-        self.raw_obstacle_maps = torch.zeros((self.trigger_size, self.num_robots, self.env_params.pLocalMapSize, self.env_params.pLocalMapSize))
-        self.local_maps = torch.zeros((self.num_dataset, self.num_robots, self.cnn_map_size, self.cnn_map_size))
-        self.obstacle_maps = torch.zeros((self.num_dataset, self.num_robots, self.cnn_map_size, self.cnn_map_size))
-        self.comm_maps = torch.zeros((self.num_dataset, self.num_robots, 2, self.cnn_map_size, self.cnn_map_size))
+        self.raw_local_maps = torch.zeros(
+            (
+                self.trigger_size,
+                self.num_robots,
+                self.env_params.pLocalMapSize,
+                self.env_params.pLocalMapSize,
+            )
+        )
+        self.raw_obstacle_maps = torch.zeros(
+            (
+                self.trigger_size,
+                self.num_robots,
+                self.env_params.pLocalMapSize,
+                self.env_params.pLocalMapSize,
+            )
+        )
+        self.local_maps = torch.zeros(
+            (self.num_dataset, self.num_robots, self.cnn_map_size, self.cnn_map_size)
+        )
+        self.obstacle_maps = torch.zeros(
+            (self.num_dataset, self.num_robots, self.cnn_map_size, self.cnn_map_size)
+        )
+        self.comm_maps = torch.zeros(
+            (self.num_dataset, self.num_robots, 2, self.cnn_map_size, self.cnn_map_size)
+        )
         self.coverage_features = torch.zeros((self.num_dataset, self.num_robots, 7))
-        self.edge_weights = torch.zeros((self.num_dataset, self.num_robots, self.num_robots))
+        self.edge_weights = torch.zeros(
+            (self.num_dataset, self.num_robots, self.num_robots)
+        )
 
         self.run_data_generation()
         self.trigger_post_processing()
         del self.raw_local_maps
         del self.raw_obstacle_maps
         self.save_dataset()
 
     def run_data_generation(self):
         num_non_converged_env = 0
+
         while self.dataset_count < self.num_dataset:
-            self.env = CoverageSystem(self.env_params, self.env_params.pNumFeatures, self.num_robots)
+            self.env = CoverageSystem(
+                self.env_params, self.env_params.pNumFeatures, self.num_robots
+            )
             self.alg = CoverageAlgorithm(self.env_params, self.num_robots, self.env)
             self.env_count += 1
-            print('Environment: ' + str(self.env_count))
+            print("Environment: " + str(self.env_count))
             num_steps = 0
             is_converged = False
-            while num_steps < self.env_params.pEpisodeSteps and not is_converged and self.dataset_count < self.num_dataset:
+
+            while (
+                num_steps < self.env_params.pEpisodeSteps
+                and not is_converged
+                and self.dataset_count < self.num_dataset
+            ):
                 if num_steps % self.every_num_step == 0:
                     is_converged = self.step_with_save()
                 else:
                     is_converged = self.step_without_save()
                 num_steps += 1
+
             if num_steps == self.env_params.pEpisodeSteps:
                 num_non_converged_env += 1
-                print('Non-converged environment: ' + str(num_non_converged_env))
+                print("Non-converged environment: " + str(num_non_converged_env))
 
-            print('Converged in ' + str(num_steps) + ' steps')
+            print("Converged in " + str(num_steps) + " steps")
 
-            num_converged_data = math.ceil(self.converged_data_ratio * num_steps / self.every_num_step)
+            num_converged_data = math.ceil(
+                self.converged_data_ratio * num_steps / self.every_num_step
+            )
             converged_data_count = 0
-            while converged_data_count < num_converged_data and self.dataset_count < self.num_dataset:
+
+            while (
+                converged_data_count < num_converged_data
+                and self.dataset_count < self.num_dataset
+            ):
                 self.step_with_save()
                 converged_data_count += 1
 
     def step_with_save(self):
         self.alg.ComputeActions()
         converged = self.alg.IsConverged()
         actions = self.alg.GetActions()
         count = self.dataset_count
         self.actions[count] = CoverageEnvUtils.to_tensor(actions)
         self.robot_positions[count] = CoverageEnvUtils.get_robot_positions(self.env)
         self.coverage_features[count] = CoverageEnvUtils.get_voronoi_features(self.env)
-        self.raw_local_maps[self.trigger_count] = CoverageEnvUtils.get_raw_local_maps(self.env, self.env_params)
-        self.raw_obstacle_maps[self.trigger_count] = CoverageEnvUtils.get_raw_obstacle_maps(self.env, self.env_params)
-        self.comm_maps[count] = CoverageEnvUtils.get_communication_maps(self.env, self.env_params, self.cnn_map_size)
-        self.edge_weights[count] = CoverageEnvUtils.get_weights(self.env, self.env_params)
+        self.raw_local_maps[self.trigger_count] = CoverageEnvUtils.get_raw_local_maps(
+            self.env, self.env_params
+        )
+        self.raw_obstacle_maps[self.trigger_count] = (
+            CoverageEnvUtils.get_raw_obstacle_maps(self.env, self.env_params)
+        )
+        self.comm_maps[count] = CoverageEnvUtils.get_communication_maps(
+            self.env, self.env_params, self.cnn_map_size
+        )
+        self.edge_weights[count] = CoverageEnvUtils.get_weights(
+            self.env, self.env_params
+        )
         self.dataset_count += 1
+
         if self.dataset_count % 100 == 0:
-            print(f'Dataset: {self.dataset_count}/{self.num_dataset}')
+            print(f"Dataset: {self.dataset_count}/{self.num_dataset}")
 
         self.trigger_count += 1
+
         if self.trigger_count == self.trigger_size:
             self.trigger_post_processing()
             self.trigger_count = 0
 
-        if(self.env.StepActions(actions)):
+        if self.env.StepActions(actions):
             return True
+
         return converged
 
     def trigger_post_processing(self):
-        if self.trigger_start_idx > self.num_dataset -1:
+        if self.trigger_start_idx > self.num_dataset - 1:
             return
-        trigger_end_idx = min(self.num_dataset, self.trigger_start_idx + self.trigger_size)
-        raw_local_maps = self.raw_local_maps[0:trigger_end_idx - self.trigger_start_idx]
+        trigger_end_idx = min(
+            self.num_dataset, self.trigger_start_idx + self.trigger_size
+        )
+        raw_local_maps = self.raw_local_maps[
+            0 : trigger_end_idx - self.trigger_start_idx
+        ]
         raw_local_maps = raw_local_maps.to(self.device)
-        resized_local_maps = CoverageEnvUtils.resize_maps(raw_local_maps, self.cnn_map_size)
-        self.local_maps[self.trigger_start_idx:trigger_end_idx] = resized_local_maps.view(-1, self.num_robots, self.cnn_map_size, self.cnn_map_size).cpu().clone()
-
-        raw_obstacle_maps = self.raw_obstacle_maps[0:trigger_end_idx - self.trigger_start_idx]
+        resized_local_maps = CoverageEnvUtils.resize_maps(
+            raw_local_maps, self.cnn_map_size
+        )
+        self.local_maps[self.trigger_start_idx : trigger_end_idx] = (
+            resized_local_maps.view(
+                -1, self.num_robots, self.cnn_map_size, self.cnn_map_size
+            )
+            .cpu()
+            .clone()
+        )
+
+        raw_obstacle_maps = self.raw_obstacle_maps[
+            0 : trigger_end_idx - self.trigger_start_idx
+        ]
         raw_obstacle_maps = raw_obstacle_maps.to(self.device)
-        resized_obstacle_maps = CoverageEnvUtils.resize_maps(raw_obstacle_maps, self.cnn_map_size)
-        self.obstacle_maps[self.trigger_start_idx:trigger_end_idx] = resized_obstacle_maps.view(-1, self.num_robots, self.cnn_map_size, self.cnn_map_size).cpu().clone()
+        resized_obstacle_maps = CoverageEnvUtils.resize_maps(
+            raw_obstacle_maps, self.cnn_map_size
+        )
+        self.obstacle_maps[self.trigger_start_idx : trigger_end_idx] = (
+            resized_obstacle_maps.view(
+                -1, self.num_robots, self.cnn_map_size, self.cnn_map_size
+            )
+            .cpu()
+            .clone()
+        )
 
         self.trigger_start_idx = trigger_end_idx
 
     def normalize_tensor(self, tensor):
         tensor_mean = tensor.mean(dim=[0, 1])
         tensor_std = tensor.std(dim=[0, 1])
         tensor = (tensor - tensor_mean) / tensor_std
+
         return tensor, tensor_mean, tensor_std
 
     def normalize_communication_maps(self):
         min_val = self.comm_maps.min()
         max_val = self.comm_maps.max()
         range_val = max_val - min_val
         self.comm_maps = (self.comm_maps - min_val) / range_val
-        print('Communication map min: ' + str(min_val))
-        print('Communication map max: ' + str(max_val))
+        print("Communication map min: " + str(min_val))
+        print("Communication map max: " + str(max_val))
+
         return min_val, range_val
 
     def save_dataset(self):
         dataset_dir_path = pathlib.Path(self.dataset_dir)
-        torch.save(self.robot_positions, dataset_dir_path / 'robot_positions.pt')
-        torch.save(self.local_maps.to_sparse(), dataset_dir_path / 'local_maps.pt')
-        torch.save(self.obstacle_maps.to_sparse(), dataset_dir_path / 'obstacle_maps.pt')
-        torch.save(self.edge_weights.to_sparse(), dataset_dir_path / 'edge_weights.pt')
-
-        torch.save(self.comm_maps.to_sparse(), dataset_dir_path / 'comm_maps.pt')
+        torch.save(self.robot_positions, dataset_dir_path / "robot_positions.pt")
+        torch.save(self.local_maps.to_sparse(), dataset_dir_path / "local_maps.pt")
+        torch.save(
+            self.obstacle_maps.to_sparse(), dataset_dir_path / "obstacle_maps.pt"
+        )
+        torch.save(self.edge_weights.to_sparse(), dataset_dir_path / "edge_weights.pt")
 
-        torch.save(self.actions, dataset_dir_path / 'actions.pt')
-        torch.save(self.coverage_features, dataset_dir_path / 'coverage_features.pt')
+        torch.save(self.comm_maps.to_sparse(), dataset_dir_path / "comm_maps.pt")
 
+        torch.save(self.actions, dataset_dir_path / "actions.pt")
+        torch.save(self.coverage_features, dataset_dir_path / "coverage_features.pt")
 
     def step_without_save(self):
         self.alg.ComputeActions()
         converged = self.alg.IsConverged()
-        if (self.env.StepActions(self.alg.GetActions())):
+
+        if self.env.StepActions(self.alg.GetActions()):
             return True
+
         return converged
 
     def get_tensor_byte_size_MB(self, tensor):
         return (tensor.element_size() * tensor.nelement()) / (1024 * 1024)
 
     def print_tensor_sizes(self, file=sys.stdout):
         # Set to two decimal places
-        print('Tensor sizes:', file=file)
-        print('Actions:', self.get_tensor_byte_size_MB(self.actions), file=file)
-        print('Robot positions:', self.get_tensor_byte_size_MB(self.robot_positions), file=file)
-        print('Raw local maps:', self.get_tensor_byte_size_MB(self.raw_local_maps), file=file)
-        print('Raw obstacle maps:', self.get_tensor_byte_size_MB(self.raw_obstacle_maps), file=file)
-        print('Local maps:', self.get_tensor_byte_size_MB(self.local_maps), file=file)
-        print('Obstacle maps:', self.get_tensor_byte_size_MB(self.obstacle_maps), file=file)
-        print('Comm maps:', self.get_tensor_byte_size_MB(self.comm_maps), file=file)
-        print('Coverage features:', self.get_tensor_byte_size_MB(self.coverage_features), file=file)
+        print("Tensor sizes:", file=file)
+        print("Actions:", self.get_tensor_byte_size_MB(self.actions), file=file)
+        print(
+            "Robot positions:",
+            self.get_tensor_byte_size_MB(self.robot_positions),
+            file=file,
+        )
+        print(
+            "Raw local maps:",
+            self.get_tensor_byte_size_MB(self.raw_local_maps),
+            file=file,
+        )
+        print(
+            "Raw obstacle maps:",
+            self.get_tensor_byte_size_MB(self.raw_obstacle_maps),
+            file=file,
+        )
+        print("Local maps:", self.get_tensor_byte_size_MB(self.local_maps), file=file)
+        print(
+            "Obstacle maps:",
+            self.get_tensor_byte_size_MB(self.obstacle_maps),
+            file=file,
+        )
+        print("Comm maps:", self.get_tensor_byte_size_MB(self.comm_maps), file=file)
+        print(
+            "Coverage features:",
+            self.get_tensor_byte_size_MB(self.coverage_features),
+            file=file,
+        )
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     config_file = sys.argv[1]
+
     if len(sys.argv) > 2:
         append_folder = sys.argv[2]
     else:
         append_folder = None
     SimpleDatasetGenerator(config_file, append_folder)
```

### Comparing `coverage_control-1.1.0/python/scripts/evaluators/controller.py` & `coverage_control-1.2.0/python/coverage_control/algorithms/controllers.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,28 +14,30 @@
 # The CoverageControl library is distributed in the hope that it will be
 # useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General
 # Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # CoverageControl library. If not, see <https://www.gnu.org/licenses/>.
-
-## @file controller.py
+# @file controller.py
 #  @brief Base classes for CVT and neural network based controllers
-
 import coverage_control.nn as cc_nn
 import torch
-from coverage_control import CoverageSystem, IOUtils, Parameters, PointVector
-from coverage_control.algorithms import (
-    CentralizedCVT,
-    ClairvoyantCVT,
-    DecentralizedCVT,
-    NearOptimalCVT,
-)
-from coverage_control.nn import CoverageEnvUtils
+
+from . import CentralizedCVT
+from . import ClairvoyantCVT
+from . import DecentralizedCVT
+from . import NearOptimalCVT
+from .. import IOUtils
+from ..core import CoverageSystem
+from ..core import Parameters
+from ..core import PointVector
+from ..nn import CoverageEnvUtils
+
+__all__ = ["ControllerCVT", "ControllerNN"]
 
 
 class ControllerCVT:
     """
     Controller class for CVT based controllers
     """
```

### Comparing `coverage_control-1.1.0/python/scripts/evaluators/deprecated/eval_multi.py` & `coverage_control-1.2.0/python/scripts/evaluators/deprecated/eval_multi.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/scripts/evaluators/deprecated/eval_rf_exp.py` & `coverage_control-1.2.0/python/scripts/evaluators/deprecated/eval_rf_exp.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/scripts/evaluators/deprecated/eval_semantic_video.py` & `coverage_control-1.2.0/python/scripts/evaluators/deprecated/eval_semantic_video.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/scripts/evaluators/deprecated/eval_video.py` & `coverage_control-1.2.0/python/scripts/evaluators/deprecated/eval_video.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/scripts/evaluators/deprecated/semantic_eval.py` & `coverage_control-1.2.0/python/scripts/evaluators/deprecated/semantic_eval.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/scripts/evaluators/eval.py` & `coverage_control-1.2.0/python/tests/deprecated/data_generators/gnn_NoCNNmaps_data_generation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,163 +1,140 @@
-# This file is part of the CoverageControl library
-#
-# Author: Saurav Agarwal
-# Contact: sauravag@seas.upenn.edu, agr.saurav1@gmail.com
-# Repository: https://github.com/KumarRobotics/CoverageControl
-#
-# Copyright (c) 2024, Saurav Agarwal
-#
-# The CoverageControl library is free software: you can redistribute it and/or
-# modify it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or (at your
-# option) any later version.
-#
-# The CoverageControl library is distributed in the hope that it will be
-# useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General
-# Public License for more details.
-#
-# You should have received a copy of the GNU General Public License along with
-# CoverageControl library. If not, see <https://www.gnu.org/licenses/>.
-
-## @file eval.py
-#  @brief Evaluates the performance of the controllers on a set of environments
-
-import os
 import sys
-
-import coverage_control as cc
+import os
+import math
+import time
 import numpy as np
-from coverage_control import CoverageSystem, IOUtils, WorldIDF
-
-from controller import ControllerCVT, ControllerNN
-
-
-## @ingroup python_api
-class Evaluator:
-    """
-    Evaluates the performance of the controllers on a set of environments
-    """
-
-    def __init__(self, in_config):
-        self.config = in_config
-        self.eval_dir = IOUtils.sanitize_path(self.config["EvalDir"])
-        self.env_dir = IOUtils.sanitize_path(self.config["EnvironmentDataDir"])
-        self.controller_dir = None
-
-        if not os.path.exists(self.env_dir):
-            os.makedirs(self.env_dir)
-
-        self.num_controllers = len(self.config["Controllers"])
-        self.controllers_configs = self.config["Controllers"]
-
-        for controller_config in self.controllers_configs:
-            c_dir = self.eval_dir + "/" + controller_config["Name"]
-
-            if not os.path.exists(c_dir):
-                os.makedirs(c_dir)
-
-        self.env_config_file = IOUtils.sanitize_path(self.config["EnvironmentConfig"])
-        self.env_config = IOUtils.load_toml(self.env_config_file)
-        self.cc_params = cc.Parameters(self.env_config_file)
-
-        self.num_robots = self.cc_params.pNumRobots
-        self.num_features = self.cc_params.pNumFeatures
-        self.num_envs = self.config["NumEnvironments"]
-        self.num_steps = self.config["NumSteps"]
-
-    def evaluate(self, save=True):
-        dataset_count = 0
-        cost_data = np.zeros((self.num_controllers, self.num_envs, self.num_steps))
-
-        while dataset_count < self.num_envs:
-            print(f"Environment {dataset_count}")
-            pos_file = self.env_dir + "/" + str(dataset_count) + ".pos"
-            env_file = self.env_dir + "/" + str(dataset_count) + ".env"
-
-            if os.path.isfile(env_file) and os.path.isfile(pos_file):
-                world_idf = WorldIDF(self.cc_params, env_file)
-                env_main = CoverageSystem(self.cc_params, world_idf, pos_file)
-            else:
-                print(f"Creating new environment {dataset_count}")
-                env_main = CoverageSystem(
-                    self.cc_params, self.num_features, self.num_robots
-                )
-                env_main.WriteEnvironment(pos_file, env_file)
-                world_idf = env_main.GetWorldIDFObject()
-
-            robot_init_pos = env_main.GetRobotPositions(force_no_noise=True)
-
-            for controller_id in range(self.num_controllers):
-                step_count = 0
-                env = CoverageSystem(self.cc_params, world_idf, robot_init_pos)
-
-                # map_dir = self.eval_dir + "/" + self.controllers[controller_id]["Name"] + "/plots/"
-                # os.makedirs(map_dir, exist_ok = True)
-                # env.PlotInitMap(map_dir, "InitMap")
-                # env.RecordPlotData()
-                # env.PlotMapVoronoi(map_dir, step_count)
-
-                if self.controllers_configs[controller_id]["Type"] == "Learning":
-                    Controller = ControllerNN
-                else:
-                    Controller = ControllerCVT
-                controller = Controller(
-                    self.controllers_configs[controller_id], self.cc_params, env
-                )
-                initial_objective_value = env.GetObjectiveValue()
-                cost_data[controller_id, dataset_count, step_count] = (
-                    env.GetObjectiveValue() / initial_objective_value
-                )
-                step_count = step_count + 1
-
-                while step_count < self.num_steps:
-                    objective_value, converged = controller.step(env)
-                    cost_data[controller_id, dataset_count, step_count] = (
-                        objective_value / initial_objective_value
-                    )
-
-                    if converged:
-                        cost_data[controller_id, dataset_count, step_count:] = (
-                            objective_value / initial_objective_value
-                        )
-
+from sklearn.metrics import pairwise_distances as pwdist
+from scipy.optimize import linear_sum_assignment
+import pyCoverageControl # Main library
+from pyCoverageControl import Point2 # for defining points
+from pyCoverageControl import PointVector # for defining list of points
+from pyCoverageControl import CoverageSystem
+from pyCoverageControl import OracleGlobalOffline
+from multiprocessing import Pool
+from torchvision.transforms import Resize
+import torch
+import cv2
+from scipy.ndimage import gaussian_filter
+import matplotlib.pylab as plt
+import seaborn as sns
+
+class DataGenerator:
+
+    def __init__(self, params_filename='parameters.yaml', dataset_count=2500, num_gaussians=5, num_robots=15, new_sz=128, num_steps_per_dataset=1, stable_dataset_count=10):
+        self.params_ = pyCoverageControl.Parameters(params_filename)
+        self.dataset_count = dataset_count
+        self.num_gaussians = num_gaussians
+        self.num_robots = num_robots
+        self.new_sz = new_sz
+        self.num_steps_per_dataset = num_steps_per_dataset
+        self.stable_dataset_count = stable_dataset_count
+
+        self.compression_ratio = self.params_.pLocalMapSize/self.new_sz
+
+        self.coverage_count = 0
+
+        self.torch_coverage_features = torch.empty(self.dataset_count, self.num_robots, 7)
+        self.torch_robot_positions = torch.empty(self.dataset_count, self.num_robots, 2)
+        self.torch_actions = torch.empty(self.dataset_count, self.num_robots, 2)
+
+        self.env = CoverageSystem(self.params_, self.num_gaussians, self.num_robots)
+        self.oracle = OracleGlobalOffline(self.params_, self.num_robots, self.env)
+
+    def Step(self):
+        cont_flag = self.oracle.Step();
+        actions = self.oracle.GetActions()
+        error_flag = self.env.StepActions(actions)
+        return cont_flag, error_flag
+
+    def StepSave(self):
+        robot_positions = self.env.GetRobotPositions()
+        for i in range(0, self.num_robots):
+            self.torch_robot_positions[self.coverage_count, i] = torch.tensor(robot_positions[i])
+
+        voronoi_features = self.env.GetLocalVoronoiFeatures()
+
+        for i in range(0, self.num_robots):
+            self.torch_coverage_features[self.coverage_count, i] = torch.tensor(voronoi_features[i])
+
+        [cont_flag, error_flag] = self.Step()
+        goals = self.oracle.GetGoals()
+        actions = self.oracle.GetActions()
+        for i in range(0, self.num_robots):
+            self.torch_actions[self.coverage_count, i] = torch.tensor(actions[i])
+
+        return cont_flag
+
+    def GenerateDataset(self):
+        while self.coverage_count < self.dataset_count:
+            print("New environment")
+            num_steps = 0
+            self.env = CoverageSystem(self.params_, self.num_gaussians, self.num_robots)
+            print("Environment created")
+            self.oracle = OracleGlobalOffline(self.params_, self.num_robots, self.env)
+            print("Oracle initialized")
+
+            cont_flag = True
+            while num_steps < math.floor(self.params_.pEpisodeSteps/self.num_steps_per_dataset):
+                for i in range(0, self.num_steps_per_dataset - 1):
+                    [cont_flag, error_flag] = self.Step()
+                    if cont_flag == False:
                         break
-                    # env.PlotMapVoronoi(map_dir, step_count)
-                    # env.RecordPlotData()
-                    step_count = step_count + 1
-
-                    if step_count % 100 == 0:
-                        print(
-                            f"Step {step_count}, Objective Value {cost_data[controller_id, dataset_count, step_count - 1]}"
-                        )
-                        print(
-                            f"Environment {dataset_count}, {controller.name}, Step {step_count}"
-                        )
-
-                if save is True:
-                    self.controller_dir = (
-                        self.eval_dir
-                        + "/"
-                        + self.controllers_configs[controller_id]["Name"]
-                    )
-                    controller_data_file = self.controller_dir + "/" + "eval.csv"
-                    np.savetxt(
-                        controller_data_file,
-                        cost_data[controller_id, : dataset_count + 1, :],
-                        delimiter=",",
-                    )
-                # env.RenderRecordedMap(self.eval_dir + "/" + self.controllers[controller_id]["Name"] + "/", "video.mp4")
-                del controller
-                del env
-            dataset_count = dataset_count + 1
-
-        return cost_data
-
-
-if __name__ == "__main__":
+                if cont_flag == False:
+                    break
 
-    config_file = sys.argv[1]
-    config = IOUtils.load_toml(config_file)
+                cont_flag = self.StepSave()
+                self.coverage_count = self.coverage_count + 1
+                num_steps = num_steps + 1
+                print(str(self.coverage_count), str(num_steps))
+                if not(self.coverage_count < self.dataset_count):
+                    break
+            for i in range(0, self.stable_dataset_count):
+                if not(self.coverage_count < self.dataset_count):
+                    break
+                cont_flag = self.StepSave()
+
+    def NormalizeTensor(self, tensor_data):
+        mean = tensor_data.mean(dim=(0,1))
+        std = tensor_data.std(dim=(0,1))
+        normalized_tensor_data = (tensor_data - mean)/std
+        return mean, std, normalized_tensor_data
+
+    def SaveDatasetSubset(self, dir_name='gnn/train', start_idx=0, end_idx=0):
+        torch.save(self.normalized_torch_coverage_features[start_idx:end_idx].clone(), dir_name + '/coverage_features.pt')
+        torch.save(self.torch_robot_positions[start_idx:end_idx].clone(), dir_name + '/robot_positions.pt')
+        torch.save(self.normalized_torch_actions[start_idx:end_idx].clone(), dir_name + '/actions.pt')
+
+    def SaveDataset(self, dir_name='gnn'):
+        if not os.path.exists(dir_name):
+            os.makedirs(dir_name)
+        if not os.path.exists(dir_name + '/train'):
+            os.makedirs(dir_name + '/train')
+        if not os.path.exists(dir_name + '/val'):
+            os.makedirs(dir_name + '/val')
+        if not os.path.exists(dir_name + '/test'):
+            os.makedirs(dir_name + '/test')
+
+        coverage_features_mean, coverage_features_std, self.normalized_torch_coverage_features = self.NormalizeTensor(self.torch_coverage_features)
+        torch.save(coverage_features_mean, dir_name + '/coverage_features_mean.pt')
+        torch.save(coverage_features_std, dir_name + '/coverage_features_std.pt')
+
+        actions_mean, actions_std, self.normalized_torch_actions = self.NormalizeTensor(self.torch_actions)
+        torch.save(actions_mean, dir_name + '/actions_mean.pt')
+        torch.save(actions_std, dir_name + '/actions_std.pt')
+
+        val_idx = int(0.7 * self.dataset_count)
+        test_idx = val_idx + int(0.2 * self.dataset_count)
+        self.SaveDatasetSubset(dir_name + '/train', 0, val_idx)
+        self.SaveDatasetSubset(dir_name + '/val', val_idx, test_idx)
+        self.SaveDatasetSubset(dir_name + '/test', test_idx, self.dataset_count)
+
+if __name__ == '__main__':
+    params_filename = 'parameters.yaml'
+    dataset_count = 1000
+    num_gaussians = 5
+    num_robots = 15
+
+    gen = DataGenerator(params_filename, dataset_count, num_gaussians, num_robots)
+    gen.GenerateDataset()
+    gen.SaveDataset('gnn_NoCNNmaps/')
 
-    evaluator = Evaluator(config)
-    evaluator.evaluate()
```

### Comparing `coverage_control-1.1.0/python/scripts/evaluators/eval_single_env.py` & `coverage_control-1.2.0/python/scripts/evaluators/eval.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,154 +1,143 @@
-# This file is part of the CoverageControl library
-#
-# Author: Saurav Agarwal
-# Contact: sauravag@seas.upenn.edu, agr.saurav1@gmail.com
-# Repository: https://github.com/KumarRobotics/CoverageControl
-#
-# Copyright (c) 2024, Saurav Agarwal
-#
-# The CoverageControl library is free software: you can redistribute it and/or
-# modify it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or (at your
-# option) any later version.
-#
-# The CoverageControl library is distributed in the hope that it will be
-# useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General
-# Public License for more details.
-#
-# You should have received a copy of the GNU General Public License along with
-# CoverageControl library. If not, see <https://www.gnu.org/licenses/>.
-
-## @file eval_single_env.py
-#  @brief Evaluate a single dataset with multiple controllers
-
+# @file eval.py
+#  @brief Evaluates the performance of the controllers on a set of environments
 import os
 import sys
 
 import coverage_control as cc
 import numpy as np
-from coverage_control import CoverageSystem, IOUtils, WorldIDF
-
-from controller import ControllerCVT, ControllerNN
+from coverage_control import CoverageSystem
+from coverage_control import IOUtils
+from coverage_control import WorldIDF
+from coverage_control.algorithms import ControllerCVT
+from coverage_control.algorithms import ControllerNN
 
 
-## @ingroup python_api
-class EvaluatorSingle:
+# @ingroup python_api
+class Evaluator:
     """
-    Class to evaluate a single environment with multiple controllers
+    Evaluates the performance of the controllers on a set of environments
     """
 
     def __init__(self, in_config):
         self.config = in_config
-        self.eval_dir = IOUtils.sanitize_path(self.config["EvalDir"]) + "/"
-        self.env_dir = IOUtils.sanitize_path(self.config["EnvironmentDataDir"]) + "/"
-        self.feature_file = self.env_dir + self.config["FeatureFile"]
-        self.pos_file = self.env_dir + self.config["RobotPosFile"]
+        self.eval_dir = IOUtils.sanitize_path(self.config["EvalDir"])
+        self.env_dir = IOUtils.sanitize_path(self.config["EnvironmentDataDir"])
+        self.controller_dir = None
 
         if not os.path.exists(self.env_dir):
             os.makedirs(self.env_dir)
 
-        if not os.path.exists(self.feature_file):
-            raise ValueError(f"Feature file {self.feature_file} does not exist")
-
-        if not os.path.exists(self.pos_file):
-            raise ValueError(f"Robot position file {self.pos_file} does not exist")
-
         self.num_controllers = len(self.config["Controllers"])
         self.controllers_configs = self.config["Controllers"]
 
+        for controller_config in self.controllers_configs:
+            c_dir = self.eval_dir + "/" + controller_config["Name"]
+
+            if not os.path.exists(c_dir):
+                os.makedirs(c_dir)
+
         self.env_config_file = IOUtils.sanitize_path(self.config["EnvironmentConfig"])
         self.env_config = IOUtils.load_toml(self.env_config_file)
         self.cc_params = cc.Parameters(self.env_config_file)
 
         self.num_robots = self.cc_params.pNumRobots
         self.num_features = self.cc_params.pNumFeatures
+        self.num_envs = self.config["NumEnvironments"]
         self.num_steps = self.config["NumSteps"]
 
-        self.plot_map = self.config["PlotMap"]
-        self.generate_video = self.config["GenerateVideo"]
-
     def evaluate(self, save=True):
-        cost_data = np.zeros((self.num_controllers, self.num_steps))
-        world_idf = WorldIDF(self.cc_params, self.feature_file)
-        env_main = CoverageSystem(self.cc_params, world_idf, self.pos_file)
-        robot_init_pos = env_main.GetRobotPositions(force_no_noise=True)
-
-        if self.plot_map:
-            map_dir = self.eval_dir + "/plots/"
-            os.makedirs(map_dir, exist_ok=True)
-            env_main.PlotInitMap(map_dir, "InitMap")
-
-        for controller_id in range(self.num_controllers):
-            step_count = 0
-            env = CoverageSystem(self.cc_params, world_idf, robot_init_pos)
-            controller_name = self.controllers_configs[controller_id]["Name"]
-
-            if self.generate_video:
-                env.RecordPlotData()
+        dataset_count = 0
+        cost_data = np.zeros((self.num_controllers, self.num_envs, self.num_steps))
 
-            if self.controllers_configs[controller_id]["Type"] == "Learning":
-                Controller = ControllerNN
+        while dataset_count < self.num_envs:
+            print(f"Environment {dataset_count}")
+            pos_file = self.env_dir + "/" + str(dataset_count) + ".pos"
+            env_file = self.env_dir + "/" + str(dataset_count) + ".env"
+
+            if os.path.isfile(env_file) and os.path.isfile(pos_file):
+                world_idf = WorldIDF(self.cc_params, env_file)
+                env_main = CoverageSystem(self.cc_params, world_idf, pos_file)
             else:
-                Controller = ControllerCVT
-            controller = Controller(
-                self.controllers_configs[controller_id], self.cc_params, env
-            )
-            initial_objective_value = env.GetObjectiveValue()
-            cost_data[controller_id, step_count] = (
-                env.GetObjectiveValue() / initial_objective_value
-            )
-            step_count = step_count + 1
-
-            while step_count < self.num_steps:
-                objective_value, converged = controller.step(env)
-                cost_data[controller_id, step_count] = (
-                    objective_value / initial_objective_value
+                print(f"Creating new environment {dataset_count}")
+                env_main = CoverageSystem(
+                    self.cc_params, self.num_features, self.num_robots
                 )
+                env_main.WriteEnvironment(pos_file, env_file)
+                world_idf = env_main.GetWorldIDFObject()
 
-                if converged and not self.generate_video:
-                    cost_data[controller_id, step_count:] = (
-                        objective_value / initial_objective_value
-                    )
-
-                    break
-
-                if self.generate_video:
-                    env.RecordPlotData()
+            robot_init_pos = env_main.GetRobotPositions(force_no_noise=True)
 
+            for controller_id in range(self.num_controllers):
+                step_count = 0
+                env = CoverageSystem(self.cc_params, world_idf, robot_init_pos)
+
+                # map_dir = self.eval_dir + "/" + self.controllers[controller_id]["Name"] + "/plots/"
+                # os.makedirs(map_dir, exist_ok = True)
+                # env.PlotInitMap(map_dir, "InitMap")
+                # env.RecordPlotData()
+                # env.PlotMapVoronoi(map_dir, step_count)
+
+                if self.controllers_configs[controller_id]["Type"] == "Learning":
+                    Controller = ControllerNN
+                else:
+                    Controller = ControllerCVT
+                controller = Controller(
+                    self.controllers_configs[controller_id], self.cc_params, env
+                )
+                initial_objective_value = env.GetObjectiveValue()
+                cost_data[controller_id, dataset_count, step_count] = (
+                    env.GetObjectiveValue() / initial_objective_value
+                )
                 step_count = step_count + 1
 
-                if step_count % 100 == 0:
-                    print(
-                        f"Step {step_count}, Objective Value {cost_data[controller_id, step_count - 1]}"
+                while step_count < self.num_steps:
+                    objective_value, converged = controller.step(env)
+                    cost_data[controller_id, dataset_count, step_count] = (
+                        objective_value / initial_objective_value
                     )
-                    print(f"{controller.name}, Step {step_count}")
-
-            if save is True:
-                controller_dir = self.eval_dir + "/" + controller_name
-
-                if not os.path.exists(controller_dir):
-                    os.makedirs(controller_dir)
 
-                controller_data_file = controller_dir + "/" + "eval.csv"
-                np.savetxt(
-                    controller_data_file, cost_data[controller_id, :], delimiter=","
-                )
-
-            if self.generate_video:
-                controller_dir = self.eval_dir + "/" + controller_name
-                env.RenderRecordedMap(controller_dir, "video.mp4")
-
-            del controller
-            del env
+                    if converged:
+                        cost_data[controller_id, dataset_count, step_count:] = (
+                            objective_value / initial_objective_value
+                        )
+
+                        break
+                    # env.PlotMapVoronoi(map_dir, step_count)
+                    # env.RecordPlotData()
+                    step_count = step_count + 1
+
+                    if step_count % 100 == 0:
+                        val = cost_data[controller_id, dataset_count, step_count - 1]
+                        print(
+                            f"Environment {dataset_count} "
+                            f"{controller.name} "
+                            f"Step {step_count} "
+                            f"Objective Value {val}"
+                        )
+
+                if save is True:
+                    self.controller_dir = (
+                        self.eval_dir
+                        + "/"
+                        + self.controllers_configs[controller_id]["Name"]
+                    )
+                    controller_data_file = self.controller_dir + "/" + "eval.csv"
+                    np.savetxt(
+                        controller_data_file,
+                        cost_data[controller_id, : dataset_count + 1, :],
+                        delimiter=",",
+                    )
+                # env.RenderRecordedMap(self.eval_dir + "/" + self.controllers[controller_id]["Name"] + "/", "video.mp4")
+                del controller
+                del env
+            dataset_count = dataset_count + 1
 
         return cost_data
 
 
 if __name__ == "__main__":
-
     config_file = sys.argv[1]
     config = IOUtils.load_toml(config_file)
 
-    evaluator = EvaluatorSingle(config)
+    evaluator = Evaluator(config)
     evaluator.evaluate()
```

### Comparing `coverage_control-1.1.0/python/scripts/training/train_cnn.py` & `coverage_control-1.2.0/python/scripts/training/train_lpac.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,107 +1,103 @@
-#  This file is part of the CoverageControl library
-#
-#  Author: Saurav Agarwal
-#  Contact: sauravag@seas.upenn.edu, agr.saurav1@gmail.com
-#  Repository: https://github.com/KumarRobotics/CoverageControl
-#
-#  Copyright (c) 2024, Saurav Agarwal
-#
-#  The CoverageControl library is free software: you can redistribute it and/or
-#  modify it under the terms of the GNU General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or (at your
-#  option) any later version.
-#
-#  The CoverageControl library is distributed in the hope that it will be
-#  useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General
-#  Public License for more details.
-#
-#  You should have received a copy of the GNU General Public License along with
-#  CoverageControl library. If not, see <https://www.gnu.org/licenses/>.
+"""
+Train the LPAC model
+"""
 
+# @file train_lpac.py
+#  @brief Train the LPAC model
 import os
 import pathlib
 import sys
 
 import torch
 import torch_geometric
 from coverage_control import IOUtils
-from coverage_control.nn import CNN, LocalMapCNNDataset, TrainModel
+from coverage_control.nn import CNNGNNDataset
+from coverage_control.nn import LPAC
+from coverage_control.nn import TrainModel
 
 # Set the device
-device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
 
 config_file = sys.argv[1]
+world_size = int(sys.argv[2])
 config = IOUtils.load_toml(config_file)
 num_workers = config["NumWorkers"]
 dataset_path = pathlib.Path(IOUtils.sanitize_path(config["DataDir"]))
 data_dir = dataset_path / "data/"
 
-cnn_model = config["CNNModel"]
-model_dir = IOUtils.sanitize_path(cnn_model["Dir"]) + "/"
+lpac_model = config["LPACModel"]
+model_dir = IOUtils.sanitize_path(lpac_model["Dir"]) + "/"
 
 if not os.path.exists(model_dir):
     os.makedirs(model_dir)
 
-model_file = model_dir + cnn_model["Model"]
-optimizer_file = model_dir + cnn_model["Optimizer"]
+model_file = model_dir + lpac_model["Model"]
+optimizer_file = model_dir + lpac_model["Optimizer"]
 
-training_config = config["CNNTraining"]
+training_config = config["LPACTraining"]
 batch_size = training_config["BatchSize"]
 num_epochs = training_config["NumEpochs"]
 learning_rate = training_config["LearningRate"]
-momentum = training_config["Momentum"]
+# momentum = training_config["Momentum"]
 weight_decay = training_config["WeightDecay"]
-output_dim = config["CNNBackBone"]["OutputDim"]
 
 use_comm_map = config["ModelConfig"]["UseCommMaps"]
-cnn_config = config["CNNBackBone"]
 
-model = CNN(cnn_config).to(device)
+model = LPAC(config).to(device)
 
-train_dataset = LocalMapCNNDataset(str(data_dir), "train", use_comm_map, output_dim)
-val_dataset = LocalMapCNNDataset(str(data_dir), "val", use_comm_map, output_dim)
-test_dataset = LocalMapCNNDataset(str(data_dir), "test", use_comm_map, output_dim)
+# cnn_pretrained_model = config["CNNModel"]["Dir"] + config["CNNModel"]["Model"]
+# model.LoadCNNBackBone(cnn_pretrained_model)
 
-model.register_buffer("target_mean", train_dataset.targets_mean)
-model.register_buffer("target_Std", train_dataset.targets_std)
+if "PreTrainedModel" in config["LPACModel"]:
+    lpac_pretrained_model = (
+        IOUtils.sanitize_path(config["LPACModel"]["Dir"])
+        + config["LPACModel"]["PreTrainedModel"]
+    )
+    model.load_model(lpac_pretrained_model)
+
+train_dataset = CNNGNNDataset(data_dir, "train", use_comm_map, world_size)
+val_dataset = CNNGNNDataset(data_dir, "val", use_comm_map, world_size)
+
+# for model in models:
+model.register_buffer("actions_mean", train_dataset.targets_mean)
+model.register_buffer("actions_std", train_dataset.targets_std)
 
 print("Loaded datasets")
 print(f"Train dataset size: {len(train_dataset)}")
 
-train_loader = torch.utils.data.DataLoader(
+train_loader = torch_geometric.loader.DataLoader(
     train_dataset, batch_size=batch_size, shuffle=True, num_workers=num_workers
 )
-val_loader = torch.utils.data.DataLoader(
+val_loader = torch_geometric.loader.DataLoader(
     val_dataset, batch_size=batch_size, shuffle=False, num_workers=num_workers
 )
-test_loader = torch.utils.data.DataLoader(
-    test_dataset, batch_size=batch_size, shuffle=False, num_workers=num_workers
-)
 
-optimizer = torch.optim.SGD(
-    model.parameters(), lr=learning_rate, momentum=momentum, weight_decay=weight_decay
+# optimizer = torch.optim.SGD(model.parameters(), lr=learning_rate, momentum=momentum, weight_decay=weight_decay)
+optimizer = torch.optim.Adam(
+    model.parameters(), lr=learning_rate, weight_decay=weight_decay
 )
 
 # Use mse loss for regression
 criterion = torch.nn.MSELoss()
 
 trainer = TrainModel(
     model,
     train_loader,
-    val_loader,
+    None,
     optimizer,
     criterion,
     num_epochs,
     device,
     model_file,
     optimizer_file,
 )
-# trainer.LoadSavedModel(model_file)
-# trainer.LoadSavedOptimizer(optimizer_file)
+# trainer = TrainModel(model, train_loader, val_loader, optimizer, criterion, num_epochs, device, model_file, optimizer_file)
+# trainer.load_saved_model(model_file)
+# trainer.load_saved_optimizer(optimizer_file)
 
 trainer.train()
 
-test_loss = trainer.Test()
-torch.save(test_loss, model_dir + "/test_loss.pt")
-print(f"Test loss: {test_loss}")
+# test_dataset = CNNGNNDataset(data_dir, "test", use_comm_map, world_size)
+# test_loader = torch_geometric.loader.DataLoader(test_dataset, batch_size=batch_size, shuffle=False, num_workers=24)
+# test_loss = trainer.Test(test_loader)
+# print(f"Test loss: {test_loss}")
```

### Comparing `coverage_control-1.1.0/python/tests/deprecated/data_generators/cnn_data_generation.py` & `coverage_control-1.2.0/python/tests/deprecated/data_generators/cnn_data_generation.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/tests/deprecated/data_generators/cnn_data_generation_NoCommsMap.py` & `coverage_control-1.2.0/python/tests/deprecated/data_generators/cnn_data_generation_NoCommsMap.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/tests/deprecated/data_generators/dense_gnn_NoCommMaps_data_generation.py` & `coverage_control-1.2.0/python/tests/deprecated/data_generators/dense_gnn_NoCommMaps_data_generation.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/tests/deprecated/data_generators/dense_gnn_data_generation.py` & `coverage_control-1.2.0/python/tests/deprecated/data_generators/dense_gnn_data_generation.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/tests/deprecated/data_generators/gnn_NoCNNmaps_data_generation.py` & `coverage_control-1.2.0/python/tests/deprecated/data_generators/sparse_gnn_data_generation.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,14 +28,17 @@
         self.new_sz = new_sz
         self.num_steps_per_dataset = num_steps_per_dataset
         self.stable_dataset_count = stable_dataset_count
 
         self.compression_ratio = self.params_.pLocalMapSize/self.new_sz
 
         self.coverage_count = 0
+        self.sparse_coverage_maps = []
+
+        self.sparse_comm_maps = []
 
         self.torch_coverage_features = torch.empty(self.dataset_count, self.num_robots, 7)
         self.torch_robot_positions = torch.empty(self.dataset_count, self.num_robots, 2)
         self.torch_actions = torch.empty(self.dataset_count, self.num_robots, 2)
 
         self.env = CoverageSystem(self.params_, self.num_gaussians, self.num_robots)
         self.oracle = OracleGlobalOffline(self.params_, self.num_robots, self.env)
@@ -46,36 +49,46 @@
         error_flag = self.env.StepActions(actions)
         return cont_flag, error_flag
 
     def StepSave(self):
         robot_positions = self.env.GetRobotPositions()
         for i in range(0, self.num_robots):
             self.torch_robot_positions[self.coverage_count, i] = torch.tensor(robot_positions[i])
-
         voronoi_features = self.env.GetLocalVoronoiFeatures()
-
+        data_coverage_maps = []
+        data_comm_maps = []
         for i in range(0, self.num_robots):
+            local_map = self.env.GetRobotLocalMap(i)
+            lmap = cv2.resize(local_map, dsize=(self.new_sz,self.new_sz), interpolation=cv2.INTER_AREA)
+            data_coverage_maps.append(torch.tensor(lmap).to_sparse_csr())
+
+            comm_map = self.env.GetCommunicationMap(i)
+            comm_map = torch.tensor(gaussian_filter(comm_map, sigma=(3,3), order=0))
+            comm_map = cv2.resize(np.array(comm_map), dsize=(self.new_sz, self.new_sz), interpolation=cv2.INTER_AREA)
+            data_comm_maps.append(torch.tensor(comm_map).to_sparse_csr())
+
             self.torch_coverage_features[self.coverage_count, i] = torch.tensor(voronoi_features[i])
 
+        self.sparse_coverage_maps.append(data_coverage_maps)
+        self.sparse_comm_maps.append(data_comm_maps)
+
         [cont_flag, error_flag] = self.Step()
         goals = self.oracle.GetGoals()
         actions = self.oracle.GetActions()
         for i in range(0, self.num_robots):
             self.torch_actions[self.coverage_count, i] = torch.tensor(actions[i])
 
         return cont_flag
 
     def GenerateDataset(self):
         while self.coverage_count < self.dataset_count:
             print("New environment")
             num_steps = 0
             self.env = CoverageSystem(self.params_, self.num_gaussians, self.num_robots)
-            print("Environment created")
             self.oracle = OracleGlobalOffline(self.params_, self.num_robots, self.env)
-            print("Oracle initialized")
 
             cont_flag = True
             while num_steps < math.floor(self.params_.pEpisodeSteps/self.num_steps_per_dataset):
                 for i in range(0, self.num_steps_per_dataset - 1):
                     [cont_flag, error_flag] = self.Step()
                     if cont_flag == False:
                         break
@@ -90,22 +103,24 @@
                     break
             for i in range(0, self.stable_dataset_count):
                 if not(self.coverage_count < self.dataset_count):
                     break
                 cont_flag = self.StepSave()
 
     def NormalizeTensor(self, tensor_data):
-        mean = tensor_data.mean(dim=(0,1))
-        std = tensor_data.std(dim=(0,1))
+        mean = tensor_data.mean(dim=(0, 1))
+        std = tensor_data.std(dim=(0, 1))
         normalized_tensor_data = (tensor_data - mean)/std
         return mean, std, normalized_tensor_data
 
     def SaveDatasetSubset(self, dir_name='gnn/train', start_idx=0, end_idx=0):
-        torch.save(self.normalized_torch_coverage_features[start_idx:end_idx].clone(), dir_name + '/coverage_features.pt')
+        torch.save(self.sparse_coverage_maps[start_idx:end_idx].clone(), dir_name + '/sparse_coverage_maps.pt')
         torch.save(self.torch_robot_positions[start_idx:end_idx].clone(), dir_name + '/robot_positions.pt')
+        torch.save(self.sparse_comm_maps[start_idx:end_idx], dir_name + '/sparse_comm_maps.pt')
+        torch.save(self.normalized_torch_coverage_features[start_idx:end_idx].clone(), dir_name + '/coverage_features.pt')
         torch.save(self.normalized_torch_actions[start_idx:end_idx].clone(), dir_name + '/actions.pt')
 
     def SaveDataset(self, dir_name='gnn'):
         if not os.path.exists(dir_name):
             os.makedirs(dir_name)
         if not os.path.exists(dir_name + '/train'):
             os.makedirs(dir_name + '/train')
@@ -126,15 +141,17 @@
         test_idx = val_idx + int(0.2 * self.dataset_count)
         self.SaveDatasetSubset(dir_name + '/train', 0, val_idx)
         self.SaveDatasetSubset(dir_name + '/val', val_idx, test_idx)
         self.SaveDatasetSubset(dir_name + '/test', test_idx, self.dataset_count)
 
 if __name__ == '__main__':
     params_filename = 'parameters.yaml'
-    dataset_count = 1000
-    num_gaussians = 5
-    num_robots = 15
-
-    gen = DataGenerator(params_filename, dataset_count, num_gaussians, num_robots)
-    gen.GenerateDataset()
-    gen.SaveDataset('gnn_NoCNNmaps/')
+    num_datasets = 5
+    for i in range(0, num_datasets):
+        dataset_count = 1000
+        num_gaussians = 5
+        num_robots = 15
+
+        gen = DataGenerator(params_filename, dataset_count, num_gaussians, num_robots)
+        gen.GenerateDataset()
+        gen.SaveDataset('gnn/' + str(i) + '/')
```

### Comparing `coverage_control-1.1.0/python/tests/deprecated/data_generators/sparse_gnn_NoCommsMap_data_generation.py` & `coverage_control-1.2.0/python/tests/deprecated/data_generators/sparse_gnn_NoCommsMap_data_generation.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/tests/deprecated/gnn.py` & `coverage_control-1.2.0/python/tests/deprecated/gnn.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/tests/deprecated/gnn_dist.py` & `coverage_control-1.2.0/python/tests/deprecated/gnn_dist.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/tests/deprecated/mlp_test.py` & `coverage_control-1.2.0/python/tests/deprecated/mlp_test.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/tests/deprecated/test_cnn.py` & `coverage_control-1.2.0/python/tests/deprecated/test_cnn.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/tests/deprecated/test_library_objects.py` & `coverage_control-1.2.0/python/tests/deprecated/test_library_objects.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/tests/deprecated/test_lpac_coverage.py` & `coverage_control-1.2.0/python/tests/deprecated/test_lpac_coverage.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/tests/deprecated/testplot.py` & `coverage_control-1.2.0/python/tests/deprecated/testplot.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/tests/deprecated/torch_compat.py` & `coverage_control-1.2.0/python/tests/deprecated/torch_compat.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/tests/test_coverage.py` & `coverage_control-1.2.0/python/tests/test_coverage.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/tests/test_coverage_env_utils.py` & `coverage_control-1.2.0/python/tests/test_coverage_env_utils.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/tests/test_env_io.py` & `coverage_control-1.2.0/python/tests/test_env_io.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/tests/test_map_generation.py` & `coverage_control-1.2.0/python/tests/test_map_generation.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/tests/test_models.py` & `coverage_control-1.2.0/python/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/tests/test_parameters.py` & `coverage_control-1.2.0/python/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/tests/test_parity.py` & `coverage_control-1.2.0/python/tests/test_parity.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/ts_jit/TorchVisionResize_32.pt` & `coverage_control-1.2.0/python/ts_jit/TorchVisionResize_32.pt`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/ts_jit/gnn_backbone.py` & `coverage_control-1.2.0/python/ts_jit/gnn_backbone.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/ts_jit/torchvision_resize.py` & `coverage_control-1.2.0/python/ts_jit/torchvision_resize.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/utils/dataset_utils.py` & `coverage_control-1.2.0/python/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/utils/generate_video.py` & `coverage_control-1.2.0/python/utils/generate_video.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/python/utils/save_gnn_params.py` & `coverage_control-1.2.0/python/utils/save_gnn_params.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/setup.sh` & `coverage_control-1.2.0/setup.sh`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/setup_utils/check_headers.sh` & `coverage_control-1.2.0/setup_utils/check_headers.sh`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/setup_utils/docker/base_images/.bashrc` & `coverage_control-1.2.0/setup_utils/docker/base_images/.bashrc`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/setup_utils/docker/base_images/.ros.bashrc` & `coverage_control-1.2.0/setup_utils/docker/base_images/.ros.bashrc`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/setup_utils/docker/base_images/build_all_images.sh` & `coverage_control-1.2.0/setup_utils/docker/base_images/build_all_images.sh`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/setup_utils/docker/base_images/ubuntu22.04-cuda-ros2.Dockerfile` & `coverage_control-1.2.0/setup_utils/docker/base_images/ubuntu22.04-cuda-ros2.Dockerfile`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/setup_utils/docker/base_images/ubuntu22.04-cuda.Dockerfile` & `coverage_control-1.2.0/setup_utils/docker/base_images/ubuntu22.04-cuda.Dockerfile`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/setup_utils/docker/base_images/ubuntu22.04-ros2.Dockerfile` & `coverage_control-1.2.0/setup_utils/docker/base_images/ubuntu22.04-ros2.Dockerfile`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/setup_utils/docker/base_images/ubuntu22.04.Dockerfile` & `coverage_control-1.2.0/setup_utils/docker/base_images/ubuntu22.04.Dockerfile`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/setup_utils/docker/create_container.sh` & `coverage_control-1.2.0/setup_utils/docker/create_container.sh`

 * *Files 12% similar despite different names*

```diff
@@ -36,23 +36,23 @@
 else
 	VOLUME_OPTION="-v ${WS_DIR}:${CONTAINER_CC_WS}:rw"
 fi
 
 if [[ ${CUDA_IMAGE} == true ]]; then
 	CONTAINER_OPTIONS+="--gpus all "
 	if [[ ${ROS_IMAGE} == true ]]; then
-		IMAGE_TAG="pytorch2.2.1-cuda12.3.1-ros2humble"
+		IMAGE_TAG="pytorch2.2.2-cuda12.2.2-ros2humble"
 	else
-		IMAGE_TAG="pytorch2.2.1-cuda12.3.1"
+		IMAGE_TAG="pytorch2.2.2-cuda12.2.2"
 	fi
 else
 	if [[ ${ROS_IMAGE} == true ]]; then
-		IMAGE_TAG="pytorch2.2.1-ros2humble"
+		IMAGE_TAG="pytorch2.2.2-ros2humble"
 	else
-		IMAGE_TAG="pytorch2.2.1"
+		IMAGE_TAG="pytorch2.2.2"
 	fi
 fi
 
 IMAGE_NAME="${IMAGE_BASE_NAME}:${IMAGE_TAG}"
 
 if [ -z ${CONTAINER_NAME} ]; then
 	CONTAINER_NAME="coverage-control-${USER}"
```

### Comparing `coverage_control-1.1.0/setup_utils/install_dependencies.sh` & `coverage_control-1.2.0/setup_utils/install_dependencies.sh`

 * *Files 0% similar despite different names*

```diff
@@ -75,21 +75,21 @@
 		echo "geographiclib install failed"
 		exit 1
 	fi
 }
 
 InstallPybind11 () {
 	echo "Setting up pybind11"
-	wget --tries=4 https://github.com/pybind/pybind11/archive/refs/tags/v2.11.1.tar.gz -P ${MAIN_DIR}/src
+	wget --tries=4 https://github.com/pybind/pybind11/archive/refs/tags/v2.12.0.tar.gz -P ${MAIN_DIR}/src
   if [ $? -ne 0 ]; then
     echo "Failed to download pybind11"
     exit 1
   fi
-	tar -xf ${MAIN_DIR}/src/v2.11.1.tar.gz -C ${MAIN_DIR}/src/
-	cmake -S ${MAIN_DIR}/src/pybind11-2.11.1 -B ${BUILD_DIR}/pybind11 -DPYBIND11_TEST=OFF ${CMAKE_END_FLAGS}
+	tar -xf ${MAIN_DIR}/src/v2.12.0.tar.gz -C ${MAIN_DIR}/src/
+	cmake -S ${MAIN_DIR}/src/pybind11-2.12.0 -B ${BUILD_DIR}/pybind11 -DPYBIND11_TEST=OFF ${CMAKE_END_FLAGS}
 	cmake --build ${BUILD_DIR}/pybind11 -j$(nproc)
 	cmake --install ${BUILD_DIR}/pybind11
 	if [ $? -eq 0 ]; then
 		echo "pybind11 install succeeded"
 	else
 		echo "pybind11 install failed"
 		exit 1
```

### Comparing `coverage_control-1.1.0/setup_utils/install_libtorch.sh` & `coverage_control-1.2.0/setup_utils/install_libtorch.sh`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/setup_utils/manylinux_2_28_before-all.sh` & `coverage_control-1.2.0/setup_utils/manylinux_2_28_before-all.sh`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/setup_utils/noxfile.py` & `coverage_control-1.2.0/setup_utils/noxfile.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.1.0/PKG-INFO` & `coverage_control-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coverage_control
-Version: 1.1.0
+Version: 1.2.0
 Summary: Library for large-scale coverage control using robot swarms
 Author-Email: Saurav Agarwal <agr.saurav1@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -709,25 +709,24 @@
 
 See full documentation at [https://KumarRobotics.github.io/CoverageControl/](https://KumarRobotics.github.io/CoverageControl/)
 
 ## Introduction
 
 Coverage control is the problem of navigating a robot swarm to collaboratively monitor features or a phenomenon of interest not known _a priori_.
 The library provides a simulation environment, algorithms, and GNN-based architectures for the coverage control problem.  
-<img align="right" width="300" src="https://github.com/KumarRobotics/CoverageControl/raw/main/doc/graphics/LPAC.gif">
+<img align="right" width="300" src="https://kumarrobotics.github.io/CoverageControl/LPAC.gif">
 
 **Key features:**  
 - The core library is written in `C++` and `CUDA` to handle large-scale simulations
 - There are `python` bindings that interface with the core library
 - Several Centroidal Voronoi Tessellation (CVT)-based algorithms (aka Lloyd's algorithms)
 - Learnable Perception-Action-Communication (LPAC) architecture for the coverage control problem is implemented in `PyTorch` and `PyTorch Geometric`
-- GPU and CPU parallelization using `CUDA` and `OpenMP`
 
 ---
-## Quick Start
+## Getting Started
 The library is available as a `pip` package. To install the package, run the following command:
 ```bash
 pip install coverage_control
 ```
 
 See [Installation](https://kumarrobotics.github.io/CoverageControl/installation.html) for more details on installation.
```


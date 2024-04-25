# Comparing `tmp/swiftest-2024.4.1.tar.gz` & `tmp/swiftest-2024.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftest-2024.4.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "swiftest-2024.4.2.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `swiftest-2024.4.1.tar` & `swiftest-2024.4.2.tar`

### file list

```diff
@@ -1,238 +1,242 @@
--rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 swiftest-2024.4.1/.dockerignore
--rw-r--r--   0        0        0     1414 2022-11-09 12:37:21.000000 swiftest-2024.4.1/.github/workflows/build_wheels.yml
--rw-r--r--   0        0        0      554 2022-11-09 12:37:21.000000 swiftest-2024.4.1/.github/workflows/build_wheels_debug.yml
--rw-r--r--   0        0        0     1104 2022-11-09 12:37:21.000000 swiftest-2024.4.1/.gitignore
--rw-r--r--   0        0        0      684 2022-11-09 12:37:21.000000 swiftest-2024.4.1/.readthedocs.yaml
--rw-r--r--   0        0        0     1916 2022-11-09 12:37:21.000000 swiftest-2024.4.1/.zenodo.json
--rw-r--r--   0        0        0      597 2022-11-09 12:37:21.000000 swiftest-2024.4.1/CITATION.cff
--rw-r--r--   0        0        0     8490 2022-11-09 12:37:21.000000 swiftest-2024.4.1/CMakeLists.txt
--rw-r--r--   0        0        0    35149 2022-11-09 12:37:21.000000 swiftest-2024.4.1/COPYING
--rw-r--r--   0        0        0     3003 2022-11-09 12:37:21.000000 swiftest-2024.4.1/Dockerfile.GNU-Linux
--rw-r--r--   0        0        0     3849 2022-11-09 12:37:21.000000 swiftest-2024.4.1/Dockerfile.Intel
--rw-r--r--   0        0        0      784 2022-11-09 12:37:21.000000 swiftest-2024.4.1/LICENSE
--rw-r--r--   0        0        0     1644 2022-11-09 12:37:21.000000 swiftest-2024.4.1/README.md
--rw-r--r--   0        0        0     6148 2022-11-09 12:37:21.000000 swiftest-2024.4.1/README_figs/.DS_Store
--rw-r--r--   0        0        0     3990 2022-11-09 12:37:21.000000 swiftest-2024.4.1/README_tables/add_body_kwargs.md
--rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 swiftest-2024.4.1/README_tables/save_kwargs.md
--rw-r--r--   0        0        0    18321 2022-11-09 12:37:21.000000 swiftest-2024.4.1/README_tables/simulation_kwargs.md
--rw-r--r--   0        0        0      817 2022-11-09 12:37:21.000000 swiftest-2024.4.1/README_tables/write_param_kwargs.md
--rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 swiftest-2024.4.1/apptainer/.gitignore
--rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 swiftest-2024.4.1/buildscripts/.gitignore
--rw-r--r--   0        0        0     2128 2022-11-09 12:37:21.000000 swiftest-2024.4.1/buildscripts/windows/hdf5-cacheinit-windows.cmake
--rw-r--r--   0        0        0     2732 2022-11-09 12:37:21.000000 swiftest-2024.4.1/buildscripts/windows/netcdf-c-cacheinit-windows.cmake
--rw-r--r--   0        0        0      555 2022-11-09 12:37:21.000000 swiftest-2024.4.1/buildscripts/windows/netcdf-fortran-cacheinit-windows.cmake
--rw-r--r--   0        0        0     4894 2022-11-09 12:37:21.000000 swiftest-2024.4.1/cmake/Modules/FindCoarray_Fortran.cmake
--rw-r--r--   0        0        0     1437 2022-11-09 12:37:21.000000 swiftest-2024.4.1/cmake/Modules/FindFFTW3.cmake
--rw-r--r--   0        0        0    11765 2022-11-09 12:37:21.000000 swiftest-2024.4.1/cmake/Modules/FindNETCDF_Fortran.cmake
--rw-r--r--   0        0        0     4894 2022-11-09 12:37:21.000000 swiftest-2024.4.1/cmake/Modules/FindOpenMP_Fortran.cmake
--rw-r--r--   0        0        0     1765 2022-11-09 12:37:21.000000 swiftest-2024.4.1/cmake/Modules/FindSHTOOLS.cmake
--rw-r--r--   0        0        0     4175 2022-11-09 12:37:21.000000 swiftest-2024.4.1/cmake/Modules/SetCompileFlag.cmake
--rw-r--r--   0        0        0     1701 2022-11-09 12:37:21.000000 swiftest-2024.4.1/cmake/Modules/SetParallelizationLibrary.cmake
--rw-r--r--   0        0        0    29642 2022-11-09 12:37:21.000000 swiftest-2024.4.1/cmake/Modules/SetSwiftestFlags.cmake
--rw-r--r--   0        0        0     3360 2022-11-09 12:37:21.000000 swiftest-2024.4.1/distclean.cmake
--rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docker/.gitignore
--rw-r--r--   0        0        0     8651 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/Makefile
--rw-r--r--   0        0        0    29037 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/_static/basic_simulation_a_vs_t_plot.png
--rw-r--r--   0        0        0    35772 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/_static/index_api_reference.svg
--rw-r--r--   0        0        0   159139 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/_static/index_contribute.svg
--rw-r--r--   0        0        0    99515 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/_static/index_getting_started.svg
--rw-r--r--   0        0        0   115443 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/_static/index_user_guide.svg
--rw-r--r--   0        0        0   223959 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/_static/logos/swiftest_logo.png
--rw-r--r--   0        0        0   148144 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/_static/logos/swiftest_logo.svg
--rw-r--r--   0        0        0   115926 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/_static/logos/swiftest_social_preview.png
--rw-r--r--   0        0        0   145924 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/_static/logos/swiftest_social_preview.svg
--rw-r--r--   0        0        0     5908 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/_static/style.css
--rw-r--r--   0        0        0   636626 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/_static/symba_gr.png
--rw-r--r--   0        0        0      151 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/_templates/autosummary/accessor.rst
--rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/_templates/autosummary/accessor_attribute.rst
--rw-r--r--   0        0        0      168 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/_templates/autosummary/accessor_callable.rst
--rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/_templates/autosummary/accessor_method.rst
--rw-r--r--   0        0        0     6339 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/api.rst
--rw-r--r--   0        0        0     6065 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/conf.py
--rw-r--r--   0        0        0      202 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/contributing.rst
--rw-r--r--   0        0        0      976 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/environment.yml
--rw-r--r--   0        0        0    14169 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/getting-started-guide/index.rst
--rw-r--r--   0        0        0     2411 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/index.rst
--rw-r--r--   0        0        0      444 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/requirements.txt
--rw-r--r--   0        0        0    10302 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/user-guide/basic-simulation.rst
--rw-r--r--   0        0        0    11642 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/user-guide/detailed-simulation-setup.rst
--rw-r--r--   0        0        0     9035 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/user-guide/gravitational-harmonics.rst
--rw-r--r--   0        0        0      894 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/user-guide/index.rst
--rw-r--r--   0        0        0     7169 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/user-guide/planetocentric-init_cond.rst
--rw-r--r--   0        0        0     2465 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/user-guide/standalone-executable.rst
--rw-r--r--   0        0        0    14430 2022-11-09 12:37:21.000000 swiftest-2024.4.1/docs/whats-new.rst
--rw-r--r--   0        0        0      712 2022-11-09 12:37:21.000000 swiftest-2024.4.1/environment.yml
--rw-r--r--   0        0        0      170 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/.gitignore
--rw-r--r--   0        0        0       76 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Basic_Simulation/.gitignore
--rw-r--r--   0        0        0     1431 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Basic_Simulation/README.txt
--rwxr-xr-x   0        0        0     4167 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Basic_Simulation/basic_simulation.py
--rw-r--r--   0        0        0     1974 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Basic_Simulation/output_reader.py
--rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Chambers2013/.gitignore
--rw-r--r--   0        0        0     1400 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Chambers2013/README.txt
--rwxr-xr-x   0        0        0     6612 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Chambers2013/initial_conditions.py
--rwxr-xr-x   0        0        0     1350 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Chambers2013/run_simulation.py
--rwxr-xr-x   0        0        0     6462 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Chambers2013/scattermovie.py
--rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Fragmentation/.gitignore
--rwxr-xr-x   0        0        0    17766 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Fragmentation/Fragmentation_Movie.py
--rw-r--r--   0        0        0     1288 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Fragmentation/README.txt
--rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Multibody_Fragmentation/.gitignore
--rwxr-xr-x   0        0        0    13106 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Multibody_Fragmentation/Multibody_Movie.py
--rw-r--r--   0        0        0     1230 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Multibody_Fragmentation/README.txt
--rw-r--r--   0        0        0       35 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Swifter_Swiftest/.gitignore
--rw-r--r--   0        0        0      203 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Swifter_Swiftest/108pl_50tp/.gitignore
--rw-r--r--   0        0        0     2212 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Swifter_Swiftest/108pl_50tp/README.txt
--rw-r--r--   0        0        0      910 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Swifter_Swiftest/108pl_50tp/cb.in
--rw-r--r--   0        0        0     1441 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Swifter_Swiftest/108pl_50tp/param.swifter.in
--rw-r--r--   0        0        0     1924 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Swifter_Swiftest/108pl_50tp/param.swiftest.in
--rw-r--r--   0        0        0    21054 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Swifter_Swiftest/108pl_50tp/pl.swifter.in
--rw-r--r--   0        0        0    22140 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Swifter_Swiftest/108pl_50tp/pl.swiftest.in
--rw-r--r--   0        0        0      790 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Swifter_Swiftest/108pl_50tp/swifter_start.in
--rw-r--r--   0        0        0    34765 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Swifter_Swiftest/108pl_50tp/swifter_swiftest_comp.eps
--rw-r--r--   0        0        0     3751 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Swifter_Swiftest/108pl_50tp/swifter_swiftest_comp.py
--rw-r--r--   0        0        0     6870 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Swifter_Swiftest/108pl_50tp/tp.swifter.in
--rw-r--r--   0        0        0     7523 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Swifter_Swiftest/108pl_50tp/tp.swiftest.in
--rw-r--r--   0        0        0      194 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Swifter_Swiftest/8pl_0tp/.gitignore
--rw-r--r--   0        0        0     2091 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Swifter_Swiftest/8pl_0tp/README.txt
--rw-r--r--   0        0        0      805 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Swifter_Swiftest/8pl_0tp/cb.swiftest.in
--rwxr-xr-x   0        0        0     5753 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Swifter_Swiftest/8pl_0tp/init_cond.py
--rw-r--r--   0        0        0     1488 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Swifter_Swiftest/8pl_0tp/param.swifter.in
--rw-r--r--   0        0        0     1763 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Swifter_Swiftest/8pl_0tp/param.swiftest.in
--rw-r--r--   0        0        0     2577 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Swifter_Swiftest/8pl_0tp/pl.swifter.in
--rw-r--r--   0        0        0     2567 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Swifter_Swiftest/8pl_0tp/pl.swiftest.in
--rw-r--r--   0        0        0   142336 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Swifter_Swiftest/8pl_0tp/swiftest_symba_vs_swifter_symba.ipynb
--rw-r--r--   0        0        0      751 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Swifter_Swiftest/8pl_0tp/tp.swifter.in
--rw-r--r--   0        0        0      751 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/Swifter_Swiftest/8pl_0tp/tp.swiftest.in
--rw-r--r--   0        0        0       44 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/helio_gr_test/.gitignore
--rw-r--r--   0        0        0     1207 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/helio_gr_test/README.txt
--rwxr-xr-x   0        0        0     5104 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/helio_gr_test/helio_gr_test.py
--rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/rmvs_swifter_comparison/.gitignore
--rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/rmvs_swifter_comparison/1pl_1tp_encounter/.gitignore
--rwxr-xr-x   0        0        0     1455 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/rmvs_swifter_comparison/1pl_1tp_encounter/init_cond.py
--rw-r--r--   0        0        0    40129 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/rmvs_swifter_comparison/1pl_1tp_encounter/swiftest_vs_swifter.ipynb
--rw-r--r--   0        0        0      412 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/rmvs_swifter_comparison/1pl_1tp_encounter/swiftest_vs_swifter.py
--rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/rmvs_swifter_comparison/8pl_16tp_encounters/.gitignore
--rwxr-xr-x   0        0        0     1379 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/rmvs_swifter_comparison/8pl_16tp_encounters/init_cond.py
--rw-r--r--   0        0        0   100370 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/rmvs_swifter_comparison/8pl_16tp_encounters/swiftest_vs_swifter.ipynb
--rw-r--r--   0        0        0      412 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/rmvs_swifter_comparison/8pl_16tp_encounters/swiftest_vs_swifter.py
--rw-r--r--   0        0        0       39 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/solar_impact/.gitignore
--rw-r--r--   0        0        0     1197 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/solar_impact/README.txt
--rwxr-xr-x   0        0        0     2742 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/solar_impact/sundiver.py
--rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/spherical_harmonics_cb/.gitignore
--rw-r--r--   0        0        0     4247 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/spherical_harmonics_cb/J2_test_pl_and_tp.py
--rw-r--r--   0        0        0     3478 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/spherical_harmonics_cb/J2_test_tp.py
--rw-r--r--   0        0        0     4194 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/spherical_harmonics_cb/spherical_harmonics_cb.py
--rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/whm_gr_test/.gitignore
--rw-r--r--   0        0        0     1197 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/whm_gr_test/README.txt
--rwxr-xr-x   0        0        0     4981 2022-11-09 12:37:21.000000 swiftest-2024.4.1/examples/whm_gr_test/whm_gr_test.py
--rw-r--r--   0        0        0     1034 2022-11-09 12:37:21.000000 swiftest-2024.4.1/fortran_docs.md
--rw-r--r--   0        0        0     6194 2022-11-09 12:37:21.000000 swiftest-2024.4.1/paper/paper.bib
--rw-r--r--   0        0        0     8716 2022-11-09 12:37:21.000000 swiftest-2024.4.1/paper/paper.md
--rw-r--r--   0        0        0   239689 2022-11-09 12:37:21.000000 swiftest-2024.4.1/paper/performance.png
--rw-r--r--   0        0        0     4290 2022-11-09 12:37:21.000000 swiftest-2024.4.1/pyproject.toml
--rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 swiftest-2024.4.1/singularity/.gitignore
--rw-r--r--   0        0        0     9712 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/CMakeLists.txt
--rw-r--r--   0        0        0    95719 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/base/base_module.f90
--rw-r--r--   0        0        0       12 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/bindings/.gitignore
--rw-r--r--   0        0        0    12309 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/bindings/bindings_module.f90
--rw-r--r--   0        0        0    14014 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/coarray/coarray_clone.f90
--rw-r--r--   0        0        0     9494 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/coarray/coarray_collect.f90
--rw-r--r--   0        0        0     5625 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/coarray/coarray_module.f90
--rw-r--r--   0        0        0    13092 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/collision/collision_check.f90
--rw-r--r--   0        0        0    13054 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/collision/collision_generate.f90
--rw-r--r--   0        0        0    32844 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/collision/collision_io.f90
--rw-r--r--   0        0        0    45702 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/collision/collision_module.f90
--rw-r--r--   0        0        0    22228 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/collision/collision_regime.f90
--rw-r--r--   0        0        0    42155 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/collision/collision_resolve.f90
--rw-r--r--   0        0        0    45879 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/collision/collision_util.f90
--rw-r--r--   0        0        0    51642 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/encounter/encounter_check.f90
--rw-r--r--   0        0        0    18165 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/encounter/encounter_io.f90
--rw-r--r--   0        0        0    27454 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/encounter/encounter_module.f90
--rw-r--r--   0        0        0    29506 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/encounter/encounter_util.f90
--rw-r--r--   0        0        0    48836 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/fraggle/fraggle_generate.f90
--rw-r--r--   0        0        0     7479 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/fraggle/fraggle_module.f90
--rw-r--r--   0        0        0    12415 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/fraggle/fraggle_util.f90
--rw-r--r--   0        0        0       23 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/globals/.gitignore
--rw-r--r--   0        0        0     8954 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/globals/globals_module.f90
--rw-r--r--   0        0        0     8970 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/globals/globals_module.f90.in
--rw-r--r--   0        0        0     8126 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/helio/helio_drift.f90
--rw-r--r--   0        0        0     5145 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/helio/helio_gr.f90
--rw-r--r--   0        0        0     7481 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/helio/helio_kick.f90
--rw-r--r--   0        0        0    13088 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/helio/helio_module.f90
--rw-r--r--   0        0        0     5331 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/helio/helio_step.f90
--rw-r--r--   0        0        0     2201 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/helio/helio_util.f90
--rw-r--r--   0        0        0     1708 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/main/main.f90
--rw-r--r--   0        0        0     3835 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/misc/io_progress_bar_module.f90
--rw-r--r--   0        0        0    12298 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/misc/lambda_function_module.f90
--rw-r--r--   0        0        0    13165 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/misc/solver_module.f90
--rw-r--r--   0        0        0     7305 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/netcdf_io/netcdf_io_implementations.f90
--rw-r--r--   0        0        0    17644 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/netcdf_io/netcdf_io_module.f90
--rw-r--r--   0        0        0     6828 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/operator/operator_cross.f90
--rw-r--r--   0        0        0     3114 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/operator/operator_mag.f90
--rw-r--r--   0        0        0     8949 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/operator/operator_module.f90
--rw-r--r--   0        0        0     3998 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/operator/operator_unit.f90
--rw-r--r--   0        0        0     5352 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/rmvs/rmvs_coarray.f90
--rw-r--r--   0        0        0     3250 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/rmvs/rmvs_discard.f90
--rw-r--r--   0        0        0     3089 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/rmvs/rmvs_encounter_check.f90
--rw-r--r--   0        0        0     5853 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/rmvs/rmvs_kick.f90
--rw-r--r--   0        0        0    24058 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/rmvs/rmvs_module.f90
--rw-r--r--   0        0        0    33567 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/rmvs/rmvs_step.f90
--rw-r--r--   0        0        0    26209 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/rmvs/rmvs_util.f90
--rw-r--r--   0        0        0     7694 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/shgrav/shgrav_accel.f90
--rw-r--r--   0        0        0     1458 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/shgrav/shgrav_module.f90
--rw-r--r--   0        0        0    26288 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/swiftest/swiftest_coarray.f90
--rw-r--r--   0        0        0    18879 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/swiftest/swiftest_discard.f90
--rw-r--r--   0        0        0    25136 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/swiftest/swiftest_drift.f90
--rw-r--r--   0        0        0     9129 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/swiftest/swiftest_driver.f90
--rw-r--r--   0        0        0    12386 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/swiftest/swiftest_gr.f90
--rw-r--r--   0        0        0   190532 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/swiftest/swiftest_io.f90
--rw-r--r--   0        0        0    20673 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/swiftest/swiftest_kick.f90
--rw-r--r--   0        0        0   144471 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/swiftest/swiftest_module.f90
--rw-r--r--   0        0        0    15411 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/swiftest/swiftest_obl.f90
--rw-r--r--   0        0        0    38438 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/swiftest/swiftest_orbel.f90
--rw-r--r--   0        0        0     1770 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/swiftest/swiftest_user.f90
--rw-r--r--   0        0        0   146697 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/swiftest/swiftest_util.f90
--rw-r--r--   0        0        0    20402 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/symba/symba_discard.f90
--rw-r--r--   0        0        0     2960 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/symba/symba_drift.f90
--rw-r--r--   0        0        0    13228 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/symba/symba_encounter_check.f90
--rw-r--r--   0        0        0     3241 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/symba/symba_gr.f90
--rw-r--r--   0        0        0    14491 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/symba/symba_kick.f90
--rw-r--r--   0        0        0    28069 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/symba/symba_module.f90
--rw-r--r--   0        0        0    14590 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/symba/symba_step.f90
--rw-r--r--   0        0        0    21903 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/symba/symba_util.f90
--rw-r--r--   0        0        0     3183 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/tides/tides_getacch_pl.f90
--rw-r--r--   0        0        0     4570 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/tides/tides_module.f90
--rw-r--r--   0        0        0     4550 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/tides/tides_spin_step.f90
--rw-r--r--   0        0        0     5031 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/walltime/walltime_implementations.f90
--rw-r--r--   0        0        0     4557 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/walltime/walltime_module.f90
--rw-r--r--   0        0        0     1322 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/whm/whm_coarray.f90
--rw-r--r--   0        0        0     5011 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/whm/whm_coord.f90
--rw-r--r--   0        0        0     2795 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/whm/whm_drift.f90
--rw-r--r--   0        0        0     5480 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/whm/whm_gr.f90
--rw-r--r--   0        0        0    12284 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/whm/whm_kick.f90
--rw-r--r--   0        0        0    19625 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/whm/whm_module.f90
--rw-r--r--   0        0        0     4929 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/whm/whm_step.f90
--rw-r--r--   0        0        0    13175 2022-11-09 12:37:21.000000 swiftest-2024.4.1/src/whm/whm_util.f90
--rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 swiftest-2024.4.1/swiftest/.gitignore
--rw-r--r--   0        0        0     2280 2022-11-09 12:37:21.000000 swiftest-2024.4.1/swiftest/CMakeLists.txt
--rw-r--r--   0        0        0      964 2022-11-09 12:37:21.000000 swiftest-2024.4.1/swiftest/__init__.py
--rw-r--r--   0        0        0     1396 2022-11-09 12:37:21.000000 swiftest-2024.4.1/swiftest/cli.py
--rw-r--r--   0        0        0     1434 2022-11-09 12:37:21.000000 swiftest-2024.4.1/swiftest/constants.py
--rw-r--r--   0        0        0      576 2022-11-09 12:37:21.000000 swiftest-2024.4.1/swiftest/core.h
--rw-r--r--   0        0        0     9852 2022-11-09 12:37:21.000000 swiftest-2024.4.1/swiftest/core.pyx
--rw-r--r--   0        0        0    15941 2022-11-09 12:37:21.000000 swiftest-2024.4.1/swiftest/data.py
--rw-r--r--   0        0        0    21140 2022-11-09 12:37:21.000000 swiftest-2024.4.1/swiftest/init_cond.py
--rw-r--r--   0        0        0    60985 2022-11-09 12:37:21.000000 swiftest-2024.4.1/swiftest/io.py
--rw-r--r--   0        0        0     7098 2022-11-09 12:37:21.000000 swiftest-2024.4.1/swiftest/shgrav.py
--rw-r--r--   0        0        0   195796 2022-11-09 12:37:21.000000 swiftest-2024.4.1/swiftest/simulation.py
-lrwxr-xr-x   0        0        0        0 2022-11-09 12:37:21.000000 swiftest-2024.4.1/swiftest/swiftest -> ../build/bin/swiftest
--rw-r--r--   0        0        0     4239 2022-11-09 12:37:21.000000 swiftest-2024.4.1/swiftest/tool.py
--rw-r--r--   0        0        0     1594 2022-11-09 12:37:21.000000 swiftest-2024.4.1/swiftest/visualize.py
--rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 swiftest-2024.4.1/tests/.gitignore
--rw-r--r--   0        0        0    12156 2022-11-09 12:37:21.000000 swiftest-2024.4.1/tests/test_fraggle.py
--rwxr-xr-x   0        0        0     7842 2022-11-09 12:37:21.000000 swiftest-2024.4.1/tests/test_integration.py
--rwxr-xr-x   0        0        0    24776 2022-11-09 12:37:21.000000 swiftest-2024.4.1/tests/test_io.py
--rw-r--r--   0        0        0     2189 2022-11-09 12:37:21.000000 swiftest-2024.4.1/tests/test_particle_type.py
--rwxr-xr-x   0        0        0     2255 2022-11-09 12:37:21.000000 swiftest-2024.4.1/tests/test_units.py
--rw-r--r--   0        0        0     2699 2022-11-09 12:37:21.000000 swiftest-2024.4.1/tests/test_xv2el2xv_dims.py
--rw-r--r--   0        0        0        8 2022-11-09 12:37:21.000000 swiftest-2024.4.1/version.txt
--rw-r--r--   0        0        0     3928 2022-11-09 12:37:21.000000 swiftest-2024.4.1/PKG-INFO
+-rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 swiftest-2024.4.2/.dockerignore
+-rw-r--r--   0        0        0     1404 2022-11-09 12:37:21.000000 swiftest-2024.4.2/.github/workflows/build_wheels.yml
+-rw-r--r--   0        0        0      544 2022-11-09 12:37:21.000000 swiftest-2024.4.2/.github/workflows/build_wheels_debug.yml
+-rw-r--r--   0        0        0     1082 2022-11-09 12:37:21.000000 swiftest-2024.4.2/.gitignore
+-rw-r--r--   0        0        0      684 2022-11-09 12:37:21.000000 swiftest-2024.4.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     1916 2022-11-09 12:37:21.000000 swiftest-2024.4.2/.zenodo.json
+-rw-r--r--   0        0        0      597 2022-11-09 12:37:21.000000 swiftest-2024.4.2/CITATION.cff
+-rw-r--r--   0        0        0     8672 2022-11-09 12:37:21.000000 swiftest-2024.4.2/CMakeLists.txt
+-rw-r--r--   0        0        0    35149 2022-11-09 12:37:21.000000 swiftest-2024.4.2/COPYING
+-rw-r--r--   0        0        0     3003 2022-11-09 12:37:21.000000 swiftest-2024.4.2/Dockerfile.GNU-Linux
+-rw-r--r--   0        0        0     3849 2022-11-09 12:37:21.000000 swiftest-2024.4.2/Dockerfile.Intel
+-rw-r--r--   0        0        0      784 2022-11-09 12:37:21.000000 swiftest-2024.4.2/LICENSE
+-rw-r--r--   0        0        0     1644 2022-11-09 12:37:21.000000 swiftest-2024.4.2/README.md
+-rw-r--r--   0        0        0     6148 2022-11-09 12:37:21.000000 swiftest-2024.4.2/README_figs/.DS_Store
+-rw-r--r--   0        0        0     3990 2022-11-09 12:37:21.000000 swiftest-2024.4.2/README_tables/add_body_kwargs.md
+-rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 swiftest-2024.4.2/README_tables/save_kwargs.md
+-rw-r--r--   0        0        0    18321 2022-11-09 12:37:21.000000 swiftest-2024.4.2/README_tables/simulation_kwargs.md
+-rw-r--r--   0        0        0      817 2022-11-09 12:37:21.000000 swiftest-2024.4.2/README_tables/write_param_kwargs.md
+-rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 swiftest-2024.4.2/apptainer/.gitignore
+-rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 swiftest-2024.4.2/buildscripts/.gitignore
+-rw-r--r--   0        0        0     2128 2022-11-09 12:37:21.000000 swiftest-2024.4.2/buildscripts/windows/hdf5-cacheinit-windows.cmake
+-rw-r--r--   0        0        0     2732 2022-11-09 12:37:21.000000 swiftest-2024.4.2/buildscripts/windows/netcdf-c-cacheinit-windows.cmake
+-rw-r--r--   0        0        0      555 2022-11-09 12:37:21.000000 swiftest-2024.4.2/buildscripts/windows/netcdf-fortran-cacheinit-windows.cmake
+-rw-r--r--   0        0        0     3227 2022-11-09 12:37:21.000000 swiftest-2024.4.2/cmake/Modules/FindCoarray_Fortran.cmake
+-rw-r--r--   0        0        0     1437 2022-11-09 12:37:21.000000 swiftest-2024.4.2/cmake/Modules/FindFFTW3.cmake
+-rw-r--r--   0        0        0    11765 2022-11-09 12:37:21.000000 swiftest-2024.4.2/cmake/Modules/FindNETCDF_Fortran.cmake
+-rw-r--r--   0        0        0     4867 2022-11-09 12:37:21.000000 swiftest-2024.4.2/cmake/Modules/FindOpenMP_Fortran.cmake
+-rw-r--r--   0        0        0     1681 2022-11-09 12:37:21.000000 swiftest-2024.4.2/cmake/Modules/FindSHTOOLS.cmake
+-rw-r--r--   0        0        0     4175 2022-11-09 12:37:21.000000 swiftest-2024.4.2/cmake/Modules/SetCompileFlag.cmake
+-rw-r--r--   0        0        0     1220 2022-11-09 12:37:21.000000 swiftest-2024.4.2/cmake/Modules/SetParallelizationLibrary.cmake
+-rw-r--r--   0        0        0    29637 2022-11-09 12:37:21.000000 swiftest-2024.4.2/cmake/Modules/SetSwiftestFlags.cmake
+-rw-r--r--   0        0        0     3360 2022-11-09 12:37:21.000000 swiftest-2024.4.2/distclean.cmake
+-rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docker/.gitignore
+-rw-r--r--   0        0        0     8651 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/Makefile
+-rw-r--r--   0        0        0    29037 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_static/basic_simulation_a_vs_t_plot.png
+-rw-r--r--   0        0        0    35772 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_static/index_api_reference.svg
+-rw-r--r--   0        0        0   159139 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_static/index_contribute.svg
+-rw-r--r--   0        0        0    99515 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_static/index_getting_started.svg
+-rw-r--r--   0        0        0   115443 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_static/index_user_guide.svg
+-rw-r--r--   0        0        0   223959 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_static/logos/swiftest_logo.png
+-rw-r--r--   0        0        0   148144 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_static/logos/swiftest_logo.svg
+-rw-r--r--   0        0        0   115926 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_static/logos/swiftest_social_preview.png
+-rw-r--r--   0        0        0   145924 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_static/logos/swiftest_social_preview.svg
+-rw-r--r--   0        0        0     5908 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_static/style.css
+-rw-r--r--   0        0        0   636626 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_static/symba_gr.png
+-rw-r--r--   0        0        0      151 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_templates/autosummary/accessor.rst
+-rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_templates/autosummary/accessor_attribute.rst
+-rw-r--r--   0        0        0      168 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_templates/autosummary/accessor_callable.rst
+-rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_templates/autosummary/accessor_method.rst
+-rw-r--r--   0        0        0     6339 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/api.rst
+-rw-r--r--   0        0        0     6065 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/conf.py
+-rw-r--r--   0        0        0      202 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/contributing.rst
+-rw-r--r--   0        0        0      976 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/environment.yml
+-rw-r--r--   0        0        0    14169 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/getting-started-guide/index.rst
+-rw-r--r--   0        0        0     2411 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/index.rst
+-rw-r--r--   0        0        0      444 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/requirements.txt
+-rw-r--r--   0        0        0    10302 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/user-guide/basic-simulation.rst
+-rw-r--r--   0        0        0    11642 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/user-guide/detailed-simulation-setup.rst
+-rw-r--r--   0        0        0     9035 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/user-guide/gravitational-harmonics.rst
+-rw-r--r--   0        0        0      894 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/user-guide/index.rst
+-rw-r--r--   0        0        0     7169 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/user-guide/planetocentric-init_cond.rst
+-rw-r--r--   0        0        0     2465 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/user-guide/standalone-executable.rst
+-rw-r--r--   0        0        0    18192 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/whats-new.rst
+-rw-r--r--   0        0        0      712 2022-11-09 12:37:21.000000 swiftest-2024.4.2/environment.yml
+-rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/.gitignore
+-rw-r--r--   0        0        0       76 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Basic_Simulation/.gitignore
+-rw-r--r--   0        0        0     1431 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Basic_Simulation/README.txt
+-rwxr-xr-x   0        0        0     4167 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Basic_Simulation/basic_simulation.py
+-rw-r--r--   0        0        0     1974 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Basic_Simulation/output_reader.py
+-rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Chambers2013/.gitignore
+-rw-r--r--   0        0        0     1400 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Chambers2013/README.txt
+-rwxr-xr-x   0        0        0     6612 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Chambers2013/initial_conditions.py
+-rwxr-xr-x   0        0        0     1350 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Chambers2013/run_simulation.py
+-rwxr-xr-x   0        0        0     6462 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Chambers2013/scattermovie.py
+-rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Coarray_Test_Particles/.gitignore
+-rwxr-xr-x   0        0        0     2075 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Coarray_Test_Particles/initial_conditions.py
+-rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Fragmentation/.gitignore
+-rwxr-xr-x   0        0        0    17766 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Fragmentation/Fragmentation_Movie.py
+-rw-r--r--   0        0        0     1288 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Fragmentation/README.txt
+-rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Multibody_Fragmentation/.gitignore
+-rwxr-xr-x   0        0        0    13106 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Multibody_Fragmentation/Multibody_Movie.py
+-rw-r--r--   0        0        0     1230 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Multibody_Fragmentation/README.txt
+-rw-r--r--   0        0        0       35 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/.gitignore
+-rw-r--r--   0        0        0      203 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/.gitignore
+-rw-r--r--   0        0        0     2212 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/README.txt
+-rw-r--r--   0        0        0      910 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/cb.in
+-rw-r--r--   0        0        0     1441 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/param.swifter.in
+-rw-r--r--   0        0        0     1924 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/param.swiftest.in
+-rw-r--r--   0        0        0    21054 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/pl.swifter.in
+-rw-r--r--   0        0        0    22140 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/pl.swiftest.in
+-rw-r--r--   0        0        0      790 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/swifter_start.in
+-rw-r--r--   0        0        0    34765 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/swifter_swiftest_comp.eps
+-rw-r--r--   0        0        0     3751 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/swifter_swiftest_comp.py
+-rw-r--r--   0        0        0     6870 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/tp.swifter.in
+-rw-r--r--   0        0        0     7523 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/tp.swiftest.in
+-rw-r--r--   0        0        0      194 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/.gitignore
+-rw-r--r--   0        0        0     2091 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/README.txt
+-rw-r--r--   0        0        0      805 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/cb.swiftest.in
+-rwxr-xr-x   0        0        0     5753 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/init_cond.py
+-rw-r--r--   0        0        0     1488 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/param.swifter.in
+-rw-r--r--   0        0        0     1763 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/param.swiftest.in
+-rw-r--r--   0        0        0     2577 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/pl.swifter.in
+-rw-r--r--   0        0        0     2567 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/pl.swiftest.in
+-rw-r--r--   0        0        0   142336 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/swiftest_symba_vs_swifter_symba.ipynb
+-rw-r--r--   0        0        0      751 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/tp.swifter.in
+-rw-r--r--   0        0        0      751 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/tp.swiftest.in
+-rw-r--r--   0        0        0       25 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/escape_from_the_solar_system/.gitignore
+-rwxr-xr-x   0        0        0     1736 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/escape_from_the_solar_system/escape.py
+-rw-r--r--   0        0        0       44 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/helio_gr_test/.gitignore
+-rw-r--r--   0        0        0     1207 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/helio_gr_test/README.txt
+-rwxr-xr-x   0        0        0     5104 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/helio_gr_test/helio_gr_test.py
+-rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/rmvs_swifter_comparison/.gitignore
+-rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/rmvs_swifter_comparison/1pl_1tp_encounter/.gitignore
+-rwxr-xr-x   0        0        0     1455 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/rmvs_swifter_comparison/1pl_1tp_encounter/init_cond.py
+-rw-r--r--   0        0        0    40129 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/rmvs_swifter_comparison/1pl_1tp_encounter/swiftest_vs_swifter.ipynb
+-rw-r--r--   0        0        0      412 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/rmvs_swifter_comparison/1pl_1tp_encounter/swiftest_vs_swifter.py
+-rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/rmvs_swifter_comparison/8pl_16tp_encounters/.gitignore
+-rwxr-xr-x   0        0        0     1379 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/rmvs_swifter_comparison/8pl_16tp_encounters/init_cond.py
+-rw-r--r--   0        0        0   100370 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/rmvs_swifter_comparison/8pl_16tp_encounters/swiftest_vs_swifter.ipynb
+-rw-r--r--   0        0        0      412 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/rmvs_swifter_comparison/8pl_16tp_encounters/swiftest_vs_swifter.py
+-rw-r--r--   0        0        0       39 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/solar_impact/.gitignore
+-rw-r--r--   0        0        0     1197 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/solar_impact/README.txt
+-rwxr-xr-x   0        0        0     3267 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/solar_impact/sundiver.py
+-rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/spherical_harmonics_cb/.gitignore
+-rw-r--r--   0        0        0     4247 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/spherical_harmonics_cb/J2_test_pl_and_tp.py
+-rw-r--r--   0        0        0     3478 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/spherical_harmonics_cb/J2_test_tp.py
+-rw-r--r--   0        0        0     4194 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/spherical_harmonics_cb/spherical_harmonics_cb.py
+-rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/whm_gr_test/.gitignore
+-rw-r--r--   0        0        0     1197 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/whm_gr_test/README.txt
+-rwxr-xr-x   0        0        0     4981 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/whm_gr_test/whm_gr_test.py
+-rw-r--r--   0        0        0     1034 2022-11-09 12:37:21.000000 swiftest-2024.4.2/fortran_docs.md
+-rw-r--r--   0        0        0     6194 2022-11-09 12:37:21.000000 swiftest-2024.4.2/paper/paper.bib
+-rw-r--r--   0        0        0     8716 2022-11-09 12:37:21.000000 swiftest-2024.4.2/paper/paper.md
+-rw-r--r--   0        0        0   239689 2022-11-09 12:37:21.000000 swiftest-2024.4.2/paper/performance.png
+-rw-r--r--   0        0        0     5139 2022-11-09 12:37:21.000000 swiftest-2024.4.2/pyproject.toml
+-rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 swiftest-2024.4.2/singularity/.gitignore
+-rw-r--r--   0        0        0    11563 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/CMakeLists.txt
+-rw-r--r--   0        0        0    92405 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/base/base_module.f90
+-rw-r--r--   0        0        0       12 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/bindings/.gitignore
+-rw-r--r--   0        0        0    12309 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/bindings/bindings_module.f90
+-rw-r--r--   0        0        0     7017 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/coarray/coarray_clone.f90
+-rw-r--r--   0        0        0     7442 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/coarray/coarray_collect.f90
+-rw-r--r--   0        0        0     3367 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/coarray/coarray_module.f90
+-rw-r--r--   0        0        0    13092 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/collision/collision_check.f90
+-rw-r--r--   0        0        0    13302 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/collision/collision_generate.f90
+-rw-r--r--   0        0        0    36608 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/collision/collision_io.f90
+-rw-r--r--   0        0        0    47339 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/collision/collision_module.f90
+-rw-r--r--   0        0        0    22624 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/collision/collision_regime.f90
+-rw-r--r--   0        0        0    39593 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/collision/collision_resolve.f90
+-rw-r--r--   0        0        0    50559 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/collision/collision_util.f90
+-rw-r--r--   0        0        0    51642 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/encounter/encounter_check.f90
+-rw-r--r--   0        0        0    18165 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/encounter/encounter_io.f90
+-rw-r--r--   0        0        0    27454 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/encounter/encounter_module.f90
+-rw-r--r--   0        0        0    29506 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/encounter/encounter_util.f90
+-rw-r--r--   0        0        0    49238 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/fraggle/fraggle_generate.f90
+-rw-r--r--   0        0        0     7479 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/fraggle/fraggle_module.f90
+-rw-r--r--   0        0        0    12594 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/fraggle/fraggle_util.f90
+-rw-r--r--   0        0        0       23 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/globals/.gitignore
+-rw-r--r--   0        0        0     8954 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/globals/globals_module.f90
+-rw-r--r--   0        0        0     8970 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/globals/globals_module.f90.in
+-rw-r--r--   0        0        0     8126 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/helio/helio_drift.f90
+-rw-r--r--   0        0        0     5145 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/helio/helio_gr.f90
+-rw-r--r--   0        0        0     7481 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/helio/helio_kick.f90
+-rw-r--r--   0        0        0    13088 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/helio/helio_module.f90
+-rw-r--r--   0        0        0     5331 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/helio/helio_step.f90
+-rw-r--r--   0        0        0     2201 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/helio/helio_util.f90
+-rw-r--r--   0        0        0     1534 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/main/main.f90
+-rw-r--r--   0        0        0     3835 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/misc/io_progress_bar_module.f90
+-rw-r--r--   0        0        0    12298 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/misc/lambda_function_module.f90
+-rw-r--r--   0        0        0    13165 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/misc/solver_module.f90
+-rw-r--r--   0        0        0     7388 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/netcdf_io/netcdf_io_implementations.f90
+-rw-r--r--   0        0        0    17666 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/netcdf_io/netcdf_io_module.f90
+-rw-r--r--   0        0        0     6828 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/operator/operator_cross.f90
+-rw-r--r--   0        0        0     3114 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/operator/operator_mag.f90
+-rw-r--r--   0        0        0     8949 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/operator/operator_module.f90
+-rw-r--r--   0        0        0     3998 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/operator/operator_unit.f90
+-rw-r--r--   0        0        0     4439 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/rmvs/rmvs_discard.f90
+-rw-r--r--   0        0        0     3089 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/rmvs/rmvs_encounter_check.f90
+-rw-r--r--   0        0        0     5853 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/rmvs/rmvs_kick.f90
+-rw-r--r--   0        0        0    24137 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/rmvs/rmvs_module.f90
+-rw-r--r--   0        0        0    33566 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/rmvs/rmvs_step.f90
+-rw-r--r--   0        0        0    26209 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/rmvs/rmvs_util.f90
+-rw-r--r--   0        0        0     7694 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/shgrav/shgrav_accel.f90
+-rw-r--r--   0        0        0     1458 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/shgrav/shgrav_module.f90
+-rw-r--r--   0        0        0    16114 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/swiftest/swiftest_coarray.f90
+-rw-r--r--   0        0        0    20114 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/swiftest/swiftest_discard.f90
+-rw-r--r--   0        0        0    25136 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/swiftest/swiftest_drift.f90
+-rw-r--r--   0        0        0     9216 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/swiftest/swiftest_driver.f90
+-rw-r--r--   0        0        0    12386 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/swiftest/swiftest_gr.f90
+-rw-r--r--   0        0        0   190418 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/swiftest/swiftest_io.f90
+-rw-r--r--   0        0        0    20673 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/swiftest/swiftest_kick.f90
+-rw-r--r--   0        0        0   141061 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/swiftest/swiftest_module.f90
+-rw-r--r--   0        0        0    15415 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/swiftest/swiftest_obl.f90
+-rw-r--r--   0        0        0    38438 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/swiftest/swiftest_orbel.f90
+-rw-r--r--   0        0        0     1770 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/swiftest/swiftest_user.f90
+-rw-r--r--   0        0        0   148284 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/swiftest/swiftest_util.f90
+-rw-r--r--   0        0        0    21950 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/symba/symba_discard.f90
+-rw-r--r--   0        0        0     2960 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/symba/symba_drift.f90
+-rw-r--r--   0        0        0    13228 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/symba/symba_encounter_check.f90
+-rw-r--r--   0        0        0     3241 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/symba/symba_gr.f90
+-rw-r--r--   0        0        0    14491 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/symba/symba_kick.f90
+-rw-r--r--   0        0        0    28069 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/symba/symba_module.f90
+-rw-r--r--   0        0        0    14590 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/symba/symba_step.f90
+-rw-r--r--   0        0        0    21903 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/symba/symba_util.f90
+-rw-r--r--   0        0        0     3183 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/tides/tides_getacch_pl.f90
+-rw-r--r--   0        0        0     4566 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/tides/tides_module.f90
+-rw-r--r--   0        0        0     4546 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/tides/tides_spin_step.f90
+-rw-r--r--   0        0        0     5031 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/walltime/walltime_implementations.f90
+-rw-r--r--   0        0        0     4557 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/walltime/walltime_module.f90
+-rw-r--r--   0        0        0     5011 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/whm/whm_coord.f90
+-rw-r--r--   0        0        0     2795 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/whm/whm_drift.f90
+-rw-r--r--   0        0        0     5480 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/whm/whm_gr.f90
+-rw-r--r--   0        0        0    12284 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/whm/whm_kick.f90
+-rw-r--r--   0        0        0    23268 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/whm/whm_module.f90
+-rw-r--r--   0        0        0     4928 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/whm/whm_step.f90
+-rw-r--r--   0        0        0    13175 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/whm/whm_util.f90
+-rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/.gitignore
+-rw-r--r--   0        0        0     2295 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/CMakeLists.txt
+-rw-r--r--   0        0        0      964 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/__init__.py
+-rw-r--r--   0        0        0     1466 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/cli.py
+-rw-r--r--   0        0        0     1393 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/cli_caf.py
+-rw-r--r--   0        0        0     1434 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/constants.py
+-rw-r--r--   0        0        0      576 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/core.h
+-rw-r--r--   0        0        0     9852 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/core.pyx
+-rw-r--r--   0        0        0    15976 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/data.py
+-rw-r--r--   0        0        0    21140 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/init_cond.py
+-rw-r--r--   0        0        0    61003 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/io.py
+-rw-r--r--   0        0        0     7098 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/shgrav.py
+-rw-r--r--   0        0        0   195796 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/simulation.py
+lrwxr-xr-x   0        0        0        0 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/swiftest -> ../build/bin/swiftest
+-rw-r--r--   0        0        0     4239 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/tool.py
+-rw-r--r--   0        0        0     1594 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/visualize.py
+-rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 swiftest-2024.4.2/tests/.gitignore
+-rw-r--r--   0        0        0     9389 2022-11-09 12:37:21.000000 swiftest-2024.4.2/tests/test_collisions.py
+-rw-r--r--   0        0        0    12156 2022-11-09 12:37:21.000000 swiftest-2024.4.2/tests/test_fraggle.py
+-rwxr-xr-x   0        0        0     7841 2022-11-09 12:37:21.000000 swiftest-2024.4.2/tests/test_integration.py
+-rwxr-xr-x   0        0        0    24776 2022-11-09 12:37:21.000000 swiftest-2024.4.2/tests/test_io.py
+-rw-r--r--   0        0        0     2189 2022-11-09 12:37:21.000000 swiftest-2024.4.2/tests/test_particle_type.py
+-rwxr-xr-x   0        0        0     2255 2022-11-09 12:37:21.000000 swiftest-2024.4.2/tests/test_units.py
+-rw-r--r--   0        0        0     2665 2022-11-09 12:37:21.000000 swiftest-2024.4.2/tests/test_xv2el2xv_dims.py
+-rw-r--r--   0        0        0        8 2022-11-09 12:37:21.000000 swiftest-2024.4.2/version.txt
+-rw-r--r--   0        0        0     3932 2022-11-09 12:37:21.000000 swiftest-2024.4.2/PKG-INFO
```

### Comparing `swiftest-2024.4.1/.github/workflows/build_wheels.yml` & `swiftest-2024.4.2/.github/workflows/build_wheels.yml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 jobs:
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        os: [ubuntu-latest, macos-11, macos-12, macos-13, macos-14]  
+        os: [ubuntu-latest, macos-12, macos-13, macos-14]  
 
     steps:
       - uses: actions/checkout@v4
 
       - name: Build wheels
         uses: pypa/cibuildwheel@v2.17.0
```

### Comparing `swiftest-2024.4.1/.github/workflows/build_wheels_debug.yml` & `swiftest-2024.4.2/.github/workflows/build_wheels_debug.yml`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 jobs:
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        os: [ubuntu-latest, macos-11, macos-12, macos-13, macos-14]  
+        os: [ubuntu-latest, macos-12, macos-13, macos-14]  
 
     steps:
       - uses: actions/checkout@v4
 
       - name: Build wheels
         uses: pypa/cibuildwheel@v2.17.0
```

### Comparing `swiftest-2024.4.1/.gitignore` & `swiftest-2024.4.2/.gitignore`

 * *Files 15% similar despite different names*

```diff
@@ -32,17 +32,14 @@
 !pyproject.toml
 **/_skbuild
 *.egg*
 swiftest-*
 __pycache__*
 _cmake*
 _dependencies
-!SHTOOLS
-!SHTOOLS/**
-
 
 #Documentation
 !.readthedocs.yaml
 !docs/
 !docs/**/*
 !docs/_build/
 docs/_build/**/*
```

### Comparing `swiftest-2024.4.1/.readthedocs.yaml` & `swiftest-2024.4.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/.zenodo.json` & `swiftest-2024.4.2/.zenodo.json`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/CITATION.cff` & `swiftest-2024.4.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/CMakeLists.txt` & `swiftest-2024.4.2/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     MESSAGE(FATAL_ERROR "In-source builds not allowed. Please make a new directory (called a build directory) and run CMake from there.\n")
 ENDIF()
 
 # Ensure scikit-build modules
 FIND_PACKAGE(Python COMPONENTS Interpreter Development.Module NumPy REQUIRED)
 
 # Set some options the user may choose
-OPTION(USE_COARRAY "Use Coarray Fortran for parallelization of test particles" OFF)
+OPTION(USE_COARRAY "Use Coarray Fortran for parallelization of test particles" ON)
 OPTION(USE_OPENMP "Use OpenMP for parallelization" ON)
 OPTION(USE_SIMD "Use SIMD vectorization" ON)
 OPTION(BUILD_SHARED_LIBS "Build using shared libraries" ON)
 
 # Define the paths to the source code and python files
 SET(SRC "${CMAKE_SOURCE_DIR}/src")
 SET(PY "${CMAKE_SOURCE_DIR}/swiftest")
@@ -134,17 +134,17 @@
 MESSAGE(STATUS "INSTALL_LIBDIR: ${INSTALL_LIBDIR}")
 MESSAGE(STATUS "INSTALL_INCLUDEDIR: ${INSTALL_INCLUDEDIR}")
 MESSAGE(STATUS "INSTALL_PYPROJ: ${INSTALL_PYPROJ}")
 MESSAGE(STATUS "CMAKE_INSTALL_RPATH: ${CMAKE_INSTALL_RPATH}")
 SET(CMAKE_INSTALL_RPATH_USE_LINK_PATH TRUE)
 
 # Have the .mod files placed in the include folder
-SET(CMAKE_Fortran_MODULE_DIRECTORY ${CMAKE_CURRENT_BINARY_DIR}/mod)
+SET(CMAKE_Fortran_MODULE_DIRECTORY ${CMAKE_BINARY_DIR}/mod)
 
-# Add our local modules to the module ldpath
+# Add our local CMake modules to the module ldpath
 FILE(TO_CMAKE_PATH "${CMAKE_SOURCE_DIR}/cmake/Modules" LOCAL_MODULE_PATH)
 LIST(APPEND CMAKE_MODULE_PATH ${LOCAL_MODULE_PATH})
 
 # Add in the external dependency libraries 
 IF (CMAKE_Fortran_COMPILER_ID MATCHES "^Intel")
     SET(COMPILER_OPTIONS "Intel" CACHE STRING "Compiler identified as Intel")
 ELSEIF (CMAKE_Fortran_COMPILER_ID STREQUAL "GNU")
@@ -163,27 +163,37 @@
     SET(BLA_VENDOR "Intel10_64lp" CACHE STRING "BLAS vendor")
 ENDIF()
 SET(BLA_STATIC ON)
 FIND_PACKAGE(BLAS REQUIRED)
 FIND_PACKAGE(LAPACK REQUIRED)
 FIND_PACKAGE(FFTW3 REQUIRED)
 FIND_PACKAGE(SHTOOLS REQUIRED)
+IF (USE_COARRAY)
+    MESSAGE(STATUS "Building with Coarray support")
+    FIND_PACKAGE(Coarray_Fortran REQUIRED)
+ENDIF()
 
-SET(HDF5_USE_STATIC_LIBRARIES ON CACHE BOOL "Use static libraries for HDF5")
+SET(HDF5_USE_STATIC_LIBRARIES OFF CACHE BOOL "Use static libraries for HDF5")
+
+IF (USE_COARRAY)
+    SET(HDF5_PREFER_PARALLEL ON CACHE BOOL "Prefer parallel HDF5")
+ELSE ()
+    SET(HDF5_PREFER_PARALLEL OFF CACHE BOOL "Prefer parallel HDF5")
+ENDIF()
 
-FIND_PACKAGE(NETCDF_Fortran REQUIRED)
 IF (MSVC)
     FIND_PACKAGE(HDF5 NAMES hdf5 COMPONENTS C HL REQUIRED CONFIG)
     MESSAGE(STATUS "HDF5_FOUND: ${HDF5_FOUND}")
     MESSAGE(STATUS "HDF5_VERSION: ${HDF5_VERSION}")
     MESSAGE(STATUS "HDF5_LIBRARIES: ${HDF5_LIBRARIES}")
     MESSAGE(STATUS "HDF5_INCLUDE_DIRS: ${HDF5_INCLUDE_DIRS}")
 ELSE ()
     FIND_PACKAGE(HDF5 COMPONENTS C HL REQUIRED)
 ENDIF ()
+FIND_PACKAGE(NETCDF_Fortran REQUIRED)
 
 MESSAGE(STATUS "CMAKE_SYSTEM_PROCESSOR: " ${CMAKE_SYSTEM_PROCESSOR})
 #####################################
 # Tell how to install this executable
 #####################################
 IF(CMAKE_SYSTEM_NAME STREQUAL "Windows")
     SET(CMAKE_INSTALL_PREFIX "C:\\Program Files\\swiftest")
@@ -191,19 +201,18 @@
     SET(CMAKE_INSTALL_PREFIX ${CMAKE_INSTALL_PREFIX} CACHE PATH "Path for install")
 ELSE()
     SET(CMAKE_INSTALL_PREFIX /usr/local CACHE PATH "Path for install")
 ENDIF()
 
 # Set the name of the swiftest library
 SET(SWIFTEST_LIBRARY ${SKBUILD_PROJECT_NAME})
+IF (USE_COARRAY)
+    SET(SWIFTEST_LIBRARY_CAF ${SWIFTEST_LIBRARY}_caf) 
+ENDIF()
 
-# Determine compiler options
-IF(NOT CMAKE_Fortran_COMPILER_SUPPORTS_F90)
-    MESSAGE(FATAL_ERROR "Fortran compiler does not support F90")
-ENDIF(NOT CMAKE_Fortran_COMPILER_SUPPORTS_F90)
 INCLUDE(SetParallelizationLibrary)
 
 INCLUDE(SetSwiftestFlags) 
 
 SET(CMAKE_POSITION_INDEPENDENT_CODE ON)
 
 # The source for the SWIFTEST binary and have it placed in the bin folder
```

### Comparing `swiftest-2024.4.1/COPYING` & `swiftest-2024.4.2/COPYING`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/Dockerfile.GNU-Linux` & `swiftest-2024.4.2/Dockerfile.GNU-Linux`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/Dockerfile.Intel` & `swiftest-2024.4.2/Dockerfile.Intel`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/LICENSE` & `swiftest-2024.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/README.md` & `swiftest-2024.4.2/README.md`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/README_figs/.DS_Store` & `swiftest-2024.4.2/README_figs/.DS_Store`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/README_tables/add_body_kwargs.md` & `swiftest-2024.4.2/README_tables/add_body_kwargs.md`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/README_tables/save_kwargs.md` & `swiftest-2024.4.2/README_tables/save_kwargs.md`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/README_tables/simulation_kwargs.md` & `swiftest-2024.4.2/README_tables/simulation_kwargs.md`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/README_tables/write_param_kwargs.md` & `swiftest-2024.4.2/README_tables/write_param_kwargs.md`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/buildscripts/windows/hdf5-cacheinit-windows.cmake` & `swiftest-2024.4.2/buildscripts/windows/hdf5-cacheinit-windows.cmake`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/buildscripts/windows/netcdf-c-cacheinit-windows.cmake` & `swiftest-2024.4.2/buildscripts/windows/netcdf-c-cacheinit-windows.cmake`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/buildscripts/windows/netcdf-fortran-cacheinit-windows.cmake` & `swiftest-2024.4.2/buildscripts/windows/netcdf-fortran-cacheinit-windows.cmake`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/cmake/Modules/FindFFTW3.cmake` & `swiftest-2024.4.2/cmake/Modules/FindFFTW3.cmake`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/cmake/Modules/FindNETCDF_Fortran.cmake` & `swiftest-2024.4.2/cmake/Modules/FindNETCDF_Fortran.cmake`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/cmake/Modules/FindOpenMP_Fortran.cmake` & `swiftest-2024.4.2/cmake/Modules/FindOpenMP_Fortran.cmake`

 * *Files 1% similar despite different names*

```diff
@@ -47,19 +47,19 @@
                 "-qopenmp -qno-openmp-simd"  # Intel
             )
         ENDIF (USE_SIMD)
     ENDIF ()
 ELSEIF (COMPILER_OPTIONS STREQUAL "GNU")
     IF (USE_SIMD)
         SET (OpenMP_Fortran_FLAG_CANDIDATES
-            "-fopenmp" # GNU
+            "-fopenmp"
         )
     ELSE ()
         SET (OpenMP_Fortran_FLAG_CANDIDATES
-            "-fopenmp -fno-openmp-simd"                   # GNU
+            "-fopenmp -fno-openmp-simd"   
         )
     ENDIF (USE_SIMD)
 
 ENDIF ()
 
 IF (DEFINED OpenMP_Fortran_FLAGS)
     SET (OpenMP_Fortran_FLAG_CANDIDATES)
```

### Comparing `swiftest-2024.4.1/cmake/Modules/FindSHTOOLS.cmake` & `swiftest-2024.4.2/cmake/Modules/FindSHTOOLS.cmake`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,11 @@
 ADD_LIBRARY(SHTOOLS::parallel UNKNOWN IMPORTED PUBLIC)
 SET_TARGET_PROPERTIES(SHTOOLS::parallel PROPERTIES 
    IMPORTED_LOCATION "${SHTOOLS_LIBRARY_MP}"
    INTERFACE_INCLUDE_DIRECTORIES "${SHTOOLS_INCLUDE_DIR}"
 )
 SET(SHTOOLS_FOUND TRUE)
 
-# These libraries are required
-# How do I get them to link to the SHTOOLS library?
-
 MARK_AS_ADVANCED(SHTOOLS_LIBRARY SHTOOLS_LIBRARY_MP SHTOOLS_INCLUDE_DIR)
 MESSAGE(STATUS "SHTOOLS library: ${SHTOOLS_LIBRARY}")
 MESSAGE(STATUS "SHTOOLS OpenMP library: ${SHTOOLS_LIBRARY_MP}")
 MESSAGE(STATUS "SHTOOLS include dir: ${SHTOOLS_INCLUDE_DIR}")
```

### Comparing `swiftest-2024.4.1/cmake/Modules/SetCompileFlag.cmake` & `swiftest-2024.4.2/cmake/Modules/SetCompileFlag.cmake`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/cmake/Modules/SetParallelizationLibrary.cmake` & `swiftest-2024.4.2/cmake/Modules/SetParallelizationLibrary.cmake`

 * *Files 16% similar despite different names*

```diff
@@ -11,26 +11,12 @@
     # Find OpenMP
     IF (NOT OpenMP_Fortran_FLAGS)
         FIND_PACKAGE (OpenMP_Fortran)
         IF (NOT OpenMP_Fortran_FLAGS)
             MESSAGE (FATAL_ERROR "Fortran compiler does not support OpenMP")
         ENDIF (NOT OpenMP_Fortran_FLAGS)
     ENDIF (NOT OpenMP_Fortran_FLAGS)
-ENDIF (USE_OPENMP)
-
-IF (USE_COARRAY)
-    IF (NOT Coarray_Fortran_FLAGS)
-        FIND_PACKAGE (Coarray_Fortran)
-        IF (NOT Coarray_Fortran_FLAGS)
-            MESSAGE (FATAL_ERROR "Fortran compiler does not support Coarrays")
-        ENDIF (NOT Coarray_Fortran_FLAGS)
-    ENDIF (NOT Coarray_Fortran_FLAGS)
-ENDIF (USE_COARRAY)
-
-IF (NOT USE_OPENMP AND NOT USE_COARRAY)
-    # Turn off both OpenMP and CAF
-    SET (OMP_NUM_PROCS 0 CACHE
-         STRING "Number of processors OpenMP may use" FORCE)
+ELSE()
+    SET (OMP_NUM_PROCS 0 CACHE STRING "Number of processors OpenMP may use" FORCE)
     UNSET (OpenMP_Fortran_FLAGS CACHE)
-    UNSET (Coarray_Fortran_FLAGS CACHE)
     UNSET (GOMP_Fortran_LINK_FLAGS CACHE)
-ENDIF (NOT USE_OPENMP AND NOT USE_COARRAY)
+ENDIF ()
```

### Comparing `swiftest-2024.4.1/cmake/Modules/SetSwiftestFlags.cmake` & `swiftest-2024.4.2/cmake/Modules/SetSwiftestFlags.cmake`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,14 @@
     # Sets the dialect standard but allow for all intrinsics
     SET_COMPILE_FLAG(CMAKE_Fortran_FLAGS "${CMAKE_Fortran_FLAGS}"
         Fortran "-std=gnu"
         )
     SET_COMPILE_FLAG(CMAKE_Fortran_FLAGS "${CMAKE_Fortran_FLAGS}"
         Fortran "-fPIC"
         )
-    
 ELSEIF (COMPILER_OPTIONS STREQUAL "Intel")
     # Disables right margin wrapping in list-directed output
     IF (WINOPT)
         SET_COMPILE_FLAG(CMAKE_Fortran_FLAGS "${CMAKE_Fortran_FLAGS}"
             Fortran  "/wrap-margin-"   # Intel Windows    
         )
         # Aligns a variable to a specified boundary and offset
```

### Comparing `swiftest-2024.4.1/distclean.cmake` & `swiftest-2024.4.2/distclean.cmake`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/docs/Makefile` & `swiftest-2024.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/docs/_static/basic_simulation_a_vs_t_plot.png` & `swiftest-2024.4.2/docs/_static/basic_simulation_a_vs_t_plot.png`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/docs/_static/index_api_reference.svg` & `swiftest-2024.4.2/docs/_static/index_api_reference.svg`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/docs/_static/index_contribute.svg` & `swiftest-2024.4.2/docs/_static/index_contribute.svg`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/docs/_static/index_getting_started.svg` & `swiftest-2024.4.2/docs/_static/index_getting_started.svg`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/docs/_static/index_user_guide.svg` & `swiftest-2024.4.2/docs/_static/index_user_guide.svg`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/docs/_static/logos/swiftest_logo.png` & `swiftest-2024.4.2/docs/_static/logos/swiftest_logo.png`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/docs/_static/logos/swiftest_logo.svg` & `swiftest-2024.4.2/docs/_static/logos/swiftest_logo.svg`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/docs/_static/logos/swiftest_social_preview.png` & `swiftest-2024.4.2/docs/_static/logos/swiftest_social_preview.png`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/docs/_static/logos/swiftest_social_preview.svg` & `swiftest-2024.4.2/docs/_static/logos/swiftest_social_preview.svg`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/docs/_static/style.css` & `swiftest-2024.4.2/docs/_static/style.css`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/docs/_static/symba_gr.png` & `swiftest-2024.4.2/docs/_static/symba_gr.png`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/docs/api.rst` & `swiftest-2024.4.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/docs/conf.py` & `swiftest-2024.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/docs/environment.yml` & `swiftest-2024.4.2/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/docs/getting-started-guide/index.rst` & `swiftest-2024.4.2/docs/getting-started-guide/index.rst`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/docs/index.rst` & `swiftest-2024.4.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/docs/user-guide/basic-simulation.rst` & `swiftest-2024.4.2/docs/user-guide/basic-simulation.rst`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/docs/user-guide/detailed-simulation-setup.rst` & `swiftest-2024.4.2/docs/user-guide/detailed-simulation-setup.rst`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/docs/user-guide/gravitational-harmonics.rst` & `swiftest-2024.4.2/docs/user-guide/gravitational-harmonics.rst`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/docs/user-guide/index.rst` & `swiftest-2024.4.2/docs/user-guide/index.rst`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/docs/user-guide/planetocentric-init_cond.rst` & `swiftest-2024.4.2/docs/user-guide/planetocentric-init_cond.rst`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/docs/user-guide/standalone-executable.rst` & `swiftest-2024.4.2/docs/user-guide/standalone-executable.rst`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/environment.yml` & `swiftest-2024.4.2/environment.yml`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Basic_Simulation/README.txt` & `swiftest-2024.4.2/examples/Basic_Simulation/README.txt`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Basic_Simulation/basic_simulation.py` & `swiftest-2024.4.2/examples/Basic_Simulation/basic_simulation.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Basic_Simulation/output_reader.py` & `swiftest-2024.4.2/examples/Basic_Simulation/output_reader.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Chambers2013/README.txt` & `swiftest-2024.4.2/examples/Chambers2013/README.txt`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Chambers2013/initial_conditions.py` & `swiftest-2024.4.2/examples/Chambers2013/initial_conditions.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Chambers2013/run_simulation.py` & `swiftest-2024.4.2/examples/Chambers2013/run_simulation.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Chambers2013/scattermovie.py` & `swiftest-2024.4.2/examples/Chambers2013/scattermovie.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Fragmentation/Fragmentation_Movie.py` & `swiftest-2024.4.2/examples/Fragmentation/Fragmentation_Movie.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Fragmentation/README.txt` & `swiftest-2024.4.2/examples/Fragmentation/README.txt`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Multibody_Fragmentation/Multibody_Movie.py` & `swiftest-2024.4.2/examples/Multibody_Fragmentation/Multibody_Movie.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Multibody_Fragmentation/README.txt` & `swiftest-2024.4.2/examples/Multibody_Fragmentation/README.txt`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Swifter_Swiftest/108pl_50tp/README.txt` & `swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/README.txt`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Swifter_Swiftest/108pl_50tp/cb.in` & `swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/cb.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Swifter_Swiftest/108pl_50tp/param.swifter.in` & `swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/param.swifter.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Swifter_Swiftest/108pl_50tp/param.swiftest.in` & `swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/param.swiftest.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Swifter_Swiftest/108pl_50tp/pl.swifter.in` & `swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/pl.swifter.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Swifter_Swiftest/108pl_50tp/pl.swiftest.in` & `swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/pl.swiftest.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Swifter_Swiftest/108pl_50tp/swifter_start.in` & `swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/swifter_start.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Swifter_Swiftest/108pl_50tp/swifter_swiftest_comp.eps` & `swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/swifter_swiftest_comp.eps`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Swifter_Swiftest/108pl_50tp/swifter_swiftest_comp.py` & `swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/swifter_swiftest_comp.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Swifter_Swiftest/108pl_50tp/tp.swifter.in` & `swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/tp.swifter.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Swifter_Swiftest/108pl_50tp/tp.swiftest.in` & `swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/tp.swiftest.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Swifter_Swiftest/8pl_0tp/README.txt` & `swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/README.txt`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Swifter_Swiftest/8pl_0tp/cb.swiftest.in` & `swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/cb.swiftest.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Swifter_Swiftest/8pl_0tp/init_cond.py` & `swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/init_cond.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Swifter_Swiftest/8pl_0tp/param.swifter.in` & `swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/param.swifter.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Swifter_Swiftest/8pl_0tp/param.swiftest.in` & `swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/param.swiftest.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Swifter_Swiftest/8pl_0tp/pl.swifter.in` & `swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/pl.swifter.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Swifter_Swiftest/8pl_0tp/pl.swiftest.in` & `swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/pl.swiftest.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Swifter_Swiftest/8pl_0tp/swiftest_symba_vs_swifter_symba.ipynb` & `swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/swiftest_symba_vs_swifter_symba.ipynb`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Swifter_Swiftest/8pl_0tp/tp.swifter.in` & `swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/tp.swifter.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/Swifter_Swiftest/8pl_0tp/tp.swiftest.in` & `swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/tp.swiftest.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/helio_gr_test/README.txt` & `swiftest-2024.4.2/examples/helio_gr_test/README.txt`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/helio_gr_test/helio_gr_test.py` & `swiftest-2024.4.2/examples/helio_gr_test/helio_gr_test.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/rmvs_swifter_comparison/1pl_1tp_encounter/init_cond.py` & `swiftest-2024.4.2/examples/rmvs_swifter_comparison/1pl_1tp_encounter/init_cond.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/rmvs_swifter_comparison/1pl_1tp_encounter/swiftest_vs_swifter.ipynb` & `swiftest-2024.4.2/examples/rmvs_swifter_comparison/1pl_1tp_encounter/swiftest_vs_swifter.ipynb`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/rmvs_swifter_comparison/8pl_16tp_encounters/init_cond.py` & `swiftest-2024.4.2/examples/rmvs_swifter_comparison/8pl_16tp_encounters/init_cond.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/rmvs_swifter_comparison/8pl_16tp_encounters/swiftest_vs_swifter.ipynb` & `swiftest-2024.4.2/examples/rmvs_swifter_comparison/8pl_16tp_encounters/swiftest_vs_swifter.ipynb`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/solar_impact/README.txt` & `swiftest-2024.4.2/examples/solar_impact/README.txt`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/solar_impact/sundiver.py` & `swiftest-2024.4.2/examples/solar_impact/sundiver.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,26 +31,37 @@
 swiftest.log     : An ASCII file containing the information on the status of the simulation as it runs.
 """
 
 import swiftest
 import numpy as np
 
 # Initialize the simulation object as a variable. Arguments may be defined here or through the sim.run() method.
-sim = swiftest.Simulation(compute_conservation_values=True, rotation=True, integrator="symba")
+sim = swiftest.Simulation(simdir='massive_sundiver',compute_conservation_values=True, rotation=True)
 
 # Add the modern planets and the Sun using the JPL Horizons Database.
 sim.add_solar_system_body(["Sun","Mercury","Venus","Earth","Mars","Jupiter","Saturn","Uranus","Neptune","Pluto"])
 
 density  = 3000.0 * sim.KG2MU / sim.M2DU**3
 
 # Make a body with a periapsis inside the Sun's radius
-q = 0.9 * swiftest.RSun * sim.M2DU
+q = 0.01 * swiftest.RSun * sim.M2DU
 a = 0.1
 e = 1.0 - q / a
 M = 2e0 * swiftest.MEarth * sim.KG2MU
 R = (3 * M  / (4 * np.pi * density)) ** (1.0 / 3.0)
 rot = 4 * sim.init_cond.sel(name="Earth")['rot']
 sim.add_body(name="Sundiver", a=a, e=e, inc=0.0, capom=0.0, omega=0.0, capm=180.0, mass=M, radius=R, Ip=[0.4,0.4,0.4], rot=rot)
 sim.get_parameter()
 
 # Run the simulation. Arguments may be defined here or thorugh the swiftest.Simulation() method.
-sim.run(tstart=0.0, tstop=2e-2, dt=0.001, istep_out=1, dump_cadence=0)
+sim.run(tstart=0.0, tstop=5e-2, dt=0.0001, istep_out=1, dump_cadence=0, integrator="rmvs")
+
+sim = swiftest.Simulation(simdir='massless_sundiver',compute_conservation_values=False, integrator="rmvs")
+
+sim.add_solar_system_body(["Sun","Mercury","Venus","Earth","Mars","Jupiter","Saturn","Uranus","Neptune","Pluto"])
+sim.add_body(name="Sundiver", a=a, e=e, inc=0.0, capom=0.0, omega=0.0, capm=180.0)
+sim.get_parameter()
+
+# Run the simulation. Arguments may be defined here or thorugh the swiftest.Simulation() method.
+sim.run(tstart=0.0, tstop=5e-2, dt=0.0001, istep_out=1, dump_cadence=0)
+
+
```

### Comparing `swiftest-2024.4.1/examples/spherical_harmonics_cb/J2_test_pl_and_tp.py` & `swiftest-2024.4.2/examples/spherical_harmonics_cb/J2_test_pl_and_tp.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/spherical_harmonics_cb/J2_test_tp.py` & `swiftest-2024.4.2/examples/spherical_harmonics_cb/J2_test_tp.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/spherical_harmonics_cb/spherical_harmonics_cb.py` & `swiftest-2024.4.2/examples/spherical_harmonics_cb/spherical_harmonics_cb.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/whm_gr_test/README.txt` & `swiftest-2024.4.2/examples/whm_gr_test/README.txt`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/examples/whm_gr_test/whm_gr_test.py` & `swiftest-2024.4.2/examples/whm_gr_test/whm_gr_test.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/fortran_docs.md` & `swiftest-2024.4.2/fortran_docs.md`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/paper/paper.bib` & `swiftest-2024.4.2/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/paper/paper.md` & `swiftest-2024.4.2/paper/paper.md`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/paper/performance.png` & `swiftest-2024.4.2/paper/performance.png`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/pyproject.toml` & `swiftest-2024.4.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "swiftest"
-version = "2024.4.1"
+version = "2024.4.2"
 authors=[
     {name = 'David A. Minton', email='daminton@purdue.edu'},
     {name = 'Carlisle Wishard'},
     {name = 'Jennifer Pouplin'},
     {name = 'Jake Elliott'},
     {name = 'Dana Singh'},
     {name = 'Kaustub Anand'},
@@ -46,14 +46,15 @@
 [project.urls]
 repository = 'https://github.com/MintonGroup/swiftest'
 documentation = 'https://swiftest.readthedocs.io/en/latest/'
 changelog = 'https://swiftest.readthedocs.io/en/latest/whats-new.html'
 
 [project.scripts]
 swiftest = "swiftest.cli:main"
+swiftest_caf = "swiftest.cli:main_caf"
 
 [build-system]
 requires = [
     "python_version>='3.9'",
     "scikit-build-core>=0.8.2",
     "cython>=3.0.8",
     "numpy>=1.26.4",
@@ -74,66 +75,84 @@
     "pytest>=8.0.0",
     "numpy>=1.26.4"
 ]
 skip = "pp* *i686 *-manylinux_i686 *_ppc64le *_s390x *-musllinux* *-win32"
 build-verbosity = 1
 
 [tool.cibuildwheel.macos.environment]
-SKBUILD_CMAKE_ARGS="-DMACHINE_CODE_VALUE=generic"
+SKBUILD_CMAKE_ARGS=["-DMACHINE_CODE_VALUE=generic","-DUSE_COARRAY:BOOL=OFF"]
 PREFIX="$(pwd)/build/deps/usr/local"
 NETCDF_FORTRAN_HOME="${PREFIX}"
 NETCDF_FORTRAN_INCLUDE="${NETCDF_FORTRAN_HOME}/include"
 NETCDF_DIR="${NETCDF_FORTRAN_HOME}/lib/cmake/netCDF"
 NETCDF_FORTRAN_DIR="${NETCDF_FORTRAN_HOME}/lib/cmake/netCDF"
 SHTOOLS_HOME="${PREFIX}"
+ARCH="$(uname -m)"
 MACOSX_DEPLOYMENT_TARGET="$(buildscripts/get_macosx_deployment_target.sh)"
 HOMEBREW_PREFIX="$(brew --prefix)"
-ARCH="$(uname -m)"
-LD_LIBRARY_PATH="${PREFIX}/lib:${HOMEBREW_PREFIX}/lib"
+LD_LIBRARY_PATH="${PREFIX}/lib:${HOMEBREW_PREFIX}/lib:${HOMEBREW_PREFIX}/lib/gcc/${GFORTRAN_VERSION}"
 DYLD_LIBRARY_PATH="${LD_LIBRARY_PATH}"
 REPAIR_LIBRARY_PATH="${LD_LIBRARY_PATH}"
-LDFLAGS="-Wl,-no_compact_unwind -L${PREFIX}/lib -L${HOMEBREW_PREFIX}/lib" 
+LDFLAGS="-Wl,-no_compact_unwind -L${PREFIX}/lib -L${HOMEBREW_PREFIX}/lib -L${HOMEBREW_PREFIX}/lib/gcc/${GFORTRAN_VERSION}" 
 CPATH="${PREFIX}/include:${HOMEBREW_PREFIX}/include"
 CPPFLAGS="-isystem ${PREFIX}/include"
 FCFLAGS="-arch ${ARCH}"
 FFLAGS="${FCFLAGS}"
 CFLAGS="${FCFLAGS} -Wno-deprecated-non-prototype -arch ${ARCH}"
 CXXFLAGS="${CFLAGS}"
-PATH="${PREFIX}/bin:${PATH}"
+MPI_HOME="${HOMEBREW_PREFIX}"
+PATH="${HOMEBREW_PREFIX}/opt/coreutils/libexec/gnubin:${HOMEBREW_PREFIX}/bin:${PREFIX}/bin:${PATH}"
+GFORTRAN_VERSION="$(buildscripts/get_gfortran_version.sh)"
+OMPI_FC="$(buildscripts/get_gfortran_path.sh)"
+CC="mpicc"
+CXX="mpic++"
+FC="mpifort"
+F77="mpifort"
+F95="mpifort"
 
 [tool.cibuildwheel.linux.environment]
-SKBUILD_CMAKE_ARGS="-DMACHINE_CODE_VALUE=generic"
+SKBUILD_CMAKE_ARGS=["-DMACHINE_CODE_VALUE=generic","-DUSE_COARRAY:BOOL=ON"]
 PREFIX="$(pwd)/build/deps/usr/local"
 NETCDF_FORTRAN_HOME="${PREFIX}"
 NETCDF_FORTRAN_INCLUDE="${NETCDF_FORTRAN_HOME}/include"
 NETCDF_DIR="${NETCDF_FORTRAN_HOME}/lib/cmake/netCDF"
 NETCDF_FORTRAN_DIR="${NETCDF_FORTRAN_HOME}/lib/cmake/netCDF"
 SHTOOLS_HOME="${PREFIX}"
+OpenCoarrays_DIR="${PREFIX}/../../opencoarrays/2.10.2/lib64/cmake/opencoarrays"
+OpenCoarrays_HOME="${PREFIX}/../../opencoarrays/2.10.2"
+MPI_HOME="/usr/lib64/openmpi"
 CPATH="${PREFIX}/include:${CPATH}"
-PATH="${PREFIX}/bin:${PATH}"
+PATH="${PREFIX}/bin:${MPI_HOME}/bin:${PATH}"
 LD_LIBRARY_PATH="${PREFIX}/lib:${HOMEBREW_PREFIX}/lib"
 CFLAGS="-Wa,--noexecstack"
 CXXFLAGS="${CFLAGS}"
 LDFLAGS="-L${PREFIX}/lib"
 REPAIR_LIBRARY_PATH="${LD_LIBRARY_PATH}"
+GFORTRAN_VERSION="$(buildscripts/get_gfortran_version.sh)"
+OMPI_FC="$(buildscripts/get_gfortran_path.sh)"
+CC="mpicc"
+CXX="mpic++"
+FC="mpifort"
+F77="mpifort"
+F95="mpifort"
 
 [tool.cibuildwheel.macos]
 before-all = [
-    "brew install coreutils pkg-config fftw vecLibFort;buildscripts/build_dependencies.sh"
+    "brew install coreutils pkg-config fftw vecLibFort opencoarrays open-mpi;buildscripts/build_dependencies.sh"
 ]
 repair-wheel-command = """\
 DYLD_LIBRARY_PATH=$REPAIR_LIBRARY_PATH delocate-wheel \
 --require-archs {delocate_archs} -w {dest_dir} -v {wheel}
 """
 
 [tool.cibuildwheel.linux]
 skip = "pp* *-manylinux_i686* *-musllinux* cp312-*_aarch64*"
 before-all = [
     "yum install epel-release -y",
-    "yum install doxygen libxml2-devel libcurl-devel fftw-static openblas-static -y",
+    "yum install doxygen libxml2-devel libcurl-devel fftw-static openblas-static openmpi-devel -y",
     "buildscripts/build_dependencies.sh"
 ]
 
 [[tool.scikit-build.generate]]
 path = "version.txt"
 location = "source"
 template = '''${version}'''
```

### Comparing `swiftest-2024.4.1/src/CMakeLists.txt` & `swiftest-2024.4.2/src/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -88,25 +88,20 @@
 )
 
 SET(COARRAY_FILES
             ${SRC}/coarray/coarray_module.f90
             ${SRC}/coarray/coarray_clone.f90
             ${SRC}/coarray/coarray_collect.f90
             ${SRC}/swiftest/swiftest_coarray.f90
-            ${SRC}/whm/whm_coarray.f90
-            ${SRC}/rmvs/rmvs_coarray.f90
 )
 
 SET(DRIVER_src ${SRC}/main/main.f90)
 
 # Combine all source files 
 set(SWIFTEST_src ${FAST_MATH_FILES} ${STRICT_MATH_FILES})
-IF(USE_COARRAY)
-    set(SWIFTEST_src ${SWIFTEST_src} ${COARRAY_FILES} )
-ENDIF ()
 
 STRING(TOUPPER "${CMAKE_BUILD_TYPE}" BT)
 
 # Turn preprocessor on for all files
 SET_SOURCE_FILES_PROPERTIES(${SWIFTEST_src} ${DRIVER_src} PROPERTIES Fortran_PREPROCESS ON)
 
 #Set strict vs fast math flags
@@ -122,48 +117,81 @@
 ENDIF()
 
 # Define the executable name
 SET(SWIFTEST_EXE swiftest_exe)
 ADD_EXECUTABLE(${SWIFTEST_EXE} ${DRIVER_src})
 SET_PROPERTY(TARGET ${SWIFTEST_EXE} PROPERTY OUTPUT_NAME swiftest)
 
+IF (USE_COARRAY)
+    SET(SWIFTEST_EXE_CAF swiftest_exe_caf)
+    ADD_EXECUTABLE(${SWIFTEST_EXE_CAF} ${DRIVER_src})
+    SET_PROPERTY(TARGET ${SWIFTEST_EXE_CAF} PROPERTY OUTPUT_NAME swiftest_caf)
+ENDIF()
+
 #####################################################
 # Add the needed libraries 
 #####################################################
 # Create a library from the source files, except the driver
 ADD_LIBRARY(${SWIFTEST_LIBRARY} ${SWIFTEST_src})
+IF (USE_COARRAY)
+    ADD_LIBRARY(${SWIFTEST_LIBRARY_CAF} ${SWIFTEST_src} ${COARRAY_FILES})
+    TARGET_COMPILE_DEFINITIONS(${SWIFTEST_LIBRARY_CAF} PUBLIC -DCOARRAY)
+    TARGET_COMPILE_DEFINITIONS(${SWIFTEST_EXE_CAF} PUBLIC -DCOARRAY)
+    SET_PROPERTY(TARGET ${SWIFTEST_LIBRARY_CAF} PROPERTY Fortran_MODULE_DIRECTORY ${CMAKE_BINARY_DIR}/mod_caf)
+ENDIF()
 
-TARGET_LINK_LIBRARIES(${SWIFTEST_LIBRARY} PUBLIC netCDF::netcdff netCDF::netcdf HDF5::HDF5 hdf5::hdf5_hl-static)
-TARGET_LINK_LIBRARIES(${SWIFTEST_EXE} PUBLIC netCDF::netcdff netCDF::netcdf HDF5::HDF5 hdf5::hdf5_hl-static)
+TARGET_LINK_LIBRARIES(${SWIFTEST_LIBRARY} PUBLIC netCDF::netcdff netCDF::netcdf HDF5::HDF5)
+TARGET_LINK_LIBRARIES(${SWIFTEST_EXE} PUBLIC netCDF::netcdff netCDF::netcdf HDF5::HDF5)
+IF (USE_COARRAY)
+    TARGET_LINK_LIBRARIES(${SWIFTEST_LIBRARY_CAF} PUBLIC netCDF::netcdff netCDF::netcdf HDF5::HDF5)
+    TARGET_LINK_LIBRARIES(${SWIFTEST_EXE_CAF} PUBLIC netCDF::netcdff netCDF::netcdf HDF5::HDF5)
+ENDIF()
 
 IF(USE_OPENMP OR USE_SIMD)
     TARGET_LINK_LIBRARIES(${SWIFTEST_LIBRARY} PUBLIC SHTOOLS::parallel)
     TARGET_LINK_LIBRARIES(${SWIFTEST_EXE} PUBLIC SHTOOLS::parallel)
 
     SET_PROPERTY(TARGET ${SWIFTEST_LIBRARY} ${SWIFTEST_EXE} APPEND_STRING PROPERTY COMPILE_FLAGS  "${OpenMP_Fortran_FLAGS} ")
     SET_PROPERTY(TARGET ${SWIFTEST_LIBRARY} ${SWIFTEST_EXE} APPEND_STRING PROPERTY LINK_FLAGS  "${OpenMP_Fortran_FLAGS} ")
+    IF (USE_COARRAY)
+        TARGET_LINK_LIBRARIES(${SWIFTEST_LIBRARY_CAF} PUBLIC SHTOOLS::parallel)
+        TARGET_LINK_LIBRARIES(${SWIFTEST_EXE_CAF} PUBLIC SHTOOLS::parallel)
+    
+        SET_PROPERTY(TARGET ${SWIFTEST_LIBRARY_CAF} ${SWIFTEST_EXE_CAF} APPEND_STRING PROPERTY COMPILE_FLAGS  "${OpenMP_Fortran_FLAGS} ")
+        SET_PROPERTY(TARGET ${SWIFTEST_LIBRARY_CAF} ${SWIFTEST_EXE_CAF} APPEND_STRING PROPERTY LINK_FLAGS  "${OpenMP_Fortran_FLAGS} ")
+    ENDIF()
 ELSE ()
     TARGET_LINK_LIBRARIES(${SWIFTEST_LIBRARY} PUBLIC SHTOOLS::serial)
     TARGET_LINK_LIBRARIES(${SWIFTEST_EXE} PUBLIC SHTOOLS::serial)
+    IF (USE_COARRAY)
+        TARGET_LINK_LIBRARIES(${SWIFTEST_LIBRARY_CAF} PUBLIC SHTOOLS::serial)
+        TARGET_LINK_LIBRARIES(${SWIFTEST_EXE_CAF} PUBLIC SHTOOLS::serial)
+    ENDIF()
 ENDIF()
 
 TARGET_LINK_LIBRARIES(${SWIFTEST_LIBRARY} PUBLIC BLAS::BLAS LAPACK::LAPACK FFTW3::FFTW3)
 
+IF(USE_COARRAY)
+    SET_PROPERTY(TARGET ${SWIFTEST_LIBRARY_CAF} ${SWIFTEST_EXE_CAF} APPEND_STRING PROPERTY COMPILE_FLAGS "${COARRAY_Fortran_FLAGS} ")
+    SET_PROPERTY(TARGET ${SWIFTEST_LIBRARY_CAF} ${SWIFTEST_EXE_CAF} APPEND_STRING PROPERTY LINK_FLAGS "${COARRAY_Fortran_FLAGS} ")
+    TARGET_LINK_LIBRARIES(${SWIFTEST_LIBRARY_CAF} PUBLIC BLAS::BLAS LAPACK::LAPACK FFTW3::FFTW3 OpenCoarrays::caf_mpi MPI::MPI_Fortran)
+ENDIF(USE_COARRAY)
+
 TARGET_LINK_LIBRARIES(${SWIFTEST_EXE} PUBLIC ${SWIFTEST_LIBRARY})
+IF (USE_COARRAY)
+    TARGET_LINK_LIBRARIES(${SWIFTEST_EXE_CAF} PUBLIC ${SWIFTEST_LIBRARY_CAF})
+ENDIF()
 
 IF (CMAKE_SYSTEM_NAME STREQUAL "Windows")
    SET_PROPERTY(TARGET ${SWIFTEST_LIBRARY} ${SWIFTEST_EXE} APPEND_STRING PROPERTY LINK_FLAGS  "/NODEFAULTLIB")
+   IF (USE_COARRAY)
+       SET_PROPERTY(TARGET ${SWIFTEST_LIBRARY_CAF} ${SWIFTEST_EXE_CAF} APPEND_STRING PROPERTY LINK_FLAGS  "/NODEFAULTLIB")
+    ENDIF()
 ENDIF()
 
-IF(USE_COARRAY)
-    TARGET_COMPILE_DEFINITIONS(${SWIFTEST_LIBRARY} PUBLIC -DCOARRAY)
-    TARGET_COMPILE_DEFINITIONS(${SWIFTEST_EXE} PUBLIC -DCOARRAY)
-    SET_PROPERTY(TARGET ${SWIFTEST_LIBRARY} ${SWIFTEST_EXE} APPEND_STRING PROPERTY COMPILE_FLAGS  "${Coarray_Fortran_FLAGS} ")
-    SET_PROPERTY(TARGET ${SWIFTEST_LIBRARY} ${SWIFTEST_EXE} APPEND_STRING PROPERTY LINK_FLAGS  "${Coarray_Fortran_FLAGS} ")
-ENDIF(USE_COARRAY)
 
 # Check to see if the compiler allows for local-spec in do concurrent statements. Set a preprocessor variable if it does
 SET(TESTFILE "${CMAKE_BINARY_DIR}/${CMAKE_FILES_DIRECTORY}")
 SET(TESTFILE "${TESTFILE}/CMakeTmp/testFortranDoConcurrentLoc.f90")
 FILE(WRITE "${TESTFILE}"
 "
 program TestDoConcurrentLoc
@@ -228,13 +256,22 @@
 ENDIF ()
 
 IF (CMAKE_SYSTEM_NAME STREQUAL "Linux")
     SET_PROPERTY(TARGET ${SWIFTEST_LIBRARY} APPEND_STRING PROPERTY LINK_FLAGS  "-Wl,-z,noexecstack")
 ENDIF()
 
 # Define the install locations
-INSTALL(TARGETS ${SWIFTEST_EXE} ${SWIFTEST_LIBRARY} 
-    RUNTIME DESTINATION ${INSTALL_BINDIR}
-    LIBRARY DESTINATION ${INSTALL_LIBDIR}
-    ARCHIVE DESTINATION ${INSTALL_LIBDIR}
-    INCLUDES DESTINATION ${INSTALL_INCLUDEDIR}
-)
+IF (USE_COARRAY)
+    INSTALL(TARGETS ${SWIFTEST_EXE} ${SWIFTEST_LIBRARY} ${SWIFTEST_EXE_CAF} ${SWIFTEST_LIBRARY_CAF} 
+        RUNTIME DESTINATION ${INSTALL_BINDIR}
+        LIBRARY DESTINATION ${INSTALL_LIBDIR}
+        ARCHIVE DESTINATION ${INSTALL_LIBDIR}
+        INCLUDES DESTINATION ${INSTALL_INCLUDEDIR}
+    )
+ELSE()
+    INSTALL(TARGETS ${SWIFTEST_EXE} ${SWIFTEST_LIBRARY} 
+        RUNTIME DESTINATION ${INSTALL_BINDIR}
+        LIBRARY DESTINATION ${INSTALL_LIBDIR}
+        ARCHIVE DESTINATION ${INSTALL_LIBDIR}
+        INCLUDES DESTINATION ${INSTALL_INCLUDEDIR}
+    )
+ENDIF()
```

### Comparing `swiftest-2024.4.1/src/base/base_module.f90` & `swiftest-2024.4.2/src/base/base_module.f90`

 * *Files 7% similar despite different names*

```diff
@@ -165,16 +165,16 @@
          !! Initial orbital energy 
       real(DP)                  :: GMtot_orig   = 0.0_DP  
          !! Initial system mass 
       real(DP), dimension(NDIM) :: L_total_orig = 0.0_DP  
          !! Initial total angular momentum vector 
       real(DP), dimension(NDIM) :: L_orbit_orig = 0.0_DP  
          !! Initial orbital angular momentum 
-      real(DP), dimension(NDIM) :: L_spin_orig  = 0.0_DP  
-         !! Initial spin angular momentum vector 
+      real(DP), dimension(NDIM) :: L_rot_orig  = 0.0_DP  
+         !! Initial rotational angular momentum vector 
       real(DP), dimension(NDIM) :: L_escape     = 0.0_DP  
          !! Angular momentum of escaped bodies (used for bookeeping) 
       real(DP)                  :: GMescape     = 0.0_DP  
          !! Mass of bodies that escaped the system (used for bookeeping) 
       real(DP)                  :: E_collisions = 0.0_DP  
          !! Energy lost from system due to collisions 
       real(DP)                  :: E_untracked  = 0.0_DP  
@@ -202,17 +202,14 @@
          !! Turn on YORP effect 
    contains
       procedure :: dealloc => base_util_dealloc_param
       procedure(abstract_io_dump_param),      deferred :: dump
       procedure(abstract_io_param_reader),    deferred :: reader
       procedure(abstract_io_param_writer),    deferred :: writer    
       procedure(abstract_io_read_in_param),   deferred :: read_in 
-#ifdef COARRAY
-      procedure :: coclone => base_coclone_param
-#endif
    end type base_parameters
 
    abstract interface
       subroutine abstract_io_dump_param(self, param_file_name)
          import base_parameters
          implicit none
          class(base_parameters),intent(in)    :: self            
@@ -737,36 +734,42 @@
          character(*), parameter :: SUCCESS_MSG = '(/, "Normal termination of Swiftest (version ", A, ")")'
          character(*), parameter :: FAIL_MSG = '(/, "Terminating Swiftest (version ", A, ") due to error!")' 
          character(*), parameter :: USAGE_MSG = '("Usage: swiftest <whm|helio|rmvs|symba> <paramfile> ' // &
                                                 '[{standard}|compact|progress]")'
          character(*), parameter :: HELP_MSG  = USAGE_MSG
          integer(I4B) :: iu
 
-         if (present(unit)) then
-            iu = unit
-         else
-            iu = OUTPUT_UNIT
+#ifdef COARRAY
+         if (this_image() == 1) then
+#endif 
+            if (present(unit)) then
+               iu = unit
+            else
+               iu = OUTPUT_UNIT
+            end if
+      
+            select case(code)
+            case(SUCCESS)
+               write(iu, SUCCESS_MSG) VERSION
+               write(iu, BAR)
+            case(USAGE) 
+               write(iu, USAGE_MSG)
+            case(HELP)
+               write(iu, HELP_MSG)
+            case default
+               write(iu, FAIL_MSG) VERSION
+               write(iu, BAR)
+               error stop -1
+            end select
+#ifdef COARRAY
          end if
-   
-         select case(code)
-         case(SUCCESS)
-            write(iu, SUCCESS_MSG) VERSION
-            write(iu, BAR)
-         case(USAGE) 
-            write(iu, USAGE_MSG)
-         case(HELP)
-            write(iu, HELP_MSG)
-         case default
-            write(iu, FAIL_MSG) VERSION
-            write(iu, BAR)
-            stop 
-         end select
-   
+#endif 
          stop
    
+         return
       end subroutine base_util_exit
 
 
       subroutine base_util_fill_arr_char_string(keeps, inserts, lfill_list)
          !! author: David A. Minton 
          !! 
          !! Performs a fill operation on a single array of type character strings.
@@ -2420,102 +2423,9 @@
          type(base_storage_frame) :: self
    
          if (allocated(self%item)) deallocate(self%item)
    
          return
       end subroutine base_final_storage_frame
 
-#ifdef COARRAY
-      subroutine base_coclone_param(self)
-         !! author: David A. Minton 
-         !! 
-         !! Broadcasts the image 1 parameter to all other images in a parameter coarray 
-         implicit none
-         ! Arguments
-         class(base_parameters),intent(inout),codimension[*]  :: self  
-            !! Collection of parameters 
-         ! Internals
-
-         call coclone(self%integrator)
-         call coclone(self%param_file_name)
-         call coclone(self%t0)
-         call coclone(self%tstart)
-         call coclone(self%tstop)
-         call coclone(self%dt)
-         call coclone(self%iloop)
-         call coclone(self%nloops)
-         call coclone(self%incbfile)
-         call coclone(self%inplfile)
-         call coclone(self%intpfile)
-         call coclone(self%nc_in)
-         call coclone(self%in_type)
-         call coclone(self%in_form)
-         call coclone(self%istep_out)
-         call coclone(self%nstep_out)
-         call coclone(self%fstep_out)
-         call coclone(self%ltstretch)
-         call coclone(self%outfile)
-         call coclone(self%out_type)
-         call coclone(self%out_form)
-         call coclone(self%out_stat)
-         call coclone(self%dump_cadence)
-         call coclone(self%rmin)
-         call coclone(self%rmax)
-         call coclone(self%rmaxu)
-         call coclone(self%qmin)
-         call coclone(self%qmin_coord)
-         call coclone(self%qmin_alo)
-         call coclone(self%qmin_ahi)
-         call coclone(self%MU2KG)
-         call coclone(self%TU2S)
-         call coclone(self%DU2M)
-         call coclone(self%GU)
-         call coclone(self%inv_c2)
-         call coclone(self%GMTINY)
-         call coclone(self%min_GMfrag)
-         call coclone(self%nfrag_reduction)
-         call coclone(self%lmtiny_pl)
-         call coclone(self%collision_model)
-         call coclone(self%encounter_save)
-         call coclone(self%lenc_save_trajectory)
-         call coclone(self%lenc_save_closest)
-         call coclone(self%interaction_loops)
-         call coclone(self%encounter_check_plpl)
-         call coclone(self%encounter_check_pltp)
-         call coclone(self%lflatten_interactions)
-         call coclone(self%lencounter_sas_plpl)
-         call coclone(self%lencounter_sas_pltp)
-         call coclone(self%lrhill_present)
-         call coclone(self%lextra_force)
-         call coclone(self%lbig_discard)
-         call coclone(self%lclose)
-         call coclone(self%lenergy)
-         call coclone(self%lnon_spherical_cb)
-         call coclone(self%lrotation)
-         call coclone(self%ltides)
-         call coclone(self%E_orbit_orig)
-         call coclone(self%GMtot_orig)
-         call coclonevec(self%L_total_orig)
-         call coclonevec(self%L_orbit_orig)
-         call coclonevec(self%L_spin_orig)
-         call coclonevec(self%L_escape)
-         call coclone(self%GMescape)
-         call coclone(self%E_collisions)
-         call coclone(self%E_untracked)
-         call coclone(self%lfirstenergy)
-         call coclone(self%lfirstkick)
-         call coclone(self%lrestart)
-         call coclone(self%display_style)
-         call coclone(self%display_unit)
-         call coclone(self%log_output )
-         call coclone(self%lgr)
-         call coclone(self%lyarkovsky)
-         call coclone(self%lyorp)
-         call coclone(self%seed)
-         call coclone(self%lcoarray)
-
-         return
-      end subroutine base_coclone_param 
-#endif
-    
 
 end module base
```

### Comparing `swiftest-2024.4.1/src/bindings/bindings_module.f90` & `swiftest-2024.4.2/src/bindings/bindings_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/coarray/coarray_collect.f90` & `swiftest-2024.4.2/src/coarray/coarray_collect.f90`

 * *Files 17% similar despite different names*

```diff
@@ -10,49 +10,47 @@
 submodule (coarray) s_coarray_collect
    use swiftest
 contains
 
    module subroutine coarray_component_collect_DP_arr1D(var,dest_img)
       !! author: David A. Minton
       !!
-      !! Collects components of a coarray derived type from all images and combines them into destination image component. The default destination image is 1
+      !! Collects components of a coarray derived type from all images and combines them into destination image component. 
+      !! The default destination image is 1
       !! real(DP) 1D allocatable array version
       implicit none
       ! Arguments
       real(DP), dimension(:), allocatable, intent(inout) :: var
       integer(I4B), intent(in),optional :: dest_img
       ! Internals
       real(DP), dimension(:), codimension[:], allocatable :: tmp
-      integer(I4B) :: i,img, ti, di, istart, iend, nmax
-      integer(I4B), allocatable :: n[:]
+      integer(I4B) :: i,img, ti, di, istart, iend
+      integer(I4B), allocatable :: n[:],nmax[:]
       logical, allocatable :: isalloc[:]
       real(DP), dimension(:), allocatable :: vari1
 
       allocate(isalloc[*])
       allocate(n[*])
+      allocate(nmax[*])
 
       if (present(dest_img)) then
          di = dest_img
       else
          di = 1
       end if
 
       isalloc = allocated(var)
       if (isalloc) then
          n = size(var)
       else
          n = 0
       end if
 
-      sync all
-
-      nmax = 0
-      do img = 1, num_images()
-         if (n[img] > nmax) nmax = n[img]
-      end do
+      nmax = n
+      call co_max(nmax)
 
       allocate(tmp(nmax)[*])
       if (isalloc) tmp(1:n) = var(1:n)
 
       if (this_image() == di) then
          do img = 1, num_images()
             if (img /= di) then
@@ -69,186 +67,108 @@
 
       deallocate(isalloc,n,tmp)
 
       return
    end subroutine coarray_component_collect_DP_arr1D
 
 
-   module subroutine coarray_component_collect_DP_arr2D(var,dest_img)
+   module subroutine coarray_component_collect_DP_vec2D(var,dest_img)
       !! author: David A. Minton
       !!
       !! Collects components of a coarray derived type from all images and combines them into destination image component . The default destination image is 1
       !! real(DP) 2D allocatable array version
       implicit none
       ! Arguments
       real(DP), dimension(:,:), allocatable, intent(inout) :: var
       integer(I4B), intent(in),optional :: dest_img
       ! Internals
       real(DP), dimension(:,:), codimension[:], allocatable :: tmp
-      integer(I4B) :: i, img, ti, di, ntot, istart, iend, nmax
-      integer(I4B), allocatable :: n1[:], n2[:]
+      integer(I4B) :: i, img, ti, di, istart, iend
+      integer(I4B), allocatable :: n[:], nmax[:]
       logical, allocatable :: isalloc[:]
       real(DP), dimension(:,:), allocatable :: vari1
 
-      allocate(n1[*])
-      allocate(n2[*])
+      allocate(n[*])
+      allocate(nmax[*])
       allocate(isalloc[*])
 
       if (present(dest_img)) then
          di = dest_img
       else
          di = 1
       end if
 
       isalloc = allocated(var)
       if (isalloc) then
-         n1 = size(var,dim=1)
-         n2 = size(var,dim=2)
+         n = size(var,dim=2)
       else
-         n1 = 0
-         n2 = 0
+         n = 0
       end if
-      sync all
-
-      nmax = 0
-      do img = 1, num_images()
-         if (n2[img] > nmax) nmax = n2[img]
-      end do
+      nmax = n
+      call co_max(nmax)
 
       allocate(tmp(NDIM,nmax)[*])
-      if (isalloc) tmp(:,1:n2) = var(:,1:n2)
+      if (isalloc) tmp(:,1:n) = var(:,1:n)
 
       if (this_image() == di) then
          do img = 1, num_images()
-            if (img /= di) then
-               allocate(vari1,source=tmp(:,1:n2[img])[img])
+            if ((img /= di).and.(isalloc[img])) then
+               allocate(vari1,source=tmp(:,1:n[img])[img])
                call util_append(var, vari1)
-               n2 = n2 + n2[img]
+               n = n + n[img]
             end if
          end do
          sync images(*)
       else
          sync images(di)
          if (allocated(var)) deallocate(var)
       end if
 
-      deallocate(isalloc,n1,n2,tmp)
-
-      return
-   end subroutine coarray_component_collect_DP_arr2D
-
-
-   module subroutine coarray_component_collect_I4B(var,dest_img)
-      !! author: David A. Minton
-      !!
-      !! Sums this component of a coarray derived type from all images and places the value in the destination image component. The default destination image is 1
-      !! integer(I4B) version
-      implicit none
-      ! Arguments
-      integer(I4B), intent(inout) :: var
-      integer(I4B), intent(in),optional :: dest_img
-      ! Internals
-      integer(I4B), allocatable :: tmp[:]
-      integer(I4B) :: img, di
-
-      if (present(dest_img)) then
-         di = dest_img
-      else
-         di = 1
-      end if
-
-      allocate(tmp[*], source=var)
-      
-      if (this_image() == di) then
-         var = 0
-         do img = 1, num_images()
-            var = var + tmp[img]
-         end do
-      else
-         var = 0
-      end if
-
-      deallocate(tmp)
+      deallocate(isalloc,n,nmax,tmp)
 
       return
-   end subroutine coarray_component_collect_I4B
-
-
-   module subroutine coarray_component_collect_I8B(var,dest_img)
-      !! author: David A. Minton
-      !!
-      !! Sums this component of a coarray derived type from all images and places the value in the destination image component. The default destination image is 1
-      !! integer(I8B) version
-      implicit none
-      ! Arguments
-      integer(I8B), intent(inout) :: var
-      integer(I4B), intent(in),optional :: dest_img
-      ! Internals
-      integer(I8B), allocatable :: tmp[:]
-      integer(I4B) :: img, di
-
-      if (present(dest_img)) then
-         di = dest_img
-      else
-         di = 1
-      end if
-
-      allocate(tmp[*], source=var)
-      
-      if (this_image() == di) then
-         var = 0
-         do img = 1, num_images()
-            var = var + tmp[img]
-         end do
-      else
-         var = 0
-      end if
-
-      deallocate(tmp)
-
-      return
-   end subroutine coarray_component_collect_I8B
+   end subroutine coarray_component_collect_DP_vec2D
 
 
    module subroutine coarray_component_collect_I4B_arr1D(var,dest_img)
       !! author: David A. Minton
       !!
-      !! Collects components of a coarray derived type from all images and combines them into destination image component . The default destination image is 1
+      !! Collects components of a coarray derived type from all images and combines them into destination image component. 
+      !! The default destination image is 1
       !! integer(I4B) 1D allocatable array version
       implicit none
       ! Arguments
       integer(I4B), dimension(:), allocatable, intent(inout) :: var
       integer(I4B), intent(in),optional :: dest_img
       ! Internals
       integer(I4B), dimension(:), codimension[:], allocatable :: tmp
-      integer(I4B) :: i,img, ti, di, istart, iend, nmax
-      integer(I4B), allocatable :: n[:]
-      logical, allocatable :: isalloc[:]
+      integer(I4B) :: i,img, ti, di, istart, iend
+      integer(I4B), allocatable, codimension[:] :: n, nmax
+      logical, allocatable, codimension[:] :: isalloc[:]
       integer(I4B), dimension(:), allocatable :: vari1
 
       allocate(isalloc[*])
       allocate(n[*])
+      allocate(nmax[*])
 
       if (present(dest_img)) then
          di = dest_img
       else
          di = 1
       end if
 
       isalloc = allocated(var)
       if (isalloc) then
          n = size(var)
       else
          n = 0
       end if
+      nmax = n
       sync all
-      nmax = 0
-      do img = 1, num_images()
-         if (n[img] > nmax) nmax = n[img]
-      end do
+      call co_max(nmax)
 
       allocate(tmp(nmax)[*])
       if (isalloc) tmp(1:n) = var(1:n)
 
       if (this_image() == di) then
          do img = 1, num_images()
             if (img /= di) then
@@ -268,48 +188,46 @@
       return
    end subroutine coarray_component_collect_I4B_arr1D
 
 
    module subroutine coarray_component_collect_lgt_arr1D(var,dest_img)
       !! author: David A. Minton
       !!
-      !! Collects components of a coarray derived type from all images and combines them into destination image component . The default destination image is 1
+      !! Collects components of a coarray derived type from all images and combines them into destination image component. 
+      !! The default destination image is 1
       !! logical 1D allocatable array version
       implicit none
       ! Arguments
       logical, dimension(:), allocatable, intent(inout) :: var
       integer(I4B), intent(in),optional :: dest_img
       ! Internals
       logical, dimension(:), codimension[:], allocatable :: tmp
       integer(I4B) :: i,img, ti, di, ntot, istart, iend, nmax
-      integer(I4B), allocatable :: n[:]
+      integer(I4B), allocatable :: n[:], nmax[:]
       logical, allocatable :: isalloc[:]
       logical, dimension(:), allocatable :: vari1
 
       allocate(isalloc[*])
       allocate(n[*])
+      allocate(nmax[*])
 
       if (present(dest_img)) then
          di = dest_img
       else
          di = 1
       end if
 
       isalloc = allocated(var)
       if (isalloc) then
          n = size(var)
       else
          n = 0
       end if
-      sync all
-      nmax = 0
-      do img = 1, num_images()
-         if (n[img] > nmax) nmax = n[img]
-      end do
-
+      nmax = n
+      call co_max(nmax)
       allocate(tmp(nmax)[*])
       if (isalloc) tmp(1:n) = var(1:n)
 
       if (this_image() == di) then
          do img = 1, num_images()
             if (img /= di) then
                allocate(vari1, source=tmp(1:n[img])[img])
@@ -324,10 +242,8 @@
       end if
 
       deallocate(isalloc,n,tmp)
 
       return
    end subroutine coarray_component_collect_lgt_arr1D
 
-
-
 end submodule s_coarray_collect
```

### Comparing `swiftest-2024.4.1/src/collision/collision_check.f90` & `swiftest-2024.4.2/src/collision/collision_check.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/collision/collision_generate.f90` & `swiftest-2024.4.2/src/collision/collision_generate.f90`

 * *Files 2% similar despite different names*

```diff
@@ -18,36 +18,44 @@
       !! Merge massive bodies no matter the regime
       !! 
       !! Adapted from David E. Kaufmann's Swifter routines symba_merge_pl.f90 and symba_discard_merge_pl.f90
       !!
       !! Adapted from Hal Levison's Swift routines symba5_merge.f and discard_mass_merge.f
       implicit none
       ! Arguments
-      class(collision_basic),   intent(inout) :: self         !! Merge fragment system object 
-      class(base_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(base_parameters),   intent(inout) :: param        !! Current run configuration parameters 
-      real(DP),                 intent(in)    :: t            !! The time of the collision
+      class(collision_basic),   intent(inout) :: self         
+         !! Merge fragment system object 
+      class(base_nbody_system), intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(base_parameters),   intent(inout) :: param        
+         !! Current run configuration parameters 
+      real(DP),                 intent(in)    :: t            
+         !! The time of the collision
 
       call self%merge(nbody_system, param, t)
 
       return
    end subroutine collision_generate_basic
 
 
    module subroutine collision_generate_bounce(self, nbody_system, param, t)
       !! author: David A. Minton
       !!
       !! In this collision model, if the collision would result in a disruption, the bodies are instead "bounced" off 
       !! of the center of mass. This is done as a reflection in the 2-body equivalent distance vector direction.
       implicit none
       ! Arguments
-      class(collision_bounce),  intent(inout) :: self         !! Bounce fragment system object 
-      class(base_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(base_parameters),   intent(inout) :: param        !! Current run configuration parameters 
-      real(DP),                 intent(in)    :: t            !! The time of the collision
+      class(collision_bounce),  intent(inout) :: self         
+         !! Bounce fragment system object 
+      class(base_nbody_system), intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(base_parameters),   intent(inout) :: param        
+         !! Current run configuration parameters 
+      real(DP),                 intent(in)    :: t            
+         !! The time of the collision
       ! Internals
       integer(I4B) :: i,j,nimp
       logical, dimension(:), allocatable :: lmask
 
       select type(nbody_system)
       class is (swiftest_nbody_system)
       select type (pl => nbody_system%pl)
@@ -98,23 +106,27 @@
    end subroutine collision_generate_bounce
 
    
    module subroutine collision_generate_hitandrun(self, nbody_system, param, t) 
       !! author: Jennifer L.L. Pouplin, Carlisle A. Wishard, and David A. Minton
       !!
       !! Create the fragments resulting from a non-catastrophic hit-and-run collision
-      !! 
       implicit none
       ! Arguments
-      class(collision_basic),   intent(inout) :: self         !! Collision system object
-      class(base_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(base_parameters),   intent(inout) :: param        !! Current run configuration parameters with SyMBA additions
-      real(DP),                 intent(in)    :: t            !! Time of collision
+      class(collision_basic),   intent(inout) :: self         
+         !! Collision system object
+      class(base_nbody_system), intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(base_parameters),   intent(inout) :: param        
+         !! Current run configuration parameters with SyMBA additions
+      real(DP),                 intent(in)    :: t            
+         !! Time of collision
       ! Result
-      integer(I4B)                            :: status           !! Status flag assigned to this outcome
+      integer(I4B)                            :: status           
+         !! Status flag assigned to this outcome
       ! Internals
       character(len=STRMAX) :: message
       logical, dimension(:), allocatable :: lmask
 
       select type(nbody_system)
       class is (swiftest_nbody_system)
       select type(pl => nbody_system%pl)
@@ -161,22 +173,26 @@
       !! Merge massive bodies in any collisional system.
       !! 
       !! Adapted from David E. Kaufmann's Swifter routines symba_merge_pl.f90 and symba_discard_merge_pl.f90
       !!
       !! Adapted from Hal Levison's Swift routines symba5_merge.f and discard_mass_merge.f
       implicit none
       ! Arguments
-      class(collision_basic),   intent(inout) :: self         !! Merge fragment system object 
-      class(base_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(base_parameters),   intent(inout) :: param        !! Current run configuration parameters 
-      real(DP),                 intent(in)    :: t            !! The time of the collision
+      class(collision_basic),   intent(inout) :: self         
+         !! Merge fragment system object 
+      class(base_nbody_system), intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(base_parameters),   intent(inout) :: param        
+         !! Current run configuration parameters 
+      real(DP),                 intent(in)    :: t            
+         !! The time of the collision
       ! Internals
       integer(I4B)                              :: i, j, ibiggest
       integer(I8B)                              :: k
-      real(DP), dimension(NDIM)                 :: L_spin_new, L_residual
+      real(DP), dimension(NDIM)                 :: L_rot_new, L_residual
       real(DP)                                  :: volume
       character(len=STRMAX) :: message
 
       select type(nbody_system)
       class is (swiftest_nbody_system)
          associate(impactors => self%impactors)
             message = "Merging"
@@ -206,24 +222,25 @@
                   volume = 4._DP / 3._DP * PI * sum(impactors%radius(:)**3)
                   fragments%mass(1) = sum(impactors%mass(:))
                   fragments%Gmass(1) =sum(impactors%Gmass(:))
                   fragments%density(1) = fragments%mass(1) / volume
                   fragments%radius(1) = (3._DP * volume / (4._DP * PI))**(THIRD)
                   if (param%lrotation) then
 #ifdef DOCONLOC
-                     do concurrent(i = 1:NDIM) shared(impactors, fragments, L_spin_new)
+                     do concurrent(i = 1:NDIM) shared(impactors, fragments, L_rot_new)
 #else
                      do concurrent(i = 1:NDIM)
 #endif
                         fragments%Ip(i,1) = sum(impactors%mass(:) * impactors%Ip(i,:)) 
-                        L_spin_new(i) = sum(impactors%L_orbit(i,:) + impactors%L_spin(i,:))
+                        L_rot_new(i) = sum(impactors%L_orbit(i,:) + impactors%L_rot(i,:))
                      end do
                      fragments%Ip(:,1) = fragments%Ip(:,1) / fragments%mass(1)
-                     fragments%rot(:,1) = L_spin_new(:) / (fragments%Ip(3,1) * fragments%mass(1) * fragments%radius(1)**2)
-                  else ! If spin is not enabled, we will consider the lost pre-collision angular momentum as "escaped" and add it to our bookkeeping variable
+                     fragments%rot(:,1) = L_rot_new(:) / (fragments%Ip(3,1) * fragments%mass(1) * fragments%radius(1)**2)
+                  else ! If rotation is not enabled, we will consider the lost pre-collision angular momentum as "escaped" and add 
+                       ! it to our bookkeeping variable
                      nbody_system%L_escape(:) = nbody_system%L_escape(:) + impactors%L_orbit(:,1) + impactors%L_orbit(:,2) 
                   end if
 
                   ! The fragment trajectory will be the barycentric trajectory
                   fragments%rb(:,1) = impactors%rbcom(:)
                   fragments%vb(:,1) = impactors%vbcom(:)
                   fragments%rc(:,1) = 0.0_DP
@@ -244,15 +261,17 @@
                            nbody_system%plpl_encounter%id1(k) = pl%id(ibiggest)
                            nbody_system%plpl_encounter%index1(k) = i
                         end if
                         if (nbody_system%plpl_encounter%id2(k) == pl%id(i)) then
                            nbody_system%plpl_encounter%id2(k) = pl%id(ibiggest)
                            nbody_system%plpl_encounter%index2(k) = i
                         end if
-                        if (nbody_system%plpl_encounter%id1(k) == nbody_system%plpl_encounter%id2(k)) nbody_system%plpl_encounter%status(k) = INACTIVE
+                        if (nbody_system%plpl_encounter%id1(k) == nbody_system%plpl_encounter%id2(k)) then
+                           nbody_system%plpl_encounter%status(k) = INACTIVE
+                        end if
                      end do
                   end do
 
                   self%status = MERGED
                   
                   call collision_resolve_mergeaddsub(nbody_system, param, t, self%status)
```

### Comparing `swiftest-2024.4.1/src/collision/collision_io.f90` & `swiftest-2024.4.2/src/collision/collision_io.f90`

 * *Files 18% similar despite different names*

```diff
@@ -165,46 +165,69 @@
             end if
 
             call netcdf_io_check( nf90_create(nc%file_name, NF90_NETCDF4, nc%id), &
                "collision_io_netcdf_initialize_output nf90_create" )
             nc%lfile_is_open = .true.
 
             ! Dimensions
-            call netcdf_io_check( nf90_def_dim(nc%id, nc%collision_id_varname, NF90_UNLIMITED, nc%collision_id_dimid), & 
+            call netcdf_io_check( nf90_def_dim(nc%id, &
+                                               nc%collision_id_dimname, &
+                                               NF90_UNLIMITED, &
+                                               nc%collision_id_dimid), & 
                "collision_io_netcdf_initialize_output nf90_def_dim collision_id_dimid"  ) ! Dimension to store collision events
-            call netcdf_io_check( nf90_def_dim(nc%id, nc%space_dimname,        NDIM,           nc%space_dimid), &
+
+            call netcdf_io_check( nf90_def_dim(nc%id, &
+                                               nc%collision_body_dimname, &
+                                               NF90_UNLIMITED, &
+                                               nc%collision_body_dimid), & 
+                "collision_io_netcdf_initialize_output nf90_def_dim collision_body_dimid") ! Dimension to store list of bodies
+
+            call netcdf_io_check( nf90_def_dim(nc%id, &
+                                               nc%space_dimname, &
+                                               NDIM, &
+                                               nc%space_dimid), &
                "collision_io_netcdf_initialize_output nf90_def_dim space_dimid") ! 3D space dimension
-            call netcdf_io_check( nf90_def_dim(nc%id, nc%name_dimname,         NF90_UNLIMITED, nc%name_dimid), & 
-               "collision_io_netcdf_initialize_output nf90_def_dim name_dimid") ! Dimension to store particle id numbers
-            call netcdf_io_check( nf90_def_dim(nc%id, nc%str_dimname,          NAMELEN,        nc%str_dimid), &
-                "collision_io_netcdf_initialize_output nf90_def_dim str_dimid") ! Dimension for string variables (character arrays)
-            call netcdf_io_check( nf90_def_dim(nc%id, nc%stage_dimname,        2,              nc%stage_dimid), &
+
+            call netcdf_io_check( nf90_def_dim(nc%id, &
+                                               nc%str_dimname, &
+                                               NAMELEN, &
+                                               nc%str_dimid), &
+               "collision_io_netcdf_initialize_output nf90_def_dim str_dimid") ! Dimension for string variables 
+
+            call netcdf_io_check( nf90_def_dim(nc%id, &
+                                               nc%stage_dimname, &
+                                               2, &
+                                               nc%stage_dimid), &
                "collision_io_netcdf_initialize_output nf90_def_dim stage_dimid"  ) ! Dimension for stage variables 
                                                                                    ! (aka "before" vs. "after")
 
             ! Dimension coordinates
-            call netcdf_io_check( nf90_def_var(nc%id, nc%collision_id_varname,  NF90_INT,  &
+            call netcdf_io_check( nf90_def_var(nc%id, nc%collision_id_dimname,  NF90_INT,  &
                [nc%collision_id_dimid], nc%collision_id_varid), &
                 "collision_io_netcdf_initialize_output nf90_def_var collision_id_varid")
 
-            call netcdf_io_check( nf90_def_var(nc%id, nc%space_dimname,         NF90_CHAR, &
+            call netcdf_io_check( nf90_def_var(nc%id, nc%collision_body_dimname, NF90_INT, &
+               nc%collision_body_dimid, nc%collision_body_varid), &
+               "collision_io_netcdf_initialize_output nf90_def_var collision_body_varid")
+
+            call netcdf_io_check( nf90_def_var(nc%id, nc%space_dimname, NF90_CHAR, &
                nc%space_dimid, nc%space_varid), &
                "collision_io_netcdf_initialize_output nf90_def_var space_varid")
 
             call netcdf_io_check( nf90_def_var(nc%id, nc%stage_dimname, NF90_CHAR, &
                [nc%str_dimid,   nc%stage_dimid], nc%stage_varid), &
                "collision_io_netcdf_initialize_output nf90_def_var stage_varid")
-         
+
             ! Variables
-            call netcdf_io_check( nf90_def_var(nc%id, nc%name_dimname,          NF90_CHAR, &
-               [nc%str_dimid,   nc%name_dimid, nc%stage_dimid, nc%collision_id_dimid], nc%name_varid),  &
-               "collision_io_netcdf_initialize_output nf90_def_var name_varid")
+            call netcdf_io_check( nf90_def_var(nc%id, nc%name_dimname,    NF90_CHAR,   &
+               [nc%str_dimid, nc%collision_body_dimid, nc%stage_dimid, nc%collision_id_dimid], nc%name_varid), &
+               "collision_io_netcdf_initialize_output nf90_def_var id_varid")
 
             call netcdf_io_check( nf90_def_var(nc%id, nc%id_varname,    NF90_INT,   &
-               [nc%name_dimid,  nc%stage_dimid, nc%collision_id_dimid], nc%id_varid), &
+               [nc%collision_body_dimid,  nc%stage_dimid, nc%collision_id_dimid], nc%id_varid), &
                "collision_io_netcdf_initialize_output nf90_def_var id_varid")
 
             call netcdf_io_check( nf90_def_var(nc%id, nc%time_dimname,    nc%out_type, &
                nc%collision_id_dimid, nc%time_varid), &   
                "collision_io_netcdf_initialize_output nf90_def_var time_varid")
 
             call netcdf_io_check( nf90_def_var(nc%id, nc%regime_varname,  NF90_CHAR, &
@@ -212,51 +235,51 @@
                "collision_io_netcdf_initialize_output nf90_def_var regime_varid")
 
             call netcdf_io_check( nf90_def_var(nc%id, nc%Qloss_varname,  nc%out_type, &
                [nc%collision_id_dimid], nc%Qloss_varid),  &
                "collision_io_netcdf_initialize_output nf90_def_var Qloss_varid")
             
             call netcdf_io_check( nf90_def_var(nc%id, nc%ptype_varname,   NF90_CHAR, &
-               [nc%str_dimid, nc%name_dimid,nc%stage_dimid, nc%collision_id_dimid], nc%ptype_varid),  &
+               [nc%str_dimid, nc%collision_body_dimid, nc%stage_dimid, nc%collision_id_dimid], nc%ptype_varid),  &
                "collision_io_netcdf_initialize_output nf90_def_var ptype_varid")
 
             call netcdf_io_check( nf90_def_var(nc%id, nc%rh_varname,      nc%out_type, &
-               [nc%space_dimid, nc%name_dimid,  nc%stage_dimid, nc%collision_id_dimid], nc%rh_varid),  &
+               [nc%space_dimid, nc%collision_body_dimid,  nc%stage_dimid, nc%collision_id_dimid], nc%rh_varid),  &
                "collision_io_netcdf_initialize_output nf90_def_var rh_varid")
 
             call netcdf_io_check( nf90_def_var(nc%id, nc%vh_varname,      nc%out_type, &
-               [nc%space_dimid, nc%name_dimid,  nc%stage_dimid, nc%collision_id_dimid], nc%vh_varid), &
+               [nc%space_dimid, nc%collision_body_dimid,  nc%stage_dimid, nc%collision_id_dimid], nc%vh_varid), &
                "collision_io_netcdf_initialize_output nf90_def_var vh_varid")
 
             call netcdf_io_check( nf90_def_var(nc%id, nc%Gmass_varname,   nc%out_type, &
-               [nc%name_dimid, nc%stage_dimid,  nc%collision_id_dimid], nc%Gmass_varid), &
+               [nc%collision_body_dimid, nc%stage_dimid,  nc%collision_id_dimid], nc%Gmass_varid), &
                "collision_io_netcdf_initialize_output nf90_def_var Gmass_varid")
 
             call netcdf_io_check( nf90_def_var(nc%id, nc%radius_varname,  nc%out_type, &
-               [nc%name_dimid, nc%stage_dimid,  nc%collision_id_dimid], nc%radius_varid), &
+               [nc%collision_body_dimid, nc%stage_dimid,  nc%collision_id_dimid], nc%radius_varid), &
                "collision_io_netcdf_initialize_output nf90_def_var radius_varid")
 
             if (param%lrotation) then
                call netcdf_io_check( nf90_def_var(nc%id, nc%Ip_varname,      nc%out_type,&
-                  [nc%space_dimid,  nc%name_dimid,    nc%stage_dimid,  nc%collision_id_dimid], nc%Ip_varid), &
+                  [nc%space_dimid,  nc%collision_body_dimid,    nc%stage_dimid,  nc%collision_id_dimid], nc%Ip_varid), &
                   "collision_io_netcdf_initialize_output nf90_def_var Ip_varid")
 
                call netcdf_io_check( nf90_def_var(nc%id, nc%rot_varname,     nc%out_type,&
-                  [nc%space_dimid, nc%name_dimid, nc%stage_dimid, nc%collision_id_dimid], nc%rot_varid), &
+                  [nc%space_dimid, nc%collision_body_dimid, nc%stage_dimid, nc%collision_id_dimid], nc%rot_varid), &
                   "collision_io_netcdf_initialize_output nf90_def_var rot_varid")
             end if
 
             if (param%lenergy) then
-               call netcdf_io_check( nf90_def_var(nc%id, nc%ke_orb_varname,  nc%out_type, &
+               call netcdf_io_check( nf90_def_var(nc%id, nc%ke_orbit_varname,  nc%out_type, &
                   [nc%stage_dimid,  nc%collision_id_dimid], nc%KE_orb_varid), &
                   "collision_io_netcdf_initialize_output nf90_def_var KE_orb_varid")
 
-               call netcdf_io_check( nf90_def_var(nc%id, nc%ke_spin_varname, nc%out_type, &
-                  [nc%stage_dimid,  nc%collision_id_dimid], nc%KE_spin_varid), &
-                  "collision_io_netcdf_initialize_output nf90_def_var KE_spin_varid")
+               call netcdf_io_check( nf90_def_var(nc%id, nc%ke_rot_varname, nc%out_type, &
+                  [nc%stage_dimid,  nc%collision_id_dimid], nc%KE_rot_varid), &
+                  "collision_io_netcdf_initialize_output nf90_def_var KE_rot_varid")
 
                call netcdf_io_check( nf90_def_var(nc%id, nc%pe_varname, nc%out_type, &
                   [nc%stage_dimid,  nc%collision_id_dimid], nc%PE_varid), &
                   "collision_io_netcdf_initialize_output nf90_def_var PE_varid")
 
                call netcdf_io_check( nf90_def_var(nc%id, nc%be_varname, nc%out_type, &
                   [nc%stage_dimid,  nc%collision_id_dimid], nc%BE_varid), &
@@ -266,17 +289,17 @@
                   "collision_io_netcdf_initialize_output nf90_def_var TE_varid")
 
                if (param%lrotation) then
                   call netcdf_io_check( nf90_def_var(nc%id, nc%L_orbit_varname, nc%out_type, &
                      [nc%space_dimid, nc%stage_dimid, nc%collision_id_dimid], nc%L_orbit_varid), &
                      "collision_io_netcdf_initialize_output nf90_def_var L_orbit_varid")
 
-                  call netcdf_io_check( nf90_def_var(nc%id, nc%L_spin_varname,nc%out_type, &
-                     [nc%space_dimid, nc%stage_dimid, nc%collision_id_dimid], nc%L_spin_varid), &
-                     "collision_io_netcdf_initialize_output nf90_def_var L_spin_varid")
+                  call netcdf_io_check( nf90_def_var(nc%id, nc%L_rot_varname,nc%out_type, &
+                     [nc%space_dimid, nc%stage_dimid, nc%collision_id_dimid], nc%L_rot_varid), &
+                     "collision_io_netcdf_initialize_output nf90_def_var L_rot_varid")
                end if
             end if 
 
             call netcdf_io_check( nf90_inquire(nc%id, nVariables=nvar), &
                "collision_io_netcdf_initialize_output nf90_inquire nVariables")
             do varid = 1, nvar
                call netcdf_io_check( nf90_inquire_variable(nc%id, varid, xtype=vartype, ndims=ndims), &
@@ -350,40 +373,42 @@
             end if
 
             write(errmsg,*) "collision_io_netcdf_open nf90_open ",trim(adjustl(nc%file_name))
             call netcdf_io_check( nf90_open(nc%file_name, mode, nc%id), errmsg)
             self%lfile_is_open = .true.
 
             ! Dimensions
-            call netcdf_io_check( nf90_inq_dimid(nc%id, nc%collision_id_varname, nc%collision_id_dimid), &
+            call netcdf_io_check( nf90_inq_dimid(nc%id, nc%collision_id_dimname, nc%collision_id_dimid), &
                "collision_io_netcdf_open nf90_inq_dimid collision_id_dimid"  )
-            call netcdf_io_check( nf90_inquire_dimension(nc%id, nc%collision_id_dimid, nc%collision_id_varname, len=nc%max_idslot),&
+            call netcdf_io_check( nf90_inquire_dimension(nc%id, nc%collision_id_dimid, nc%collision_id_dimname, len=nc%max_idslot),&
                "collision_io_find_idslot nf90_inquire_dimension max_idslot"  )
             call netcdf_io_check( nf90_inq_dimid(nc%id, nc%space_dimname, nc%space_dimid), &
                "collision_io_netcdf_open nf90_inq_dimid space_dimid"  )
-            call netcdf_io_check( nf90_inq_dimid(nc%id, nc%name_dimname, nc%name_dimid), &
-               "collision_io_netcdf_open nf90_inq_dimid name_dimid"  )
+            call netcdf_io_check( nf90_inq_dimid(nc%id, nc%collision_body_dimname, nc%collision_body_dimid), &
+               "collision_io_netcdf_open nf90_inq_dimid collision_body_dimid"  )
             call netcdf_io_check( nf90_inq_dimid(nc%id, nc%str_dimname, nc%str_dimid), &
                "collision_io_netcdf_open nf90_inq_dimid str_dimid"  )
             call netcdf_io_check( nf90_inq_dimid(nc%id, nc%stage_dimname, nc%stage_dimid), &
                "collision_io_netcdf_open nf90_inq_dimid stage_dimid"  )
 
             ! Dimension coordinates
-            call netcdf_io_check( nf90_inq_varid(nc%id, nc%collision_id_varname, nc%collision_id_varid), &
+            call netcdf_io_check( nf90_inq_varid(nc%id, nc%collision_id_dimname, nc%collision_id_varid), &
                "collision_io_netcdf_open nf90_inq_varid collision_id_varid" )
+            call netcdf_io_check( nf90_inq_varid(nc%id, nc%collision_body_dimname, nc%collision_body_varid), &
+               "collision_io_netcdf_open nf90_inq_varid collision_body_varid" )
             call netcdf_io_check( nf90_inq_varid(nc%id, nc%space_dimname, nc%space_varid), &
                "collision_io_netcdf_open nf90_inq_varid space_varid" )
-            call netcdf_io_check( nf90_inq_varid(nc%id, nc%name_dimname, nc%name_varid), &
-               "collision_io_netcdf_open nf90_inq_varid name_varid" )
             call netcdf_io_check( nf90_inq_varid(nc%id, nc%stage_dimname, nc%stage_varid), &
                "collision_io_netcdf_open nf90_inq_varid stage_varid" )
 
             ! Required Variables
-            call netcdf_io_check( nf90_inq_varid(nc%id, nc%id_varname, nc%id_varid), &
+            call netcdf_io_check( nf90_inq_varid(nc%id, nc%name_dimname, nc%id_varid), &
                "collision_io_netcdf_open nf90_inq_varid name_varid" )
+            call netcdf_io_check( nf90_inq_varid(nc%id, nc%id_varname, nc%id_varid), &
+               "collision_io_netcdf_open nf90_inq_varid id_varid" )
             call netcdf_io_check( nf90_inq_varid(nc%id, nc%time_dimname, nc%time_varid), &
                "collision_io_netcdf_open nf90_inq_varid time_varid" )
             call netcdf_io_check( nf90_inq_varid(nc%id, nc%regime_varname, nc%regime_varid), &
                "collision_io_netcdf_open nf90_inq_varid regime_varid" )
             call netcdf_io_check( nf90_inq_varid(nc%id, nc%Qloss_varname, nc%Qloss_varid), &
                "collision_io_netcdf_open nf90_inq_varid Qloss_varid" )
             call netcdf_io_check( nf90_inq_varid(nc%id, nc%ptype_varname, nc%ptype_varid), &
@@ -401,29 +426,29 @@
                call netcdf_io_check( nf90_inq_varid(nc%id, nc%Ip_varname, nc%Ip_varid), &
                   "collision_io_netcdf_open nf90_inq_varid Ip_varid" )
                call netcdf_io_check( nf90_inq_varid(nc%id, nc%rot_varname, nc%rot_varid), &
                   "collision_io_netcdf_open nf90_inq_varid rot_varid" )
             end if
 
             if (param%lenergy) then
-               call netcdf_io_check( nf90_inq_varid(nc%id, nc%ke_orb_varname, nc%ke_orb_varid), &
+               call netcdf_io_check( nf90_inq_varid(nc%id, nc%ke_orbit_varname, nc%ke_orb_varid), &
                   "collision_io_netcdf_open nf90_inq_varid ke_orb_varid" )
                call netcdf_io_check( nf90_inq_varid(nc%id, nc%pe_varname, nc%pe_varid), &
                   "collision_io_netcdf_open nf90_inq_varid pe_varid" )
                call netcdf_io_check( nf90_inq_varid(nc%id, nc%be_varname, nc%be_varid), &
                   "collision_io_netcdf_open nf90_inq_varid be_varid" )
                call netcdf_io_check( nf90_inq_varid(nc%id, nc%te_varname, nc%te_varid), &
                   "collision_io_netcdf_open nf90_inq_varid te_varid" )
                call netcdf_io_check( nf90_inq_varid(nc%id, nc%L_orbit_varname, nc%L_orbit_varid), &
                   "collision_io_netcdf_open nf90_inq_varid L_orbit_varid" )
                if (param%lrotation) then
-                  call netcdf_io_check( nf90_inq_varid(nc%id, nc%ke_spin_varname, nc%ke_spin_varid), &
-                     "collision_io_netcdf_open nf90_inq_varid ke_spin_varid" )
-                  call netcdf_io_check( nf90_inq_varid(nc%id, nc%L_spin_varname, nc%L_spin_varid), &
-                     "collision_io_netcdf_open nf90_inq_varid L_spin_varid" )
+                  call netcdf_io_check( nf90_inq_varid(nc%id, nc%ke_rot_varname, nc%ke_rot_varid), &
+                     "collision_io_netcdf_open nf90_inq_varid ke_rot_varid" )
+                  call netcdf_io_check( nf90_inq_varid(nc%id, nc%L_rot_varname, nc%L_rot_varid), &
+                     "collision_io_netcdf_open nf90_inq_varid L_rot_varid" )
                end if
             end if
 
          end associate
       end select 
 
       return
@@ -437,16 +462,17 @@
       use netcdf
       implicit none
       ! Arguments
       class(collision_snapshot),   intent(in)    :: self    !! Swiftest encounter structure
       class(encounter_storage), intent(inout) :: history !! Collision history object
       class(base_parameters),      intent(inout) :: param   !! Current run configuration parameters
       ! Internals
-      integer(I4B)           :: i, idslot, old_mode, npl, stage, tmp, ntp
+      integer(I4B)           :: i, idslot, old_mode, stage, tmp
       character(len=NAMELEN) :: charstring
+      class(swiftest_cb), allocatable :: cb
       class(swiftest_pl), allocatable :: pl
       class(swiftest_tp), allocatable :: tp 
 
       select type(nc => history%nc)
       class is (collision_netcdf_parameters)
          associate(collider => self%collider, impactors => self%collider%impactors, fragments => self%collider%fragments, &
                    eslot => self%collider%collision_id)
@@ -467,35 +493,63 @@
                "collision_io_netcdf_write_frame_snapshot nf90_put_var Qloss_varid" )
 
             select type(before =>self%collider%before)
             class is (swiftest_nbody_system)
             select type(after =>self%collider%after)
             class is (swiftest_nbody_system)
                do stage = 1,2
+                  if (allocated(cb)) deallocate(cb)
                   if (allocated(pl)) deallocate(pl)
                   if (allocated(tp)) deallocate(tp)
                   select case(stage)
                   case(1)
+                     if (allocated(before%cb)) allocate(cb, source=before%cb)
                      if (allocated(before%pl)) allocate(pl, source=before%pl)
                      if (allocated(before%tp)) allocate(tp, source=before%tp)
                   case(2)
+                     if (allocated(after%cb)) allocate(cb, source=after%cb)
                      if (allocated(after%pl)) allocate(pl, source=after%pl)
                      if (allocated(after%tp)) allocate(tp, source=after%tp)
                   end select
 
-                  if (.not. (allocated(pl) .or. allocated(tp))) cycle
+                  if (.not. (allocated(pl) .or. allocated(tp) .or. allocated(cb))) cycle
+
+                  idslot = 0
+                  if (allocated(cb)) then
+                     idslot = idslot + 1
+                     call netcdf_io_check( nf90_put_var(nc%id, nc%collision_body_varid, idslot, start=[ idslot, stage, eslot]), &
+                           "collision_io_netcdf_write_frame_snapshot nf90_put_var collision_body_varid: cb")
+                     call netcdf_io_check( nf90_put_var(nc%id, nc%id_varid,     cb%id,     start=[   idslot, stage, eslot]), &
+                        "collision_io_netcdf_write_frame_snapshot nf90_put_var id_varid: cb"  )
+                     charstring = trim(adjustl(cb%info%name))
+                     call netcdf_io_check( nf90_put_var(nc%id, nc%name_varid,   charstring,   start=[1, idslot, stage, eslot], &
+                        count=[NAMELEN,1,1,1]), "collision_io_netcdf_write_frame_snapshot nf90_put_var name_varid: cb"  )
+                     charstring = trim(adjustl(cb%info%particle_type))
+                     call netcdf_io_check( nf90_put_var(nc%id, nc%ptype_varid,  charstring,   start=[1, idslot, stage, eslot], &
+                        count=[NAMELEN,1,1,1]), "collision_io_netcdf_write_frame_snapshot nf90_put_var particle_type_varid: cb" )
+                     call netcdf_io_check( nf90_put_var(nc%id, nc%Gmass_varid,  cb%Gmass,  start=[   idslot, stage, eslot]), &
+                        "collision_io_netcdf_write_frame_snapshot nf90_put_var Gmass_varid: cb")
+                     call netcdf_io_check( nf90_put_var(nc%id, nc%radius_varid, cb%radius, start=[   idslot, stage, eslot]), &
+                        "collision_io_netcdf_write_frame_snapshot nf90_put_var radius_varid: cb")
+                     if (param%lrotation) then
+                        call netcdf_io_check( nf90_put_var(nc%id, nc%Ip_varid,  cb%Ip(:),   start=[1, idslot, stage, eslot], &
+                           count=[NDIM,1,1,1]), "collision_io_netcdf_write_frame_snapshot nf90_put_var Ip_varid: cb")
+                        call netcdf_io_check( nf90_put_var(nc%id, nc%rot_varid,    cb%rot(:)*RAD2DEG,  &
+                           start=[1, idslot, stage, eslot], count=[NDIM,1,1,1]), &
+                           "collision_io_netcdf_write_frame_snapshot nf90_put_var rotx_varid: cb")
+                     end if                    
+                  end if
 
                   if (allocated(pl)) then
-                     npl = pl%nbody
-                     ! This ensures that there first idslot will have the first body in it, not id 0 which is the default for a new 
-                     ! idvals array
-                     if (.not.allocated(nc%idvals)) allocate(nc%idvals, source=pl%id)
-                     do i = 1, npl
-                        call nc%find_idslot(pl%id(i), idslot) 
-                        call netcdf_io_check( nf90_put_var(nc%id, nc%id_varid,     pl%id(i),     start=[   idslot, stage, eslot]), &
+                     call pl%sort("mass", ascending=.false.)
+                     do i = 1, pl%nbody
+                        idslot = idslot + 1
+                        call netcdf_io_check( nf90_put_var(nc%id, nc%collision_body_varid, idslot, start=[ idslot, stage, eslot]), &
+                           "collision_io_netcdf_write_frame_snapshot nf90_put_var collision_body_varid: pl")
+                        call netcdf_io_check( nf90_put_var(nc%id, nc%id_varid, pl%id(i), start=[idslot, stage, eslot]), &
                            "collision_io_netcdf_write_frame_snapshot nf90_put_var id_varid: pl")
                         charstring = trim(adjustl(pl%info(i)%name))
                         call netcdf_io_check( nf90_put_var(nc%id, nc%name_varid,   charstring,   start=[1, idslot, stage, eslot], &
                            count=[NAMELEN,1,1,1]), "collision_io_netcdf_write_frame_snapshot nf90_put_var name_varid: pl")
                         charstring = trim(adjustl(pl%info(i)%particle_type))
                         call netcdf_io_check( nf90_put_var(nc%id, nc%ptype_varid,  charstring,   start=[1, idslot, stage, eslot], &
                            count=[NAMELEN,1,1,1]), "collision_io_netcdf_write_frame_snapshot nf90_put_var particle_type_varid: pl")
@@ -514,53 +568,53 @@
                               start=[1, idslot, stage, eslot], count=[NDIM,1,1,1]), &
                               "collision_io_netcdf_write_frame_snapshot nf90_put_var rotx_varid: pl")
                         end if
                      end do
                   end if
 
                   if (allocated(tp)) then
-                     ntp = tp%nbody
-                     ! This ensures that there first idslot will have the first body in it, not id 0 which is the default for a new 
-                     ! idvals array
-                     if (.not.allocated(nc%idvals)) allocate(nc%idvals, source=tp%id)
-                     do i = 1, ntp
-                        call nc%find_idslot(tp%id(i), idslot)
-                        call netcdf_io_check( nf90_put_var(nc%id, nc%id_varid,     tp%id(i),     start=[   idslot, stage, eslot]), &
+                     call tp%sort("id", ascending=.true.)
+                     do i = 1, tp%nbody
+                        idslot = idslot + 1
+                        call netcdf_io_check( nf90_put_var(nc%id, nc%collision_body_varid, idslot, start=[ idslot, stage, eslot]), &
+                           "collision_io_netcdf_write_frame_snapshot nf90_put_var collision_body_varid: tp")
+                        call netcdf_io_check( nf90_put_var(nc%id, nc%id_varid,     tp%id(i),     start=[idslot, stage, eslot]), &
                            "collision_io_netcdf_write_frame_snapshot nf90_put_var id_varid: tp"  )
                         charstring = trim(adjustl(tp%info(i)%name))
                         call netcdf_io_check( nf90_put_var(nc%id, nc%name_varid,   charstring,   start=[1, idslot, stage, eslot], &
                            count=[NAMELEN,1,1,1]), "collision_io_netcdf_write_frame_snapshot nf90_put_var name_varid: tp"  )
                         charstring = trim(adjustl(tp%info(i)%particle_type))
                         call netcdf_io_check( nf90_put_var(nc%id, nc%ptype_varid,  charstring,   start=[1, idslot, stage, eslot], &
                            count=[NAMELEN,1,1,1]), "collision_io_netcdf_write_frame_snapshot nf90_put_var particle_type_varid: tp" )
                         call netcdf_io_check( nf90_put_var(nc%id, nc%rh_varid,     tp%rh(:,i),   start=[1, idslot, stage, eslot], &
                            count=[NDIM,1,1,1]), "collision_io_netcdf_write_frame_snapshot nf90_put_var rh_varid: tp"  )
                         call netcdf_io_check( nf90_put_var(nc%id, nc%vh_varid,     tp%vh(:,i),   start=[1, idslot, stage, eslot], &
                            count=[NDIM,1,1,1]), "collision_io_netcdf_write_frame_snapshot nf90_put_var vh_varid: tp"  )
                      end do
                   end if
+
                end do
             end select
             end select
 
             if (param%lenergy) then
                call netcdf_io_check( nf90_put_var(nc%id, nc%ke_orb_varid,  collider%ke_orbit(:), start=[   1, eslot], &
                   count=[      2, 1]), "collision_io_netcdf_write_frame_snapshot nf90_put_var ke_orb_varid before" )
-               call netcdf_io_check( nf90_put_var(nc%id, nc%ke_spin_varid, collider%ke_spin(:),  start=[   1, eslot], &
-                  count=[      2, 1]), "collision_io_netcdf_write_frame_snapshot nf90_put_var ke_spin_varid before" )
+               call netcdf_io_check( nf90_put_var(nc%id, nc%ke_rot_varid, collider%ke_rot(:),  start=[   1, eslot], &
+                  count=[      2, 1]), "collision_io_netcdf_write_frame_snapshot nf90_put_var ke_rot_varid before" )
                call netcdf_io_check( nf90_put_var(nc%id, nc%pe_varid,      collider%pe(:),       start=[   1, eslot], &
                   count=[      2, 1]), "collision_io_netcdf_write_frame_snapshot nf90_put_var pe_varid before" )
                call netcdf_io_check( nf90_put_var(nc%id, nc%be_varid,      collider%be(:),       start=[   1, eslot], &
                   count=[      2, 1]), "collision_io_netcdf_write_frame_snapshot nf90_put_var pe_varid before" )
                call netcdf_io_check( nf90_put_var(nc%id, nc%te_varid,      collider%te(:),       start=[   1, eslot], &
                   count=[      2, 1]), "collision_io_netcdf_write_frame_snapshot nf90_put_var pe_varid tefore" )
                call netcdf_io_check( nf90_put_var(nc%id, nc%L_orbit_varid,   collider%L_orbit(:,:), start=[1, 1, eslot], &
                   count=[NDIM, 2, 1]), "collision_io_netcdf_write_frame_snapshot nf90_put_var L_orbit_varid before" )
-               call netcdf_io_check( nf90_put_var(nc%id, nc%L_spin_varid,   collider%L_spin(:,:),  start=[1, 1, eslot], &
-                  count=[NDIM, 2, 1]), "collision_io_netcdf_write_frame_snapshot nf90_put_var L_spin_varid before" )
+               call netcdf_io_check( nf90_put_var(nc%id, nc%L_rot_varid,   collider%L_rot(:,:),  start=[1, 1, eslot], &
+                  count=[NDIM, 2, 1]), "collision_io_netcdf_write_frame_snapshot nf90_put_var L_rot_varid before" )
             end if
       
             call netcdf_io_check( nf90_set_fill(nc%id, old_mode, tmp) )
          end associate
       end select
       return
    end subroutine collision_io_netcdf_write_frame_snapshot
```

### Comparing `swiftest-2024.4.1/src/collision/collision_module.f90` & `swiftest-2024.4.2/src/collision/collision_module.f90`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 ! Swiftest is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License 
 ! as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 ! Swiftest is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty 
 ! of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 ! You should have received a copy of the GNU General Public License along with Swiftest. 
 ! If not, see: https://www.gnu.org/licenses. 
 
-
 module collision
    !! author: The Purdue Swiftest Team - David A. Minton, Carlisle A. Wishard, Jennifer L.L. Pouplin, and Jacob R. Elliott
    !!
    !! Definition of classes and methods used to determine close encounters
    use globals
    use base
    use encounter
@@ -21,223 +20,227 @@
    character(len=*), parameter :: COLLISION_OUTFILE = 'collisions.nc'  !! Name of NetCDF output file for collision information
 #ifdef COARRAY
    character(len=STRMAX) :: COLLISION_LOG_OUT !! Name of log file for collision diagnostic information (each co-image gets its own)
 #else
    character(len=*), parameter :: COLLISION_LOG_OUT = "collisions.log" !! Name of log file for collision diagnostic information
 #endif
 
-   !>Symbolic names for collisional outcomes from collresolve_resolve:
+   !>Symbolic names for collisional outcomes 
    integer(I4B), parameter :: COLLRESOLVE_REGIME_MERGE              =  1
    integer(I4B), parameter :: COLLRESOLVE_REGIME_DISRUPTION         =  2
    integer(I4B), parameter :: COLLRESOLVE_REGIME_SUPERCATASTROPHIC  =  3
    integer(I4B), parameter :: COLLRESOLVE_REGIME_GRAZE_AND_MERGE    =  4
    integer(I4B), parameter :: COLLRESOLVE_REGIME_HIT_AND_RUN        =  5
+   integer(I4B), parameter :: REGIME_CB_IMPACT                      = 6
+   integer(I4B), parameter :: REGIME_EJECTED                        = 7
    character(len=NAMELEN),parameter :: REGIME_NAME_MERGE = "Merge"
    character(len=NAMELEN),parameter :: REGIME_NAME_DISRUPTION = "Disruption"
    character(len=NAMELEN),parameter :: REGIME_NAME_SUPERCATASTROPHIC = "Supercatastrophic"
    character(len=NAMELEN),parameter :: REGIME_NAME_GRAZE_AND_MERGE = "Graze and Merge"
    character(len=NAMELEN),parameter :: REGIME_NAME_HIT_AND_RUN = "Hit and Run"
-   character(len=NAMELEN),dimension(5), parameter :: REGIME_NAMES = [REGIME_NAME_MERGE, REGIME_NAME_DISRUPTION, &
+   character(len=NAMELEN),parameter :: REGIME_NAME_CB_IMPACT = "Central Body Impact"
+   character(len=NAMELEN),parameter :: REGIME_NAME_EJECTED = "Ejected"
+   character(len=NAMELEN),dimension(7), parameter :: REGIME_NAMES = [REGIME_NAME_MERGE, REGIME_NAME_DISRUPTION, &
                                                      REGIME_NAME_SUPERCATASTROPHIC, REGIME_NAME_GRAZE_AND_MERGE, &
-                                                     REGIME_NAME_HIT_AND_RUN]
-   real(DP), parameter :: MAX_ROT_SI = 7.108e-4 !! Spin limit in rad/s of cohesionless body from Holsapple (2007)
+                                                     REGIME_NAME_HIT_AND_RUN, REGIME_NAME_CB_IMPACT, REGIME_NAME_EJECTED]
+   real(DP), parameter :: MAX_ROT_SI = 7.108e-4 !! Rotational limit in rad/s of cohesionless body from Holsapple (2007)
 
    !> Swiftest class for tracking pl-pl close encounters in a step when collisions are possible
    type, extends(encounter_list) :: collision_list_plpl
    contains
-         !! Processes the pl-pl encounter list remove only those encounters that led to a collision
       procedure :: extract_collisions => collision_resolve_extract_plpl      
-         !! Checks if a test particle is going to collide with a massive body
+         !! Processes the pl-pl encounter list remove only those encounters that led to a collision
       procedure :: collision_check    => collision_check_plpl 
-         !! Process the pl-pl collision list, then modifiy the massive bodies based on the outcome of the collision
+         !! Checks if a test particle is going to collide with a massive body
       procedure :: resolve_collision  => collision_resolve_plpl 
+         !! Process the pl-pl collision list, then modifiy the massive bodies based on the outcome of the collision
       final     ::                       collision_final_plpl
    end type collision_list_plpl
 
 
    !> Class for tracking pl-tp close encounters in a step when collisions are possible
    type, extends(encounter_list) :: collision_list_pltp
    contains
-         !! Processes the pl-tp encounter list remove only those encounters that led to a collision
       procedure :: extract_collisions => collision_resolve_extract_pltp 
-         !! Checks if a test particle is going to collide with a massive body
+         !! Processes the pl-tp encounter list remove only those encounters that led to a collision
       procedure :: collision_check    => collision_check_pltp 
-      procedure :: resolve_collision  => collision_resolve_pltp         !! Process the pl-tp collision list
+         !! Checks if a test particle is going to collide with a massive body
       final     ::                       collision_final_pltp
+      procedure :: resolve_collision  => collision_resolve_pltp         !! Process the pl-tp collision list
    end type collision_list_pltp
 
 
    !> Class definition for the variables that describe the bodies involved in the collision
    type, extends(base_object) :: collision_impactors
-         !! Number of bodies involved in the collision
       integer(I4B)                                 :: ncoll  
-         !! Index of bodies involved in the collision
+         !! Number of bodies involved in the collision
       integer(I4B), dimension(:),      allocatable :: id 
-         !! Two-body equivalent position vectors of the collider bodies prior to collision in system barycentric coordinates
+         !! Index of bodies involved in the collision
       real(DP),     dimension(NDIM,2)              :: rb  
-         !! Two-body equivalent velocity vectors of the collider bodies prior to collision in system barycentric coordinate
+         !! Two-body equivalent position vectors of the collider bodies prior to collision in system barycentric coordinates
       real(DP),     dimension(NDIM,2)              :: vb 
-         !! Two-body equivalent position vectors of the collider bodies prior to collision in collision center of mass coordinates
+         !! Two-body equivalent velocity vectors of the collider bodies prior to collision in system barycentric coordinate
       real(DP),     dimension(NDIM,2)              :: rc 
-         !! Two-body equivalent velocity vectors of the collider bodies prior to collision in collision center of mass coordinates
+         !! Two-body equivalent position vectors of the collider bodies prior to collision in collision center of mass coordinates
       real(DP),     dimension(NDIM,2)              :: vc 
-         !! Two-body equivalent principal axes moments of inertia the collider bodies prior to collision
+         !! Two-body equivalent velocity vectors of the collider bodies prior to collision in collision center of mass coordinates
       real(DP),     dimension(NDIM,2)              :: rot 
-         !! Two-body equivalent spin angular momentum vectors of the collider bodies prior to collision
-      real(DP),     dimension(NDIM,2)              :: L_spin    
-         !! Two-body equivalent orbital angular momentum vectors of the collider bodies prior to collision
+         !! Two-body equivalent principal axes moments of inertia the collider bodies prior to collision
+      real(DP),     dimension(NDIM,2)              :: L_rot    
+         !! Two-body equivalent rotational angular momentum vectors of the collider bodies prior to collision
       real(DP),     dimension(NDIM,2)              :: L_orbit   
-         !! Orbital kinetic energy of each individual impactor
+         !! Two-body equivalent orbital angular momentum vectors of the collider bodies prior to collision
       real(DP),     dimension(2)                   :: ke_orbit  
-         !! Spin kinetic energy of each individual impactor
-      real(DP),     dimension(2)                   :: ke_spin   
-         !! Binding energy of each individual impactor
+         !! Orbital kinetic energy of each individual impactor
+      real(DP),     dimension(2)                   :: ke_rot   
+         !! Rotational kinetic energy of each individual impactor
       real(DP),     dimension(2)                   :: be  
-         !! Two-body equivalent principal axes moments of inertia the collider bodies prior to collision
+         !! Binding energy of each individual impactor
       real(DP),     dimension(NDIM,2)              :: Ip 
-         !! Two-body equivalent G*mass of the collider bodies prior to the collision
+         !! Two-body equivalent principal axes moments of inertia the collider bodies prior to collision
       real(DP),     dimension(2)                   :: Gmass 
-         !! Two-body equivalent mass of the collider bodies prior to the collision
+         !! Two-body equivalent G*mass of the collider bodies prior to the collision
       real(DP),     dimension(2)                   :: mass      
-         !! Two-body equivalent radii of the collider bodies prior to the collision
+         !! Two-body equivalent mass of the collider bodies prior to the collision
       real(DP),     dimension(2)                   :: radius    
-         !! Energy lost during the collision
+         !! Two-body equivalent radii of the collider bodies prior to the collision
       real(DP)                                     :: Qloss     
-         !! Collresolve regime code for this collision
+         !! Energy lost during the collision
       integer(I4B)                                 :: regime    
-         !! Distribution of fragment mass determined by the regime calculation (largest fragment, second largest, and remainder)    
+         !! Collresolve regime code for this collision
       real(DP),     dimension(:),      allocatable :: mass_dist 
-         !! Mass of central body (used to compute potential energy in regime determination)
+         !! Distribution of fragment mass determined by the regime calculation (largest fragment, second largest, and remainder)    
       real(DP)                                     :: Mcb       
+         !! Mass of central body (used to compute potential energy in regime determination)
 
       ! Values in a coordinate frame center
-              !! x-direction unit vector of collisional system ed on the collider barycenter and collisional system unit vectors 
       real(DP), dimension(NDIM) :: x_unit 
-         !! y-direction unit vector of collisional system
+         !! x-direction unit vector of collisional system ed on the collider barycenter and collisional system unit vectors 
       real(DP), dimension(NDIM) :: y_unit 
-         !! z-direction unit vector of collisional system
+         !! y-direction unit vector of collisional system
       real(DP), dimension(NDIM) :: z_unit 
-         !! velocity direction unit vector of collisional system
+         !! z-direction unit vector of collisional system
       real(DP), dimension(NDIM) :: v_unit 
-         !! Center of mass position vector of the collider nbody_system in nbody_system barycentric coordinates
+         !! velocity direction unit vector of collisional system
       real(DP), dimension(NDIM) :: rbcom  
-         !! Velocity vector of the center of mass of the collider nbody_system in nbody_system barycentric coordinates
+         !! Center of mass position vector of the collider nbody_system in nbody_system barycentric coordinates
       real(DP), dimension(NDIM) :: vbcom  
-         !! Impact point position vector of the collider nbody_system in nbody_system barycentric coordinates
+         !! Velocity vector of the center of mass of the collider nbody_system in nbody_system barycentric coordinates
       real(DP), dimension(NDIM) :: rcimp  
-         !! The impact point velocity vector is the component of the velocity in the distance vector direction
+         !! Impact point position vector of the collider nbody_system in nbody_system barycentric coordinates
       real(DP), dimension(NDIM) :: bounce_unit  
+         !! The impact point velocity vector is the component of the velocity in the distance vector direction
 
    contains
-         !! Consolidates a multi-body collision into an equivalent 2-body collision
       procedure :: consolidate           => collision_resolve_consolidate_impactors 
-         !! Resets the collider object variables to 0 and deallocates the index and mass distributions
+         !! Consolidates a multi-body collision into an equivalent 2-body collision
       procedure :: dealloc               => collision_util_dealloc_impactors        
-         !! Sets the coordinate system of the impactors
+         !! Resets the collider object variables to 0 and deallocates the index and mass distributions
       procedure :: set_coordinate_system => collision_util_set_coordinate_impactors 
-         !! Finalizer will deallocate all allocatables
+         !! Sets the coordinate system of the impactors
       final     ::                          collision_final_impactors               
+         !! Finalizer will deallocate all allocatables
    end type collision_impactors
 
 
    !> Class definition for the variables that describe a collection of fragments in barycentric coordinates
    type, extends(base_object) :: collision_fragments
-         !! Number of bodies
       integer(I4B)                                           :: nbody = 0    
-         !! Total mass of fragments       
+         !! Number of bodies
       real(DP)                                               :: mtot         
-         !! Identifier
+         !! Total mass of fragments       
       integer(I4B),              dimension(:),   allocatable :: id           
-         !! Particle metadata information
+         !! Identifier
       class(base_particle_info), dimension(:),   allocatable :: info         
-         !! An integrator-specific status indicator 
+         !! Particle metadata information
       integer(I4B),              dimension(:),   allocatable :: status       
-         !! Heliocentric position
+         !! An integrator-specific status indicator 
       real(DP),                  dimension(:,:), allocatable :: rh           
-         !! Heliocentric velocity
+         !! Heliocentric position
       real(DP),                  dimension(:,:), allocatable :: vh           
-         !! Barycentric position
+         !! Heliocentric velocity
       real(DP),                  dimension(:,:), allocatable :: rb           
-         !! Barycentric velocity
+         !! Barycentric position
       real(DP),                  dimension(:,:), allocatable :: vb           
-         !! Position vectors in the collision coordinate frame
+         !! Barycentric velocity
       real(DP),                  dimension(:,:), allocatable :: rc           
-         !! Velocity vectors in the collision coordinate frame
+         !! Position vectors in the collision coordinate frame
       real(DP),                  dimension(:,:), allocatable :: vc           
-         !! Array of radial direction unit vectors of individual fragments in the collisional coordinate frame
+         !! Velocity vectors in the collision coordinate frame
       real(DP),                  dimension(:,:), allocatable :: r_unit       
-         !! Array of velocity direction unit vectors of individual fragments in the collisional coordinate frame
+         !! Array of radial direction unit vectors of individual fragments in the collisional coordinate frame
       real(DP),                  dimension(:,:), allocatable :: v_unit       
-         !! Array of tangential direction unit vectors of individual fragments in the collisional coordinate frame
+         !! Array of velocity direction unit vectors of individual fragments in the collisional coordinate frame
       real(DP),                  dimension(:,:), allocatable :: t_unit       
-         !! Array of normal direction unit vectors of individual fragments in the collisional coordinate frame
+         !! Array of tangential direction unit vectors of individual fragments in the collisional coordinate frame
       real(DP),                  dimension(:,:), allocatable :: n_unit       
-         !! rotation vectors of fragments
+         !! Array of normal direction unit vectors of individual fragments in the collisional coordinate frame
       real(DP),                  dimension(:,:), allocatable :: rot          
-         !! Principal axes moment of inertia for fragments
+         !! rotation vectors of fragments
       real(DP),                  dimension(:,:), allocatable :: Ip           
-         !! G*mass of fragments
+         !! Principal axes moment of inertia for fragments
       real(DP),                  dimension(:),   allocatable :: Gmass        
-         !! masses of fragments
+         !! G*mass of fragments
       real(DP),                  dimension(:),   allocatable :: mass         
-         !! Radii  of fragments
+         !! masses of fragments
       real(DP),                  dimension(:),   allocatable :: radius       
          !! Radii  of fragments
       real(DP),                  dimension(:),   allocatable :: density      
-         !! Array of radial distance magnitudes of individual fragments in the collisional coordinate frame 
+         !! Radii  of fragments
       real(DP),                  dimension(:),   allocatable :: rmag         
          !! Array of radial distance magnitudes of individual fragments in the collisional coordinate frame 
       real(DP),                  dimension(:),   allocatable :: vmag         
-         !! Array of rotation magnitudes of individual fragments 
+         !! Array of radial distance magnitudes of individual fragments in the collisional coordinate frame 
       real(DP),                  dimension(:),   allocatable :: rotmag       
-         !! Array of indices indicating which impactor body (1 or 2) the fragment originates from
+         !! Array of rotation magnitudes of individual fragments 
       integer(I4B),              dimension(:),   allocatable :: origin_body  
-         !! Orbital angular momentum vector of all fragments
+         !! Array of indices indicating which impactor body (1 or 2) the fragment originates from
       real(DP),                  dimension(NDIM)             :: L_orbit_tot  
-         !! Spin angular momentum vector of all fragments
-      real(DP),                  dimension(NDIM)             :: L_spin_tot   
-         !! Orbital angular momentum vector of each individual fragment
+         !! Orbital angular momentum vector of all fragments
+      real(DP),                  dimension(NDIM)             :: L_rot_tot   
+         !! Rotational angular momentum vector of all fragments
       real(DP),                  dimension(:,:), allocatable :: L_orbit      
-         !! Spin angular momentum vector of each individual fragment
-      real(DP),                  dimension(:,:), allocatable :: L_spin       
-         !! Orbital kinetic energy of all fragments
+         !! Orbital angular momentum vector of each individual fragment
+      real(DP),                  dimension(:,:), allocatable :: L_rot       
+         !! Rotational angular momentum vector of each individual fragment
       real(DP)                                               :: ke_orbit_tot 
-         !! Spin kinetic energy of all fragments
-      real(DP)                                               :: ke_spin_tot  
-         !! Potential energy of all fragments
+         !! Orbital kinetic energy of all fragments
+      real(DP)                                               :: ke_rot_tot  
+         !! Rotational kinetic energy of all fragments
       real(DP)                                               :: pe           
-         !! Binding energy of all fragments
+         !! Potential energy of all fragments
       real(DP)                                               :: be           
-         !! Orbital kinetic energy of each individual fragment
+         !! Binding energy of all fragments
       real(DP),                  dimension(:), allocatable   :: ke_orbit     
-         !! Spin kinetic energy of each individual fragment
-      real(DP),                  dimension(:), allocatable   :: ke_spin      
+         !! Orbital kinetic energy of each individual fragment
+      real(DP),                  dimension(:), allocatable   :: ke_rot      
+         !! Rotational kinetic energy of each individual fragment
    contains
-         !! Deallocates all allocatable arrays and sets everything else to 0
       procedure :: dealloc               => collision_util_dealloc_fragments        
-         !! Allocates all allocatables
+         !! Deallocates all allocatable arrays and sets everything else to 0
       procedure :: setup                 => collision_util_setup_fragments          
-         !! Resets all position and velocity-dependent fragment quantities in order to do a fresh calculation (does not reset mass, 
+         !! Allocates all allocatables
          !! radius, or other values that get set prior to the call to fraggle_generate)
+         !! Resets all position and velocity-dependent fragment quantities in order to do a fresh calculation (does not reset mass, 
       procedure :: reset                 => collision_util_reset_fragments          
-         !! Sets the coordinate system of the fragments
       procedure :: set_coordinate_system => collision_util_set_coordinate_fragments 
-         !! Finalizer deallocates all allocatables
+         !! Sets the coordinate system of the fragments
       final     ::                          collision_final_fragments               
+         !! Finalizer deallocates all allocatables
    end type collision_fragments
 
 
    type :: collision_basic
       !! This class defines a collisional system that stores impactors and fragments. This is written so that various collision 
       !! models (i.e. Fraggle) could potentially be used to resolve collision by defining extended types of encounters_impactors 
       !! and/or encounetr_fragments
       !!
       !! The generate method for this class is the merge model. This a
-         !! Object containing information on the pre-collision system llows any extended type to have access to the merge procedure
-         !! by selecting the collision_basic parent class
+      !! Object containing information on the pre-collision system llows any extended type to have access to the merge procedure
+      !! by selecting the collision_basic parent class
       class(collision_fragments), allocatable :: fragments           
          !! Object containing information on the post-collision system
       class(collision_impactors), allocatable :: impactors           
          !! A snapshot of the subset of the nbody_system involved in the collision
       class(base_nbody_system),   allocatable :: before              
          !! A snapshot of the subset of the nbody_system containing products of the collision
       class(base_nbody_system),   allocatable :: after               
@@ -267,338 +270,344 @@
          !! Angular momentum scale factor (a convenience unit that is derived from dscale, tscale, and mscale)
       real(DP) :: Lscale = 1.0_DP 
 
       ! For the following variables, index 1 re
          !! Before/after orbital angular momentum  fers to the *entire* n-body system in its pre-collisional state and index 2 
          !! refers to the system in its post-collisional state
       real(DP), dimension(NDIM,2) :: L_orbit  
-         !! Before/after spin angular momentum 
-      real(DP), dimension(NDIM,2) :: L_spin   
+         !! Before/after rotational angular momentum 
+      real(DP), dimension(NDIM,2) :: L_rot   
          !! Before/after total nbody_system angular momentum 
       real(DP), dimension(NDIM,2) :: L_total  
          !! Before/after orbital kinetic energy
       real(DP), dimension(2)      :: ke_orbit 
-         !! Before/after spin kinetic energy
-      real(DP), dimension(2)      :: ke_spin  
+         !! Before/after rotational kinetic energy
+      real(DP), dimension(2)      :: ke_rot  
          !! Before/after potential energy
       real(DP), dimension(2)      :: pe       
          !! Before/after binding energy
       real(DP), dimension(2)      :: be       
          !! Before/after total system energy
       real(DP), dimension(2)      :: te       
 
    contains
-         !! Merges the impactors to make a single final body
       procedure :: generate                   => collision_generate_basic                  
          !! Merges the impactors to make a single final body
       procedure :: hitandrun                  => collision_generate_hitandrun              
          !! Merges the impactors to make a single final body
       procedure :: merge                      => collision_generate_merge                  
-         !! Add fragments to nbody_system
+         !! Merges the impactors to make a single final body
       procedure :: add_fragments              => collision_util_add_fragments_to_collider  
+         !! Add fragments to nbody_system
+      procedure :: get_energy_and_momentum    => collision_util_get_energy_and_momentum    
          !! Calculates total nbody_system energy in either the pre-collision outcome state (lbefore = .true.) or the post-collision
          !! outcome state (lbefore = .false.)
-      procedure :: get_energy_and_momentum    => collision_util_get_energy_and_momentum    
-         !! Deallocates all allocatables
       procedure :: dealloc                    => collision_util_dealloc_basic            
-         !! Determine which fragmentation regime the set of impactors will be
+         !! Deallocates all allocatables
       procedure :: get_regime                 => collision_regime_collider              
-         !! Initializer for the encounter collision system and the before/after snapshots
+         !! Determine which fragmentation regime the set of impactors will be
       procedure :: setup                      => collision_util_setup_collider             
-         !! Initializer for the impactors for the encounter collision system. Deallocates old impactors before creating new ones
+         !! Initializer for the encounter collision system and the before/after snapshots
       procedure :: setup_impactors            => collision_util_setup_impactors_collider   
-         !! Initializer for the fragments of the collision system. 
+         !! Initializer for the impactors for the encounter collision system. Deallocates old impactors before creating new ones
       procedure :: setup_fragments            => collision_util_setup_fragments_collider   
-         !! Sets the coordinate system of the collisional system
+         !! Initializer for the fragments of the collision system. 
       procedure :: set_coordinate_system      => collision_util_set_coordinate_collider    
-         !! Scales dimenional quantities to ~O(1) with respect to the collisional system.  
+         !! Sets the coordinate system of the collisional system
       procedure :: set_natural_scale          => collision_util_set_natural_scale_factors  
-         !! Restores dimenional quantities back to the original system units
+         !! Scales dimenional quantities to ~O(1) with respect to the collisional system.  
       procedure :: set_original_scale         => collision_util_set_original_scale_factors 
+         !! Restores dimenional quantities back to the original system units
       final     ::                               collision_final_basic
    end type collision_basic
 
    
    type, extends(collision_basic) :: collision_bounce
    contains 
          !! If a collision would result in a disruption, "bounce" the bodies instead.
       procedure :: generate => collision_generate_bounce 
    end type collision_bounce
 
 
    !! NetCDF dimension and variable names for the enounter save object
    type, extends(encounter_netcdf_parameters) :: collision_netcdf_parameters
-              !! ID for the stage dimension 
       integer(I4B)       :: stage_dimid  
-         !! ID for the stage variable  
+         !! ID for the stage dimension 
       integer(I4B)       :: stage_varid  
-         !! name of the stage dimension (before/after)
+         !! ID for the stage variable  
       character(NAMELEN) :: stage_dimname = "stage"             
-         !! The stage coordinate labels
+         !! name of the stage dimension (before/after)
       character(len=6), dimension(2) :: stage_coords = ["before", "after "] 
-
-         !! ID for the collision event dimension       
+         !! The stage coordinate labels
       integer(I4B)       :: collision_id_dimid                 
-
-         !! name of the energy loss variable
+         !! ID for the collision event dimension 
+      character(NAMELEN) :: collision_body_dimname = "collision_body"
+         !! name of the collision body dimension 
+      integer(I4B) :: collision_body_dimid
+         !! Netcdf ID for the collision body dimension
+      integer(I4B) :: collision_body_varid
+         !! Netcdf ID for the collision body variable
       character(NAMELEN) :: Qloss_varname  = "Qloss"   
-         !! ID for the energy loss variable 
+         !! name of the energy loss variable
       integer(I4B)       :: Qloss_varid                
-         !! name of the collision regime variable
+         !! ID for the energy loss variable 
       character(NAMELEN) :: regime_varname = "regime"  
-         !! ID for the collision regime variable
+         !! name of the collision regime variable
       integer(I4B)       :: regime_varid               
+         !! ID for the collision regime variable
    contains
          !! Initialize a set of parameters used to identify a NetCDF output object
       procedure :: initialize => collision_io_netcdf_initialize_output 
          !! Opens an old file
       procedure :: open       => collision_io_netcdf_open              
    end type collision_netcdf_parameters
 
 
    type, extends(encounter_snapshot)  :: collision_snapshot
-         !! Indicates that this snapshot contains at least one collision 
+      !! Indicates that this snapshot contains at least one collision 
       logical                             :: lcollision 
-         !! Collider object at this snapshot
       class(collision_basic), allocatable :: collider  
+         !! Collider object at this snapshot
    contains
-         !! Writes a frame of encounter data to file 
       procedure :: write_frame => collision_io_netcdf_write_frame_snapshot 
-         !! Deallocates all allocatables
+         !! Writes a frame of encounter data to file 
       procedure :: dealloc     => collision_util_dealloc_snapshot          
-         !! Gets an array of all id values saved in this snapshot
+         !! Deallocates all allocatables
       procedure :: get_idvals  => collision_util_get_idvalues_snapshot     
+         !! Gets an array of all id values saved in this snapshot
    end type collision_snapshot
 
 
    !> A class that that is used to store simulation history data between file output
    type, extends(encounter_storage) :: collision_storage
    contains
          !! Dumps contents of encounter history to file
       procedure :: dump           => collision_io_netcdf_dump 
          !! Take a minimal snapshot of the nbody_system through an encounter
-      procedure :: take_snapshot  => collision_util_snapshot  
+      procedure :: take_snapshot  => collision_util_take_snapshot  
+         !! Maps body id values to storage index values so we don't have to use unlimited dimensions for id
+      procedure :: save_energy_snapshot  => collision_util_save_energy_snapshot  
          !! Maps body id values to storage index values so we don't have to use unlimited dimensions for id
       procedure :: make_index_map => collision_util_index_map 
    end type collision_storage
 
 
    interface
       module subroutine collision_generate_basic(self, nbody_system, param, t)
          implicit none
-            !! Merge fragment nbody_system object 
          class(collision_basic),   intent(inout) :: self          
-            !! Swiftest nbody system object
+            !! Merge fragment nbody_system object 
          class(base_nbody_system), intent(inout) :: nbody_system 
-            !! Current run configuration parameters 
+            !! Swiftest nbody system object
          class(base_parameters),   intent(inout) :: param        
-            !! The time of the collision
+            !! Current run configuration parameters 
          real(DP),                 intent(in)    :: t            
+            !! The time of the collision
       end subroutine collision_generate_basic 
 
       module subroutine collision_generate_bounce(self, nbody_system, param, t)
          implicit none
-            !! Bounce fragment nbody_system object 
          class(collision_bounce),  intent(inout) :: self         
-            !! Swiftest nbody system object
+            !! Bounce fragment nbody_system object 
          class(base_nbody_system), intent(inout) :: nbody_system 
-            !! Current run configuration parameters 
+            !! Swiftest nbody system object
          class(base_parameters),   intent(inout) :: param        
-            !! The time of the collision
+            !! Current run configuration parameters 
          real(DP),                 intent(in)    :: t            
+            !! The time of the collision
       end subroutine collision_generate_bounce 
 
       module subroutine collision_generate_hitandrun(self, nbody_system, param, t) 
          implicit none
          class(collision_basic),   intent(inout) :: self
-            !! Swiftest nbody system object
          class(base_nbody_system), intent(inout) :: nbody_system 
-            !! Current run configuration parameters with SyMBA additions
+            !! Swiftest nbody system object
          class(base_parameters),   intent(inout) :: param        
-            !! Time of collision
+            !! Current run configuration parameters with SyMBA additions
          real(DP),                 intent(in)    :: t            
+            !! Time of collision
       end subroutine collision_generate_hitandrun
 
       module subroutine collision_generate_merge(self, nbody_system, param, t)
          implicit none
-            !! Merge fragment nbody_system object 
          class(collision_basic),   intent(inout) :: self          
-            !! Swiftest nbody system object
+            !! Merge fragment nbody_system object 
          class(base_nbody_system), intent(inout) :: nbody_system 
-            !! Current run configuration parameters 
+            !! Swiftest nbody system object
          class(base_parameters),   intent(inout) :: param        
-            !! The time of the collision
+            !! Current run configuration parameters 
          real(DP),                 intent(in)    :: t            
+            !! The time of the collision
       end subroutine collision_generate_merge
     
       module subroutine collision_io_collider_message(pl, collidx, collider_message)
          implicit none
-            !! Swiftest massive body object
          class(base_object),            intent(in)    :: pl               
-            !! Index of collisional colliders%idx members
+            !! Swiftest massive body object
          integer(I4B),    dimension(:), intent(in)    :: collidx          
-            !! The message to print to the screen.
+            !! Index of collisional colliders%idx members
          character(*),                  intent(inout) :: collider_message 
+            !! The message to print to the screen.
       end subroutine collision_io_collider_message
 
       module subroutine collision_io_log_regime(impactors)
          implicit none
-            !! Collision system object
          class(collision_impactors), intent(inout) :: impactors  
+            !! Collision system object
       end subroutine collision_io_log_regime
 
       module subroutine collision_io_netcdf_dump(self, param)
          implicit none
-            !! Collision storage object
          class(collision_storage), intent(inout) :: self  
-            !! Current run configuration parameters 
+            !! Collision storage object
          class(base_parameters),   intent(inout) :: param 
+            !! Current run configuration parameters 
       end subroutine collision_io_netcdf_dump
 
       module subroutine collision_io_netcdf_initialize_output(self, param)
          implicit none
-            !! Parameters used to identify a particular NetCDF dataset
          class(collision_netcdf_parameters), intent(inout) :: self  
-              !! Current run configuration parameters   
+            !! Parameters used to identify a particular NetCDF dataset
          class(base_parameters),   intent(in)    :: param 
+            !! Current run configuration parameters   
       end subroutine collision_io_netcdf_initialize_output
 
       module subroutine collision_io_netcdf_open(self, param, readonly)
          implicit none
-            !! Parameters used to identify a particular NetCDF dataset
          class(collision_netcdf_parameters), intent(inout) :: self     
-            !! Current run configuration parameters
+            !! Parameters used to identify a particular NetCDF dataset
          class(base_parameters),             intent(in)    :: param    
-            !! Logical flag indicating that this should be open read only
+            !! Current run configuration parameters
          logical, optional,                  intent(in)    :: readonly 
+            !! Logical flag indicating that this should be open read only
       end subroutine collision_io_netcdf_open
 
       module subroutine collision_io_netcdf_write_frame_snapshot(self, history, param)
          implicit none
-            !! Swiftest encounter structure
          class(collision_snapshot),   intent(in)    :: self  
-            !! Collision history object
+            !! Swiftest encounter structure
          class(encounter_storage), intent(inout) :: history 
-            !! Current run configuration parameters
+            !! Collision history object
          class(base_parameters),      intent(inout) :: param   
+            !! Current run configuration parameters
       end subroutine collision_io_netcdf_write_frame_snapshot
 
       module subroutine collision_regime_collider(self, nbody_system, param)
          implicit none 
-            !! Collision system object
          class(collision_basic),   intent(inout) :: self         
-            !! Swiftest nbody system object
+            !! Collision system object
          class(base_nbody_system), intent(in)    :: nbody_system 
-            !! Current Swiftest run configuration parameters
+            !! Swiftest nbody system object
          class(base_parameters),   intent(in)    :: param        
+            !! Current Swiftest run configuration parameters
       end subroutine collision_regime_collider
 
       module subroutine collision_check_plpl(self, nbody_system, param, t, dt, irec, lany_collision)
          implicit none
-            !! encounter list object
          class(collision_list_plpl), intent(inout) :: self           
-            !! Swiftest nbody system object
+            !! encounter list object
          class(base_nbody_system),   intent(inout) :: nbody_system   
-            !! Current run configuration parameters 
+            !! Swiftest nbody system object
          class(base_parameters),     intent(inout) :: param          
-            !! current time
+            !! Current run configuration parameters 
          real(DP),                   intent(in)    :: t              
-            !! step size
+            !! current time
          real(DP),                   intent(in)    :: dt             
-            !! Current recursion level
+            !! step size
          integer(I4B),               intent(in)    :: irec           
-            !! Returns true if any pair of encounters resulted in a collision 
+            !! Current recursion level
          logical,                    intent(out)   :: lany_collision 
+            !! Returns true if any pair of encounters resulted in a collision 
       end subroutine collision_check_plpl
 
       module subroutine collision_check_pltp(self, nbody_system, param, t, dt, irec, lany_collision)
          implicit none
-            !!  encounter list object
          class(collision_list_pltp), intent(inout) :: self           
-            !! Swiftest nbody system object
+            !!  encounter list object
          class(base_nbody_system),   intent(inout) :: nbody_system   
-            !! Current run configuration parameters 
+            !! Swiftest nbody system object
          class(base_parameters),     intent(inout) :: param          
-            !! current time
+            !! Current run configuration parameters 
          real(DP),                   intent(in)    :: t              
-            !! step size
+            !! current time
          real(DP),                   intent(in)    :: dt             
-            !! Current recursion level
+            !! step size
          integer(I4B),               intent(in)    :: irec           
-            !! Returns true if any pair of encounters resulted in a collision 
+            !! Current recursion level
          logical,                    intent(out)   :: lany_collision 
+            !! Returns true if any pair of encounters resulted in a collision 
       end subroutine collision_check_pltp
 
       module subroutine collision_resolve_consolidate_impactors(self, nbody_system, param, idx_parent, lflag)
          implicit none
-            !! Collision impactors object
          class(collision_impactors),               intent(out)   :: self         
-            !! Swiftest nbody system object
+            !! Collision impactors object
          class(base_nbody_system),                 intent(inout) :: nbody_system 
-            !! Current run configuration parameters with Swiftest additions
+            !! Swiftest nbody system object
          class(base_parameters),                   intent(in)    :: param       
-            !! Index of the two bodies considered the "parents" of the collision
+            !! Current run configuration parameters with Swiftest additions
          integer(I4B),               dimension(:), intent(inout) :: idx_parent 
-            !! Logical flag indicating whether a impactors%id was successfully created or not
+            !! Index of the two bodies considered the "parents" of the collision
          logical,                                  intent(out)   :: lflag      
+            !! Logical flag indicating whether a impactors%id was successfully created or not
       end subroutine collision_resolve_consolidate_impactors
    
       module subroutine collision_resolve_extract_plpl(self, nbody_system, param)
          implicit none
-            !! pl-pl encounter list
          class(collision_list_plpl), intent(inout) :: self         
-            !! Swiftest nbody system object
+            !! pl-pl encounter list
          class(base_nbody_system),   intent(inout) :: nbody_system 
-            !! Current run configuration parameters
+            !! Swiftest nbody system object
          class(base_parameters),     intent(in)    :: param        
+            !! Current run configuration parameters
       end subroutine collision_resolve_extract_plpl
 
       module subroutine collision_resolve_extract_pltp(self, nbody_system, param)
          implicit none
-            !! pl-tp encounter list
          class(collision_list_pltp), intent(inout) :: self   
-            !! Swiftest nbody system object
+            !! pl-tp encounter list
          class(base_nbody_system),   intent(inout) :: nbody_system
-            !! Current run configuration parameters
+            !! Swiftest nbody system object
          class(base_parameters),     intent(in)    :: param  
+            !! Current run configuration parameters
       end subroutine collision_resolve_extract_pltp
 
       module subroutine collision_resolve_make_impactors_pl(pl, idx)
          implicit none
-            !! Massive body object
          class(base_object),           intent(inout) :: pl 
-         !! Array holding the indices of the two bodies involved in the collision
+            !! Massive body object
          integer(I4B), dimension(:), intent(in)    :: idx 
+            !! Array holding the indices of the two bodies involved in the collision
       end subroutine collision_resolve_make_impactors_pl
 
       module subroutine collision_resolve_mergeaddsub(nbody_system, param, t, status)
-              !! Swiftest nbody system object
          class(base_nbody_system), intent(inout) :: nbody_system 
-              !! Current run configuration parameters with Swiftest additions 
+            !! Swiftest nbody system object
          class(base_parameters),   intent(inout) :: param  
-            !! Time of collision
+            !! Current run configuration parameters with Swiftest additions 
          real(DP),                  intent(in)    :: t      
-            !! Status flag to assign to adds
+            !! Time of collision
          integer(I4B),              intent(in)    :: status 
+            !! Status flag to assign to adds
       end subroutine collision_resolve_mergeaddsub
    
       module subroutine collision_resolve_plpl(self, nbody_system, param, t, dt, irec)
          implicit none
-            !! pl-pl encounter list
          class(collision_list_plpl), intent(inout) :: self   
-            !! Swiftest nbody system object
+            !! pl-pl encounter list
          class(base_nbody_system),   intent(inout) :: nbody_system 
-              !! Current run configuration parameters with Swiftest additions
+            !! Swiftest nbody system object
          class(base_parameters),     intent(inout) :: param  
-            !! Current simulation time
+              !! Current run configuration parameters with Swiftest additions
          real(DP),                   intent(in)    :: t      
-            !! Current simulation step size
+            !! Current simulation time
          real(DP),                   intent(in)    :: dt     
-            !! Current recursion level
+            !! Current simulation step size
          integer(I4B),               intent(in)    :: irec   
+            !! Current recursion level
       end subroutine collision_resolve_plpl
    
       module subroutine collision_resolve_pltp(self, nbody_system, param, t, dt, irec)
          implicit none
             !! pl-tp encounter list
          class(collision_list_pltp), intent(inout) :: self   
             !! Swiftest nbody system object
@@ -611,20 +620,20 @@
          real(DP),                   intent(in)    :: dt     
             !! Current recursion level
          integer(I4B),               intent(in)    :: irec   
       end subroutine collision_resolve_pltp
 
       module subroutine collision_util_add_fragments_to_collider(self, nbody_system, param)
          implicit none
-            !! Collision system object
          class(collision_basic),  intent(in)    :: self         
-            !! Swiftest nbody system object
+            !! Collision system object
          class(base_nbody_system), intent(inout) :: nbody_system 
-            !! Current Swiftest run configuration parameters
+            !! Swiftest nbody system object
          class(base_parameters),   intent(in)    :: param        
+            !! Current Swiftest run configuration parameters
       end subroutine collision_util_add_fragments_to_collider
 
       module subroutine collision_util_bounce_one(r,v,rcom,vcom,radius)
          implicit none
          real(DP), dimension(:), intent(inout) :: r,v
          real(DP), dimension(:), intent(in)    :: rcom,vcom
          real(DP),               intent(in)    :: radius
@@ -633,223 +642,236 @@
       module subroutine collision_util_dealloc_fragments(self)
          implicit none
          class(collision_fragments), intent(inout) :: self
       end subroutine collision_util_dealloc_fragments
 
       module subroutine collision_util_dealloc_snapshot(self)
          implicit none
-            !! Collsion snapshot object
          class(collision_snapshot),  intent(inout) :: self 
+            !! Collsion snapshot object
       end subroutine collision_util_dealloc_snapshot
 
       module subroutine collision_util_reset_fragments(self)
          implicit none
          class(collision_fragments), intent(inout) :: self
       end subroutine collision_util_reset_fragments
 
       module subroutine collision_util_set_coordinate_collider(self)
          implicit none
-            !! collisional system
          class(collision_basic), intent(inout) :: self      
+            !! collisional system
       end subroutine collision_util_set_coordinate_collider
 
       module subroutine collision_util_set_coordinate_fragments(self)
          implicit none
-            !! Collisional nbody_system
          class(collision_fragments), intent(inout) :: self      
+            !! Collisional nbody_system
       end subroutine collision_util_set_coordinate_fragments
 
       module subroutine collision_util_set_coordinate_impactors(self)
          implicit none
-            !! collisional system
          class(collision_impactors), intent(inout) :: self      
+            !! collisional system
       end subroutine collision_util_set_coordinate_impactors
 
       module subroutine collision_util_setup_collider(self, nbody_system, param)
          use base, only : base_nbody_system, base_parameters
          implicit none
-            !! Encounter collision system object
          class(collision_basic),   intent(inout) :: self         
-            !! Current nbody system. Used as a mold for the before/after snapshots
+            !! Encounter collision system object
          class(base_nbody_system), intent(in)    :: nbody_system 
-            !! Current Swiftest run configuration parameters
+            !! Current nbody system. Used as a mold for the before/after snapshots
          class(base_parameters),   intent(inout) :: param        
+            !! Current Swiftest run configuration parameters
       end subroutine collision_util_setup_collider
    
       module subroutine collision_util_setup_impactors_collider(self)
          implicit none
-            !! Encounter collision system object
          class(collision_basic), intent(inout) :: self   
+            !! Encounter collision system object
       end subroutine collision_util_setup_impactors_collider
    
       module subroutine collision_util_setup_fragments_collider(self, nfrag)
          implicit none
-            !! Encounter collision system object
          class(collision_basic), intent(inout) :: self  
-            !! Number of fragments to create
+            !! Encounter collision system object
          integer(I4B),           intent(in)    :: nfrag 
+            !! Number of fragments to create
       end subroutine collision_util_setup_fragments_collider
 
       module subroutine collision_util_shift_vector_to_origin(m_frag, vec_frag)
          implicit none
-            !! Fragment masses
          real(DP), dimension(:),   intent(in)    :: m_frag    
-            !! Fragment positions or velocities in the center of mass frame
+            !! Fragment masses
          real(DP), dimension(:,:), intent(inout) :: vec_frag  
+            !! Fragment positions or velocities in the center of mass frame
       end subroutine
 
       module subroutine collision_util_get_idvalues_snapshot(self, idvals)
          implicit none
-            !! Collision snapshot object
          class(collision_snapshot),               intent(in)  :: self   
-            !! Array of all id values saved in this snapshot
+            !! Collision snapshot object
          integer(I4B), dimension(:), allocatable, intent(out) :: idvals 
+            !! Array of all id values saved in this snapshot
       end subroutine collision_util_get_idvalues_snapshot
 
       module subroutine collision_util_get_energy_and_momentum(self, nbody_system, param, phase)
          use base, only : base_nbody_system, base_parameters
          implicit none
-            !! Encounter collision system object
          class(collision_basic),   intent(inout) :: self         
-            !! Swiftest nbody system object
+            !! Encounter collision system object
          class(base_nbody_system), intent(inout) :: nbody_system 
-            !! Current Swiftest run configuration parameters
+            !! Swiftest nbody system object
          class(base_parameters),   intent(inout) :: param        
-            !! One of "before" or "after", indicating which phase of the calculation this needs to be done
+            !! Current Swiftest run configuration parameters
          character(len=*),         intent(in)    :: phase        
+            !! One of "before" or "after", indicating which phase of the calculation this needs to be done
       end subroutine collision_util_get_energy_and_momentum
 
       module subroutine collision_util_index_map(self)
          implicit none
-            !! Collision storage object 
          class(collision_storage), intent(inout) :: self  
+            !! Collision storage object 
       end subroutine collision_util_index_map
 
       module subroutine collision_util_dealloc_impactors(self)
          implicit none
-            !! Collision system object
          class(collision_impactors),  intent(inout) :: self 
+            !! Collision system object
       end subroutine collision_util_dealloc_impactors
 
       module subroutine collision_util_dealloc_basic(self)
          implicit none
-            !! Collision system object
          class(collision_basic), intent(inout) :: self  
+            !! Collision system object
       end subroutine collision_util_dealloc_basic
 
-      module subroutine collision_util_snapshot(self, param, nbody_system, t, arg)
+      module subroutine collision_util_save_energy_snapshot(self, stage, nbody_system, iframe_start, iframe_end)
+         implicit none
+         class(collision_storage), intent(inout) :: self  
+            !! Collision storage object with snapshots
+         character(len=*), intent(in) :: stage
+            !! Phase of the collision, either 'before' or 'after'
+         class(base_nbody_system), intent(inout) :: nbody_system
+            !! Swiftest nbody system object with energy information stored in it
+         integer(I4B), intent(in) :: iframe_start 
+            !! Starting frame index to save the snapshot
+         integer(I4B), intent(in) :: iframe_end   
+            !! Ending frame index to save the snapshot
+      end subroutine collision_util_save_energy_snapshot
+   
+      module subroutine collision_util_take_snapshot(self, param, nbody_system, t, arg)
          implicit none
-            !! Swiftest storage object
          class(collision_storage), intent(inout)        :: self         
-            !! Current run configuration parameters
+            !! Swiftest storage object
          class(base_parameters),      intent(inout)        :: param        
-            !! Swiftest nbody system object to store
+            !! Current run configuration parameters
          class(base_nbody_system),    intent(inout)        :: nbody_system 
-            !! Time of snapshot if different from nbody_system time
+            !! Swiftest nbody system object to store
          real(DP),                    intent(in), optional :: t            
-            !! "before": takes a snapshot just before the collision. "after" takes the snapshot just after the collision.
+            !! Time of snapshot if different from nbody_system time
          character(*),                intent(in), optional :: arg          
-      end subroutine collision_util_snapshot
+            !! "before": takes a snapshot just before the collision. "after" takes the snapshot just after the collision.
+      end subroutine collision_util_take_snapshot
 
       module subroutine collision_util_set_natural_scale_factors(self)
          implicit none
-            !! collision system object
          class(collision_basic), intent(inout) :: self  
+            !! collision system object
       end subroutine collision_util_set_natural_scale_factors
 
       module subroutine collision_util_set_original_scale_factors(self)
          implicit none
-            !! collision system object
          class(collision_basic), intent(inout) :: self  
+            !! collision system object
       end subroutine collision_util_set_original_scale_factors
 
       module subroutine collision_util_setup_fragments(self, n)
          implicit none
-            !! Swiftest generic body object
          class(collision_fragments), intent(inout) :: self  
-            !! Number of particles to allocate space for
+            !! Swiftest generic body object
          integer(I4B),               intent(in)    :: n     
+            !! Number of particles to allocate space for
       end subroutine collision_util_setup_fragments
 
       module subroutine collision_util_velocity_torque(dL, mass, r, v)
          implicit none
-            !! Change in angular momentum to apply
          real(DP), dimension(:), intent(in)    :: dL   
-            !! Mass of body
+            !! Change in angular momentum to apply
          real(DP),               intent(in)    :: mass 
-            !! Position of body wrt system center of mass
+            !! Mass of body
          real(DP), dimension(:), intent(in)    :: r  
-            !! Velocity of body wrt system center of mass
+            !! Position of body wrt system center of mass
          real(DP), dimension(:), intent(inout) :: v 
+            !! Velocity of body wrt system center of mass
       end subroutine collision_util_velocity_torque
    end interface
 
    contains
 
       subroutine collision_final_fragments(self)
          !! author: David A. Minton
          !!
          !! Finalizer will deallocate all allocatables
          implicit none
-            !! Collision impactors storage object
          type(collision_fragments),  intent(inout) :: self 
+            !! Collision impactors storage object
 
          call self%dealloc()
 
          return
       end subroutine collision_final_fragments
 
       subroutine collision_final_impactors(self)
          !! author: David A. Minton
          !!
          !! Finalizer will deallocate all allocatables
          implicit none
-            !! Collision impactors storage object
          type(collision_impactors),  intent(inout) :: self 
+            !! Collision impactors storage object
 
          call self%dealloc()
 
          return
       end subroutine collision_final_impactors
 
       subroutine collision_final_plpl(self)
          !! author: David A. Minton
          !!
          !! Finalizer will deallocate all allocatables
          implicit none
-            !! PL-PL collision list object
          type(collision_list_plpl),  intent(inout) :: self 
+            !! PL-PL collision list object
 
          call self%dealloc()
 
          return
       end subroutine collision_final_plpl
 
       subroutine collision_final_pltp(self)
          !! author: David A. Minton
          !!
          !! Finalizer will deallocate all allocatables
          implicit none
-            !! PL-TP collision list object
          type(collision_list_pltp),  intent(inout) :: self 
+            !! PL-TP collision list object
 
          call self%dealloc()
 
          return
       end subroutine collision_final_pltp
 
       subroutine collision_final_basic(self)
          !! author: David A. Minton
          !!
          !! Finalizer will deallocate all allocatables
          implicit none
-            !!  Collision system object
          type(collision_basic),  intent(inout) :: self 
+            !!  Collision system object
 
          call self%dealloc()
 
          return
       end subroutine collision_final_basic
 
-
 end module collision
```

### Comparing `swiftest-2024.4.1/src/collision/collision_regime.f90` & `swiftest-2024.4.2/src/collision/collision_regime.f90`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,30 @@
 ! Swiftest is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty 
 ! of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 ! You should have received a copy of the GNU General Public License along with Swiftest. 
 ! If not, see: https://www.gnu.org/licenses. 
 
 submodule(collision) s_collision_regime
    use swiftest
-
 contains
 
-
    module subroutine collision_regime_collider(self, nbody_system, param)
       !! Author: Jennifer L.L. Pouplin, Carlisle A. Wishard, and David A. Minton 
       !!
-      !! Determine which fragmentation regime the set of impactors will be. This subroutine is a wrapper for the non-polymorphic raggle_regime_collresolve subroutine.
+      !! Determine which fragmentation regime the set of impactors will be. This subroutine is a wrapper for the non-polymorphic 
+      !! fraggle_regime_collresolve subroutine.
       !! It converts to SI units prior to calling
       implicit none 
       ! Arguments
-      class(collision_basic),   intent(inout) :: self         !! Collision system impactors object
-      class(base_nbody_system), intent(in)    :: nbody_system !! Swiftest nbody system object
-      class(base_parameters),   intent(in)    :: param        !! Current Swiftest run configuration parameters
+      class(collision_basic),   intent(inout) :: self         
+         !! Collision system impactors object
+      class(base_nbody_system), intent(in)    :: nbody_system 
+         !! Swiftest nbody system object
+      class(base_parameters),   intent(in)    :: param        
+         !! Current Swiftest run configuration parameters
       ! Internals
       real (DP) :: mtot
         
       associate(impactors => self%impactors)
       select type (nbody_system)
       class is (swiftest_nbody_system)
       select type(param)
@@ -54,82 +56,106 @@
       !! Author: Jennifer L.L. Pouplin, Carlisle A. Wishard, and David A. Minton 
       !!
       !! Determine the collisional regime of two colliding bodies based on the model by Leinhard and Stewart (2012)
       !!
       !! This is a wrapper subroutine that converts quantities to SI units and calls the main LS12 subroutine
       implicit none
       ! Arguments
-      class(collision_basic),       intent(inout) :: collider     !! The impactors to determine the regime for
-      class(swiftest_nbody_system), intent(in)    :: nbody_system !! Swiftest n-body system object
-      class(swiftest_parameters),   intent(in)    :: param        !! The current parameters
+      class(collision_basic),       intent(inout) :: collider     
+         !! The impactors to determine the regime for
+      class(swiftest_nbody_system), intent(in)    :: nbody_system 
+         !! Swiftest n-body system object
+      class(swiftest_parameters),   intent(in)    :: param        
+         !! The current parameters
       ! Internals
       integer(I4B) :: i,jtarg, jproj
       real(DP), dimension(2) :: radius_si, mass_si, density_si
       real(DP) :: min_mfrag_si, Mcb_si
       real(DP), dimension(NDIM)  :: x1_si, v1_si, x2_si, v2_si
       real(DP) :: mlr, mslr, mslr_hr, mtot, dentot, Qloss, Qmerge
-      integer(I4B), parameter :: NMASS_DIST = 3   !! Number of mass bins returned by the regime calculation (largest fragment, second largest, and remainder)  
-      real(DP), dimension(NDIM) :: Ip, rot, L_spin
+      integer(I4B), parameter :: NMASS_DIST = 3   ! Number of mass bins returned by the regime calculation (largest fragment, second
+                                                  ! largest, and remainder)  
+      real(DP), dimension(NDIM) :: Ip, rot, L_rot
       real(DP) :: radius, volume
       
       associate(impactors => collider%impactors)
 
-         ! Convert all quantities to SI units and determine which of the pair is the projectile vs. target before sending them to the regime determination subroutine
+         ! Convert all quantities to SI units and determine which of the pair is the projectile vs. target before sending them to 
+         ! the regime determination subroutine
          if (impactors%mass(1) > impactors%mass(2)) then
             jtarg = 1
             jproj = 2
          else
             jtarg = 2
             jproj = 1
          end if
-         mass_si(:)    = impactors%mass([jtarg, jproj]) * param%MU2KG         !! The two-body equivalent masses of the collider system
-         radius_si(:)  = impactors%radius([jtarg, jproj]) * param%DU2M        !! The two-body equivalent radii of the collider system
-         density_si(:) = mass_si(:) / (4.0_DP / 3._DP * PI * radius_si(:)**3) !! The two-body equivalent density of the collider system
-         x1_si(:)      = impactors%rb(:,jtarg) * param%DU2M                   !! The first body of the two-body equivalent position vector the collider system
-         v1_si(:)      = impactors%vb(:,jtarg) * param%DU2M / param%TU2S      !! The first body of the two-body equivalent velocity vector the collider system
-         x2_si(:)      = impactors%rb(:,jproj) * param%DU2M                   !! The second body of the two-body equivalent position vector the collider system
-         v2_si(:)      = impactors%vb(:,jproj) * param%DU2M / param%TU2S      !! The second body of the two-body equivalent velocity vector the collider system
-         Mcb_si        = nbody_system%cb%mass * param%MU2KG                         !! The central body mass of the system
-         min_mfrag_si  = (param%min_GMfrag / param%GU) * param%MU2KG          !! The minimum fragment mass to generate. Collider systems that would otherwise generate less massive fragments than this value will be forced to merge instead
+         ! The two-body equivalent masses of the collider system
+         mass_si(:)    = impactors%mass([jtarg, jproj]) * param%MU2KG 
+         
+         ! The two-body equivalent radii of the collider system
+         radius_si(:)  = impactors%radius([jtarg, jproj]) * param%DU2M 
+
+         ! The two-body equivalent density of the collider system
+         density_si(:) = mass_si(:) / (4.0_DP / 3._DP * PI * radius_si(:)**3) 
+
+         ! The first body of the two-body equivalent position vector the collider system
+         x1_si(:)      = impactors%rb(:,jtarg) * param%DU2M                   
+
+         ! The first body of the two-body equivalent velocity vector the collider system
+         v1_si(:)      = impactors%vb(:,jtarg) * param%DU2M / param%TU2S      
+
+         ! The second body of the two-body equivalent position vector the collider system
+         x2_si(:)      = impactors%rb(:,jproj) * param%DU2M                   
+
+         ! The second body of the two-body equivalent velocity vector the collider system
+         v2_si(:)      = impactors%vb(:,jproj) * param%DU2M / param%TU2S      
+
+         ! The central body mass of the system
+         Mcb_si        = nbody_system%cb%mass * param%MU2KG           
+         
+         ! The minimum fragment mass to generate. Collider systems that would otherwise generate less massive fragments than this 
+         ! value will be forced to merge instead
+         min_mfrag_si  = (param%min_GMfrag / param%GU) * param%MU2KG 
       
          mtot = sum(mass_si(:)) 
          dentot = sum(mass_si(:) * density_si(:)) / mtot 
 
-         !! Use the positions and velocities of the parents from indside the step (at collision) to calculate the collisional regime
+         ! Use the positions and velocities of the parents from indside the step (at collision) to calculate the collisional regime
          call collision_regime_LS12_SI(Mcb_si, mass_si(jtarg), mass_si(jproj), radius_si(jtarg), radius_si(jproj), &
                                        x1_si(:), x2_si(:), v1_si(:), v2_si(:), density_si(jtarg), density_si(jproj), &
                                        min_mfrag_si, impactors%regime, mlr, mslr, mslr_hr, Qloss, Qmerge)
 
          ! Convert back from SI to system units
          mlr = mlr / param%MU2KG
          mslr = mslr / param%MU2kg
          mslr_hr = mslr_hr / param%MU2kg
          Qloss = Qloss * (param%TU2S / param%DU2M)**2 / param%MU2KG
          Qmerge = Qmerge * (param%TU2S / param%DU2M)**2 / param%MU2KG
          mtot = mtot / param%MU2kg
 
-         ! If this is came back as a merger, check to make sure that the rotation of the merged body doesn't exceed the spin barrier
+         ! If this is came back as a merger, check to make sure that the rotation of the merged body doesn't exceed the rotation 
+         ! barrier
          if (impactors%regime == COLLRESOLVE_REGIME_MERGE) then
             volume = 4._DP / 3._DP * PI * sum(impactors%radius(:)**3)
             radius = (3._DP * volume / (4._DP * PI))**(THIRD)
 #ifdef DOCONLOC
-            do concurrent(i = 1:NDIM) shared(impactors,Ip,L_spin)
+            do concurrent(i = 1:NDIM) shared(impactors,Ip,L_rot)
 #else
             do concurrent(i = 1:NDIM)
 #endif
                Ip(i) = sum(impactors%mass(:) * impactors%Ip(i,:)) 
-               L_spin(i) = sum(impactors%L_orbit(i,:) + impactors%L_spin(i,:))
+               L_rot(i) = sum(impactors%L_orbit(i,:) + impactors%L_rot(i,:))
             end do
             Ip(:) = Ip(:) / mtot
-            rot(:) = L_spin(:) / (Ip(3) * mtot * radius**2)
-            if (.mag.rot(:) > collider%max_rot) then ! The merged body would spin too fast, so reclasify this as a hit and run
+            rot(:) = L_rot(:) / (Ip(3) * mtot * radius**2)
+            if (.mag.rot(:) > collider%max_rot) then ! The merged body would rotation too fast, so reclasify this as a hit and run
                mlr = impactors%mass(jtarg)
-               mslr = mslr_hr
+               mslr = impactors%mass(jproj)
                impactors%regime = COLLRESOLVE_REGIME_HIT_AND_RUN
-               impactors%Qloss = Qloss
+               impactors%Qloss = 0.0_DP
             else
                mlr =  mtot
                mslr = 0.0_DP
                impactors%Qloss = Qmerge
             end if
          else
             impactors%Qloss = Qloss
@@ -166,30 +192,45 @@
       !!          Outcomes during the End Stage of Planet Formation. ApJ 751, 32. https://doi.org/10.1088/0004-637X/751/1/32
       !!
       implicit none
       ! Arguments
       real(DP), intent(in)           :: Mcb, m1, m2, rad1, rad2, den1, den2, min_mfrag 
       real(DP), dimension(:), intent(in)  :: rh1, rh2, vb1, vb2
       integer(I4B), intent(out)         :: regime
-      real(DP), intent(out)          :: Mlr, Mslr, Mslr_hitandrun ! Largest and second-largest remnant defined for various regimes
-      real(DP), intent(out)          :: Qloss  !! The energy lost in the collision if it was a fragmentation event
-      real(DP), intent(out)          :: Qmerge !! The energy lost in the collision if it was a perfect merger
+      real(DP), intent(out)          :: Mlr, Mslr, Mslr_hitandrun 
+         !! Largest and second-largest remnant defined for various regimes
+      real(DP), intent(out)          :: Qloss  
+         !! The energy lost in the collision if it was a fragmentation event
+      real(DP), intent(out)          :: Qmerge 
+         !! The energy lost in the collision if it was a perfect merger
       ! Constants
-      integer(I4B), parameter :: N1 = 1  !number of objects with mass equal to the largest remnant from LS12
-      integer(I4B), parameter :: N2 = 2  !number of objects with mass larger than second largest remnant from LS12
-      real(DP), parameter   :: DENSITY1 = 1000.0_DP !standard density parameter from LS12 [kg/m3]
-      real(DP), parameter   :: MU_BAR = 0.37_DP !0.385#0.37#0.3333# 3.978 # 1/3 material parameter for hydrodynamic planet-size bodies (LS12)
-      real(DP), parameter   :: BETA = 2.85_DP !slope of sfd for remnants from LS12 2.85
-      real(DP), parameter   :: ETA = -1.50_DP !! LS12 eq. (44)
-      real(DP), parameter   :: C1 = 2.43_DP  !! Kokubo & Genda (2010) eq. (3)
-      real(DP), parameter   :: C2 = -0.0408_DP !! Kokubo & Genda (2010) eq. (3)
-      real(DP), parameter   :: C3 = 1.86_DP !! Kokubo & Genda (2010) eq. (3)
-      real(DP), parameter   :: C4 = 1.08_DP !! Kokubo & Genda (2010) eq. (3)
-      real(DP), parameter   :: CRUFU = 2.0_DP - 3 * MU_BAR ! central potential variable from Rufu and Aharonson (2019)
-      real(DP), parameter   :: SUPERCAT_QRATIO = 1.8_DP ! See Section 4.1 of LS12
+      integer(I4B), parameter :: N1 = 1 
+          !!number of objects with mass equal to the largest remnant from LS12
+      integer(I4B), parameter :: N2 = 2  
+         !! number of objects with mass larger than second largest remnant from LS12
+      real(DP), parameter   :: DENSITY1 = 1000.0_DP 
+         !! standard density parameter from LS12 [kg/m3]
+      real(DP), parameter   :: MU_BAR = 0.37_DP 
+         !!0.385#0.37#0.3333# 3.978 # 1/3 material parameter for hydrodynamic planet-size bodies (LS12)
+      real(DP), parameter   :: BETA = 2.85_DP 
+         !! slope of sfd for remnants from LS12 2.85
+      real(DP), parameter   :: ETA = -1.50_DP 
+         !! LS12 eq. (44)
+      real(DP), parameter   :: C1 = 2.43_DP 
+         !! Kokubo & Genda (2010) eq. (3)
+      real(DP), parameter   :: C2 = -0.0408_DP 
+         !! Kokubo & Genda (2010) eq. (3)
+      real(DP), parameter   :: C3 = 1.86_DP 
+         !! Kokubo & Genda (2010) eq. (3)
+      real(DP), parameter   :: C4 = 1.08_DP 
+         !! Kokubo & Genda (2010) eq. (3)
+      real(DP), parameter   :: CRUFU = 2.0_DP - 3 * MU_BAR 
+         !! central potential variable from Rufu and Aharonson (2019)
+      real(DP), parameter   :: SUPERCAT_QRATIO = 1.8_DP 
+         !! See Section 4.1 of LS12
       ! Internals
       real(DP)           :: a1, alpha, aint, b, bcrit, c_star, egy, zeta, l, lint, mu, phi, theta, ke, pe
       real(DP)           :: Qr, Qrd_pstar, Qr_erosion, Qr_supercat
       real(DP)           :: Vhr, Verosion, Vescp, Vhill, Vimp, Vsupercat
       real(DP)           :: Mint, Mtot, Mtmp, Mbig, Msmall
       real(DP)           :: Rc1, rhill 
       real(DP)           :: Mresidual
@@ -312,16 +353,16 @@
       contains
 
          function calc_Qrd_pstar(Mtarg, Mp, alpha, c_star) result(Qrd_pstar)
             !! author: Jennifer L.L. Pouplin and Carlisle A. Wishard
             !!
             !! Calculates the corrected Q* for oblique impacts. See Eq. (15) of LS12.
             !!       Reference:
-            !!       Leinhardt, Z.M., Stewart, S.T., 2012. Collisions between Gravity-dominated Bodies. I. Outcome Regimes and Scaling 
-            !!          Laws 745, 79. https://doi.org/10.1088/0004-637X/745/1/79
+            !!       Leinhardt, Z.M., Stewart, S.T., 2012. Collisions between Gravity-dominated Bodies. I. Outcome Regimes and 
+            !!          Scaling Laws 745, 79. https://doi.org/10.1088/0004-637X/745/1/79
             !! 
             implicit none
             ! Arguments
             real(DP),intent(in) :: Mtarg, Mp, alpha, c_star
             ! Result
             real(DP)      :: Qrd_pstar
             ! Internals
@@ -387,19 +428,19 @@
          function calc_b(proj_pos, proj_vel, targ_pos, targ_vel) result(sintheta)
             !! author: Jennifer L.L. Pouplin, Carlisle A. Wishard, and David A. Minton
             !!
             !! Calculates the impact factor b = sin(theta), where theta is the angle between the relative velocity
             !! and distance vectors of the target and projectile bodies. See Fig. 2 of Leinhardt and Stewart (2012)
             !! 
             implicit none
-            !! Arguments
+            ! Arguments
             real(DP), dimension(:), intent(in) :: proj_pos, proj_vel, targ_pos, targ_vel
-            !! Result
+            ! Result
             real(DP)             :: sintheta
-            !! Internals
+            ! Internals
             real(DP), dimension(NDIM)     :: imp_vel, distance, x_cross_v      
 
             imp_vel(:) = proj_vel(:) - targ_vel(:)
             distance(:) = proj_pos(:) - targ_pos(:)
             x_cross_v(:) = distance(:) .cross. imp_vel(:) 
             sintheta = norm2(x_cross_v(:)) / norm2(distance(:)) / norm2(imp_vel(:))
             return 
@@ -409,19 +450,19 @@
          function calc_c_star(Rc1) result(c_star)
             !! author: David A. Minton
             !!
             !! Calculates c_star as a function of impact equivalent radius. It interpolates between 5 for ~1 km sized bodies to
             !! 1.8 for ~10000 km sized bodies. See LS12 Fig. 4 for details.
             !! 
             implicit none
-            !! Arguments
+            ! Arguments
             real(DP), intent(in) :: Rc1
-            !! Result
+            ! Result
             real(DP)             :: c_star
-            !! Internals
+            ! Internals
             real(DP), parameter  :: loR   = 1.0e3_DP ! Lower bound of interpolation size (m)
             real(DP), parameter  :: hiR   = 1.0e7_DP ! Upper bound of interpolation size (m)
             real(DP), parameter  :: loval = 5.0_DP   ! Value of C* at lower bound
             real(DP), parameter  :: hival = 1.9_DP   ! Value of C* at upper bound
 
             if (Rc1 < loR) then
                c_star = loval
```

### Comparing `swiftest-2024.4.1/src/collision/collision_resolve.f90` & `swiftest-2024.4.2/src/collision/collision_resolve.f90`

 * *Files 9% similar despite different names*

```diff
@@ -11,23 +11,28 @@
    use swiftest
 contains
 
    module subroutine collision_resolve_consolidate_impactors(self, nbody_system, param, idx_parent, lflag)
       !! author: David A. Minton
       !! 
       !! Loops through the pl-pl collision list and groups families together by index. Outputs the indices of all impactors%id 
-      !! members, and pairs of quantities (x and v vectors, mass, radius, L_spin, and Ip) that can be used to resolve the 
+      !! members, and pairs of quantities (x and v vectors, mass, radius, L_rot, and Ip) that can be used to resolve the 
       !! collisional outcome.
       implicit none
       ! Arguments
-      class(collision_impactors),intent(out) :: self !! Collision impactors object
-      class(base_nbody_system),intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(base_parameters), intent(in) :: param !! Current run configuration parameters with Swiftest additions
-      integer(I4B), dimension(:), intent(inout) :: idx_parent !! Index of the two bodies considered the "parents" of the collision
-      logical, intent(out) :: lflag !! Logical flag indicating whether a impactors%id was successfully created or not
+      class(collision_impactors),intent(out) :: self 
+         !! Collision impactors object
+      class(base_nbody_system),intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(base_parameters), intent(in) :: param 
+         !! Current run configuration parameters with Swiftest additions
+      integer(I4B), dimension(:), intent(inout) :: idx_parent 
+         !! Index of the two bodies considered the "parents" of the collision
+      logical, intent(out) :: lflag 
+         !! Logical flag indicating whether a impactors%id was successfully created or not
       ! Internals
       type collidx_array
          integer(I4B), dimension(:), allocatable :: id
          integer(I4B), dimension(:), allocatable :: idx
       end type collidx_array
       type(collidx_array), dimension(2) :: parent_child_index_array
       integer(I4B), dimension(2)       :: nchild
@@ -80,52 +85,52 @@
             ! Consolidate the groups of collsional parents with any children they may have into a single "impactors%id" index array
             nimpactors = 2 + sum(nchild(:))
             allocate(impactors%id(nimpactors))
             impactors%id = [parent_child_index_array(1)%idx(:),parent_child_index_array(2)%idx(:)]
 
             impactors%ncoll = count(pl%lcollision(impactors%id(:)))
             impactors%id = pack(impactors%id(:), pl%lcollision(impactors%id(:)))
-            impactors%L_spin(:,:) = 0.0_DP
+            impactors%L_rot(:,:) = 0.0_DP
             impactors%Ip(:,:) = 0.0_DP
 
             ! Find the barycenter of each body along with its children, if it has any
             do j = 1, 2
                impactors%rb(:, j)  = pl%rh(:, idx_parent(j)) + cb%rb(:)
                impactors%vb(:, j)  = pl%vb(:, idx_parent(j))
                ! Assume principal axis rotation about axis corresponding to highest moment of inertia (3rd Ip)
                if (param%lrotation) then
                   impactors%Ip(:, j) = impactors%mass(j) * pl%Ip(:, idx_parent(j))
-                  impactors%L_spin(:, j) = impactors%Ip(3, j) * impactors%radius(j)**2 * pl%rot(:, idx_parent(j))
+                  impactors%L_rot(:, j) = impactors%Ip(3, j) * impactors%radius(j)**2 * pl%rot(:, idx_parent(j))
                end if
 
                if (nchild(j) > 0) then
                   do i = 1, nchild(j) ! Loop over all children and take the mass weighted mean of the properties
                      idx_child = parent_child_index_array(j)%idx(i + 1)
                      if (.not. pl%lcollision(idx_child)) cycle
                      mchild = pl%mass(idx_child)
                      xchild(:) = pl%rh(:, idx_child) + cb%rb(:)
                      vchild(:) = pl%vb(:, idx_child)
                      volchild = (4.0_DP / 3.0_DP) * PI * pl%radius(idx_child)**3
                      volume(j) = volume(j) + volchild
-                     ! Get angular momentum of the child-parent pair and add that to the spin
-                     ! Add the child's spin
+                     ! Get angular momentum of the child-parent pair and add that to the rotation
+                     ! Add the child's rotation
                      if (param%lrotation) then
                         xcom(:) = (impactors%mass(j) * impactors%rb(:,j) + mchild * xchild(:)) / (impactors%mass(j) + mchild)
                         vcom(:) = (impactors%mass(j) * impactors%vb(:,j) + mchild * vchild(:)) / (impactors%mass(j) + mchild)
                         xc(:) = impactors%rb(:, j) - xcom(:)
                         vc(:) = impactors%vb(:, j) - vcom(:)
                         xcrossv(:) = xc(:) .cross. vc(:) 
-                        impactors%L_spin(:, j) = impactors%L_spin(:, j) + impactors%mass(j) * xcrossv(:)
+                        impactors%L_rot(:, j) = impactors%L_rot(:, j) + impactors%mass(j) * xcrossv(:)
          
                         xc(:) = xchild(:) - xcom(:)
                         vc(:) = vchild(:) - vcom(:)
                         xcrossv(:) = xc(:) .cross. vc(:) 
-                        impactors%L_spin(:, j) = impactors%L_spin(:, j) + mchild * xcrossv(:)
+                        impactors%L_rot(:, j) = impactors%L_rot(:, j) + mchild * xcrossv(:)
 
-                        impactors%L_spin(:, j) = impactors%L_spin(:, j) + mchild * pl%Ip(3, idx_child)  &
+                        impactors%L_rot(:, j) = impactors%L_rot(:, j) + mchild * pl%Ip(3, idx_child)  &
                                                                                  * pl%radius(idx_child)**2 &
                                                                                  * pl%rot(:, idx_child)
                         impactors%Ip(:, j) = impactors%Ip(:, j) + mchild * pl%Ip(:, idx_child)
                      end if
 
                      ! Merge the child and parent
                      impactors%mass(j) = impactors%mass(j) + mchild
@@ -133,15 +138,15 @@
                      impactors%vb(:, j) = vcom(:)
                   end do
                end if
                density(j) = impactors%mass(j) / volume(j)
                impactors%radius(j) = (3 * volume(j) / (4 * PI))**(1.0_DP / 3.0_DP)
                if (param%lrotation) then
                   impactors%Ip(:, j) = impactors%Ip(:, j) / impactors%mass(j)
-                  impactors%rot(:,j) = impactors%L_spin(:, j) / (impactors%Ip(3,j) * impactors%mass(j) * impactors%radius(j)**2)
+                  impactors%rot(:,j) = impactors%L_rot(:, j) / (impactors%Ip(3,j) * impactors%mass(j) * impactors%radius(j)**2)
                end if
             end do
             lflag = .true.
 
             mtot = sum(impactors%mass(:))
             xcom(:) = (impactors%mass(1) * impactors%rb(:, 1) + impactors%mass(2) * impactors%rb(:, 2)) / mtot
             vcom(:) = (impactors%mass(1) * impactors%vb(:, 1) + impactors%mass(2) * impactors%vb(:, 2)) / mtot
@@ -181,17 +186,20 @@
    module subroutine collision_resolve_extract_plpl(self, nbody_system, param)
       !! author: David A. Minton
       !! 
       !! Processes the pl-pl encounter list remove only those encounters that led to a collision
       !!
       implicit none
       ! Arguments
-      class(collision_list_plpl), intent(inout) :: self         !! pl-pl encounter list
-      class(base_nbody_system),   intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(base_parameters),     intent(in)    :: param        !! Current run configuration parameters
+      class(collision_list_plpl), intent(inout) :: self         
+         !! pl-pl encounter list
+      class(base_nbody_system),   intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(base_parameters),     intent(in)    :: param        
+         !! Current run configuration parameters
       ! Internals
       logical,      dimension(:), allocatable :: lplpl_collision
       logical,      dimension(:), allocatable :: lplpl_unique_parent
       integer(I4B), dimension(:), pointer     :: plparent
       integer(I4B)                            :: nunique_parent
       integer(I8B)                            :: ncollisions, index_coll, k, nplplenc
       integer(I8B), dimension(:), allocatable :: unique_parent_idx, collision_idx
@@ -250,20 +258,23 @@
 
       return
    end subroutine collision_resolve_extract_plpl
 
 
    module subroutine collision_resolve_extract_pltp(self, nbody_system, param)
       implicit none
-      class(collision_list_pltp), intent(inout) :: self   !! pl-tp encounter list
-      class(base_nbody_system),   intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(base_parameters),     intent(in)    :: param  !! Current run configuration parameters
+      class(collision_list_pltp), intent(inout) :: self   
+         !! pl-tp encounter list
+      class(base_nbody_system),   intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(base_parameters),     intent(in)    :: param  
+         !! Current run configuration parameters
       ! Internals
       logical,      dimension(:), allocatable :: lpltp_collision
-      integer(I8B)                            :: ncollisions, index_coll, k, npltpenc
+      integer(I8B)                            :: ncollisions, k, npltpenc
       integer(I8B), dimension(:), allocatable :: collision_idx
 
       select type(nbody_system)
       class is (swiftest_nbody_system)
       select type (pl => nbody_system%pl)
       class is (swiftest_pl)
       select type (tp => nbody_system%tp)
@@ -303,16 +314,18 @@
       !! including those that collide with the children.
       !! 
       !! Adapted from David E. Kaufmann's Swifter routine swiftest_merge_pl.f90
       !!
       !! Adapted from Hal Levison's Swift routine symba5_merge.f
       implicit none
       ! Arguments
-      class(base_object),           intent(inout) :: pl !! Swiftest massive body object
-      integer(I4B), dimension(:), intent(in)      :: idx  !! Array holding the indices of the two bodies involved in the collision
+      class(base_object),           intent(inout) :: pl 
+         !! Swiftest massive body object
+      integer(I4B), dimension(:), intent(in)      :: idx  
+         !! Array holding the indices of the two bodies involved in the collision
       ! Internals
       integer(I4B)                              :: i, j, index_parent, index_child, p1, p2
       integer(I4B)                              :: nchild_inherit, nchild_orig, nchild_new
       integer(I4B), dimension(:), allocatable   :: temp
 
       select type(pl)
       class is (swiftest_pl)
@@ -362,18 +375,22 @@
       !! author:  David A. Minton
       !!
       !! Fills the pl_discards and pl_adds with removed and added bodies
       !!  
       use symba, only : symba_pl
       implicit none
       ! Arguments
-      class(base_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(base_parameters),   intent(inout) :: param        !! Current run configuration parameters with Swiftest additions
-      real(DP),                 intent(in)    :: t            !! Time of collision
-      integer(I4B),             intent(in)    :: status       !! Status flag to assign to adds
+      class(base_nbody_system), intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(base_parameters),   intent(inout) :: param        
+         !! Current run configuration parameters with Swiftest additions
+      real(DP),                 intent(in)    :: t            
+         !! Time of collision
+      integer(I4B),             intent(in)    :: status       
+         !! Status flag to assign to adds
       ! Internals
       integer(I4B) :: i, ibiggest, ismallest, iother, nimpactors, nfrag, nameidx
       logical, dimension(:), allocatable  :: lmask
       class(swiftest_pl), allocatable :: plnew, plsub
       character(*), parameter :: FRAGFMT = '("Newbody",I0.7)'
       character(*), parameter :: MERGEFMT = '(A,I0.7)'
       character(*), parameter :: MERGE_PREPEND_TEXT = "_MERGE"
@@ -455,45 +472,29 @@
             case(DISRUPTED,HIT_AND_RUN_DISRUPT)
                if (status == DISRUPTED) then
                   write(origin_type,*) "Disruption"
                else if (status == HIT_AND_RUN_DISRUPT) then
                   write(origin_type,*) "Hit and run fragmentation"
                end if
                call plnew%info(1)%copy(pl%info(ibiggest))
-               plnew%status(1) = OLD_PARTICLE
                do i = 2, nfrag
                   write(newname, FRAGFMT) fragments%id(i)
                   call plnew%info(i)%set_value(origin_type=origin_type, origin_time=t, name=newname, &
                                                 origin_rh=plnew%rh(:,i), origin_vh=plnew%vh(:,i), &
                                                 collision_id=collider%maxid_collision)
                end do
                do i = 1, nimpactors
                   if (impactors%id(i) == ibiggest) cycle
                   iother = ibiggest
                   call pl%info(impactors%id(i))%set_value(status=origin_type, discard_time=t, &
                                                             discard_rh=pl%rh(:,i), discard_vh=pl%vh(:,i), &
                                                             discard_body_id=iother)
                end do 
             case(MERGED)
-               write(origin_type,*) "Merger"
                call plnew%info(1)%copy(pl%info(ibiggest))
-               nbody_system%maxid = nbody_system%maxid + 1
-               plnew%id(1) = nbody_system%maxid
-
-               ! Appends an index number to the end of the original name to make it unique, but still identifiable as the original.
-               ! If there is already an index number appended, replace it
-               write(merge_text,MERGEFMT) MERGE_PREPEND_TEXT,plnew%id(1)
-               merge_text_length = len(trim(adjustl(merge_text)))
-               nameidx = index(plnew%info(1)%name, MERGE_PREPEND_TEXT) - 1
-               if (nameidx < 0) nameidx = min(len(trim(adjustl(plnew%info(1)%name))), NAMELEN - merge_text_length)
-               write(newname,*) trim(adjustl(plnew%info(1)%name(1:nameidx))) // trim(adjustl(merge_text))
-               plnew%status(1) = NEW_PARTICLE
-               call plnew%info(1)%set_value(origin_type=origin_type, origin_time=t, name=newname, &
-                                            origin_rh=plnew%rh(:,1), origin_vh=plnew%vh(:,1), &
-                                            collision_id=collider%maxid_collision)
                do i = 1, nimpactors
                   if (impactors%id(i) == ibiggest) cycle
 
                   iother = ibiggest
                   call pl%info(impactors%id(i))%set_value(status="MERGED", discard_time=t, discard_rh=pl%rh(:,i), &
                                                             discard_vh=pl%vh(:,i), discard_body_id=iother)
                end do 
@@ -528,16 +529,14 @@
             allocate(lmask, mold=pl%lmask)
             lmask(:) = .false.
             lmask(impactors%id(:)) = .true.
             
             allocate(plsub, mold=pl)
             call pl%spill(plsub, lmask, ldestructive=.false.)
 
-            ! call pl_discards%append(plsub, lsource_mask=[(.true., i = 1, nimpactors)])
-
             ! Save the before/after snapshots
             select type(before => collider%before)
             class is (swiftest_nbody_system)
                call move_alloc(plsub, before%pl)
             end select
 
             select type(after => collider%after)
@@ -557,96 +556,98 @@
    module subroutine collision_resolve_plpl(self, nbody_system, param, t, dt, irec)
       !! author: David A. Minton
       !! 
       !! Process the pl-pl collision list, then modifiy the massive bodies based on the outcome of the collision
       !! 
       implicit none
       ! Arguments
-      class(collision_list_plpl), intent(inout) :: self   !! Swiftest pl-pl encounter list
-      class(base_nbody_system),   intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(base_parameters),     intent(inout) :: param  !! Current run configuration parameters with Swiftest additions
-      real(DP),                   intent(in)    :: t      !! Current simulation time
-      real(DP),                   intent(in)    :: dt     !! Current simulation step size
-      integer(I4B),               intent(in)    :: irec   !! Current recursion level
+      class(collision_list_plpl), intent(inout) :: self   
+         !! Swiftest pl-pl encounter list
+      class(base_nbody_system),   intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(base_parameters),     intent(inout) :: param  
+         !! Current run configuration parameters with Swiftest additions
+      real(DP),                   intent(in)    :: t      
+         !! Current simulation time
+      real(DP),                   intent(in)    :: dt     
+         !! Current simulation step size
+      integer(I4B),               intent(in)    :: irec   
+         !! Current recursion level
       ! Internals
       real(DP) :: E_before, E_after, mnew
-      real(DP), dimension(NDIM) ::L_before, L_after, dL
       logical :: lplpl_collision
-      character(len=STRMAX) :: timestr, idstr
+      character(len=STRMAX) :: timestr
       integer(I4B), dimension(2) :: idx_parent       !! Index of the two bodies considered the "parents" of the collision
       logical  :: lgoodcollision
-      integer(I4B) :: i, j, nnew, loop
+      integer(I4B) :: i, j, nnew, loop, npl_orig, npl_new, iframe_start, iframe_end
       integer(I8B) :: k, ncollisions
       integer(I4B), dimension(:), allocatable :: idnew
       integer(I4B), parameter :: MAXCASCADE = 1000
   
       select type (nbody_system)
       class is (swiftest_nbody_system)
       select type(pl => nbody_system%pl)
       class is (swiftest_pl)
       select type(param)
       class is (swiftest_parameters)
          associate(plpl_collision => nbody_system%plpl_collision, &
-                   collision_history => nbody_system%collision_history, pl => nbody_system%pl, cb => nbody_system%cb, &
-                   collider => nbody_system%collider, fragments => nbody_system%collider%fragments, &
+                   collision_history => nbody_system%collision_history, &
+                   pl => nbody_system%pl, cb => nbody_system%cb, &
+                   collider => nbody_system%collider, &
+                   fragments => nbody_system%collider%fragments, &
                    impactors => nbody_system%collider%impactors)
             if (plpl_collision%nenc == 0) return ! No collisions to resolve
 
-
             ! Make sure that the heliocentric and barycentric coordinates are consistent with each other
             call pl%vb2vh(nbody_system%cb) 
             call pl%rh2rb(nbody_system%cb)
 
             ! Get the energy before the collision is resolved
             if (param%lenergy) then
                call nbody_system%get_energy_and_momentum(param)
                E_before = nbody_system%te
-               L_before(:) = nbody_system%L_total(:)
             end if
 
             do loop = 1, MAXCASCADE
                associate( idx1 => plpl_collision%index1, idx2 => plpl_collision%index2)
                   ncollisions = plpl_collision%nenc
+                  if (ncollisions == 0) exit
                   write(timestr,*) t
                   call swiftest_io_log_one_message(COLLISION_LOG_OUT, "")
                   call swiftest_io_log_one_message(COLLISION_LOG_OUT,&
                                                             "***********************************************************" // &
                                                             "***********************************************************")
                   call swiftest_io_log_one_message(COLLISION_LOG_OUT, "Collision between massive bodies detected at time t = " // &
                                                             trim(adjustl(timestr)))
                   call swiftest_io_log_one_message(COLLISION_LOG_OUT, &
                                                             "***********************************************************" // &
                                                             "***********************************************************")
-
+                  iframe_start = collision_history%iframe + 1
                   do k = 1_I8B, ncollisions
                      idx_parent(1) = pl%kin(idx1(k))%parent
                      idx_parent(2) = pl%kin(idx2(k))%parent
                      call impactors%consolidate(nbody_system, param, idx_parent, lgoodcollision)
                      if ((.not. lgoodcollision) .or. any(pl%status(idx_parent(:)) /= COLLIDED)) cycle
 
-                     ! Advance the collision id number and save it
-                     collider%maxid_collision = max(collider%maxid_collision, maxval(nbody_system%pl%info(:)%collision_id))
-                     collider%maxid_collision = collider%maxid_collision + 1
-                     collider%collision_id = collider%maxid_collision
-                     write(idstr,*) collider%collision_id
-                     call swiftest_io_log_one_message(COLLISION_LOG_OUT, "collision_id " // trim(adjustl(idstr)))
-
                      ! Get the collision regime
                      call collider%get_regime(nbody_system, param)
 
+                     ! Temporarily store the original status of the parent bodies so we can compute the energy change correctly
                      call collision_history%take_snapshot(param,nbody_system, t, "before") 
 
                      ! Generate the new bodies resulting from the collision
                      call collider%generate(nbody_system, param, t)
 
                      call collision_history%take_snapshot(param,nbody_system, t, "after") 
 
                      plpl_collision%status(k) = collider%status
                      call impactors%dealloc()
                   end do
+                  iframe_end = collision_history%iframe
+                  if (param%lenergy) call collision_history%save_energy_snapshot("before", nbody_system, iframe_start, iframe_end)
 
                   ! Destroy the collision list now that the collisions are resolved
                   call plpl_collision%setup(0_I8B)
 
                   if ((nbody_system%pl_adds%nbody == 0) .and. (.not.any(pl%ldiscard(:)))) exit
                   if (allocated(idnew)) deallocate(idnew)
                   nnew = nbody_system%pl_adds%nbody
@@ -660,32 +661,20 @@
                   ! Destroy the add/discard list so that we don't append the same body multiple times if another collision 
                   ! is detected
                   call nbody_system%pl_discards%setup(0, param)
                   call nbody_system%pl_adds%setup(0, param)
 
                   if (param%lenergy) then
                      call nbody_system%get_energy_and_momentum(param)
-                     L_after(:) = nbody_system%L_total(:)
-                     dL = L_after(:) - L_before(:)
-
-                     ! Add some velocity torque to the new bodies to remove residual angular momentum difference
-                     do j = 1, nnew
-                        i = findloc(pl%id,idnew(j),dim=1)
-                        if (i == 0) cycle
-                        call collision_util_velocity_torque(-dL * pl%mass(i)/mnew, pl%mass(i), pl%rb(:,i), pl%vb(:,i)) 
-                     end do
-
-                     call nbody_system%get_energy_and_momentum(param)
+                     ! call nbody_system%get_energy_and_momentum(param)
                      E_after = nbody_system%te
                      nbody_system%E_collisions = nbody_system%E_collisions + (E_after - E_before)
-                     L_after(:) = nbody_system%L_total(:)
-                     dL = L_after(:) - L_before(:)
+                     call collision_history%save_energy_snapshot("after", nbody_system, iframe_start, iframe_end)
                   end if
 
-
                   ! Check whether or not any of the particles that were just added are themselves in a collision state. This will 
                   ! generate a new plpl_collision 
                   call self%collision_check(nbody_system, param, t, dt, irec, lplpl_collision)
 
                   if (.not.lplpl_collision) exit
                   if (loop == MAXCASCADE) then
                      call swiftest_io_log_one_message(COLLISION_LOG_OUT,"A runaway collisional cascade has been detected in " // &
@@ -707,108 +696,92 @@
    end subroutine collision_resolve_plpl
 
 
    module subroutine collision_resolve_pltp(self, nbody_system, param, t, dt, irec)
       !! author: David A. Minton
       !! 
       !! Process the pl-tp collision list, then modifiy the massive bodies based on the outcome of the collision
-      !! 
       implicit none
       ! Arguments
-      class(collision_list_pltp), intent(inout) :: self   !! Swiftest pl-pl encounter list
-      class(base_nbody_system),   intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(base_parameters),     intent(inout) :: param  !! Current run configuration parameters with Swiftest additions
-      real(DP),                   intent(in)    :: t      !! Current simulation tim
-      real(DP),                   intent(in)    :: dt     !! Current simulation step size
-      integer(I4B),               intent(in)    :: irec   !! Current recursion level
+      class(collision_list_pltp), intent(inout) :: self   
+         !! Swiftest pl-pl encounter list
+      class(base_nbody_system),   intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(base_parameters),     intent(inout) :: param  
+         !! Current run configuration parameters with Swiftest additions
+      real(DP),                   intent(in)    :: t      
+         !! Current simulation time
+      real(DP),                   intent(in)    :: dt     
+         !! Current simulation step size
+      integer(I4B),               intent(in)    :: irec   
+         !! Current recursion level
       ! Internals
       class(swiftest_pl), allocatable :: plsub
       class(swiftest_tp), allocatable :: tpsub
-      logical :: lpltp_collision
-      character(len=STRMAX) :: timestr, idstr
-      integer(I4B) :: i, j, nnew, loop
+      character(len=STRMAX) :: timestr
       integer(I8B) :: k, ncollisions
-      integer(I4B), dimension(:), allocatable :: idnew      
-      logical, dimension(:), allocatable :: lmask
+      logical, dimension(:), allocatable :: ldiscard_pl, ldiscard_tp
      
       ! Make sure coordinate systems are all synced up due to being inside the recursion at this point
       select type(nbody_system)
       class is (swiftest_nbody_system)
       select type(param)
       class is (swiftest_parameters)
          associate(pltp_collision => nbody_system%pltp_collision, &
-            collision_history => nbody_system%collision_history, pl => nbody_system%pl, cb => nbody_system%cb, &
-            tp => nbody_system%tp, collider => nbody_system%collider, impactors => nbody_system%collider%impactors)
+            collision_history => nbody_system%collision_history, &
+            pl => nbody_system%pl, &
+            cb => nbody_system%cb, &
+            tp => nbody_system%tp, &
+            collider => nbody_system%collider, &
+            impactors => nbody_system%collider%impactors)
+
             call pl%vb2vh(nbody_system%cb)
             call tp%vb2vh(nbody_system%cb%vb)
             call pl%b2h(nbody_system%cb)
             call tp%b2h(nbody_system%cb)
 
             ! Restructure the massive bodies based on the outcome of the collision
             call tp%rearray(nbody_system, param)
 
             ! Check for discards
             call nbody_system%tp%discard(nbody_system, param)
 
             associate(idx1 => pltp_collision%index1, idx2 => pltp_collision%index2)
                ncollisions = pltp_collision%nenc
                write(timestr,*) t
-               call swiftest_io_log_one_message(COLLISION_LOG_OUT, "")
-               call swiftest_io_log_one_message(COLLISION_LOG_OUT,"***********************************************************" // &
-                                                                  "***********************************************************")
-               call swiftest_io_log_one_message(COLLISION_LOG_OUT, "Collision between test particle and massive body detected " // &
-                                                                   "at time t = " // trim(adjustl(timestr)))
-               call swiftest_io_log_one_message(COLLISION_LOG_OUT,"***********************************************************" // &
-                                                                  "***********************************************************")
-
                do k = 1_I8B, ncollisions
-                  ! Advance the collision id number and save it
-                  collider%maxid_collision = max(collider%maxid_collision, maxval(nbody_system%pl%info(:)%collision_id))
-                  collider%maxid_collision = collider%maxid_collision + 1
-                  collider%collision_id = collider%maxid_collision
-                  write(idstr,*) collider%collision_id
-                  call swiftest_io_log_one_message(COLLISION_LOG_OUT, "collision_id " // trim(adjustl(idstr)))
-                  collider%impactors%regime = COLLRESOLVE_REGIME_MERGE
-                  allocate(lmask, mold=pl%lmask)
-                  lmask(:) = .false.
-                  lmask(idx1(k)) = .true.
-                  
-                  allocate(plsub, mold=pl)
-                  call pl%spill(plsub, lmask, ldestructive=.false.)
-      
-                  ! Save the before snapshots
-                  select type(before => collider%before)
-                  class is (swiftest_nbody_system)
-                     call move_alloc(plsub, before%pl)
-                  end select
-
-                  deallocate(lmask)
-                  allocate(lmask, mold=tp%lmask)
-                  lmask(:) = .false.
-                  lmask(idx2(k)) = .true.
-                  
-                  allocate(tpsub, mold=tp)
-                  call tp%spill(tpsub, lmask, ldestructive=.false.)
-      
-                  ! Save the before snapshots
-                  select type(before => collider%before)
-                  class is (swiftest_nbody_system)
-                     call move_alloc(tpsub, before%tp)
-                  end select
-
-                  call collision_history%take_snapshot(param,nbody_system, t, "particle") 
-
-                  call impactors%dealloc()
+                  call swiftest_io_log_one_message(COLLISION_LOG_OUT, "")
+                  call swiftest_io_log_one_message(COLLISION_LOG_OUT,"***********************************************************" &
+                                                                  // "***********************************************************")
+                  call swiftest_io_log_one_message(COLLISION_LOG_OUT, "Collision between test particle and massive body detected " &
+                                                                  //  "at time t = " // trim(adjustl(timestr)))
+                  call swiftest_io_log_one_message(COLLISION_LOG_OUT,"***********************************************************" &
+                                                                 //  "***********************************************************")
+
+                  impactors%regime = COLLRESOLVE_REGIME_MERGE
+                  allocate(ldiscard_pl, mold=pl%ldiscard)
+                  ldiscard_pl(:) = .false.
+                  ldiscard_tp(idx1(k)) = .true.
+
+                  allocate(ldiscard_tp, mold=tp%ldiscard)
+                  ldiscard_tp(:) = .false.
+                  ldiscard_tp(idx2(k)) = .true.
+                 
+                  ! Save the system snapshot
+                  call tp%save_discard(ldiscard_pl,nbody_system,collider%before)
+                  call pl%save_discard(ldiscard_tp,nbody_system,collider%before)
+                  call collision_history%take_snapshot(param,nbody_system, t, "before") 
+                  call pl%save_discard(ldiscard_tp,nbody_system,collider%after)
+                  call collision_history%take_snapshot(param,nbody_system, t, "after") 
                end do
 
                ! Destroy the collision list now that the collisions are resolved
                call pltp_collision%setup(0_I8B)
 
             end associate
-
          end associate
       end select
       end select
 
       return
    end subroutine collision_resolve_pltp
```

### Comparing `swiftest-2024.4.1/src/collision/collision_util.f90` & `swiftest-2024.4.2/src/collision/collision_util.f90`

 * *Files 9% similar despite different names*

```diff
@@ -13,17 +13,20 @@
 
    module subroutine collision_util_add_fragments_to_collider(self, nbody_system, param)
       !! Author: David A. Minton
       !!
       !! Adds fragments to the temporary system pl object
       implicit none
       ! Arguments
-      class(collision_basic),   intent(in)    :: self      !! Collision system system object
-      class(base_nbody_system), intent(inout) :: nbody_system    !! Swiftest nbody system object
-      class(base_parameters),   intent(in)    :: param     !! Current Swiftest run configuration parameters
+      class(collision_basic),   intent(in)    :: self      
+         !! Collision system system object
+      class(base_nbody_system), intent(inout) :: nbody_system    
+         !! Swiftest nbody system object
+      class(base_parameters),   intent(in)    :: param    
+          !! Current Swiftest run configuration parameters
       ! Internals
       integer(I4B) :: i, npl_before, npl_after, nfrag
       logical, dimension(:), allocatable :: lexclude
 
       select type(nbody_system)
       class is (swiftest_nbody_system)
          associate(fragments => self%fragments, impactors => self%impactors, pl => nbody_system%pl, cb => nbody_system%cb)
@@ -92,16 +95,18 @@
 
    module subroutine collision_util_get_idvalues_snapshot(self, idvals)
       !! author: David A. Minton
       !!
       !! Returns an array of all id values saved in this snapshot
       implicit none
       ! Arguments
-      class(collision_snapshot),               intent(in)  :: self   !! Collision snapshot object
-      integer(I4B), dimension(:), allocatable, intent(out) :: idvals !! Array of all id values saved in this snapshot
+      class(collision_snapshot),               intent(in)  :: self   
+         !! Collision snapshot object
+      integer(I4B), dimension(:), allocatable, intent(out) :: idvals 
+         !! Array of all id values saved in this snapshot
       ! Internals
       integer(I4B) :: npl_before, ntp_before, npl_after, ntp_after, ntot, nlo, nhi
 
       select type(before => self%collider%before)
       class is (swiftest_nbody_system)
       select type(after => self%collider%after)
       class is (swiftest_nbody_system)
@@ -146,19 +151,22 @@
    module subroutine collision_util_get_energy_and_momentum(self, nbody_system, param, phase)
       !! Author: David A. Minton
       !!
       !! Calculates total system energy in either the pre-collision outcome state (phase = "before") or the post-collision outcome 
       !! state (lbefore = .false.)
       implicit none
       ! Arguments
-      class(collision_basic),   intent(inout) :: self         !! Encounter collision system object
-      class(base_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(base_parameters),   intent(inout) :: param        !! Current Swiftest run configuration parameters
-      character(len=*),         intent(in)    :: phase        !! One of "before" or "after", indicating which phase of the 
-                                                              !!    calculation this needs to be done
+      class(collision_basic),   intent(inout) :: self         
+         !! Collision system object
+      class(base_nbody_system), intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(base_parameters),   intent(inout) :: param        
+         !! Current Swiftest run configuration parameters
+      character(len=*),         intent(in)    :: phase        
+         !! One of "before" or "after", indicating which phase of the calculation this needs to be done
       ! Internals
       integer(I4B) :: i, phase_val, nfrag
 
       select case(phase)
       case("before")
          phase_val = 1
       case("after")
@@ -177,66 +185,66 @@
             if (phase_val == 1) then
 #ifdef DOCONLOC
                do concurrent(i = 1:2) shared(impactors)
 #else
                do concurrent(i = 1:2)
 #endif
                   impactors%ke_orbit(i) = 0.5_DP * impactors%mass(i) * dot_product(impactors%vc(:,i), impactors%vc(:,i))
-                  impactors%ke_spin(i) = 0.5_DP * impactors%mass(i) * impactors%radius(i)**2 * impactors%Ip(3,i)  & 
+                  impactors%ke_rot(i) = 0.5_DP * impactors%mass(i) * impactors%radius(i)**2 * impactors%Ip(3,i)  & 
                                                 * dot_product(impactors%rot(:,i), impactors%rot(:,i))
                   impactors%be(i) = -3 * impactors%Gmass(i) * impactors%mass(i) / (5 * impactors%radius(i))
                   impactors%L_orbit(1,i) = impactors%mass(i) * (impactors%rc(2,i) * impactors%vc(3,i) &
                                                               - impactors%rc(3,i) * impactors%vc(2,i))
                   impactors%L_orbit(2,i) = impactors%mass(i) * (impactors%rc(3,i) * impactors%vc(1,i) &
                                                               - impactors%rc(1,i) * impactors%vc(3,i))
                   impactors%L_orbit(3,i) = impactors%mass(i) * (impactors%rc(1,i) * impactors%vc(2,i) &
                                                               - impactors%rc(2,i) * impactors%vc(1,i))
-                  impactors%L_spin(:,i) = impactors%mass(i) * impactors%radius(i)**2 * impactors%Ip(3,i) * impactors%rot(:,i)
+                  impactors%L_rot(:,i) = impactors%mass(i) * impactors%radius(i)**2 * impactors%Ip(3,i) * impactors%rot(:,i)
                end do
                self%L_orbit(:,phase_val) = sum(impactors%L_orbit(:,1:2),dim=2)
-               self%L_spin(:,phase_val) = sum(impactors%L_spin(:,1:2),dim=2)
-               self%L_total(:,phase_val) = self%L_orbit(:,phase_val) + self%L_spin(:,phase_val) 
+               self%L_rot(:,phase_val) = sum(impactors%L_rot(:,1:2),dim=2)
+               self%L_total(:,phase_val) = self%L_orbit(:,phase_val) + self%L_rot(:,phase_val) 
                self%ke_orbit(phase_val) = sum(impactors%ke_orbit(1:2))
-               self%ke_spin(phase_val) = sum(impactors%ke_spin(1:2))
+               self%ke_rot(phase_val) = sum(impactors%ke_rot(1:2))
                self%be(phase_val) = sum(impactors%be(1:2))
                call swiftest_util_get_potential_energy(2, [(.true., i = 1, 2)], 0.0_DP, impactors%Gmass, impactors%mass, & 
                                                             impactors%rb, self%pe(phase_val))
-               self%te(phase_val) = self%ke_orbit(phase_val) + self%ke_spin(phase_val) + self%be(phase_val) + self%pe(phase_val)
+               self%te(phase_val) = self%ke_orbit(phase_val) + self%ke_rot(phase_val) + self%be(phase_val) + self%pe(phase_val)
             else if (phase_val == 2) then
 #ifdef DOCONLOC
                do concurrent(i = 1:nfrag) shared(fragments)
 #else
                do concurrent(i = 1:nfrag)
 #endif
                   fragments%ke_orbit(i) = 0.5_DP * fragments%mass(i) * dot_product(fragments%vc(:,i), fragments%vc(:,i))
-                  fragments%ke_spin(i) = 0.5_DP * fragments%mass(i) * fragments%radius(i)**2 * fragments%Ip(3,i) & 
+                  fragments%ke_rot(i) = 0.5_DP * fragments%mass(i) * fragments%radius(i)**2 * fragments%Ip(3,i) & 
                                                 * dot_product(fragments%rot(:,i), fragments%rot(:,i))
                   fragments%L_orbit(1,i) = fragments%mass(i) * (fragments%rc(2,i) * fragments%vc(3,i) - &
                                                                 fragments%rc(3,i) * fragments%vc(2,i))
                   fragments%L_orbit(2,i) = fragments%mass(i) * (fragments%rc(3,i) * fragments%vc(1,i) - &
                                                                 fragments%rc(1,i) * fragments%vc(3,i))
                   fragments%L_orbit(3,i) = fragments%mass(i) * (fragments%rc(1,i) * fragments%vc(2,i) - &
                                                                 fragments%rc(2,i) * fragments%vc(1,i))
-                  fragments%L_spin(:,i) = fragments%mass(i) * fragments%radius(i)**2 * fragments%Ip(3,i) * fragments%rot(:,i)
+                  fragments%L_rot(:,i) = fragments%mass(i) * fragments%radius(i)**2 * fragments%Ip(3,i) * fragments%rot(:,i)
                end do
                call swiftest_util_get_potential_energy(nfrag, [(.true., i = 1, nfrag)], 0.0_DP, fragments%Gmass, fragments%mass, &
                                                       fragments%rb, fragments%pe)
                fragments%be = sum(-3*fragments%Gmass(1:nfrag)*fragments%mass(1:nfrag)/(5*fragments%radius(1:nfrag)))
                fragments%L_orbit_tot(:) = sum(fragments%L_orbit(:,1:nfrag),dim=2)
-               fragments%L_spin_tot(:) = sum(fragments%L_spin(:,1:nfrag),dim=2)
+               fragments%L_rot_tot(:) = sum(fragments%L_rot(:,1:nfrag),dim=2)
                fragments%ke_orbit_tot = sum(fragments%ke_orbit(1:nfrag))
-               fragments%ke_spin_tot = sum(fragments%ke_spin(1:nfrag))
+               fragments%ke_rot_tot = sum(fragments%ke_rot(1:nfrag))
                self%L_orbit(:,phase_val) = fragments%L_orbit_tot(:)
-               self%L_spin(:,phase_val) = fragments%L_spin_tot(:)
-               self%L_total(:,phase_val) = self%L_orbit(:,phase_val) + self%L_spin(:,phase_val) 
+               self%L_rot(:,phase_val) = fragments%L_rot_tot(:)
+               self%L_total(:,phase_val) = self%L_orbit(:,phase_val) + self%L_rot(:,phase_val) 
                self%ke_orbit(phase_val) = fragments%ke_orbit_tot
-               self%ke_spin(phase_val) = fragments%ke_spin_tot
+               self%ke_rot(phase_val) = fragments%ke_rot_tot
                self%be(phase_val) = fragments%be
                self%pe(phase_val) = fragments%pe
-               self%te(phase_val) = self%ke_orbit(phase_val) + self%ke_spin(phase_val) + self%be(phase_val) + self%pe(phase_val)
+               self%te(phase_val) = self%ke_orbit(phase_val) + self%ke_rot(phase_val) + self%be(phase_val) + self%pe(phase_val)
             end if
 
          end associate
       end select
       end select
 
       return
@@ -245,15 +253,16 @@
 
    module subroutine collision_util_index_map(self)
       !! author: David A. Minton
       !!
       !! Maps body id values to storage index values so we don't have to use unlimited dimensions for id
       implicit none
       ! Arguments
-      class(collision_storage), intent(inout) :: self  !! Swiftest storage object
+      class(collision_storage), intent(inout) :: self  
+         !! Collision storage object
       ! Internals
       integer(I4B), dimension(:), allocatable :: idvals
       real(DP), dimension(:), allocatable :: tvals
 
       call self%get_index_values(idvals, tvals)
 
       ! Consolidate ids to only unique values
@@ -269,15 +278,16 @@
 
    module subroutine collision_util_dealloc_snapshot(self)
       !! author: David A. Minton
       !!
       !! Finalizer will deallocate all allocatables
       implicit none
       ! Arguments
-      class(collision_snapshot),  intent(inout) :: self !! Collsion snapshot object
+      class(collision_snapshot),  intent(inout) :: self 
+         !! Collsion snapshot object
 
       if (allocated(self%collider)) then
          call self%collider%dealloc()
          deallocate(self%collider)
       end if
 
       call self%encounter_snapshot%dealloc()
@@ -289,24 +299,25 @@
    module subroutine collision_util_dealloc_impactors(self)
       !! author: David A. Minton
       !!
       !! Resets the collider object variables to 0 and deallocates the index and mass distributions
       implicit none
       ! Arguments
       class(collision_impactors),  intent(inout) :: self
+         !! Collision impactors object
 
       if (allocated(self%id)) deallocate(self%id)
       if (allocated(self%mass_dist)) deallocate(self%mass_dist)
       self%ncoll = 0
       self%rb(:,:) = 0.0_DP
       self%vb(:,:) = 0.0_DP
       self%rot(:,:) = 0.0_DP
-      self%L_spin(:,:) = 0.0_DP
+      self%L_rot(:,:) = 0.0_DP
       self%L_orbit(:,:) = 0.0_DP
-      self%ke_spin(:) = 0.0_DP
+      self%ke_rot(:) = 0.0_DP
       self%ke_orbit(:) = 0.0_DP
       self%Ip(:,:) = 0.0_DP
       self%mass(:) = 0.0_DP
       self%radius(:) = 0.0_DP
       self%Qloss = 0.0_DP
       self%regime = 0
 
@@ -325,14 +336,15 @@
    module subroutine collision_util_dealloc_fragments(self)
       !! author: David A. Minton
       !!
       !! Deallocates all allocatables
       implicit none
       ! Arguments
       class(collision_fragments),  intent(inout) :: self
+         !! Collision fragments object
 
       self%nbody = 0
       if (allocated(self%id)) deallocate(self%id)
       if (allocated(self%info)) deallocate(self%info) 
       if (allocated(self%status)) deallocate(self%status) 
       if (allocated(self%rh)) deallocate(self%rh)
       if (allocated(self%vh)) deallocate(self%vh)
@@ -349,29 +361,30 @@
       if (allocated(self%radius)) deallocate(self%radius)
       if (allocated(self%density)) deallocate(self%density)
       if (allocated(self%rmag)) deallocate(self%rmag)
       if (allocated(self%vmag)) deallocate(self%vmag)
       if (allocated(self%rotmag)) deallocate(self%rotmag)
       if (allocated(self%origin_body)) deallocate(self%origin_body)
       if (allocated(self%L_orbit)) deallocate(self%L_orbit)
-      if (allocated(self%L_spin)) deallocate(self%L_spin)
+      if (allocated(self%L_rot)) deallocate(self%L_rot)
       if (allocated(self%ke_orbit)) deallocate(self%ke_orbit)
-      if (allocated(self%ke_spin)) deallocate(self%ke_spin)
+      if (allocated(self%ke_rot)) deallocate(self%ke_rot)
 
       return
    end subroutine collision_util_dealloc_fragments
 
 
    module subroutine collision_util_dealloc_basic(self)
       !! author: David A. Minton
       !!
       !! Resets the collider nbody_system and deallocates all allocatables
       implicit none
       ! Arguments
-      class(collision_basic), intent(inout) :: self  !! Collision system object
+      class(collision_basic), intent(inout) :: self  
+         !! Collision system object
 
       if (allocated(self%impactors)) then 
          call self%impactors%dealloc()
          deallocate(self%impactors)
       end if
 
       if (allocated(self%fragments)) then
@@ -394,18 +407,18 @@
             if (allocated(after%pl)) deallocate(after%pl)
             if (allocated(after%tp)) deallocate(after%tp)
          end select
          deallocate(self%after)
       end if
 
       self%L_orbit(:,:) = 0.0_DP
-      self%L_spin(:,:) = 0.0_DP
+      self%L_rot(:,:) = 0.0_DP
       self%L_total(:,:) = 0.0_DP
       self%ke_orbit(:) = 0.0_DP
-      self%ke_spin(:) = 0.0_DP
+      self%ke_rot(:) = 0.0_DP
       self%pe(:) = 0.0_DP
       self%te(:) = 0.0_DP
 
       self%dscale = 1.0_DP 
       self%mscale = 1.0_DP 
       self%tscale = 1.0_DP 
       self%vscale = 1.0_DP 
@@ -421,14 +434,15 @@
       !! author: David A. Minton
       !!
       !! Resets all position and velocity-dependent fragment quantities in order to do a fresh calculation (does not reset mass, 
       !! radius, or other values that get set prior to the call to fraggle_generate)
       implicit none
       ! Arguments
       class(collision_fragments), intent(inout) :: self
+         !! Collision fragments object
 
       self%rc(:,:) = 0.0_DP
       self%vc(:,:) = 0.0_DP
       self%rh(:,:) = 0.0_DP
       self%vh(:,:) = 0.0_DP
       self%rb(:,:) = 0.0_DP
       self%vb(:,:) = 0.0_DP
@@ -438,36 +452,38 @@
       self%n_unit(:,:) = 0.0_DP
 
       self%rmag(:) = 0.0_DP
       self%vmag(:) = 0.0_DP
       self%rotmag(:) = 0.0_DP
 
       self%L_orbit_tot(:) = 0.0_DP 
-      self%L_spin_tot(:)  = 0.0_DP 
+      self%L_rot_tot(:)  = 0.0_DP 
       self%L_orbit(:,:)   = 0.0_DP 
-      self%L_spin(:,:)    = 0.0_DP 
+      self%L_rot(:,:)    = 0.0_DP 
       self%ke_orbit_tot   = 0.0_DP 
-      self%ke_spin_tot    = 0.0_DP 
+      self%ke_rot_tot    = 0.0_DP 
       self%pe             = 0.0_DP 
       self%be             = 0.0_DP 
       self%ke_orbit(:)    = 0.0_DP 
-      self%ke_spin(:)     = 0.0_DP 
+      self%ke_rot(:)     = 0.0_DP 
 
       return
    end subroutine collision_util_reset_fragments
 
 
    module subroutine collision_util_setup_fragments(self, n)
       !! author: David A. Minton
       !!
       !! Constructor for fragment class. Allocates space for all particles and
       implicit none
       ! Arguments
-      class(collision_fragments), intent(inout) :: self  !! Swiftest generic body object
-      integer(I4B),               intent(in)    :: n     !! Number of particles to allocate space for
+      class(collision_fragments), intent(inout) :: self  
+         !! Collision fragments
+      integer(I4B),               intent(in)    :: n     
+         !! Number of particles to allocate space for
       ! Internals
       integer(I4B) :: i
 
       if (n < 0) return
 
       self%nbody = n
       if (n == 0) return
@@ -492,17 +508,17 @@
       if (allocated(self%radius)) deallocate(self%radius); allocate(self%radius(n))
       if (allocated(self%density)) deallocate(self%density); allocate(self%density(n))
       if (allocated(self%rmag)) deallocate(self%rmag); allocate(self%rmag(n))
       if (allocated(self%vmag)) deallocate(self%vmag); allocate(self%vmag(n))
       if (allocated(self%rotmag)) deallocate(self%rotmag); allocate(self%rotmag(n))
       if (allocated(self%origin_body)) deallocate(self%origin_body); allocate(self%origin_body(n))
       if (allocated(self%L_orbit)) deallocate(self%L_orbit); allocate(self%L_orbit(NDIM, n))
-      if (allocated(self%L_spin)) deallocate(self%L_spin); allocate(self%L_spin(NDIM, n))
+      if (allocated(self%L_rot)) deallocate(self%L_rot); allocate(self%L_rot(NDIM, n))
       if (allocated(self%ke_orbit)) deallocate(self%ke_orbit); allocate(self%ke_orbit(n))
-      if (allocated(self%ke_spin)) deallocate(self%ke_spin); allocate(self%ke_spin(n))
+      if (allocated(self%ke_rot)) deallocate(self%ke_rot); allocate(self%ke_rot(n))
 
       self%id(:) = 0
       select type(info => self%info)
       class is (swiftest_particle_info)
          do i = 1, n
             call info(i)%set_value(&
                name = "UNNAMED", &
@@ -540,37 +556,38 @@
       self%radius(:)   = 0.0_DP
       self%density(:)   = 0.0_DP
       self%rmag(:)   = 0.0_DP
       self%vmag(:)   = 0.0_DP
       self%rotmag(:)   = 0.0_DP
       self%origin_body(:)   = 0
       self%L_orbit_tot(:)   = 0.0_DP
-      self%L_spin_tot(:)   = 0.0_DP
+      self%L_rot_tot(:)   = 0.0_DP
       self%L_orbit(:,:)   = 0.0_DP
-      self%L_spin(:,:)   = 0.0_DP
+      self%L_rot(:,:)   = 0.0_DP
       self%ke_orbit_tot = 0.0_DP
-      self%ke_spin_tot = 0.0_DP
+      self%ke_rot_tot = 0.0_DP
       self%pe = 0.0_DP
       self%be = 0.0_DP
       self%ke_orbit(:)   = 0.0_DP
-      self%ke_spin(:)   = 0.0_DP
+      self%ke_rot(:)   = 0.0_DP
 
       return
    end subroutine collision_util_setup_fragments
 
 
    module subroutine collision_util_set_coordinate_collider(self)
       !! author: David A. Minton
       !! 
       !!
       !! Defines the collisional coordinate nbody_system, including the unit vectors of both the nbody_system and individual 
       !! fragments.
       implicit none
       ! Arguments
-      class(collision_basic),    intent(inout) :: self      !! Collisional nbody_system
+      class(collision_basic),    intent(inout) :: self      
+         !! Collisional system
 
       associate(fragments => self%fragments, impactors => self%impactors)
          call impactors%set_coordinate_system() 
 
          if (.not.allocated(self%fragments)) return
          call fragments%set_coordinate_system()
 
@@ -584,15 +601,16 @@
    module subroutine collision_util_set_coordinate_fragments(self)
       !! author: David A. Minton
       !!
       !! Defines the collisional coordinate nbody_system, including the unit vectors of both the nbody_system and individual 
       !! fragments.
       implicit none
       ! Arguments
-      class(collision_fragments), intent(inout) :: self      !! Collisional nbody_system
+      class(collision_fragments), intent(inout) :: self      
+         !! Collisional fragments object
 
       associate(fragments => self, nfrag => self%nbody)
          if ((nfrag == 0) .or. (.not.any(fragments%rc(:,:) > 0.0_DP))) return
 
          fragments%rmag(:) = .mag. fragments%rc(:,:)
          fragments%vmag(:) = .mag. fragments%vc(:,:)
          fragments%rotmag(:) = .mag. fragments%rot(:,:)
@@ -611,29 +629,30 @@
    module subroutine collision_util_set_coordinate_impactors(self)
       !! author: David A. Minton
       !!
       !! Defines the collisional coordinate nbody_system, including the unit vectors of both the nbody_system and individual 
       !! fragments.
       implicit none
       ! Arguments
-      class(collision_impactors), intent(inout) :: self      !! Collisional nbody_system
+      class(collision_impactors), intent(inout) :: self      
+         !! Collisional impactors object
       ! Internals
       real(DP), dimension(NDIM) ::  delta_r, delta_v, L_total
       real(DP)   ::  L_mag, mtot
 
       associate(impactors => self)
          delta_v(:) = impactors%vb(:, 2) - impactors%vb(:, 1)
          delta_r(:) = impactors%rb(:, 2) - impactors%rb(:, 1)
    
          ! We will initialize fragments on a plane defined by the pre-impact nbody_system, with the z-axis aligned with the angular 
          ! momentum vector and the y-axis aligned with the pre-impact distance vector.
 
          ! y-axis is the separation distance
          impactors%y_unit(:) = .unit.delta_r(:) 
-         L_total = impactors%L_orbit(:,1) + impactors%L_orbit(:,2) + impactors%L_spin(:,1) + impactors%L_spin(:,2)
+         L_total = impactors%L_orbit(:,1) + impactors%L_orbit(:,2) + impactors%L_rot(:,1) + impactors%L_rot(:,2)
 
          L_mag = .mag.L_total(:)
          if (L_mag > sqrt(tiny(L_mag))) then
             impactors%z_unit(:) = .unit.L_total(:) 
          else ! Not enough angular momentum to determine a z-axis direction. We'll just pick a random direction
             call random_number(impactors%z_unit(:))
             impactors%z_unit(:) = .unit.impactors%z_unit(:) 
@@ -675,17 +694,20 @@
    module subroutine collision_util_setup_collider(self, nbody_system, param)
       !! author: David A. Minton
       !!
       !! Initializer for the encounter collision system. Sets up impactors and the before/after snapshots,
       !! but not fragments. Those are setup later when the number of fragments is known.
       implicit none
       ! Arguments
-      class(collision_basic),   intent(inout) :: self         !! Encounter collision system object
-      class(base_nbody_system), intent(in)    :: nbody_system !! Current nbody system. Used as a mold for the before/after snapshots
-      class(base_parameters),   intent(inout) :: param        !! Current Swiftest run configuration parameters
+      class(collision_basic),   intent(inout) :: self         
+         !! Collision system object
+      class(base_nbody_system), intent(in)    :: nbody_system 
+         !! Current nbody system. Used as a mold for the before/after snapshots
+      class(base_parameters),   intent(inout) :: param        
+         !! Current Swiftest run configuration parameters
 
       call self%setup_impactors()
       if (allocated(self%before)) deallocate(self%before)
       if (allocated(self%after)) deallocate(self%after)
 
       allocate(self%before, mold=nbody_system)
       allocate(self%after,  mold=nbody_system)
@@ -698,31 +720,34 @@
 
    module subroutine collision_util_setup_impactors_collider(self)
       !! author: David A. Minton
       !!
       !! Initializer for the impactors for the encounter collision system. Deallocates old impactors before creating new ones
       implicit none
       ! Arguments
-      class(collision_basic), intent(inout) :: self   !! Encounter collision system object
+      class(collision_basic), intent(inout) :: self   
+         !! Collision system object
 
       if (allocated(self%impactors)) deallocate(self%impactors)
       allocate(collision_impactors :: self%impactors)
 
       return
    end subroutine collision_util_setup_impactors_collider
 
 
    module subroutine collision_util_setup_fragments_collider(self, nfrag)
       !! author: David A. Minton
       !!
       !! Initializer for the fragments of the collision system. 
       implicit none
       ! Arguments
-      class(collision_basic), intent(inout) :: self  !! Encounter collision system object
-      integer(I4B),            intent(in)    :: nfrag !! Number of fragments to create
+      class(collision_basic), intent(inout) :: self 
+          !! collision system object
+      integer(I4B),            intent(in)    :: nfrag 
+         !! Number of fragments to create
 
       if (allocated(self%fragments)) deallocate(self%fragments)
       allocate(collision_fragments :: self%fragments)
       call self%fragments%setup(nfrag)
 
       return
    end subroutine collision_util_setup_fragments_collider
@@ -730,16 +755,18 @@
 
    module subroutine collision_util_shift_vector_to_origin(m_frag, vec_frag)
       !! Author: Jennifer L.L. Pouplin, Carlisle A. Wishard, and David A. Minton
       !!
       !! Adjusts the position or velocity of the fragments as needed to align them with the center of mass origin
       implicit none
       ! Arguments
-      real(DP), dimension(:),   intent(in)    :: m_frag    !! Fragment masses
-      real(DP), dimension(:,:), intent(inout) :: vec_frag  !! Fragment positions or velocities in the center of mass frame
+      real(DP), dimension(:),   intent(in)    :: m_frag    
+         !! Fragment masses
+      real(DP), dimension(:,:), intent(inout) :: vec_frag  
+         !! Fragment positions or velocities in the center of mass frame
 
       ! Internals
       real(DP), dimension(NDIM) :: mvec_frag, COM_offset
       integer(I4B) :: i, nfrag
       real(DP) :: mtot
 
       mvec_frag(:) = 0.0_DP
@@ -754,135 +781,235 @@
          vec_frag(:, i) = vec_frag(:, i) + COM_offset(:)
       end do
 
       return
    end subroutine collision_util_shift_vector_to_origin
 
 
-   module subroutine collision_util_snapshot(self, param, nbody_system, t, arg)
+   module subroutine collision_util_take_snapshot(self, param, nbody_system, t, arg)
       !! author: David A. Minton
       !!
       !! Takes a minimal snapshot of the state of the nbody_system during a collision to record the before and after states of the
       !! system through the collision.
       implicit none
       ! Internals
-      class(collision_storage), intent(inout)          :: self   !! Swiftest storage object
-      class(base_parameters),   intent(inout)          :: param  !! Current run configuration parameters
-      class(base_nbody_system), intent(inout)          :: nbody_system !! Swiftest nbody system object to store
-      real(DP),                 intent(in),   optional :: t      !! Time of snapshot if different from nbody_system time
-      character(*),             intent(in),   optional :: arg    !! "before": takes a snapshot just before the collision. "after" 
-                                                                 !!    takes the snapshot just after the collision.
+      class(collision_storage), intent(inout)          :: self   
+         !! Collision storage object
+      class(base_parameters),   intent(inout)          :: param  
+         !! Current run configuration parameters
+      class(base_nbody_system), intent(inout)          :: nbody_system 
+         !! Swiftest nbody system object to store
+      real(DP),                 intent(in),   optional :: t      
+         !! Time of snapshot if different from nbody_system time
+      character(*),             intent(in),   optional :: arg    
+         !! "before": takes a snapshot just before the collision. 
+         !! "after" : takes the snapshot just after the collision.
       ! Arguments
       class(collision_snapshot), allocatable, save :: snapshot
       character(len=:), allocatable :: stage
       integer(I4B) :: i,phase_val
-      character(len=STRMAX) :: message
+      character(len=STRMAX) :: message, idstr
 
       if (present(arg)) then
          stage = arg
       else
          stage = ""
       end if 
 
       select type (nbody_system)
       class is (swiftest_nbody_system)
       select type(param)
       class is (swiftest_parameters)
+         if (stage /= "after") then
+            ! Advance the collision id number and save it
+            associate(collider => nbody_system%collider)
+               collider%maxid_collision = max(collider%maxid_collision, maxval(nbody_system%pl%info(:)%collision_id))
+               collider%maxid_collision = collider%maxid_collision + 1
+               collider%collision_id = collider%maxid_collision
+               write(idstr,*) collider%collision_id
+               call swiftest_io_log_one_message(COLLISION_LOG_OUT, "collision_id " // trim(adjustl(idstr)))
+            end associate
+         end if
 
          select case (stage)
          case ("before")
             phase_val = 1
+
             allocate(collision_snapshot :: snapshot)
             allocate(snapshot%collider, source=nbody_system%collider) 
             snapshot%t = t
+
          case ("after")
             phase_val = 2
          case ("particle")
             phase_val = -1
             allocate(collision_snapshot :: snapshot)
             allocate(snapshot%collider, source=nbody_system%collider) 
          case default
-            write(*,*) "collision_util_snapshot requies either 'before', 'after', or 'particle' passed to 'arg'"
+            write(*,*) "collision_util_take_snapshot requies either 'before', 'after', or 'particle' passed to 'arg'"
             return
          end select
 
          if (stage /= "particle" ) then
-            ! Get and record the energy of the system before the collision
-            call nbody_system%get_energy_and_momentum(param)
-            snapshot%collider%L_orbit(:,phase_val) = nbody_system%L_orbit(:)
-            snapshot%collider%L_spin(:,phase_val) = nbody_system%L_spin(:)
-            snapshot%collider%L_total(:,phase_val) = nbody_system%L_total(:)
-            snapshot%collider%ke_orbit(phase_val) = nbody_system%ke_orbit
-            snapshot%collider%ke_spin(phase_val) = nbody_system%ke_spin
-            snapshot%collider%pe(phase_val) = nbody_system%pe
-            snapshot%collider%be(phase_val) = nbody_system%be
-            snapshot%collider%te(phase_val) = nbody_system%te
-
             if (stage == "after") then
                select type(before_snap => snapshot%collider%before )
                class is (swiftest_nbody_system)
                select type(before_orig => nbody_system%collider%before)
-                  class is (swiftest_nbody_system)
-                  select type(plsub => before_orig%pl)
-                  class is (swiftest_pl)
-                     ! Log the properties of the old and new bodies
-                     call swiftest_io_log_one_message(COLLISION_LOG_OUT, "Removing bodies:")
-                     do i = 1, plsub%nbody
-                        write(message,*) trim(adjustl(plsub%info(i)%name)), " (", trim(adjustl(plsub%info(i)%particle_type)),")"
-                        call swiftest_io_log_one_message(COLLISION_LOG_OUT, message)
-                     end do
-
-                     allocate(before_snap%pl, source=plsub)
-                  end select
-                  deallocate(before_orig%pl)
+               class is (swiftest_nbody_system)
+                  if (allocated(before_orig%pl)) then
+                     select type(plsub => before_orig%pl)
+                     class is (swiftest_pl)
+                        ! Log the properties of the old and new bodies
+                        call swiftest_io_log_one_message(COLLISION_LOG_OUT, "Removing bodies:")
+                        do i = 1, plsub%nbody
+                           write(message,*) trim(adjustl(plsub%info(i)%name)), " (", trim(adjustl(plsub%info(i)%particle_type)),")"
+                           call swiftest_io_log_one_message(COLLISION_LOG_OUT, message)
+                        end do
+                        if (allocated(before_snap%pl)) deallocate(before_snap%pl)
+                        allocate(before_snap%pl, source=plsub)
+                     end select
+                     deallocate(before_orig%pl)
+                  end if
+
+                  if (allocated(before_orig%tp)) then   
+                     select type(tpsub => before_orig%tp)
+                     class is (swiftest_tp)
+                        ! Log the properties of the old and new bodies
+                        call swiftest_io_log_one_message(COLLISION_LOG_OUT, "Removing bodies:")
+                        do i = 1, tpsub%nbody
+                           write(message,*) trim(adjustl(tpsub%info(i)%name)), " (", trim(adjustl(tpsub%info(i)%particle_type)),")"
+                           call swiftest_io_log_one_message(COLLISION_LOG_OUT, message)
+                        end do
+                        if (allocated(before_snap%tp)) deallocate(before_snap%tp)
+                        allocate(before_snap%tp, source=tpsub)
+                     end select
+                     deallocate(before_orig%tp)
+                  end if
+
+                  if (allocated(before_orig%cb)) then
+                     select type(cbsub => before_orig%cb)
+                     class is (swiftest_cb)
+                        call swiftest_io_log_one_message(COLLISION_LOG_OUT, "Collision with the central body")
+                        call swiftest_io_log_one_message(COLLISION_LOG_OUT, & 
+                           "***********************************************************" // &
+                           "***********************************************************")
+                        if (allocated(before_snap%cb)) deallocate(before_snap%cb)
+                        allocate(before_snap%cb, source=cbsub)
+                     end select
+                     deallocate(before_orig%cb)
+                  end if
+
                end select
                end select
 
                select type(after_snap => snapshot%collider%after )
                class is (swiftest_nbody_system)
                select type(after_orig => nbody_system%collider%after)
                class is (swiftest_nbody_system)
-                  select type(plnew => after_orig%pl)
-                  class is (swiftest_pl)
-                     call swiftest_io_log_one_message(COLLISION_LOG_OUT, "Adding bodies:")
-                     do i = 1, plnew%nbody
-                        write(message,*) trim(adjustl(plnew%info(i)%name)), " (", trim(adjustl(plnew%info(i)%particle_type)),")"
-                        call swiftest_io_log_one_message(COLLISION_LOG_OUT, message)
-                     end do
-                     call swiftest_io_log_one_message(COLLISION_LOG_OUT, & 
-                        "***********************************************************" // &
-                        "***********************************************************")
-                     allocate(after_snap%pl, source=plnew)
-                  end select
-                  deallocate(after_orig%pl)
+                  if (allocated(after_orig%pl)) then
+                     select type(plnew => after_orig%pl)
+                     class is (swiftest_pl)
+                        call swiftest_io_log_one_message(COLLISION_LOG_OUT, "Adding bodies:")
+                        do i = 1, plnew%nbody
+                           write(message,*) trim(adjustl(plnew%info(i)%name)), " (", trim(adjustl(plnew%info(i)%particle_type)),")"
+                           call swiftest_io_log_one_message(COLLISION_LOG_OUT, message)
+                        end do
+                        call swiftest_io_log_one_message(COLLISION_LOG_OUT, & 
+                           "***********************************************************" // &
+                           "***********************************************************")
+                        allocate(after_snap%pl, source=plnew)
+                     end select
+                     deallocate(after_orig%pl)
+                  end if
+                  if (allocated(after_orig%cb)) then
+                     select type(cbnew => after_orig%cb)
+                     class is (swiftest_cb)
+                        allocate(after_snap%cb, source=cbnew)
+                     end select
+                     deallocate(after_orig%cb)
+                  end if
                end select
                end select
             end if
          end if
 
          if ((stage == "after") .or. (stage == "particle")) then
             ! Save the snapshot for posterity
             call self%save(snapshot)
             deallocate(snapshot)
          end if
       end select
       end select
 
       return
-   end subroutine collision_util_snapshot
+   end subroutine collision_util_take_snapshot
+
+
+   module subroutine collision_util_save_energy_snapshot(self, stage, nbody_system, iframe_start, iframe_end)
+      !! author: David A. Minton
+      !!
+      !! Retroactively save the energy of the system before and after a collision to an existing snapshot 
+      implicit none
+      ! Arguments
+      class(collision_storage), intent(inout) :: self  
+         !! Collision storage object with snapshots
+      character(len=*), intent(in) :: stage
+         !! Phase of the collision, either 'before' or 'after'
+      class(base_nbody_system), intent(inout) :: nbody_system
+         !! Swiftest nbody system object with energy information stored in it
+      integer(I4B), intent(in) :: iframe_start 
+         !! Starting frame index to save the snapshot
+      integer(I4B), intent(in) :: iframe_end   
+         !! Ending frame index to save the snapshot
+      ! Internals
+      integer(I4B) :: i, phase_val
+
+      ! Save the energy in the before snapshots
+      select case (stage)
+      case ("before")
+         phase_val = 1
+      case ("after")
+         phase_val = 2
+      case default
+         write(*,*) "collision_util_take_snapshot requies either 'before' or 'after'"
+         return
+      end select
+
+      select type(nbody_system)
+      class is (swiftest_nbody_system)
+
+         do i = iframe_start, iframe_end
+            if (allocated(self%frame(i)%item)) then
+               select type(snapshot => self%frame(i)%item)
+               class is (collision_snapshot)
+                  snapshot%collider%L_orbit(:,phase_val) = nbody_system%L_orbit(:)
+                  snapshot%collider%L_rot(:,phase_val) = nbody_system%L_rot(:)
+                  snapshot%collider%L_total(:,phase_val) = nbody_system%L_total(:)
+                  snapshot%collider%ke_orbit(phase_val) = nbody_system%ke_orbit
+                  snapshot%collider%ke_rot(phase_val) = nbody_system%ke_rot
+                  snapshot%collider%pe(phase_val) = nbody_system%pe
+                  snapshot%collider%be(phase_val) = nbody_system%be
+                  snapshot%collider%te(phase_val) = nbody_system%te
+               end select
+            end if
+         end do
+      end select
+
+   end subroutine collision_util_save_energy_snapshot
 
 
    module subroutine collision_util_set_natural_scale_factors(self)
       !! author: David A. Minton
       !!
       !! Scales dimenional quantities to ~O(1) with respect to the collisional system. 
       !! This scaling makes it it easier to converge on a solution without having floating point issues
       implicit none
       ! Arguments
-      class(collision_basic), intent(inout) :: self  !! Collision system object
+      class(collision_basic), intent(inout) :: self  
+         !! Collision system object
       ! Internals
       integer(I4B) :: i
       real(DP) :: vesc
 
       associate(collider => self, fragments => self%fragments, impactors => self%impactors)
          ! Set primary scale factors (mass, length, and time) based on the impactor properties at the time of collision
          collider%mscale = minval(impactors%mass(:))
@@ -904,21 +1031,21 @@
          impactors%vb(:,:)      = impactors%vb(:,:)       / collider%vscale
          impactors%rc(:,:)      = impactors%rc(:,:)       / collider%dscale
          impactors%vc(:,:)      = impactors%vc(:,:)       / collider%vscale
          impactors%mass(:)      = impactors%mass(:)       / collider%mscale
          impactors%Gmass(:)     = impactors%Gmass(:)      / (collider%dscale**3/collider%tscale**2)
          impactors%Mcb          = impactors%Mcb           / collider%mscale
          impactors%radius(:)    = impactors%radius(:)     / collider%dscale
-         impactors%L_spin(:,:)  = impactors%L_spin(:,:)   / collider%Lscale
+         impactors%L_rot(:,:)  = impactors%L_rot(:,:)   / collider%Lscale
          impactors%L_orbit(:,:) = impactors%L_orbit(:,:)  / collider%Lscale
          impactors%ke_orbit(:)  = impactors%ke_orbit(:)   / collider%Escale
-         impactors%ke_spin(:)   = impactors%ke_spin(:)    / collider%Escale
+         impactors%ke_rot(:)   = impactors%ke_rot(:)    / collider%Escale
 
          do concurrent(i = 1:2)
-            impactors%rot(:,i) = impactors%L_spin(:,i) / (impactors%mass(i) * impactors%radius(i)**2 * impactors%Ip(3,i))
+            impactors%rot(:,i) = impactors%L_rot(:,i) / (impactors%mass(i) * impactors%radius(i)**2 * impactors%Ip(3,i))
          end do
 
          fragments%mtot      = fragments%mtot      / collider%mscale
          fragments%mass(:)   = fragments%mass(:)   / collider%mscale
          fragments%Gmass(:)  = fragments%Gmass(:)  / (collider%dscale**3/collider%tscale**2)
          fragments%radius(:) = fragments%radius(:) / collider%dscale
          impactors%Qloss     = impactors%Qloss     / collider%Escale
@@ -934,15 +1061,16 @@
    module subroutine collision_util_set_original_scale_factors(self)
       !! author: David A. Minton
       !!
       !! Restores dimenional quantities back to the system units
       use, intrinsic :: ieee_exceptions
       implicit none
       ! Arguments
-      class(collision_basic),      intent(inout) :: self      !! Fragment system object
+      class(collision_basic),      intent(inout) :: self      
+         !! Collision system object
       ! Internals
       integer(I4B) :: i
       logical, dimension(size(IEEE_ALL))      :: fpe_halting_modes
 
       call ieee_get_halting_mode(IEEE_ALL,fpe_halting_modes)  ! Save the current halting modes so we can turn them off temporarily
       call ieee_set_halting_mode(IEEE_ALL,.false.)
 
@@ -958,24 +1086,24 @@
          impactors%Mcb       = impactors%Mcb       * collider%mscale
          impactors%mass_dist = impactors%mass_dist * collider%mscale
          impactors%radius    = impactors%radius    * collider%dscale
          impactors%rb        = impactors%rb        * collider%dscale
          impactors%vb        = impactors%vb        * collider%vscale
          impactors%rc        = impactors%rc        * collider%dscale
          impactors%vc        = impactors%vc        * collider%vscale
-         impactors%L_spin    = impactors%L_spin    * collider%Lscale
+         impactors%L_rot    = impactors%L_rot    * collider%Lscale
          impactors%L_orbit   = impactors%L_orbit   * collider%Lscale
          impactors%ke_orbit  = impactors%ke_orbit  * collider%Escale
-         impactors%ke_spin   = impactors%ke_spin   * collider%Escale
+         impactors%ke_rot   = impactors%ke_rot   * collider%Escale
 #ifdef DOCONLOC
          do concurrent(i = 1:2) shared(impactors)
 #else
          do concurrent(i = 1:2)
 #endif
-            impactors%rot(:,i) = impactors%L_spin(:,i) * (impactors%mass(i) * impactors%radius(i)**2 * impactors%Ip(3,i))
+            impactors%rot(:,i) = impactors%L_rot(:,i) * (impactors%mass(i) * impactors%radius(i)**2 * impactors%Ip(3,i))
          end do
    
          fragments%mtot      = fragments%mtot      * collider%mscale
          fragments%mass(:)   = fragments%mass(:)   * collider%mscale
          fragments%Gmass(:)  = fragments%Gmass(:)  * (collider%dscale**3/collider%tscale**2)
          fragments%radius(:) = fragments%radius(:) * collider%dscale
          fragments%rot(:,:)  = fragments%rot(:,:)  / collider%tscale
@@ -983,18 +1111,18 @@
          fragments%vc(:,:)   = fragments%vc(:,:)   * collider%vscale
          fragments%rb(:,:)   = fragments%rb(:,:)   * collider%dscale
          fragments%vb(:,:)   = fragments%vb(:,:)   * collider%vscale
 
          impactors%Qloss = impactors%Qloss * collider%Escale
 
          collider%L_orbit(:,:) = collider%L_orbit(:,:) * collider%Lscale
-         collider%L_spin(:,:)  = collider%L_spin(:,:)  * collider%Lscale
+         collider%L_rot(:,:)  = collider%L_rot(:,:)  * collider%Lscale
          collider%L_total(:,:) = collider%L_total(:,:) * collider%Lscale
          collider%ke_orbit(:)  = collider%ke_orbit(:)  * collider%Escale
-         collider%ke_spin(:)   = collider%ke_spin(:)   * collider%Escale
+         collider%ke_rot(:)   = collider%ke_rot(:)   * collider%Escale
          collider%pe(:)        = collider%pe(:)        * collider%Escale
          collider%be(:)        = collider%be(:)        * collider%Escale
          collider%te(:)        = collider%te(:)        * collider%Escale
          collider%min_mfrag    = collider%min_mfrag    * collider%mscale
          collider%max_rot      = collider%max_rot      / collider%tscale
    
          collider%mscale = 1.0_DP
@@ -1012,18 +1140,22 @@
 
    module subroutine collision_util_velocity_torque(dL, mass, r, v)
       !! author: David A. Minton
       !!
       !! Applies a torque to a body's center of mass velocity given a change in angular momentum
       implicit none
       ! Arguments
-      real(DP), dimension(:), intent(in)    :: dL   !! Change in angular momentum to apply
-      real(DP),               intent(in)    :: mass !! Mass of body
-      real(DP), dimension(:), intent(in)    :: r    !! Position of body wrt system center of mass
-      real(DP), dimension(:), intent(inout) :: v !! Velocity of body wrt system center of mass
+      real(DP), dimension(:), intent(in)    :: dL   
+         !! Change in angular momentum to apply
+      real(DP),               intent(in)    :: mass 
+         !! Mass of body
+      real(DP), dimension(:), intent(in)    :: r 
+         !! Position of body wrt system center of mass
+      real(DP), dimension(:), intent(inout) :: v 
+         !! Velocity of body wrt system center of mass
       ! Internals
       real(DP), dimension(NDIM) :: dL_unit, r_unit, vapply
       real(DP) :: rmag, vmag, vapply_mag
 
       dL_unit(:) = .unit. dL
       r_unit(:) = .unit.r(:)
       rmag = .mag.r(:)
```

### Comparing `swiftest-2024.4.1/src/encounter/encounter_check.f90` & `swiftest-2024.4.2/src/encounter/encounter_check.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/encounter/encounter_io.f90` & `swiftest-2024.4.2/src/encounter/encounter_io.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/encounter/encounter_module.f90` & `swiftest-2024.4.2/src/encounter/encounter_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/encounter/encounter_util.f90` & `swiftest-2024.4.2/src/encounter/encounter_util.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/fraggle/fraggle_generate.f90` & `swiftest-2024.4.2/src/fraggle/fraggle_generate.f90`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,21 @@
       !! author: Jennifer L.L. Pouplin, Carlisle A. Wishard, and David A. Minton
       !!
       !! Create the fragments resulting from a non-catastrophic disruption collision
       !! 
       implicit none
       ! Arguments
       class(collision_fraggle), intent(inout) :: self
-      class(base_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(base_parameters),   intent(inout) :: param        !! Current run configuration parameters 
-      real(DP),                 intent(in)    :: t            !! Time of collision
+         !! Fraggle collisional system object
+      class(base_nbody_system), intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(base_parameters),   intent(inout) :: param        
+         !! Current run configuration parameters 
+      real(DP),                 intent(in)    :: t            
+         !! Time of collision
       ! Internals
       integer(I4B)          :: i, ibiggest
       real(DP), dimension(NDIM) :: L_residual, vbcom_orig
       character(len=STRMAX) :: message 
       logical               :: lfailure
 
       select type(nbody_system)
@@ -56,15 +60,15 @@
             end select
             call collision_io_collider_message(pl, impactors%id, message)
             call swiftest_io_log_one_message(COLLISION_LOG_OUT, trim(adjustl(message)))
             call self%set_mass_dist(param) 
             call self%disrupt(nbody_system, param, t, lfailure)
             if (lfailure) then
                call swiftest_io_log_one_message(COLLISION_LOG_OUT, & 
-                                           "Fraggle failed to find a solution to match energy contraint. Treating this as a merge.") 
+                                           "Fraggle failed to find a solution to match energy contraint. Treating this as a merge.")
                call self%merge(nbody_system, param, t) ! Use the default collision model, which is merge
                return
             end if
 
             associate (fragments => self%fragments)
                ! Get the energy and momentum of the system before and after the collision
                call self%get_energy_and_momentum(nbody_system, param, phase="before")
@@ -114,19 +118,24 @@
    module subroutine fraggle_generate_disrupt(self, nbody_system, param, t, lfailure)
       !! Author: Jennifer L.L. Pouplin, Carlisle A. Wishard, and David A. Minton
       !!
       !! Generates a nbody_system of fragments in barycentric coordinates that conserves energy and momentum.
       use, intrinsic :: ieee_exceptions
       implicit none
       ! Arguments
-      class(collision_fraggle), intent(inout) :: self         !! Fraggle system object the outputs will be the fragmentation 
-      class(base_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(base_parameters),   intent(inout) :: param        !! Current run configuration parameters 
-      real(DP),                 intent(in)    :: t            !! Time of collision 
-      logical,                  intent(out)   :: lfailure     !! Answers the question: Should this have been a merger instead?
+      class(collision_fraggle), intent(inout) :: self         
+         !! Fraggle system object the outputs will be the fragmentation 
+      class(base_nbody_system), intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(base_parameters),   intent(inout) :: param        
+         !! Current run configuration parameters 
+      real(DP),                 intent(in)    :: t            
+         !! Time of collision 
+      logical,                  intent(out)   :: lfailure     
+         !! Answers the question: Should this have been a merger instead?
        ! Internals
       logical                              :: lk_plpl
       logical, dimension(size(IEEE_ALL))   :: fpe_halting_modes, fpe_quiet_modes
       real(DP)                             :: dE
       real(DP), dimension(NDIM)            :: dL
       character(len=STRMAX)                :: message
       real(DP), parameter                  :: fail_scale_initial = 1.0003_DP
@@ -200,16 +209,16 @@
             write(message,*) "Actual  :    dE = ",dE
             call swiftest_io_log_one_message(COLLISION_LOG_OUT, message)
             write(message,*) "Actual  :    dL = ",dL
             call swiftest_io_log_one_message(COLLISION_LOG_OUT, message)
 
          end if
          call self%set_original_scale()
-         self%max_rot = MAX_ROT_SI * param%TU2S ! Re-compute the spin limit from scratch so it doesn't drift due to floating point 
-                                                ! errors every time we convert
+         self%max_rot = MAX_ROT_SI * param%TU2S ! Re-compute the rotation limit from scratch so it doesn't drift due to floating 
+                                                ! point errors every time we convert
 
          ! Restore the big array
          if (lk_plpl) call pl%flatten(param)
       end associate
       end select
       end select
       call ieee_set_halting_mode(IEEE_ALL,fpe_halting_modes)  ! Restore the original halting modes
@@ -218,23 +227,27 @@
    end subroutine fraggle_generate_disrupt
 
 
    module subroutine fraggle_generate_hitandrun(self, nbody_system, param, t) 
       !! author: Jennifer L.L. Pouplin, Carlisle A. Wishard, and David A. Minton
       !!
       !! Create the fragments resulting from a non-catastrophic hit-and-run collision
-      !! 
       implicit none
       ! Arguments
-      class(collision_fraggle), intent(inout) :: self         !! Collision system object
-      class(base_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(base_parameters),   intent(inout) :: param        !! Current run configuration parameters 
-      real(DP),                 intent(in)    :: t            !! Time of collision
+      class(collision_fraggle), intent(inout) :: self         
+         !! Collision system object
+      class(base_nbody_system), intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(base_parameters),   intent(inout) :: param        
+         !! Current run configuration parameters 
+      real(DP),                 intent(in)    :: t            
+         !! Time of collision
       ! Result
-      integer(I4B)                            :: status       !! Status flag assigned to this outcome
+      integer(I4B)                            :: status       
+         !! Status flag assigned to this outcome
       ! Internals
       integer(I4B)                            :: i, ibiggest, jtarg, jproj
       logical                                 :: lpure 
       character(len=STRMAX) :: message
 
       select type(nbody_system)
       class is (swiftest_nbody_system)
@@ -299,46 +312,50 @@
       !!
       !! Merge massive bodies in any collisional system. If the rotation is too high, switch to hit and run.
       !! 
       !! Adapted from David E. Kaufmann's Swifter routines symba_merge_pl.f90 and symba_discard_merge_pl.f90
       !!
       !! Adapted from Hal Levison's Swift routines symba5_merge.f and discard_mass_merge.f
       implicit none
-      class(collision_fraggle), intent(inout) :: self         !! Fraggle system object
-      class(base_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(base_parameters),   intent(inout) :: param        !! Current run configuration parameters 
-      real(DP),                 intent(in)    :: t            !! The time of the collision
+      class(collision_fraggle), intent(inout) :: self         
+         !! Fraggle system object
+      class(base_nbody_system), intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(base_parameters),   intent(inout) :: param        
+         !! Current run configuration parameters 
+      real(DP),                 intent(in)    :: t            
+         !! The time of the collision
 
       ! Internals
       integer(I4B)                              :: i
-      real(DP), dimension(NDIM)                 :: L_spin_new, Ip, rot
+      real(DP), dimension(NDIM)                 :: L_rot_new, Ip, rot
       real(DP)                                  :: rotmag, mass, volume, radius
 
       select type(nbody_system)
       class is (swiftest_nbody_system)
          associate(impactors => self%impactors)
             mass = sum(impactors%mass(:))
             volume = 4._DP / 3._DP * PI * sum(impactors%radius(:)**3)
             radius = (3._DP * volume / (4._DP * PI))**(THIRD)
 #ifdef DOCONLOC
-            do concurrent(i = 1:NDIM) shared(impactors, Ip, L_spin_new)
+            do concurrent(i = 1:NDIM) shared(impactors, Ip, L_rot_new)
 #else
             do concurrent(i = 1:NDIM)
 #endif
                Ip(i) = sum(impactors%mass(:) * impactors%Ip(i,:)) 
-               L_spin_new(i) = sum(impactors%L_orbit(i,:) + impactors%L_spin(i,:))
+               L_rot_new(i) = sum(impactors%L_orbit(i,:) + impactors%L_rot(i,:))
             end do
             Ip(:) = Ip(:) / mass
-            rot(:) = L_spin_new(:) / (Ip(3) * mass * radius**2)
+            rot(:) = L_rot_new(:) / (Ip(3) * mass * radius**2)
             rotmag = .mag.rot(:)
             if (rotmag < self%max_rot) then
                call self%collision_basic%merge(nbody_system, param, t)
             else
                call swiftest_io_log_one_message(COLLISION_LOG_OUT, &
-                                                "Merger would break the spin barrier. Converting to pure hit and run" )
+                                                "Merger would break the rotation barrier. Converting to pure hit and run" )
                impactors%mass_dist(1:2) = impactors%mass(1:2)
                call self%hitandrun(nbody_system, param, t)
             end if
 
          end associate
       end select
       return 
@@ -350,18 +367,22 @@
       !!
       !! Initializes the position vectors of the fragments around the center of mass based on the collision style.
       !! For hit and run with disruption, the fragments are generated in a random cloud around the smallest of the two colliders 
       !! (body 2). For disruptive collisions, the fragments are generated in a random cloud around the impact point. Bodies are 
       !! checked for overlap and regenerated if they overlap.
       implicit none
       ! Arguments
-      class(collision_fraggle),     intent(inout) :: collider     !! Fraggle collision system object
-      class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(swiftest_parameters),   intent(inout) :: param        !! Current run configuration parameters 
-      logical,                      intent(out)   :: lfailure     !! Did the velocity computation fail?
+      class(collision_fraggle),     intent(inout) :: collider     
+         !! Fraggle collision system object
+      class(swiftest_nbody_system), intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(swiftest_parameters),   intent(inout) :: param        
+         !! Current run configuration parameters 
+      logical,                      intent(out)   :: lfailure     
+         !! Did the velocity computation fail?
       ! Internals
       real(DP)  :: dis, direction, rdistance
       real(DP), dimension(NDIM,2) :: fragment_cloud_center
       real(DP), dimension(NDIM) :: rwalk
       real(DP), dimension(2) :: fragment_cloud_radius
       logical, dimension(collider%fragments%nbody) :: loverlap
       real(DP), dimension(collider%fragments%nbody) :: mass_rscale, phi, theta, u
@@ -533,17 +554,20 @@
    module subroutine fraggle_generate_rot_vec(collider, nbody_system, param)
       !! Author: Jennifer L.L. Pouplin, Carlisle A. Wishard, and David A. Minton
       !!
       !! Computes an initial "guess" for the rotation states of fragments based on angular momentum and energy constraints.
       !! These will be adjusted later when the final fragment velocities are computed in fraggle_generate_vel_vec
       implicit none
       ! Arguments
-      class(collision_fraggle),     intent(inout) :: collider     !! Fraggle collision system object
-      class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(swiftest_parameters),   intent(inout) :: param        !! Current run configuration parameters 
+      class(collision_fraggle),     intent(inout) :: collider     
+         !! Fraggle collision system object
+      class(swiftest_nbody_system), intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(swiftest_parameters),   intent(inout) :: param        
+         !! Current run configuration parameters 
       ! Internals
       integer(I4B) :: i
       real(DP), parameter :: FRAG_ROT_FAC = 0.1_DP ! Fraction of projectile rotation magnitude to add as random noise to fragment 
                                                    ! rotation
       real(DP), parameter :: hitandrun_momentum_transfer = 0.01_DP ! Fraction of projectile momentum transfered to target in a hit  
                                                                    ! and run
       real(DP) :: mass_fac
@@ -556,20 +580,20 @@
          lhitandrun = (impactors%regime == COLLRESOLVE_REGIME_HIT_AND_RUN) 
 
          ! Initialize fragment rotations and velocities to be pre-impact rotation for body 1, and randomized for bodies >1 and 
          ! scaled to the original rotation.  This will get updated later when conserving angular momentum
          mass_fac = fragments%mass(1) / impactors%mass(1)
          fragments%rot(:,1) = mass_fac**(5.0_DP/3.0_DP) * impactors%rot(:,1)
 
-         ! If mass was added, also add spin angular momentum
+         ! If mass was added, also add rotational angular momentum
          if (mass_fac > 1.0_DP) then
             dL(:) = (fragments%mass(1) - impactors%mass(1)) * (impactors%rc(:,2) - impactors%rc(:,1)) &
                                                       .cross. (impactors%vc(:,2) - impactors%vc(:,1))
             drot(:) = dL(:) / (fragments%mass(1) * fragments%radius(1)**2 * fragments%Ip(3,1))
-            ! Check to make sure we haven't broken the spin barrier. Reduce the rotation change if so
+            ! Check to make sure we haven't broken the rotation barrier. Reduce the rotation change if so
             do i = 1, MAXLOOP
                if (.mag.(fragments%rot(:,1) + drot(:)) < collider%max_rot) exit
                if (i == MAXLOOP) drot(:) = 0.0_DP
                where(drot(:) > TINY(1.0_DP))
                   drot(:) = drot(:) / 2
                elsewhere
                   drot(:) = 0.0_DP
@@ -616,18 +640,22 @@
       !! Author:  David A. Minton
       !!
       !! Generates an initial velocity distribution. For disruptions, the velocity magnitude is set to be
       !! 2x the escape velocity of the colliding pair. For hit and runs the velocity magnitude is set to be
       !! 2x the escape velocity of the smallest of the two bodies.
       implicit none
       ! Arguments
-      class(collision_fraggle),     intent(inout) :: collider     !! Fraggle collision system object
-      class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(swiftest_parameters),   intent(inout) :: param        !! Current run configuration parameters 
-      logical,                      intent(out)   :: lfailure     !! Did the velocity computation fail?
+      class(collision_fraggle),     intent(inout) :: collider     
+         !! Fraggle collision system object
+      class(swiftest_nbody_system), intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(swiftest_parameters),   intent(inout) :: param        
+         !! Current run configuration parameters 
+      logical,                      intent(out)   :: lfailure     
+         !! Did the velocity computation fail?
       ! Internals
       real(DP), parameter :: ENERGY_SUCCESS_METRIC = 0.1_DP !! Relative energy error to accept as a success (success also must be 
                                                             !! energy-losing in addition to being within the metric amount)
       real(DP), parameter :: ENERGY_CONVERGENCE_TOL = 1e-3_DP !! Relative change in error before giving up on energy convergence
       real(DP)  :: MOMENTUM_SUCCESS_METRIC = 10*epsilon(1.0_DP) !! Relative angular momentum error to accept as a success 
                                                                 !! (should be *much* stricter than energy)
       integer(I4B) :: i, j, loop, try, istart, nfrag, nsteps, nsteps_best, posloop
@@ -747,23 +775,23 @@
                call fragments%set_coordinate_system()
 
                E_residual = huge(1.0_DP)
                inner: do loop = 1, MAXLOOP
                   nsteps = nsteps + 1
                   mfrag = sum(fragments%mass(istart:fragments%nbody))
 
-                  ! Try to put residual angular momentum into the spin, but if this would go past the spin barrier, then put it into
-                  ! velocity shear instead 
+                  ! Try to put residual angular momentum into the rotation, but if this would go past the rotation barrier, then put
+                  ! it into velocity shear instead 
                   call collider_local%get_energy_and_momentum(nbody_system, param, phase="after")
                   L_mag_factor = .mag.(collider_local%L_total(:,1) + collider_local%L_total(:,2))
                   L_residual(:) = (collider_local%L_total(:,2) / L_mag_factor - collider_local%L_total(:,1) / L_mag_factor)
                   L_residual_unit(:) = .unit. L_residual(:)
                   if (nsteps == 1) L_residual_best(:) = L_residual(:) * L_mag_factor
 
-                  ! Use equipartition of spin kinetic energy to distribution spin angular momentum
+                  ! Use equipartition of rotational kinetic energy to distribution rotational angular momentum
 #ifdef DOCONLOC
                   do concurrent(i = istart:fragments%nbody) shared(DLi_mag, fragments)
 #else
                   do concurrent(i = istart:fragments%nbody)
 #endif
                      dLi_mag(i) = ((fragments%mass(i) / fragments%mass(istart)) * &
                                    (fragments%radius(i) / fragments%radius(istart))**2 * &
@@ -774,16 +802,16 @@
                   do i = istart,fragments%nbody
                      dL(:) = -dL1_mag * dLi_mag(i) * L_residual_unit(:)
                      drot(:) = dL(:) / (fragments%mass(i) * fragments%Ip(3,i) * fragments%radius(i)**2)
                      rot_new(:) = fragments%rot(:,i) + drot(:)
                      if (.mag.rot_new(:) < collider_local%max_rot) then
                         fragments%rot(:,i) = rot_new(:)
                         fragments%rotmag(i) = .mag.fragments%rot(:,i)
-                     else ! We would break the spin barrier here. Add a random component of rotation that is less than what would 
-                          ! break the limit. The rest will go in velocity shear
+                     else ! We would break the rotation barrier here. Add a random component of rotation that is less than what 
+                          ! would break the limit. The rest will go in velocity shear
                         call random_number(drot)
                         call random_number(rn)
                         drot(:) = (rn * collider_local%max_rot - fragments%rotmag(i)) * 2 * (drot(:) - 0.5_DP)
                         fragments%rot(:,i) = fragments%rot(:,i) + drot(:)
                         fragments%rotmag(i) = .mag.fragments%rot(:,i)
                         if (fragments%rotmag(i) > collider%max_rot) then
                            fragments%rotmag(i) = 0.5_DP * collider%max_rot
@@ -879,15 +907,16 @@
          else 
             call swiftest_io_log_one_message(COLLISION_LOG_OUT,"Fraggle velocity calculation converged after " &
                                                               // trim(adjustl(message)) // " steps.")
 
             call collider%get_energy_and_momentum(nbody_system, param, phase="after")
             L_mag_factor = .mag.(collider%L_total(:,1) + collider%L_total(:,2))
             L_residual(:) = (collider%L_total(:,2) / L_mag_factor - collider%L_total(:,1)) / L_mag_factor
-            call collision_util_velocity_torque(-L_residual(:) * L_mag_factor, collider%fragments%mtot, impactors%rbcom, impactors%vbcom)
+            call collision_util_velocity_torque(-L_residual(:) * L_mag_factor, collider%fragments%mtot, &
+                                                impactors%rbcom, impactors%vbcom)
             nfrag = collider%fragments%nbody
 
 #ifdef DOCONLOC
             do concurrent(i = 1:nfrag) shared(collider, impactors)
 #else
             do concurrent(i = 1:nfrag)
 #endif
```

### Comparing `swiftest-2024.4.1/src/fraggle/fraggle_module.f90` & `swiftest-2024.4.2/src/fraggle/fraggle_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/fraggle/fraggle_util.f90` & `swiftest-2024.4.2/src/fraggle/fraggle_util.f90`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,22 @@
 
    module subroutine fraggle_util_restructure(self, nbody_system, param, lfailure)
       !! author: David A. Minton
       !!
       !! Restructures the fragment distribution after a failure to converge on a solution.
       implicit none
       ! Arguments
-      class(collision_fraggle),     intent(inout) :: self         !! Fraggle collision system object
-      class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(swiftest_parameters),   intent(inout) :: param        !! Current run configuration parameters 
-      logical,                      intent(out)   :: lfailure     !! Did the computation fail?
+      class(collision_fraggle),     intent(inout) :: self         
+         !! Fraggle collision system object
+      class(swiftest_nbody_system), intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(swiftest_parameters),   intent(inout) :: param        
+         !! Current run configuration parameters 
+      logical,                      intent(out)   :: lfailure     
+         !! Did the computation fail?
       ! Internals
       class(collision_fragments), allocatable :: new_fragments
       integer(I4B) :: i,nnew, nold
       real(DP) :: volume
 
       associate(old_fragments => self%fragments)
          lfailure = .false.
@@ -84,30 +88,31 @@
    end subroutine fraggle_util_restructure
 
    module subroutine fraggle_util_set_mass_dist(self, param)
       !! author: David A. Minton
       !!
       !! Sets the mass of fragments based on the mass distribution returned by the regime calculation.
       !! This subroutine must be run after the the setup routine has been run on the fragments
-      !!
       use, intrinsic :: ieee_exceptions
       implicit none
       ! Arguments
-      class(collision_fraggle),   intent(inout) :: self  !! Fraggle collision system object
-      class(swiftest_parameters), intent(in)    :: param !! Current Swiftest run configuration parameters
+      class(collision_fraggle),   intent(inout) :: self  
+         !! Fraggle collision system object
+      class(swiftest_parameters), intent(in)    :: param 
+         !! Current Swiftest run configuration parameters
       ! Internals
       integer(I4B)              :: i, j, jproj, jtarg, istart, nfragmax
       real(DP), dimension(2)    :: volume
       real(DP), dimension(NDIM) :: Ip_avg
       real(DP) ::  mremaining, mtot, mcumul, G, mass_noise
       real(DP), dimension(:), allocatable :: mass
       real(DP)  :: beta 
-      integer(I4B), parameter :: MASS_NOISE_FACTOR = 5  !! The number of digits of random noise that get added to the minimum mass value to prevent identical masses from being generated in a single run 
-      integer(I4B), parameter :: NFRAGMAX_UNSCALED = 100  !! Maximum number of fragments that can be generated
- !! Minimum number of fragments that can be generated 
+      integer(I4B), parameter :: MASS_NOISE_FACTOR = 5  ! The number of digits of random noise that get added to the minimum mass 
+                                                        ! value to prevent identical masses from being generated in a single run 
+      integer(I4B), parameter :: NFRAGMAX_UNSCALED = 100  ! Maximum number of fragments that can be generated
       integer(I4B), dimension(:), allocatable :: ind
       logical :: flipper
       logical, dimension(size(IEEE_ALL))      :: fpe_halting_modes
 
       call ieee_get_halting_mode(IEEE_ALL,fpe_halting_modes)  ! Save the current halting modes so we can turn them off temporarily
       call ieee_set_halting_mode(IEEE_ALL,.false.)
      
@@ -127,15 +132,16 @@
          end if
 
          select case(impactors%regime)
          case(COLLRESOLVE_REGIME_DISRUPTION, COLLRESOLVE_REGIME_SUPERCATASTROPHIC, COLLRESOLVE_REGIME_HIT_AND_RUN)
             ! The first two bins of the mass_dist are the largest and second-largest fragments that came out of collision_regime.
             ! The remainder from the third bin will be distributed among nfrag-2 bodies. 
 
-            !Add a small amount of noise to the last digits of the minimum mass value so that multiple fragments don't get generated with identical mass values
+            ! Add a small amount of noise to the last digits of the minimum mass value so that multiple fragments don't get 
+            ! generated with identical mass values
             call random_number(mass_noise)
             mass_noise = 1.0_DP + mass_noise * epsilon(1.0_DP) * 10**(MASS_NOISE_FACTOR)
             min_mfrag = (param%min_GMfrag / param%GU) * mass_noise
             
             mremaining = impactors%mass_dist(iMrem)
             nfrag = iMrem - 1 
             Mslr = impactors%mass_dist(iMslr)
@@ -179,15 +185,16 @@
             beta = 3.0_DP
             call solve_roots(fraggle_util_sfd_function,beta)
 
             do i = iMrem,nfrag
                mass(i) = Mslr * (i-1)**(-beta/3.0_DP)
             end do
 
-            ! There may still be some small residual due to round-off error. If so, simply add it to the last bin of the mass distribution.
+            ! There may still be some small residual due to round-off error. If so, simply add it to the last bin of the mass 
+            ! distribution.
             mremaining = fragments%mtot - sum(mass(1:nfrag))
             if (mremaining < 0.0_DP) then
                mass(iMlr) = mass(iMlr) + mremaining
             else
                mass(iMslr) = mass(iMslr) + mremaining
             end if
 
@@ -196,35 +203,39 @@
             call util_sort_rearrange(mass, ind, nfrag)
             call move_alloc(mass, fragments%mass)
 
             fragments%Gmass(:) = G * fragments%mass(:)
 
             ! Compute physical properties of the new fragments
             select case(impactors%regime)
-            case(COLLRESOLVE_REGIME_HIT_AND_RUN)  ! The hit and run case always preserves the largest body intact, so there is no need to recompute the physical properties of the first fragment
+            case(COLLRESOLVE_REGIME_HIT_AND_RUN)  
+               ! The hit and run case always preserves the largest body intact, so there is no need to recompute the physical 
+               ! properties of the first fragment
                fragments%radius(1) = impactors%radius(jtarg)
                fragments%density(1) = impactors%mass_dist(iMlr) / volume(jtarg)
                fragments%Ip(:, 1) = impactors%Ip(:,1)
                istart = 2
             case default
                istart = 1
             end select
 
             fragments%density(istart:nfrag) = fragments%mtot / sum(volume(:))
-            fragments%radius(istart:nfrag) = (3 * fragments%mass(istart:nfrag) / (4 * PI * fragments%density(istart:nfrag)))**(1.0_DP / 3.0_DP)
+            fragments%radius(istart:nfrag) = (3 * fragments%mass(istart:nfrag) / &
+                                             (4 * PI * fragments%density(istart:nfrag)))**(1.0_DP / 3.0_DP)
 #ifdef DOCONLOC
             do concurrent(i = istart:nfrag) shared(fragments,Ip_avg)
 #else
             do concurrent(i = istart:nfrag)
 #endif
                fragments%Ip(:, i) = Ip_avg(:)
             end do
 
-            ! For catastrophic impacts, we will assign each of the n>2 fragments to one of the two original bodies so that the fragment cloud occupies 
-            ! roughly the same space as both original bodies. For all other disruption cases, we use body 2 as the center of the cloud.
+            ! For catastrophic impacts, we will assign each of the n>2 fragments to one of the two original bodies so that the 
+            ! fragment cloud occupies roughly the same space as both original bodies. For all other disruption cases, we use body 2
+            ! as the center of the cloud.
             fragments%origin_body(1) = 1_I1B
             fragments%origin_body(2) = 2_I1B
             if (impactors%regime == COLLRESOLVE_REGIME_SUPERCATASTROPHIC) then
                mcumul = fragments%mass(1)
                flipper = .true.
                j = 2
                do i = 1, nfrag
```

### Comparing `swiftest-2024.4.1/src/globals/globals_module.f90` & `swiftest-2024.4.2/src/globals/globals_module.f90`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
    integer(I4B), parameter :: LOWERCASE_BEGIN  = iachar('a') !! ASCII character set parameter for lower to upper conversion - start 
                                                              !! of lowercase
    integer(I4B), parameter :: LOWERCASE_END    = iachar('z') !! ASCII character set parameter for lower to upper conversion - end of 
                                                              !! lowercase
    integer(I4B), parameter :: UPPERCASE_OFFSET = iachar('A') - iachar('a') !! ASCII character set parameter for lower to upper 
                                                                            !! conversion - offset between upper and lower
 
-   character(*), parameter :: VERSION = "2024.4.0" !! Swiftest version
+   character(*), parameter :: VERSION = "2024.4.2" !! Swiftest version
 
    !> Symbolic name for integrator types
    character(*), parameter :: UNKNOWN_INTEGRATOR = "UKNOWN INTEGRATOR"
    character(*), parameter :: INT_BS                 = "Bulirsch-Stoer"
    character(*), parameter :: INT_HELIO              = "Democratic Heliocentric"
    character(*), parameter :: INT_RA15               = "Radau 15th order"
    character(*), parameter :: INT_TU4                = "T+U 4th order"
```

### Comparing `swiftest-2024.4.1/src/globals/globals_module.f90.in` & `swiftest-2024.4.2/src/globals/globals_module.f90.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/helio/helio_drift.f90` & `swiftest-2024.4.2/src/helio/helio_drift.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/helio/helio_gr.f90` & `swiftest-2024.4.2/src/helio/helio_gr.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/helio/helio_kick.f90` & `swiftest-2024.4.2/src/helio/helio_kick.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/helio/helio_module.f90` & `swiftest-2024.4.2/src/helio/helio_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/helio/helio_step.f90` & `swiftest-2024.4.2/src/helio/helio_step.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/helio/helio_util.f90` & `swiftest-2024.4.2/src/helio/helio_util.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/main/main.f90` & `swiftest-2024.4.2/src/main/main.f90`

 * *Files 10% similar despite different names*

```diff
@@ -15,23 +15,12 @@
    use swiftest
    implicit none
 
    character(len=:), allocatable             :: integrator        !! Integrator type code (see globals for symbolic names)
    character(len=:), allocatable             :: param_file_name   !! Name of the file containing user-defined parameters
    character(len=:), allocatable             :: display_style     !! Style of the output display {"STANDARD", "COMPACT", "PROGRESS"}). Default is "STANDARD"
 
-   ! Read in command line arguments
    call swiftest_io_get_args(integrator, param_file_name, display_style, from_cli=.true.)
-
-   ! Execute the driver
    call swiftest_driver(integrator, param_file_name, display_style)
-
-
-#ifdef COARRAY
-   if (this_image() == 1) then
-#endif
-      call base_util_exit(SUCCESS)
-#ifdef COARRAY
-   end if ! (this_image() == 1) 
-#endif
+   call base_util_exit(SUCCESS)
 
 end program main
```

### Comparing `swiftest-2024.4.1/src/misc/io_progress_bar_module.f90` & `swiftest-2024.4.2/src/misc/io_progress_bar_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/misc/lambda_function_module.f90` & `swiftest-2024.4.2/src/misc/lambda_function_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/misc/solver_module.f90` & `swiftest-2024.4.2/src/misc/solver_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/netcdf_io/netcdf_io_implementations.f90` & `swiftest-2024.4.2/src/netcdf_io/netcdf_io_implementations.f90`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 
    module subroutine netcdf_io_check(status, call_identifier)
       !! author: Carlisle A. Wishard, Dana Singh, and David A. Minton
       !!
       !! Checks the status of all NetCDF operations to catch errors
       implicit none
       ! Arguments
-      integer, intent (in) :: status !! The status code returned by a NetCDF function
-      character(len=*), intent(in), optional :: call_identifier !! String that indicates which calling function caused the error for diagnostic purposes
+      integer, intent (in) :: status 
+         !! The status code returned by a NetCDF function
+      character(len=*), intent(in), optional :: call_identifier 
+         !! String that indicates which calling function caused the error for diagnostic purposes
 
       if(status /= NF90_NOERR) then
          if (present(call_identifier)) write(*,*) "NetCDF error in ",trim(call_identifier)
          write(*,*) trim(nf90_strerror(status))
          call base_util_exit(FAILURE)
       end if
 
@@ -53,16 +55,17 @@
       return
    end subroutine netcdf_io_close
 
 
    module subroutine netcdf_io_find_tslot(self, t, tslot)
       !! author: David A. Minton
       !! 
-      !! Given an open NetCDF file and a value of time t, finds the index of the time value (aka the time slot) to place a new set of data.
-      !! The returned value of tslot will correspond to the first index value where the value of t is greater than or equal to the saved time value.
+      !! Given an open NetCDF file and a value of time t, finds the index of the time value (aka the time slot) to place a new set 
+      !! of data.  The returned value of tslot will correspond to the first index value where the value of t is greater than or 
+      !! equal to the saved time value.
       use, intrinsic :: ieee_exceptions
       use, intrinsic :: ieee_arithmetic
       implicit none
       ! Arguments
       class(netcdf_parameters), intent(inout) :: self  !! Parameters used to identify a particular NetCDF dataset
       real(DP),                 intent(in)    :: t     !! The value of time to search for
       integer(I4B),             intent(out)   :: tslot !! The index of the time slot where this data belongs
@@ -73,15 +76,16 @@
 
       call ieee_get_halting_mode(IEEE_ALL,fpe_halting_modes)  ! Save the current halting modes so we can turn them off temporarily
       call ieee_set_halting_mode(IEEE_ALL,.false.)
 
       if (.not.self%lfile_is_open) return
       tslot = 0
 
-      call netcdf_io_check( nf90_inquire_dimension(self%id, self%time_dimid, self%time_dimname, len=self%max_tslot), "netcdf_io_find_tslot nf90_inquire_dimension max_tslot"  )
+      call netcdf_io_check( nf90_inquire_dimension(self%id, self%time_dimid, self%time_dimname, len=self%max_tslot), &
+                             "netcdf_io_find_tslot nf90_inquire_dimension max_tslot"  )
       if (self%max_tslot > 0) then
          allocate(tvals(self%max_tslot))
          call netcdf_io_check( nf90_get_var(self%id, self%time_varid, tvals(:), start=[1]), "netcdf_io_find_tslot get_var"  )
          where(.not.ieee_is_normal(tvals(:))) tvals(:) = huge(1.0_DP)
       else
          allocate(tvals(1))
          tvals(1) = huge(1.0_DP)
@@ -102,15 +106,16 @@
    end subroutine netcdf_io_find_tslot
 
 
    module subroutine netcdf_io_find_idslot(self, id, idslot)
       !! author: David A. Minton
       !! 
       !! Given an open NetCDF file and a value of id, finds the index of the id value (aka the id slot) to place a new set of data.
-      !! The returned value of idslot will correspond to the first index value where the value of id is greater than or equal to the saved id value.
+      !! The returned value of idslot will correspond to the first index value where the value of id is greater than or equal to the
+      !! saved id value.
       implicit none
       ! Arguments
       class(netcdf_parameters), intent(inout) :: self   !! Parameters used to identify a particular NetCDF dataset
       integer(I4B),             intent(in)    :: id     !! The value of id to search for
       integer(I4B),             intent(out)   :: idslot !! The index of the id slot where this data belongs
       ! Internals
       integer(I4B), dimension(:), allocatable :: idvals
@@ -139,24 +144,26 @@
 
    module subroutine netcdf_io_get_idvals(self)
       !! author: David A. Minton
       !! 
       !! Gets a full list of id values 
       implicit none
       ! Arguments
-      class(netcdf_parameters),                            intent(inout) :: self   !! Parameters used to identify a particular NetCDF dataset
+      class(netcdf_parameters), intent(inout) :: self   
+         !! Parameters used to identify a particular NetCDF dataset
       ! Internals
 
       if (.not.self%lfile_is_open) return
 
       if (allocated(self%idvals)) deallocate(self%idvals)
-      call netcdf_io_check( nf90_inquire_dimension(self%id, self%name_dimid, self%name_dimname, len=self%max_idslot), "netcdf_io_find_tslot nf90_inquire_dimension max_tslot"  )
+      call netcdf_io_check( nf90_inquire_dimension(self%id, self%name_dimid, self%name_dimname, len=self%max_idslot), &
+                           "netcdf_io_find_tslot nf90_inquire_dimension max_tslot"  )
       if (self%max_idslot > 0) then
          allocate(self%idvals(self%max_idslot))
-         call netcdf_io_check( nf90_get_var(self%id, self%id_varid, self%idvals(:), start=[1]), "netcdf_io_find_idslot get_var"  )
+         call netcdf_io_check( nf90_get_var(self%id, self%id_varid, self%idvals(:), start=[1]), "netcdf_io_find_idslot get_var" )
       else
          allocate(self%idvals(1))
          self%idvals(1) = 0
       end if
 
       return
    end subroutine netcdf_io_get_idvals
```

### Comparing `swiftest-2024.4.1/src/netcdf_io/netcdf_io_module.f90` & `swiftest-2024.4.2/src/netcdf_io/netcdf_io_module.f90`

 * *Files 4% similar despite different names*

```diff
@@ -186,22 +186,22 @@
          !! name of the Love number variable
       integer(I4B) :: k2_varid 
          !! ID for the Love number variable
       character(NAMELEN) :: q_varname = "Q"
          !! name of the energy dissipation variable
       integer(I4B) :: Q_varid 
          !! ID for the energy dissipation variable
-      character(NAMELEN) :: ke_orb_varname = "KE_orb"
+      character(NAMELEN) :: ke_orbit_varname = "KE_orbit"
          !! name of the system orbital kinetic energy variable
       integer(I4B) :: KE_orb_varid
          !! ID for the system orbital kinetic energy variable
-      character(NAMELEN) :: ke_spin_varname = "KE_spin"
-         !! name of the system spin kinetic energy variable
-      integer(I4B) :: KE_spin_varid
-         !! ID for the system spin kinetic energy variable
+      character(NAMELEN) :: ke_rot_varname = "KE_rot"
+         !! name of the system rotational kinetic energy variable
+      integer(I4B) :: KE_rot_varid
+         !! ID for the system rotational kinetic energy variable
       character(NAMELEN) :: pe_varname = "PE"
          !! name of the system potential energy variable
       integer(I4B) :: PE_varid 
          !! ID for the system potential energy variable
       character(NAMELEN) :: be_varname = "BE"
          !! name of the system binding energy variable
       integer(I4B) :: BE_varid 
@@ -210,18 +210,18 @@
          !! name of the system binding energy variable
       integer(I4B) :: TE_varid 
          !! ID for the system binding energy variable
       character(NAMELEN) :: L_orbit_varname = "L_orbit"
          !! name of the orbital angular momentum vector variable
       integer(I4B) :: L_orbit_varid 
          !! ID for the system orbital angular momentum vector variable
-      character(NAMELEN) :: L_spin_varname = "L_spin"
-         !! name of the spin angular momentum vector variable
-      integer(I4B) :: L_spin_varid 
-         !! ID for the system spin angular momentum vector variable
+      character(NAMELEN) :: L_rot_varname = "L_rot"
+         !! name of the rotational angular momentum vector variable
+      integer(I4B) :: L_rot_varid 
+         !! ID for the system rotational angular momentum vector variable
       character(NAMELEN) :: L_escape_varname = "L_escape"
          !! name of the escaped angular momentum vector variable
       integer(I4B) :: L_escape_varid
          !! ID for the escaped angular momentum vector variable
       character(NAMELEN) :: E_collisions_varname = "E_collisions"
          !! name of the escaped angular momentum y variable 
       integer(I4B) :: E_collisions_varid
@@ -238,15 +238,15 @@
          !! name of the origin type variable 
       integer(I4B) :: origin_type_varid
          !! ID for the origin type
       character(NAMELEN) :: origin_time_varname = "origin_time"
          !! name of the time of origin variable
       integer(I4B) :: origin_time_varid
          !! ID for the origin time
-      character(NAMELEN) :: collision_id_varname = "collision_id"
+      character(NAMELEN) :: collision_id_dimname = "collision_id"
          !! name of the collision id variable
       integer(I4B) :: collision_id_varid
          !! Netcdf ID for the origin collision ID
       character(NAMELEN) :: origin_rh_varname = "origin_rh" 
          !! name of the heliocentric position vector of the body at the time of origin variable
       integer(I4B) :: origin_rh_varid
          !! ID for the origin position vector variable
```

### Comparing `swiftest-2024.4.1/src/operator/operator_cross.f90` & `swiftest-2024.4.2/src/operator/operator_cross.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/operator/operator_mag.f90` & `swiftest-2024.4.2/src/operator/operator_mag.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/operator/operator_module.f90` & `swiftest-2024.4.2/src/operator/operator_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/operator/operator_unit.f90` & `swiftest-2024.4.2/src/operator/operator_unit.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/rmvs/rmvs_discard.f90` & `swiftest-2024.4.2/src/symba/symba_drift.f90`

 * *Files 22% similar despite different names*

```diff
@@ -3,61 +3,61 @@
 ! Swiftest is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License 
 ! as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 ! Swiftest is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty 
 ! of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 ! You should have received a copy of the GNU General Public License along with Swiftest. 
 ! If not, see: https://www.gnu.org/licenses. 
 
-submodule(rmvs) s_rmvs_discard
+  submodule (symba) s_symba_drift
    use swiftest
-contains  
+contains
 
-   module subroutine rmvs_discard_tp(self, nbody_system, param)
+   module subroutine symba_drift_pl(self, nbody_system, param, dt)
       !! author: David A. Minton
       !!
-      !! Check to see if test particles should be discarded based on pericenter passage distances with respect to planets encountered
-      !!
-      !! Adapted from Hal Levison's Swift routine discard_pl.f
-      !! Adapted from Hal Levison's Swift routine rmvs_discard_pl.f90
+      !! Wrapper function used to call the body drift routine from a symba_pl structure
       implicit none
       ! Arguments
-      class(rmvs_tp),               intent(inout) :: self   !! RMVS test particle object
+      class(symba_pl),              intent(inout) :: self   !! Helio massive body object
       class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(swiftest_parameters),   intent(inout) :: param  !! Current run configuration parameters 
-      ! Internals
-      integer(I4B)                                 :: i
-      character(len=STRMAX) :: timestr, idstri, idstrj, message
+      class(swiftest_parameters),   intent(in)    :: param  !! Current run configuration parameters 
+      real(DP),                     intent(in)    :: dt     !! Stepsize
 
       if (self%nbody == 0) return
-
-      associate(tp => self, ntp => self%nbody, pl => nbody_system%pl, t => nbody_system%t)
-         do i = 1, ntp
-            associate(iplperP => tp%plperP(i))
-               if ((tp%status(i) == ACTIVE) .and. (tp%lperi(i))) then 
-                  if ((tp%peri(i) < pl%radius(iplperP))) then
-                     tp%status(i) = DISCARDED_PLQ
-                     write(idstri, *) tp%id(i)
-                     write(idstrj, *) pl%id(iplperP)
-                     write(timestr, *) t
-                     write(message, *) "Particle "  // trim(adjustl(tp%info(i)%name)) // " (" // trim(adjustl(idstri)) &
-                              // ") q with respect to massive body " // trim(adjustl(pl%info(iplperP)%name))   &
-                              // " (" // trim(adjustl(idstrj)) // ") is too small at t = " // trim(adjustl(timestr))
-                     call swiftest_io_log_one_message(COLLISION_LOG_OUT,message)
-                     tp%ldiscard(i) = .true.
-                     tp%lmask(i) = .false.
-                     pl%ldiscard(iplperP) = .true.
-                     call tp%info(i)%set_value(status="DISCARDED_PLQ", discard_time=t, discard_rh=tp%rh(:,i), &
-                                               discard_vh=tp%vh(:,i), discard_body_id=pl%id(iplperP))
-                  end if
-               end if
-            end associate
-         end do
-         ! Call the base method that this overrides
-         call swiftest_discard_tp(tp, nbody_system, param)
+      associate(pl => self, npl => self%nbody)
+         select type(nbody_system)
+         class is (symba_nbody_system)
+            pl%lmask(1:npl) = pl%status(1:npl) /= INACTIVE .and. pl%levelg(1:npl) == nbody_system%irec
+            call helio_drift_body(pl, nbody_system, param, dt)
+            pl%lmask(1:npl) = pl%status(1:npl) /= INACTIVE 
+         end select
       end associate
 
-
       return
+   end subroutine symba_drift_pl
+
+
+   module subroutine symba_drift_tp(self, nbody_system, param, dt)
+      !! author: David A. Minton
+      !!
+      !! Wrapper function used to call the body drift routine from a symba_pl structure
+      implicit none
+      ! Arguments
+      class(symba_tp),              intent(inout) :: self   !! Helio massive body object
+      class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
+      class(swiftest_parameters),   intent(in)    :: param  !! Current run configuration parameters 
+      real(DP),                     intent(in)    :: dt     !! Stepsize
 
-   end subroutine rmvs_discard_tp
+      if (self%nbody == 0) return
+      associate (tp => self, ntp => self%nbody)
+         select type(nbody_system)
+         class is (symba_nbody_system)
+            tp%lmask(1:ntp) = tp%status(1:ntp) /= INACTIVE .and. tp%levelg(1:ntp) == nbody_system%irec
+            call helio_drift_body(tp, nbody_system, param, dt)
+            tp%lmask(1:ntp) = tp%status(1:ntp) /= INACTIVE 
+         end select
+      end associate
+
+      return
+   end subroutine symba_drift_tp
 
-end submodule s_rmvs_discard
+end submodule s_symba_drift
```

### Comparing `swiftest-2024.4.1/src/rmvs/rmvs_encounter_check.f90` & `swiftest-2024.4.2/src/rmvs/rmvs_encounter_check.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/rmvs/rmvs_kick.f90` & `swiftest-2024.4.2/src/rmvs/rmvs_kick.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/rmvs/rmvs_module.f90` & `swiftest-2024.4.2/src/rmvs/rmvs_module.f90`

 * *Files 7% similar despite different names*

```diff
@@ -23,376 +23,485 @@
    real(DP),     private, parameter :: RHSCALE = 3.5_DP
    real(DP),     private, parameter :: RHPSCALE = 1.0_DP
    real(DP),     private, parameter :: FACQDT = 2.0_DP
 
 
    !> In the RMVS integrator, pl-tp encounters are handeled, but not pl-pl 
    type, extends(whm_nbody_system) :: rmvs_nbody_system
-      logical                               :: lplanetocentric = .false.  !! Flag that indicates that the object is a planetocentric set of masive bodies used for close encounter calculations
-      real(DP)                              :: rts                        !! fraction of Hill's sphere radius to use as radius of encounter region
-      real(DP), dimension(:,:), allocatable :: vbeg                       !! Planet velocities at beginning ot step
+      logical                               :: lplanetocentric = .false.  
+         !! Flag that indicates that the object is a planetocentric set of masive bodies used for close encounter calculations
+      real(DP)                              :: rts                        
+         !! fraction of Hill's sphere radius to use as radius of encounter region
+      real(DP), dimension(:,:), allocatable :: vbeg                       
+         !! Planet velocities at beginning ot step
    contains
       !> Replace the abstract procedures with concrete ones
-      procedure :: dealloc    => rmvs_util_dealloc_system           !! Performs RMVS-specific deallocation
-      procedure :: initialize => rmvs_util_setup_initialize_system  !! Performs RMVS-specific initilization steps, including generating the close encounter planetocentric structures
-      procedure :: step       => rmvs_step_system                   !! Advance the RMVS nbody system forward in time by one step
-#ifdef COARRAY
-      procedure :: coclone                 => rmvs_coarray_coclone_system  !! Clones the image 1 body object to all other images in the coarray structure.
-#endif
+      procedure :: dealloc    => rmvs_util_dealloc_system           
+         !! Performs RMVS-specific deallocation
+      procedure :: initialize => rmvs_util_setup_initialize_system  
+         !! Performs RMVS-specific initilization steps, including generating the close encounter planetocentric structures
+      procedure :: step       => rmvs_step_system                   
+         !! Advance the RMVS nbody system forward in time by one step
    end type rmvs_nbody_system
 
    type, private :: rmvs_interp
-      real(DP), dimension(:, :), allocatable :: x     !! interpolated heliocentric planet position for outer encounter
-      real(DP), dimension(:, :), allocatable :: v     !! interpolated heliocentric planet velocity for outer encounter
-      real(DP), dimension(:, :), allocatable :: aobl  !! Encountering planet's oblateness acceleration value
-      real(DP), dimension(:, :), allocatable :: atide !! Encountering planet's tidal acceleration value
+      real(DP), dimension(:, :), allocatable :: x     
+         !! interpolated heliocentric planet position for outer encounter
+      real(DP), dimension(:, :), allocatable :: v     
+         !! interpolated heliocentric planet velocity for outer encounter
+      real(DP), dimension(:, :), allocatable :: aobl  
+         !! Encountering planet's oblateness acceleration value
+      real(DP), dimension(:, :), allocatable :: atide 
+         !! Encountering planet's tidal acceleration value
    contains
-      procedure :: dealloc => rmvs_util_dealloc_interp !! Deallocates all allocatable arrays
-      final     ::            rmvs_final_interp   !! Finalizes the RMVS interpolated nbody_system variables object - deallocates all allocatables
-#ifdef COARRAY
-      procedure :: coclone => rmvs_coarray_coclone_interp
-#endif
+      procedure :: dealloc => rmvs_util_dealloc_interp 
+         !! Deallocates all allocatable arrays
+      final ::   rmvs_final_interp   
+         !! Finalizes the RMVS interpolated nbody_system variables object - deallocates all allocatables
    end type rmvs_interp
 
 
    !> RMVS central body particle class 
    type, extends(whm_cb) :: rmvs_cb
-      type(rmvs_interp), dimension(:), allocatable :: outer !! interpolated heliocentric central body position for outer encounters
-      type(rmvs_interp), dimension(:), allocatable :: inner !! interpolated heliocentric central body position for inner encounters
-      logical                                      :: lplanetocentric = .false.  !! Flag that indicates that the object is a planetocentric set of masive bodies used for close encounter calculations
+      type(rmvs_interp), dimension(:), allocatable :: outer 
+         !! interpolated heliocentric central body position for outer encounters
+      type(rmvs_interp), dimension(:), allocatable :: inner 
+         !! interpolated heliocentric central body position for inner encounters
+      logical                                      :: lplanetocentric = .false.  
+         !! Flag that indicates that the object is a planetocentric set of masive bodies used for close encounter calculations
    contains
-      procedure :: dealloc => rmvs_util_dealloc_cb !! Deallocates all allocatable arrays
-      final     ::            rmvs_final_cb   !! Finalizes the RMVS central body object - deallocates all allocatables
-#ifdef COARRAY
-      procedure :: coclone   => rmvs_coarray_coclone_cb      !! Clones the image 1 body object to all other images in the coarray structure.
-#endif 
+      procedure :: dealloc => rmvs_util_dealloc_cb 
+         !! Deallocates all allocatable arrays
+      final     ::            rmvs_final_cb   
+         !! Finalizes the RMVS central body object - deallocates all allocatables
    end type rmvs_cb
 
 
    !! RMVS test particle class
    type, extends(whm_tp) :: rmvs_tp
       !! Note to developers: If you add componenets to this class, be sure to update methods and subroutines that traverse the
       !!    component list, such as rmvs_util_setup_tp and rmvs_util_spill_tp
       ! encounter steps)
-      logical,      dimension(:),   allocatable :: lperi  !! planetocentric pericenter passage flag (persistent for a full rmvs time step) over a full RMVS time step)
-      integer(I4B), dimension(:),   allocatable :: plperP !! index of planet associated with pericenter distance peri (persistent over a full RMVS time step)
-      integer(I4B), dimension(:),   allocatable :: plencP !! index of planet that test particle is encountering (not persistent for a full RMVS time step)
+      logical, dimension(:),   allocatable :: lperi  
+         !! planetocentric pericenter passage flag (persistent for a full rmvs time step) over a full RMVS time step)
+      integer(I4B), dimension(:),   allocatable :: plperP 
+         !! index of planet associated with pericenter distance peri (persistent over a full RMVS time step)
+      integer(I4B), dimension(:),   allocatable :: plencP 
+         !! index of planet that test particle is encountering (not persistent for a full RMVS time step)
 
       ! The following are used to correctly set the oblateness values of the acceleration during an inner encounter with a planet
-      type(rmvs_cb)                             :: cb_heliocentric !! Copy of original central body object passed to close encounter (used for oblateness acceleration during planetocentric encoountters)
-      real(DP),     dimension(:,:), allocatable :: rheliocentric   !! original heliocentric position (used for oblateness calculation during close encounters)
-      integer(I4B)                              :: index           !!  inner substep number within current set
-      integer(I4B)                              :: ipleP           !!  index value of encountering planet
-      logical                                   :: lplanetocentric = .false.  !! Flag that indicates that the object is a planetocentric set of masive bodies used for close encounter calculations
+      type(rmvs_cb)                             :: cb_heliocentric 
+         !! Copy of original central body object passed to close encounter (used for oblateness acceleration during planetocentric 
+         !! encoountters)
+      real(DP),     dimension(:,:), allocatable :: rheliocentric   
+         !! original heliocentric position (used for oblateness calculation during close encounters)
+      integer(I4B)                              :: index           
+         !!  inner substep number within current set
+      integer(I4B)                              :: ipleP           
+         !!  index value of encountering planet
+      logical                                   :: lplanetocentric = .false.  
+         !! Flag that indicates that the object is a planetocentric set of masive bodies used for close encounter calculations
    contains
-      procedure :: discard         => rmvs_discard_tp             !! Check to see if test particles should be discarded based on pericenter passage distances with respect to planets encountered
-      procedure :: encounter_check => rmvs_encounter_check_tp     !! Checks if any test particles are undergoing a close encounter with a massive body
-      procedure :: accel           => rmvs_kick_getacch_tp        !! Calculates either the standard or modified version of the acceleration depending if the
-                                                                  !!    if the test particle is undergoing a close encounter or not
-      procedure :: setup           => rmvs_util_setup_tp               !! Constructor method - Allocates space for the input number of bodiess
-      procedure :: append          => rmvs_util_append_tp         !! Appends elements from one structure to another
-      procedure :: dealloc         => rmvs_util_dealloc_tp        !! Deallocates all allocatable arrays
-      procedure :: fill            => rmvs_util_fill_tp           !! "Fills" bodies from one object into another depending on the results of a mask (uses the UNPACK intrinsic)
-      procedure :: resize          => rmvs_util_resize_tp         !! Checks the current size of a Swiftest body against the requested size and resizes it if it is too small.
-      procedure :: sort            => rmvs_util_sort_tp           !! Sorts body arrays by a sortable componen
-      procedure :: rearrange       => rmvs_util_sort_rearrange_tp !! Rearranges the order of array elements of body based on an input index array. Used in sorting methods
-      procedure :: spill           => rmvs_util_spill_tp          !! "Spills" bodies from one object to another depending on the results of a mask (uses the PACK intrinsic)
-      final     ::                    rmvs_final_tp          !! Finalizes the RMVS test particle object - deallocates all allocatables
-#ifdef COARRAY
-      procedure :: coclone   => rmvs_coarray_coclone_tp      !! Clones the image 1 body object to all other images in the coarray structure.
-      procedure :: cocollect => rmvs_coarray_cocollect_tp      !! Clones the image 1 body object to all other images in the coarray structure.
-#endif 
+      procedure :: discard         => rmvs_discard_tp             
+         !! Check to see if test particles should be discarded based on pericenter passage distances with respect to planets encountered
+      procedure :: encounter_check => rmvs_encounter_check_tp     
+         !! Checks if any test particles are undergoing a close encounter with a massive body
+      procedure :: accel           => rmvs_kick_getacch_tp        
+         !! Calculates either the standard or modified version of the acceleration depending if the
+                                                                  
+         !!    if the test particle is undergoing a close encounter or not
+      procedure :: setup           => rmvs_util_setup_tp               
+         !! Constructor method - Allocates space for the input number of bodiess
+      procedure :: append          => rmvs_util_append_tp         
+         !! Appends elements from one structure to another
+      procedure :: dealloc         => rmvs_util_dealloc_tp        
+         !! Deallocates all allocatable arrays
+      procedure :: fill            => rmvs_util_fill_tp           
+         !! "Fills" bodies from one object into another depending on the results of a mask (uses the UNPACK intrinsic)
+      procedure :: resize          => rmvs_util_resize_tp         
+         !! Checks the current size of a Swiftest body against the requested size and resizes it if it is too small.
+      procedure :: sort            => rmvs_util_sort_tp           
+         !! Sorts body arrays by a sortable componen
+      procedure :: rearrange       => rmvs_util_sort_rearrange_tp 
+         !! Rearranges the order of array elements of body based on an input index array. Used in sorting methods
+      procedure :: spill           => rmvs_util_spill_tp          
+         !! "Spills" bodies from one object to another depending on the results of a mask (uses the PACK intrinsic)
+      final     ::                    rmvs_final_tp          
+         !! Finalizes the RMVS test particle object - deallocates all allocatables
    end type rmvs_tp
 
  
    !> RMVS massive body particle class
    type, extends(whm_pl) :: rmvs_pl
-      integer(I4B),             dimension(:), allocatable :: nenc                      !! number of test particles encountering planet this full rmvs time step
-      integer(I4B),             dimension(:), allocatable :: tpenc1P                   !! index of first test particle encountering planet
-      integer(I4B),             dimension(:), allocatable :: plind                     !! Connects the planetocentric indices back to the heliocentric planet list
-      type(rmvs_interp),        dimension(:), allocatable :: outer                     !! interpolated heliocentric central body position for outer encounters
-      type(rmvs_interp),        dimension(:), allocatable :: inner                     !! interpolated heliocentric central body position for inner encounters
-      class(rmvs_nbody_system), dimension(:), allocatable :: planetocentric            !! Planetocentric version of the massive body objects (one for each massive body)
-      logical                                             :: lplanetocentric = .false. !! Flag that indicates that the object is a planetocentric set of masive bodies used for close encounter calculations
+      integer(I4B),             dimension(:), allocatable :: nenc                      
+         !! number of test particles encountering planet this full rmvs time step
+      integer(I4B),             dimension(:), allocatable :: tpenc1P                   
+         !! index of first test particle encountering planet
+      integer(I4B),             dimension(:), allocatable :: plind                     
+         !! Connects the planetocentric indices back to the heliocentric planet list
+      type(rmvs_interp),        dimension(:), allocatable :: outer                     
+         !! interpolated heliocentric central body position for outer encounters
+      type(rmvs_interp),        dimension(:), allocatable :: inner                     
+         !! interpolated heliocentric central body position for inner encounters
+      class(rmvs_nbody_system), dimension(:), allocatable :: planetocentric            
+         !! Planetocentric version of the massive body objects (one for each massive body)
+      logical                                             :: lplanetocentric = .false. 
+         !! Flag that indicates that the object is a planetocentric set of masive bodies used for close encounter calculations
    contains
-      procedure :: setup     => rmvs_util_setup_pl          !! Constructor method - Allocates space for the input number of bodiess
-      procedure :: append    => rmvs_util_append_pl         !! Appends elements from one structure to another
-      procedure :: dealloc   => rmvs_util_dealloc_pl        !! Deallocates all allocatable arrays
-      procedure :: fill      => rmvs_util_fill_pl           !! "Fills" bodies from one object into another depending on the results of a mask (uses the UNPACK intrinsic)
-      procedure :: resize    => rmvs_util_resize_pl         !! Checks the current size of a Swiftest body against the requested size and resizes it if it is too small.
-      procedure :: sort      => rmvs_util_sort_pl           !! Sorts body arrays by a sortable componen
-      procedure :: rearrange => rmvs_util_sort_rearrange_pl !! Rearranges the order of array elements of body based on an input index array. Used in sorting methods
-      procedure :: spill     => rmvs_util_spill_pl          !! "Spills" bodies from one object to another depending on the results of a mask (uses the PACK intrinsic)
-      final     ::              rmvs_final_pl               !! Finalizes the RMVS massive body object - deallocates all allocatables
-#ifdef COARRAY
-      procedure :: coclone   => rmvs_coarray_coclone_pl      !! Clones the image 1 body object to all other images in the coarray structure.
-#endif 
+      procedure :: setup     => rmvs_util_setup_pl          
+         !! Constructor method - Allocates space for the input number of bodiess
+      procedure :: append    => rmvs_util_append_pl         
+         !! Appends elements from one structure to another
+      procedure :: dealloc   => rmvs_util_dealloc_pl        
+         !! Deallocates all allocatable arrays
+      procedure :: fill      => rmvs_util_fill_pl           
+         !! "Fills" bodies from one object into another depending on the results of a mask (uses the UNPACK intrinsic)
+      procedure :: resize    => rmvs_util_resize_pl         
+         !! Checks the current size of a Swiftest body against the requested size and resizes it if it is too small.
+      procedure :: sort      => rmvs_util_sort_pl           
+         !! Sorts body arrays by a sortable componen
+      procedure :: rearrange => rmvs_util_sort_rearrange_pl 
+         !! Rearranges the order of array elements of body based on an input index array. Used in sorting methods
+      procedure :: spill     => rmvs_util_spill_pl          
+         !! "Spills" bodies from one object to another depending on the results of a mask (uses the PACK intrinsic)
+      final     ::              rmvs_final_pl               
+         !! Finalizes the RMVS massive body object - deallocates all allocatables
    end type rmvs_pl
 
    interface
       module subroutine rmvs_discard_tp(self, nbody_system, param)
          implicit none
-         class(rmvs_tp),               intent(inout) :: self   !! RMVS test particle object
-         class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-         class(swiftest_parameters),   intent(inout) :: param  !! Current run configuration parameters 
+         class(rmvs_tp),               intent(inout) :: self   
+            !! RMVS test particle object
+         class(swiftest_nbody_system), intent(inout) :: nbody_system 
+            !! Swiftest nbody system object
+         class(swiftest_parameters),   intent(inout) :: param  
+            !! Current run configuration parameters 
       end subroutine rmvs_discard_tp
 
       module function rmvs_encounter_check_tp(self, param, nbody_system, dt) result(lencounter)
          implicit none
-         class(rmvs_tp),             intent(inout) :: self       !! RMVS test particle object  
-         class(swiftest_parameters), intent(inout) :: param      !! Current run configuration parameters 
-         class(rmvs_nbody_system),   intent(inout) :: nbody_system     !! RMVS nbody system object
-         real(DP),                   intent(in)    :: dt         !! step size
-         logical                                   :: lencounter !! Returns true if there is at least one close encounter      
+         class(rmvs_tp),             intent(inout) :: self       
+            !! RMVS test particle object  
+         class(swiftest_parameters), intent(inout) :: param      
+            !! Current run configuration parameters 
+         class(rmvs_nbody_system),   intent(inout) :: nbody_system     
+            !! RMVS nbody system object
+         real(DP),                   intent(in)    :: dt         
+            !! step size
+         logical                                   :: lencounter 
+            !! Returns true if there is at least one close encounter      
       end function rmvs_encounter_check_tp
 
       module subroutine rmvs_kick_getacch_tp(self, nbody_system, param, t, lbeg)
          implicit none
-         class(rmvs_tp),               intent(inout) :: self   !! RMVS test particle data structure
-         class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest central body particle data structuree 
-         class(swiftest_parameters),   intent(inout) :: param  !! Current run configuration parameters
-         real(DP),                     intent(in)    :: t      !! Current time
-         logical,                      intent(in)    :: lbeg   !! Logical flag that determines whether or not this is the beginning or end of the step
+         class(rmvs_tp),               intent(inout) :: self   
+            !! RMVS test particle data structure
+         class(swiftest_nbody_system), intent(inout) :: nbody_system 
+            !! Swiftest central body particle data structuree 
+         class(swiftest_parameters),   intent(inout) :: param  
+            !! Current run configuration parameters
+         real(DP),                     intent(in)    :: t      
+            !! Current time
+         logical,                      intent(in)    :: lbeg   
+            !! Logical flag that determines whether or not this is the beginning or end of the step
       end subroutine rmvs_kick_getacch_tp
 
       module subroutine rmvs_util_setup_pl(self, n, param)
          implicit none
-         class(rmvs_pl),             intent(inout) :: self  !! RMVS massive body object
-         integer(I4B),               intent(in)    :: n     !! Number of particles to allocate space for
-         class(swiftest_parameters), intent(in)    :: param !! Current run configuration parameters
+         class(rmvs_pl),             intent(inout) :: self  
+            !! RMVS massive body object
+         integer(I4B),               intent(in)    :: n     
+            !! Number of particles to allocate space for
+         class(swiftest_parameters), intent(in)    :: param 
+            !! Current run configuration parameters
       end subroutine rmvs_util_setup_pl
 
       module subroutine rmvs_util_setup_initialize_system(self, system_history, param)
          implicit none
-         class(rmvs_nbody_system),                intent(inout) :: self           !! RMVS system object
-         class(swiftest_storage),    allocatable, intent(inout) :: system_history !! Stores the system history between output dumps
-         class(swiftest_parameters),              intent(inout) :: param          !! Current run configuration parameters 
+         class(rmvs_nbody_system),                intent(inout) :: self           
+            !! RMVS system object
+         class(swiftest_storage),    allocatable, intent(inout) :: system_history 
+            !! Stores the system history between output dumps
+         class(swiftest_parameters),              intent(inout) :: param          
+            !! Current run configuration parameters 
       end subroutine rmvs_util_setup_initialize_system
 
       module subroutine rmvs_util_setup_tp(self, n, param)
          implicit none
-         class(rmvs_tp),            intent(inout) :: self !! RMVS test particle object
-         integer(I4B),              intent(in)    :: n     !! Number of particles to allocate space for
-         class(swiftest_parameters), intent(in)    :: param !! Current run configuration parametere
+         class(rmvs_tp),            intent(inout) :: self 
+            !! RMVS test particle object
+         integer(I4B),              intent(in)    :: n     
+            !! Number of particles to allocate space for
+         class(swiftest_parameters), intent(in)    :: param 
+            !! Current run configuration parametere
       end subroutine rmvs_util_setup_tp
 
       module subroutine rmvs_util_append_pl(self, source, lsource_mask)
          implicit none
-         class(rmvs_pl),                  intent(inout) :: self         !! RMVS massive body object
-         class(swiftest_body),            intent(in)    :: source       !! Source object to append
-         logical, dimension(:),           intent(in)    :: lsource_mask !! Logical mask indicating which elements to append to
+         class(rmvs_pl),                  intent(inout) :: self         
+            !! RMVS massive body object
+         class(swiftest_body),            intent(in)    :: source       
+            !! Source object to append
+         logical, dimension(:),           intent(in)    :: lsource_mask 
+            !! Logical mask indicating which elements to append to
       end subroutine rmvs_util_append_pl
 
       module subroutine rmvs_util_append_tp(self, source, lsource_mask)
          implicit none
-         class(rmvs_tp),                  intent(inout) :: self         !! RMVS test particle object
-         class(swiftest_body),            intent(in)    :: source       !! Source object to append
-         logical, dimension(:),           intent(in)    :: lsource_mask !! Logical mask indicating which elements to append to
+         class(rmvs_tp),                  intent(inout) :: self         
+            !! RMVS test particle object
+         class(swiftest_body),            intent(in)    :: source       
+            !! Source object to append
+         logical, dimension(:),           intent(in)    :: lsource_mask 
+            !! Logical mask indicating which elements to append to
       end subroutine rmvs_util_append_tp
 
       module subroutine rmvs_util_dealloc_cb(self)
          implicit none
-         class(rmvs_cb),  intent(inout) :: self !! RMVS central body object
+         class(rmvs_cb),  intent(inout) :: self 
+            !! RMVS central body object
       end subroutine rmvs_util_dealloc_cb
 
       module subroutine rmvs_util_dealloc_interp(self)
          implicit none
-         class(rmvs_interp),  intent(inout) :: self !! RMVS interpolated nbody_system variables object
+         class(rmvs_interp),  intent(inout) :: self 
+            !! RMVS interpolated nbody_system variables object
       end subroutine rmvs_util_dealloc_interp
 
       module subroutine rmvs_util_dealloc_pl(self)
          implicit none
-         class(rmvs_pl),  intent(inout) :: self !! RMVS massive body object
+         class(rmvs_pl),  intent(inout) :: self 
+            !! RMVS massive body object
       end subroutine rmvs_util_dealloc_pl
 
       module subroutine rmvs_util_dealloc_system(self)
          implicit none
          class(rmvs_nbody_system), intent(inout) :: self
       end subroutine rmvs_util_dealloc_system
 
       module subroutine rmvs_util_dealloc_tp(self)
          implicit none
-         class(rmvs_tp),  intent(inout) :: self !! RMVS test particle object
+         class(rmvs_tp),  intent(inout) :: self 
+            !! RMVS test particle object
       end subroutine rmvs_util_dealloc_tp
 
       module subroutine rmvs_util_fill_pl(self, inserts, lfill_list)
          implicit none
-         class(rmvs_pl),        intent(inout) :: self       !! RMVS massive body object 
-         class(swiftest_body),  intent(in)    :: inserts    !! Inserted object 
-         logical, dimension(:), intent(in)    :: lfill_list !! Logical array of bodies to merge into the keeps
+         class(rmvs_pl),        intent(inout) :: self       
+            !! RMVS massive body object 
+         class(swiftest_body),  intent(in)    :: inserts    
+            !! Inserted object 
+         logical, dimension(:), intent(in)    :: lfill_list 
+            !! Logical array of bodies to merge into the keeps
       end subroutine rmvs_util_fill_pl
 
       module subroutine rmvs_util_fill_tp(self, inserts, lfill_list)
          implicit none
-         class(rmvs_tp),        intent(inout) :: self        !! RMVS massive body object
-         class(swiftest_body),  intent(in)    :: inserts     !!  Inserted object 
-         logical, dimension(:), intent(in)    :: lfill_list !! Logical array of bodies to merge into the keeps
+         class(rmvs_tp),        intent(inout) :: self        
+            !! RMVS massive body object
+         class(swiftest_body),  intent(in)    :: inserts     
+            !!  Inserted object 
+         logical, dimension(:), intent(in)    :: lfill_list 
+            !! Logical array of bodies to merge into the keeps
       end subroutine rmvs_util_fill_tp
 
       module subroutine rmvs_util_resize_pl(self, nnew)
          implicit none
-         class(rmvs_pl), intent(inout) :: self  !! RMVS massive body object
-         integer(I4B),   intent(in)    :: nnew  !! New size neded
+         class(rmvs_pl), intent(inout) :: self  
+            !! RMVS massive body object
+         integer(I4B),   intent(in)    :: nnew  
+            !! New size neded
       end subroutine rmvs_util_resize_pl
 
       module subroutine rmvs_util_resize_tp(self, nnew)
          implicit none
-         class(rmvs_tp), intent(inout) :: self  !! RMVS test particle object
-         integer(I4B),   intent(in)    :: nnew  !! New size neded
+         class(rmvs_tp), intent(inout) :: self  
+            !! RMVS test particle object
+         integer(I4B),   intent(in)    :: nnew  
+            !! New size neded
       end subroutine rmvs_util_resize_tp
 
       module subroutine rmvs_util_sort_pl(self, sortby, ascending)
          implicit none
-         class(rmvs_pl), intent(inout) :: self      !! RMVS massive body object
-         character(*),   intent(in)    :: sortby    !! Sorting attribute
-         logical,        intent(in)    :: ascending !! Logical flag indicating whether or not the sorting should be in ascending or descending order
+         class(rmvs_pl), intent(inout) :: self      
+            !! RMVS massive body object
+         character(*),   intent(in)    :: sortby    
+            !! Sorting attribute
+         logical,        intent(in)    :: ascending 
+            !! Logical flag indicating whether or not the sorting should be in ascending or descending order
       end subroutine rmvs_util_sort_pl   
 
       module subroutine rmvs_util_sort_tp(self, sortby, ascending)
          implicit none
-         class(rmvs_tp), intent(inout) :: self      !! RMVS test particle object
-         character(*),   intent(in)    :: sortby    !! Sorting attribute
-         logical,        intent(in)    :: ascending !! Logical flag indicating whether or not the sorting should be in ascending or descending order
+         class(rmvs_tp), intent(inout) :: self      
+            !! RMVS test particle object
+         character(*),   intent(in)    :: sortby    
+            !! Sorting attribute
+         logical,        intent(in)    :: ascending 
+            !! Logical flag indicating whether or not the sorting should be in ascending or descending order
       end subroutine rmvs_util_sort_tp
 
       module subroutine rmvs_util_sort_rearrange_pl(self, ind)
          implicit none
-         class(rmvs_pl),               intent(inout) :: self !! RMVS massive body object
-         integer(I4B),   dimension(:), intent(in)    :: ind  !! Index array used to restructure the body (should contain all 1:n index values in the desired order)
+         class(rmvs_pl),               intent(inout) :: self 
+            !! RMVS massive body object
+         integer(I4B),   dimension(:), intent(in)    :: ind  
+            !! Index array used to restructure the body (should contain all 1:n index values in the desired order)
       end subroutine rmvs_util_sort_rearrange_pl
 
       module subroutine rmvs_util_sort_rearrange_tp(self, ind)
          implicit none
-         class(rmvs_tp),                intent(inout) :: self !! RMVS test particle object
-         integer(I4B),    dimension(:), intent(in)    :: ind  !! Index array used to restructure the body (should contain all 1:n index values in the desired order)
+         class(rmvs_tp),                intent(inout) :: self 
+            !! RMVS test particle object
+         integer(I4B),    dimension(:), intent(in)    :: ind  
+            !! Index array used to restructure the body (should contain all 1:n index values in the desired order)
       end subroutine rmvs_util_sort_rearrange_tp
 
       module subroutine rmvs_util_spill_pl(self, discards, lspill_list, ldestructive)
          implicit none
-         class(rmvs_pl),        intent(inout) :: self         !! RMVS massive body object
-         class(swiftest_body),  intent(inout) :: discards     !! Discarded object 
-         logical, dimension(:), intent(in)    :: lspill_list  !! Logical array of bodies to spill into the discards
-         logical,               intent(in)    :: ldestructive !! Logical flag indicating whether or not this operation should alter the keeps array or not
+         class(rmvs_pl),        intent(inout) :: self         
+            !! RMVS massive body object
+         class(swiftest_body),  intent(inout) :: discards     
+            !! Discarded object 
+         logical, dimension(:), intent(in)    :: lspill_list  
+            !! Logical array of bodies to spill into the discards
+         logical,               intent(in)    :: ldestructive 
+            !! Logical flag indicating whether or not this operation should alter the keeps array or not
       end subroutine rmvs_util_spill_pl
 
       module subroutine rmvs_util_spill_tp(self, discards, lspill_list, ldestructive)
          implicit none
-         class(rmvs_tp),        intent(inout) :: self         !! RMVS test particle object
-         class(swiftest_body),  intent(inout) :: discards     !! Discarded object 
-         logical, dimension(:), intent(in)    :: lspill_list  !! Logical array of bodies to spill into the discards
-         logical,               intent(in)    :: ldestructive !! Logical flag indicating whether or not this operation should alter the keeps array or not
+         class(rmvs_tp),        intent(inout) :: self         
+            !! RMVS test particle object
+         class(swiftest_body),  intent(inout) :: discards     
+            !! Discarded object 
+         logical, dimension(:), intent(in)    :: lspill_list  
+            !! Logical array of bodies to spill into the discards
+         logical,               intent(in)    :: ldestructive 
+            !! Logical flag indicating whether or not this operation should alter the keeps array or not
       end subroutine rmvs_util_spill_tp
 
       module subroutine rmvs_step_system(self, param, t, dt)
          implicit none
-         class(rmvs_nbody_system),   intent(inout) :: self    !! RMVS nbody system object
-         class(swiftest_parameters), intent(inout) :: param  !! Current run configuration parameters 
-         real(DP),                   intent(in)    :: t      !! Simulation time
-         real(DP),                   intent(in)    :: dt     !! Current stepsize
+         class(rmvs_nbody_system),   intent(inout) :: self    
+            !! RMVS nbody system object
+         class(swiftest_parameters), intent(inout) :: param  
+            !! Current run configuration parameters 
+         real(DP),                   intent(in)    :: t      
+            !! Simulation time
+         real(DP),                   intent(in)    :: dt     
+            !! Current stepsize
       end subroutine rmvs_step_system
 
    end interface
 
 
 #ifdef COARRAY
    interface coclone
-      module subroutine rmvs_coarray_component_clone_interp_arr1D(var,src_img)
-         implicit none
-         type(rmvs_interp), dimension(:), allocatable, intent(inout) :: var
-         integer(I4B), intent(in),optional :: src_img
-      end subroutine rmvs_coarray_component_clone_interp_arr1D
+      module procedure rmvs_coarray_coclone_tp
    end interface
 
    interface cocollect
-      module subroutine rmvs_coarray_cocollect_tp(self)
-         implicit none
-         class(rmvs_tp),intent(inout),codimension[*]  :: self  !! RMVS pl object
-      end subroutine rmvs_coarray_cocollect_tp
+      module procedure rmvs_coarray_cocollect_tp
    end interface
 
-   interface
-      module subroutine rmvs_coarray_coclone_cb(self)
-         implicit none
-         class(rmvs_cb),intent(inout),codimension[*]  :: self  !! RMVS tp object
-      end subroutine rmvs_coarray_coclone_cb
-
-      module subroutine rmvs_coarray_coclone_interp(self)
-         implicit none
-         class(rmvs_interp),intent(inout),codimension[*]  :: self  !! RMVS tp object
-      end subroutine rmvs_coarray_coclone_interp
-
-      module subroutine rmvs_coarray_coclone_pl(self)
-         implicit none
-         class(rmvs_pl),intent(inout),codimension[*]  :: self  !! RMVS pl object
-      end subroutine rmvs_coarray_coclone_pl
-
-      module subroutine rmvs_coarray_coclone_system(self)
-         implicit none
-         class(rmvs_nbody_system),intent(inout),codimension[*]  :: self  !! RMVS nbody system object
-      end subroutine rmvs_coarray_coclone_system
-
-      module subroutine rmvs_coarray_coclone_tp(self)
-         implicit none
-         class(rmvs_tp),intent(inout),codimension[*]  :: self  !! RMVS tp object
-      end subroutine rmvs_coarray_coclone_tp
-   end interface
 #endif
 
    contains
 
       subroutine rmvs_final_cb(self)
          !! author: David A. Minton
          !!
          !! Finalize the RMVS massive body object - deallocates all allocatables
          implicit none
          ! Arguments
-         type(rmvs_cb),  intent(inout) :: self !! RMVS central body object
-
+         type(rmvs_cb),  intent(inout) :: self 
+            !! RMVS central body object
          call self%dealloc()
-
          return
       end subroutine rmvs_final_cb
 
 
       subroutine rmvs_final_interp(self)
          !! author: David A. Minton
          !!
          !! Finalize the RMVS nbody system object - deallocates all allocatables
          implicit none
          ! Arguments
-         type(rmvs_interp),  intent(inout) :: self !! RMVS nbody system object
-
+         type(rmvs_interp),  intent(inout) :: self 
+            !! RMVS nbody system object
          call self%dealloc()
-
          return
       end subroutine rmvs_final_interp
 
 
       subroutine rmvs_final_pl(self)
          !! author: David A. Minton
          !!
          !! Finalize the RMVS massive body object - deallocates all allocatables
          implicit none
          ! Arguments
-         type(rmvs_pl),  intent(inout) :: self !! RMVS massive body object
-
+         type(rmvs_pl),  intent(inout) :: self 
+            !! RMVS massive body object
          call self%dealloc()
-
          return
       end subroutine rmvs_final_pl
 
 
       subroutine rmvs_final_tp(self)
          !! author: David A. Minton
          !!
          !! Finalize the RMVS test particle object - deallocates all allocatables
          implicit none
          ! Arguments
-         type(rmvs_tp),  intent(inout) :: self !! RMVS test particle object
-
+         type(rmvs_tp),  intent(inout) :: self 
+            !! RMVS test particle object
          call self%dealloc()
-
          return
       end subroutine rmvs_final_tp
 
 
+#ifdef COARRAY
+
+   subroutine rmvs_coarray_coclone_tp(tp)
+      !! author: David A. Minton
+      !!
+      !! Broadcasts the image 1 object to all other images in a coarray 
+      implicit none
+      ! Arguments
+      type(rmvs_tp),intent(inout),codimension[*]  :: tp  !! RMVS pl object
+
+      call coclone(tp%lperi)
+      call coclone(tp%plperP) 
+      call coclone(tp%plencP)
+      call co_broadcast(tp%index,1)
+      call co_broadcast(tp%ipleP,1)
+      call co_broadcast(tp%lplanetocentric,1)
+
+      call coclone(tp%whm_tp)
+
+      return
+   end subroutine rmvs_coarray_coclone_tp
+
+
+   subroutine rmvs_coarray_cocollect_tp(tp)
+      !! author: David A. Minton
+      !!
+      !! Broadcasts the image 1 object to all other images in a coarray 
+      implicit none
+      ! Arguments
+      type(rmvs_tp),intent(inout),codimension[*]  :: tp  !! RMVS pl object
+
+      call cocollect(tp%lperi)
+      call cocollect(tp%plperP) 
+      call cocollect(tp%plencP)
+
+      call cocollect(tp%whm_tp)
+
+      return
+   end subroutine rmvs_coarray_cocollect_tp
+
+#endif 
+
+
 end module rmvs
```

### Comparing `swiftest-2024.4.1/src/rmvs/rmvs_step.f90` & `swiftest-2024.4.2/src/rmvs/rmvs_step.f90`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                         tp%lmask(1:ntp) = .not. tp%lmask(1:ntp)
                         call pl%set_beg_end(rbeg = rbeg, rend = rend)
                         tp%lfirst = .true.
                         call tp%step(nbody_system, param, t, dt)
                         tp%lmask(1:ntp) = .true.
                         pl%lfirst = lfirstpl
                         tp%lfirst = .true.
-                        ! if (param%ltides) call nbody_system%step_spin(param, t, dt)
+                        ! if (param%ltides) call nbody_system%step_rot(param, t, dt)
                      else
                         call whm_step_system(nbody_system, param, t, dt)
                      end if
                   end associate
                end select
             end select
          end select
```

### Comparing `swiftest-2024.4.1/src/rmvs/rmvs_util.f90` & `swiftest-2024.4.2/src/rmvs/rmvs_util.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/shgrav/shgrav_accel.f90` & `swiftest-2024.4.2/src/shgrav/shgrav_accel.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/shgrav/shgrav_module.f90` & `swiftest-2024.4.2/src/shgrav/shgrav_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/swiftest/swiftest_discard.f90` & `swiftest-2024.4.2/src/swiftest/swiftest_discard.f90`

 * *Files 11% similar despite different names*

```diff
@@ -13,311 +13,319 @@
    module subroutine swiftest_discard_system(self, param)
       !! author: David A. Minton
       !!
       !! Calls the discard methods for each body class and then the write method if any discards were detected
       !!
       implicit none
       ! Arguments
-      class(swiftest_nbody_system), intent(inout) :: self   !! Swiftest nbody_system object
-      class(swiftest_parameters),   intent(inout) :: param  !! Current run configuration parameters
+      class(swiftest_nbody_system), intent(inout) :: self   
+         !! Swiftest nbody_system object
+      class(swiftest_parameters),   intent(inout) :: param  
+         !! Current run configuration parameters
       ! Internals
-      logical :: lpl_discards, ltp_discards, lpl_check, ltp_check
-      logical, dimension(:), allocatable :: ldiscard
-      integer(I4B) :: i, nstart, nend, nsub
-      character(len=STRMAX) :: idstr
-      class(swiftest_pl), allocatable :: plsub
-      class(swiftest_tp), allocatable :: tpsub
+      logical :: lpl_check, ltp_check
+      logical :: ldiscard_pl = .false. 
+      logical :: ldiscard_tp = .false.
+
+      integer(I4B) :: i
 
       lpl_check = allocated(self%pl_discards) .and. self%pl%nbody > 0
       ltp_check = allocated(self%tp_discards) .and. self%tp%nbody > 0
 
-      associate(nbody_system => self,tp => self%tp,pl => self%pl,tp_discards => self%tp_discards,pl_discards => self%pl_discards, &
-               npl => self%pl%nbody, ntp => self%tp%nbody, t => self%t, collision_history => self%collision_history, &
-               collider => self%collider)
-         lpl_discards = .false.
-         ltp_discards = .false.
-         if (lpl_check .and. pl%nbody > 0) then
-            pl%ldiscard = pl%status(:) /= ACTIVE
+      associate(nbody_system => self,&
+                tp => self%tp, &
+                pl => self%pl,&
+                npl => self%pl%nbody, &
+                ntp => self%tp%nbody)
+         if (lpl_check .and. npl > 0) then
             call pl%discard(nbody_system, param)
-            if (npl > 0) lpl_discards = any(pl%ldiscard(1:npl))
+            ldiscard_pl = any(pl%ldiscard(:))
          end if
             
-         if (ltp_check .and. tp%nbody > 0) then
-            tp%ldiscard = tp%status(:) /= ACTIVE
+         if (ltp_check .and. ntp > 0) then
             call tp%discard(nbody_system, param)
-            if (ntp > 0) ltp_discards = any(tp%ldiscard(1:ntp))
-            if (npl > 0) lpl_discards = any(pl%ldiscard(1:npl))
+            ldiscard_tp = any(tp%ldiscard(:)) 
          end if
 
-         if (ltp_discards.or.lpl_discards) then
-            ! Advance the collision id number and save it
-            collider%maxid_collision = collider%maxid_collision + 1
-            collider%collision_id = collider%maxid_collision
-            collider%impactors%regime = COLLRESOLVE_REGIME_MERGE
-            write(idstr,*) collider%collision_id
-            call swiftest_io_log_one_message(COLLISION_LOG_OUT, "collision_id " // trim(adjustl(idstr)))
-
-            if (ltp_discards) then
-               allocate(ldiscard, source=tp%ldiscard(:))
-               do i = 1, ntp
-                  if (ldiscard(i)) call tp%info(i)%set_value(collision_id=collider%collision_id)
-               end do
-               allocate(tpsub, mold=tp)
-               call tp%spill(tpsub, ldiscard, ldestructive=.true.)
-               nsub = tpsub%nbody
-               nstart = tp_discards%nbody + 1
-               nend = tp_discards%nbody + nsub
-               call tp_discards%append(tpsub, lsource_mask=[(.true., i = 1, nsub)])
-               deallocate(ldiscard)
-               select type(before => collider%before)
-               class is (swiftest_nbody_system)
-                  if (allocated(before%tp)) deallocate(before%tp)
-                  allocate(before%tp, source=tp_discards)
-               end select
-               call tp_discards%setup(0,param) 
-            end if
-
-            if (lpl_discards) then ! In the base integrators, massive bodies are not true discards. The discard is 
-                                              ! simply used to trigger a snapshot.
-               if (param%lenergy) call self%conservation_report(param, lterminal=.false.)
-               allocate(ldiscard, source=pl%ldiscard(:))
-               do i = 1, npl
-                  if (ldiscard(i)) call pl%info(i)%set_value(collision_id=collider%collision_id)
-               end do
-               allocate(plsub, mold=pl)
-               call pl%spill(plsub, ldiscard, ldestructive=.false.)
-               nsub = plsub%nbody
-               nstart = pl_discards%nbody + 1
-               nend = pl_discards%nbody + nsub
-               call pl_discards%append(plsub, lsource_mask=[(.true., i = 1, nsub)])
-               deallocate(ldiscard)
-               pl%ldiscard(1:npl) = .false.
-               ! Save the before snapshots
-               select type(before => collider%before)
-               class is (swiftest_nbody_system)
-                  if (allocated(before%pl)) deallocate(before%pl)
-                  allocate(before%pl, source=pl_discards)
-               end select
-               call pl_discards%setup(0,param) 
-            end if
-
-
-            call collision_history%take_snapshot(param,nbody_system, t, "particle") 
-         end if
-         
+         if (ldiscard_pl) call pl%rearray(nbody_system, param) 
+         if (ldiscard_tp) call tp%rearray(nbody_system, param)
       end associate
 
       return
    end subroutine swiftest_discard_system
 
 
    module subroutine swiftest_discard_pl(self, nbody_system, param)
       !! author: David A. Minton
       !!
       !! Placeholder method for discarding massive bodies. This method does nothing except to ensure that the discard flag is set 
       !! to false. This method is intended to be overridden by more advanced integrators.
       implicit none
       ! Arguments
-      class(swiftest_pl),           intent(inout) :: self   !! Swiftest massive body object
-      class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(swiftest_parameters),   intent(inout) :: param  !! Current run configuration parameter
+      class(swiftest_pl),           intent(inout) :: self   
+         !! Swiftest massive body object
+      class(swiftest_nbody_system), intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(swiftest_parameters),   intent(inout) :: param  
+         !! Current run configuration parameter
 
       if (self%nbody == 0) return
-      self%ldiscard(1:self%nbody) = .false.
+      associate(pl => self, cb => nbody_system%cb)
+         pl%ldiscard = pl%status(:) /= ACTIVE
+         if ((param%rmin >= 0.0_DP) .or. (param%rmax >= 0.0_DP) .or. &
+             (param%rmaxu >= 0.0_DP) .or. ((param%qmin >= 0.0_DP) .and. (param%qmin_coord == "BARY"))) call pl%h2b(cb) 
+
+         if ((param%rmin >= 0.0_DP) .or. &
+             (param%rmax >= 0.0_DP) .or. & 
+             (param%rmaxu >= 0.0_DP)) call swiftest_discard_cb_body(pl, nbody_system, param)
+         if (param%qmin >= 0.0_DP) call swiftest_discard_peri_body(pl, nbody_system, param)
+      end associate
 
       return
    end subroutine swiftest_discard_pl
 
 
    module subroutine swiftest_discard_tp(self, nbody_system, param)
       !! author: David A. Minton
       !!
       !! Check to see if particles should be discarded based on their positions relative to the massive bodies
       !! 
       !! Adapted from David E. Kaufmann's Swifter routine: discard.f90
       !! Adapted from Hal Levison's Swift routine discard.
       implicit none
       ! Arguments
-      class(swiftest_tp),           intent(inout) :: self   !! Swiftest test particle object
-      class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(swiftest_parameters),   intent(inout) :: param  !! Current run configuration parameter
+      class(swiftest_tp),           intent(inout) :: self   
+         !! Swiftest test particle object
+      class(swiftest_nbody_system), intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(swiftest_parameters),   intent(inout) :: param  
+         !! Current run configuration parameter
 
       if (self%nbody == 0) return
 
-      associate(tp => self, ntp => self%nbody, cb => nbody_system%cb, pl => nbody_system%pl, npl => nbody_system%pl%nbody, &
-                tp_discards => nbody_system%tp_discards, pl_discards => nbody_system%pl_discards)
-
+      associate(tp => self, cb => nbody_system%cb, pl => nbody_system%pl)
+         tp%ldiscard = tp%status(:) /= ACTIVE
          if ((param%rmin >= 0.0_DP) .or. (param%rmax >= 0.0_DP) .or. &
              (param%rmaxu >= 0.0_DP) .or. ((param%qmin >= 0.0_DP) .and. (param%qmin_coord == "BARY"))) then
             call pl%h2b(cb) 
             call tp%h2b(cb) 
          end if
 
          if ((param%rmin >= 0.0_DP) .or. &
              (param%rmax >= 0.0_DP) .or. & 
-             (param%rmaxu >= 0.0_DP)) then
-               call swiftest_discard_cb_tp(tp, nbody_system, param)
-         end if
-         if (param%qmin >= 0.0_DP) then
-            call swiftest_discard_peri_tp(tp, nbody_system, param)
-         end if
-         if (param%lclose) then
-            call swiftest_discard_pl_tp(tp, nbody_system, param)
-         end if
+             (param%rmaxu >= 0.0_DP)) call swiftest_discard_cb_body(tp, nbody_system, param)
+         if (param%qmin >= 0.0_DP) call swiftest_discard_peri_body(tp, nbody_system, param)
+         if (param%lclose) call swiftest_discard_pl_tp(tp, nbody_system, param)
       end associate
 
       return
    end subroutine swiftest_discard_tp
 
 
-   subroutine swiftest_discard_cb_tp(tp, nbody_system, param)
+   subroutine swiftest_discard_cb_body(body, nbody_system, param)
       !! author: David A. Minton
       !!
-      !!  Check to see if test particles should be discarded based on their positions relative to the Sun
-      !!        or because they are unbound from the nbody_system
+      !!  Check to see if bodies (massive or test particle) should be discarded based on their positions relative to the Sun or 
+      !!  because they are unbound from the nbody_system
       !!
       !! Adapted from David E. Kaufmann's Swifter routine: discard_sun.f90
       !! Adapted from Hal Levison's Swift routine discard_sun.f
       implicit none
       ! Arguments
-      class(swiftest_tp),           intent(inout) :: tp     !! Swiftest test particle object
-      class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(swiftest_parameters),   intent(in)    :: param  !! Current run configuration parameters
+      class(swiftest_body),         intent(inout) :: body   
+         !! Swiftest body object
+      class(swiftest_nbody_system), intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(swiftest_parameters),   intent(inout) :: param  
+         !! Current run configuration parameters
       ! Internals
-      integer(I4B)        :: i
+      integer(I4B)        :: i, nsub, nstart, nend
       real(DP)            :: energy, vb2, rb2, rh2, rmin2, rmax2, rmaxu2
       character(len=STRMAX) :: idstr, timestr, message
+      class(swiftest_tp), allocatable :: tpsub
+      logical, allocatable, dimension(:) :: ldiscard
+
+      associate(nbody => body%nbody, &
+                cb => nbody_system%cb, &
+                Gmtot => nbody_system%Gmtot, &
+                t => nbody_system%t, &
+                collider => nbody_system%collider, &
+                impactors => nbody_system%collider%impactors, &
+                collision_history => nbody_system%collision_history)
 
-      associate(ntp => tp%nbody, cb => nbody_system%cb, Gmtot => nbody_system%Gmtot)
          rmin2 = max(param%rmin * param%rmin, cb%radius * cb%radius)
          rmax2 = param%rmax**2
          rmaxu2 = param%rmaxu**2
-         do i = 1, ntp
-            if (tp%status(i) == ACTIVE) then
-               rh2 = dot_product(tp%rh(:, i), tp%rh(:, i))
+         do i = 1, nbody
+            if (body%status(i) == ACTIVE) then
+               rh2 = dot_product(body%rh(:, i), body%rh(:, i))
                if ((param%rmax >= 0.0_DP) .and. (rh2 > rmax2)) then
-                  tp%status(i) = DISCARDED_RMAX
-                  write(idstr, *) tp%id(i)
-                  write(timestr, *) nbody_system%t
-                  write(message, *) "Particle " // trim(adjustl(tp%info(i)%name)) // " ("  // trim(adjustl(idstr)) // ")" // &
+                  body%status(i) = DISCARDED_RMAX
+                  write(idstr, *) body%id(i)
+                  write(timestr, *) t
+                  write(message, *) "Body " // trim(adjustl(body%info(i)%name)) // " ("  // trim(adjustl(idstr)) // ")" // &
                               " too far from the central body at t = " // trim(adjustl(timestr))
                   call swiftest_io_log_one_message(COLLISION_LOG_OUT, message)
-                  tp%ldiscard(i) = .true.
-                  tp%lmask(i) = .false.
-                  call tp%info(i)%set_value(status="DISCARDED_RMAX", discard_time=nbody_system%t, discard_rh=tp%rh(:,i), &
-                                            discard_vh=tp%vh(:,i))
+                  body%ldiscard(i) = .true.
+                  body%lmask(i) = .false.
+                  call body%info(i)%set_value(status="DISCARDED_RMAX", discard_time=nbody_system%t, discard_rh=body%rh(:,i), &
+                                            discard_vh=body%vh(:,i))
+                  impactors%regime = REGIME_EJECTED 
                else if ((param%rmin >= 0.0_DP) .and. (rh2 < rmin2)) then
-                  tp%status(i) = DISCARDED_RMIN
-                  write(idstr, *) tp%id(i)
-                  write(timestr, *) nbody_system%t
-                  write(message, *) "Particle " // trim(adjustl(tp%info(i)%name)) // " ("  // trim(adjustl(idstr)) // ")" // &
+                  body%status(i) = DISCARDED_RMIN
+                  write(idstr, *) body%id(i)
+                  write(timestr, *) t
+                  write(message, *) "Body " // trim(adjustl(body%info(i)%name)) // " ("  // trim(adjustl(idstr)) // ")" // &
                               " too close to the central body at t = " // trim(adjustl(timestr))
                   call swiftest_io_log_one_message(COLLISION_LOG_OUT, message)
-                  tp%ldiscard(i) = .true.
-                  tp%lmask(i) = .false.
-                  call tp%info(i)%set_value(status="DISCARDED_RMIN", discard_time=nbody_system%t, discard_rh=tp%rh(:,i), &
-                                            discard_vh=tp%vh(:,i), discard_body_id=cb%id)
+                  body%ldiscard(i) = .true.
+                  body%lmask(i) = .false.
+                  call body%info(i)%set_value(status="DISCARDED_RMIN", discard_time=nbody_system%t, discard_rh=body%rh(:,i), &
+                                            discard_vh=body%vh(:,i), discard_body_id=cb%id)
+                  impactors%regime = REGIME_CB_IMPACT
                else if (param%rmaxu >= 0.0_DP) then
-                  rb2 = dot_product(tp%rb(:, i),  tp%rb(:, i))
-                  vb2 = dot_product(tp%vb(:, i), tp%vb(:, i))
+                  rb2 = dot_product(body%rb(:, i),  body%rb(:, i))
+                  vb2 = dot_product(body%vb(:, i), body%vb(:, i))
                   energy = 0.5_DP * vb2 - Gmtot / sqrt(rb2)
                   if ((energy > 0.0_DP) .and. (rb2 > rmaxu2)) then
-                     tp%status(i) = DISCARDED_RMAXU
-                     write(idstr, *) tp%id(i)
-                     write(timestr, *) nbody_system%t
-                     write(message, *) "Particle " // trim(adjustl(tp%info(i)%name)) // " ("  // trim(adjustl(idstr)) // ")" // &
+                     body%status(i) = DISCARDED_RMAXU
+                     write(idstr, *) body%id(i)
+                     write(timestr, *) t
+                     write(message, *) "Body " // trim(adjustl(body%info(i)%name)) // " ("  // trim(adjustl(idstr)) // ")" // &
                                  " is unbound and too far from barycenter at t = " // trim(adjustl(timestr))
                      call swiftest_io_log_one_message(COLLISION_LOG_OUT, message)
-                     tp%ldiscard(i) = .true.
-                     tp%lmask(i) = .false.
-                     call tp%info(i)%set_value(status="DISCARDED_RMAXU", discard_time=nbody_system%t, discard_rh=tp%rh(:,i), &
-                                               discard_vh=tp%vh(:,i))
+                     body%ldiscard(i) = .true.
+                     body%lmask(i) = .false.
+                     call body%info(i)%set_value(status="DISCARDED_RMAXU", discard_time=nbody_system%t, discard_rh=body%rh(:,i), &
+                                               discard_vh=body%vh(:,i))
+                     impactors%regime = REGIME_EJECTED
                   end if
                end if
+
+               ! Save the system snapshot
+               if (body%ldiscard(i)) then
+                  allocate(ldiscard, mold=body%ldiscard(:))
+                  ldiscard(:) = .false.
+                  ldiscard(i) = .true.
+                  call body%save_discard(ldiscard,nbody_system,collider%before)
+                  ! The base class doesn't do a before/after comparison, so we just save the before snapshot
+                  call collision_history%take_snapshot(param,nbody_system, t, "particle") 
+               end if
             end if
          end do
       end associate
 
       return
-   end subroutine swiftest_discard_cb_tp
+   end subroutine swiftest_discard_cb_body
 
 
-   subroutine swiftest_discard_peri_tp(tp, nbody_system, param)
+   subroutine swiftest_discard_peri_body(body, nbody_system, param)
       !! author: David A. Minton
       !!
-      !! Check to see if a test particle should be discarded because its perihelion distance becomes too small
+      !! Check to see if a body (massive or test particle) should be discarded because its perihelion distance becomes too small
       !!
       !! Adapted from David E. Kaufmann's Swifter routine: discard_peri.f90
       !! Adapted from Hal Levison's Swift routine discard_peri.f
       implicit none
       ! Arguments
-      class(swiftest_tp),           intent(inout) :: tp   !! Swiftest test particle object
-      class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(swiftest_parameters),   intent(in)    :: param  !! Current run configuration parameterss
+      class(swiftest_body),         intent(inout) :: body 
+         !! Swiftest body object
+      class(swiftest_nbody_system), intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(swiftest_parameters),   intent(inout) :: param  
+         !! Current run configuration parameterss
       ! Internals
       integer(I4B)              :: i, j, ih
       real(DP)                  :: r2
       real(DP), dimension(NDIM) :: dx
       character(len=STRMAX) :: idstr, timestr, message
+      logical, allocatable, dimension(:) :: ldiscard
    
-      associate(cb => nbody_system%cb, ntp => tp%nbody, pl => nbody_system%pl, npl => nbody_system%pl%nbody, t => nbody_system%t)
-         call tp%get_peri(nbody_system, param)
-         do i = 1, ntp
-            if (tp%status(i) == ACTIVE) then
-               if (tp%isperi(i) == 0) then
+      associate(cb => nbody_system%cb, &
+                nbody => body%nbody, &
+                pl => nbody_system%pl, &
+                npl => nbody_system%pl%nbody, &
+                t => nbody_system%t, &
+                collider => nbody_system%collider, &
+                impactors => nbody_system%collider%impactors, &
+                collision_history => nbody_system%collision_history)
+         call body%get_peri(nbody_system, param)
+         do i = 1, nbody
+            if (body%status(i) == ACTIVE) then
+               if (body%isperi(i) == 0) then
+                  ! Check to make sure the body isn't too close to any of the planets, as this case will be handled elsewhere
                   ih = 1
                   do j = 1, npl
-                     dx(:) = tp%rh(:, i) - pl%rh(:, j)
+                     dx(:) = body%rh(:, i) - pl%rh(:, j)
                      r2 = dot_product(dx(:), dx(:))
                      if (r2 <= (pl%rhill(j))**2) ih = 0
                   end do
                   if (ih == 1) then
-                     if ((tp%atp(i) >= param%qmin_alo) .and.    &
-                        (tp%atp(i) <= param%qmin_ahi) .and.    &           
-                        (tp%peri(i) <= param%qmin)) then
-                        tp%status(i) = DISCARDED_PERI
-                        write(idstr, *) tp%id(i)
+                     if ((body%atp(i) >= param%qmin_alo) .and.    &
+                        (body%atp(i) <= param%qmin_ahi) .and.    &           
+                        (body%peri(i) <= param%qmin)) then
+                        body%status(i) = DISCARDED_PERI
+                        write(idstr, *) body%id(i)
                         write(timestr, *) nbody_system%t
-                        write(message, *) "Particle " // trim(adjustl(tp%info(i)%name)) // " ("  // trim(adjustl(idstr)) // ")" // &
+                        write(message, *) "Body " // trim(adjustl(body%info(i)%name)) // " ("  // trim(adjustl(idstr)) // ")" // &
                                     " perihelion distance too small at t = " // trim(adjustl(timestr))
                         
                         call swiftest_io_log_one_message(COLLISION_LOG_OUT, message)
-                        tp%ldiscard(i) = .true.
-                        call tp%info(i)%set_value(status="DISCARDED_PERI", discard_time=nbody_system%t, discard_rh=tp%rh(:,i), &
-                                                  discard_vh=tp%vh(:,i), discard_body_id=cb%id)
+                        body%ldiscard(i) = .true.
+                        call body%info(i)%set_value(status="DISCARDED_PERI", discard_time=nbody_system%t, discard_rh=body%rh(:,i), &
+                                                  discard_vh=body%vh(:,i), discard_body_id=cb%id)
+
+                        ! Save the system snapshot
+                        impactors%regime = REGIME_CB_IMPACT
+                        allocate(ldiscard, mold=body%ldiscard(:))
+                        ldiscard(:) = .false.
+                        ldiscard(i) = .true.
+                        call body%save_discard(ldiscard,nbody_system,collider%before)
+                        call collision_history%take_snapshot(param,nbody_system, t, "particle") 
                      end if
                   end if
                end if
             end if
          end do
       end associate
 
       return
-   end subroutine swiftest_discard_peri_tp
+   end subroutine swiftest_discard_peri_body
 
 
    subroutine swiftest_discard_pl_tp(tp, nbody_system, param)
       !! author: David A. Minton
       !!
       !! Check to see if test particles should be discarded based on their positions relative to the massive bodies
       !!
       !! Adapted from David E. Kaufmann's Swifter routine: discard_pl.f90
       !! Adapted from Hal Levison's Swift routine discard_pl.f
       implicit none
       ! Arguments
-      class(swiftest_tp),           intent(inout) :: tp     !! Swiftest test particle object
-      class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(swiftest_parameters),   intent(in)    :: param  !! Current run configuration parameters
+      class(swiftest_tp),           intent(inout) :: tp     
+         !! Swiftest test particle object
+      class(swiftest_nbody_system), intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(swiftest_parameters),   intent(inout) :: param  
+         !! Current run configuration parameters
       ! Internals 
       integer(I4B)              :: i, j, isp
       real(DP)                  :: r2min, radius
       real(DP), dimension(NDIM) :: dx, dv
       character(len=STRMAX) :: idstri, idstrj, timestr, message
+      logical, allocatable, dimension(:) :: ldiscard_tp, ldiscard_pl
    
-      associate(ntp => tp%nbody, pl => nbody_system%pl, npl => nbody_system%pl%nbody, t => nbody_system%t, dt => param%dt)
+      associate(ntp => tp%nbody, &
+                pl => nbody_system%pl, &
+                npl => nbody_system%pl%nbody, &
+                t => nbody_system%t, &
+                dt => param%dt, &
+                collider => nbody_system%collider, &
+                impactors => nbody_system%collider%impactors, &
+                collision_history => nbody_system%collision_history)
          do i = 1, ntp
             if (tp%status(i) == ACTIVE) then
                do j = 1, npl
                   dx(:) = tp%rh(:, i) - pl%rh(:, j)
                   dv(:) = tp%vh(:, i) - pl%vh(:, j)
                   radius = pl%radius(j)
                   call swiftest_discard_pl_close(dx(:), dv(:), dt, radius**2, isp, r2min)
@@ -332,14 +340,29 @@
                                                    // "  too close to massive body " // trim(adjustl(pl%info(j)%name)) // " (" &
                                                    // trim(adjustl(idstrj)) // ")" &
                                                    // " at t = " // trim(adjustl(timestr))
                      call swiftest_io_log_one_message(COLLISION_LOG_OUT, message)
                      tp%ldiscard(i) = .true.
                      call tp%info(i)%set_value(status="DISCARDED_PLR", discard_time=nbody_system%t, discard_rh=tp%rh(:,i), &
                                                discard_vh=tp%vh(:,i), discard_body_id=pl%id(j))
+
+                     ! Save the system snapshot
+                     impactors%regime = COLLRESOLVE_REGIME_MERGE
+                     allocate(ldiscard_tp, mold=tp%ldiscard(:))
+                     allocate(ldiscard_Pl, mold=Pl%ldiscard(:))
+                     ldiscard_tp(:) = .false.
+                     ldiscard_pl(:) = .false.
+                     ldiscard_tp(i) = .true.
+                     ldiscard_pl(j) = .true.
+                     call tp%save_discard(ldiscard_pl,nbody_system,collider%before)
+                     call pl%save_discard(ldiscard_tp,nbody_system,collider%before)
+                     call collision_history%take_snapshot(param,nbody_system, t, "before") 
+                     call pl%save_discard(ldiscard_tp,nbody_system,collider%after)
+                     call collision_history%take_snapshot(param,nbody_system, t, "after") 
+
                      exit
                   end if
                end do
             end if
          end do
       end associate
 
@@ -353,18 +376,28 @@
       !!  Check to see if a test particle and massive body are having, or will have within the next time step, an encounter such
       !!          that the separation distance r is less than some critical radius rcrit (or r**2 < rcrit**2 = r2crit)
       !!
       !! Adapted from David E. Kaufmann's Swifter routine: discard_pl_close.f90
       !! Adapted from Hal Levison's Swift routine discard_pl_close.f
       implicit none
       ! Arguments
-      real(DP), dimension(:), intent(in)    :: dx, dv
-      real(DP), intent(in)                  :: dt, r2crit
-      integer(I4B), intent(out)             :: iflag
-      real(DP), intent(out)                 :: r2min
+      real(DP), dimension(:), intent(in)    :: dx
+         !! Difference in distance vectors
+      real(DP), dimension(:), intent(in)    :: dv 
+         !! Difference in velocity vectors
+      real(DP), intent(in)                  :: dt 
+         !! Time step
+      real(DP), intent(in)                  :: r2crit 
+         !! Square of the critical radius at which the test particle and massive body are considered to be in close proximity
+      integer(I4B), intent(out)             :: iflag 
+         !! Flag indicating whether the test particle and massive body are in close proximity. 
+         !! iflag == 1 means they are considered close
+         !! iflag == 0 means they are not considered close
+      real(DP), intent(out)                 :: r2min 
+         !! Minimum separation distance between the test particle and massive body within the next time step
       ! Internals
       real(DP) :: r2, v2, vdotr, tmin
       
       r2 = dot_product(dx(:), dx(:))
       if (r2 <= r2crit) then
          iflag = 1
       else
```

### Comparing `swiftest-2024.4.1/src/swiftest/swiftest_drift.f90` & `swiftest-2024.4.2/src/swiftest/swiftest_drift.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/swiftest/swiftest_driver.f90` & `swiftest-2024.4.2/src/swiftest/swiftest_driver.f90`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,21 @@
                                                                    !! {"STANDARD", "COMPACT", "PROGRESS"}). Default is "STANDARD"   
 
       ! Internals
       class(swiftest_nbody_system), allocatable :: nbody_system !! Polymorphic object containing the nbody system to be integrated
       type(swiftest_parameters)                 :: param             !! Run configuration parameters
       class(swiftest_storage),      allocatable :: system_history    !! Stores the system history between output dumps
       type(walltimer)                           :: integration_timer !! Object used for computing elapsed wall time
-
       !> Read in the user-defined parameters file and the initial conditions of the nbody_system
       param%integrator = trim(adjustl(integrator))
       param%display_style = trim(adjustl(display_style))
       call param%read_in(param_file_name)
-#ifdef COARRAY
+#ifdef COARRAY  
       if (.not.param%lcoarray .and. (this_image() /= 1)) stop ! Single image mode
+      sync all
 #endif
 
       associate(t0       => param%t0, &
          tstart          => param%tstart, &
          dt              => param%dt, &
          tstop           => param%tstop, &
          iloop           => param%iloop, &
@@ -82,16 +82,20 @@
          !$ nthreads = omp_get_max_threads() ! In the *parallel* case
 #ifdef COARRAY
          if (this_image() == 1 .or. param%log_output) then
 #endif 
             !$ write(param%display_unit,'(a)')   ' OpenMP parameters:'
             !$ write(param%display_unit,'(a)')   ' ------------------'
             !$ write(param%display_unit,'(a,i3,/)') ' Number of threads = ', nthreads 
-            !$ if (param%log_output) write(*,'(a,i3)') ' OpenMP: Number of threads = ',nthreads
 #ifdef COARRAY
+            if (this_image() ==1) then
+#endif
+               !$ if (param%log_output) write(*,'(a,i3)') ' OpenMP: Number of threads = ',nthreads
+#ifdef COARRAY
+            end if
             if (param%lcoarray) then
                write(param%display_unit,*)   ' Coarray parameters:'
                write(param%display_unit,*)   ' -------------------'
                write(param%display_unit,*) ' Number of images = ', num_images()
                if (param%log_output .and. this_image() == 1) write(*,'(a,i3)') ' Coarray: Number of images = ',num_images()
             else
                write(param%display_unit,*)   ' Coarrays disabled.'
@@ -100,15 +104,17 @@
          end if
 #endif 
          if (param%log_output) flush(param%display_unit)
 
 #ifdef COARRAY  
          ! The following line lets us read in the input files one image at a time. Letting each image read the input in is faster 
          ! than broadcasting all of the data
-         if (param%lcoarray .and. (this_image() /= 1)) sync images(this_image() - 1)
+         if (param%lcoarray) then
+            if (this_image() > 1) sync images(this_image() - 1)
+         end if
 #endif 
          call nbody_system%initialize(system_history, param)
 #ifdef COARRAY  
          if (param%lcoarray .and. (this_image() < num_images())) sync images(this_image() + 1)
 
          ! Distribute test particles to the various images
          if (param%lcoarray) call nbody_system%coarray_distribute(param)
@@ -163,24 +169,24 @@
 #endif
                   end if
 #ifdef COARRAY
                   if (this_image() == 1 .or. param%log_output) then
 #endif
                      call integration_timer%report(message="Integration steps:", unit=display_unit)
 #ifdef COARRAY  
-                  end if !(this_image() == 1)
+                  end if 
 #endif
                   call nbody_system%display_run_information(param, integration_timer)
                   call integration_timer%reset()
 #ifdef COARRAY
                   if (this_image() == 1 .or. param%log_output) then
 #endif
                      if (param%lenergy) call nbody_system%conservation_report(param, lterminal=.true.)
 #ifdef COARRAY
-                  end if ! (this_image() == 1)
+                  end if 
 #endif
                end if
             end if
 
          end do
          ! Dump any remaining history if it exists
          call nbody_system%dump(param, system_history)
```

### Comparing `swiftest-2024.4.1/src/swiftest/swiftest_gr.f90` & `swiftest-2024.4.2/src/swiftest/swiftest_gr.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/swiftest/swiftest_io.f90` & `swiftest-2024.4.2/src/swiftest/swiftest_io.f90`

 * *Files 1% similar despite different names*

```diff
@@ -24,18 +24,20 @@
          !!
          !! Formats a pair of variables and corresponding values for the compact display output. Generic interface for different 
          !! variable types to format.
          procedure :: fmt_I4B, fmt_I8B, fmt_DP
       end interface
 
       ! Arguments
-      class(swiftest_nbody_system), intent(in) :: self  !! Swiftest nbody system object   
-      class(swiftest_parameters),   intent(in) :: param !! Input colleciton of user-defined parameters
-      class(*),                     intent(in) :: timer !! Object used for computing elapsed wall time  (must be unlimited 
-                                                        !! polymorphic because the walltimer module requires base)
+      class(swiftest_nbody_system), intent(in) :: self  
+         !! Swiftest nbody system object   
+      class(swiftest_parameters),   intent(in) :: param 
+         !! Input colleciton of user-defined parameters
+      class(*),                     intent(in) :: timer 
+         !! Object used for computing elapsed wall time  (must be unlimited polymorphic because the walltimer module requires base)
       ! Internals
       character(len=:), allocatable :: formatted_output
 
       select type(timer)
       class is (walltimer)
          formatted_output = fmt("ILOOP",param%iloop) // fmt("T",self%t) // fmt("NPL",self%pl%nbody) // fmt("NTP",self%tp%nbody) 
          select type(pl => self%pl)
@@ -44,16 +46,16 @@
          end select
          if (param%lenergy) then
             formatted_output = formatted_output // fmt("LTOTERR",self%L_total_error) // fmt("ETOTERR",self%te_error) &
                              // fmt("MTOTERR",self%Mtot_error) // fmt("KEOERR",self%ke_orbit_error) // fmt("PEERR",self%pe_error) &
                              // fmt("EORBERR",self%E_orbit_error) // fmt("EUNTRERR",self%E_untracked_error) &
                              // fmt("LESCERR",self%L_escape_error) // fmt("MESCERR",self%Mescape_error)
             if (param%lclose) formatted_output = formatted_output // fmt("ECOLLERR",self%Ecoll_error)
-            if (param%lrotation) formatted_output = formatted_output // fmt("KESPINERR",self%ke_spin_error) &
-                             // fmt("LSPINERR",self%L_spin_error) 
+            if (param%lrotation) formatted_output = formatted_output // fmt("KEROTERR",self%ke_rot_error) &
+                             // fmt("LROTERR",self%L_rot_error) 
          end if
 
          if (.not. timer%main_is_started) then ! This is the start of a new run
             formatted_output =  formatted_output // fmt("WT",0.0_DP) // fmt("IWT",0.0_DP) // fmt("WTPS",0.0_DP) 
          else
             formatted_output = formatted_output // fmt("WT",timer%wall_main) // fmt("IWT",timer%wall_step) &
                                                // fmt("WTPS",timer%wall_per_substep)
@@ -121,16 +123,16 @@
       !! Reports the current state of energy, mass, and angular momentum conservation in a run
       implicit none
       ! Arguments
       class(swiftest_nbody_system), intent(inout) :: self      !! Swiftest nbody system object
       class(swiftest_parameters),   intent(inout) :: param     !! Input colleciton of user-defined parameters
       logical,                      intent(in)    :: lterminal !! Indicates whether to output information to the terminal screen
       ! Internals
-      real(DP), dimension(NDIM)       :: L_total_now,  L_orbit_now,  L_spin_now
-      real(DP)                        :: ke_orbit_now,  ke_spin_now,  pe_now,  E_orbit_now, be_now, be_cb_now, be_cb_orig, te_now
+      real(DP), dimension(NDIM)       :: L_total_now,  L_orbit_now,  L_rot_now
+      real(DP)                        :: ke_orbit_now,  ke_rot_now,  pe_now,  E_orbit_now, be_now, be_cb_now, be_cb_orig, te_now
       real(DP)                        :: GMtot_now
       character(len=*), parameter     :: EGYTERMFMT = '(" DL/L0 = ", ES12.5, "; DE_orbit/|E0| = ", ES12.5,' &
                                                      //'"; DE_total/|E0| = ", ES12.5, "; DM/M0 = ", ES12.5)'
 
       associate(nbody_system => self, pl => self%pl, cb => self%cb, npl => self%pl%nbody, display_unit => param%display_unit)
 
          select type(self)
@@ -138,42 +140,42 @@
          class is (whm_nbody_system)
             call pl%vh2vb(cb)
          end select
          call pl%rh2rb(cb)
 
          call nbody_system%get_energy_and_momentum(param) 
          ke_orbit_now = nbody_system%ke_orbit
-         ke_spin_now = nbody_system%ke_spin
+         ke_rot_now = nbody_system%ke_rot
          pe_now = nbody_system%pe
          be_now = nbody_system%be
          be_cb_now = nbody_system%be_cb
          te_now = nbody_system%te
          L_orbit_now(:) = nbody_system%L_orbit(:)
-         L_spin_now(:) = nbody_system%L_spin(:)
+         L_rot_now(:) = nbody_system%L_rot(:)
          E_orbit_now = ke_orbit_now + pe_now
          L_total_now(:) = nbody_system%L_total(:) + nbody_system%L_escape(:)
          GMtot_now = nbody_system%GMtot + nbody_system%GMescape 
 
          if (param%lfirstenergy) then
             nbody_system%ke_orbit_orig = ke_orbit_now
-            nbody_system%ke_spin_orig = ke_spin_now
+            nbody_system%ke_rot_orig = ke_rot_now
             nbody_system%pe_orig = pe_now
             nbody_system%be_orig = be_now
             nbody_system%te_orig = te_now
             nbody_system%E_orbit_orig = E_orbit_now
             nbody_system%GMtot_orig = GMtot_now
             nbody_system%L_orbit_orig(:) = L_orbit_now(:)
-            nbody_system%L_spin_orig(:) = L_spin_now(:)
+            nbody_system%L_rot_orig(:) = L_rot_now(:)
             nbody_system%L_total_orig(:) = L_total_now(:)
             param%lfirstenergy = .false.
          end if
 
          if (.not.param%lfirstenergy) then 
             nbody_system%ke_orbit_error = (ke_orbit_now - nbody_system%ke_orbit_orig) / abs(nbody_system%te_orig)
-            nbody_system%ke_spin_error = (ke_spin_now - nbody_system%ke_spin_orig) / abs(nbody_system%te_orig)
+            nbody_system%ke_rot_error = (ke_rot_now - nbody_system%ke_rot_orig) / abs(nbody_system%te_orig)
             nbody_system%pe_error = (pe_now - nbody_system%pe_orig) / abs(nbody_system%te_orig)
 
             be_cb_orig = -(3 * cb%GM0**2 / param%GU) / (5 * cb%R0)
             nbody_system%be_error = (be_now - nbody_system%be_orig) / abs(nbody_system%te_orig) + (be_cb_now - be_cb_orig) & 
                                     / abs(nbody_system%te_orig)
 
             if (abs(nbody_system%E_orbit_orig) < 10*tiny(1.0_DP)) then
@@ -183,15 +185,15 @@
             end if
             nbody_system%Ecoll_error = nbody_system%E_collisions / abs(nbody_system%te_orig)
             nbody_system%E_untracked_error = nbody_system%E_untracked / abs(nbody_system%te_orig)
             nbody_system%te_error = (nbody_system%te - nbody_system%te_orig - nbody_system%E_collisions - nbody_system%E_untracked)&
                                    / abs(nbody_system%te_orig) + (be_cb_now - be_cb_orig) / abs(nbody_system%te_orig)
 
             nbody_system%L_orbit_error = norm2(L_orbit_now(:) - nbody_system%L_orbit_orig(:)) / norm2(nbody_system%L_total_orig(:))
-            nbody_system%L_spin_error = norm2(L_spin_now(:) - nbody_system%L_spin_orig(:)) / norm2(nbody_system%L_total_orig(:))
+            nbody_system%L_rot_error = norm2(L_rot_now(:) - nbody_system%L_rot_orig(:)) / norm2(nbody_system%L_total_orig(:))
             nbody_system%L_escape_error = norm2(nbody_system%L_escape(:)) / norm2(nbody_system%L_total_orig(:))
             nbody_system%L_total_error = norm2(L_total_now(:) - nbody_system%L_total_orig(:)) / norm2(nbody_system%L_total_orig(:))
 
             nbody_system%Mescape_error = nbody_system%GMescape / nbody_system%GMtot_orig
 #ifdef COARRAY
    if (this_image() == 1 .or. param%log_output) then
 #endif 
@@ -317,19 +319,20 @@
 #ifdef COARRAY
       if (this_image() == num_images() .or. param%log_output) then
 #endif
          if (phase_val == -1) then
             write(param%display_unit, *)" *************** Swiftest stop " // trim(adjustl(param%integrator)) // " *************** "
             if (param%display_style == "COMPACT") write(*,*) "SWIFTEST STOP" // trim(adjustl(param%integrator))
             if (param%log_output) close(param%display_unit)
+         else
+            if (param%log_output) flush(param%display_unit)
          end if
 
 #ifdef COARRAY
       end if ! this_image() == num_images()
-      if (param%log_output) flush(param%display_unit)
 #endif
 
       return
    end subroutine swiftest_io_display_run_information
 
 
    module subroutine swiftest_io_dump_param(self, param_file_name)
@@ -703,17 +706,17 @@
                               "netcdf_io_get_t0_values_system time_varid" )
 
          if (param%lenergy) then
             call netcdf_io_check( nf90_get_var(nc%id, nc%KE_orb_varid, rtemp, start=[tslot], count=[1]), & 
                                   "netcdf_io_get_t0_values_system KE_orb_varid" )
             self%ke_orbit_orig = rtemp(1)
 
-            call netcdf_io_check( nf90_get_var(nc%id, nc%KE_spin_varid, rtemp, start=[tslot], count=[1]), &
-                                 "netcdf_io_get_t0_values_system KE_spin_varid" )
-            self%ke_spin_orig = rtemp(1)
+            call netcdf_io_check( nf90_get_var(nc%id, nc%KE_rot_varid, rtemp, start=[tslot], count=[1]), &
+                                 "netcdf_io_get_t0_values_system KE_rot_varid" )
+            self%ke_rot_orig = rtemp(1)
 
             call netcdf_io_check( nf90_get_var(nc%id, nc%PE_varid, rtemp, start=[tslot], count=[1]), &
                                   "netcdf_io_get_t0_values_system PE_varid" )
             self%pe_orig = rtemp(1)
 
             call netcdf_io_check( nf90_get_var(nc%id, nc%BE_varid, rtemp, start=[tslot], count=[1]), &
                                   "netcdf_io_get_t0_values_system BE_varid" )
@@ -723,18 +726,18 @@
                                   "netcdf_io_get_t0_values_system TE_varid" )
             self%te_orig = rtemp(1)
 
             self%E_orbit_orig = self%ke_orbit_orig + self%pe_orig
 
             call netcdf_io_check( nf90_get_var(nc%id, nc%L_orbit_varid, self%L_orbit_orig(:), start=[1,tslot], count=[NDIM,1]), &
                                   "netcdf_io_get_t0_values_system L_orbit_varid" )
-            call netcdf_io_check( nf90_get_var(nc%id, nc%L_spin_varid, self%L_spin_orig(:), start=[1,tslot], count=[NDIM,1]), &
-                                  "netcdf_io_get_t0_values_system L_spin_varid" )
+            call netcdf_io_check( nf90_get_var(nc%id, nc%L_rot_varid, self%L_rot_orig(:), start=[1,tslot], count=[NDIM,1]), &
+                                  "netcdf_io_get_t0_values_system L_rot_varid" )
 
-            self%L_total_orig(:) = self%L_orbit_orig(:) + self%L_spin_orig(:) 
+            self%L_total_orig(:) = self%L_orbit_orig(:) + self%L_rot_orig(:) 
 
             call netcdf_io_check( nf90_get_var(nc%id, nc%Gmass_varid, vals, start=[1,tslot], count=[idmax,1]), &
                                   "netcdf_io_get_t0_values_system Gmass_varid" )
             call nc%get_valid_masks(plmask,tpmask)
             self%GMtot_orig = vals(1) + sum(vals(2:idmax), plmask(:))
 
             cb%GM0 = vals(1)
@@ -801,15 +804,14 @@
       use, intrinsic :: ieee_arithmetic
       implicit none
       ! Arguments
       class(swiftest_netcdf_parameters), intent(inout) :: self  !! Parameters used to for writing a NetCDF dataset to file
       class(swiftest_parameters),        intent(in)    :: param !! Current run configuration parameters 
       ! Internals
       integer(I4B) :: nvar, varid, vartype
-      integer(I4B) :: status
       real(DP) :: dfill
       real(SP) :: sfill
       integer(I4B), parameter :: NO_FILL = 0
       logical :: fileExists
       character(len=STRMAX) :: errmsg
       integer(I4B) :: i, ndims
 
@@ -936,15 +938,15 @@
             call netcdf_io_check( nf90_def_var(nc%id, nc%origin_rh_varname, nc%out_type, [nc%space_dimid, nc%name_dimid], &
                                                nc%origin_rh_varid), &
                                   "netcdf_io_initialize_output nf90_def_var origin_rh_varid"  )
             call netcdf_io_check( nf90_def_var(nc%id, nc%origin_vh_varname, nc%out_type, [nc%space_dimid, nc%name_dimid], &
                                                nc%origin_vh_varid), &
                                   "netcdf_io_initialize_output nf90_def_var origin_vh_varid"  )
 
-            call netcdf_io_check( nf90_def_var(nc%id, nc%collision_id_varname, NF90_INT, nc%name_dimid, nc%collision_id_varid), &
+            call netcdf_io_check( nf90_def_var(nc%id, nc%collision_id_dimname, NF90_INT, nc%name_dimid, nc%collision_id_varid), &
                                   "netcdf_io_initialize_output nf90_def_var collision_id_varid"  )
             call netcdf_io_check( nf90_def_var(nc%id, nc%discard_time_varname, nc%out_type, nc%name_dimid, nc%discard_time_varid), &
                                   "netcdf_io_initialize_output nf90_def_var discard_time_varid"  )
             call netcdf_io_check( nf90_def_var(nc%id, nc%discard_rh_varname, nc%out_type, [nc%space_dimid, nc%name_dimid], &
                                                nc%discard_rh_varid), &
                                   "netcdf_io_initialize_output nf90_def_var discard_rh_varid"  )
             call netcdf_io_check( nf90_def_var(nc%id, nc%discard_vh_varname, nc%out_type, [nc%space_dimid, nc%name_dimid], &
@@ -994,30 +996,30 @@
          !    call netcdf_io_check( nf90_def_var(nc%id, nc%k2_varname, nc%out_type, [nc%name_dimid, nc%time_dimid], nc%k2_varid), &
          !                        "netcdf_io_initialize_output nf90_def_var k2_varid"  )
          !    call netcdf_io_check( nf90_def_var(nc%id, nc%q_varname, nc%out_type, [nc%name_dimid, nc%time_dimid], nc%Q_varid), &
          !                        "netcdf_io_initialize_output nf90_def_var Q_varid"  )
          ! end if
 
          if (param%lenergy) then
-            call netcdf_io_check( nf90_def_var(nc%id, nc%ke_orb_varname, nc%out_type, nc%time_dimid, nc%KE_orb_varid), &
+            call netcdf_io_check( nf90_def_var(nc%id, nc%ke_orbit_varname, nc%out_type, nc%time_dimid, nc%KE_orb_varid), &
                                   "netcdf_io_initialize_output nf90_def_var KE_orb_varid"  )
-            call netcdf_io_check( nf90_def_var(nc%id, nc%ke_spin_varname, nc%out_type, nc%time_dimid, nc%KE_spin_varid), &
-                                  "netcdf_io_initialize_output nf90_def_var KE_spin_varid"  )
+            call netcdf_io_check( nf90_def_var(nc%id, nc%ke_rot_varname, nc%out_type, nc%time_dimid, nc%KE_rot_varid), &
+                                  "netcdf_io_initialize_output nf90_def_var KE_rot_varid"  )
             call netcdf_io_check( nf90_def_var(nc%id, nc%pe_varname, nc%out_type, nc%time_dimid, nc%PE_varid), &
                                   "netcdf_io_initialize_output nf90_def_var PE_varid"  )
             call netcdf_io_check( nf90_def_var(nc%id, nc%be_varname, nc%out_type, nc%time_dimid, nc%BE_varid), &
                                   "netcdf_io_initialize_output nf90_def_var BE_varid"  )
             call netcdf_io_check( nf90_def_var(nc%id, nc%te_varname, nc%out_type, nc%time_dimid, nc%TE_varid), &
                                   "netcdf_io_initialize_output nf90_def_var TE_varid"  )
             call netcdf_io_check( nf90_def_var(nc%id, nc%L_orbit_varname, nc%out_type, [nc%space_dimid, nc%time_dimid], &
                                                nc%L_orbit_varid), &
                                   "netcdf_io_initialize_output nf90_def_var L_orbit_varid"  )
-            call netcdf_io_check( nf90_def_var(nc%id, nc%L_spin_varname, nc%out_type, [nc%space_dimid, nc%time_dimid], &
-                                               nc%L_spin_varid), &
-                                  "netcdf_io_initialize_output nf90_def_var L_spin_varid"  )
+            call netcdf_io_check( nf90_def_var(nc%id, nc%L_rot_varname, nc%out_type, [nc%space_dimid, nc%time_dimid], &
+                                               nc%L_rot_varid), &
+                                  "netcdf_io_initialize_output nf90_def_var L_rot_varid"  )
             call netcdf_io_check( nf90_def_var(nc%id, nc%L_escape_varname, nc%out_type, [nc%space_dimid, nc%time_dimid], &
                                                nc%L_escape_varid), &
                                   "netcdf_io_initialize_output nf90_def_var L_escape_varid"  )
             call netcdf_io_check( nf90_def_var(nc%id, nc%E_collisions_varname, nc%out_type, nc%time_dimid, nc%E_collisions_varid), &
                                   "netcdf_io_initialize_output nf90_def_var E_collisions_varid"  )
             call netcdf_io_check( nf90_def_var(nc%id, nc%E_untracked_varname, nc%out_type, nc%time_dimid, nc%E_untracked_varid), &
                                   "netcdf_io_initialize_output nf90_def_var E_untracked_varid"  )
@@ -1235,29 +1237,29 @@
          if (param%lmtiny_pl) status = nf90_inq_varid(nc%id, nc%nplm_varname, nc%nplm_varid)
 
          if (param%lclose) then
             status = nf90_inq_varid(nc%id, nc%origin_type_varname, nc%origin_type_varid)
             status = nf90_inq_varid(nc%id, nc%origin_time_varname, nc%origin_time_varid)
             status = nf90_inq_varid(nc%id, nc%origin_rh_varname, nc%origin_rh_varid)
             status = nf90_inq_varid(nc%id, nc%origin_vh_varname, nc%origin_vh_varid)
-            status = nf90_inq_varid(nc%id, nc%collision_id_varname, nc%collision_id_varid)
+            status = nf90_inq_varid(nc%id, nc%collision_id_dimname, nc%collision_id_varid)
             status = nf90_inq_varid(nc%id, nc%discard_time_varname, nc%discard_time_varid)
             status = nf90_inq_varid(nc%id, nc%discard_rh_varname, nc%discard_rh_varid)
             status = nf90_inq_varid(nc%id, nc%discard_vh_varname, nc%discard_vh_varid)
             status = nf90_inq_varid(nc%id, nc%discard_body_id_varname, nc%discard_body_id_varid)
          end if
 
          if (param%lenergy) then
-            status = nf90_inq_varid(nc%id, nc%ke_orb_varname, nc%KE_orb_varid)
-            status = nf90_inq_varid(nc%id, nc%ke_spin_varname, nc%KE_spin_varid)
+            status = nf90_inq_varid(nc%id, nc%ke_orbit_varname, nc%KE_orb_varid)
+            status = nf90_inq_varid(nc%id, nc%ke_rot_varname, nc%KE_rot_varid)
             status = nf90_inq_varid(nc%id, nc%pe_varname, nc%PE_varid)
             status = nf90_inq_varid(nc%id, nc%be_varname, nc%BE_varid)
             status = nf90_inq_varid(nc%id, nc%te_varname, nc%TE_varid)
             status = nf90_inq_varid(nc%id, nc%L_orbit_varname, nc%L_orbit_varid)
-            status = nf90_inq_varid(nc%id, nc%L_spin_varname, nc%L_spin_varid)
+            status = nf90_inq_varid(nc%id, nc%L_rot_varname, nc%L_rot_varid)
             status = nf90_inq_varid(nc%id, nc%L_escape_varname, nc%L_escape_varid)
             status = nf90_inq_varid(nc%id, nc%E_collisions_varname, nc%E_collisions_varid)
             status = nf90_inq_varid(nc%id, nc%E_untracked_varname, nc%E_untracked_varid)
             status = nf90_inq_varid(nc%id, nc%GMescape_varname, nc%GMescape_varid)
          end if
 
          status = nf90_inq_varid(nc%id, nc%c_lm_varname, nc%c_lm_varid)
@@ -1686,37 +1688,37 @@
                                   "netcdf_io_read_hdr_system nf90_getvar nplm_varid"  )
             else
                self%pl%nplm = count(plmmask(:))
             end if
          end if
 
          if (param%lenergy) then
-            status = nf90_inq_varid(nc%id, nc%ke_orb_varname, nc%KE_orb_varid)
+            status = nf90_inq_varid(nc%id, nc%ke_orbit_varname, nc%KE_orb_varid)
             if (status == NF90_NOERR) call netcdf_io_check( nf90_get_var(nc%id, nc%KE_orb_varid, self%ke_orbit, start=[tslot]), &
                                   "netcdf_io_read_hdr_system nf90_getvar KE_orb_varid"  )
-            status = nf90_inq_varid(nc%id, nc%ke_spin_varname, nc%KE_spin_varid)
-            if (status == NF90_NOERR) call netcdf_io_check( nf90_get_var(nc%id, nc%KE_spin_varid, self%ke_spin, start=[tslot]), &
-                                  "netcdf_io_read_hdr_system nf90_getvar KE_spin_varid"  )
+            status = nf90_inq_varid(nc%id, nc%ke_rot_varname, nc%KE_rot_varid)
+            if (status == NF90_NOERR) call netcdf_io_check( nf90_get_var(nc%id, nc%KE_rot_varid, self%ke_rot, start=[tslot]), &
+                                  "netcdf_io_read_hdr_system nf90_getvar KE_rot_varid"  )
             status = nf90_inq_varid(nc%id, nc%pe_varname, nc%PE_varid)
             if (status == NF90_NOERR) call netcdf_io_check( nf90_get_var(nc%id, nc%PE_varid, self%pe, start=[tslot]), &
                                   "netcdf_io_read_hdr_system nf90_getvar PE_varid"  )
             status = nf90_inq_varid(nc%id, nc%be_varname, nc%BE_varid)
             if (status == NF90_NOERR) call netcdf_io_check( nf90_get_var(nc%id, nc%BE_varid, self%be, start=[tslot]), &
                                   "netcdf_io_read_hdr_system nf90_getvar BE_varid"  )
             status = nf90_inq_varid(nc%id, nc%te_varname, nc%TE_varid)
             if (status == NF90_NOERR) call netcdf_io_check( nf90_get_var(nc%id, nc%TE_varid, self%te, start=[tslot]), &
                                   "netcdf_io_read_hdr_system nf90_getvar TE_varid"  )
             status = nf90_inq_varid(nc%id, nc%L_orbit_varname, nc%L_orbit_varid)
             if (status == NF90_NOERR) call netcdf_io_check( nf90_get_var(nc%id, nc%L_orbit_varid, self%L_orbit(:), & 
                                                                          start=[1,tslot], count=[NDIM,1]), &
                                   "netcdf_io_read_hdr_system nf90_getvar L_orbit_varid"  )
-            status = nf90_inq_varid(nc%id, nc%L_spin_varname, nc%L_spin_varid)
-            if (status == NF90_NOERR) call netcdf_io_check( nf90_get_var(nc%id, nc%L_spin_varid, self%L_spin(:), start=[1,tslot], &
+            status = nf90_inq_varid(nc%id, nc%L_rot_varname, nc%L_rot_varid)
+            if (status == NF90_NOERR) call netcdf_io_check( nf90_get_var(nc%id, nc%L_rot_varid, self%L_rot(:), start=[1,tslot], &
                                                             count=[NDIM,1]), &
-                                  "netcdf_io_read_hdr_system nf90_getvar L_spin_varid"  )
+                                  "netcdf_io_read_hdr_system nf90_getvar L_rot_varid"  )
             status = nf90_inq_varid(nc%id, nc%L_escape_varname, nc%L_escape_varid)
             if (status == NF90_NOERR) call netcdf_io_check( nf90_get_var(nc%id, nc%L_escape_varid, self%L_escape(:), &
                                                                          start=[1, tslot], count=[NDIM,1]), &
                                   "netcdf_io_read_hdr_system nf90_getvar L_escape_varid"  )
             status = nf90_inq_varid(nc%id, nc%E_collisions_varname, nc%E_collisions_varid)
             if (status == NF90_NOERR) call netcdf_io_check( nf90_get_var(nc%id, nc%E_collisions_varid, self%E_collisions, &
                                                                          start=[tslot]), &
@@ -1896,15 +1898,15 @@
             do i = 1, npl
                call pl%info(i)%set_value(origin_vh=vectemp(:,plind(i)))
             end do
             do i = 1, ntp
                call tp%info(i)%set_value(origin_vh=vectemp(:,tpind(i)))
             end do
 
-            status = nf90_inq_varid(nc%id, nc%collision_id_varname, nc%collision_id_varid)
+            status = nf90_inq_varid(nc%id, nc%collision_id_dimname, nc%collision_id_varid)
             if (status == NF90_NOERR) then
                call netcdf_io_check( nf90_get_var(nc%id, nc%collision_id_varid, itemp), &
                                   "netcdf_io_read_particle_info_system nf90_getvar collision_id_varid"  )
                do i = 1, npl
                   call pl%info(i)%set_value(collision_id=itemp(plind(i)))
                end do
                do i = 1, ntp
@@ -2124,17 +2126,15 @@
       !! Write a frame of output of the central body
       implicit none
       ! Arguments
       class(swiftest_cb),                intent(inout)    :: self  !! Swiftest base object
       class(swiftest_netcdf_parameters), intent(inout) :: nc    !! Parameters used to for writing a NetCDF dataset to file
       class(swiftest_parameters),        intent(inout) :: param !! Current run configuration parameters 
       ! Internals
-      integer(I4B)                              :: idslot, old_mode, tmp, i
-      integer(I4B), dimension(:), allocatable   :: lm_coords
-      integer(I4B) :: status
+      integer(I4B)                              :: idslot, old_mode, tmp
 
       associate(tslot => nc%tslot)
          call self%write_info(nc, param)
 
          call netcdf_io_check( nf90_set_fill(nc%id, NF90_NOFILL, old_mode), &
                                   "swiftest_io_netcdf_write_frame_cb nf90_set_fill"  )
 
@@ -2230,26 +2230,26 @@
 #endif
       if (param%lmtiny_pl) call netcdf_io_check( nf90_put_var(nc%id, nc%nplm_varid, self%pl%nplm, start=[tslot]), &
                                   "netcdf_io_write_hdr_system nf90_put_var nplm_varid"  )
 
       if (param%lenergy) then
          call netcdf_io_check( nf90_put_var(nc%id, nc%KE_orb_varid, self%ke_orbit, start=[tslot]), &
                                   "netcdf_io_write_hdr_system nf90_put_var KE_orb_varid"  )
-         call netcdf_io_check( nf90_put_var(nc%id, nc%KE_spin_varid, self%ke_spin, start=[tslot]), &
-                                  "netcdf_io_write_hdr_system nf90_put_var KE_spin_varid"  )
+         call netcdf_io_check( nf90_put_var(nc%id, nc%KE_rot_varid, self%ke_rot, start=[tslot]), &
+                                  "netcdf_io_write_hdr_system nf90_put_var KE_rot_varid"  )
          call netcdf_io_check( nf90_put_var(nc%id, nc%PE_varid, self%pe, start=[tslot]), &
                                   "netcdf_io_write_hdr_system nf90_put_var PE_varid"  )
          call netcdf_io_check( nf90_put_var(nc%id, nc%BE_varid, self%be, start=[tslot]), &
                                   "netcdf_io_write_hdr_system nf90_put_var BE_varid"  )
          call netcdf_io_check( nf90_put_var(nc%id, nc%TE_varid, self%te, start=[tslot]), &
                                   "netcdf_io_write_hdr_system nf90_put_var TE_varid"  )
          call netcdf_io_check( nf90_put_var(nc%id, nc%L_orbit_varid, self%L_orbit(:), start=[1,tslot], count=[NDIM,1]), &
                                   "netcdf_io_write_hdr_system nf90_put_var L_orbit_varid"  )
-         call netcdf_io_check( nf90_put_var(nc%id, nc%L_spin_varid, self%L_spin(:), start=[1,tslot], count=[NDIM,1]), &
-                                  "netcdf_io_write_hdr_system nf90_put_var L_spin_varid"  )
+         call netcdf_io_check( nf90_put_var(nc%id, nc%L_rot_varid, self%L_rot(:), start=[1,tslot], count=[NDIM,1]), &
+                                  "netcdf_io_write_hdr_system nf90_put_var L_rot_varid"  )
          call netcdf_io_check( nf90_put_var(nc%id, nc%L_escape_varid, self%L_escape(:), start=[1,tslot], count=[NDIM,1]), &
                                   "netcdf_io_write_hdr_system nf90_put_var L_escape_varid"  )
          call netcdf_io_check( nf90_put_var(nc%id, nc%E_collisions_varid, self%E_collisions, start=[tslot]), &
                                   "netcdf_io_write_hdr_system nf90_put_var E_collisions_varid"  )
          call netcdf_io_check( nf90_put_var(nc%id, nc%E_untracked_varid, self%E_untracked, start=[tslot]), &
                                   "netcdf_io_write_hdr_system nf90_put_var E_untracked_varid"  )
          call netcdf_io_check( nf90_put_var(nc%id, nc%GMescape_varid, self%GMescape, start=[tslot]), &
@@ -2443,26 +2443,31 @@
       character(STRMAX)              :: line                              !! Line of the input file
       character(len=:), allocatable  :: line_trim,param_name, param_value !! Strings used to parse the param file
       character(*),parameter         :: linefmt = '(A)'                   !! Format code for simple text string
       integer(I4B)                   :: nseeds, nseeds_from_file
       logical                        :: seed_set = .false.      !! Is the random seed set in the input file?
       real(DP)                       :: tratio, y
 #ifdef COARRAY
-      type(swiftest_parameters), codimension[*], save :: coparam
-     
-   if (this_image() == 1) then
-      coparam = self
-      associate(param => coparam) 
+      type(swiftest_parameters), codimension[:], allocatable :: param
+
+      select type(self)
+      type is (swiftest_parameters)
+         allocate(param[*], source = self)
+      end select
+
 #else
       associate(param => self) 
 #endif
          ! Parse the file line by line, extracting tokens then matching them up with known parameters if possible
          call random_seed(size = nseeds)
          if (allocated(param%seed)) deallocate(param%seed)
          allocate(param%seed(nseeds))
+#ifdef COARRAY
+      if (this_image() == 1) then
+#endif
          open(unit = unit, file = param%param_file_name, status = 'old', err = 667, iomsg = iomsg)
          do
             read(unit = unit, fmt = linefmt, end = 1, err = 667, iomsg = iomsg) line
             line_trim = trim(adjustl(line))
             ilength = len(line_trim)
             if ((ilength /= 0)) then 
                ifirst = 1
@@ -2594,20 +2599,20 @@
                case("LORBIT_ORIG")
                   read(param_value, *, err = 667, iomsg = iomsg) param%L_orbit_orig(1)
                   do i = 2, NDIM
                      ifirst = ilast + 2
                      param_value = swiftest_io_get_token(line, ifirst, ilast, iostat) 
                      read(param_value, *, err = 667, iomsg = iomsg) param%L_orbit_orig(i)
                   end do
-               case("LSPIN_ORIG")
-                  read(param_value, *, err = 667, iomsg = iomsg) param%L_spin_orig(1)
+               case("LROT_ORIG")
+                  read(param_value, *, err = 667, iomsg = iomsg) param%L_rot_orig(1)
                   do i = 2, NDIM
                      ifirst = ilast + 2
                      param_value = swiftest_io_get_token(line, ifirst, ilast, iostat) 
-                     read(param_value, *, err = 667, iomsg = iomsg) param%L_spin_orig(i)
+                     read(param_value, *, err = 667, iomsg = iomsg) param%L_rot_orig(i)
                   end do
                case("LESCAPE")
                   read(param_value, *, err = 667, iomsg = iomsg) param%L_escape(1)
                   do i = 2, NDIM
                      ifirst = ilast + 2
                      param_value = swiftest_io_get_token(line, ifirst, ilast, iostat) 
                      read(param_value, *, err = 667, iomsg = iomsg) param%L_escape(i)
@@ -2735,15 +2740,15 @@
             end if
             if ((param%out_form /= "EL") .and. (param%out_form /= "XV") .and. (param%out_form /= "XVEL")) then
                write(iomsg,*) 'Invalid out_form: ',trim(adjustl(param%out_form))
                iostat = -1
                return
             end if
             if ((param%out_stat /= "NEW") .and. (param%out_stat /= "REPLACE") .and. (param%out_stat /= "APPEND")  &
-          .and. (param%out_stat /= "UNKNOWN")) then
+            .and. (param%out_stat /= "UNKNOWN")) then
                write(iomsg,*) 'Invalid out_stat: ',trim(adjustl(param%out_stat))
                iostat = -1
                return
             end if
          end if
          if (param%qmin > 0.0_DP) then
             if ((param%qmin_coord /= "HELIO") .and. (param%qmin_coord /= "BARY")) then
@@ -2768,19 +2773,18 @@
             iostat = -1
             return
          end if
 
          ! Calculate the G for the nbody_system units
          param%GU = GC / (param%DU2M**3 / (param%MU2KG * param%TU2S**2))
 
-
          if ((param%encounter_save /= "NONE")       .and. &
-             (param%encounter_save /= "TRAJECTORY") .and. &
-             (param%encounter_save /= "CLOSEST")    .and. &
-             (param%encounter_save /= "BOTH")) then
+               (param%encounter_save /= "TRAJECTORY") .and. &
+               (param%encounter_save /= "CLOSEST")    .and. &
+               (param%encounter_save /= "BOTH")) then
             write(iomsg,*) 'Invalid encounter_save parameter: ',trim(adjustl(param%out_type))
             write(iomsg,*) 'Valid options are NONE, TRAJECTORY, CLOSEST, or BOTH'
             iostat = -1
             return
          end if
 
          param%lenc_save_trajectory = (param%encounter_save == "TRAJECTORY") .or. (param%encounter_save == "BOTH")
@@ -2799,35 +2803,35 @@
          if (param%lmtiny_pl .and. param%GMTINY < 0.0_DP) then
             write(iomsg,*) "GMTINY invalid or not set: ", param%GMTINY
             iostat = -1
             return
          end if
 
          if ((param%collision_model /= "MERGE")       .and. &
-             (param%collision_model /= "BOUNCE")    .and. &
-             (param%collision_model /= "FRAGGLE")) then
+               (param%collision_model /= "BOUNCE")    .and. &
+               (param%collision_model /= "FRAGGLE")) then
             write(iomsg,*) 'Invalid collision_model parameter: ',trim(adjustl(param%out_type))
             write(iomsg,*) 'Valid options are MERGE, BOUNCE, or FRAGGLE'
             iostat = -1
             return
          end if
 
+         if (seed_set) then
+            call random_seed(put = param%seed)
+         else
+            call random_seed(get = param%seed)
+         end if
          if (param%collision_model == "FRAGGLE" ) then
-            if (seed_set) then
-               call random_seed(put = param%seed)
-            else
-               call random_seed(get = param%seed)
-            end if
             if (param%min_GMfrag < 0.0_DP) param%min_GMfrag = param%GMTINY
             if (param%nfrag_reduction < 1.0_DP) then
                write(iomsg,*) "Warning: NFRAG_REDUCTION value invalid. Setting to 1.0" 
                param%nfrag_reduction = 1.0_DP
             end if
          end if
-   
+
          ! Determine if the GR flag is set correctly for this integrator
          select case(param%integrator)
          case(INT_WHM, INT_RMVS, INT_HELIO, INT_SYMBA)
          case default   
             if (param%lgr) write(iomsg, *) 'GR is not yet implemented for this integrator. This parameter will be ignored.'
             param%lgr = .false.
          end select
@@ -2873,63 +2877,61 @@
             write(*,*) "Unknown value for parameter ENCOUNTER_CHECK_PLTP: -> ",trim(adjustl(param%encounter_check_pltp))
             write(*,*) "Must be one of the following: TRIANGULAR or SORTSWEEP"
             write(*,*) "Using default value of TRIANGULAR"
             param%encounter_check_pltp = "TRIANGULAR"
             param%lencounter_sas_pltp = .false.
          end select
 
-
          if (param%lcoarray) then
 #ifdef COARRAY
             if (num_images() == 1) then
                write(iomsg, *) "Only one Coarray image detected. Coarrays will not be used."
                param%lcoarray = .false.
             end if
 
             select case(param%integrator)
             case(INT_WHM, INT_RMVS, INT_HELIO)
             case default   
                write(iomsg, *) "Coarray-based parallelization of test particles are not compatible with this integrator. " &
-                            // "This parameter will be ignored."
+                              // "This parameter will be ignored."
                param%lcoarray = .false.
             end select
 #else
             write(iomsg,*) "Coarray capability not detected. Swiftest must be compiled with Coarrays enabled. to use this feature."
             param%lcoarray = .false.
 #endif
          end if
 
          iostat = 0
-
-      end associate
-
 #ifdef COARRAY
-   end if ! this_image() == 1
-      call coparam%coclone()
+      end if ! this_image() == 1
+#else
+      end associate
 #endif
-      select type(param => self)
+      select type(self)
       type is (swiftest_parameters)
 #ifdef COARRAY
-         param = coparam
+         call coclone(param)
+         self = param
 #endif
-         call param%set_display(param%display_style)
+         call self%set_display(self%display_style)
 
-         if (.not.param%lrestart) then
+         if (.not.self%lrestart) then
 #ifdef COARRAY
-            if (this_image() == 1 .or. param%log_output) then
+            if (this_image() == 1 .or. self%log_output) then
 #endif
-               call param%writer(unit = param%display_unit, iotype = "none", v_list = [0], iostat = iostat, iomsg = iomsg)
-               if (param%log_output) flush(param%display_unit) 
+               call self%writer(unit = self%display_unit, iotype = "none", v_list = [0], iostat = iostat, iomsg = iomsg)
+               if (self%log_output) flush(self%display_unit) 
 #ifdef COARRAY
             end if !(this_image() == 1)
-            write(COLLISION_LOG_OUT,'("collision_coimage",I0.3,".log")') this_image()
+            write(COLLISION_LOG_OUT,'("collision_coimage",I0.4,".log")') this_image()
 #endif
             ! A minimal log of collision outcomes is stored in the following log file
             ! More complete data on collisions is stored in the NetCDF output files
-            call swiftest_io_log_start(param, COLLISION_LOG_OUT, "Collision logfile")
+            call swiftest_io_log_start(self, COLLISION_LOG_OUT, "Collision logfile")
          end if
          ! Print the contents of the parameter file to standard output
       end select
 
       return 
       667 continue
       write(*,*) "Error reading param file: ", trim(adjustl(iomsg))
@@ -3370,15 +3372,15 @@
          if (self%tp%nbody > 0) self%tp%id(:) = [(i, i = self%pl%nbody + 1, self%pl%nbody + 1 + self%tp%nbody)]
          self%maxid = self%pl%nbody + self%tp%nbody
          ! Copy over param file variable inputs
          self%E_orbit_orig = param%E_orbit_orig
          self%GMtot_orig = param%GMtot_orig
          self%L_total_orig(:) = param%L_total_orig(:)
          self%L_orbit_orig(:) = param%L_orbit_orig(:)
-         self%L_spin_orig(:) = param%L_spin_orig(:)
+         self%L_rot_orig(:) = param%L_rot_orig(:)
          self%L_escape(:) = param%L_escape(:)
          self%E_collisions = param%E_collisions
          self%E_untracked = param%E_untracked
       else
          allocate(tmp_param, source=param)
          nc%file_name = param%nc_in
          tmp_param%out_form = param%in_form
@@ -3562,15 +3564,15 @@
       select case(display_style)
       case ('STANDARD')
          self%display_unit = OUTPUT_UNIT !! stdout from iso_fortran_env
          self%log_output = .false.
       case ('COMPACT', 'PROGRESS')
 #ifdef COARRAY
          if (self%lcoarray) then
-            write(SWIFTEST_LOG_FILE,'("swiftest_coimage",I0.3,".log")') this_image()
+            write(SWIFTEST_LOG_FILE,'("swiftest_coimage",I0.4,".log")') this_image()
          else
             write(SWIFTEST_LOG_FILE,'("swiftest.log")')
          end if 
 #endif
          inquire(file=SWIFTEST_LOG_FILE, exist=fileExists)
          if (self%lrestart.and.fileExists) then
             open(unit=SWIFTEST_LOG_OUT, file=SWIFTEST_LOG_FILE, status="OLD", position="APPEND", err = 667, iomsg = errmsg)
```

### Comparing `swiftest-2024.4.1/src/swiftest/swiftest_kick.f90` & `swiftest-2024.4.2/src/swiftest/swiftest_kick.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/swiftest/swiftest_module.f90` & `swiftest-2024.4.2/src/swiftest/swiftest_module.f90`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,14 @@
    use base
    use encounter
    use collision
    use walltime
    use io_progress_bar
    use netcdf_io
    use solver
-#ifdef COARRAY
-   use coarray
-#endif
    !use advisor_annotate
    !$ use omp_lib
    implicit none
    public
 
    type, extends(netcdf_parameters) :: swiftest_netcdf_parameters
    contains
@@ -61,17 +58,14 @@
          !! Initialize a set of parameters used to identify a NetCDF output object
       procedure :: get_valid_masks => swiftest_io_netcdf_get_valid_masks   
          !! Gets logical masks indicating which bodies are valid pl and tp type at the current time
       procedure :: open            => swiftest_io_netcdf_open 
          !! Opens a NetCDF file and does the variable inquiries to activate variable ids
       procedure :: flush           => swiftest_io_netcdf_flush 
          !! Flushes a NetCDF file by closing it then opening it again
-#ifdef COARRAY
-      procedure :: coclone   => swiftest_coarray_coclone_nc
-#endif
    end type swiftest_netcdf_parameters
 
 
    type, extends(base_storage) :: swiftest_storage
       class(swiftest_netcdf_parameters), allocatable :: nc 
          !! NetCDF object attached to this storage object
    contains
@@ -108,18 +102,14 @@
       integer(I4B)                            :: nchild
          !! number of children in merger list
       integer(I4B), dimension(:), allocatable :: child
          !! Index of children particles
    contains
       procedure :: dealloc  => swiftest_util_dealloc_kin 
          !! Deallocates all allocatable arrays
-#ifdef COARRAY
-      procedure :: coclone => swiftest_coarray_coclone_kin 
-         !! Clones the image 1 body object to all other images in the coarray structure.
-#endif
       final :: swiftest_final_kin
          !! Finalizes the Swiftest kinship object - deallocates all allocatables
    end type swiftest_kinship
 
 
    type, extends(base_particle_info) :: swiftest_particle_info
       character(len=NAMELEN)    :: name            
@@ -259,22 +249,18 @@
          !! Sets the inverse heliocentric radius term (1/rh**3)
       procedure :: sort            => swiftest_util_sort_body               
          !! Sorts body arrays by a sortable componen
       procedure :: rearrange       => swiftest_util_sort_rearrange_body     
          !! Rearranges the order of array elements of body based on an input index array. Used in sorting methods
       procedure :: spill           => swiftest_util_spill_body              
          !! "Spills" bodies from one object to another depending on the results of a mask (uses the PACK intrinsic)
+      procedure :: save_discard => swiftest_util_save_discard_body
+         !! Saves a snapshot of the this body to the collision storage object
       generic   :: read_frame      => read_frame_bin                        
          !! Add the generic read frame for Fortran binary files
-#ifdef COARRAY
-      procedure :: coclone         => swiftest_coarray_coclone_body         
-         !! Clones the image 1 body object to all other images in the coarray structure.
-      procedure :: cocollect       => swiftest_coarray_cocollect_body       
-         !! Collects all body object array components from all images and combines them into the image 1 body object
-#endif
    end type swiftest_body
 
 
    type, abstract, extends(base_object) :: swiftest_cb
    !> An abstract class for a generic central body in a Swiftest simulation
       class(swiftest_particle_info), allocatable  :: info              
          !! Particle metadata information
@@ -343,19 +329,14 @@
          !! Deallocates all allocatables and resets all values to defaults 
       procedure :: read_in      => swiftest_io_read_in_cb            
          !! Read in central body initial conditions from an ASCII file
       procedure :: write_frame  => swiftest_io_netcdf_write_frame_cb 
          !! I/O routine for writing out a single frame of time-series data for all bodies in the system in NetCDF format  
       procedure :: write_info   => swiftest_io_netcdf_write_info_cb  
          !! Dump contents of particle information metadata to file
-
-#ifdef COARRAY
-      procedure :: coclone      => swiftest_coarray_coclone_cb       
-         !! Clones the image 1 body object to all other images in the coarray structure.
-#endif
    end type swiftest_cb
 
 
    type, abstract, extends(swiftest_body) :: swiftest_pl
          !! Superclass that defines the generic elements of a Swiftest particle 
       real(DP),                dimension(:),   allocatable :: mass    
          !! Body mass (units MU)
@@ -456,18 +437,14 @@
       procedure :: sort           => swiftest_util_sort_pl           
          !! Sorts body arrays by a sortable component
       procedure :: rearrange      => swiftest_util_sort_rearrange_pl 
          !! Rearranges the order of array elements of body based on an input index array. Used in sorting methods
       procedure :: spill          => swiftest_util_spill_pl          
          !! "Spills" bodies from one object to another depending on the results of a mask (uses the PACK intrinsic)
       generic   :: set_renc       => set_renc_I4B, set_renc_DP 
-#ifdef COARRAY
-      procedure :: coclone      => swiftest_coarray_coclone_pl       
-         !! Clones the image 1 body object to all other images in the coarray structure.
-#endif
    end type swiftest_pl
 
 
    type, abstract, extends(swiftest_body) :: swiftest_tp
       
          !! Superclass that defines the generic elements of a Swiftest test particle 
       integer(I4B), dimension(:,:), allocatable :: k_pltp 
@@ -514,20 +491,14 @@
          !! Method used to construct the vectorized form of the central body mass
       procedure :: sort      => swiftest_util_sort_tp           
          !! Sorts body arrays by a sortable component
       procedure :: rearrange => swiftest_util_sort_rearrange_tp 
          !! Rearranges the order of array elements of body based on an input index array. Used in sorting methods
       procedure :: spill     => swiftest_util_spill_tp          
          !! "Spills" bodies from one object to another depending on the results of a mask (uses the PACK intrinsic)
-#ifdef COARRAY
-      procedure :: coclone      => swiftest_coarray_coclone_tp    
-         !! Clones the image 1 object to all other images in the coarray structure.
-      procedure :: cocollect    => swiftest_coarray_cocollect_tp  
-         !! Collects all object array components from all images and combines them into the image 1 object
-#endif
    end type swiftest_tp
 
 
    !> An abstract class for a basic Swiftest nbody system 
    type, abstract, extends(base_nbody_system) :: swiftest_nbody_system
          !! This superclass contains a minimial nbody_system of a set of test particles (tp), massive bodies (pl), and a central 
          !! body (cb). 
@@ -563,34 +534,34 @@
          !! The current maximum particle id number 
       real(DP)                        :: t = -1.0_DP            
          !! Integration current time
       real(DP)                        :: GMtot = 0.0_DP         
          !! Total nbody_system mass - used for barycentric coordinate conversion
       real(DP)                        :: ke_orbit = 0.0_DP      
          !! nbody_system orbital kinetic energy
-      real(DP)                        :: ke_spin = 0.0_DP       
-         !! nbody_system spin kinetic energy
+      real(DP)                        :: ke_rot = 0.0_DP       
+         !! nbody_system rotational kinetic energy
       real(DP)                        :: pe = 0.0_DP            
          !! nbody_system potential energy
       real(DP)                        :: be = 0.0_DP            
          !! nbody_system binding energy of all bodies
       real(DP)                        :: te = 0.0_DP            
          !! nbody_system total energy
       real(DP)                        :: oblpot = 0.0_DP        
          !! nbody_system potential energy due to oblateness of the central body
       real(DP), dimension(NDIM)       :: L_orbit = 0.0_DP       
          !! nbody_system orbital angular momentum vector
-      real(DP), dimension(NDIM)       :: L_spin = 0.0_DP        
-         !! nbody_system spin angular momentum vector
+      real(DP), dimension(NDIM)       :: L_rot = 0.0_DP        
+         !! nbody_system rotational angular momentum vector
       real(DP), dimension(NDIM)       :: L_total = 0.0_DP       
          !! nbody_system angular momentum vector
       real(DP)                        :: ke_orbit_orig = 0.0_DP 
          !! Initial orbital kinetic energy
-      real(DP)                        :: ke_spin_orig = 0.0_DP  
-         !! Initial spin kinetic energy
+      real(DP)                        :: ke_rot_orig = 0.0_DP  
+         !! Initial rotational kinetic energy
       real(DP)                        :: pe_orig = 0.0_DP       
          !! Initial potential energy
       real(DP)                        :: be_orig = 0.0_DP       
          !! Initial gravitational binding energy
       real(DP)                        :: te_orig = 0.0_DP       
          !! Initial total energy (sum of all sources of energy tracked)
       real(DP)                        :: be_cb   = 0.0_DP       
@@ -600,36 +571,36 @@
          !! Initial orbital energy
       real(DP)                        :: GMtot_orig = 0.0_DP    
          !! Initial nbody_system mass
       real(DP), dimension(NDIM)       :: L_total_orig = 0.0_DP  
          !! Initial total angular momentum vector
       real(DP), dimension(NDIM)       :: L_orbit_orig = 0.0_DP  
          !! Initial orbital angular momentum
-      real(DP), dimension(NDIM)       :: L_spin_orig = 0.0_DP   
-         !! Initial spin angular momentum vector
+      real(DP), dimension(NDIM)       :: L_rot_orig = 0.0_DP   
+         !! Initial rotational angular momentum vector
       real(DP), dimension(NDIM)       :: L_escape = 0.0_DP      
          !! Angular momentum of bodies that escaped the nbody_system (used for bookeeping)
       real(DP)                        :: GMescape = 0.0_DP      
          !! Mass of bodies that escaped the nbody_system (used for bookeeping)
       real(DP)                        :: E_collisions = 0.0_DP  
          !! Energy lost from nbody_system due to collisions
       real(DP)                        :: E_untracked = 0.0_DP   
          !! Energy gained from nbody_system due to escaped bodies
 
       ! Energy, momentum, and mass errors (used in error reporting)
       real(DP)                        :: ke_orbit_error    = 0.0_DP
-      real(DP)                        :: ke_spin_error     = 0.0_DP
+      real(DP)                        :: ke_rot_error     = 0.0_DP
       real(DP)                        :: pe_error          = 0.0_DP
       real(DP)                        :: be_error          = 0.0_DP
       real(DP)                        :: E_orbit_error     = 0.0_DP
       real(DP)                        :: Ecoll_error       = 0.0_DP
       real(DP)                        :: E_untracked_error = 0.0_DP
       real(DP)                        :: te_error          = 0.0_DP
       real(DP)                        :: L_orbit_error     = 0.0_DP
-      real(DP)                        :: L_spin_error      = 0.0_DP
+      real(DP)                        :: L_rot_error      = 0.0_DP
       real(DP)                        :: L_escape_error    = 0.0_DP
       real(DP)                        :: L_total_error     = 0.0_DP
       real(DP)                        :: Mtot_error        = 0.0_DP
       real(DP)                        :: Mescape_error     = 0.0_DP
 
       logical                         :: lbeg                 
          !! True if this is the beginning of a step. This is used so that test particle steps can be calculated separately from 
@@ -679,23 +650,21 @@
          !! Rescales the nbody_system into a new set of units
       procedure :: initialize_output_file  => swiftest_io_initialize_output_file_system                  
          !! Write a frame of input data from file
       procedure :: initialize              => swiftest_util_setup_initialize_system                
          !! Initialize the nbody_system from input files
       procedure :: init_particle_info      => swiftest_util_setup_initialize_particle_info_system  
          !! Initialize the nbody_system from input files
-    ! procedure :: step_spin               => tides_step_spin_system                               
-         !! Steps the spins of the massive & central bodies due to tides.
+    ! procedure :: step_rot               => tides_step_rot_system                               
+         !! Steps the rotations of the massive & central bodies due to tides.
       procedure :: set_msys                => swiftest_util_set_msys                               
          !! Sets the value of msys from the masses of nbody_system bodies.
       procedure :: validate_ids            => swiftest_util_valid_id_system                        
          !! Validate the numerical ids passed to the nbody_system and save the maximum value
 #ifdef COARRAY
-      procedure :: coclone                 => swiftest_coarray_coclone_system                      
-         !! Clones the image 1 body object to all other images in the coarray structure.
       procedure :: coarray_collect         => swiftest_coarray_collect_system                      
          !! Collects all the test particles from other images into the image #1 test particle system
       procedure :: coarray_distribute      => swiftest_coarray_distribute_system                   
          !! Distributes test particles from image #1 out to all images.
       procedure :: coarray_balance         => swiftest_coarray_balance_system                      
          !! Checks whether or not the test particle coarrays need to be rebalanced.
 #endif
@@ -2286,14 +2255,26 @@
          implicit none
          class(swiftest_tp), intent(inout) :: self 
             !! Swiftest test particle object
          integer(I4B),       intent(in)    :: nnew 
             !! New size neded
       end subroutine swiftest_util_resize_tp
 
+      module subroutine swiftest_util_save_discard_body(self, ldiscard_mask, nbody_system, snapshot)
+         implicit none
+         class(swiftest_body), intent(inout) :: self 
+            !! Swiftest body object
+         logical, dimension(:), intent(in) :: ldiscard_mask 
+            !! Logical mask indicating which elements to discard
+         class(swiftest_nbody_system), intent(inout) :: nbody_system 
+            !! Swiftest nbody system object
+         class(base_nbody_system), intent(inout) :: snapshot
+            !! Nbody system object to store the snapshot of the discard system
+      end subroutine swiftest_util_save_discard_body
+
       module subroutine swiftest_util_set_beg_end_pl(self, rbeg, rend, vbeg)
          implicit none
          class(swiftest_pl),       intent(inout)          :: self 
             !! Swiftest massive body object
          real(DP), dimension(:,:), intent(in),   optional :: rbeg 
             !! Position vectors at beginning of step
          real(DP), dimension(:,:), intent(in),   optional :: rend 
@@ -2575,20 +2556,15 @@
          implicit none
       end subroutine swiftest_util_version
    end interface
 
 #ifdef COARRAY
    interface
       module subroutine swiftest_coarray_balance_system(nbody_system, param)
-         !! author: David A. Minton
-         !!
-         !! Checks whether or not the system needs to be rebalance. Rebalancing occurs when the image with the smallest number of 
-         !! test particles has <90% of that of the image with the largest number of test particles.
          implicit none
-         ! Arguments
          class(swiftest_nbody_system), intent(inout) :: nbody_system 
             !! Swiftest nbody system 
          class(swiftest_parameters),   intent(inout) :: param        
             !! Current run configuration parameters 
       end subroutine swiftest_coarray_balance_system
 
       module subroutine swiftest_coarray_collect_system(nbody_system, param)
@@ -2617,117 +2593,50 @@
 
       module subroutine swiftest_coarray_component_clone_info_arr1D(var,src_img)
          implicit none
          type(swiftest_particle_info), dimension(:), allocatable, intent(inout) :: var
          integer(I4B), intent(in),optional :: src_img
       end subroutine swiftest_coarray_component_clone_info_arr1D
 
-      module subroutine swiftest_coarray_component_clone_kin_arr1D(var,src_img)
+      module subroutine swiftest_coarray_coclone_param(param)
          implicit none
-         type(swiftest_kinship), dimension(:), allocatable, intent(inout) :: var
-         integer(I4B), intent(in),optional :: src_img
-      end subroutine swiftest_coarray_component_clone_kin_arr1D
+         type(swiftest_parameters),intent(inout),codimension[*]  :: param  
+      end subroutine swiftest_coarray_coclone_param
    end interface
 
    interface cocollect
       module subroutine swiftest_coarray_component_collect_info_arr1D(var,dest_img)
          implicit none
          type(swiftest_particle_info), dimension(:), allocatable, intent(inout) :: var
          integer(I4B), intent(in),optional :: dest_img
       end subroutine
    end interface
 
-   interface 
-      module subroutine swiftest_coarray_coclone_body(self)
-         implicit none
-         class(swiftest_body),intent(inout),codimension[*]  :: self  
-            !! Swiftest body object
-      end subroutine swiftest_coarray_coclone_body
-
-      module subroutine swiftest_coarray_coclone_cb(self)
-         implicit none
-         class(swiftest_cb),intent(inout),codimension[*]  :: self  
-            !! Swiftest cb object
-      end subroutine swiftest_coarray_coclone_cb
-
-      module subroutine swiftest_coarray_coclone_kin(self)
-         implicit none
-         class(swiftest_kinship),intent(inout),codimension[*]  :: self  
-            !! Swiftest kinship object
-      end subroutine swiftest_coarray_coclone_kin
-
-      module subroutine swiftest_coarray_coclone_nc(self)
-         implicit none
-         class(swiftest_netcdf_parameters),intent(inout),codimension[*]  :: self  
-            !! Swiftest body object
-      end subroutine swiftest_coarray_coclone_nc
-
-      module subroutine swiftest_coarray_coclone_pl(self)
-         implicit none
-         class(swiftest_pl),intent(inout),codimension[*]  :: self  
-            !! Swiftest pl object
-      end subroutine swiftest_coarray_coclone_pl
-
-      module subroutine swiftest_coarray_coclone_tp(self)
-         implicit none
-         class(swiftest_tp),intent(inout),codimension[*]  :: self  
-            !! Swiftest tp object
-      end subroutine swiftest_coarray_coclone_tp
-
-      module subroutine swiftest_coarray_coclone_system(self)
-         implicit none
-         class(swiftest_nbody_system),intent(inout),codimension[*]  :: self  
-            !! Swiftest nbody system object
-      end subroutine swiftest_coarray_coclone_system
-
-      module subroutine swiftest_coarray_cocollect_body(self)
-         implicit none
-         class(swiftest_body),intent(inout), codimension[*] :: self 
-            !! Swiftest body object
-      end subroutine swiftest_coarray_cocollect_body
-
-      module subroutine swiftest_coarray_cocollect_tp(self)
-         implicit none
-         class(swiftest_tp),intent(inout), codimension[*] :: self 
-            !! Swiftest tp object
-      end subroutine swiftest_coarray_cocollect_tp
-   end interface
-
 #endif
 
    contains
       subroutine swiftest_final_kin(self)
-         
-            !! author: David A. Minton
-         
-            !!
-         
-            !! Finalize the swiftest kinship object - deallocates all allocatables
+         !! author: David A. Minton
+         !!
+         !! Finalize the swiftest kinship object - deallocates all allocatables
          implicit none
          ! Argument
          type(swiftest_kinship),  intent(inout) :: self 
             !! SyMBA kinship object
-   
          call self%dealloc()
-   
          return
       end subroutine swiftest_final_kin
 
 
       subroutine swiftest_final_storage(self)
-         
-            !! author: David A. Minton
-         
-            !!
-         
-            !! Finalizer for the storage data type
+         !! author: David A. Minton
+         !!
+         !! Finalizer for the storage data type
          implicit none
          ! Arguments
          type(swiftest_storage) :: self
-
+            !! Swiftest storage object
          call self%dealloc()
-   
          return
       end subroutine swiftest_final_storage
-   
 
 end module swiftest
```

### Comparing `swiftest-2024.4.1/src/swiftest/swiftest_obl.f90` & `swiftest-2024.4.2/src/swiftest/swiftest_obl.f90`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
    end function
 
 
    module subroutine swiftest_obl_rot_matrix(n, rot, rot_matrix, rot_matrix_inv)
       !! author: Kaustub P. Anand
       !! 
       !! Generate a rotation matrix and its inverse to rotate the coordinate frame to align the rotation axis along the z axis for 
-      !! correct spin calculation
+      !! correct rotation calculation
       !! 
 
       implicit none
       ! Arguments
       integer(I4B),             intent(in)           :: n               !! Number of bodies
       real(DP), dimension(NDIM), intent(in)          :: rot             !! Central body rotation vector
       real(DP), dimension(NDIM, NDIM), intent(inout) :: rot_matrix      !! rotation matrix
```

### Comparing `swiftest-2024.4.1/src/swiftest/swiftest_orbel.f90` & `swiftest-2024.4.2/src/swiftest/swiftest_orbel.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/swiftest/swiftest_user.f90` & `swiftest-2024.4.2/src/swiftest/swiftest_user.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/swiftest/swiftest_util.f90` & `swiftest-2024.4.2/src/swiftest/swiftest_util.f90`

 * *Files 2% similar despite different names*

```diff
@@ -185,17 +185,14 @@
       class is (swiftest_pl)
          call util_append(self%mass, source%mass, lsource_mask=lsource_mask)
          call util_append(self%Gmass, source%Gmass, lsource_mask=lsource_mask)
          call util_append(self%rhill, source%rhill, lsource_mask=lsource_mask)
          call util_append(self%renc, source%renc, lsource_mask=lsource_mask)
          call util_append(self%radius, source%radius, lsource_mask=lsource_mask)
          call util_append(self%density, source%density, lsource_mask=lsource_mask)
-         call util_append(self%rbeg, source%rbeg, lsource_mask=lsource_mask)
-         call util_append(self%rend, source%rend, lsource_mask=lsource_mask)
-         call util_append(self%vbeg, source%vbeg, lsource_mask=lsource_mask)
          call util_append(self%Ip, source%Ip, lsource_mask=lsource_mask)
          call util_append(self%rot, source%rot, lsource_mask=lsource_mask)
          call util_append(self%k2, source%k2, lsource_mask=lsource_mask)
          call util_append(self%Q, source%Q, lsource_mask=lsource_mask)
          call util_append(self%tlag, source%tlag, lsource_mask=lsource_mask)
          call util_append(self%kin, source%kin, lsource_mask=lsource_mask)
          call util_append(self%lmtiny, source%lmtiny, lsource_mask=lsource_mask)
@@ -247,16 +244,18 @@
       !!
       !! Convert massive bodies from heliocentric to barycentric coordinates (position and velocity)
       !!
       !! Adapted from David E. Kaufmann's Swifter routine coord_h2b.f90 
       !! Adapted from Hal Levison's Swift routine coord_h2b.f 
       implicit none
       ! Arguments
-      class(swiftest_pl), intent(inout) :: self !! Swiftest massive body object
-      class(swiftest_cb), intent(inout) :: cb   !! Swiftest central body object
+      class(swiftest_pl), intent(inout) :: self 
+         !! Swiftest massive body object
+      class(swiftest_cb), intent(inout) :: cb   
+         !! Swiftest central body object
       ! Internals
       integer(I4B)  :: i
       real(DP)      :: Gmtot
       real(DP), dimension(NDIM) :: xtmp, vtmp
 
       if (self%nbody == 0) return
       associate(pl => self, npl => self%nbody)
@@ -318,16 +317,18 @@
       !!
       !! Convert massive bodies from barycentric to heliocentric coordinates (position and velocity)
       !!
       !! Adapted from David E. Kaufmann's Swifter routine coord_b2h.f90 
       !! Adapted from Hal Levison's Swift routine coord_b2h.f 
       implicit none
       ! Arguments
-      class(swiftest_pl),     intent(inout) :: self !! Swiftest massive body object
-      class(swiftest_cb),  intent(inout) :: cb   !! Swiftest central body object
+      class(swiftest_pl),  intent(inout) :: self 
+         !! Swiftest massive body object
+      class(swiftest_cb),  intent(inout) :: cb   
+         !! Swiftest central body object
       ! Internals
       integer(I4B)          :: i, npl
 
       if (self%nbody == 0) return
 
       associate(pl => self)
          npl = self%nbody
@@ -350,16 +351,18 @@
       !!
       !! Convert test particles from barycentric to heliocentric coordinates (position and velocity)
       !!
       !! Adapted from David E. Kaufmann's Swifter routine coord_b2h_tp.f90 
       !! Adapted from Hal Levison's Swift routine coord_b2h_tp.f 
       implicit none
       ! Arguments
-      class(swiftest_tp),     intent(inout) :: self !! Swiftest massive body object
-      class(swiftest_cb),  intent(in)    :: cb   !! Swiftest central body object
+      class(swiftest_tp),  intent(inout) :: self 
+         !! Swiftest massive body object
+      class(swiftest_cb),  intent(in)    :: cb   
+         !! Swiftest central body object
       ! Internals
       integer(I4B) :: i, ntp
 
       if (self%nbody == 0) return
 
       associate(tp => self)
          ntp = self%nbody
@@ -382,16 +385,18 @@
       !!
       !! Convert massive bodies from barycentric to heliocentric coordinates (velocity only)
       !!
       !! Adapted from David E. Kaufmann's Swifter routine coord_vb2vh.f90 
       !! Adapted from Hal Levison's Swift routine coord_vb2vh.f 
       implicit none
       ! Arguments
-      class(swiftest_pl), intent(inout) :: self !! Swiftest massive body object
-      class(swiftest_cb), intent(inout) :: cb   !! Swiftest central body object
+      class(swiftest_pl), intent(inout) :: self 
+         !! Swiftest massive body object
+      class(swiftest_cb), intent(inout) :: cb   
+         !! Swiftest central body object
       ! Internals
       integer(I4B)              :: i, npl
 
       if (self%nbody == 0) return
 
       associate(pl => self)
          npl = self%nbody
@@ -417,16 +422,18 @@
       !!
       !! Convert test particles from barycentric to heliocentric coordinates (velocity only)
       !!
       !! Adapted from David E. Kaufmann's Swifter routine coord_vb2vh_tp.f90 
       !! Adapted from Hal Levison's Swift routine coord_vb2h_tp.f 
       implicit none
       ! Arguments
-      class(swiftest_tp),     intent(inout) :: self !! Swiftest test particle object
-      real(DP), dimension(:), intent(in)    :: vbcb !! Barycentric velocity of the central body
+      class(swiftest_tp),     intent(inout) :: self 
+         !! Swiftest test particle object
+      real(DP), dimension(:), intent(in)    :: vbcb 
+         !! Barycentric velocity of the central body
 
       if (self%nbody == 0) return
 
       associate(tp => self, ntp => self%nbody)
          where (tp%lmask(1:ntp))
             tp%vh(1, 1:ntp) = tp%vb(1, 1:ntp) - vbcb(1)
             tp%vh(2, 1:ntp) = tp%vb(2, 1:ntp) - vbcb(2)
@@ -443,16 +450,18 @@
       !!
       !! Convert massive bodies from heliocentric to barycentric coordinates (velocity only)
       !!
       !! Adapted from David E. Kaufmann's Swifter routine coord_vh2vb.f90 
       !! Adapted from Hal Levison's Swift routine coord_vh2b.f 
       implicit none
       ! Arguments
-      class(swiftest_pl), intent(inout) :: self !! Swiftest massive body object
-      class(swiftest_cb), intent(inout) :: cb   !! Swiftest central body object
+      class(swiftest_pl), intent(inout) :: self 
+         !! Swiftest massive body object
+      class(swiftest_cb), intent(inout) :: cb   
+         !! Swiftest central body object
       ! Internals
       integer(I4B)  :: i, npl
       real(DP)      :: Gmtot
 
       if (self%nbody == 0) return
 
       associate(pl => self)
@@ -481,16 +490,18 @@
       !!
       !! Convert test particles from heliocentric to barycentric coordinates (velocity only)
       !!
       !! Adapted from David E. Kaufmann's Swifter routine coord_vh2vb_tp.f90
       !! Adapted from Hal Levison's Swift routine coord_vh2b_tp.f 
       implicit none
       ! Arguments
-      class(swiftest_tp),     intent(inout) :: self !! Swiftest test particle object
-      real(DP), dimension(:), intent(in)    :: vbcb !! Barycentric velocity of the central body
+      class(swiftest_tp),     intent(inout) :: self 
+         !! Swiftest test particle object
+      real(DP), dimension(:), intent(in)    :: vbcb 
+         !! Barycentric velocity of the central body
 
       if (self%nbody == 0) return
 
       associate(tp => self, ntp => self%nbody)
          where (tp%lmask(1:ntp))
             tp%vb(1, 1:ntp) = tp%vh(1, 1:ntp) + vbcb(1)
             tp%vb(2, 1:ntp) = tp%vh(2, 1:ntp) + vbcb(2)
@@ -507,16 +518,18 @@
       !!
       !! Convert position vectors of massive bodies from heliocentric to barycentric coordinates (position only)
       !!
       !! Adapted from David E. Kaufmann's Swifter routine coord_h2b.f90 
       !! Adapted from Hal Levison's Swift routine coord_h2b.f 
       implicit none
       ! Arguments
-      class(swiftest_pl), intent(inout) :: self !! Swiftest massive body object
-      class(swiftest_cb), intent(inout) :: cb   !! Swiftest central body object
+      class(swiftest_pl), intent(inout) :: self 
+         !! Swiftest massive body object
+      class(swiftest_cb), intent(inout) :: cb   
+         !! Swiftest central body object
       ! Internals
       integer(I4B)  :: i
       real(DP)      :: Gmtot
       real(DP), dimension(NDIM) :: xtmp
 
       if (self%nbody == 0) return
       associate(pl => self, npl => self%nbody)
@@ -543,16 +556,18 @@
       !!
       !! Convert test particles from heliocentric to barycentric coordinates (position only)
       !!
       !! Adapted from David E. Kaufmann's Swifter routine coord_h2b_tp.f90 
       !! Adapted from Hal Levison's Swift routine coord_h2b_tp.f 
       implicit none
       ! Arguments
-      class(swiftest_tp), intent(inout) :: self !! Swiftest test particle object
-      class(swiftest_cb), intent(in) :: cb      !! Swiftest central body object
+      class(swiftest_tp), intent(inout) :: self 
+         !! Swiftest test particle object
+      class(swiftest_cb), intent(in) :: cb      
+         !! Swiftest central body object
       ! Internals
       integer(I4B) :: i, ntp
 
       if (self%nbody == 0) return
       associate(tp => self)
          ntp = self%nbody
 #ifdef DOCONLOC
@@ -596,19 +611,20 @@
 
 
    module subroutine swiftest_util_copy_particle_info_arr(source, dest, idx)
       !! author: David A. Minton
       !!
       !! Copies contents from an array of one particle information objects to another.
       implicit none
-      class(swiftest_particle_info), dimension(:), intent(in)             :: source !! Source object to copy into
-      class(swiftest_particle_info), dimension(:), intent(inout)          :: dest   !! Swiftest body object with particle metadata 
-                                                                                    !! information object
-      integer(I4B),                  dimension(:), intent(in),   optional :: idx    !! Optional array of indices to draw the source 
-                                                                                    !! object
+      class(swiftest_particle_info), dimension(:), intent(in)             :: source 
+         !! Source object to copy into
+      class(swiftest_particle_info), dimension(:), intent(inout)          :: dest   
+         !! Swiftest body object with particle metadata information object
+      integer(I4B),                  dimension(:), intent(in),   optional :: idx    
+         !! Optional array of indices to draw the source object
       ! Internals
       integer(I4B) :: i, j, n, nsource, ndest
 
       if (size(source) == 0) return
 
       if (present(idx)) then
          n = size(idx)
@@ -815,46 +831,46 @@
       if (allocated(self%collider)) deallocate(self%collider)
       if (allocated(self%encounter_history)) deallocate(self%encounter_history)
       if (allocated(self%collision_history)) deallocate(self%collision_history)
 
       self%t = -1.0_DP            
       self%GMtot = 0.0_DP         
       self%ke_orbit = 0.0_DP      
-      self%ke_spin = 0.0_DP       
+      self%ke_rot = 0.0_DP       
       self%pe = 0.0_DP            
       self%be = 0.0_DP            
       self%te = 0.0_DP            
       self%oblpot = 0.0_DP        
       self%L_orbit = 0.0_DP        
-      self%L_spin = 0.0_DP         
+      self%L_rot = 0.0_DP         
       self%L_total = 0.0_DP          
       self%ke_orbit_orig = 0.0_DP 
-      self%ke_spin_orig = 0.0_DP  
+      self%ke_rot_orig = 0.0_DP  
       self%pe_orig = 0.0_DP       
       self%be_orig = 0.0_DP       
       self%E_orbit_orig = 0.0_DP   
       self%GMtot_orig = 0.0_DP    
       self%L_total_orig = 0.0_DP     
       self%L_orbit_orig = 0.0_DP   
-      self%L_spin_orig = 0.0_DP    
+      self%L_rot_orig = 0.0_DP    
       self%L_escape = 0.0_DP       
       self%GMescape = 0.0_DP      
       self%E_collisions = 0.0_DP   
       self%E_untracked = 0.0_DP    
 
       self%ke_orbit_error    = 0.0_DP
-      self%ke_spin_error     = 0.0_DP
+      self%ke_rot_error     = 0.0_DP
       self%pe_error          = 0.0_DP
       self%be_error          = 0.0_DP
       self%E_orbit_error     = 0.0_DP
       self%Ecoll_error       = 0.0_DP
       self%E_untracked_error = 0.0_DP
       self%te_error          = 0.0_DP
       self%L_orbit_error     = 0.0_DP
-      self%L_spin_error      = 0.0_DP
+      self%L_rot_error      = 0.0_DP
       self%L_escape_error    = 0.0_DP
       self%L_total_error     = 0.0_DP
       self%Mtot_error        = 0.0_DP
       self%Mescape_error     = 0.0_DP
 
       return
    end subroutine swiftest_util_dealloc_system
@@ -993,17 +1009,14 @@
             !! Fill components specific to the massive body class
             call util_fill(keeps%mass,    inserts%mass,    lfill_list)
             call util_fill(keeps%Gmass,   inserts%Gmass,   lfill_list)
             call util_fill(keeps%rhill,   inserts%rhill,   lfill_list)
             call util_fill(keeps%renc,    inserts%renc,    lfill_list)
             call util_fill(keeps%radius,  inserts%radius,  lfill_list)
             call util_fill(keeps%density, inserts%density, lfill_list)
-            call util_fill(keeps%rbeg,    inserts%rbeg,    lfill_list)
-            call util_fill(keeps%rend,    inserts%rend,    lfill_list)
-            call util_fill(keeps%vbeg,    inserts%vbeg,    lfill_list)
             call util_fill(keeps%Ip,      inserts%Ip,      lfill_list)
             call util_fill(keeps%rot,     inserts%rot,     lfill_list)
             call util_fill(keeps%k2,      inserts%k2,      lfill_list)
             call util_fill(keeps%Q,       inserts%Q,       lfill_list)
             call util_fill(keeps%tlag,    inserts%tlag,    lfill_list)
             call util_fill(keeps%kin,     inserts%kin,     lfill_list)
             call util_fill(keeps%nplenc,  inserts%nplenc,  lfill_list)
@@ -1200,34 +1213,34 @@
       !!  
       !! Adapted from Martin Duncan's Swift routine anal_energy.f
       implicit none
       class(swiftest_nbody_system), intent(inout) :: self     !! Swiftest nbody system object
       class(swiftest_parameters),   intent(in)    :: param    !! Current run configuration parameters
       ! Internals
       integer(I4B) :: i,j, npl
-      real(DP) :: kecb, kespincb
-      real(DP), dimension(self%pl%nbody) :: kepl, kespinpl
+      real(DP) :: kecb, kerotcb
+      real(DP), dimension(self%pl%nbody) :: kepl, kerotpl
       real(DP), dimension(NDIM,self%pl%nbody) :: Lplorbit
-      real(DP), dimension(NDIM,self%pl%nbody) :: Lplspin
-      real(DP), dimension(NDIM) :: Lcborbit, Lcbspin
+      real(DP), dimension(NDIM,self%pl%nbody) :: Lplrot
+      real(DP), dimension(NDIM) :: Lcborbit, Lcbrot
       real(DP), dimension(NDIM) :: h
 
       associate(nbody_system => self, pl => self%pl, cb => self%cb)
          npl = self%pl%nbody
          nbody_system%L_orbit(:) = 0.0_DP
-         nbody_system%L_spin(:) = 0.0_DP
+         nbody_system%L_rot(:) = 0.0_DP
          nbody_system%L_total(:) = 0.0_DP
          nbody_system%ke_orbit = 0.0_DP
-         nbody_system%ke_spin = 0.0_DP
+         nbody_system%ke_rot = 0.0_DP
 
          nbody_system%GMtot = cb%Gmass
          if (npl > 0) then
             kepl(:) = 0.0_DP
             Lplorbit(:,:) = 0.0_DP
-            Lplspin(:,:) = 0.0_DP
+            Lplrot(:,:) = 0.0_DP
             pl%lmask(1:npl) = pl%status(1:npl) /= INACTIVE
             nbody_system%GMtot = nbody_system%GMtot + sum(pl%Gmass(1:npl), pl%lmask(1:npl)) 
          end if
             
          kecb = cb%mass * dot_product(cb%vb(:), cb%vb(:))
          nbody_system%be_cb = -3*cb%Gmass * cb%mass / (5 * cb%radius) 
          Lcborbit(:) = cb%mass * (cb%rb(:) .cross. cb%vb(:))
@@ -1247,52 +1260,52 @@
 
                ! Kinetic energy from orbit
                kepl(i) = pl%mass(i) * dot_product(pl%vb(:,i), pl%vb(:,i)) 
             end do
          end if
 
          if (param%lrotation) then
-            kespincb = cb%mass * cb%Ip(3) * cb%radius**2 * dot_product(cb%rot(:), cb%rot(:))
+            kerotcb = cb%mass * cb%Ip(3) * cb%radius**2 * dot_product(cb%rot(:), cb%rot(:))
 
             ! For simplicity, we always assume that the rotation pole is the 3rd principal axis
-            Lcbspin(:) = cb%Ip(3) * cb%mass * cb%radius**2 * cb%rot(:)
+            Lcbrot(:) = cb%Ip(3) * cb%mass * cb%radius**2 * cb%rot(:)
 
             if (npl > 0) then
 #ifdef DOCONLOC
-               do concurrent (i = 1:npl, pl%lmask(i)) shared(pl,Lplspin,kespinpl)
+               do concurrent (i = 1:npl, pl%lmask(i)) shared(pl,Lplrot,kerotpl)
 #else
                do concurrent (i = 1:npl, pl%lmask(i))
 #endif
                   ! Currently we assume that the rotation pole is the 3rd principal axis
-                  ! Angular momentum from spin
-                  Lplspin(:,i) = pl%mass(i) * pl%Ip(3,i) * pl%radius(i)**2 * pl%rot(:,i)
+                  ! Angular momentum from rotation
+                  Lplrot(:,i) = pl%mass(i) * pl%Ip(3,i) * pl%radius(i)**2 * pl%rot(:,i)
 
-                  ! Kinetic energy from spin
-                  kespinpl(i) = pl%mass(i) * pl%Ip(3,i) * pl%radius(i)**2 * dot_product(pl%rot(:,i), pl%rot(:,i))
+                  ! Kinetic energy from rotation
+                  kerotpl(i) = pl%mass(i) * pl%Ip(3,i) * pl%radius(i)**2 * dot_product(pl%rot(:,i), pl%rot(:,i))
                end do
 
-               nbody_system%ke_spin = 0.5_DP * (kespincb + sum(kespinpl(1:npl), pl%lmask(1:npl)))
+               nbody_system%ke_rot = 0.5_DP * (kerotcb + sum(kerotpl(1:npl), pl%lmask(1:npl)))
             else
-               nbody_system%ke_spin = 0.5_DP * kespincb
+               nbody_system%ke_rot = 0.5_DP * kerotcb
             end if
 
             if (npl > 0) then
 #ifdef DOCONLOC
-               do concurrent (j = 1:NDIM) shared(nbody_system,pl,Lplspin,Lcbspin)
+               do concurrent (j = 1:NDIM) shared(nbody_system,pl,Lplrot,Lcbrot)
 #else
                do concurrent (j = 1:NDIM)
 #endif
-                  nbody_system%L_spin(j) = Lcbspin(j) + sum(Lplspin(j,1:npl), pl%lmask(1:npl))
+                  nbody_system%L_rot(j) = Lcbrot(j) + sum(Lplrot(j,1:npl), pl%lmask(1:npl))
                end do
             else
-               nbody_system%L_spin(:) = Lcbspin(:)
+               nbody_system%L_rot(:) = Lcbrot(:)
             end if
          else
-            nbody_system%ke_spin = 0.0_DP
-            nbody_system%L_spin(:) = 0.0_DP
+            nbody_system%ke_rot = 0.0_DP
+            nbody_system%L_rot(:) = 0.0_DP
          end if
  
          if (npl > 0) then
             if (param%lflatten_interactions) then
                call swiftest_util_get_potential_energy(npl, pl%nplpl, pl%k_plpl, pl%lmask, cb%Gmass, pl%Gmass, pl%mass, pl%rb, &
                                                       nbody_system%pe)
             else
@@ -1321,16 +1334,16 @@
          end if
 
          if ((param%lclose .and. (npl > 0))) then
             nbody_system%be = sum(-3*pl%Gmass(1:npl)*pl%mass(1:npl)/(5*pl%radius(1:npl)), pl%lmask(1:npl)) 
          else
             nbody_system%be = 0.0_DP
          end if
-         nbody_system%te = nbody_system%ke_orbit + nbody_system%ke_spin + nbody_system%pe + nbody_system%be 
-         nbody_system%L_total(:) = nbody_system%L_orbit(:) + nbody_system%L_spin(:)
+         nbody_system%te = nbody_system%ke_orbit + nbody_system%ke_rot + nbody_system%pe + nbody_system%be 
+         nbody_system%L_total(:) = nbody_system%L_orbit(:) + nbody_system%L_rot(:)
       end associate
 
       return
    end subroutine swiftest_util_get_energy_and_momentum_system
 
 
    module subroutine swiftest_util_get_potential_energy_flat(npl, nplpl, k_plpl, lmask, GMcb, Gmass, mass, rb, pe)
@@ -1698,16 +1711,22 @@
       logical, dimension(:), allocatable :: lmask
       class(encounter_list), allocatable :: plplenc_old
       logical :: lencounter
 
       associate(pl => self, tp => nbody_system%tp, cb => nbody_system%cb, pl_adds => nbody_system%pl_adds)
 
          npl = pl%nbody
-         nadd = pl_adds%nbody
          if (npl == 0) return
+
+         if (allocated(nbody_system%pl_adds)) then
+            nadd = pl_adds%nbody
+         else
+            nadd = 0
+         end if
+
          ! Deallocate any temporary variables
          if (allocated(pl%rbeg)) deallocate(pl%rbeg)
          if (allocated(pl%rend)) deallocate(pl%rend)
 
          ! Remove the discards and destroy the list, as the nbody_system already tracks pl_discards elsewhere
          allocate(lmask(npl))
          lmask(1:npl) = pl%ldiscard(1:npl)
@@ -2189,14 +2208,57 @@
       call util_resize(self%peri, nnew)
       call util_resize(self%atp, nnew)
 
       return
    end subroutine swiftest_util_resize_tp
 
 
+   module subroutine swiftest_util_save_discard_body(self, ldiscard_mask, nbody_system, snapshot)
+      !! author: David A. Minton
+      !!
+      !! Saves the discarded bodies from a Swiftest body object to a snapshot object
+      implicit none
+      ! Arguments
+      class(swiftest_body), intent(inout) :: self 
+         !! Swiftest body object
+      logical, dimension(:), intent(in) :: ldiscard_mask 
+         !! Logical mask indicating which elements to discard
+      class(swiftest_nbody_system), intent(inout) :: nbody_system 
+         !! Swiftest nbody system object
+      class(base_nbody_system), intent(inout) :: snapshot
+         !! Swiftest nbody system object to store the snapshot of the discard system. Typically this will be something like 
+         !! nbody_system%collider%before or nbody_system%collider%after
+      ! Internals
+      class(swiftest_tp), allocatable :: tp_discards
+      class(swiftest_pl), allocatable :: pl_discards
+
+      select type(snapshot)
+      class is (swiftest_nbody_system)
+         select type(self)
+         class is (swiftest_tp)
+            allocate(tp_discards, mold=self)
+            call self%spill(tp_discards, ldiscard_mask, ldestructive=.false.)
+            if (allocated(snapshot%tp)) deallocate(snapshot%tp)
+            allocate(snapshot%tp, source=tp_discards)
+         class is (swiftest_pl)
+            allocate(pl_discards, mold=self)
+            call self%spill(pl_discards, ldiscard_mask, ldestructive=.false.)
+            if (allocated(snapshot%pl)) deallocate(snapshot%pl)
+            allocate(snapshot%pl, source=pl_discards)
+         end select
+   
+         if (nbody_system%collider%impactors%regime == REGIME_CB_IMPACT) then
+            if (allocated(snapshot%cb)) deallocate(snapshot%cb)
+            allocate(snapshot%cb, source=nbody_system%cb)
+         end if
+      end select
+      return
+   end subroutine swiftest_util_save_discard_body
+
+
    module subroutine swiftest_util_set_beg_end_pl(self, rbeg, rend, vbeg)
       !! author: David A. Minton
       !! 
       !! Sets one or more of the values of rbeg, rend, and vbeg
       implicit none
       ! Arguments
       class(swiftest_pl),       intent(inout)          :: self !! Swiftest massive body object
@@ -2446,37 +2508,39 @@
       rh(1:self%nbody) = .mag. self%rh(:,1:self%nbody)
       self%rhill(1:self%nbody) = rh(1:self%nbody) * (self%Gmass(1:self%nbody) / cb%Gmass / 3)**THIRD 
 
       return
    end subroutine swiftest_util_set_rhill_approximate
 
    module subroutine swiftest_util_setup_construct_system(nbody_system, param)
-
       !! author: David A. Minton
       !!
       !! Constructor for a Swiftest nbody system. Creates the nbody system object based on the user-input integrator
       !! 
       implicit none
       ! Arguments
-      class(swiftest_nbody_system), allocatable, intent(inout) :: nbody_system !! Swiftest nbody_system object
-      class(swiftest_parameters),                intent(inout) :: param        !! Current run configuration parameters
+      class(swiftest_nbody_system), allocatable, intent(inout) :: nbody_system 
+         !! Swiftest nbody_system object
+      class(swiftest_parameters),                intent(inout) :: param        
+         !! Current run configuration parameters
       select case(param%integrator)
       case (INT_BS)
          write(*,*) 'Bulirsch-Stoer integrator not yet enabled'
        case (INT_HELIO)
          allocate(helio_nbody_system :: nbody_system)
          select type(nbody_system)
          class is (helio_nbody_system)
             allocate(helio_cb :: nbody_system%cb)
             allocate(helio_pl :: nbody_system%pl)
             allocate(helio_tp :: nbody_system%tp)
             allocate(helio_pl :: nbody_system%pl_discards)
             allocate(helio_tp :: nbody_system%tp_discards)
          end select
          param%collision_model = "MERGE"
+         param%lenergy = .false.
       case (INT_RA15)
          write(*,*) 'Radau integrator not yet enabled'
       case (INT_TU4)
          write(*,*) 'INT_TU4 integrator not yet enabled'
       case (INT_WHM)
          allocate(whm_nbody_system :: nbody_system)
          select type(nbody_system)
@@ -2484,25 +2548,27 @@
             allocate(whm_cb :: nbody_system%cb)
             allocate(whm_pl :: nbody_system%pl)
             allocate(whm_tp :: nbody_system%tp)
             allocate(whm_pl :: nbody_system%pl_discards)
             allocate(whm_tp :: nbody_system%tp_discards)
          end select
          param%collision_model = "MERGE"
+         param%lenergy = .false.
       case (INT_RMVS)
          allocate(rmvs_nbody_system :: nbody_system)
          select type(nbody_system)
          class is (rmvs_nbody_system)
             allocate(rmvs_cb :: nbody_system%cb)
             allocate(rmvs_pl :: nbody_system%pl)
             allocate(rmvs_tp :: nbody_system%tp)
             allocate(rmvs_pl :: nbody_system%pl_discards)
             allocate(rmvs_tp :: nbody_system%tp_discards)
          end select
          param%collision_model = "MERGE"
+         param%lenergy = .false.
       case (INT_SYMBA)
          allocate(symba_nbody_system :: nbody_system)
          select type(nbody_system)
          class is (symba_nbody_system)
             allocate(symba_cb :: nbody_system%cb)
             allocate(symba_pl :: nbody_system%pl)
             allocate(symba_tp :: nbody_system%tp)
@@ -2878,45 +2944,45 @@
       allocate(snapshot%cb, source=nbody_system%cb )
       allocate(snapshot%pl, source=nbody_system%pl )
       allocate(snapshot%tp, source=nbody_system%tp )
 
       snapshot%t                 = nbody_system%t
       snapshot%GMtot             = nbody_system%GMtot
       snapshot%ke_orbit          = nbody_system%ke_orbit
-      snapshot%ke_spin           = nbody_system%ke_spin
+      snapshot%ke_rot           = nbody_system%ke_rot
       snapshot%pe                = nbody_system%pe
       snapshot%be                = nbody_system%be
       snapshot%te                = nbody_system%te
       snapshot%oblpot            = nbody_system%oblpot
       snapshot%L_orbit           = nbody_system%L_orbit
-      snapshot%L_spin            = nbody_system%L_spin
+      snapshot%L_rot            = nbody_system%L_rot
       snapshot%L_total           = nbody_system%L_total
       snapshot%ke_orbit_orig     = nbody_system%ke_orbit_orig
-      snapshot%ke_spin_orig      = nbody_system%ke_spin_orig
+      snapshot%ke_rot_orig      = nbody_system%ke_rot_orig
       snapshot%pe_orig           = nbody_system%pe_orig
       snapshot%be_orig           = nbody_system%be_orig
       snapshot%E_orbit_orig      = nbody_system%E_orbit_orig
       snapshot%GMtot_orig        = nbody_system%GMtot_orig
       snapshot%L_total_orig      = nbody_system%L_total_orig
       snapshot%L_orbit_orig      = nbody_system%L_orbit_orig
-      snapshot%L_spin_orig       = nbody_system%L_spin_orig
+      snapshot%L_rot_orig       = nbody_system%L_rot_orig
       snapshot%L_escape          = nbody_system%L_escape
       snapshot%GMescape          = nbody_system%GMescape
       snapshot%E_collisions      = nbody_system%E_collisions
       snapshot%E_untracked       = nbody_system%E_untracked
       snapshot%ke_orbit_error    = nbody_system%ke_orbit_error   
-      snapshot%ke_spin_error     = nbody_system%ke_spin_error    
+      snapshot%ke_rot_error     = nbody_system%ke_rot_error    
       snapshot%pe_error          = nbody_system%pe_error         
       snapshot%be_error          = nbody_system%be_error         
       snapshot%E_orbit_error     = nbody_system%E_orbit_error    
       snapshot%Ecoll_error       = nbody_system%Ecoll_error      
       snapshot%E_untracked_error = nbody_system%E_untracked_error
       snapshot%te_error          = nbody_system%te_error         
       snapshot%L_orbit_error     = nbody_system%L_orbit_error    
-      snapshot%L_spin_error      = nbody_system%L_spin_error     
+      snapshot%L_rot_error      = nbody_system%L_rot_error     
       snapshot%L_escape_error    = nbody_system%L_escape_error   
       snapshot%L_total_error     = nbody_system%L_total_error    
       snapshot%Mtot_error        = nbody_system%Mtot_error       
       snapshot%Mescape_error     = nbody_system%Mescape_error    
       snapshot%lbeg              = nbody_system%lbeg
 
 
@@ -3205,18 +3271,18 @@
          call util_sort_rearrange(pl%rbeg,    ind, npl)
          call util_sort_rearrange(pl%vbeg,    ind, npl)
          call util_sort_rearrange(pl%Ip,      ind, npl)
          call util_sort_rearrange(pl%rot,     ind, npl)
          call util_sort_rearrange(pl%k2,      ind, npl)
          call util_sort_rearrange(pl%Q,       ind, npl)
          call util_sort_rearrange(pl%tlag,    ind, npl)
-         call util_sort_rearrange(pl%kin,        ind, npl)
-         call util_sort_rearrange(pl%lmtiny,     ind, npl)
-         call util_sort_rearrange(pl%nplenc,     ind, npl)
-         call util_sort_rearrange(pl%ntpenc,     ind, npl)
+         call util_sort_rearrange(pl%kin,     ind, npl)
+         call util_sort_rearrange(pl%lmtiny,  ind, npl)
+         call util_sort_rearrange(pl%nplenc,  ind, npl)
+         call util_sort_rearrange(pl%ntpenc,  ind, npl)
 
          if (allocated(pl%k_plpl)) deallocate(pl%k_plpl)
 
          call swiftest_util_sort_rearrange_body(pl, ind)
       end associate
 
       return
@@ -3421,15 +3487,14 @@
             !! Spill components specific to the massive body class
             call util_spill(keeps%mass,    discards%mass,    lspill_list, ldestructive)
             call util_spill(keeps%Gmass,   discards%Gmass,   lspill_list, ldestructive)
             call util_spill(keeps%rhill,   discards%rhill,   lspill_list, ldestructive)
             call util_spill(keeps%renc,    discards%renc,    lspill_list, ldestructive)
             call util_spill(keeps%radius,  discards%radius,  lspill_list, ldestructive)
             call util_spill(keeps%density, discards%density, lspill_list, ldestructive)
-            call util_spill(keeps%rbeg,    discards%rbeg,    lspill_list, ldestructive)
             call util_spill(keeps%rend,    discards%rend,    lspill_list, ldestructive)
             call util_spill(keeps%vbeg,    discards%vbeg,    lspill_list, ldestructive)
             call util_spill(keeps%Ip,      discards%Ip,      lspill_list, ldestructive)
             call util_spill(keeps%rot,     discards%rot,     lspill_list, ldestructive)
             call util_spill(keeps%k2,      discards%k2,      lspill_list, ldestructive)
             call util_spill(keeps%Q,       discards%Q,       lspill_list, ldestructive)
             call util_spill(keeps%tlag,    discards%tlag,    lspill_list, ldestructive)
```

### Comparing `swiftest-2024.4.1/src/symba/symba_discard.f90` & `swiftest-2024.4.2/src/symba/symba_discard.f90`

 * *Files 4% similar despite different names*

```diff
@@ -119,39 +119,39 @@
       class(symba_pl),           intent(inout) :: pl
       class(symba_nbody_system), intent(inout) :: nbody_system
       class(swiftest_parameters),   intent(inout) :: param
       integer(I4B),              intent(in)    :: ipl
       logical,                   intent(in)         :: lescape_body
       ! Internals
       real(DP), dimension(NDIM) :: Lpl, L_total, Lcb, xcom, vcom, drot0, drot1
-      real(DP)                  :: pe, be, ke_orbit, ke_spin, becb0, becb1
+      real(DP)                  :: pe, be, ke_orbit, ke_rot, becb0, becb1
       integer(I4B)              :: i, oldstat
    
       select type(cb => nbody_system%cb)
       class is (symba_cb)
    
          ! Add the potential, binding, and kinetic energy of the lost body to the records
          pe = -cb%Gmass * pl%mass(ipl) / norm2(pl%rb(:, ipl) - cb%rb(:))
          be = -3*pl%Gmass(ipl) * pl%mass(ipl) / (5 * pl%radius(ipl))
          ke_orbit = 0.5_DP * pl%mass(ipl) * dot_product(pl%vb(:, ipl), pl%vb(:, ipl)) 
          if (param%lrotation) then
-            ke_spin  = 0.5_DP * pl%mass(ipl) * pl%radius(ipl)**2 * pl%Ip(3, ipl) * dot_product(pl%rot(:, ipl), pl%rot(:, ipl))
+            ke_rot  = 0.5_DP * pl%mass(ipl) * pl%radius(ipl)**2 * pl%Ip(3, ipl) * dot_product(pl%rot(:, ipl), pl%rot(:, ipl))
          else
-            ke_spin = 0.0_DP
+            ke_rot = 0.0_DP
          end if
    
          if (lescape_body) then
             nbody_system%GMescape = nbody_system%GMescape + pl%Gmass(ipl)
             do i = 1, pl%nbody
                if (i == ipl) cycle
                pe = pe - pl%Gmass(i) * pl%mass(ipl) / norm2(pl%rb(:, ipl) - pl%rb(:, i))
             end do
 
-            nbody_system%E_collisions  = nbody_system%E_collisions + ke_orbit + ke_spin + pe + be
-            nbody_system%E_untracked  = nbody_system%E_untracked - (ke_orbit + ke_spin + pe + be)
+            nbody_system%E_collisions  = nbody_system%E_collisions + ke_orbit + ke_rot + pe + be
+            nbody_system%E_untracked  = nbody_system%E_untracked - (ke_orbit + ke_rot + pe + be)
    
             L_total(:) = 0.0_DP
             do i = 1, pl%nbody
                Lpl(:) = pL%mass(i) * (pl%rb(:,i) .cross. pl%vb(:, i))
                L_total(:) = L_total(:) + Lpl(:)
             end do
             L_total(:) = L_total(:) + cb%mass * (cb%rb(:) .cross. cb%vb(:))
@@ -176,15 +176,15 @@
             Lpl(:) = (pl%rb(:,ipl) - xcom(:)) .cross. (pL%vb(:,ipl) - vcom(:))
             if (param%lrotation) Lpl(:) = Lpl(:) + pl%radius(ipl)**2 * pl%Ip(3,ipl) * pl%rot(:, ipl)
             Lpl(:) = pl%mass(ipl) * Lpl(:)
      
             Lcb(:) = cb%mass * ((cb%rb(:) - xcom(:)) .cross. (cb%vb(:) - vcom(:)))
    
             ke_orbit = ke_orbit + 0.5_DP * cb%mass * dot_product(cb%vb(:), cb%vb(:)) 
-            if (param%lrotation) ke_spin = ke_spin + 0.5_DP * cb%mass * cb%radius**2 * cb%Ip(3) * dot_product(cb%rot(:), cb%rot(:))
+            if (param%lrotation) ke_rot = ke_rot + 0.5_DP * cb%mass * cb%radius**2 * cb%Ip(3) * dot_product(cb%rot(:), cb%rot(:))
             ! Update mass of central body to be consistent with its total mass
             becb0 = -(3 * cb%Gmass * cb%mass) / (5 * cb%radius)
             cb%dGM = cb%dGM + pl%Gmass(ipl)
             cb%dR = cb%dR + 1.0_DP / 3.0_DP * (pl%radius(ipl) / cb%radius)**3 - 2.0_DP / 9.0_DP * (pl%radius(ipl) / cb%radius)**6
             cb%Gmass = cb%GM0 + cb%dGM
             cb%mass = cb%Gmass / param%GU
             cb%radius = cb%R0 + cb%dR
@@ -194,15 +194,15 @@
             ! Add planet angular momentum to central body accumulator
             cb%dL(:) = Lpl(:) + cb%dL(:) + Lcb(:)
             ! Update rotation of central body to by consistent with its angular momentum 
             if (param%lrotation) then
                drot0(:) = cb%L0(:)/ (cb%Ip(3) * cb%mass * cb%radius**2)  
                drot1(:) = cb%dL(:) / (cb%Ip(3) * cb%mass * cb%radius**2)
                cb%rot(:) = drot0(:) + drot1(:)
-               ke_spin  = ke_spin - 0.5_DP * cb%mass * cb%radius**2 * cb%Ip(3) * dot_product(cb%rot(:), cb%rot(:)) 
+               ke_rot  = ke_rot - 0.5_DP * cb%mass * cb%radius**2 * cb%Ip(3) * dot_product(cb%rot(:), cb%rot(:)) 
             end if
             cb%rb(:) = xcom(:)
             cb%vb(:) = vcom(:)
             ke_orbit = ke_orbit - 0.5_DP * cb%mass * dot_product(cb%vb(:), cb%vb(:)) 
 
             ! Add the change in central body binding energy to the collision energy tracker
             nbody_system%E_collisions  = nbody_system%E_collisions + (becb1 - becb0)
@@ -223,18 +223,14 @@
       !! Adapted from David E. Kaufmann's Swifter routine: symba_discard_pl.f90
       !! Adapted from Hal Levison's Swift routine discard_massive5.f 
       implicit none
       ! Arguments
       class(symba_pl),              intent(inout) :: pl     !! SyMBA test particle object
       class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
       class(swiftest_parameters),   intent(in)    :: param  !! Current run configuration parameters 
-      ! Internals
-      logical, dimension(pl%nbody) ::  ldiscard
-      integer(I4B) :: i, nstart, nend, nsub
-      class(symba_pl), allocatable            :: plsub
     
       ! First check for collisions with the central body
       associate(npl => pl%nbody, cb => nbody_system%cb, pl_discards => nbody_system%pl_discards)
          if (npl == 0) return 
          if ((param%rmin >= 0.0_DP) .or. (param%rmax >= 0.0_DP) .or.  (param%rmaxu >= 0.0_DP)) then
             call symba_discard_cb_pl(pl, nbody_system, param)
          end if
@@ -284,29 +280,28 @@
       return
    end subroutine symba_discard_nonplpl_conservation
 
 
    subroutine symba_discard_peri_pl(pl, nbody_system, param)
       !! author: David A. Minton
       !!
-      !! Check to see if a test particle should be discarded because its perihelion distance becomes too small
+      !! Check to see if a massive body should be discarded because its perihelion distance becomes too small
       !!
       !! Adapted from David E. Kaufmann's Swifter routine: symba_discard_peri_pl.f90
       !! Adapted from Hal Levison's Swift routine discard_mass_peri.f
       implicit none
       ! Arguments
       class(symba_pl),              intent(inout) :: pl     !! SyMBA massive body object
       class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
       class(swiftest_parameters),   intent(in)    :: param  !! Current run configuration parameters
       ! Internals
       logical               :: lfirst_orig
       integer(I4B)          :: i
       character(len=STRMAX) :: timestr, idstr, message
 
-
       lfirst_orig = pl%lfirst
       pl%lfirst = nbody_system%lfirst_peri
       if (nbody_system%lfirst_peri) then
          call pl%get_peri(nbody_system, param)          
          nbody_system%lfirst_peri = .false.
       else
          call pl%get_peri(nbody_system, param)          
@@ -343,43 +338,72 @@
       implicit none
       ! Arguments
       class(symba_pl),              intent(inout) :: self   !! SyMBA test particle object
       class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
       class(swiftest_parameters),   intent(inout) :: param  !! Current run configuration parameters 
       ! Internals
       real(DP) :: E_orbit_before, E_orbit_after
+      logical, dimension(:), allocatable :: ldiscard
+      integer(I4B) :: i, nstart, nend, nsub
+      logical :: cb_collide
+      class(swiftest_pl), allocatable :: plsub
    
       select type(nbody_system)
       class is (symba_nbody_system)
          select type(param)
          class is (swiftest_parameters)
-            associate(pl => self, plpl_encounter => nbody_system%plpl_encounter, plpl_collision => nbody_system%plpl_collision)
+            associate(pl => self, &
+                      npl => self%nbody, &
+                      t => nbody_system%t, &
+                      plpl_encounter => nbody_system%plpl_encounter, &
+                      plpl_collision => nbody_system%plpl_collision, &
+                      collider => nbody_system%collider, &
+                      impactors => nbody_system%collider%impactors, &
+                      collision_history => nbody_system%collision_history, &
+                      pl_discards => nbody_system%pl_discards)
                call pl%vb2vh(nbody_system%cb) 
                call pl%rh2rb(nbody_system%cb)
-               !call plpl_encounter%write(pl, pl, param) TODO: write the encounter list writer for NetCDF
 
                call symba_discard_nonplpl(self, nbody_system, param)
 
                if (.not.any(pl%ldiscard(:))) return
 
+               ! Save the before snapshots
                if (param%lenergy) then
                   call nbody_system%get_energy_and_momentum(param)
                   E_orbit_before = nbody_system%te
+                  call nbody_system%conservation_report(param, lterminal=.false.)
                end if
 
+               allocate(ldiscard, source=pl%ldiscard(:))
+               if (any(pl%status(:) == DISCARDED_RMIN) .or. any(pl%status(:) == DISCARDED_PERI)) then
+                  impactors%regime = REGIME_CB_IMPACT
+               else
+                  impactors%regime = REGIME_EJECTED
+               end if
+               call pl%save_discard(ldiscard,nbody_system,collider%before)
+               call collision_history%take_snapshot(param,nbody_system, t, "before") 
+
                call symba_discard_nonplpl_conservation(self, nbody_system, param)
 
                call pl%rearray(nbody_system, param)
 
+               ldiscard(:) = .false.
+               call pl%save_discard(ldiscard,nbody_system,collider%after) ! This ensures that the Sun gets saved in the "after" slot
+               call collision_history%take_snapshot(param,nbody_system, t, "after") 
+
                if (param%lenergy) then
+                  call collision_history%save_energy_snapshot("before", nbody_system, &
+                                                              collision_history%iframe,collision_history%iframe)
                   call nbody_system%get_energy_and_momentum(param)
                   E_orbit_after = nbody_system%te
                   nbody_system%E_collisions = nbody_system%E_collisions + (E_orbit_after - E_orbit_before)
+                  call collision_history%save_energy_snapshot("after", nbody_system, &
+                                                               collision_history%iframe,collision_history%iframe)
                end if
-
             end associate
          end select 
       end select
 
       return
    end subroutine symba_discard_pl
```

### Comparing `swiftest-2024.4.1/src/symba/symba_drift.f90` & `swiftest-2024.4.2/src/symba/symba_gr.f90`

 * *Files 17% similar despite different names*

```diff
@@ -3,61 +3,69 @@
 ! Swiftest is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License 
 ! as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 ! Swiftest is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty 
 ! of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 ! You should have received a copy of the GNU General Public License along with Swiftest. 
 ! If not, see: https://www.gnu.org/licenses. 
 
-  submodule (symba) s_symba_drift
+submodule(symba) s_symba_gr
    use swiftest
 contains
 
-   module subroutine symba_drift_pl(self, nbody_system, param, dt)
+   pure module subroutine symba_gr_p4_pl(self, nbody_system, param, dt)
       !! author: David A. Minton
       !!
-      !! Wrapper function used to call the body drift routine from a symba_pl structure
+      !! Position kick to massive bodies due to p**4 term in the post-Newtonian correction
+      !!    Based on Saha & Tremaine (1994) Eq. 28
+      !!
+      !! Adapted from David A. Minton's Swifter routine routine gr_symba_p4.f90
       implicit none
       ! Arguments
-      class(symba_pl),              intent(inout) :: self   !! Helio massive body object
+      class(symba_pl),              intent(inout) :: self   !! SyMBA massive body object
       class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
       class(swiftest_parameters),   intent(in)    :: param  !! Current run configuration parameters 
-      real(DP),                     intent(in)    :: dt     !! Stepsize
+      real(DP),                     intent(in)    :: dt     !! Step size
 
       if (self%nbody == 0) return
+
       associate(pl => self, npl => self%nbody)
          select type(nbody_system)
          class is (symba_nbody_system)
             pl%lmask(1:npl) = pl%status(1:npl) /= INACTIVE .and. pl%levelg(1:npl) == nbody_system%irec
-            call helio_drift_body(pl, nbody_system, param, dt)
+            call helio_gr_p4_pl(pl, nbody_system, param, dt)
             pl%lmask(1:npl) = pl%status(1:npl) /= INACTIVE 
          end select
       end associate
 
-      return
-   end subroutine symba_drift_pl
+   return
+   end subroutine symba_gr_p4_pl
 
 
-   module subroutine symba_drift_tp(self, nbody_system, param, dt)
+   pure module subroutine symba_gr_p4_tp(self, nbody_system, param, dt)
       !! author: David A. Minton
       !!
-      !! Wrapper function used to call the body drift routine from a symba_pl structure
+      !! Position kick to test particles due to p**4 term in the post-Newtonian correction
+      !!    Based on Saha & Tremaine (1994) Eq. 28
+      !!
+      !! Adapted from David A. Minton's Swifter routine routine gr_symba_p4.f90
       implicit none
       ! Arguments
-      class(symba_tp),              intent(inout) :: self   !! Helio massive body object
+      class(symba_tp),              intent(inout) :: self   !! SyMBA test particle object
       class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
       class(swiftest_parameters),   intent(in)    :: param  !! Current run configuration parameters 
-      real(DP),                     intent(in)    :: dt     !! Stepsize
+      real(DP),                     intent(in)    :: dt     !! Step size
 
       if (self%nbody == 0) return
-      associate (tp => self, ntp => self%nbody)
+
+      associate(tp => self, ntp => self%nbody)
          select type(nbody_system)
          class is (symba_nbody_system)
             tp%lmask(1:ntp) = tp%status(1:ntp) /= INACTIVE .and. tp%levelg(1:ntp) == nbody_system%irec
-            call helio_drift_body(tp, nbody_system, param, dt)
+            call helio_gr_p4_tp(tp, nbody_system, param, dt)
             tp%lmask(1:ntp) = tp%status(1:ntp) /= INACTIVE 
          end select
       end associate
 
-      return
-   end subroutine symba_drift_tp
+   return
+   end subroutine symba_gr_p4_tp
 
-end submodule s_symba_drift
+end submodule s_symba_gr
```

### Comparing `swiftest-2024.4.1/src/symba/symba_encounter_check.f90` & `swiftest-2024.4.2/src/symba/symba_encounter_check.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/symba/symba_gr.f90` & `swiftest-2024.4.2/src/whm/whm_drift.f90`

 * *Files 24% similar despite different names*

```diff
@@ -3,69 +3,58 @@
 ! Swiftest is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License 
 ! as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 ! Swiftest is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty 
 ! of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 ! You should have received a copy of the GNU General Public License along with Swiftest. 
 ! If not, see: https://www.gnu.org/licenses. 
 
-submodule(symba) s_symba_gr
+submodule(whm) whm_drift
    use swiftest
 contains
 
-   pure module subroutine symba_gr_p4_pl(self, nbody_system, param, dt)
+   module subroutine whm_drift_pl(self, nbody_system, param, dt)
       !! author: David A. Minton
       !!
-      !! Position kick to massive bodies due to p**4 term in the post-Newtonian correction
-      !!    Based on Saha & Tremaine (1994) Eq. 28
+      !! Loop through planets and call Danby drift routine
       !!
-      !! Adapted from David A. Minton's Swifter routine routine gr_symba_p4.f90
+      !! Adapted from Hal Levison's Swift routine drift.f
+      !! Adapted from David E. Kaufmann's Swifter routine whm_drift.f90
       implicit none
       ! Arguments
-      class(symba_pl),              intent(inout) :: self   !! SyMBA massive body object
-      class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(swiftest_parameters),   intent(in)    :: param  !! Current run configuration parameters 
-      real(DP),                     intent(in)    :: dt     !! Step size
+      class(whm_pl),                 intent(inout) :: self   !! WHM massive body particle data structure
+      class(swiftest_nbody_system),  intent(inout) :: nbody_system !! WHM nbody system object
+      class(swiftest_parameters),    intent(in)    :: param  !! Current run configuration parameters 
+      real(DP),                      intent(in)    :: dt     !! Stepsize
+      ! Internals
+      integer(I4B)                              :: i
+      integer(I4B), dimension(:), allocatable   :: iflag
+      character(len=STRMAX) :: message
 
       if (self%nbody == 0) return
 
       associate(pl => self, npl => self%nbody)
-         select type(nbody_system)
-         class is (symba_nbody_system)
-            pl%lmask(1:npl) = pl%status(1:npl) /= INACTIVE .and. pl%levelg(1:npl) == nbody_system%irec
-            call helio_gr_p4_pl(pl, nbody_system, param, dt)
-            pl%lmask(1:npl) = pl%status(1:npl) /= INACTIVE 
-         end select
+         allocate(iflag(npl))
+         iflag(:) = 0
+         call swiftest_drift_all(pl%muj, pl%xj, pl%vj, npl, param, dt, pl%lmask, iflag)
+         if (any(iflag(1:npl) /= 0)) then
+            where(iflag(1:npl) /= 0) 
+               pl%status(1:npl) = DISCARDED_DRIFTERR
+               pl%lmask(1:npl) = .false.
+            end where
+            do i = 1, npl
+               if (iflag(i) /= 0) then 
+                  write(message, *) " Planet ", pl%id(i), " is lost!!!!!!!!!!!!",new_line('A'), &
+                                      pl%muj(i), dt, new_line('A'), &
+                                      pl%xj(:,i),new_line('A'), &
+                                      pl%vj(:,i),new_line('A'), &
+                                    " STOPPING "
+                  call swiftest_io_log_one_message(COLLISION_LOG_OUT, message)
+               end if
+            end do
+            call base_util_exit(FAILURE,param%display_unit)
+         end if
       end associate
 
-   return
-   end subroutine symba_gr_p4_pl
+      return
+   end subroutine whm_drift_pl
 
-
-   pure module subroutine symba_gr_p4_tp(self, nbody_system, param, dt)
-      !! author: David A. Minton
-      !!
-      !! Position kick to test particles due to p**4 term in the post-Newtonian correction
-      !!    Based on Saha & Tremaine (1994) Eq. 28
-      !!
-      !! Adapted from David A. Minton's Swifter routine routine gr_symba_p4.f90
-      implicit none
-      ! Arguments
-      class(symba_tp),              intent(inout) :: self   !! SyMBA test particle object
-      class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-      class(swiftest_parameters),   intent(in)    :: param  !! Current run configuration parameters 
-      real(DP),                     intent(in)    :: dt     !! Step size
-
-      if (self%nbody == 0) return
-
-      associate(tp => self, ntp => self%nbody)
-         select type(nbody_system)
-         class is (symba_nbody_system)
-            tp%lmask(1:ntp) = tp%status(1:ntp) /= INACTIVE .and. tp%levelg(1:ntp) == nbody_system%irec
-            call helio_gr_p4_tp(tp, nbody_system, param, dt)
-            tp%lmask(1:ntp) = tp%status(1:ntp) /= INACTIVE 
-         end select
-      end associate
-
-   return
-   end subroutine symba_gr_p4_tp
-
-end submodule s_symba_gr
+end submodule whm_drift
```

### Comparing `swiftest-2024.4.1/src/symba/symba_kick.f90` & `swiftest-2024.4.2/src/symba/symba_kick.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/symba/symba_module.f90` & `swiftest-2024.4.2/src/symba/symba_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/symba/symba_step.f90` & `swiftest-2024.4.2/src/symba/symba_step.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/symba/symba_util.f90` & `swiftest-2024.4.2/src/symba/symba_util.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/tides/tides_getacch_pl.f90` & `swiftest-2024.4.2/src/tides/tides_getacch_pl.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/tides/tides_module.f90` & `swiftest-2024.4.2/src/tides/tides_module.f90`

 * *Files 2% similar despite different names*

```diff
@@ -65,28 +65,28 @@
       module function tides_derivs_eval(self, x, t) result(y)
          class(tides_derivs_func), intent(inout) :: self
          real(DP), dimension(:), intent(in) :: x
          real(DP),                 intent(in) :: t
          real(DP), dimension(:), allocatable  :: y
       end function tides_derivs_eval
 
-      module function tides_spin_derivs(rot_pl_cb, t, dt, rbeg, rend) result(drot) !! Need to add more arguments so we can pull in mass, radius, Ip, J2, etc...
+      module function tides_rot_derivs(rot_pl_cb, t, dt, rbeg, rend) result(drot) !! Need to add more arguments so we can pull in mass, radius, Ip, J2, etc...
          real(DP), dimension(:,:),     intent(in) :: rot_pl_cb !! Array of rotations. The last element is the central body, and all others are massive bodies
          real(DP),                     intent(in) :: t         !! Current time, which is used to interpolate the massive body positions
          real(DP),                     intent(in) :: dt        !! Total step size
          real(DP), dimension(:,:),     intent(in) :: rbeg
          real(DP), dimension(:,:),     intent(in) :: rend
          real(DP), dimension(:,:), allocatable    :: drot
-      end function tides_spin_derivs
+      end function tides_rot_derivs
 
-      module subroutine tides_step_spin_system(self, param, t, dt)
+      module subroutine tides_step_rot_system(self, param, t, dt)
          implicit none
          class(base_nbody_system), intent(inout) :: self   !! Swiftest nbody system object
          class(base_parameters),   intent(in)    :: param  !! Current run configuration parameters  
          real(DP),                     intent(in)    :: t     !! Simulation time
          real(DP),                     intent(in)    :: dt    !! Current stepsize
-      end subroutine tides_step_spin_system
+      end subroutine tides_step_rot_system
    
    end interface
 
 
 end module
```

### Comparing `swiftest-2024.4.1/src/tides/tides_spin_step.f90` & `swiftest-2024.4.2/src/tides/tides_spin_step.f90`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-submodule(tides) s_tides_step_spin
+submodule(tides) s_tides_step_rot
    use swiftest
 
 contains
 
-   module subroutine tides_step_spin_system(self, param, t, dt)
+   module subroutine tides_step_rot_system(self, param, t, dt)
       !! author: Jennifer L.L. Pouplin and David A. Minton
       !!
-      !! Integrates the spin equations for central and massive bodies of the nbody_system subjected to tides.
+      !! Integrates the rotation equations for central and massive bodies of the nbody_system subjected to tides.
       implicit none
       ! Arguments
       class(base_nbody_system), intent(inout) :: self   !! Swiftest nbody system object
       class(base_parameters),   intent(in)    :: param  !! Current run configuration parameters  
       real(DP),                     intent(in)    :: t     !! Simulation time
       real(DP),                     intent(in)    :: dt    !! Current stepsize
       ! Internals
@@ -20,28 +20,28 @@
       real(DP)                                  :: subdt 
 
       select type(self)
       class is (swiftest_nbody_system)
          associate(pl => self%pl, npl => self%pl%nbody, cb => self%cb)
             allocate(rot0(NDIM*(npl+1)))
             ! rot0 = [pack(pl%rot(:,1:npl),.true.), pack(cb%rot(:),.true.)]
-            ! Use this space call the ode_solver, passing tides_spin_derivs as the function:
+            ! Use this space call the ode_solver, passing tides_rot_derivs as the function:
             ! subdt = dt / 20._DP
-            ! rot1(:) = swiftest_util_solve_rkf45(lambda_obj(tides_spin_derivs, subdt, pl%rbeg, pl%rend), rot0, dt, subdt,tol)
+            ! rot1(:) = swiftest_util_solve_rkf45(lambda_obj(tides_rot_derivs, subdt, pl%rbeg, pl%rend), rot0, dt, subdt,tol)
             ! ! Recover with unpack
             ! pl%rot(:,1:npl) = unpack(rot1...
             ! cb%rot(:) = unpack(rot1...
          end associate
       end select
 
       return
-   end subroutine tides_step_spin_system
+   end subroutine tides_step_rot_system
 
 
-   module function tides_spin_derivs(rot_pl_cb, t, dt, rbeg, rend) result(drot) !! Need to add more arguments so we can pull in mass, radius, Ip, J2, etc...
+   module function tides_rot_derivs(rot_pl_cb, t, dt, rbeg, rend) result(drot) !! Need to add more arguments so we can pull in mass, radius, Ip, J2, etc...
       !! author: Jennifer L.L. Pouplin and David A. Minton
       !!
       !! function used to calculate the derivatives that are fed to the ODE solver
       implicit none
       ! Arguments
       real(DP), dimension(:,:),     intent(in) :: rot_pl_cb !! Array of rotations. The last element is the central body, and all others are massive bodies
       real(DP),                     intent(in) :: t         !! Current time, which is used to interpolate the massive body positions
@@ -65,15 +65,15 @@
          ! Calculate Ncb and Npl as a function of xinterp
          !drot(:,i) = -Mcb / (Mcb + Mpl(i)) * (N_Tpl + N_Rpl)
          !drot(:,n) = drot(:,n) - Mcb / (Mcb + Mpl(i) * (N_Tcb + N_Rcb)
          !
       end do
 
       return
-   end function tides_spin_derivs
+   end function tides_rot_derivs
 
    module function tides_derivs_eval(self, x, t) result(y)
       implicit none
       ! Arguments
       class(tides_derivs_func), intent(inout) :: self
       real(DP), dimension(:), intent(in) :: x
       real(DP),                 intent(in) :: t
@@ -101,8 +101,8 @@
       f%dt = dt
       allocate(f%rbeg, source = rbeg)
       allocate(f%rend, source = rend)
 
       return
    end function tides_derivs_init
 
-end submodule s_tides_step_spin
+end submodule s_tides_step_rot
```

### Comparing `swiftest-2024.4.1/src/walltime/walltime_implementations.f90` & `swiftest-2024.4.2/src/walltime/walltime_implementations.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/walltime/walltime_module.f90` & `swiftest-2024.4.2/src/walltime/walltime_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/whm/whm_coord.f90` & `swiftest-2024.4.2/src/whm/whm_coord.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/whm/whm_gr.f90` & `swiftest-2024.4.2/src/whm/whm_gr.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/whm/whm_kick.f90` & `swiftest-2024.4.2/src/whm/whm_kick.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/src/whm/whm_module.f90` & `swiftest-2024.4.2/src/whm/whm_module.f90`

 * *Files 20% similar despite different names*

```diff
@@ -20,310 +20,510 @@
    type, extends(swiftest_cb) :: whm_cb
    contains
    end type whm_cb
 
 
    !> WHM massive body particle class
    type, extends(swiftest_pl) :: whm_pl
-      real(DP), dimension(:),   allocatable :: eta    !! Jacobi mass
-      real(DP), dimension(:,:), allocatable :: xj     !! Jacobi position
-      real(DP), dimension(:,:), allocatable :: vj     !! Jacobi velocity
-      real(DP), dimension(:),   allocatable :: muj    !! Jacobi mu: GMcb * eta(i) / eta(i - 1) 
-      real(DP), dimension(:),   allocatable :: ir3j    !! Third term of heliocentric acceleration
-      !! Note to developers: If you add componenets to this class, be sure to update methods and subroutines that traverse the
-      !!    component list, such as whm_util_setup_pl and whm_util_spill_pl
+      real(DP), dimension(:),   allocatable :: eta    
+         !! Jacobi mass
+      real(DP), dimension(:,:), allocatable :: xj     
+         !! Jacobi position
+      real(DP), dimension(:,:), allocatable :: vj     
+         !! Jacobi velocity
+      real(DP), dimension(:),   allocatable :: muj    
+         !! Jacobi mu: GMcb * eta(i) / eta(i - 1) 
+      real(DP), dimension(:),   allocatable :: ir3j    
+         !! Third term of heliocentric acceleration
+      ! Note to developers: If you add componenets to this class, be sure to update methods and subroutines that traverse the
+      !    component list, such as whm_util_setup_pl and whm_util_spill_pl
    contains
-      procedure :: h2j         => whm_coord_h2j_pl           !! Convert position and velcoity vectors from heliocentric to Jacobi coordinates 
-      procedure :: j2h         => whm_coord_j2h_pl           !! Convert position and velcoity vectors from Jacobi to helliocentric coordinates 
-      procedure :: vh2vj       => whm_coord_vh2vj_pl         !! Convert velocity vectors from heliocentric to Jacobi coordinates 
-      procedure :: drift       => whm_drift_pl               !! Loop through massive bodies and call Danby drift routine to jacobi coordinates
-      procedure :: accel_gr    => whm_gr_kick_getacch_pl     !! Acceleration term arising from the post-Newtonian correction
-      procedure :: gr_pos_kick => whm_gr_p4_pl               !! Position kick due to p**4 term in the post-Newtonian correction
-      procedure :: accel       => whm_kick_getacch_pl        !! Compute heliocentric accelerations of massive bodies
-      procedure :: kick        => whm_kick_vh_pl             !! Kick heliocentric velocities of massive bodies
-      procedure :: append      => whm_util_append_pl         !! Appends elements from one structure to another
-      procedure :: dealloc     => whm_util_dealloc_pl        !! Deallocates all allocatable arrays
-      procedure :: fill        => whm_util_fill_pl           !! "Fills" bodies from one object into another depending on the results of a mask (uses the UNPACK intrinsic)
-      procedure :: resize      => whm_util_resize_pl         !! Checks the current size of a Swiftest body against the requested size and resizes it if it is too small.
-      procedure :: set_ir3     => whm_util_set_ir3j          !! Sets both the heliocentric and jacobi inverse radius terms (1/rj**3 and 1/rh**3)
-      procedure :: set_mu      => whm_util_set_mu_eta_pl     !! Sets the Jacobi mass value for all massive bodies.
-      procedure :: sort        => whm_util_sort_pl           !! Sort a WHM massive body object in-place. 
-      procedure :: rearrange   => whm_util_sort_rearrange_pl !! Rearranges the order of array elements of body based on an input index array. Used in sorting methods
-      procedure :: spill       => whm_util_spill_pl          !! "Spills" bodies from one object to another depending on the results of a mask (uses the PACK intrinsic)
-      procedure :: setup       => whm_util_setup_pl          !! Constructor method - Allocates space for the input number of bodiess
-      procedure :: step        => whm_step_pl                !! Steps the body forward one stepsize
-      final     ::                whm_final_pl               !! Finalizes the WHM massive body object - deallocates all allocatables
-#ifdef COARRAY
-      procedure :: coclone      => whm_coarray_coclone_pl       !! Clones the image 1 body object to all other images in the coarray structure.
-#endif 
+      procedure :: h2j         => whm_coord_h2j_pl           
+         !! Convert position and velcoity vectors from heliocentric to Jacobi coordinates 
+      procedure :: j2h         => whm_coord_j2h_pl           
+         !! Convert position and velcoity vectors from Jacobi to helliocentric coordinates 
+      procedure :: vh2vj       => whm_coord_vh2vj_pl         
+         !! Convert velocity vectors from heliocentric to Jacobi coordinates 
+      procedure :: drift       => whm_drift_pl               
+         !! Loop through massive bodies and call Danby drift routine to jacobi coordinates
+      procedure :: accel_gr    => whm_gr_kick_getacch_pl     
+         !! Acceleration term arising from the post-Newtonian correction
+      procedure :: gr_pos_kick => whm_gr_p4_pl               
+         !! Position kick due to p**4 term in the post-Newtonian correction
+      procedure :: accel       => whm_kick_getacch_pl        
+         !! Compute heliocentric accelerations of massive bodies
+      procedure :: kick        => whm_kick_vh_pl             
+         !! Kick heliocentric velocities of massive bodies
+      procedure :: append      => whm_util_append_pl         
+         !! Appends elements from one structure to another
+      procedure :: dealloc     => whm_util_dealloc_pl        
+         !! Deallocates all allocatable arrays
+      procedure :: fill        => whm_util_fill_pl           
+         !! "Fills" bodies from one object into another depending on the results of a mask (uses the UNPACK intrinsic)
+      procedure :: resize      => whm_util_resize_pl         
+         !! Checks the current size of a Swiftest body against the requested size and resizes it if it is too small.
+      procedure :: set_ir3     => whm_util_set_ir3j          
+         !! Sets both the heliocentric and jacobi inverse radius terms (1/rj**3 and 1/rh**3)
+      procedure :: set_mu      => whm_util_set_mu_eta_pl     
+         !! Sets the Jacobi mass value for all massive bodies.
+      procedure :: sort        => whm_util_sort_pl           
+         !! Sort a WHM massive body object in-place. 
+      procedure :: rearrange   => whm_util_sort_rearrange_pl 
+         !! Rearranges the order of array elements of body based on an input index array. Used in sorting methods
+      procedure :: spill       => whm_util_spill_pl          
+         !! "Spills" bodies from one object to another depending on the results of a mask (uses the PACK intrinsic)
+      procedure :: setup       => whm_util_setup_pl          
+         !! Constructor method - Allocates space for the input number of bodiess
+      procedure :: step        => whm_step_pl                
+         !! Steps the body forward one stepsize
+      final     ::                whm_final_pl               
+         !! Finalizes the WHM massive body object - deallocates all allocatables
    end type whm_pl
 
 
-   !! WHM test particle class
+   !> WHM test particle class
    type, extends(swiftest_tp) :: whm_tp
-      !! Note to developers: If you add componenets to this class, be sure to update methods and subroutines that traverse the
-      !!    component list, such as whm_util_spill_tp
+      ! Note to developers: If you add componenets to this class, be sure to update methods and subroutines that traverse the
+      !    component list, such as whm_util_spill_tp
    contains
-      procedure :: accel_gr    => whm_gr_kick_getacch_tp !! Acceleration term arising from the post-Newtonian correction
-      procedure :: gr_pos_kick => whm_gr_p4_tp           !! Position kick due to p**4 term in the post-Newtonian correction
-      procedure :: accel       => whm_kick_getacch_tp    !! Compute heliocentric accelerations of test particles
-      procedure :: kick        => whm_kick_vh_tp         !! Kick heliocentric velocities of test particles
-      procedure :: step        => whm_step_tp            !! Steps the particle forward one stepsize
-      final     ::                whm_final_tp      !! Finalizes the WHM test particle object - deallocates all allocatables 
+      procedure :: accel_gr    => whm_gr_kick_getacch_tp 
+         !! Acceleration term arising from the post-Newtonian correction
+      procedure :: gr_pos_kick => whm_gr_p4_tp           
+         !! Position kick due to p**4 term in the post-Newtonian correction
+      procedure :: accel       => whm_kick_getacch_tp    
+         !! Compute heliocentric accelerations of test particles
+      procedure :: kick        => whm_kick_vh_tp         
+         !! Kick heliocentric velocities of test particles
+      procedure :: step        => whm_step_tp            
+         !! Steps the particle forward one stepsize
+      final     ::                whm_final_tp      
+         !! Finalizes the WHM test particle object - deallocates all allocatables 
    end type whm_tp
 
    !> An abstract class for the WHM integrator nbody system 
    type, extends(swiftest_nbody_system) :: whm_nbody_system
    contains
-      !> Replace the abstract procedures with concrete ones
-      procedure :: initialize   => whm_util_setup_initialize_system !! Performs WHM-specific initilization steps, like calculating the Jacobi masses
-      procedure :: step         => whm_step_system             !! Advance the WHM nbody system forward in time by one step
-      final     ::                 whm_final_system       !! Finalizes the WHM nbody_system object - deallocates all allocatables 
+      ! Replace the abstract procedures with concrete ones
+      procedure :: initialize   => whm_util_setup_initialize_system 
+         !! Performs WHM-specific initilization steps, like calculating the Jacobi masses
+      procedure :: step         => whm_step_system             
+         !! Advance the WHM nbody system forward in time by one step
+      final     ::                 whm_final_system       
+         !! Finalizes the WHM nbody_system object - deallocates all allocatables 
    end type whm_nbody_system
 
    interface
       module subroutine whm_coord_h2j_pl(self, cb)
          implicit none
-         class(whm_pl),      intent(inout) :: self   !! WHM massive body particle data structure
-         class(swiftest_cb), intent(inout) :: cb     !! Swiftest central body particle data structuree
+         class(whm_pl),      intent(inout) :: self   
+            !! WHM massive body particle data structure
+         class(swiftest_cb), intent(inout) :: cb     
+            !! Swiftest central body particle data structuree
       end subroutine whm_coord_h2j_pl
 
       module subroutine whm_coord_j2h_pl(self, cb)
          implicit none
-         class(whm_pl),      intent(inout) :: self   !! WHM massive body particle data structure
-         class(swiftest_cb), intent(inout) :: cb     !! Swiftest central body particle data structuree
+         class(whm_pl),      intent(inout) :: self   
+            !! WHM massive body particle data structure
+         class(swiftest_cb), intent(inout) :: cb     
+            !! Swiftest central body particle data structuree
       end subroutine whm_coord_j2h_pl
 
       module subroutine whm_coord_vh2vj_pl(self, cb)
          implicit none
-         class(whm_pl),      intent(inout) :: self   !! WHM massive body particle data structure
-         class(swiftest_cb), intent(inout) :: cb     !! Swiftest central body particle data structuree
+         class(whm_pl),      intent(inout) :: self   
+            !! WHM massive body particle data structure
+         class(swiftest_cb), intent(inout) :: cb     
+            !! Swiftest central body particle data structuree
       end subroutine whm_coord_vh2vj_pl
 
       module subroutine whm_drift_pl(self, nbody_system, param, dt)
          implicit none
-         class(whm_pl),                intent(inout) :: self   !! WHM massive body particle data structure
-         class(swiftest_nbody_system), intent(inout) :: nbody_system !! WHM nbody system object
-         class(swiftest_parameters),   intent(in)    :: param  !! Current run configuration parameters 
-         real(DP),                     intent(in)    :: dt     !! Stepsize
+         class(whm_pl),                intent(inout) :: self   
+            !! WHM massive body particle data structure
+         class(swiftest_nbody_system), intent(inout) :: nbody_system 
+            !! WHM nbody system object
+         class(swiftest_parameters),   intent(in)    :: param  
+            !! Current run configuration parameters 
+         real(DP),                     intent(in)    :: dt     
+            !! Stepsize
       end subroutine whm_drift_pl
 
       !> Get heliocentric accelration of massive bodies
       module subroutine whm_kick_getacch_pl(self, nbody_system, param, t, lbeg)
          implicit none
-         class(whm_pl),                intent(inout) :: self   !! WHM massive body particle data structure
-         class(swiftest_nbody_system), intent(inout) :: nbody_system !! WHM nbody system object
-         class(swiftest_parameters),   intent(inout) :: param  !! Current run configuration parameters 
-         real(DP),                     intent(in)    :: t      !! Current simulation time
-         logical,                      intent(in)    :: lbeg   !! Logical flag that determines whether or not this is the beginning or end of the step
+         class(whm_pl),                intent(inout) :: self   
+            !! WHM massive body particle data structure
+         class(swiftest_nbody_system), intent(inout) :: nbody_system 
+            !! WHM nbody system object
+         class(swiftest_parameters),   intent(inout) :: param  
+            !! Current run configuration parameters 
+         real(DP),                     intent(in)    :: t      
+            !! Current simulation time
+         logical,                      intent(in)    :: lbeg   
+            !! Logical flag that determines whether or not this is the beginning or end of the step
       end subroutine whm_kick_getacch_pl
 
       !> Get heliocentric accelration of the test particle
       module subroutine whm_kick_getacch_tp(self, nbody_system, param, t, lbeg)
          implicit none
-         class(whm_tp),                intent(inout) :: self   !! WHM test particle data structure
-         class(swiftest_nbody_system), intent(inout) :: nbody_system !! WHM nbody system object
-         class(swiftest_parameters),   intent(inout) :: param  !! Current run configuration parameters
-         real(DP),                     intent(in)    :: t      !! Current time
-         logical,                      intent(in)    :: lbeg   !! Logical flag that determines whether or not this is the beginning or end of the step
+         class(whm_tp),                intent(inout) :: self   
+            !! WHM test particle data structure
+         class(swiftest_nbody_system), intent(inout) :: nbody_system 
+            !! WHM nbody system object
+         class(swiftest_parameters),   intent(inout) :: param  
+            !! Current run configuration parameters
+         real(DP),                     intent(in)    :: t      
+            !! Current time
+         logical,                      intent(in)    :: lbeg   
+            !! Logical flag that determines whether or not this is the beginning or end of the step
       end subroutine whm_kick_getacch_tp
 
       module subroutine whm_kick_vh_pl(self, nbody_system, param, t, dt, lbeg)
          implicit none
-         class(whm_pl),                intent(inout) :: self   !! WHM massive body object
-         class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-         class(swiftest_parameters),   intent(inout) :: param  !! Current run configuration parameters 
-         real(DP),                     intent(in)    :: t      !! Current time
-         real(DP),                     intent(in)    :: dt     !! Stepsize
-         logical,                      intent(in)    :: lbeg   !! Logical flag indicating whether this is the beginning of the half step or not. 
+         class(whm_pl),                intent(inout) :: self   
+            !! WHM massive body object
+         class(swiftest_nbody_system), intent(inout) :: nbody_system 
+            !! Swiftest nbody system object
+         class(swiftest_parameters),   intent(inout) :: param  
+            !! Current run configuration parameters 
+         real(DP),                     intent(in)    :: t      
+            !! Current time
+         real(DP),                     intent(in)    :: dt     
+            !! Stepsize
+         logical,                      intent(in)    :: lbeg   
+            !! Logical flag indicating whether this is the beginning of the half step or not. 
       end subroutine whm_kick_vh_pl
 
       module subroutine whm_kick_vh_tp(self, nbody_system, param, t, dt, lbeg)
          implicit none
-         class(whm_tp),                intent(inout) :: self   !! WHM test particle object
-         class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-         class(swiftest_parameters),   intent(inout) :: param  !! Current run configuration parameters 
-         real(DP),                     intent(in)    :: t      !! Current time
-         real(DP),                     intent(in)    :: dt     !! Stepsize
-         logical,                      intent(in)    :: lbeg   !! Logical flag indicating whether this is the beginning of the half step or not. 
+         class(whm_tp),                intent(inout) :: self   
+            !! WHM test particle object
+         class(swiftest_nbody_system), intent(inout) :: nbody_system 
+            !! Swiftest nbody system object
+         class(swiftest_parameters),   intent(inout) :: param  
+            !! Current run configuration parameters 
+         real(DP),                     intent(in)    :: t      
+            !! Current time
+         real(DP),                     intent(in)    :: dt     
+            !! Stepsize
+         logical,                      intent(in)    :: lbeg   
+            !! Logical flag indicating whether this is the beginning of the half step or not. 
       end subroutine whm_kick_vh_tp
 
       pure module subroutine whm_gr_kick_getacch_pl(self, param)
          implicit none
-         class(whm_pl),              intent(inout) :: self  !! WHM massive body particle data structure
-         class(swiftest_parameters), intent(in)    :: param !! Current run configuration parameters 
+         class(whm_pl),              intent(inout) :: self  
+            !! WHM massive body particle data structure
+         class(swiftest_parameters), intent(in)    :: param 
+            !! Current run configuration parameters 
       end subroutine whm_gr_kick_getacch_pl
 
       pure module subroutine whm_gr_kick_getacch_tp(self, param)
          implicit none
-         class(whm_tp),              intent(inout) :: self  !! WHM test particle data structure
-         class(swiftest_parameters), intent(in)    :: param !! Current run configuration parameters
+         class(whm_tp),              intent(inout) :: self  
+            !! WHM test particle data structure
+         class(swiftest_parameters), intent(in)    :: param 
+            !! Current run configuration parameters
       end subroutine whm_gr_kick_getacch_tp
 
       pure module subroutine whm_gr_p4_pl(self, nbody_system, param, dt)
          implicit none
-         class(whm_pl),                intent(inout) :: self  !! WHM massive body object
-         class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system
-         class(swiftest_parameters),   intent(in)    :: param !! Current run configuration parameters 
-         real(DP),                     intent(in)    :: dt    !! Step size
+         class(whm_pl),                intent(inout) :: self  
+            !! WHM massive body object
+         class(swiftest_nbody_system), intent(inout) :: nbody_system 
+            !! Swiftest nbody system
+         class(swiftest_parameters),   intent(in)    :: param 
+            !! Current run configuration parameters 
+         real(DP),                     intent(in)    :: dt    
+            !! Step size
       end subroutine whm_gr_p4_pl
 
       pure module subroutine whm_gr_p4_tp(self, nbody_system, param, dt)
          implicit none
-         class(whm_tp),                intent(inout) :: self   !! WHM test particle object
-         class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system
-         class(swiftest_parameters),   intent(in)    :: param  !! Current run configuration parameters 
-         real(DP),                     intent(in)    :: dt     !! Step size
+         class(whm_tp),                intent(inout) :: self   
+            !! WHM test particle object
+         class(swiftest_nbody_system), intent(inout) :: nbody_system 
+            !! Swiftest nbody system
+         class(swiftest_parameters),   intent(in)    :: param  
+            !! Current run configuration parameters 
+         real(DP),                     intent(in)    :: dt     
+            !! Step size
       end subroutine whm_gr_p4_tp
 
       !> Reads WHM massive body object in from file
       module subroutine whm_util_setup_pl(self, n, param)
          implicit none
-         class(whm_pl),             intent(inout) :: self  !! WHM massive body objectobject
-         integer(I4B),              intent(in)    :: n     !! Number of particles to allocate space for
-         class(swiftest_parameters), intent(in)    :: param !! Current run configuration parameters
+         class(whm_pl),             intent(inout) :: self  
+            !! WHM massive body objectobject
+         integer(I4B),              intent(in)    :: n     
+            !! Number of particles to allocate space for
+         class(swiftest_parameters), intent(in)    :: param 
+            !! Current run configuration parameters
       end subroutine whm_util_setup_pl
 
       module subroutine whm_util_setup_initialize_system(self, system_history, param)
          implicit none
-         class(whm_nbody_system),                 intent(inout) :: self            !! WHM nbody system object
-         class(swiftest_storage),    allocatable, intent(inout) :: system_history  !! Stores the system history between output dumps
-         class(swiftest_parameters),              intent(inout) :: param           !! Current run configuration parameters 
+         class(whm_nbody_system),                 intent(inout) :: self            
+            !! WHM nbody system object
+         class(swiftest_storage),    allocatable, intent(inout) :: system_history  
+            !! Stores the system history between output dumps
+         class(swiftest_parameters),              intent(inout) :: param           
+            !! Current run configuration parameters 
       end subroutine whm_util_setup_initialize_system
 
       module subroutine whm_step_pl(self, nbody_system, param, t, dt)
          implicit none
-         class(whm_pl),                intent(inout) :: self   !! WHM massive body object
-         class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody_system object
-         class(swiftest_parameters),   intent(inout) :: param  !! Current run configuration parameters 
-         real(DP),                     intent(in)    :: t       !! Simulation time
-         real(DP),                     intent(in)    :: dt     !! Current stepsize
+         class(whm_pl),                intent(inout) :: self   
+            !! WHM massive body object
+         class(swiftest_nbody_system), intent(inout) :: nbody_system 
+            !! Swiftest nbody_system object
+         class(swiftest_parameters),   intent(inout) :: param  
+            !! Current run configuration parameters 
+         real(DP),                     intent(in)    :: t       
+            !! Simulation time
+         real(DP),                     intent(in)    :: dt     
+            !! Current stepsize
       end subroutine whm_step_pl
 
       module subroutine whm_step_system(self, param, t, dt)
          implicit none
-         class(whm_nbody_system),    intent(inout) :: self    !! WHM nbody_system object
-         class(swiftest_parameters), intent(inout) :: param  !! Current run configuration parameters 
-         real(DP),                   intent(in)    :: t      !! Simulation time
-         real(DP),                   intent(in)    :: dt     !! Current stepsize
+         class(whm_nbody_system),    intent(inout) :: self    
+            !! WHM nbody_system object
+         class(swiftest_parameters), intent(inout) :: param  
+            !! Current run configuration parameters 
+         real(DP),                   intent(in)    :: t      
+            !! Simulation time
+         real(DP),                   intent(in)    :: dt     
+            !! Current stepsize
       end subroutine whm_step_system
 
       module subroutine whm_step_tp(self, nbody_system, param, t, dt)
          implicit none
-         class(whm_tp),                intent(inout) :: self   !! WHM test particle data structure
-         class(swiftest_nbody_system), intent(inout) :: nbody_system !! Swiftest nbody system object
-         class(swiftest_parameters),   intent(inout) :: param  !! Current run configuration parameters
-         real(DP),                     intent(in)    :: t      !! Current simulation time
-         real(DP),                     intent(in)    :: dt     !! Stepsize
+         class(whm_tp),                intent(inout) :: self   
+            !! WHM test particle data structure
+         class(swiftest_nbody_system), intent(inout) :: nbody_system 
+            !! Swiftest nbody system object
+         class(swiftest_parameters),   intent(inout) :: param  
+            !! Current run configuration parameters
+         real(DP),                     intent(in)    :: t      
+            !! Current simulation time
+         real(DP),                     intent(in)    :: dt     
+            !! Stepsize
       end subroutine whm_step_tp
 
       module subroutine whm_util_append_pl(self, source, lsource_mask)
          implicit none
-         class(whm_pl),                   intent(inout) :: self         !! WHM massive body object
-         class(swiftest_body),            intent(in)    :: source       !! Source object to append
-         logical, dimension(:),           intent(in)    :: lsource_mask !! Logical mask indicating which elements to append to
+         class(whm_pl),                   intent(inout) :: self         
+            !! WHM massive body object
+         class(swiftest_body),            intent(in)    :: source       
+            !! Source object to append
+         logical, dimension(:),           intent(in)    :: lsource_mask 
+            !! Logical mask indicating which elements to append to
       end subroutine whm_util_append_pl
 
       module subroutine whm_util_dealloc_pl(self)
          implicit none
-         class(whm_pl),  intent(inout) :: self !! WHM massive body object
+         class(whm_pl),  intent(inout) :: self 
+            !! WHM massive body object
       end subroutine whm_util_dealloc_pl
 
       module subroutine whm_util_spill_pl(self, discards, lspill_list, ldestructive)
          implicit none
-         class(whm_pl),         intent(inout) :: self        !! WHM massive body object
-         class(swiftest_body),      intent(inout) :: discards    !! Discarded object 
-         logical, dimension(:), intent(in)    :: lspill_list !! Logical array of bodies to spill into the discards
-         logical,               intent(in)    :: ldestructive !! Logical flag indicating whether or not this operation should alter the keeps array or not
+         class(whm_pl),         intent(inout) :: self        
+            !! WHM massive body object
+         class(swiftest_body),      intent(inout) :: discards    
+            !! Discarded object 
+         logical, dimension(:), intent(in)    :: lspill_list 
+            !! Logical array of bodies to spill into the discards
+         logical,               intent(in)    :: ldestructive 
+            !! Logical flag indicating whether or not this operation should alter the keeps array or not
       end subroutine whm_util_spill_pl
 
       module subroutine whm_util_fill_pl(self, inserts, lfill_list)
          implicit none
-         class(whm_pl),         intent(inout) :: self       !! WHM massive body object
-         class(swiftest_body),  intent(in)    :: inserts    !! inserted object 
-         logical, dimension(:), intent(in)    :: lfill_list !! Logical array of bodies to merge into the keeps
+         class(whm_pl),         intent(inout) :: self       
+            !! WHM massive body object
+         class(swiftest_body),  intent(in)    :: inserts    
+            !! inserted object 
+         logical, dimension(:), intent(in)    :: lfill_list 
+            !! Logical array of bodies to merge into the keeps
       end subroutine whm_util_fill_pl
 
       module subroutine whm_util_resize_pl(self, nnew)
          implicit none
-         class(whm_pl), intent(inout) :: self  !! WHM massive body object
-         integer(I4B),  intent(in)    :: nnew  !! New size neded
+         class(whm_pl), intent(inout) :: self  
+            !! WHM massive body object
+         integer(I4B),  intent(in)    :: nnew  
+            !! New size neded
       end subroutine whm_util_resize_pl
 
       module subroutine whm_util_set_ir3j(self)
          implicit none
-         class(whm_pl),                intent(inout) :: self    !! WHM massive body object
+         class(whm_pl),                intent(inout) :: self    
+            !! WHM massive body object
       end subroutine whm_util_set_ir3j
 
       module subroutine whm_util_set_mu_eta_pl(self, cb)
          implicit none
-         class(whm_pl),                intent(inout) :: self    !! WHM massive body object
-         class(swiftest_cb),           intent(inout) :: cb     !! Swiftest central body object
+         class(whm_pl),                intent(inout) :: self    
+            !! WHM massive body object
+         class(swiftest_cb),           intent(inout) :: cb     
+            !! Swiftest central body object
       end subroutine whm_util_set_mu_eta_pl
 
       module subroutine whm_util_sort_pl(self, sortby, ascending)
          implicit none
-         class(whm_pl), intent(inout) :: self        !! WHM massive body object
-         character(*),  intent(in)    :: sortby    !! Sorting attribute
-         logical,       intent(in)    :: ascending !! Logical flag indicating whether or not the sorting should be in ascending or descending order
+         class(whm_pl), intent(inout) :: self       
+             !! WHM massive body object
+         character(*),  intent(in)    :: sortby    
+            !! Sorting attribute
+         logical,       intent(in)    :: ascending 
+            !! Logical flag indicating whether or not the sorting should be in ascending or descending order
       end subroutine whm_util_sort_pl
 
       module subroutine whm_util_sort_rearrange_pl(self, ind)
          implicit none
-         class(whm_pl),               intent(inout) :: self !! WHM massive body object
-         integer(I4B),  dimension(:), intent(in)    :: ind  !! Index array used to restructure the body (should contain all 1:n index values in the desired order)
+         class(whm_pl),               intent(inout) :: self 
+            !! WHM massive body object
+         integer(I4B),  dimension(:), intent(in)    :: ind  
+            !! Index array used to restructure the body (should contain all 1:n index values in the desired order)
       end subroutine whm_util_sort_rearrange_pl
    end interface
 
 #ifdef COARRAY
-   interface
-      module subroutine whm_coarray_coclone_pl(self)
-         implicit none
-         class(whm_pl),intent(inout),codimension[*]  :: self  !! WHM pl object
-      end subroutine whm_coarray_coclone_pl
+   interface coclone
+      module procedure whm_coarray_coclone_tp
+   end interface
+
+   interface cocollect
+      module procedure whm_coarray_cocollect_tp
    end interface
 #endif
 
    contains
 
       subroutine whm_final_pl(self)
          !! author: David A. Minton
          !!
          !! Finalize the WHM massive body object - deallocates all allocatables
          implicit none
          ! Argument
-         type(whm_pl),  intent(inout) :: self !! WHM massive body object
-
+         type(whm_pl),  intent(inout) :: self 
+            !! WHM massive body object
          call self%dealloc()
-
          return
       end subroutine whm_final_pl
 
 
       subroutine whm_final_system(self)
          !! author: David A. Minton
          !!
          !! Finalize the WHM nbody system object - deallocates all allocatables
          implicit none
          ! Arguments
-         type(whm_nbody_system),  intent(inout) :: self !! WHM nbody system object
-
+         type(whm_nbody_system),  intent(inout) :: self 
+            !! WHM nbody system object
          call self%dealloc()
-
          return
       end subroutine whm_final_system
 
 
       subroutine whm_final_tp(self)
          !! author: David A. Minton
          !!
          !! Finalize the WHM test particle object - deallocates all allocatables
          implicit none
          ! Arguments
-         type(whm_tp),  intent(inout) :: self !! WHM test particle object
-
+         type(whm_tp),  intent(inout) :: self 
+            !! WHM test particle object
          call self%dealloc()
-
          return
       end subroutine whm_final_tp
 
+#ifdef COARRAY
+
+   subroutine whm_coarray_coclone_tp(tp)
+      !! author: David A. Minton
+      !!
+      !! Broadcasts the image 1 object to all other images in a coarray 
+      implicit none
+      ! Arguments
+      type(whm_tp),intent(inout),codimension[*]  :: tp  !! WHM tp object
+
+      call co_broadcast(tp%lfirst,1)
+      call co_broadcast(tp%nbody,1)
+      call coclone(tp%id)
+      call coclone(tp%info)
+      call coclone(tp%lmask)
+      call coclone(tp%status)
+      call coclone(tp%ldiscard)
+      call coclone(tp%lcollision)
+      call coclone(tp%lencounter)
+      call coclone(tp%mu)
+      call coclone(tp%rh)
+      call coclone(tp%vh)
+      call coclone(tp%rb)
+      call coclone(tp%vb)
+      call coclone(tp%ah)
+      call coclone(tp%aobl)
+      call coclone(tp%agr)
+      call coclone(tp%atide)
+      call coclone(tp%isperi)
+      call coclone(tp%peri)
+      call coclone(tp%atp)
+      call coclone(tp%a)
+      call coclone(tp%e)
+      call coclone(tp%inc)
+      call coclone(tp%capom)
+      call coclone(tp%omega)
+      call coclone(tp%capm) 
+      call coclone(tp%nplenc)
+
+      return
+   end subroutine whm_coarray_coclone_tp
+
+
+   subroutine whm_coarray_cocollect_tp(tp)
+      !! author: David A. Minton
+      !!
+      !! Collects all object array components from all images and combines them into the image 1 object
+      implicit none
+      ! Arguments
+      type(whm_tp),intent(inout),codimension[*]  :: tp  !! Swiftest body object
+
+      call co_sum(tp%npltp,1)
+      call cocollect(tp%nplenc)
+      call co_sum(tp%nbody,1)
+      call cocollect(tp%id)
+      call cocollect(tp%info)
+      call cocollect(tp%lmask)
+      call cocollect(tp%status)
+      call cocollect(tp%ldiscard)
+      call cocollect(tp%lcollision)
+      call cocollect(tp%lencounter)
+      call cocollect(tp%mu)
+      call cocollect(tp%rh)
+      call cocollect(tp%vh)
+      call cocollect(tp%rb)
+      call cocollect(tp%vb)
+      call cocollect(tp%ah)
+      call cocollect(tp%aobl)
+      call cocollect(tp%agr)
+      call cocollect(tp%atide)
+      call cocollect(tp%ir3h)
+      call cocollect(tp%isperi)
+      call cocollect(tp%peri)
+      call cocollect(tp%atp)
+      call cocollect(tp%a)
+      call cocollect(tp%e)
+      call cocollect(tp%inc)
+      call cocollect(tp%capom)
+      call cocollect(tp%omega)
+      call cocollect(tp%capm)
+
+      return
+   end subroutine whm_coarray_cocollect_tp
+
+#endif
+
 end module whm
```

### Comparing `swiftest-2024.4.1/src/whm/whm_step.f90` & `swiftest-2024.4.2/src/whm/whm_step.f90`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
       real(DP),                   intent(in)    :: dt    !! Current stepsize
 
       associate(nbody_system => self, cb => self%cb, pl => self%pl, tp => self%tp)
          tp%lfirst = pl%lfirst
          call pl%step(nbody_system, param, t, dt)
          call tp%step(nbody_system, param, t, dt)
          call cb%rotphase_update(param, dt)
-         ! if (param%ltides) call nbody_system%step_spin(param, t, dt)
+         ! if (param%ltides) call nbody_system%step_rot(param, t, dt)
 
       end associate
       return
    end subroutine whm_step_system 
 
 
    module subroutine whm_step_pl(self, nbody_system, param, t, dt)
```

### Comparing `swiftest-2024.4.1/src/whm/whm_util.f90` & `swiftest-2024.4.2/src/whm/whm_util.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/swiftest/CMakeLists.txt` & `swiftest-2024.4.2/swiftest/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 EXECUTE_PROCESS(
   COMMAND "${Python_EXECUTABLE}"
   -c "import numpy; print(numpy.get_include())"
   OUTPUT_VARIABLE NUMPY_INCLUDE_DIR
   OUTPUT_STRIP_TRAILING_WHITESPACE
 )
 
-TARGET_LINK_LIBRARIES(${CORE} PUBLIC ${SWIFTEST_LIBRARY} netCDF::netcdff HDF5::HDF5)
+TARGET_LINK_LIBRARIES(${CORE} PUBLIC ${SWIFTEST_LIBRARY} netCDF::netcdff netCDF::netcdf HDF5::HDF5)
 
 IF(USE_OPENMP OR USE_SIMD)
     TARGET_LINK_LIBRARIES(${CORE} PUBLIC SHTOOLS::parallel)
 ELSE()
     TARGET_LINK_LIBRARIES(${CORE} PUBLIC SHTOOLS::serial)
 ENDIF ()
```

### Comparing `swiftest-2024.4.1/swiftest/__init__.py` & `swiftest-2024.4.2/swiftest/__init__.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/swiftest/cli.py` & `swiftest-2024.4.2/swiftest/cli_caf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 import pty
 import subprocess
 import sys
 
 def main():
-    """Executes the 'swiftest_driver' binary located in the package root, passing along any command-line arguments, and streams the output to the terminal in real-time, handling progress bars correctly by using a pseudo-terminal."""
+    """Executes the 'swiftest' binary located in the package root, passing along any command-line arguments, and streams the output to the terminal in real-time, handling progress bars correctly by using a pseudo-terminal."""
 
     # Determine the path to the binary relative to this script
     package_root = os.path.dirname(os.path.abspath(__file__))
-    binary_path = os.path.join(package_root, 'swiftest')
+    binary_path = os.path.join(package_root, 'swiftest_caf')
 
     # sys.argv[1:] contains all the arguments passed to the script, excluding the script name itself
     args = [binary_path] + sys.argv[1:]
 
     # Use pty to spawn the process and create a pseudo-terminal
     main_fd, subordinate_fd = pty.openpty()
```

### Comparing `swiftest-2024.4.1/swiftest/constants.py` & `swiftest-2024.4.2/swiftest/constants.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/swiftest/core.h` & `swiftest-2024.4.2/swiftest/core.h`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/swiftest/core.pyx` & `swiftest-2024.4.2/swiftest/core.pyx`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/swiftest/data.py` & `swiftest-2024.4.2/swiftest/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,16 +53,16 @@
             DataArray containing the magnitude of the vector quantity 
         """
         dim = "space"
         ord = None
         
         if dim not in self.dims:
             raise ValueError(f"Dimension {dim} not found in DataArray")
-        if name is None:
-            name = self.name + "_mag"
+        if name is None and isinstance(self.name, str):
+                name = self.name + "_mag"
         da = xr.apply_ufunc(
             np.linalg.norm, self.where(~np.isnan(self)), input_core_dims=[[dim]], kwargs={"ord": ord, "axis": -1}, dask="allowed"
         )
         
         da = da.rename(name)
         return SwiftestDataArray(da)
```

### Comparing `swiftest-2024.4.1/swiftest/init_cond.py` & `swiftest-2024.4.2/swiftest/init_cond.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/swiftest/io.py` & `swiftest-2024.4.2/swiftest/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 param_keys = ['! VERSION'] + int_param + float_param + upper_str_param + lower_str_param+ bool_param
 
 # This defines SwiftestDataset variables that are strings, which must be processed due to quirks in how NetCDF-Fortran
 # handles strings differently than Python's Xarray.
 string_varnames = ["name", "particle_type", "origin_type", "stage", "regime"]
 char_varnames = ["space"]
-int_varnames = ["id", "ntp", "npl", "nplm", "discard_body_id", "collision_id", "status"]
+int_varnames = ["id", "ntp", "npl", "nplm", "discard_body_id", "collision_id", "status", "collision_body"]
 
 def _bool2yesno(boolval):
     """
     Converts a boolean into a string of either "YES" or "NO".
 
     Parameters
     ----------
```

### Comparing `swiftest-2024.4.1/swiftest/shgrav.py` & `swiftest-2024.4.2/swiftest/shgrav.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/swiftest/simulation.py` & `swiftest-2024.4.2/swiftest/simulation.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/swiftest/tool.py` & `swiftest-2024.4.2/swiftest/tool.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/swiftest/visualize.py` & `swiftest-2024.4.2/swiftest/visualize.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/tests/test_fraggle.py` & `swiftest-2024.4.2/tests/test_fraggle.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/tests/test_integration.py` & `swiftest-2024.4.2/tests/test_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         def fit_func(x,slope,b):
             """
             Linear function for curve fitting
             """
             return slope * x + b
         
         # Calculate the angular momentum error
-        sim.data['L_tot'] = sim.data['L_orbit'] + sim.data['L_spin'] + sim.data['L_escape']
+        sim.data['L_tot'] = sim.data['L_orbit'] + sim.data['L_rot'] + sim.data['L_escape']
         sim.data['DL'] = sim.data['L_tot'] - sim.data['L_tot'].isel(time=0)
         L_error = sim.data['DL'].magnitude() / sim.data['L_tot'].isel(time=0).magnitude()
 
         # Calculate the energy error
         E_error = (sim.data['TE'] - sim.data['TE'].isel(time=0)) / sim.data['TE'].isel(time=0)
 
         # Calculate the mass error
```

### Comparing `swiftest-2024.4.1/tests/test_io.py` & `swiftest-2024.4.2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/tests/test_particle_type.py` & `swiftest-2024.4.2/tests/test_particle_type.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/tests/test_units.py` & `swiftest-2024.4.2/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.1/tests/test_xv2el2xv_dims.py` & `swiftest-2024.4.2/tests/test_xv2el2xv_dims.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
  You should have received a copy of the GNU General Public License along with Swiftest. 
  If not, see: https://www.gnu.org/licenses. 
 """
 import swiftest
 import unittest
 import os
 import tempfile
-import astropy.constants as const
 import numpy as np
 
 class TestUnits(unittest.TestCase):
     def setUp(self):
         # Initialize a target and surface for testing
         self.tmpdir=tempfile.TemporaryDirectory()
         self.simdir = self.tmpdir.name
```

### Comparing `swiftest-2024.4.1/PKG-INFO` & `swiftest-2024.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: swiftest
-Version: 2024.4.1
-Keywords: astronomy astrophysics planetary n-body integrator symplectic wisdom-holman symba
+Version: 2024.4.2
+Keywords: astronomy,astrophysics,planetary,n-body,integrator,symplectic,wisdom-holman,symba
 Author: Carlisle Wishard, Jennifer Pouplin, Jake Elliott, Dana Singh, Kaustub Anand
-Author-Email: David A. Minton <daminton@purdue.edu>
-Maintainer-Email: David A. Minton <daminton@purdue.edu>
+Author-Email: "David A. Minton" <daminton@purdue.edu>
+Maintainer-Email: "David A. Minton" <daminton@purdue.edu>
 License: Copyright 2023 - David Minton 
         The Swiftest development team: David Minton, Carlisle Wishard, Jennifer Pouplin, Jake Elliott, Dana Singh, & Kaustub Anand
         
         This file is part of Swiftest.
         Swiftest is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License 
         as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
         Swiftest is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
```


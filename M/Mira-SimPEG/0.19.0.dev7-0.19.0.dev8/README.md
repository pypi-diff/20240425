# Comparing `tmp/mira_simpeg-0.19.0.dev7.tar.gz` & `tmp/mira_simpeg-0.19.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mira_simpeg-0.19.0.dev7.tar", max compression
+gzip compressed data, was "mira_simpeg-0.19.0.dev8.tar", max compression
```

## Comparing `mira_simpeg-0.19.0.dev7.tar` & `mira_simpeg-0.19.0.dev8.tar`

### file list

```diff
@@ -1,182 +1,182 @@
--rw-r--r--   0        0        0     1109 2024-01-11 21:39:39.291988 mira_simpeg-0.19.0.dev7/LICENSE
--rw-r--r--   0        0        0     2807 2024-02-06 18:26:29.916399 mira_simpeg-0.19.0.dev7/pyproject.toml
--rw-r--r--   0        0        0     6106 2024-01-11 21:39:39.291988 mira_simpeg-0.19.0.dev7/README.rst
--rw-r--r--   0        0        0     3458 2024-01-11 21:39:39.291988 mira_simpeg-0.19.0.dev7/SimPEG/__init__.py
--rw-r--r--   0        0        0      158 2023-10-05 16:26:57.174949 mira_simpeg-0.19.0.dev7/SimPEG/base/__init__.py
--rw-r--r--   0        0        0    17746 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev7/SimPEG/base/pde_simulation.py
--rw-r--r--   0        0        0      895 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev7/SimPEG/dask/__init__.py
--rw-r--r--   0        0        0     2856 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev7/SimPEG/dask/data_misfit.py
--rw-r--r--   0        0        0        0 2023-10-05 16:26:57.174949 mira_simpeg-0.19.0.dev7/SimPEG/dask/electromagnetics/__init__.py
--rw-r--r--   0        0        0        0 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev7/SimPEG/dask/electromagnetics/frequency_domain/__init__.py
--rw-r--r--   0        0        0     7742 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev7/SimPEG/dask/electromagnetics/frequency_domain/simulation.py
--rw-r--r--   0        0        0        0 2023-10-05 16:26:57.174949 mira_simpeg-0.19.0.dev7/SimPEG/dask/electromagnetics/static/__init__.py
--rw-r--r--   0        0        0        0 2023-10-05 16:26:57.174949 mira_simpeg-0.19.0.dev7/SimPEG/dask/electromagnetics/static/induced_polarization/__init__.py
--rw-r--r--   0        0        0     4104 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev7/SimPEG/dask/electromagnetics/static/induced_polarization/simulation.py
--rw-r--r--   0        0        0     1869 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev7/SimPEG/dask/electromagnetics/static/induced_polarization/simulation_2d.py
--rw-r--r--   0        0        0        0 2023-10-05 16:26:57.174949 mira_simpeg-0.19.0.dev7/SimPEG/dask/electromagnetics/static/resistivity/__init__.py
--rw-r--r--   0        0        0     5153 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev7/SimPEG/dask/electromagnetics/static/resistivity/simulation.py
--rw-r--r--   0        0        0     6529 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev7/SimPEG/dask/electromagnetics/static/resistivity/simulation_2d.py
--rw-r--r--   0        0        0        0 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev7/SimPEG/dask/electromagnetics/time_domain/__init__.py
--rw-r--r--   0        0        0    12179 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev7/SimPEG/dask/electromagnetics/time_domain/simulation.py
--rw-r--r--   0        0        0     7379 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev7/SimPEG/dask/inverse_problem.py
--rw-r--r--   0        0        0     4523 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev7/SimPEG/dask/objective_function.py
--rw-r--r--   0        0        0        0 2023-10-05 16:26:57.174949 mira_simpeg-0.19.0.dev7/SimPEG/dask/potential_fields/__init__.py
--rw-r--r--   0        0        0     3907 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev7/SimPEG/dask/potential_fields/base.py
--rw-r--r--   0        0        0        0 2023-10-05 16:26:57.174949 mira_simpeg-0.19.0.dev7/SimPEG/dask/potential_fields/gravity/__init__.py
--rw-r--r--   0        0        0      660 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev7/SimPEG/dask/potential_fields/gravity/simulation.py
--rw-r--r--   0        0        0        0 2023-10-05 16:26:57.174949 mira_simpeg-0.19.0.dev7/SimPEG/dask/potential_fields/magnetics/__init__.py
--rw-r--r--   0        0        0     1041 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev7/SimPEG/dask/potential_fields/magnetics/simulation.py
--rw-r--r--   0        0        0     6767 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev7/SimPEG/dask/simulation.py
--rw-r--r--   0        0        0     2577 2024-01-12 17:21:33.855753 mira_simpeg-0.19.0.dev7/SimPEG/dask/utils.py
--rw-r--r--   0        0        0    14075 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev7/SimPEG/data.py
--rw-r--r--   0        0        0     7307 2024-01-12 17:21:33.856459 mira_simpeg-0.19.0.dev7/SimPEG/data_misfit.py
--rw-r--r--   0        0        0      917 2024-01-12 17:21:33.856459 mira_simpeg-0.19.0.dev7/SimPEG/directives/__init__.py
--rw-r--r--   0        0        0   109022 2024-01-12 17:21:33.857750 mira_simpeg-0.19.0.dev7/SimPEG/directives/directives.py
--rw-r--r--   0        0        0    19820 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev7/SimPEG/directives/pgi_directives.py
--rw-r--r--   0        0        0    13400 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev7/SimPEG/directives/sim_directives.py
--rw-r--r--   0        0        0     1133 2024-01-12 17:21:33.858767 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/__init__.py
--rw-r--r--   0        0        0      210 2023-10-05 16:26:57.190595 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/analytics/__init__.py
--rw-r--r--   0        0        0     7105 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/analytics/DC.py
--rw-r--r--   0        0        0     8525 2024-01-12 17:21:33.858767 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/analytics/FDEM.py
--rw-r--r--   0        0        0     5084 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/analytics/FDEMcasing.py
--rw-r--r--   0        0        0    11443 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/analytics/FDEMDipolarfields.py
--rw-r--r--   0        0        0     5853 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/analytics/NSEM.py
--rw-r--r--   0        0        0     5381 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/analytics/TDEM.py
--rw-r--r--   0        0        0     6977 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/base.py
--rw-r--r--   0        0        0    23172 2024-01-12 17:21:33.859755 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/base_1d.py
--rw-r--r--   0        0        0     2011 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/frequency_domain/__init__.py
--rw-r--r--   0        0        0    60417 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/frequency_domain/fields.py
--rw-r--r--   0        0        0    13112 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/frequency_domain/receivers.py
--rw-r--r--   0        0        0    27311 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/frequency_domain/simulation.py
--rw-r--r--   0        0        0    11528 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/frequency_domain/simulation_1d.py
--rw-r--r--   0        0        0    43188 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/frequency_domain/sources.py
--rw-r--r--   0        0        0     2795 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/frequency_domain/survey.py
--rw-r--r--   0        0        0     1755 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/__init__.py
--rw-r--r--   0        0        0    26411 2024-01-11 21:39:39.324633 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/fields.py
--rw-r--r--   0        0        0    22562 2024-01-12 17:21:33.860755 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/receivers.py
--rw-r--r--   0        0        0    27228 2024-01-11 21:39:39.324633 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/simulation.py
--rw-r--r--   0        0        0    12406 2024-01-12 17:21:33.860755 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/simulation_1d.py
--rw-r--r--   0        0        0     7644 2024-01-11 21:39:39.326827 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/sources.py
--rw-r--r--   0        0        0     8922 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/survey.py
--rw-r--r--   0        0        0      793 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/utils/__init__.py
--rw-r--r--   0        0        0     5445 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/utils/analytic_1d.py
--rw-r--r--   0        0        0    18826 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/utils/data_utils.py
--rw-r--r--   0        0        0     5072 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/utils/data_viewer.py
--rw-r--r--   0        0        0     7488 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/utils/edi_files_utils.py
--rw-r--r--   0        0        0    22004 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/utils/plot_data_types.py
--rw-r--r--   0        0        0    30007 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/utils/plot_utils.py
--rw-r--r--   0        0        0     1338 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/utils/solutions_1d.py
--rw-r--r--   0        0        0     7617 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/utils/source_utils.py
--rw-r--r--   0        0        0    18430 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/utils/test_utils.py
--rw-r--r--   0        0        0      129 2023-10-05 16:26:57.206219 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/__init__.py
--rw-r--r--   0        0        0     1212 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/induced_polarization/__init__.py
--rw-r--r--   0        0        0     2144 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/induced_polarization/run.py
--rw-r--r--   0        0        0     4194 2024-01-12 17:21:33.860755 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/induced_polarization/simulation.py
--rw-r--r--   0        0        0      637 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/induced_polarization/survey.py
--rw-r--r--   0        0        0     2050 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/resistivity/__init__.py
--rw-r--r--   0        0        0     8282 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/resistivity/fields.py
--rw-r--r--   0        0        0     8412 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/resistivity/fields_2d.py
--rw-r--r--   0        0        0    41758 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/resistivity/IODC.py
--rw-r--r--   0        0        0    16671 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/resistivity/receivers.py
--rw-r--r--   0        0        0     2089 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/resistivity/run.py
--rw-r--r--   0        0        0    22651 2024-01-12 17:21:33.861755 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/resistivity/simulation.py
--rw-r--r--   0        0        0    11514 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/resistivity/simulation_1d.py
--rw-r--r--   0        0        0    27954 2024-01-12 17:21:33.863160 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/resistivity/simulation_2d.py
--rw-r--r--   0        0        0     7782 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/resistivity/sources.py
--rw-r--r--   0        0        0    12123 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/resistivity/survey.py
--rw-r--r--   0        0        0     4071 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/resistivity/utils.py
--rw-r--r--   0        0        0     1656 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/spectral_induced_polarization/__init__.py
--rw-r--r--   0        0        0     2105 2023-10-05 16:26:57.206219 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/spectral_induced_polarization/data.py
--rw-r--r--   0        0        0    14850 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/spectral_induced_polarization/receivers.py
--rw-r--r--   0        0        0     5028 2023-10-05 16:26:57.206219 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/spectral_induced_polarization/run.py
--rw-r--r--   0        0        0    21261 2024-01-11 21:39:39.343188 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/spectral_induced_polarization/simulation.py
--rw-r--r--   0        0        0     2962 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/spectral_induced_polarization/simulation_2d.py
--rw-r--r--   0        0        0     8465 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/spectral_induced_polarization/sources.py
--rw-r--r--   0        0        0     4149 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/spectral_induced_polarization/survey.py
--rw-r--r--   0        0        0     1124 2024-01-12 17:21:33.863160 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/spontaneous_potential/__init__.py
--rw-r--r--   0        0        0     6658 2024-01-12 17:21:33.864168 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/spontaneous_potential/simulation.py
--rw-r--r--   0        0        0     1011 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/spontaneous_potential/sources.py
--rw-r--r--   0        0        0     1950 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/utils/__init__.py
--rw-r--r--   0        0        0    66992 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/utils/static_utils.py
--rw-r--r--   0        0        0     2290 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/time_domain/__init__.py
--rw-r--r--   0        0        0    24091 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/time_domain/fields.py
--rw-r--r--   0        0        0    12251 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/time_domain/receivers.py
--rw-r--r--   0        0        0    39494 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/time_domain/simulation.py
--rw-r--r--   0        0        0    14465 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/time_domain/simulation_1d.py
--rw-r--r--   0        0        0    71847 2024-01-12 17:21:33.865252 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/time_domain/sources.py
--rw-r--r--   0        0        0     1070 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/time_domain/survey.py
--rw-r--r--   0        0        0      947 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/utils/__init__.py
--rw-r--r--   0        0        0    16473 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/utils/current_utils.py
--rw-r--r--   0        0        0     6593 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/utils/em1d_utils.py
--rw-r--r--   0        0        0     5831 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/utils/testing_utils.py
--rw-r--r--   0        0        0     3578 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/utils/waveform_utils.py
--rw-r--r--   0        0        0     1528 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/viscous_remanent_magnetization/__init__.py
--rw-r--r--   0        0        0     6800 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/viscous_remanent_magnetization/receivers.py
--rw-r--r--   0        0        0    39890 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/viscous_remanent_magnetization/simulation.py
--rw-r--r--   0        0        0    18560 2024-01-12 17:21:33.865252 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/viscous_remanent_magnetization/sources.py
--rw-r--r--   0        0        0     2338 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/viscous_remanent_magnetization/survey.py
--rw-r--r--   0        0        0    20152 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/viscous_remanent_magnetization/waveforms.py
--rw-r--r--   0        0        0    13959 2024-01-12 17:21:33.866228 mira_simpeg-0.19.0.dev7/SimPEG/fields.py
--rw-r--r--   0        0        0       24 2023-10-05 16:26:57.230943 mira_simpeg-0.19.0.dev7/SimPEG/flow/__init__.py
--rw-r--r--   0        0        0     1136 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev7/SimPEG/flow/richards/__init__.py
--rw-r--r--   0        0        0    33981 2024-01-11 21:39:39.360202 mira_simpeg-0.19.0.dev7/SimPEG/flow/richards/empirical.py
--rw-r--r--   0        0        0     3618 2024-01-11 21:39:39.360202 mira_simpeg-0.19.0.dev7/SimPEG/flow/richards/receivers.py
--rw-r--r--   0        0        0    13567 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev7/SimPEG/flow/richards/simulation.py
--rw-r--r--   0        0        0     2798 2024-01-12 17:21:33.866228 mira_simpeg-0.19.0.dev7/SimPEG/flow/richards/survey.py
--rw-r--r--   0        0        0    10625 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev7/SimPEG/inverse_problem.py
--rw-r--r--   0        0        0     3329 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev7/SimPEG/inversion.py
--rw-r--r--   0        0        0   213269 2024-01-12 17:21:33.867169 mira_simpeg-0.19.0.dev7/SimPEG/maps.py
--rw-r--r--   0        0        0     1527 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev7/SimPEG/meta/__init__.py
--rw-r--r--   0        0        0    16903 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev7/SimPEG/meta/simulation.py
--rw-r--r--   0        0        0     1218 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev7/SimPEG/models.py
--rw-r--r--   0        0        0    14724 2024-01-12 17:21:33.868175 mira_simpeg-0.19.0.dev7/SimPEG/objective_function.py
--rw-r--r--   0        0        0    39604 2024-01-12 17:21:33.869168 mira_simpeg-0.19.0.dev7/SimPEG/optimization.py
--rw-r--r--   0        0        0      589 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/__init__.py
--rw-r--r--   0        0        0    13464 2024-01-12 17:21:33.870181 mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/base.py
--rw-r--r--   0        0        0     1100 2024-01-12 17:21:33.870181 mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/gravity/__init__.py
--rw-r--r--   0        0        0     2272 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/gravity/analytics.py
--rw-r--r--   0        0        0     2271 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/gravity/receivers.py
--rw-r--r--   0        0        0     9057 2024-01-12 17:21:33.871168 mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/gravity/simulation.py
--rw-r--r--   0        0        0      407 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/gravity/sources.py
--rw-r--r--   0        0        0     4774 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/gravity/survey.py
--rw-r--r--   0        0        0     1174 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/magnetics/__init__.py
--rw-r--r--   0        0        0     9821 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/magnetics/analytics.py
--rw-r--r--   0        0        0     2228 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/magnetics/receivers.py
--rw-r--r--   0        0        0    31502 2024-01-12 17:21:33.871168 mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/magnetics/simulation.py
--rw-r--r--   0        0        0     3669 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/magnetics/sources.py
--rw-r--r--   0        0        0     2693 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/magnetics/survey.py
--rw-r--r--   0        0        0    15572 2024-01-12 17:21:33.872185 mira_simpeg-0.19.0.dev7/SimPEG/props.py
--rw-r--r--   0        0        0     8134 2024-01-12 17:21:33.872578 mira_simpeg-0.19.0.dev7/SimPEG/regularization/__init__.py
--rw-r--r--   0        0        0    43137 2024-02-06 18:21:38.636361 mira_simpeg-0.19.0.dev7/SimPEG/regularization/base.py
--rw-r--r--   0        0        0     3908 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev7/SimPEG/regularization/correspondence.py
--rw-r--r--   0        0        0     9843 2024-01-12 17:21:33.872578 mira_simpeg-0.19.0.dev7/SimPEG/regularization/cross_gradient.py
--rw-r--r--   0        0        0     5244 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev7/SimPEG/regularization/jtv.py
--rw-r--r--   0        0        0    32347 2024-01-12 17:21:33.872578 mira_simpeg-0.19.0.dev7/SimPEG/regularization/pgi.py
--rw-r--r--   0        0        0    16758 2024-02-06 18:21:38.637365 mira_simpeg-0.19.0.dev7/SimPEG/regularization/regularization_mesh.py
--rw-r--r--   0        0        0    10363 2024-02-06 18:21:38.638358 mira_simpeg-0.19.0.dev7/SimPEG/regularization/sparse.py
--rw-r--r--   0        0        0       39 2023-10-05 16:26:57.247510 mira_simpeg-0.19.0.dev7/SimPEG/seismic/__init__.py
--rw-r--r--   0        0        0      760 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev7/SimPEG/seismic/straight_ray_tomography/__init__.py
--rw-r--r--   0        0        0     3578 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev7/SimPEG/seismic/straight_ray_tomography/simulation.py
--rw-r--r--   0        0        0     1688 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev7/SimPEG/seismic/straight_ray_tomography/survey.py
--rw-r--r--   0        0        0    19552 2024-01-12 17:21:33.872578 mira_simpeg-0.19.0.dev7/SimPEG/simulation.py
--rw-r--r--   0        0        0    17616 2024-01-12 17:21:33.872578 mira_simpeg-0.19.0.dev7/SimPEG/survey.py
--rw-r--r--   0        0        0     6705 2024-01-12 17:21:33.872578 mira_simpeg-0.19.0.dev7/SimPEG/utils/__init__.py
--rw-r--r--   0        0        0    39084 2024-01-12 17:21:33.877582 mira_simpeg-0.19.0.dev7/SimPEG/utils/code_utils.py
--rw-r--r--   0        0        0      531 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev7/SimPEG/utils/coord_utils.py
--rw-r--r--   0        0        0     4104 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev7/SimPEG/utils/counter_utils.py
--rw-r--r--   0        0        0      687 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev7/SimPEG/utils/curv_utils.py
--rw-r--r--   0        0        0       98 2023-10-05 16:26:57.263144 mira_simpeg-0.19.0.dev7/SimPEG/utils/drivers/__init__.py
--rw-r--r--   0        0        0     8117 2024-01-12 17:21:33.877582 mira_simpeg-0.19.0.dev7/SimPEG/utils/drivers/gravity_driver.py
--rw-r--r--   0        0        0     9736 2024-01-12 17:21:33.877582 mira_simpeg-0.19.0.dev7/SimPEG/utils/drivers/magnetics_driver.py
--rw-r--r--   0        0        0      631 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev7/SimPEG/utils/io_utils/__init__.py
--rw-r--r--   0        0        0    36848 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev7/SimPEG/utils/io_utils/io_utils_electromagnetics.py
--rw-r--r--   0        0        0     4825 2024-01-12 17:21:33.877582 mira_simpeg-0.19.0.dev7/SimPEG/utils/io_utils/io_utils_general.py
--rw-r--r--   0        0        0    13183 2024-01-12 17:21:33.877582 mira_simpeg-0.19.0.dev7/SimPEG/utils/io_utils/io_utils_pf.py
--rw-r--r--   0        0        0    14546 2024-02-06 18:21:38.638358 mira_simpeg-0.19.0.dev7/SimPEG/utils/mat_utils.py
--rw-r--r--   0        0        0     3480 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev7/SimPEG/utils/mesh_utils.py
--rw-r--r--   0        0        0    16902 2024-01-12 17:21:33.877582 mira_simpeg-0.19.0.dev7/SimPEG/utils/model_builder.py
--rw-r--r--   0        0        0     7038 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev7/SimPEG/utils/model_utils.py
--rw-r--r--   0        0        0    67694 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev7/SimPEG/utils/pgi_utils.py
--rw-r--r--   0        0        0    12916 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev7/SimPEG/utils/plot_utils.py
--rw-r--r--   0        0        0    10049 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev7/SimPEG/utils/solver_utils.py
--rw-r--r--   0        0        0     8080 1970-01-01 00:00:00.000000 mira_simpeg-0.19.0.dev7/PKG-INFO
+-rw-r--r--   0        0        0     1109 2024-01-11 21:39:39.291988 mira_simpeg-0.19.0.dev8/LICENSE
+-rw-r--r--   0        0        0     2807 2024-04-25 18:57:44.664220 mira_simpeg-0.19.0.dev8/pyproject.toml
+-rw-r--r--   0        0        0     6106 2024-01-11 21:39:39.291988 mira_simpeg-0.19.0.dev8/README.rst
+-rw-r--r--   0        0        0     3458 2024-01-11 21:39:39.291988 mira_simpeg-0.19.0.dev8/SimPEG/__init__.py
+-rw-r--r--   0        0        0      158 2023-10-05 16:26:57.174949 mira_simpeg-0.19.0.dev8/SimPEG/base/__init__.py
+-rw-r--r--   0        0        0    17746 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/base/pde_simulation.py
+-rw-r--r--   0        0        0      895 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/__init__.py
+-rw-r--r--   0        0        0     2856 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/data_misfit.py
+-rw-r--r--   0        0        0        0 2023-10-05 16:26:57.174949 mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/frequency_domain/__init__.py
+-rw-r--r--   0        0        0     7742 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/frequency_domain/simulation.py
+-rw-r--r--   0        0        0        0 2023-10-05 16:26:57.174949 mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/static/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-05 16:26:57.174949 mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/static/induced_polarization/__init__.py
+-rw-r--r--   0        0        0     4104 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/static/induced_polarization/simulation.py
+-rw-r--r--   0        0        0     1869 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/static/induced_polarization/simulation_2d.py
+-rw-r--r--   0        0        0        0 2023-10-05 16:26:57.174949 mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/static/resistivity/__init__.py
+-rw-r--r--   0        0        0     5153 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/static/resistivity/simulation.py
+-rw-r--r--   0        0        0     6529 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/static/resistivity/simulation_2d.py
+-rw-r--r--   0        0        0        0 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/time_domain/__init__.py
+-rw-r--r--   0        0        0    18322 2024-04-25 18:57:44.664220 mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/time_domain/simulation.py
+-rw-r--r--   0        0        0     7379 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/inverse_problem.py
+-rw-r--r--   0        0        0     4523 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/objective_function.py
+-rw-r--r--   0        0        0        0 2023-10-05 16:26:57.174949 mira_simpeg-0.19.0.dev8/SimPEG/dask/potential_fields/__init__.py
+-rw-r--r--   0        0        0     3907 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/potential_fields/base.py
+-rw-r--r--   0        0        0        0 2023-10-05 16:26:57.174949 mira_simpeg-0.19.0.dev8/SimPEG/dask/potential_fields/gravity/__init__.py
+-rw-r--r--   0        0        0      660 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/potential_fields/gravity/simulation.py
+-rw-r--r--   0        0        0        0 2023-10-05 16:26:57.174949 mira_simpeg-0.19.0.dev8/SimPEG/dask/potential_fields/magnetics/__init__.py
+-rw-r--r--   0        0        0     1041 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/potential_fields/magnetics/simulation.py
+-rw-r--r--   0        0        0     6763 2024-04-12 20:56:06.259702 mira_simpeg-0.19.0.dev8/SimPEG/dask/simulation.py
+-rw-r--r--   0        0        0     3132 2024-04-25 18:57:44.664220 mira_simpeg-0.19.0.dev8/SimPEG/dask/utils.py
+-rw-r--r--   0        0        0    14075 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/data.py
+-rw-r--r--   0        0        0     7307 2024-01-12 17:21:33.856459 mira_simpeg-0.19.0.dev8/SimPEG/data_misfit.py
+-rw-r--r--   0        0        0      917 2024-01-12 17:21:33.856459 mira_simpeg-0.19.0.dev8/SimPEG/directives/__init__.py
+-rw-r--r--   0        0        0   109257 2024-04-25 16:00:58.227398 mira_simpeg-0.19.0.dev8/SimPEG/directives/directives.py
+-rw-r--r--   0        0        0    19820 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/directives/pgi_directives.py
+-rw-r--r--   0        0        0    13400 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/directives/sim_directives.py
+-rw-r--r--   0        0        0     1133 2024-01-12 17:21:33.858767 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/__init__.py
+-rw-r--r--   0        0        0      210 2023-10-05 16:26:57.190595 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/__init__.py
+-rw-r--r--   0        0        0     7105 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/DC.py
+-rw-r--r--   0        0        0     8525 2024-01-12 17:21:33.858767 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/FDEM.py
+-rw-r--r--   0        0        0     5084 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/FDEMcasing.py
+-rw-r--r--   0        0        0    11443 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/FDEMDipolarfields.py
+-rw-r--r--   0        0        0     5853 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/NSEM.py
+-rw-r--r--   0        0        0     5381 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/TDEM.py
+-rw-r--r--   0        0        0     6977 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/base.py
+-rw-r--r--   0        0        0    23172 2024-01-12 17:21:33.859755 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/base_1d.py
+-rw-r--r--   0        0        0     2011 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/__init__.py
+-rw-r--r--   0        0        0    60417 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/fields.py
+-rw-r--r--   0        0        0    13112 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/receivers.py
+-rw-r--r--   0        0        0    27311 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/simulation.py
+-rw-r--r--   0        0        0    11528 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/simulation_1d.py
+-rw-r--r--   0        0        0    43188 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/sources.py
+-rw-r--r--   0        0        0     2795 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/survey.py
+-rw-r--r--   0        0        0     1755 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/__init__.py
+-rw-r--r--   0        0        0    26411 2024-01-11 21:39:39.324633 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/fields.py
+-rw-r--r--   0        0        0    22562 2024-01-12 17:21:33.860755 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/receivers.py
+-rw-r--r--   0        0        0    27228 2024-01-11 21:39:39.324633 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/simulation.py
+-rw-r--r--   0        0        0    12406 2024-01-12 17:21:33.860755 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/simulation_1d.py
+-rw-r--r--   0        0        0     7644 2024-01-11 21:39:39.326827 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/sources.py
+-rw-r--r--   0        0        0     8922 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/survey.py
+-rw-r--r--   0        0        0      793 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/__init__.py
+-rw-r--r--   0        0        0     5445 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/analytic_1d.py
+-rw-r--r--   0        0        0    18826 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/data_utils.py
+-rw-r--r--   0        0        0     5072 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/data_viewer.py
+-rw-r--r--   0        0        0     7488 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/edi_files_utils.py
+-rw-r--r--   0        0        0    22004 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/plot_data_types.py
+-rw-r--r--   0        0        0    30007 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/plot_utils.py
+-rw-r--r--   0        0        0     1338 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/solutions_1d.py
+-rw-r--r--   0        0        0     7617 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/source_utils.py
+-rw-r--r--   0        0        0    18430 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/test_utils.py
+-rw-r--r--   0        0        0      129 2023-10-05 16:26:57.206219 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/__init__.py
+-rw-r--r--   0        0        0     1212 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/induced_polarization/__init__.py
+-rw-r--r--   0        0        0     2144 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/induced_polarization/run.py
+-rw-r--r--   0        0        0     4194 2024-01-12 17:21:33.860755 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/induced_polarization/simulation.py
+-rw-r--r--   0        0        0      637 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/induced_polarization/survey.py
+-rw-r--r--   0        0        0     2050 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/__init__.py
+-rw-r--r--   0        0        0     8282 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/fields.py
+-rw-r--r--   0        0        0     8412 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/fields_2d.py
+-rw-r--r--   0        0        0    41758 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/IODC.py
+-rw-r--r--   0        0        0    16671 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/receivers.py
+-rw-r--r--   0        0        0     2089 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/run.py
+-rw-r--r--   0        0        0    22651 2024-01-12 17:21:33.861755 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/simulation.py
+-rw-r--r--   0        0        0    11514 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/simulation_1d.py
+-rw-r--r--   0        0        0    27954 2024-01-12 17:21:33.863160 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/simulation_2d.py
+-rw-r--r--   0        0        0     7782 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/sources.py
+-rw-r--r--   0        0        0    12123 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/survey.py
+-rw-r--r--   0        0        0     4071 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/utils.py
+-rw-r--r--   0        0        0     1656 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/__init__.py
+-rw-r--r--   0        0        0     2105 2023-10-05 16:26:57.206219 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/data.py
+-rw-r--r--   0        0        0    14850 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/receivers.py
+-rw-r--r--   0        0        0     5028 2023-10-05 16:26:57.206219 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/run.py
+-rw-r--r--   0        0        0    21261 2024-01-11 21:39:39.343188 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/simulation.py
+-rw-r--r--   0        0        0     2962 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/simulation_2d.py
+-rw-r--r--   0        0        0     8465 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/sources.py
+-rw-r--r--   0        0        0     4149 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/survey.py
+-rw-r--r--   0        0        0     1124 2024-01-12 17:21:33.863160 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spontaneous_potential/__init__.py
+-rw-r--r--   0        0        0     6658 2024-01-12 17:21:33.864168 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spontaneous_potential/simulation.py
+-rw-r--r--   0        0        0     1011 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spontaneous_potential/sources.py
+-rw-r--r--   0        0        0     1950 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/utils/__init__.py
+-rw-r--r--   0        0        0    66992 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/utils/static_utils.py
+-rw-r--r--   0        0        0     2290 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/__init__.py
+-rw-r--r--   0        0        0    24117 2024-04-12 20:56:06.263737 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/fields.py
+-rw-r--r--   0        0        0    12502 2024-04-12 20:56:06.263737 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/receivers.py
+-rw-r--r--   0        0        0    39494 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/simulation.py
+-rw-r--r--   0        0        0    14465 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/simulation_1d.py
+-rw-r--r--   0        0        0    71847 2024-01-12 17:21:33.865252 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/sources.py
+-rw-r--r--   0        0        0     1070 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/survey.py
+-rw-r--r--   0        0        0      947 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/utils/__init__.py
+-rw-r--r--   0        0        0    16473 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/utils/current_utils.py
+-rw-r--r--   0        0        0     6593 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/utils/em1d_utils.py
+-rw-r--r--   0        0        0     5831 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/utils/testing_utils.py
+-rw-r--r--   0        0        0     3578 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/utils/waveform_utils.py
+-rw-r--r--   0        0        0     1528 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/viscous_remanent_magnetization/__init__.py
+-rw-r--r--   0        0        0     6800 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/viscous_remanent_magnetization/receivers.py
+-rw-r--r--   0        0        0    39890 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/viscous_remanent_magnetization/simulation.py
+-rw-r--r--   0        0        0    18560 2024-01-12 17:21:33.865252 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/viscous_remanent_magnetization/sources.py
+-rw-r--r--   0        0        0     2338 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/viscous_remanent_magnetization/survey.py
+-rw-r--r--   0        0        0    20152 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/viscous_remanent_magnetization/waveforms.py
+-rw-r--r--   0        0        0    13959 2024-01-12 17:21:33.866228 mira_simpeg-0.19.0.dev8/SimPEG/fields.py
+-rw-r--r--   0        0        0       24 2023-10-05 16:26:57.230943 mira_simpeg-0.19.0.dev8/SimPEG/flow/__init__.py
+-rw-r--r--   0        0        0     1136 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/flow/richards/__init__.py
+-rw-r--r--   0        0        0    33981 2024-01-11 21:39:39.360202 mira_simpeg-0.19.0.dev8/SimPEG/flow/richards/empirical.py
+-rw-r--r--   0        0        0     3618 2024-01-11 21:39:39.360202 mira_simpeg-0.19.0.dev8/SimPEG/flow/richards/receivers.py
+-rw-r--r--   0        0        0    13567 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/flow/richards/simulation.py
+-rw-r--r--   0        0        0     2798 2024-01-12 17:21:33.866228 mira_simpeg-0.19.0.dev8/SimPEG/flow/richards/survey.py
+-rw-r--r--   0        0        0    10625 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/inverse_problem.py
+-rw-r--r--   0        0        0     3329 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/inversion.py
+-rw-r--r--   0        0        0   213269 2024-01-12 17:21:33.867169 mira_simpeg-0.19.0.dev8/SimPEG/maps.py
+-rw-r--r--   0        0        0     1527 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/meta/__init__.py
+-rw-r--r--   0        0        0    16903 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/meta/simulation.py
+-rw-r--r--   0        0        0     1218 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/models.py
+-rw-r--r--   0        0        0    14724 2024-01-12 17:21:33.868175 mira_simpeg-0.19.0.dev8/SimPEG/objective_function.py
+-rw-r--r--   0        0        0    39604 2024-01-12 17:21:33.869168 mira_simpeg-0.19.0.dev8/SimPEG/optimization.py
+-rw-r--r--   0        0        0      589 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/__init__.py
+-rw-r--r--   0        0        0    13464 2024-01-12 17:21:33.870181 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/base.py
+-rw-r--r--   0        0        0     1100 2024-01-12 17:21:33.870181 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/gravity/__init__.py
+-rw-r--r--   0        0        0     2272 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/gravity/analytics.py
+-rw-r--r--   0        0        0     2271 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/gravity/receivers.py
+-rw-r--r--   0        0        0     9057 2024-01-12 17:21:33.871168 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/gravity/simulation.py
+-rw-r--r--   0        0        0      407 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/gravity/sources.py
+-rw-r--r--   0        0        0     4774 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/gravity/survey.py
+-rw-r--r--   0        0        0     1174 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/magnetics/__init__.py
+-rw-r--r--   0        0        0     9821 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/magnetics/analytics.py
+-rw-r--r--   0        0        0     2228 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/magnetics/receivers.py
+-rw-r--r--   0        0        0    31502 2024-01-12 17:21:33.871168 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/magnetics/simulation.py
+-rw-r--r--   0        0        0     3669 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/magnetics/sources.py
+-rw-r--r--   0        0        0     2693 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/magnetics/survey.py
+-rw-r--r--   0        0        0    15572 2024-01-12 17:21:33.872185 mira_simpeg-0.19.0.dev8/SimPEG/props.py
+-rw-r--r--   0        0        0     8134 2024-01-12 17:21:33.872578 mira_simpeg-0.19.0.dev8/SimPEG/regularization/__init__.py
+-rw-r--r--   0        0        0    43137 2024-02-06 18:21:38.636361 mira_simpeg-0.19.0.dev8/SimPEG/regularization/base.py
+-rw-r--r--   0        0        0     3908 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/regularization/correspondence.py
+-rw-r--r--   0        0        0     9843 2024-01-12 17:21:33.872578 mira_simpeg-0.19.0.dev8/SimPEG/regularization/cross_gradient.py
+-rw-r--r--   0        0        0     5244 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/regularization/jtv.py
+-rw-r--r--   0        0        0    32347 2024-01-12 17:21:33.872578 mira_simpeg-0.19.0.dev8/SimPEG/regularization/pgi.py
+-rw-r--r--   0        0        0    16758 2024-02-06 18:21:38.637365 mira_simpeg-0.19.0.dev8/SimPEG/regularization/regularization_mesh.py
+-rw-r--r--   0        0        0    10363 2024-02-06 18:21:38.638358 mira_simpeg-0.19.0.dev8/SimPEG/regularization/sparse.py
+-rw-r--r--   0        0        0       39 2023-10-05 16:26:57.247510 mira_simpeg-0.19.0.dev8/SimPEG/seismic/__init__.py
+-rw-r--r--   0        0        0      760 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/seismic/straight_ray_tomography/__init__.py
+-rw-r--r--   0        0        0     3578 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/seismic/straight_ray_tomography/simulation.py
+-rw-r--r--   0        0        0     1688 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/seismic/straight_ray_tomography/survey.py
+-rw-r--r--   0        0        0    19552 2024-01-12 17:21:33.872578 mira_simpeg-0.19.0.dev8/SimPEG/simulation.py
+-rw-r--r--   0        0        0    17616 2024-01-12 17:21:33.872578 mira_simpeg-0.19.0.dev8/SimPEG/survey.py
+-rw-r--r--   0        0        0     6705 2024-01-12 17:21:33.872578 mira_simpeg-0.19.0.dev8/SimPEG/utils/__init__.py
+-rw-r--r--   0        0        0    39084 2024-01-12 17:21:33.877582 mira_simpeg-0.19.0.dev8/SimPEG/utils/code_utils.py
+-rw-r--r--   0        0        0      531 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/utils/coord_utils.py
+-rw-r--r--   0        0        0     4104 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/utils/counter_utils.py
+-rw-r--r--   0        0        0      687 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/utils/curv_utils.py
+-rw-r--r--   0        0        0       98 2023-10-05 16:26:57.263144 mira_simpeg-0.19.0.dev8/SimPEG/utils/drivers/__init__.py
+-rw-r--r--   0        0        0     8117 2024-01-12 17:21:33.877582 mira_simpeg-0.19.0.dev8/SimPEG/utils/drivers/gravity_driver.py
+-rw-r--r--   0        0        0     9736 2024-01-12 17:21:33.877582 mira_simpeg-0.19.0.dev8/SimPEG/utils/drivers/magnetics_driver.py
+-rw-r--r--   0        0        0      631 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/utils/io_utils/__init__.py
+-rw-r--r--   0        0        0    36848 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/utils/io_utils/io_utils_electromagnetics.py
+-rw-r--r--   0        0        0     4825 2024-01-12 17:21:33.877582 mira_simpeg-0.19.0.dev8/SimPEG/utils/io_utils/io_utils_general.py
+-rw-r--r--   0        0        0    13183 2024-01-12 17:21:33.877582 mira_simpeg-0.19.0.dev8/SimPEG/utils/io_utils/io_utils_pf.py
+-rw-r--r--   0        0        0    14546 2024-02-06 18:21:38.638358 mira_simpeg-0.19.0.dev8/SimPEG/utils/mat_utils.py
+-rw-r--r--   0        0        0     3480 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/utils/mesh_utils.py
+-rw-r--r--   0        0        0    16902 2024-01-12 17:21:33.877582 mira_simpeg-0.19.0.dev8/SimPEG/utils/model_builder.py
+-rw-r--r--   0        0        0     7038 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/utils/model_utils.py
+-rw-r--r--   0        0        0    67694 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/utils/pgi_utils.py
+-rw-r--r--   0        0        0    12916 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/utils/plot_utils.py
+-rw-r--r--   0        0        0    10049 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/utils/solver_utils.py
+-rw-r--r--   0        0        0     8080 1970-01-01 00:00:00.000000 mira_simpeg-0.19.0.dev8/PKG-INFO
```

### Comparing `mira_simpeg-0.19.0.dev7/LICENSE` & `mira_simpeg-0.19.0.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/pyproject.toml` & `mira_simpeg-0.19.0.dev8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #SimPEG: Simulation and Parameter Estimation in Geophysics
 #
 #SimPEG is a python package for simulation and gradient based
 #parameter estimation in the context of geophysical applications.
 
 [tool.poetry]
 name = "Mira-SimPEG"
-version = "0.19.0.dev7"
+version = "0.19.0.dev8"
 license = "MIT"
 description = "Mira Geoscience fork of SimPEG: Simulation and Parameter Estimation in Geophysics"
 
 authors = ["Rowan Cockett <rowanc1@gmail.com>", "dominiquef@mirageoscience.com"]
 repository = "http://github.com/simpeg/simpeg"
 documentation = "https://docs.simpeg.xyz/"
 homepage = "http://simpeg.xyz/"
```

### Comparing `mira_simpeg-0.19.0.dev7/README.rst` & `mira_simpeg-0.19.0.dev8/README.rst`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/__init__.py` & `mira_simpeg-0.19.0.dev8/SimPEG/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/base/pde_simulation.py` & `mira_simpeg-0.19.0.dev8/SimPEG/base/pde_simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/dask/__init__.py` & `mira_simpeg-0.19.0.dev8/SimPEG/dask/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/dask/data_misfit.py` & `mira_simpeg-0.19.0.dev8/SimPEG/dask/data_misfit.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/dask/electromagnetics/frequency_domain/simulation.py` & `mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/frequency_domain/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/dask/electromagnetics/static/induced_polarization/simulation.py` & `mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/static/induced_polarization/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/dask/electromagnetics/static/induced_polarization/simulation_2d.py` & `mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/static/induced_polarization/simulation_2d.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/dask/electromagnetics/static/resistivity/simulation.py` & `mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/static/resistivity/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/dask/electromagnetics/static/resistivity/simulation_2d.py` & `mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/static/resistivity/simulation_2d.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/dask/electromagnetics/time_domain/simulation.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/simulation_1d.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,417 +1,371 @@
-import dask
-import dask.array
-
-from ....electromagnetics.time_domain.simulation import BaseTDEMSimulation as Sim
-from ....utils import Zero
-from multiprocessing import cpu_count
+from ..base_1d import BaseEM1DSimulation
+from .sources import StepOffWaveform
+from .receivers import (
+    PointMagneticFluxDensity,
+    PointMagneticField,
+    PointMagneticFluxTimeDerivative,
+)
 import numpy as np
-import scipy.sparse as sp
-from dask import array, delayed
-from SimPEG.dask.simulation import dask_Jvec, dask_Jtvec, dask_getJtJdiag
-from SimPEG.dask.utils import get_parallel_blocks
-import zarr
-from time import time
-from tqdm import tqdm
-
-Sim.sensitivity_path = "./sensitivity/"
-Sim.store_sensitivities = "ram"
-
-Sim.getJtJdiag = dask_getJtJdiag
-Sim.Jvec = dask_Jvec
-Sim.Jtvec = dask_Jtvec
-Sim.clean_on_model_update = ["_Jmatrix", "_jtjdiag"]
-
-
-def fields(self, m=None, return_Ainv=False):
-    if m is not None:
-        self.model = m
-
-    f = self.fieldsPair(self)
-    f[:, self._fieldType + "Solution", 0] = self.getInitialFields()
-    Ainv = {}
-    ATinv = {}
-
-    for tInd, dt in enumerate(self.time_steps):
-        if dt not in Ainv:
-            A = self.getAdiag(tInd)
-            Ainv[dt] = self.solver(sp.csr_matrix(A), **self.solver_opts)
-            if return_Ainv:
-                ATinv[dt] = self.solver(sp.csr_matrix(A.T), **self.solver_opts)
-
-        Asubdiag = self.getAsubdiag(tInd)
-        rhs = -Asubdiag * f[:, (self._fieldType + "Solution"), tInd]
-
-        if (
-            np.abs(self.survey.source_list[0].waveform.eval(self.times[tInd + 1]))
-            > 1e-8
-        ):
-            rhs += self.getRHS(tInd + 1)
-
-        sol = Ainv[dt] * rhs
-        f[:, self._fieldType + "Solution", tInd + 1] = sol
-
-    for A in Ainv.values():
-        A.clean()
-
-    if return_Ainv:
-        return f, ATinv
-    else:
-        return f, None
-
-
-Sim.fields = fields
-
-
-def dask_getSourceTerm(self, tInd):
-    """
-    Assemble the source term. This ensures that the RHS is a vector / array
-    of the correct size
-    """
-    source_list = self.survey.source_list
-    source_block = np.array_split(source_list, cpu_count())
-
-    def source_evaluation(simulation, sources, time):
-        s_m, s_e = [], []
-        for source in sources:
-            sm, se = source.eval(simulation, time)
-            s_m.append(sm)
-            s_e.append(se)
-
-        return s_m, s_e
-
-    block_compute = []
-    for block in source_block:
-        block_compute.append(
-            delayed(source_evaluation, pure=True)(self, block, self.times[tInd])
-        )
-
-    eval = dask.compute(block_compute)[0]
-
-    s_m, s_e = [], []
-    for block in eval:
-        if block[0]:
-            s_m.append(block[0])
-            s_e.append(block[1])
-
-    if isinstance(s_m[0][0], Zero):
-        return Zero(), np.vstack(s_e).T
-
-    return np.vstack(s_m).T, np.vstack(s_e).T
-
-
-Sim.getSourceTerm = dask_getSourceTerm
-
-
-def dask_dpred(self, m=None, f=None, compute_J=False):
-    """
-    dpred(m, f=None)
-    Create the projected data from a model.
-    The fields, f, (if provided) will be used for the predicted data
-    instead of recalculating the fields (which may be expensive!).
-
-    .. math::
-
-        d_\\text{pred} = P(f(m))
-
-    Where P is a projection of the fields onto the data space.
-    """
-    if self.survey is None:
-        raise AttributeError(
-            "The survey has not yet been set and is required to compute "
-            "data. Please set the survey for the simulation: "
-            "simulation.survey = survey"
-        )
-    # ct = time()
-    if f is None:
-        if m is None:
-            m = self.model
-        f, Ainv = self.fields(m, return_Ainv=compute_J)
-
-    # print(f"took {time() - ct} s to compute fields")
-    def evaluate_receiver(source, receiver, mesh, time_mesh, fields):
-        return receiver.eval(source, mesh, time_mesh, fields).flatten()
-
-    row = delayed(evaluate_receiver, pure=True)
-    rows = []
-    for src in self.survey.source_list:
-        for rx in src.receiver_list:
-            rows.append(
-                array.from_delayed(
-                    row(src, rx, self.mesh, self.time_mesh, f),
-                    dtype=np.float32,
-                    shape=(rx.nD,),
-                )
-            )
-
-    data = array.hstack(rows).compute()
-
-    if compute_J and self._Jmatrix is None:
-        Jmatrix = self.compute_J(f=f, Ainv=Ainv)
-        return data, Jmatrix
-
-    return data
-
-
-Sim.dpred = dask_dpred
-Sim.field_derivs = None
-
 
-@delayed
-def block_deriv(time_index, field_type, source_list, mesh, time_mesh, fields, Jmatrix):
-    """Compute derivatives for sources and receivers in a block"""
-    field_len = len(fields[source_list[0], field_type, 0])
-    df_duT = []
-    rx_count = 0
-    for source in source_list:
-        sources_block = []
-
-        for rx in source.receiver_list:
-            PTv = rx.getP(mesh, time_mesh, fields).tocsr()
-            derivative_fun = getattr(fields, "_{}Deriv".format(rx.projField), None)
-            rx_ind = np.arange(rx_count, rx_count + rx.nD).astype(int)
-            cur = derivative_fun(
-                time_index,
-                source,
-                None,
-                PTv[:, (time_index * field_len) : ((time_index + 1) * field_len)].T,
-                adjoint=True,
-            )
-            sources_block.append(cur[0])
-
-            if not isinstance(cur[1], Zero):
-                Jmatrix[rx_ind, :] += cur[1].T
-
-            rx_count += rx.nD
-
-        df_duT.append(sources_block)
-
-    return df_duT
-
-
-def compute_field_derivs(simulation, Jmatrix, fields):
-    """
-    Compute the derivative of the fields
-    """
-    df_duT = []
-
-    for time_index in range(simulation.nT + 1):
-        df_duT.append(
-            block_deriv(
-                time_index,
-                simulation._fieldType + "Solution",
-                simulation.survey.source_list,
-                simulation.mesh,
-                simulation.time_mesh,
-                fields,
-                Jmatrix,
-            )
-        )
-
-    df_duT = dask.compute(df_duT)[0]
-
-    return df_duT
-
-
-@delayed
-def deriv_block(
-    s_id, r_id, b_id, ATinv_df_duT_v, Asubdiag, local_ind, sub_ind, simulation, tInd
-):
-    if (s_id, r_id, b_id) not in ATinv_df_duT_v:
-        # last timestep (first to be solved)
-        stacked_block = simulation.field_derivs[tInd + 1][s_id][r_id].toarray()[
-            :, sub_ind
-        ]
-
-    else:
-        stacked_block = np.asarray(
-            simulation.field_derivs[tInd + 1][s_id][r_id][:, sub_ind]
-            - Asubdiag.T * ATinv_df_duT_v[(s_id, r_id, b_id)][:, local_ind]
-        )
-
-    return stacked_block
-
-
-def update_deriv_blocks(address, tInd, indices, derivatives, solve, shape):
-    if address not in derivatives:
-        deriv_array = np.zeros(shape)
-    else:
-        deriv_array = derivatives[address].compute()
-
-    if address in indices:
-        columns, local_ind = indices[address]
-        deriv_array[:, local_ind] = solve[:, columns]
-
-    derivatives[address] = delayed(deriv_array)
-
-
-def get_field_deriv_block(
-    simulation, block: dict, tInd: int, AdiagTinv, ATinv_df_duT_v: dict, time_mask
-):
-    """
-    Stack the blocks of field derivatives for a given timestep and call the direct solver.
-    """
-    stacked_blocks = []
-    indices = {}
-    count = 0
-
-    Asubdiag = None
-    if tInd < simulation.nT - 1:
-        Asubdiag = simulation.getAsubdiag(tInd + 1)
-
-    for (s_id, r_id, b_id), (rx_ind, j_ind) in block.items():
-        # Cut out early data
-        rx = simulation.survey.source_list[s_id].receiver_list[r_id]
-        time_check = np.kron(time_mask, np.ones(rx.locations.shape[0], dtype=bool))[
-            rx_ind
-        ]
-        sub_ind = rx_ind[time_check]
-        local_ind = np.arange(rx_ind.shape[0])[time_check]
-
-        if len(sub_ind) < 1:
-            continue
-
-        indices[(s_id, r_id, b_id)] = (
-            np.arange(count, count + len(sub_ind)),
-            local_ind,
-        )
-        count += len(sub_ind)
-        deriv_comp = deriv_block(
-            s_id,
-            r_id,
-            b_id,
-            ATinv_df_duT_v,
-            Asubdiag,
-            local_ind,
-            sub_ind,
-            simulation,
-            tInd,
+from .survey import Survey
+from scipy.constants import mu_0
+from scipy.interpolate import InterpolatedUnivariateSpline as iuSpline
+from scipy.special import roots_legendre
+
+from empymod import filters
+from empymod.transform import get_dlf_points
+
+from geoana.kernels.tranverse_electric_reflections import rTE_forward, rTE_gradient
+
+from ...utils import validate_type, validate_string
+
+
+class Simulation1DLayered(BaseEM1DSimulation):
+    """
+    Simulation class for simulating the TEM response over a 1D layered Earth
+    for a single sounding.
+    """
+
+    def __init__(self, survey=None, time_filter="key_81_CosSin_2009", **kwargs):
+        super().__init__(survey=survey, **kwargs)
+        self._coefficients_set = False
+        self.time_filter = time_filter
+
+    @property
+    def survey(self):
+        """The survey for the simulation
+        Returns
+        -------
+        SimPEG.electromagnetics.time_domain.survey.Survey
+        """
+        if self._survey is None:
+            raise AttributeError("Simulation must have a survey set")
+        return self._survey
+
+    @survey.setter
+    def survey(self, value):
+        if value is not None:
+            value = validate_type("survey", value, Survey, cast=False)
+        self._survey = value
+
+    @property
+    def time_filter(self):
+        return self._time_filter
+
+    @time_filter.setter
+    def time_filter(self, value):
+        self._time_filter = validate_string(
+            "time_filter",
+            value,
+            ["key_81_CosSin_2009", "key_201_CosSin_2012", "key_601_CosSin_2009"],
         )
 
-        stacked_blocks.append(
-            array.from_delayed(
-                deriv_comp,
-                dtype=float,
-                shape=(
-                    simulation.field_derivs[tInd][s_id][r_id].shape[0],
-                    len(local_ind),
-                ),
-            )
-        )
-    if len(stacked_blocks) > 0:
-        blocks = array.hstack(stacked_blocks).compute()
-        solve = AdiagTinv * blocks
-    else:
-        solve = None
-
-    update_list = []
-    for address in block:
-        shape = (
-            simulation.field_derivs[tInd][address[0]][address[1]].shape[0],
-            len(block[address][0]),
-        )
-        update_list.append(
-            update_deriv_blocks(address, tInd, indices, ATinv_df_duT_v, solve, shape)
+        if self._time_filter == "key_81_CosSin_2009":
+            self._fftfilt = filters.key_81_CosSin_2009()
+        elif self._time_filter == "key_201_CosSin_2012":
+            self._fftfilt = filters.key_201_CosSin_2012()
+        elif self._time_filter == "key_601_CosSin_2009":
+            self._fftfilt = filters.key_601_CosSin_2009()
+
+    def get_coefficients(self):
+        if self._coefficients_set is False:
+            self._compute_coefficients()
+        return (
+            self._As,
+            self._frequencies,
+            self._lambs,
+            self._unique_lambs,
+            self._inv_lambs,
+            self._C0s,
+            self._C1s,
         )
-    dask.compute(update_list)
-
-    return ATinv_df_duT_v
-
 
-@delayed
-def compute_rows(
-    simulation,
-    tInd,
-    address,  # (s_id, r_id, b_id)
-    indices,  # (rx_ind, j_ind),
-    ATinv_df_duT_v,
-    fields,
-    Jmatrix,
-    ftype,
-    time_mask,
-):
-    """
-    Compute the rows of the sensitivity matrix for a given source and receiver.
-    """
-    src = simulation.survey.source_list[address[0]]
-    rx = src.receiver_list[address[1]]
-    time_check = np.kron(time_mask, np.ones(rx.locations.shape[0], dtype=bool))[
-        indices[0]
-    ]
-    local_ind = np.arange(indices[0].shape[0])[time_check]
-
-    if len(local_ind) < 1:
+    def _set_coefficients(self, coefficients):
+        self._As = coefficients[0]
+        self._frequencies = coefficients[1]
+        self._lambs = coefficients[2]
+        self._unique_lambs = coefficients[3]
+        self._inv_lambs = coefficients[4]
+        self._C0s = coefficients[5]
+        self._C1s = coefficients[6]
+        self._coefficients_set = True
         return
 
-    dAsubdiagT_dm_v = simulation.getAsubdiagDeriv(
-        tInd,
-        fields[src, ftype, tInd],
-        ATinv_df_duT_v[address][:, local_ind],
-        adjoint=True,
-    )
-
-    dRHST_dm_v = simulation.getRHSDeriv(
-        tInd + 1, src, ATinv_df_duT_v[address][:, local_ind], adjoint=True
-    )  # on nodes of time mesh
-
-    un_src = fields[src, ftype, tInd + 1]
-    # cell centered on time mesh
-    dAT_dm_v = simulation.getAdiagDeriv(
-        tInd, un_src, ATinv_df_duT_v[address][:, local_ind], adjoint=True
-    )
+    def _compute_coefficients(self):
+        if self._coefficients_set:
+            return
+        self._compute_hankel_coefficients()
+        survey = self.survey
+
+        t_min = np.infty
+        t_max = -np.infty
+        x, w = roots_legendre(251)
+        # loop through source and receiver lists to find the minimum and maximum
+        # evaluation times for the step response
+        for src in survey.source_list:
+            for rx in src.receiver_list:
+                wave = src.waveform
+                if isinstance(wave, StepOffWaveform):
+                    times = rx.times[rx.times > 0]
+                    t_min = min(times.min(), t_min)
+                    t_max = max(times.max(), t_max)
+                else:
+                    try:
+                        times = rx.times - wave.time_nodes[:, None]
+                        times[times < 0.0] = 0.0
+                        quad_points = (times[:-1] - times[1:])[..., None] * (
+                            x + 1
+                        ) + times[1:, :, None]
+                        t_min = min(quad_points[quad_points > 0].min(), t_min)
+                        t_max = max(quad_points[quad_points > 0].max(), t_max)
+                    except AttributeError:
+                        raise TypeError(
+                            f"Unsupported source waveform object of {src.waveform}"
+                        )
+
+        omegas, t_spline_points = get_dlf_points(self._fftfilt, np.r_[t_min, t_max], -1)
+        omegas = omegas.reshape(-1)
+        n_omega = len(omegas)
+        n_t = len(t_spline_points)
+
+        n_base = len(self._fftfilt.base)
+        A_dft = np.zeros((n_t, n_omega))
+        for i in range(n_t):
+            A_dft[i, i : i + n_base] = self._fftfilt.cos * (-2.0 / np.pi)
+        A_dft = A_dft[::-1]  # shuffle these back
+
+        # Calculate the interpolating spline basis functions for each spline point
+        splines = []
+        for i in range(n_t):
+            e = np.zeros(n_t)
+            e[i] = 1.0
+            sp = iuSpline(np.log(t_spline_points[::-1]), e, k=5)
+            splines.append(sp)
+        # As will go from frequency to time domain
+        As = []
+        for src in survey.source_list:
+            for rx in src.receiver_list:
+                #######
+                # Fourier Transform coefficients
+                ######
+                wave = src.waveform
+
+                def func(t, i):
+                    out = np.zeros_like(t)
+                    t = t.copy()
+                    t[
+                        (t > 0.0) & (t <= t_spline_points.min())
+                    ] = t_spline_points.min()  # constant at very low ts
+                    out[t > 0.0] = splines[i](np.log(t[t > 0.0])) / t[t > 0.0]
+                    return out
+
+                # Then calculate the values at each time
+                A = np.zeros((len(rx.times), n_t))
+                if isinstance(wave, StepOffWaveform):
+                    # do not need to do too much fancy here, just need to interpolate
+                    # from t_spline_points to rx.times (at positive times)...
+                    for i in range(n_t):
+                        A[:, i] = func(rx.times, i)
+                else:
+                    # loop over pairs of nodes and use gaussian quadrature to integrate
+
+                    time_nodes = wave.time_nodes
+                    n_interval = len(time_nodes) - 1
+                    quad_times = []
+                    for i in range(n_interval):
+                        b = rx.times - time_nodes[i]
+                        b = np.maximum(b, 0.0)
+                        a = rx.times - time_nodes[i + 1]
+                        a = np.maximum(a, 0.0)
+                        quad_times = (b - a)[:, None] * (x + 1) / 2.0 + a[:, None]
+                        quad_scale = (b - a) / 2
+                        wave_eval = wave.eval_deriv(rx.times[:, None] - quad_times)
+                        for i in range(n_t):
+                            A[:, i] -= np.sum(
+                                quad_scale[:, None]
+                                * w
+                                * wave_eval
+                                * func(quad_times, i),
+                                axis=-1,
+                            )
+                if isinstance(rx, (PointMagneticFluxDensity, PointMagneticField)):
+                    As.append(A @ (A_dft / omegas))
+                else:
+                    As.append(A @ A_dft)
+                if isinstance(
+                    rx, (PointMagneticFluxTimeDerivative, PointMagneticFluxDensity)
+                ):
+                    As[-1] *= mu_0
+
+            self._frequencies = omegas / (2 * np.pi)
+            self._As = As
+        self._coefficients_set = True
+
+    def dpred(self, m, f=None):
+        """
+        Return predicted data.
+        Predicted data, (`_pred`) are computed when
+        self.fields is called.
+        """
+        if f is None:
+            f = self.fields(m)
+
+        return f
+
+    def fields(self, m):
+        """
+        This method evaluates the Hankel transform for each source and
+        receiver and outputs it as a list. Used for computing response
+        or sensitivities.
+        """
+        self._compute_coefficients()
 
-    Jmatrix[indices[1][time_check], :] += (-dAT_dm_v - dAsubdiagT_dm_v + dRHST_dm_v).T
+        self.model = m
 
+        C0s = self._C0s
+        C1s = self._C1s
 
-def compute_J(self, f=None, Ainv=None):
-    """
-    Compute the rows for the sensitivity matrix.
-    """
+        frequencies = self._frequencies
+        unique_lambs = self._unique_lambs
+        inv_lambs = self._inv_lambs
+        W = self._W
 
-    if f is None:
-        f, Ainv = self.fields(self.model, return_Ainv=True)
+        sig = self.compute_complex_sigma(frequencies)
+        mu = self.compute_complex_mu(frequencies)
 
-    ftype = self._fieldType + "Solution"
-    Jmatrix = delayed(np.zeros((self.survey.nD, self.model.size), dtype=np.float32))
-    simulation_times = np.r_[0, np.cumsum(self.time_steps)] + self.t0
-    data_times = self.survey.source_list[0].receiver_list[0].times
-    blocks = get_parallel_blocks(
-        self.survey.source_list, self.model.shape[0], self.max_chunk_size
-    )
-    self.field_derivs = compute_field_derivs(self, Jmatrix, f)
-    ATinv_df_duT_v = {}
-    for tInd, dt in tqdm(zip(reversed(range(self.nT)), reversed(self.time_steps))):
-        AdiagTinv = Ainv[dt]
-        j_row_updates = []
-        time_mask = data_times > simulation_times[tInd]
-
-        for block in blocks.values():
-            ATinv_df_duT_v = get_field_deriv_block(
-                self, block, tInd, AdiagTinv, ATinv_df_duT_v, time_mask
-            )
-
-            for address, indices in block.items():
-                j_row_updates.append(
-                    compute_rows(
-                        self,
-                        tInd,
-                        address,
-                        indices,
-                        ATinv_df_duT_v,
-                        f,
-                        Jmatrix,
-                        ftype,
-                        time_mask,
-                    )
-                )
-        dask.compute(j_row_updates)
-    for A in Ainv.values():
-        A.clean()
-
-    if self.store_sensitivities == "disk":
-        del Jmatrix
-        return array.from_zarr(self.sensitivity_path + f"J.zarr")
-    else:
-        return Jmatrix.compute()
+        rTE = rTE_forward(frequencies, unique_lambs, sig, mu, self.thicknesses)
+        rTE = rTE[:, inv_lambs]
+        v = ((C0s * rTE) @ self._fhtfilt.j0 + (C1s * rTE) @ self._fhtfilt.j1) @ W.T
 
+        return self._project_to_data(v.T)
 
-Sim.compute_J = compute_J
+    def getJ(self, m, f=None):
+        self.model = m
+        if getattr(self, "_J", None) is None:
+            self._J = {}
+            self._compute_coefficients()
+
+            C0s = self._C0s
+            C1s = self._C1s
+            lambs = self._lambs
+            frequencies = self._frequencies
+            unique_lambs = self._unique_lambs
+            inv_lambs = self._inv_lambs
+            # Had to convert this to an array for a tensor operation (?)
+            W = self._W.toarray()
+
+            sig = self.compute_complex_sigma(frequencies)
+            mu = self.compute_complex_mu(frequencies)
+
+            if self.hMap is not None:
+                # Grab a copy
+                C0s_dh = C0s.copy()
+                C1s_dh = C1s.copy()
+                h_vec = self.h
+                i = 0
+                for i_src, src in enumerate(self.survey.source_list):
+                    h = h_vec[i_src]
+                    nD = sum(rx.locations.shape[0] for rx in src.receiver_list)
+                    ip1 = i + nD
+                    v = np.exp(-lambs[i:ip1] * h)
+                    C0s_dh[i:ip1] *= v * -lambs[i:ip1]
+                    C1s_dh[i:ip1] *= v * -lambs[i:ip1]
+                    i = ip1
+                    # J will be n_d * n_src (each source has it's own h)...
+
+                rTE = rTE_forward(frequencies, unique_lambs, sig, mu, self.thicknesses)
+                rTE = rTE[:, inv_lambs]
+                v_dh_temp = (
+                    W
+                    @ (
+                        (C0s_dh * rTE) @ self._fhtfilt.j0
+                        + (C1s_dh * rTE) @ self._fhtfilt.j1
+                    ).T
+                )
+                # need to re-arange v_dh as it's currently (n_data x n_freqs)
+                # however it already contains all the relevant information...
+                # just need to map it from the rx index to the source index associated..
+                v_dh = np.zeros((self.survey.nSrc, *v_dh_temp.shape))
+
+                i = 0
+                for i_src, src in enumerate(self.survey.source_list):
+                    nD = sum(rx.locations.shape[0] for rx in src.receiver_list)
+                    ip1 = i + nD
+                    v_dh[i_src, i:ip1] = v_dh_temp[i:ip1]
+                    i = ip1
+                v_dh = np.transpose(v_dh, (1, 2, 0))
+                self._J["dh"] = self._project_to_data(v_dh)
+
+            if (
+                self.sigmaMap is not None
+                or self.muMap is not None
+                or self.thicknessesMap is not None
+            ):
+                rTE_ds, rTE_dh, rTE_dmu = rTE_gradient(
+                    frequencies, unique_lambs, sig, mu, self.thicknesses
+                )
+                if self.sigmaMap is not None:
+                    rTE_ds = rTE_ds[..., inv_lambs]
+                    v_ds = (
+                        (
+                            (C0s * rTE_ds) @ self._fhtfilt.j0
+                            + (C1s * rTE_ds) @ self._fhtfilt.j1
+                        )
+                        @ W.T
+                    ).T
+                    self._J["ds"] = self._project_to_data(v_ds)
+                if self.muMap is not None:
+                    rTE_dmu = rTE_dmu[..., inv_lambs]
+                    v_dmu = (
+                        (
+                            (C0s * rTE_dmu) @ self._fhtfilt.j0
+                            + (C1s * rTE_dmu) @ self._fhtfilt.j1
+                        )
+                        @ W.T
+                    ).T
+                    self._J["dmu"] = self._project_to_data(v_dmu)
+                if self.thicknessesMap is not None:
+                    rTE_dh = rTE_dh[..., inv_lambs]
+                    v_dthick = (
+                        (
+                            (C0s * rTE_dh) @ self._fhtfilt.j0
+                            + (C1s * rTE_dh) @ self._fhtfilt.j1
+                        )
+                        @ W.T
+                    ).T
+                    self._J["dthick"] = self._project_to_data(v_dthick)
+        return self._J
+
+    def _project_to_data(self, v):
+        As = self._As
+        if v.ndim == 3:
+            out = np.empty((self.survey.nD, v.shape[-1]))
+        else:
+            out = np.empty((self.survey.nD))
+        i_dat = 0
+        i_A = 0
+        i = 0
+        for src in self.survey.source_list:
+            for rx in src.receiver_list:
+                i_datp1 = i_dat + rx.nD
+                n_locs = rx.locations.shape[0]
+                i_p1 = i + n_locs
+                v_slice = v[np.arange(i, i_p1)]
+                # this should order it as location changing faster than time
+                # i.e. loc_1 t_1, loc_2 t_1, loc1 t2, loc2 t2
+                if v.ndim == 3:
+                    if isinstance(rx, (PointMagneticFluxDensity, PointMagneticField)):
+                        d = np.einsum("ij,...jk->...ik", As[i_A], v_slice.imag)
+                    else:
+                        d = np.einsum("ij,...jk->...ik", As[i_A], v_slice.real)
+                    out[i_dat:i_datp1] = d.reshape((-1, v.shape[-1]), order="F")
+                else:
+                    if isinstance(rx, (PointMagneticFluxDensity, PointMagneticField)):
+                        d = np.einsum("ij,...j->...i", As[i_A], v_slice.imag)
+                    else:
+                        d = np.einsum("ij,...j->...i", As[i_A], v_slice.real)
+                    out[i_dat:i_datp1] = d.reshape(-1, order="F")
+                i_dat = i_datp1
+                i = i_p1
+                i_A += 1
+        return out
```

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/dask/inverse_problem.py` & `mira_simpeg-0.19.0.dev8/SimPEG/dask/inverse_problem.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/dask/objective_function.py` & `mira_simpeg-0.19.0.dev8/SimPEG/dask/objective_function.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/dask/potential_fields/base.py` & `mira_simpeg-0.19.0.dev8/SimPEG/dask/potential_fields/base.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/dask/potential_fields/gravity/simulation.py` & `mira_simpeg-0.19.0.dev8/SimPEG/dask/potential_fields/gravity/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/dask/potential_fields/magnetics/simulation.py` & `mira_simpeg-0.19.0.dev8/SimPEG/dask/potential_fields/magnetics/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/dask/simulation.py` & `mira_simpeg-0.19.0.dev8/SimPEG/dask/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import warnings
 from ..data import SyntheticData
 import numpy as np
 from .utils import compute
 
 Sim._max_ram = 16
 
+
 @property
 def max_ram(self):
     "Maximum ram in (Gb)"
     return self._max_ram
 
 
 @max_ram.setter
@@ -58,15 +59,15 @@
     self._n_cpu = other
 
 
 Sim.n_cpu = n_cpu
 
 
 def make_synthetic_data(
-        self, m, relative_error=0.05, noise_floor=0.0, f=None, add_noise=False, **kwargs
+    self, m, relative_error=0.05, noise_floor=0.0, f=None, add_noise=False, **kwargs
 ):
     """
     Make synthetic data given a model, and a standard deviation.
     :param numpy.ndarray m: geophysical model
     :param numpy.ndarray relative_error: standard deviation
     :param numpy.ndarray noise_floor: noise floor
     :param numpy.ndarray f: fields for the given model (if pre-calculated)
@@ -102,20 +103,21 @@
         survey=self.survey,
         dobs=dobs,
         dclean=dclean,
         relative_error=relative_error,
         noise_floor=noise_floor,
     )
 
+
 Sim.make_synthetic_data = make_synthetic_data
 
 
 @property
 def workers(self):
-    if getattr(self, '_workers', None) is None:
+    if getattr(self, "_workers", None) is None:
         self._workers = None
 
     return self._workers
 
 
 @workers.setter
 def workers(self, workers):
@@ -123,15 +125,15 @@
 
 
 Sim.workers = workers
 
 
 def dask_Jvec(self, m, v):
     """
-        Compute sensitivity matrix (J) and vector (v) product.
+    Compute sensitivity matrix (J) and vector (v) product.
     """
     self.model = m
 
     if isinstance(self.Jmatrix, np.ndarray):
         return self.Jmatrix @ v.astype(np.float32)
 
     if isinstance(self.Jmatrix, Future):
@@ -141,15 +143,15 @@
 
 
 Sim.Jvec = dask_Jvec
 
 
 def dask_Jtvec(self, m, v):
     """
-        Compute adjoint sensitivity matrix (J^T) and vector (v) product.
+    Compute adjoint sensitivity matrix (J^T) and vector (v) product.
     """
     self.model = m
 
     if isinstance(self.Jmatrix, np.ndarray):
         return self.Jmatrix.T @ v.astype(np.float32)
 
     if isinstance(self.Jmatrix, Future):
@@ -170,21 +172,19 @@
         if self.workers is None:
             self._Jmatrix = self.compute_J()
         else:
             client = get_client()  # Assumes a Client already exists
 
             if self.store_sensitivities == "ram":
                 self._Jmatrix = client.persist(
-                    delayed(self.compute_J)(),
-                    workers=self.workers
+                    delayed(self.compute_J)(), workers=self.workers
                 )
             else:
                 self._Jmatrix = client.compute(
-                    delayed(self.compute_J)(),
-                    workers=self.workers
+                    delayed(self.compute_J)(), workers=self.workers
                 )
 
     elif isinstance(self._Jmatrix, Future):
         self._Jmatrix.result()
         if self.store_sensitivities == "disk":
             self._Jmatrix = array.from_zarr(self.sensitivity_path + f"J.zarr")
 
@@ -222,19 +222,21 @@
     def evaluate_receiver(source, receiver, mesh, fields):
         return receiver.eval(source, mesh, fields).flatten()
 
     row = delayed(evaluate_receiver, pure=True)
     rows = []
     for src in self.survey.source_list:
         for rx in src.receiver_list:
-            rows.append(array.from_delayed(
-                row(src, rx, self.mesh, f),
-                dtype=np.float32,
-                shape=(rx.nD,),
-            ))
+            rows.append(
+                array.from_delayed(
+                    row(src, rx, self.mesh, f),
+                    dtype=np.float32,
+                    shape=(rx.nD,),
+                )
+            )
 
     data = array.hstack(rows).compute()
 
     if compute_J and self._Jmatrix is None:
         Jmatrix = self.compute_J(f=f, Ainv=Ainv)
         return data, Jmatrix
 
@@ -242,27 +244,27 @@
 
 
 Sim.dpred = dask_dpred
 
 
 def dask_getJtJdiag(self, m, W=None):
     """
-        Return the diagonal of JtJ
+    Return the diagonal of JtJ
     """
     self.model = m
     if getattr(self, "_jtjdiag", None) is None:
         if isinstance(self.Jmatrix, Future):
             self.Jmatrix  # Wait to finish
 
         if W is None:
             W = np.ones(self.nD)
         else:
             W = W.diagonal() ** 2.0
 
-        diag = array.einsum('i,ij,ij->j', W, self.Jmatrix, self.Jmatrix)
+        diag = array.einsum("i,ij,ij->j", W, self.Jmatrix, self.Jmatrix)
 
         if isinstance(diag, array.Array):
             diag = np.asarray(diag.compute())
 
         self._jtjdiag = diag
 
-    return self._jtjdiag
+    return self._jtjdiag
```

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/dask/utils.py` & `mira_simpeg-0.19.0.dev8/SimPEG/dask/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -36,42 +36,59 @@
     try:
         client = get_client()
         return client.compute(job, workers=self.workers)
     except ValueError:
         return job.compute()
 
 
-def get_parallel_blocks(source_list: list, m_size: int, max_chunk_size: int):
+def get_parallel_blocks(source_list: list, m_size: int, max_chunk_size: int) -> list:
     """
     Get the blocks of sources and receivers to be computed in parallel.
 
-    Stored as a dictionary of source, receiver pairs index. The value is an array of indices
+    Stored as a list of tuples for
+    (source, receiver, block index) and array of indices
     for the rows of the sensitivity matrix.
     """
     data_block_size = np.ceil(max_chunk_size / (m_size * 8.0 * 1e-6))
     row_count = 0
     row_index = 0
     block_count = 0
-    blocks = {0: {}}
+    blocks = [[]]
+
     for s_id, src in enumerate(source_list):
         for r_id, rx in enumerate(src.receiver_list):
             indices = np.arange(rx.nD).astype(int)
             chunks = np.array_split(
                 indices, int(np.ceil(len(indices) / data_block_size))
             )
 
             for ind, chunk in enumerate(chunks):
                 chunk_size = len(chunk)
 
                 # Condition to start a new block
                 if (row_count + chunk_size) > (data_block_size * cpu_count()):
                     row_count = 0
                     block_count += 1
-                    blocks[block_count] = {}
+                    blocks.append([])
 
-                blocks[block_count][(s_id, r_id, ind)] = chunk, np.arange(
-                    row_index, row_index + chunk_size
-                ).astype(int)
+                blocks[block_count].append(
+                    (
+                        (s_id, r_id, ind),
+                        (
+                            chunk,
+                            np.arange(row_index, row_index + chunk_size).astype(int),
+                            rx.locations.shape[0],
+                        ),
+                    )
+                )
                 row_index += chunk_size
                 row_count += chunk_size
 
+    # Re-split over cpu_count if too few blocks
+    if len(blocks) < cpu_count():
+        flatten_blocks = []
+        for block in blocks:
+            flatten_blocks += block
+
+        chunks = np.array_split(np.arange(len(flatten_blocks)), cpu_count())
+        return [[flatten_blocks[i] for i in chunk] for chunk in chunks]
     return blocks
```

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/data.py` & `mira_simpeg-0.19.0.dev8/SimPEG/data.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/data_misfit.py` & `mira_simpeg-0.19.0.dev8/SimPEG/data_misfit.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/directives/__init__.py` & `mira_simpeg-0.19.0.dev8/SimPEG/directives/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/directives/directives.py` & `mira_simpeg-0.19.0.dev8/SimPEG/directives/directives.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,15 +396,15 @@
         int
         """
         return self._seed
 
     @seed.setter
     def seed(self, value):
         if value is not None:
-            value = validate_integer("seed", value, min_val=1)
+            value = validate_integer("seed", value, min_val=0)
         self._seed = value
 
     def validate(self, directive_list):
         ind = [isinstance(d, BaseBetaEstimator) for d in directive_list.dList]
         assert np.sum(ind) == 1, (
             "Multiple directives for computing initial beta detected in directives list. "
             "Only one directive can be used to set the initial beta."
@@ -525,15 +525,17 @@
 
     For a description of the power iteration approach for estimating the larges eigenvalue,
     see :func:`SimPEG.utils.eigenvalue_by_power_iteration`.
 
     """
 
     def __init__(self, beta0_ratio=1.0, n_pw_iter=4, seed=None, **kwargs):
-        super().__init__(beta0_ratio, seed, **kwargs)
+        super().__init__(
+            beta0_ratio=beta0_ratio, n_pw_iter=n_pw_iter, seed=seed, **kwargs
+        )
         self.n_pw_iter = n_pw_iter
 
     @property
     def n_pw_iter(self):
         """Number of power iterations for estimating largest eigenvalues.
 
         Returns
@@ -3158,14 +3160,15 @@
     cartesian_model = None
     mappings = []
     regularization = []
 
     def __init__(
         self, simulations: list, regularizations: ComboObjectiveFunction, **kwargs
     ):
+        self.reference_angles = (False, False, False)
         self.simulations = simulations
         self.regularizations = regularizations
 
         set_kwargs(self, **kwargs)
 
     @property
     def target(self):
@@ -3212,20 +3215,24 @@
             indices = np.hstack(indices)
             nC = mapping.shape[0]
             vec_model = cartesian2spherical(np.vstack(vec_model).T)
             vec_ref = cartesian2spherical(np.vstack(vec_ref).T).flatten()
             model[indices] = vec_model.flatten()
 
             angle_map = []
-            for ind, reg_fun in enumerate(self.regularizations.objfcts):
+            for ind, (reg_fun, ref_angle) in enumerate(
+                zip(self.regularizations.objfcts, self.reference_angles)
+            ):
                 reg_fun.model = model
                 reg_fun.reference_model[indices] = vec_ref
 
                 if ind > 0:
-                    reg_fun.alpha_s = 0
+                    if not ref_angle:
+                        reg_fun.alpha_s = 0
+
                     reg_fun.eps_q = np.pi
                     reg_fun.units = "radian"
                     angle_map.append(reg_fun.mapping)
                 else:
                     reg_fun.units = "amplitude"
 
             # Turn of cross-gradient on angles
```

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/directives/pgi_directives.py` & `mira_simpeg-0.19.0.dev8/SimPEG/directives/pgi_directives.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/directives/sim_directives.py` & `mira_simpeg-0.19.0.dev8/SimPEG/directives/sim_directives.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/__init__.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/analytics/DC.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/DC.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/analytics/FDEM.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/FDEM.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/analytics/FDEMcasing.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/FDEMcasing.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/analytics/FDEMDipolarfields.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/FDEMDipolarfields.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/analytics/NSEM.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/NSEM.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/analytics/TDEM.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/TDEM.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/base.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/base.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/base_1d.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/base_1d.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/frequency_domain/__init__.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/frequency_domain/fields.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/fields.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/frequency_domain/receivers.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/receivers.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/frequency_domain/simulation.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/frequency_domain/simulation_1d.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/simulation_1d.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/frequency_domain/sources.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/sources.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/frequency_domain/survey.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/survey.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/__init__.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/fields.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/fields.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/receivers.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/receivers.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/simulation.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/simulation_1d.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/simulation_1d.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/sources.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/sources.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/survey.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/survey.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/utils/__init__.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/utils/analytic_1d.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/analytic_1d.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/utils/data_utils.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/utils/data_viewer.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/data_viewer.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/utils/edi_files_utils.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/edi_files_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/utils/plot_data_types.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/plot_data_types.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/utils/plot_utils.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/utils/solutions_1d.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/solutions_1d.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/utils/source_utils.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/source_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/natural_source/utils/test_utils.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/induced_polarization/__init__.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/induced_polarization/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/induced_polarization/run.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/induced_polarization/run.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/induced_polarization/simulation.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/induced_polarization/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/induced_polarization/survey.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/induced_polarization/survey.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/resistivity/__init__.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/resistivity/fields.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/fields.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/resistivity/fields_2d.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/fields_2d.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/resistivity/IODC.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/IODC.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/resistivity/receivers.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/receivers.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/resistivity/run.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/run.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/resistivity/simulation.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/resistivity/simulation_1d.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/simulation_1d.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/resistivity/simulation_2d.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/simulation_2d.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/resistivity/sources.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/sources.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/resistivity/survey.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/survey.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/resistivity/utils.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/spectral_induced_polarization/__init__.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/spectral_induced_polarization/data.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/data.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/spectral_induced_polarization/receivers.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/receivers.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/spectral_induced_polarization/run.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/run.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/spectral_induced_polarization/simulation.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/spectral_induced_polarization/simulation_2d.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/simulation_2d.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/spectral_induced_polarization/sources.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/sources.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/spectral_induced_polarization/survey.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/survey.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/spontaneous_potential/__init__.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spontaneous_potential/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/spontaneous_potential/simulation.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spontaneous_potential/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/spontaneous_potential/sources.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spontaneous_potential/sources.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/utils/__init__.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/static/utils/static_utils.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/utils/static_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/time_domain/__init__.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/time_domain/fields.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,16 @@
             )
         return self._bDeriv_u(tInd, src, dun_dm_v) + self._bDeriv_m(tInd, src, v)
 
     def _dbdtDeriv(self, tInd, src, dun_dm_v, v, adjoint=False):
         if adjoint is True:
             return (
                 self._dbdtDeriv_u(tInd, src, v, adjoint),
-                self._dbdtDeriv_m(tInd, src, v, adjoint),
+                Zero()
+                # self._dbdtDeriv_m(tInd, src, v, adjoint),
             )
         return self._dbdtDeriv_u(tInd, src, dun_dm_v) + self._dbdtDeriv_m(tInd, src, v)
 
     def _hDeriv(self, tInd, src, dun_dm_v, v, adjoint=False):
         if adjoint is True:
             return (
                 self._hDeriv_u(tInd, src, v, adjoint),
@@ -156,15 +157,15 @@
         for i, src in enumerate(source_list):
             s_m = src.s_m(self.simulation, self._times[tInd])
             dbdt[:, i] = dbdt[:, i] + s_m
         return dbdt
 
     def _dbdtDeriv_u(self, tInd, src, dun_dm_v, adjoint=False):
         if adjoint is True:
-            return -self._eDeriv_u(tInd, src, self._edgeCurl.T * dun_dm_v, adjoint)
+            return -self._eDeriv_u(tInd, src, self._edgeCurl.T @ dun_dm_v, adjoint)
         return -(self._edgeCurl * self._eDeriv_u(tInd, src, dun_dm_v))
 
     def _dbdtDeriv_m(self, tInd, src, v, adjoint=False):
         if adjoint is True:
             return -(self._eDeriv_m(tInd, src, self._edgeCurl.T * v, adjoint))
         return -(
             self._edgeCurl * self._eDeriv_m(tInd, src, v)
@@ -175,15 +176,15 @@
         for i, src in enumerate(source_list):
             s_e = src.s_e(self.simulation, self._times[tInd])
             e[:, i] = e[:, i] - self._MeSigmaI * s_e
         return e
 
     def _eDeriv_u(self, tInd, src, dun_dm_v, adjoint=False):
         if adjoint is True:
-            return self._MfMui.T * (self._edgeCurl * (self._MeSigmaI.T * dun_dm_v))
+            return self._MfMui.T @ (self._edgeCurl @ (self._MeSigmaI.T @ dun_dm_v))
         return self._MeSigmaI * (self._edgeCurl.T * (self._MfMui * dun_dm_v))
 
     def _eDeriv_m(self, tInd, src, v, adjoint=False):
         _, s_e = src.eval(self.simulation, self._times[tInd])
         bSolution = self[[src], "bSolution", tInd].flatten()
 
         _, s_eDeriv = src.evalDeriv(self._times[tInd], self, adjoint=adjoint)
```

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/time_domain/receivers.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/receivers.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,22 +95,25 @@
         f : SimPEG.electromagnetics.time_domain.fields.FieldsTDEM
 
         Returns
         -------
         scipy.sparse.csr_matrix
             P, the interpolation matrix
         """
-        P = Zero()
-        field = f._GLoc(self.projField)
-        for strength, comp in zip(self.orientation, ["x", "y", "z"]):
-            if strength != 0.0:
-                P = P + strength * mesh.get_interpolation_matrix(
-                    self.locations, field + comp
-                )
-        return P
+        if getattr(self, "spatialP", None) is None:
+            P = Zero()
+            field = f._GLoc(self.projField)
+            for strength, comp in zip(self.orientation, ["x", "y", "z"]):
+                if strength != 0.0:
+                    P = P + strength * mesh.get_interpolation_matrix(
+                        self.locations, field + comp
+                    )
+            self.spatialP = P
+
+        return self.spatialP
 
     def getTimeP(self, time_mesh, f):
         """Get time projection matrix from mesh to receivers.
 
         Only constructed when called.
 
         Parameters
@@ -120,16 +123,21 @@
         f : SimPEG.electromagnetics.time_domain.fields.FieldsTDEM
 
         Returns
         -------
         scipy.sparse.csr_matrix
             P, the interpolation matrix
         """
-        projected_time_grid = f._TLoc(self.projField)
-        return time_mesh.get_interpolation_matrix(self.times, projected_time_grid)
+        if getattr(self, "timeP", None) is None:
+            projected_time_grid = f._TLoc(self.projField)
+            self.timeP = time_mesh.get_interpolation_matrix(
+                self.times, projected_time_grid
+            )
+
+        return self.timeP
 
     def getP(self, mesh, time_mesh, f):
         """Returns projection matrices as a list for all components collected by the receivers.
 
         Parameters
         ----------
         mesh : discretize.BaseMesh
```

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/time_domain/simulation.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/time_domain/simulation_1d.py` & `mira_simpeg-0.19.0.dev8/SimPEG/flow/richards/simulation.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,371 +1,422 @@
-from ..base_1d import BaseEM1DSimulation
-from .sources import StepOffWaveform
-from .receivers import (
-    PointMagneticFluxDensity,
-    PointMagneticField,
-    PointMagneticFluxTimeDerivative,
-)
 import numpy as np
+import scipy.sparse as sp
+import time
+
+from ... import utils
+from ...simulation import BaseTimeSimulation
+from ... import optimization
+from ...utils import (
+    validate_type,
+    validate_ndarray_with_shape,
+    deprecate_property,
+    validate_string,
+    validate_integer,
+    validate_float,
+)
+from ...props import NestedModeler
+
+from .empirical import BaseHydraulicConductivity
+from .empirical import BaseWaterRetention
+
 
-from .survey import Survey
-from scipy.constants import mu_0
-from scipy.interpolate import InterpolatedUnivariateSpline as iuSpline
-from scipy.special import roots_legendre
+class SimulationNDCellCentered(BaseTimeSimulation):
+    """Richards Simulation"""
+
+    def __init__(
+        self,
+        mesh,
+        hydraulic_conductivity,
+        water_retention,
+        boundary_conditions,
+        initial_conditions,
+        method="mixed",
+        do_newton=False,
+        root_finder_max_iter=30,
+        root_finder_tol=1e-4,
+        **kwargs
+    ):
+        debug = kwargs.pop("debug", None)
+        if debug is not None:
+            self.debug = debug
+        super().__init__(mesh=mesh, **kwargs)
+        self.hydraulic_conductivity = hydraulic_conductivity
+        self.water_retention = water_retention
+        self.boundary_conditions = boundary_conditions
+        self.initial_conditions = initial_conditions
+        self.method = method
+        self.do_newton = do_newton
+        self.root_finder_max_iter = root_finder_max_iter
+        self.root_finder_tol = root_finder_tol
+
+    hydraulic_conductivity = NestedModeler(
+        BaseHydraulicConductivity, "hydraulic conductivity function"
+    )
+    water_retention = NestedModeler(BaseWaterRetention, "water retention curve")
+
+    # TODO: This can also be a function(time, u_ii)
+    @property
+    def boundary_conditions(self):
+        """The boundary conditions.
+
+        Returns
+        -------
+        numpy.ndarray
+        """
+        return self._boundary_conditions
+
+    @boundary_conditions.setter
+    def boundary_conditions(self, value):
+        self._boundary_conditions = validate_ndarray_with_shape(
+            "boundary_conditions", value
+        )
+
+    @property
+    def initial_conditions(self):
+        """The initial conditions.
+
+        Returns
+        -------
+        numpy.ndarray
+        """
+        return self._initial_conditions
 
-from empymod import filters
-from empymod.transform import get_dlf_points
+    @initial_conditions.setter
+    def initial_conditions(self, value):
+        self._initial_conditions = validate_ndarray_with_shape(
+            "initial_conditions", value
+        )
 
-from geoana.kernels.tranverse_electric_reflections import rTE_forward, rTE_gradient
+    debug = deprecate_property(
+        BaseTimeSimulation.verbose, "debug", "verbose", removal_version="0.19.0"
+    )
 
-from ...utils import validate_type, validate_string
+    @property
+    def method(self):
+        """Formulation used.
 
+        See notes in Celia et al., 1990
 
-class Simulation1DLayered(BaseEM1DSimulation):
-    """
-    Simulation class for simulating the TEM response over a 1D layered Earth
-    for a single sounding.
-    """
+        Returns
+        -------
+        {"mixed", "head"}
+        """
+        return self._method
 
-    def __init__(self, survey=None, time_filter="key_81_CosSin_2009", **kwargs):
-        super().__init__(survey=survey, **kwargs)
-        self._coefficients_set = False
-        self.time_filter = time_filter
+    @method.setter
+    def method(self, value):
+        self._method = validate_string("method", value, ["mixed", "head"])
 
     @property
-    def survey(self):
-        """The survey for the simulation
+    def do_newton(self):
+        """Do a Newton iteration vs. a Picard iteration.
+
         Returns
         -------
-        SimPEG.electromagnetics.time_domain.survey.Survey
+        bool
         """
-        if self._survey is None:
-            raise AttributeError("Simulation must have a survey set")
-        return self._survey
-
-    @survey.setter
-    def survey(self, value):
-        if value is not None:
-            value = validate_type("survey", value, Survey, cast=False)
-        self._survey = value
+        return self._do_newton
+
+    @do_newton.setter
+    def do_newton(self, value):
+        self._do_newton = validate_type("do_newton", value, bool)
+        if hasattr(self, "_root_finder"):
+            del self._root_finder
 
     @property
-    def time_filter(self):
-        return self._time_filter
+    def root_finder_max_iter(self):
+        """Maximum iterations for root_finder iteration.
 
-    @time_filter.setter
-    def time_filter(self, value):
-        self._time_filter = validate_string(
-            "time_filter",
-            value,
-            ["key_81_CosSin_2009", "key_201_CosSin_2012", "key_601_CosSin_2009"],
+        Returns
+        -------
+        int
+        """
+        return self._root_finder_max_iter
+
+    @root_finder_max_iter.setter
+    def root_finder_max_iter(self, value):
+        self._root_finder_max_iter = validate_integer(
+            "root_finder_max_iter", value, min_val=1
         )
+        if hasattr(self, "_root_finder"):
+            del self._root_finder
 
-        if self._time_filter == "key_81_CosSin_2009":
-            self._fftfilt = filters.key_81_CosSin_2009()
-        elif self._time_filter == "key_201_CosSin_2012":
-            self._fftfilt = filters.key_201_CosSin_2012()
-        elif self._time_filter == "key_601_CosSin_2009":
-            self._fftfilt = filters.key_601_CosSin_2009()
-
-    def get_coefficients(self):
-        if self._coefficients_set is False:
-            self._compute_coefficients()
-        return (
-            self._As,
-            self._frequencies,
-            self._lambs,
-            self._unique_lambs,
-            self._inv_lambs,
-            self._C0s,
-            self._C1s,
+    @property
+    def root_finder_tol(self):
+        return self._root_finder_tol
+
+    @root_finder_tol.setter
+    def root_finder_tol(self, value):
+        self._root_finder_tol = validate_float(
+            "root_finder_tol", value, min_val=0.0, inclusive_min=False
         )
+        if hasattr(self, "_root_finder"):
+            del self._root_finder
+
+    def getBoundaryConditions(self, ii, u_ii):
+        if isinstance(self.boundary_conditions, np.ndarray):
+            return self.boundary_conditions
+
+        time = self.time_mesh.cell_centers_x[ii]
+
+        return self.boundary_conditions(time, u_ii)
+
+    @property
+    def root_finder(self):
+        """Root-finding Algorithm"""
+        if getattr(self, "_root_finder", None) is None:
+            self._root_finder = optimization.NewtonRoot(
+                doLS=self.do_newton,
+                maxIter=self.root_finder_max_iter,
+                tol=self.root_finder_tol,
+                Solver=self.solver,
+            )
+        return self._root_finder
+
+    @utils.timeIt
+    def fields(self, m=None):
+        if self.water_retention.needs_model or self.hydraulic_conductivity.needs_model:
+            assert m is not None
+        else:
+            assert m is None
 
-    def _set_coefficients(self, coefficients):
-        self._As = coefficients[0]
-        self._frequencies = coefficients[1]
-        self._lambs = coefficients[2]
-        self._unique_lambs = coefficients[3]
-        self._inv_lambs = coefficients[4]
-        self._C0s = coefficients[5]
-        self._C1s = coefficients[6]
-        self._coefficients_set = True
-        return
-
-    def _compute_coefficients(self):
-        if self._coefficients_set:
-            return
-        self._compute_hankel_coefficients()
-        survey = self.survey
-
-        t_min = np.infty
-        t_max = -np.infty
-        x, w = roots_legendre(251)
-        # loop through source and receiver lists to find the minimum and maximum
-        # evaluation times for the step response
-        for src in survey.source_list:
-            for rx in src.receiver_list:
-                wave = src.waveform
-                if isinstance(wave, StepOffWaveform):
-                    times = rx.times[rx.times > 0]
-                    t_min = min(times.min(), t_min)
-                    t_max = max(times.max(), t_max)
-                else:
-                    try:
-                        times = rx.times - wave.time_nodes[:, None]
-                        times[times < 0.0] = 0.0
-                        quad_points = (times[:-1] - times[1:])[..., None] * (
-                            x + 1
-                        ) + times[1:, :, None]
-                        t_min = min(quad_points[quad_points > 0].min(), t_min)
-                        t_max = max(quad_points[quad_points > 0].max(), t_max)
-                    except AttributeError:
-                        raise TypeError(
-                            f"Unsupported source waveform object of {src.waveform}"
-                        )
-
-        omegas, t_spline_points = get_dlf_points(self._fftfilt, np.r_[t_min, t_max], -1)
-        omegas = omegas.reshape(-1)
-        n_omega = len(omegas)
-        n_t = len(t_spline_points)
-
-        n_base = len(self._fftfilt.base)
-        A_dft = np.zeros((n_t, n_omega))
-        for i in range(n_t):
-            A_dft[i, i : i + n_base] = self._fftfilt.cos * (-2.0 / np.pi)
-        A_dft = A_dft[::-1]  # shuffle these back
-
-        # Calculate the interpolating spline basis functions for each spline point
-        splines = []
-        for i in range(n_t):
-            e = np.zeros(n_t)
-            e[i] = 1.0
-            sp = iuSpline(np.log(t_spline_points[::-1]), e, k=5)
-            splines.append(sp)
-        # As will go from frequency to time domain
-        As = []
-        for src in survey.source_list:
-            for rx in src.receiver_list:
-                #######
-                # Fourier Transform coefficients
-                ######
-                wave = src.waveform
-
-                def func(t, i):
-                    out = np.zeros_like(t)
-                    t = t.copy()
-                    t[
-                        (t > 0.0) & (t <= t_spline_points.min())
-                    ] = t_spline_points.min()  # constant at very low ts
-                    out[t > 0.0] = splines[i](np.log(t[t > 0.0])) / t[t > 0.0]
-                    return out
-
-                # Then calculate the values at each time
-                A = np.zeros((len(rx.times), n_t))
-                if isinstance(wave, StepOffWaveform):
-                    # do not need to do too much fancy here, just need to interpolate
-                    # from t_spline_points to rx.times (at positive times)...
-                    for i in range(n_t):
-                        A[:, i] = func(rx.times, i)
-                else:
-                    # loop over pairs of nodes and use gaussian quadrature to integrate
-
-                    time_nodes = wave.time_nodes
-                    n_interval = len(time_nodes) - 1
-                    quad_times = []
-                    for i in range(n_interval):
-                        b = rx.times - time_nodes[i]
-                        b = np.maximum(b, 0.0)
-                        a = rx.times - time_nodes[i + 1]
-                        a = np.maximum(a, 0.0)
-                        quad_times = (b - a)[:, None] * (x + 1) / 2.0 + a[:, None]
-                        quad_scale = (b - a) / 2
-                        wave_eval = wave.eval_deriv(rx.times[:, None] - quad_times)
-                        for i in range(n_t):
-                            A[:, i] -= np.sum(
-                                quad_scale[:, None]
-                                * w
-                                * wave_eval
-                                * func(quad_times, i),
-                                axis=-1,
-                            )
-                if isinstance(rx, (PointMagneticFluxDensity, PointMagneticField)):
-                    As.append(A @ (A_dft / omegas))
-                else:
-                    As.append(A @ A_dft)
-                if isinstance(
-                    rx, (PointMagneticFluxTimeDerivative, PointMagneticFluxDensity)
-                ):
-                    As[-1] *= mu_0
-
-            self._frequencies = omegas / (2 * np.pi)
-            self._As = As
-        self._coefficients_set = True
+        tic = time.time()
+        u = list(range(self.nT + 1))
+        u[0] = self.initial_conditions
+        for ii, dt in enumerate(self.time_steps):
+            bc = self.getBoundaryConditions(ii, u[ii])
+            u[ii + 1] = self.root_finder.root(
+                lambda hn1m, return_g=True: self.getResidual(
+                    m, u[ii], hn1m, dt, bc, return_g=return_g  # noqa: B023
+                ),
+                u[ii],
+            )
+            if self.verbose:
+                print(
+                    "Solving Fields ({0:4d}/{1:d} - {2:3.1f}% Done) {3:d} "
+                    "Iterations, {4:4.2f} seconds".format(
+                        ii + 1,
+                        self.nT,
+                        100.0 * (ii + 1) / self.nT,
+                        self.root_finder.iter,
+                        time.time() - tic,
+                    )
+                )
+        return u
 
     def dpred(self, m, f=None):
-        """
-        Return predicted data.
-        Predicted data, (`_pred`) are computed when
-        self.fields is called.
+        r"""
+        Create the projected data from a model.
+
+        The field, f, (if provided) will be used for the predicted data
+        instead of recalculating the fields (which may be expensive!).
+
+        .. math::
+
+            d_\text{pred} = P(f(m), m)
+
+        Where P is a projection of the fields onto the data space.
         """
         if f is None:
             f = self.fields(m)
 
-        return f
+        Ds = list(range(len(self.survey.receiver_list)))
+
+        for ii, rx in enumerate(self.survey.receiver_list):
+            Ds[ii] = rx(f, self)
 
-    def fields(self, m):
+        return np.concatenate(Ds)
+
+    @property
+    def Dz(self):
+        if self.mesh.dim == 1:
+            return self.mesh.face_x_divergence
+
+        if self.mesh.dim == 2:
+            mats = (
+                utils.spzeros(self.mesh.nC, self.mesh.vnF[0]),
+                self.mesh.face_y_divergence,
+            )
+        elif self.mesh.dim == 3:
+            mats = (
+                utils.spzeros(self.mesh.nC, self.mesh.vnF[0] + self.mesh.vnF[1]),
+                self.mesh.face_z_divergence,
+            )
+        return sp.hstack(mats, format="csr")
+
+    @utils.timeIt
+    def diagsJacobian(self, m, hn, hn1, dt, bc):
+        """Diagonals and rhs of the jacobian system
+
+        The matrix that we are computing has the form::
+
+        .. code::
+
+            .-                                      -. .-  -.   .-  -.
+            |  Adiag                                 | | h1 |   | b1 |
+            |   Asub    Adiag                        | | h2 |   | b2 |
+            |            Asub    Adiag               | | h3 | = | b3 |
+            |                 ...     ...            | | .. |   | .. |
+            |                         Asub    Adiag  | | hn |   | bn |
+            '-                                      -' '-  -'   '-  -'
         """
-        This method evaluates the Hankel transform for each source and
-        receiver and outputs it as a list. Used for computing response
-        or sensitivities.
+        if m is not None:
+            self.model = m
+
+        DIV = self.mesh.face_divergence
+        GRAD = self.mesh.cell_gradient
+        BC = self.mesh.cell_gradient_BC
+        AV = self.mesh.aveF2CC.T
+        Dz = self.Dz
+
+        dT = self.water_retention.derivU(hn)
+        dT1 = self.water_retention.derivU(hn1)
+        dTm = self.water_retention.derivM(hn)
+        dTm1 = self.water_retention.derivM(hn1)
+
+        K1 = self.hydraulic_conductivity(hn1)
+        dK1 = self.hydraulic_conductivity.derivU(hn1)
+        dKm1 = self.hydraulic_conductivity.derivM(hn1)
+
+        # Compute part of the derivative of:
+        #
+        #       DIV*diag(GRAD*hn1+BC*bc)*(AV*(1.0/K))^-1
+
+        DdiagGh1 = DIV * utils.sdiag(GRAD * hn1 + BC * bc)
+        diagAVk2_AVdiagK2 = (
+            utils.sdiag((AV * (1.0 / K1)) ** (-2)) * AV * utils.sdiag(K1 ** (-2))
+        )
+
+        Asub = (-1.0 / dt) * dT
+
+        Adiag = (
+            (1.0 / dt) * dT1
+            - DdiagGh1 * diagAVk2_AVdiagK2 * dK1
+            - DIV * utils.sdiag(1.0 / (AV * (1.0 / K1))) * GRAD
+            - Dz * diagAVk2_AVdiagK2 * dK1
+        )
+
+        B = (
+            DdiagGh1 * diagAVk2_AVdiagK2 * dKm1
+            + Dz * diagAVk2_AVdiagK2 * dKm1
+            + (1.0 / dt) * (dTm - dTm1)
+        )
+
+        return Asub, Adiag, B
+
+    @utils.timeIt
+    def getResidual(self, m, hn, h, dt, bc, return_g=True):
+        """Used by the root finder when going between timesteps
+
+        Where h is the proposed value for the next time iterate (h_{n+1})
         """
-        self._compute_coefficients()
+        if m is not None:
+            self.model = m
 
-        self.model = m
+        DIV = self.mesh.face_divergence
+        GRAD = self.mesh.cell_gradient
+        BC = self.mesh.cell_gradient_BC
+        AV = self.mesh.aveF2CC.T
+        Dz = self.Dz
+
+        T = self.water_retention(h)
+        dT = self.water_retention.derivU(h)
+        Tn = self.water_retention(hn)
+        K = self.hydraulic_conductivity(h)
+        dK = self.hydraulic_conductivity.derivU(h)
+
+        aveK = 1.0 / (AV * (1.0 / K))
+
+        RHS = DIV * utils.sdiag(aveK) * (GRAD * h + BC * bc) + Dz * aveK
+        if self.method == "mixed":
+            r = (T - Tn) / dt - RHS
+        elif self.method == "head":
+            r = dT * (h - hn) / dt - RHS
+
+        if not return_g:
+            return r
+
+        J = dT / dt - DIV * utils.sdiag(aveK) * GRAD
+        if self.do_newton:
+            DDharmAve = utils.sdiag(aveK**2) * AV * utils.sdiag(K ** (-2)) * dK
+            J = J - DIV * utils.sdiag(GRAD * h + BC * bc) * DDharmAve - Dz * DDharmAve
 
-        C0s = self._C0s
-        C1s = self._C1s
+        return r, J
 
-        frequencies = self._frequencies
-        unique_lambs = self._unique_lambs
-        inv_lambs = self._inv_lambs
-        W = self._W
-
-        sig = self.compute_complex_sigma(frequencies)
-        mu = self.compute_complex_mu(frequencies)
-
-        rTE = rTE_forward(frequencies, unique_lambs, sig, mu, self.thicknesses)
-        rTE = rTE[:, inv_lambs]
-        v = ((C0s * rTE) @ self._fhtfilt.j0 + (C1s * rTE) @ self._fhtfilt.j1) @ W.T
-
-        return self._project_to_data(v.T)
-
-    def getJ(self, m, f=None):
-        self.model = m
-        if getattr(self, "_J", None) is None:
-            self._J = {}
-            self._compute_coefficients()
-
-            C0s = self._C0s
-            C1s = self._C1s
-            lambs = self._lambs
-            frequencies = self._frequencies
-            unique_lambs = self._unique_lambs
-            inv_lambs = self._inv_lambs
-            # Had to convert this to an array for a tensor operation (?)
-            W = self._W.toarray()
-
-            sig = self.compute_complex_sigma(frequencies)
-            mu = self.compute_complex_mu(frequencies)
-
-            if self.hMap is not None:
-                # Grab a copy
-                C0s_dh = C0s.copy()
-                C1s_dh = C1s.copy()
-                h_vec = self.h
-                i = 0
-                for i_src, src in enumerate(self.survey.source_list):
-                    h = h_vec[i_src]
-                    nD = sum(rx.locations.shape[0] for rx in src.receiver_list)
-                    ip1 = i + nD
-                    v = np.exp(-lambs[i:ip1] * h)
-                    C0s_dh[i:ip1] *= v * -lambs[i:ip1]
-                    C1s_dh[i:ip1] *= v * -lambs[i:ip1]
-                    i = ip1
-                    # J will be n_d * n_src (each source has it's own h)...
-
-                rTE = rTE_forward(frequencies, unique_lambs, sig, mu, self.thicknesses)
-                rTE = rTE[:, inv_lambs]
-                v_dh_temp = (
-                    W
-                    @ (
-                        (C0s_dh * rTE) @ self._fhtfilt.j0
-                        + (C1s_dh * rTE) @ self._fhtfilt.j1
-                    ).T
-                )
-                # need to re-arange v_dh as it's currently (n_data x n_freqs)
-                # however it already contains all the relevant information...
-                # just need to map it from the rx index to the source index associated..
-                v_dh = np.zeros((self.survey.nSrc, *v_dh_temp.shape))
-
-                i = 0
-                for i_src, src in enumerate(self.survey.source_list):
-                    nD = sum(rx.locations.shape[0] for rx in src.receiver_list)
-                    ip1 = i + nD
-                    v_dh[i_src, i:ip1] = v_dh_temp[i:ip1]
-                    i = ip1
-                v_dh = np.transpose(v_dh, (1, 2, 0))
-                self._J["dh"] = self._project_to_data(v_dh)
-
-            if (
-                self.sigmaMap is not None
-                or self.muMap is not None
-                or self.thicknessesMap is not None
-            ):
-                rTE_ds, rTE_dh, rTE_dmu = rTE_gradient(
-                    frequencies, unique_lambs, sig, mu, self.thicknesses
-                )
-                if self.sigmaMap is not None:
-                    rTE_ds = rTE_ds[..., inv_lambs]
-                    v_ds = (
-                        (
-                            (C0s * rTE_ds) @ self._fhtfilt.j0
-                            + (C1s * rTE_ds) @ self._fhtfilt.j1
-                        )
-                        @ W.T
-                    ).T
-                    self._J["ds"] = self._project_to_data(v_ds)
-                if self.muMap is not None:
-                    rTE_dmu = rTE_dmu[..., inv_lambs]
-                    v_dmu = (
-                        (
-                            (C0s * rTE_dmu) @ self._fhtfilt.j0
-                            + (C1s * rTE_dmu) @ self._fhtfilt.j1
-                        )
-                        @ W.T
-                    ).T
-                    self._J["dmu"] = self._project_to_data(v_dmu)
-                if self.thicknessesMap is not None:
-                    rTE_dh = rTE_dh[..., inv_lambs]
-                    v_dthick = (
-                        (
-                            (C0s * rTE_dh) @ self._fhtfilt.j0
-                            + (C1s * rTE_dh) @ self._fhtfilt.j1
-                        )
-                        @ W.T
-                    ).T
-                    self._J["dthick"] = self._project_to_data(v_dthick)
-        return self._J
-
-    def _project_to_data(self, v):
-        As = self._As
-        if v.ndim == 3:
-            out = np.empty((self.survey.nD, v.shape[-1]))
-        else:
-            out = np.empty((self.survey.nD))
-        i_dat = 0
-        i_A = 0
-        i = 0
-        for src in self.survey.source_list:
-            for rx in src.receiver_list:
-                i_datp1 = i_dat + rx.nD
-                n_locs = rx.locations.shape[0]
-                i_p1 = i + n_locs
-                v_slice = v[np.arange(i, i_p1)]
-                # this should order it as location changing faster than time
-                # i.e. loc_1 t_1, loc_2 t_1, loc1 t2, loc2 t2
-                if v.ndim == 3:
-                    if isinstance(rx, (PointMagneticFluxDensity, PointMagneticField)):
-                        d = np.einsum("ij,...jk->...ik", As[i_A], v_slice.imag)
-                    else:
-                        d = np.einsum("ij,...jk->...ik", As[i_A], v_slice.real)
-                    out[i_dat:i_datp1] = d.reshape((-1, v.shape[-1]), order="F")
-                else:
-                    if isinstance(rx, (PointMagneticFluxDensity, PointMagneticField)):
-                        d = np.einsum("ij,...j->...i", As[i_A], v_slice.imag)
-                    else:
-                        d = np.einsum("ij,...j->...i", As[i_A], v_slice.real)
-                    out[i_dat:i_datp1] = d.reshape(-1, order="F")
-                i_dat = i_datp1
-                i = i_p1
-                i_A += 1
-        return out
+    @utils.timeIt
+    def Jfull(self, m=None, f=None):
+        if f is None:
+            f = self.fields(m)
+
+        nn = len(f) - 1
+        Asubs, Adiags, Bs = list(range(nn)), list(range(nn)), list(range(nn))
+        for ii in range(nn):
+            dt = self.time_steps[ii]
+            bc = self.getBoundaryConditions(ii, f[ii])
+            Asubs[ii], Adiags[ii], Bs[ii] = self.diagsJacobian(
+                m, f[ii], f[ii + 1], dt, bc
+            )
+        Ad = sp.block_diag(Adiags)
+        zRight = utils.spzeros((len(Asubs) - 1) * Asubs[0].shape[0], Adiags[0].shape[1])
+        zTop = utils.spzeros(Adiags[0].shape[0], len(Adiags) * Adiags[0].shape[1])
+        As = sp.vstack((zTop, sp.hstack((sp.block_diag(Asubs[1:]), zRight))))
+        A = As + Ad
+        B = np.array(sp.vstack(Bs).todense())
+
+        Ainv = self.solver(A, **self.solver_opts)
+        AinvB = Ainv * B
+        z = np.zeros((self.mesh.nC, B.shape[1]))
+        du_dm = np.vstack((z, AinvB))
+        J = self.survey.deriv(self, f, du_dm_v=du_dm)  # not multiplied by v
+        return J
+
+    @utils.timeIt
+    def Jvec(self, m, v, f=None):
+        if f is None:
+            f = self.fields(m)
+
+        JvC = list(range(len(f) - 1))  # Cell to hold each row of the long vector
+
+        # This is done via forward substitution.
+        bc = self.getBoundaryConditions(0, f[0])
+        temp, Adiag, B = self.diagsJacobian(m, f[0], f[1], self.time_steps[0], bc)
+        Adiaginv = self.solver(Adiag, **self.solver_opts)
+        JvC[0] = Adiaginv * (B * v)
+
+        for ii in range(1, len(f) - 1):
+            bc = self.getBoundaryConditions(ii, f[ii])
+            Asub, Adiag, B = self.diagsJacobian(
+                m, f[ii], f[ii + 1], self.time_steps[ii], bc
+            )
+            Adiaginv = self.solver(Adiag, **self.solver_opts)
+            JvC[ii] = Adiaginv * (B * v - Asub * JvC[ii - 1])
+
+        du_dm_v = np.concatenate([np.zeros(self.mesh.nC)] + JvC)
+        Jv = self.survey.deriv(self, f, du_dm_v=du_dm_v, v=v)
+        return Jv
+
+    @utils.timeIt
+    def Jtvec(self, m, v, f=None):
+        if f is None:
+            f = self.field(m)
+
+        PTv, PTdv = self.survey.derivAdjoint(self, f, v=v)
+
+        # This is done via backward substitution.
+        minus = 0
+        BJtv = 0
+        for ii in range(len(f) - 1, 0, -1):
+            bc = self.getBoundaryConditions(ii - 1, f[ii - 1])
+            Asub, Adiag, B = self.diagsJacobian(
+                m, f[ii - 1], f[ii], self.time_steps[ii - 1], bc
+            )
+            # select the correct part of v
+            vpart = list(range((ii) * Adiag.shape[0], (ii + 1) * Adiag.shape[0]))
+            AdiaginvT = self.solver(Adiag.T, **self.solver_opts)
+            JTvC = AdiaginvT * (PTv[vpart] - minus)
+            minus = Asub.T * JTvC  # this is now the super diagonal.
+            BJtv = BJtv + B.T * JTvC
+
+        return BJtv + PTdv
+
+
+SimulationNDCellCentred = SimulationNDCellCentered
```

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/time_domain/sources.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/sources.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/time_domain/survey.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/survey.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/utils/__init__.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/utils/current_utils.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/utils/current_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/utils/em1d_utils.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/utils/em1d_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/utils/testing_utils.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/utils/testing_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/utils/waveform_utils.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/utils/waveform_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/viscous_remanent_magnetization/__init__.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/viscous_remanent_magnetization/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/viscous_remanent_magnetization/receivers.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/viscous_remanent_magnetization/receivers.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/viscous_remanent_magnetization/simulation.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/viscous_remanent_magnetization/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/viscous_remanent_magnetization/sources.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/viscous_remanent_magnetization/sources.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/viscous_remanent_magnetization/survey.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/viscous_remanent_magnetization/survey.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/electromagnetics/viscous_remanent_magnetization/waveforms.py` & `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/viscous_remanent_magnetization/waveforms.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/fields.py` & `mira_simpeg-0.19.0.dev8/SimPEG/fields.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/flow/richards/__init__.py` & `mira_simpeg-0.19.0.dev8/SimPEG/flow/richards/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/flow/richards/empirical.py` & `mira_simpeg-0.19.0.dev8/SimPEG/flow/richards/empirical.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/flow/richards/receivers.py` & `mira_simpeg-0.19.0.dev8/SimPEG/flow/richards/receivers.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/flow/richards/survey.py` & `mira_simpeg-0.19.0.dev8/SimPEG/flow/richards/survey.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/inverse_problem.py` & `mira_simpeg-0.19.0.dev8/SimPEG/inverse_problem.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/inversion.py` & `mira_simpeg-0.19.0.dev8/SimPEG/inversion.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/maps.py` & `mira_simpeg-0.19.0.dev8/SimPEG/maps.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/meta/__init__.py` & `mira_simpeg-0.19.0.dev8/SimPEG/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/meta/simulation.py` & `mira_simpeg-0.19.0.dev8/SimPEG/meta/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/models.py` & `mira_simpeg-0.19.0.dev8/SimPEG/models.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/objective_function.py` & `mira_simpeg-0.19.0.dev8/SimPEG/objective_function.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/optimization.py` & `mira_simpeg-0.19.0.dev8/SimPEG/optimization.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/__init__.py` & `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/base.py` & `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/base.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/gravity/__init__.py` & `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/gravity/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/gravity/analytics.py` & `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/gravity/analytics.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/gravity/receivers.py` & `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/gravity/receivers.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/gravity/simulation.py` & `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/gravity/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/gravity/survey.py` & `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/gravity/survey.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/magnetics/__init__.py` & `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/magnetics/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/magnetics/analytics.py` & `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/magnetics/analytics.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/magnetics/receivers.py` & `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/magnetics/receivers.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/magnetics/simulation.py` & `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/magnetics/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/magnetics/sources.py` & `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/magnetics/sources.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/potential_fields/magnetics/survey.py` & `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/magnetics/survey.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/props.py` & `mira_simpeg-0.19.0.dev8/SimPEG/props.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/regularization/__init__.py` & `mira_simpeg-0.19.0.dev8/SimPEG/regularization/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/regularization/base.py` & `mira_simpeg-0.19.0.dev8/SimPEG/regularization/base.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/regularization/correspondence.py` & `mira_simpeg-0.19.0.dev8/SimPEG/regularization/correspondence.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/regularization/cross_gradient.py` & `mira_simpeg-0.19.0.dev8/SimPEG/regularization/cross_gradient.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/regularization/jtv.py` & `mira_simpeg-0.19.0.dev8/SimPEG/regularization/jtv.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/regularization/pgi.py` & `mira_simpeg-0.19.0.dev8/SimPEG/regularization/pgi.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/regularization/regularization_mesh.py` & `mira_simpeg-0.19.0.dev8/SimPEG/regularization/regularization_mesh.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/regularization/sparse.py` & `mira_simpeg-0.19.0.dev8/SimPEG/regularization/sparse.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/seismic/straight_ray_tomography/__init__.py` & `mira_simpeg-0.19.0.dev8/SimPEG/seismic/straight_ray_tomography/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/seismic/straight_ray_tomography/simulation.py` & `mira_simpeg-0.19.0.dev8/SimPEG/seismic/straight_ray_tomography/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/seismic/straight_ray_tomography/survey.py` & `mira_simpeg-0.19.0.dev8/SimPEG/seismic/straight_ray_tomography/survey.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/simulation.py` & `mira_simpeg-0.19.0.dev8/SimPEG/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/survey.py` & `mira_simpeg-0.19.0.dev8/SimPEG/survey.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/utils/__init__.py` & `mira_simpeg-0.19.0.dev8/SimPEG/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/utils/code_utils.py` & `mira_simpeg-0.19.0.dev8/SimPEG/utils/code_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/utils/coord_utils.py` & `mira_simpeg-0.19.0.dev8/SimPEG/utils/coord_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/utils/counter_utils.py` & `mira_simpeg-0.19.0.dev8/SimPEG/utils/counter_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/utils/curv_utils.py` & `mira_simpeg-0.19.0.dev8/SimPEG/utils/curv_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/utils/drivers/gravity_driver.py` & `mira_simpeg-0.19.0.dev8/SimPEG/utils/drivers/gravity_driver.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/utils/drivers/magnetics_driver.py` & `mira_simpeg-0.19.0.dev8/SimPEG/utils/drivers/magnetics_driver.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/utils/io_utils/__init__.py` & `mira_simpeg-0.19.0.dev8/SimPEG/utils/io_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/utils/io_utils/io_utils_electromagnetics.py` & `mira_simpeg-0.19.0.dev8/SimPEG/utils/io_utils/io_utils_electromagnetics.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/utils/io_utils/io_utils_general.py` & `mira_simpeg-0.19.0.dev8/SimPEG/utils/io_utils/io_utils_general.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/utils/io_utils/io_utils_pf.py` & `mira_simpeg-0.19.0.dev8/SimPEG/utils/io_utils/io_utils_pf.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/utils/mat_utils.py` & `mira_simpeg-0.19.0.dev8/SimPEG/utils/mat_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/utils/mesh_utils.py` & `mira_simpeg-0.19.0.dev8/SimPEG/utils/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/utils/model_builder.py` & `mira_simpeg-0.19.0.dev8/SimPEG/utils/model_builder.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/utils/model_utils.py` & `mira_simpeg-0.19.0.dev8/SimPEG/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/utils/pgi_utils.py` & `mira_simpeg-0.19.0.dev8/SimPEG/utils/pgi_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/utils/plot_utils.py` & `mira_simpeg-0.19.0.dev8/SimPEG/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/SimPEG/utils/solver_utils.py` & `mira_simpeg-0.19.0.dev8/SimPEG/utils/solver_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev7/PKG-INFO` & `mira_simpeg-0.19.0.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mira-SimPEG
-Version: 0.19.0.dev7
+Version: 0.19.0.dev8
 Summary: Mira Geoscience fork of SimPEG: Simulation and Parameter Estimation in Geophysics
 Home-page: http://simpeg.xyz/
 License: MIT
 Keywords: geophysics inverse problem
 Author: Rowan Cockett
 Author-email: rowanc1@gmail.com
 Classifier: Development Status :: 4 - Beta
```


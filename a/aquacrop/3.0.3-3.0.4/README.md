# Comparing `tmp/aquacrop-3.0.3.tar.gz` & `tmp/aquacrop-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aquacrop-3.0.3.tar", last modified: Mon Apr 22 07:45:33 2024, max compression
+gzip compressed data, was "aquacrop-3.0.4.tar", last modified: Thu Apr 25 09:11:05 2024, max compression
```

## Comparing `aquacrop-3.0.3.tar` & `aquacrop-3.0.4.tar`

### file list

```diff
@@ -1,156 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:45:33.972730 aquacrop-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-22 07:44:15.000000 aquacrop-3.0.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-22 07:44:15.000000 aquacrop-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-22 07:44:15.000000 aquacrop-3.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-04-22 07:45:33.972730 aquacrop-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-22 07:44:15.000000 aquacrop-3.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:45:33.936730 aquacrop-3.0.3/aquacrop/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16549 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:45:33.956730 aquacrop-3.0.3/aquacrop/data/
--rw-r--r--   0 runner    (1001) docker     (127)   426881 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/CP.dat
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/CP.st
--rw-r--r--   0 runner    (1001) docker     (127)   987475 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/CP_EC-EARTH[CP,RCP45,2021-2040]WG.dat
--rw-r--r--   0 runner    (1001) docker     (127)   986768 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/CP_EC-EARTH[CP,RCP45,2041-2060]WG.dat
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/CP_EC-EARTH[CP,RCP45,2041-2060]WG.st
--rw-r--r--   0 runner    (1001) docker     (127)   986731 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/CP_EC-EARTH[CP,RCP45,2061-2080]WG.dat
--rw-r--r--   0 runner    (1001) docker     (127)   987315 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/CP_EC-EARTH[CP,RCP85,2021-2040]WG.dat
--rw-r--r--   0 runner    (1001) docker     (127)   986714 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/CP_EC-EARTH[CP,RCP85,2041-2060]WG.dat
--rw-r--r--   0 runner    (1001) docker     (127)   986454 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/CP_EC-EARTH[CP,RCP85,2061-2080]WG.dat
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/MaunaLoaCO2.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   298004 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/brussels_climate.txt
--rw-r--r--   0 runner    (1001) docker     (127)   364555 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/brussels_future.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1229865 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/champion_climate.txt
--rw-r--r--   0 runner    (1001) docker     (127)   509978 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/cordoba_climate.txt
--rw-r--r--   0 runner    (1001) docker     (127)   112533 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/hyderabad_climate.txt
--rw-r--r--   0 runner    (1001) docker     (127)   513605 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/lincolnshire_climate.txt
--rw-r--r--   0 runner    (1001) docker     (127)   513550 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/norfolk_climate.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/paddyrice_hyderabad_matlab.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/paddyrice_hyderabad_windows.OUT
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/potato_matlab.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/potato_windows.OUT
--rw-r--r--   0 runner    (1001) docker     (127)   514134 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/suffolk_climate.txt
--rw-r--r--   0 runner    (1001) docker     (127)   236759 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/tunis_climate.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/tunis_test_1_SandyLoam_matlab.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/tunis_test_1_SandyLoam_windows.OUT
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/tunis_test_1_matlab.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/tunis_test_1_windows.OUT
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/tunis_test_2_long_matlab.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/tunis_test_2_long_windows.OUT
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/tunis_test_3_30taw_matlab.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8550 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/tunis_test_3_30taw_windows.OUT
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/tunis_test_6_matlab.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/tunis_test_6_windows.OUT
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/tunis_wheat_gw15_matlab.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8579 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/data/tunis_wheat_gw15_windows.OUT
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:45:33.960730 aquacrop-3.0.3/aquacrop/entities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/entities/clockStruct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/entities/co2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16950 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/entities/crop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:45:33.960730 aquacrop-3.0.3/aquacrop/entities/crops/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/entities/crops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49082 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/entities/crops/crop_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/entities/fieldManagement.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/entities/groundWater.py
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/entities/initParamVariables.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/entities/inititalWaterContent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/entities/irrigationManagement.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/entities/modelConstants.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/entities/moistureDepletion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/entities/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/entities/paramStruct.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/entities/rootZoneWaterContent.py
--rw-r--r--   0 runner    (1001) docker     (127)    17959 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/entities/soil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/entities/soilProfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/entities/temperatureStressCoefficients.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/entities/totalAvailableWater.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/entities/waterEvaporation.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/entities/waterStressCoefficients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:45:33.964730 aquacrop-3.0.3/aquacrop/initialize/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/initialize/calculate_HIGC.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/initialize/calculate_HI_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/initialize/compute_crop_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/initialize/compute_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/initialize/create_soil_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/initialize/read_clocks_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/initialize/read_field_managment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/initialize/read_groundwater_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/initialize/read_irrigation_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    11505 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/initialize/read_model_initial_conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/initialize/read_model_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/initialize/read_weather_inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:45:33.964730 aquacrop-3.0.3/aquacrop/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/scripts/checkIfPackageIsCompiled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/scripts/initiate_library.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      928 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/scripts/initiate_library.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:45:33.968730 aquacrop-3.0.3/aquacrop/solution/
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/HIadj_pollination.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/HIadj_post_anthesis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/HIadj_pre_anthesis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/HIref_current_day.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/adjust_CCx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/aeration_stress.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/biomass_accumulation.py
--rw-r--r--   0 runner    (1001) docker     (127)    19914 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/canopy_cover.py
--rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/capillary_rise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/cc_development.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/cc_required_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/check_groundwater_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    12956 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/drainage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/evap_layer_water_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/germination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/groundwater_inflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/growing_degree_day.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/growth_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8998 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/harvest_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/infiltration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/irrigation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/pre_irrigation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/rainfall_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/root_development.py
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/root_zone_water.py
--rw-r--r--   0 runner    (1001) docker     (127)    18445 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/soil_evaporation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/temperature_stress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/test.py
--rw-r--r--   0 runner    (1001) docker     (127)    21533 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/transpiration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/update_CCx_CDC.py
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/solution/water_stress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:45:33.968730 aquacrop-3.0.3/aquacrop/timestep/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/timestep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/timestep/check_if_model_is_finished.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/timestep/outputs_when_model_is_finished.py
--rw-r--r--   0 runner    (1001) docker     (127)     9687 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/timestep/reset_initial_conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16098 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/timestep/run_single_timestep.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/timestep/update_time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:45:33.972730 aquacrop-3.0.3/aquacrop/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/utils/lars.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-22 07:44:15.000000 aquacrop-3.0.3/aquacrop/utils/prepare_weather.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:45:33.972730 aquacrop-3.0.3/aquacrop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-04-22 07:45:33.000000 aquacrop-3.0.3/aquacrop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-22 07:45:33.000000 aquacrop-3.0.3/aquacrop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 07:45:33.000000 aquacrop-3.0.3/aquacrop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-22 07:45:33.000000 aquacrop-3.0.3/aquacrop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-22 07:45:33.000000 aquacrop-3.0.3/aquacrop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-22 07:44:15.000000 aquacrop-3.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-22 07:45:33.972730 aquacrop-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-22 07:44:15.000000 aquacrop-3.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:45:33.972730 aquacrop-3.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-22 07:44:15.000000 aquacrop-3.0.3/tests/test_bug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-22 07:44:15.000000 aquacrop-3.0.3/tests/test_co2_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-22 07:44:15.000000 aquacrop-3.0.3/tests/test_groundwater_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-04-22 07:44:15.000000 aquacrop-3.0.3/tests/test_irrigation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-22 07:44:15.000000 aquacrop-3.0.3/tests/test_model_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-22 07:44:15.000000 aquacrop-3.0.3/tests/test_model_not_running.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-22 07:44:15.000000 aquacrop-3.0.3/tests/test_model_step_finished.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-22 07:44:15.000000 aquacrop-3.0.3/tests/test_model_step_less_than_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-22 07:44:15.000000 aquacrop-3.0.3/tests/test_model_step_not_finished.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-22 07:44:15.000000 aquacrop-3.0.3/tests/test_model_till_termination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-22 07:44:15.000000 aquacrop-3.0.3/tests/test_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-22 07:44:15.000000 aquacrop-3.0.3/tests/test_v7.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:05.345435 aquacrop-3.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-25 09:09:55.000000 aquacrop-3.0.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 09:09:55.000000 aquacrop-3.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-25 09:09:55.000000 aquacrop-3.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-04-25 09:11:05.345435 aquacrop-3.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-25 09:09:55.000000 aquacrop-3.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:05.301435 aquacrop-3.0.4/aquacrop/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-25 09:09:55.000000 aquacrop-3.0.4/aquacrop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16549 2024-04-25 09:09:55.000000 aquacrop-3.0.4/aquacrop/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:05.325435 aquacrop-3.0.4/aquacrop/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   426881 2024-04-25 09:09:55.000000 aquacrop-3.0.4/aquacrop/data/CP.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-25 09:09:55.000000 aquacrop-3.0.4/aquacrop/data/CP.st
+-rw-r--r--   0 runner    (1001) docker     (127)   987475 2024-04-25 09:09:55.000000 aquacrop-3.0.4/aquacrop/data/CP_EC-EARTH[CP,RCP45,2021-2040]WG.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   986768 2024-04-25 09:09:55.000000 aquacrop-3.0.4/aquacrop/data/CP_EC-EARTH[CP,RCP45,2041-2060]WG.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-25 09:09:55.000000 aquacrop-3.0.4/aquacrop/data/CP_EC-EARTH[CP,RCP45,2041-2060]WG.st
+-rw-r--r--   0 runner    (1001) docker     (127)   986731 2024-04-25 09:09:55.000000 aquacrop-3.0.4/aquacrop/data/CP_EC-EARTH[CP,RCP45,2061-2080]WG.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   987315 2024-04-25 09:09:55.000000 aquacrop-3.0.4/aquacrop/data/CP_EC-EARTH[CP,RCP85,2021-2040]WG.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   986714 2024-04-25 09:09:55.000000 aquacrop-3.0.4/aquacrop/data/CP_EC-EARTH[CP,RCP85,2041-2060]WG.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   986454 2024-04-25 09:09:55.000000 aquacrop-3.0.4/aquacrop/data/CP_EC-EARTH[CP,RCP85,2061-2080]WG.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-25 09:09:55.000000 aquacrop-3.0.4/aquacrop/data/MaunaLoaCO2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 09:09:55.000000 aquacrop-3.0.4/aquacrop/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   298004 2024-04-25 09:09:55.000000 aquacrop-3.0.4/aquacrop/data/brussels_climate.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   364555 2024-04-25 09:09:55.000000 aquacrop-3.0.4/aquacrop/data/brussels_future.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   513536 2024-04-25 09:09:55.000000 aquacrop-3.0.4/aquacrop/data/cambridge_climate.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1229865 2024-04-25 09:09:55.000000 aquacrop-3.0.4/aquacrop/data/champion_climate.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   509978 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/data/cordoba_climate.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   112533 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/data/hyderabad_climate.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   513605 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/data/lincolnshire_climate.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   513550 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/data/norfolk_climate.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   512956 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/data/north_yorks_climate.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   512725 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/data/northumberland_climate.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/data/paddyrice_hyderabad_matlab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/data/paddyrice_hyderabad_windows.OUT
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/data/potato_matlab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/data/potato_windows.OUT
+-rw-r--r--   0 runner    (1001) docker     (127)   514134 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/data/suffolk_climate.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   236759 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/data/tunis_climate.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/data/tunis_test_1_SandyLoam_matlab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/data/tunis_test_1_SandyLoam_windows.OUT
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/data/tunis_test_1_matlab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/data/tunis_test_1_windows.OUT
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/data/tunis_test_2_long_matlab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/data/tunis_test_2_long_windows.OUT
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/data/tunis_test_3_30taw_matlab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8550 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/data/tunis_test_3_30taw_windows.OUT
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/data/tunis_test_6_matlab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/data/tunis_test_6_windows.OUT
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/data/tunis_wheat_gw15_matlab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8579 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/data/tunis_wheat_gw15_windows.OUT
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:05.329435 aquacrop-3.0.4/aquacrop/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/entities/clockStruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/entities/co2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16950 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/entities/crop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:05.329435 aquacrop-3.0.4/aquacrop/entities/crops/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/entities/crops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49082 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/entities/crops/crop_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/entities/fieldManagement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/entities/groundWater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/entities/initParamVariables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/entities/inititalWaterContent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/entities/irrigationManagement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/entities/modelConstants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/entities/moistureDepletion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/entities/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/entities/paramStruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/entities/rootZoneWaterContent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17959 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/entities/soil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/entities/soilProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/entities/temperatureStressCoefficients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/entities/totalAvailableWater.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/entities/waterEvaporation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/entities/waterStressCoefficients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:05.333435 aquacrop-3.0.4/aquacrop/initialize/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/initialize/calculate_HIGC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/initialize/calculate_HI_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/initialize/compute_crop_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/initialize/compute_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/initialize/create_soil_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/initialize/read_clocks_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/initialize/read_field_managment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/initialize/read_groundwater_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/initialize/read_irrigation_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11505 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/initialize/read_model_initial_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/initialize/read_model_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/initialize/read_weather_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:05.333435 aquacrop-3.0.4/aquacrop/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/scripts/checkIfPackageIsCompiled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/scripts/initiate_library.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      928 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/scripts/initiate_library.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:05.341435 aquacrop-3.0.4/aquacrop/solution/
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/HIadj_pollination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/HIadj_post_anthesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/HIadj_pre_anthesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/HIref_current_day.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/adjust_CCx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/aeration_stress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/biomass_accumulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19914 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/canopy_cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/capillary_rise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/cc_development.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/cc_required_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/check_groundwater_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12956 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/drainage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/evap_layer_water_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/germination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/groundwater_inflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/growing_degree_day.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/growth_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8998 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/harvest_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/infiltration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/irrigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/pre_irrigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/rainfall_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/root_development.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/root_zone_water.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18445 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/soil_evaporation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/temperature_stress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21533 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/transpiration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/update_CCx_CDC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/solution/water_stress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:05.341435 aquacrop-3.0.4/aquacrop/timestep/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/timestep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/timestep/check_if_model_is_finished.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/timestep/outputs_when_model_is_finished.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9687 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/timestep/reset_initial_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16098 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/timestep/run_single_timestep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/timestep/update_time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:05.341435 aquacrop-3.0.4/aquacrop/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/utils/lars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-25 09:09:56.000000 aquacrop-3.0.4/aquacrop/utils/prepare_weather.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:05.341435 aquacrop-3.0.4/aquacrop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-04-25 09:11:05.000000 aquacrop-3.0.4/aquacrop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-25 09:11:05.000000 aquacrop-3.0.4/aquacrop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:11:05.000000 aquacrop-3.0.4/aquacrop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-25 09:11:05.000000 aquacrop-3.0.4/aquacrop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 09:11:05.000000 aquacrop-3.0.4/aquacrop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-25 09:09:56.000000 aquacrop-3.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-25 09:11:05.345435 aquacrop-3.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 09:09:56.000000 aquacrop-3.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:05.341435 aquacrop-3.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-25 09:09:56.000000 aquacrop-3.0.4/tests/test_bug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-25 09:09:56.000000 aquacrop-3.0.4/tests/test_co2_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-25 09:09:56.000000 aquacrop-3.0.4/tests/test_groundwater_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-04-25 09:09:56.000000 aquacrop-3.0.4/tests/test_irrigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-25 09:09:56.000000 aquacrop-3.0.4/tests/test_model_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-25 09:09:56.000000 aquacrop-3.0.4/tests/test_model_not_running.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-25 09:09:56.000000 aquacrop-3.0.4/tests/test_model_step_finished.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-25 09:09:56.000000 aquacrop-3.0.4/tests/test_model_step_less_than_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-25 09:09:56.000000 aquacrop-3.0.4/tests/test_model_step_not_finished.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-25 09:09:56.000000 aquacrop-3.0.4/tests/test_model_till_termination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-25 09:09:56.000000 aquacrop-3.0.4/tests/test_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-25 09:09:56.000000 aquacrop-3.0.4/tests/test_v7.py
```

### Comparing `aquacrop-3.0.3/CONTRIBUTING.md` & `aquacrop-3.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/LICENSE` & `aquacrop-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/PKG-INFO` & `aquacrop-3.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquacrop
-Version: 3.0.3
+Version: 3.0.4
 Summary: Soil-Crop-Water model based on AquaCrop-OS.
 Home-page: https://github.com/aquacropos/aquacrop
 Author: Tim Foster
 Author-email: timothy.foster@manchester.ac.uk
 Project-URL: Bug Tracker, https://github.com/aquacropos/aquacrop/issues
 Keywords: aquacrop,aquacropos,aquacrop-ospy,python
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aquacrop Version: 3.0.3 Summary: Soil-Crop-Water
+Metadata-Version: 2.1 Name: aquacrop Version: 3.0.4 Summary: Soil-Crop-Water
 model based on AquaCrop-OS. Home-page: https://github.com/aquacropos/aquacrop
 Author: Tim Foster Author-email: timothy.foster@manchester.ac.uk Project-URL:
 Bug Tracker, https://github.com/aquacropos/aquacrop/issues Keywords:
 aquacrop,aquacropos,aquacrop-ospy,python Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: License :: OSI Approved :: MIT License Classifier:
```

### Comparing `aquacrop-3.0.3/README.md` & `aquacrop-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/core.py` & `aquacrop-3.0.4/aquacrop/core.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/CP.dat` & `aquacrop-3.0.4/aquacrop/data/CP.dat`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/CP_EC-EARTH[CP,RCP45,2021-2040]WG.dat` & `aquacrop-3.0.4/aquacrop/data/CP_EC-EARTH[CP,RCP45,2021-2040]WG.dat`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/CP_EC-EARTH[CP,RCP45,2041-2060]WG.dat` & `aquacrop-3.0.4/aquacrop/data/CP_EC-EARTH[CP,RCP45,2041-2060]WG.dat`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/CP_EC-EARTH[CP,RCP45,2061-2080]WG.dat` & `aquacrop-3.0.4/aquacrop/data/CP_EC-EARTH[CP,RCP45,2061-2080]WG.dat`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/CP_EC-EARTH[CP,RCP85,2021-2040]WG.dat` & `aquacrop-3.0.4/aquacrop/data/CP_EC-EARTH[CP,RCP85,2021-2040]WG.dat`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/CP_EC-EARTH[CP,RCP85,2041-2060]WG.dat` & `aquacrop-3.0.4/aquacrop/data/CP_EC-EARTH[CP,RCP85,2041-2060]WG.dat`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/CP_EC-EARTH[CP,RCP85,2061-2080]WG.dat` & `aquacrop-3.0.4/aquacrop/data/CP_EC-EARTH[CP,RCP85,2061-2080]WG.dat`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/MaunaLoaCO2.txt` & `aquacrop-3.0.4/aquacrop/data/MaunaLoaCO2.txt`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/brussels_climate.txt` & `aquacrop-3.0.4/aquacrop/data/brussels_climate.txt`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/brussels_future.txt` & `aquacrop-3.0.4/aquacrop/data/brussels_future.txt`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/champion_climate.txt` & `aquacrop-3.0.4/aquacrop/data/champion_climate.txt`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/cordoba_climate.txt` & `aquacrop-3.0.4/aquacrop/data/cordoba_climate.txt`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/hyderabad_climate.txt` & `aquacrop-3.0.4/aquacrop/data/hyderabad_climate.txt`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/lincolnshire_climate.txt` & `aquacrop-3.0.4/aquacrop/data/lincolnshire_climate.txt`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/norfolk_climate.txt` & `aquacrop-3.0.4/aquacrop/data/norfolk_climate.txt`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/paddyrice_hyderabad_matlab.txt` & `aquacrop-3.0.4/aquacrop/data/paddyrice_hyderabad_matlab.txt`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/paddyrice_hyderabad_windows.OUT` & `aquacrop-3.0.4/aquacrop/data/paddyrice_hyderabad_windows.OUT`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/potato_matlab.txt` & `aquacrop-3.0.4/aquacrop/data/potato_matlab.txt`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/potato_windows.OUT` & `aquacrop-3.0.4/aquacrop/data/potato_windows.OUT`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/suffolk_climate.txt` & `aquacrop-3.0.4/aquacrop/data/suffolk_climate.txt`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/tunis_climate.txt` & `aquacrop-3.0.4/aquacrop/data/tunis_climate.txt`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/tunis_test_1_SandyLoam_matlab.txt` & `aquacrop-3.0.4/aquacrop/data/tunis_test_1_SandyLoam_matlab.txt`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/tunis_test_1_SandyLoam_windows.OUT` & `aquacrop-3.0.4/aquacrop/data/tunis_test_1_SandyLoam_windows.OUT`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/tunis_test_1_matlab.txt` & `aquacrop-3.0.4/aquacrop/data/tunis_test_1_matlab.txt`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/tunis_test_1_windows.OUT` & `aquacrop-3.0.4/aquacrop/data/tunis_test_1_windows.OUT`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/tunis_test_2_long_matlab.txt` & `aquacrop-3.0.4/aquacrop/data/tunis_test_2_long_matlab.txt`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/tunis_test_2_long_windows.OUT` & `aquacrop-3.0.4/aquacrop/data/tunis_test_2_long_windows.OUT`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/tunis_test_3_30taw_matlab.txt` & `aquacrop-3.0.4/aquacrop/data/tunis_test_3_30taw_matlab.txt`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/tunis_test_3_30taw_windows.OUT` & `aquacrop-3.0.4/aquacrop/data/tunis_test_3_30taw_windows.OUT`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/tunis_test_6_matlab.txt` & `aquacrop-3.0.4/aquacrop/data/tunis_test_6_matlab.txt`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/tunis_test_6_windows.OUT` & `aquacrop-3.0.4/aquacrop/data/tunis_test_6_windows.OUT`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/tunis_wheat_gw15_matlab.txt` & `aquacrop-3.0.4/aquacrop/data/tunis_wheat_gw15_matlab.txt`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/data/tunis_wheat_gw15_windows.OUT` & `aquacrop-3.0.4/aquacrop/data/tunis_wheat_gw15_windows.OUT`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/entities/clockStruct.py` & `aquacrop-3.0.4/aquacrop/entities/clockStruct.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/entities/co2.py` & `aquacrop-3.0.4/aquacrop/entities/co2.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/entities/crop.py` & `aquacrop-3.0.4/aquacrop/entities/crop.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/entities/crops/crop_params.py` & `aquacrop-3.0.4/aquacrop/entities/crops/crop_params.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/entities/fieldManagement.py` & `aquacrop-3.0.4/aquacrop/entities/fieldManagement.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/entities/groundWater.py` & `aquacrop-3.0.4/aquacrop/entities/groundWater.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/entities/initParamVariables.py` & `aquacrop-3.0.4/aquacrop/entities/initParamVariables.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/entities/inititalWaterContent.py` & `aquacrop-3.0.4/aquacrop/entities/inititalWaterContent.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/entities/irrigationManagement.py` & `aquacrop-3.0.4/aquacrop/entities/irrigationManagement.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/entities/output.py` & `aquacrop-3.0.4/aquacrop/entities/output.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/entities/paramStruct.py` & `aquacrop-3.0.4/aquacrop/entities/paramStruct.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/entities/rootZoneWaterContent.py` & `aquacrop-3.0.4/aquacrop/entities/rootZoneWaterContent.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/entities/soil.py` & `aquacrop-3.0.4/aquacrop/entities/soil.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/entities/soilProfile.py` & `aquacrop-3.0.4/aquacrop/entities/soilProfile.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/entities/temperatureStressCoefficients.py` & `aquacrop-3.0.4/aquacrop/entities/temperatureStressCoefficients.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/entities/waterEvaporation.py` & `aquacrop-3.0.4/aquacrop/entities/waterEvaporation.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/entities/waterStressCoefficients.py` & `aquacrop-3.0.4/aquacrop/entities/waterStressCoefficients.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/initialize/calculate_HIGC.py` & `aquacrop-3.0.4/aquacrop/initialize/calculate_HIGC.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/initialize/calculate_HI_linear.py` & `aquacrop-3.0.4/aquacrop/initialize/calculate_HI_linear.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/initialize/compute_crop_calendar.py` & `aquacrop-3.0.4/aquacrop/initialize/compute_crop_calendar.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/initialize/compute_variables.py` & `aquacrop-3.0.4/aquacrop/initialize/compute_variables.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/initialize/create_soil_profile.py` & `aquacrop-3.0.4/aquacrop/initialize/create_soil_profile.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/initialize/read_clocks_parameters.py` & `aquacrop-3.0.4/aquacrop/initialize/read_clocks_parameters.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/initialize/read_field_managment.py` & `aquacrop-3.0.4/aquacrop/initialize/read_field_managment.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/initialize/read_groundwater_table.py` & `aquacrop-3.0.4/aquacrop/initialize/read_groundwater_table.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/initialize/read_irrigation_management.py` & `aquacrop-3.0.4/aquacrop/initialize/read_irrigation_management.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/initialize/read_model_initial_conditions.py` & `aquacrop-3.0.4/aquacrop/initialize/read_model_initial_conditions.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/initialize/read_model_parameters.py` & `aquacrop-3.0.4/aquacrop/initialize/read_model_parameters.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/initialize/read_weather_inputs.py` & `aquacrop-3.0.4/aquacrop/initialize/read_weather_inputs.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/scripts/checkIfPackageIsCompiled.py` & `aquacrop-3.0.4/aquacrop/scripts/checkIfPackageIsCompiled.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/scripts/initiate_library.py` & `aquacrop-3.0.4/aquacrop/scripts/initiate_library.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/scripts/initiate_library.sh` & `aquacrop-3.0.4/aquacrop/scripts/initiate_library.sh`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/HIadj_pollination.py` & `aquacrop-3.0.4/aquacrop/solution/HIadj_pollination.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/HIadj_post_anthesis.py` & `aquacrop-3.0.4/aquacrop/solution/HIadj_post_anthesis.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/HIadj_pre_anthesis.py` & `aquacrop-3.0.4/aquacrop/solution/HIadj_pre_anthesis.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/HIref_current_day.py` & `aquacrop-3.0.4/aquacrop/solution/HIref_current_day.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/adjust_CCx.py` & `aquacrop-3.0.4/aquacrop/solution/adjust_CCx.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/aeration_stress.py` & `aquacrop-3.0.4/aquacrop/solution/aeration_stress.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/biomass_accumulation.py` & `aquacrop-3.0.4/aquacrop/solution/biomass_accumulation.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/canopy_cover.py` & `aquacrop-3.0.4/aquacrop/solution/canopy_cover.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/capillary_rise.py` & `aquacrop-3.0.4/aquacrop/solution/capillary_rise.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/cc_development.py` & `aquacrop-3.0.4/aquacrop/solution/cc_development.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/cc_required_time.py` & `aquacrop-3.0.4/aquacrop/solution/cc_required_time.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/check_groundwater_table.py` & `aquacrop-3.0.4/aquacrop/solution/check_groundwater_table.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/drainage.py` & `aquacrop-3.0.4/aquacrop/solution/drainage.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/evap_layer_water_content.py` & `aquacrop-3.0.4/aquacrop/solution/evap_layer_water_content.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/germination.py` & `aquacrop-3.0.4/aquacrop/solution/germination.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/groundwater_inflow.py` & `aquacrop-3.0.4/aquacrop/solution/groundwater_inflow.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/growing_degree_day.py` & `aquacrop-3.0.4/aquacrop/solution/growing_degree_day.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/growth_stage.py` & `aquacrop-3.0.4/aquacrop/solution/growth_stage.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/harvest_index.py` & `aquacrop-3.0.4/aquacrop/solution/harvest_index.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/infiltration.py` & `aquacrop-3.0.4/aquacrop/solution/infiltration.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/irrigation.py` & `aquacrop-3.0.4/aquacrop/solution/irrigation.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/pre_irrigation.py` & `aquacrop-3.0.4/aquacrop/solution/pre_irrigation.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/rainfall_partition.py` & `aquacrop-3.0.4/aquacrop/solution/rainfall_partition.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/root_development.py` & `aquacrop-3.0.4/aquacrop/solution/root_development.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/root_zone_water.py` & `aquacrop-3.0.4/aquacrop/solution/root_zone_water.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/soil_evaporation.py` & `aquacrop-3.0.4/aquacrop/solution/soil_evaporation.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/temperature_stress.py` & `aquacrop-3.0.4/aquacrop/solution/temperature_stress.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/transpiration.py` & `aquacrop-3.0.4/aquacrop/solution/transpiration.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/update_CCx_CDC.py` & `aquacrop-3.0.4/aquacrop/solution/update_CCx_CDC.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/solution/water_stress.py` & `aquacrop-3.0.4/aquacrop/solution/water_stress.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/timestep/check_if_model_is_finished.py` & `aquacrop-3.0.4/aquacrop/timestep/check_if_model_is_finished.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/timestep/outputs_when_model_is_finished.py` & `aquacrop-3.0.4/aquacrop/timestep/outputs_when_model_is_finished.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/timestep/reset_initial_conditions.py` & `aquacrop-3.0.4/aquacrop/timestep/reset_initial_conditions.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/timestep/run_single_timestep.py` & `aquacrop-3.0.4/aquacrop/timestep/run_single_timestep.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/timestep/update_time.py` & `aquacrop-3.0.4/aquacrop/timestep/update_time.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/utils/lars.py` & `aquacrop-3.0.4/aquacrop/utils/lars.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop/utils/prepare_weather.py` & `aquacrop-3.0.4/aquacrop/utils/prepare_weather.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/aquacrop.egg-info/PKG-INFO` & `aquacrop-3.0.4/aquacrop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquacrop
-Version: 3.0.3
+Version: 3.0.4
 Summary: Soil-Crop-Water model based on AquaCrop-OS.
 Home-page: https://github.com/aquacropos/aquacrop
 Author: Tim Foster
 Author-email: timothy.foster@manchester.ac.uk
 Project-URL: Bug Tracker, https://github.com/aquacropos/aquacrop/issues
 Keywords: aquacrop,aquacropos,aquacrop-ospy,python
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aquacrop Version: 3.0.3 Summary: Soil-Crop-Water
+Metadata-Version: 2.1 Name: aquacrop Version: 3.0.4 Summary: Soil-Crop-Water
 model based on AquaCrop-OS. Home-page: https://github.com/aquacropos/aquacrop
 Author: Tim Foster Author-email: timothy.foster@manchester.ac.uk Project-URL:
 Bug Tracker, https://github.com/aquacropos/aquacrop/issues Keywords:
 aquacrop,aquacropos,aquacrop-ospy,python Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: License :: OSI Approved :: MIT License Classifier:
```

### Comparing `aquacrop-3.0.3/aquacrop.egg-info/SOURCES.txt` & `aquacrop-3.0.4/aquacrop.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,22 @@
 aquacrop/data/CP_EC-EARTH[CP,RCP85,2021-2040]WG.dat
 aquacrop/data/CP_EC-EARTH[CP,RCP85,2041-2060]WG.dat
 aquacrop/data/CP_EC-EARTH[CP,RCP85,2061-2080]WG.dat
 aquacrop/data/MaunaLoaCO2.txt
 aquacrop/data/__init__.py
 aquacrop/data/brussels_climate.txt
 aquacrop/data/brussels_future.txt
+aquacrop/data/cambridge_climate.txt
 aquacrop/data/champion_climate.txt
 aquacrop/data/cordoba_climate.txt
 aquacrop/data/hyderabad_climate.txt
 aquacrop/data/lincolnshire_climate.txt
 aquacrop/data/norfolk_climate.txt
+aquacrop/data/north_yorks_climate.txt
+aquacrop/data/northumberland_climate.txt
 aquacrop/data/paddyrice_hyderabad_matlab.txt
 aquacrop/data/paddyrice_hyderabad_windows.OUT
 aquacrop/data/potato_matlab.txt
 aquacrop/data/potato_windows.OUT
 aquacrop/data/suffolk_climate.txt
 aquacrop/data/tunis_climate.txt
 aquacrop/data/tunis_test_1_SandyLoam_matlab.txt
```

### Comparing `aquacrop-3.0.3/setup.cfg` & `aquacrop-3.0.4/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = aquacrop
-version = 3.0.3
+version = 3.0.4
 author = Tim Foster
 author_email = timothy.foster@manchester.ac.uk
 description = Soil-Crop-Water model based on AquaCrop-OS.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = aquacrop, aquacropos, aquacrop-ospy, python
 url = https://github.com/aquacropos/aquacrop
```

### Comparing `aquacrop-3.0.3/tests/test_bug.py` & `aquacrop-3.0.4/tests/test_bug.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/tests/test_co2_timeseries.py` & `aquacrop-3.0.4/tests/test_co2_timeseries.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/tests/test_groundwater_table.py` & `aquacrop-3.0.4/tests/test_groundwater_table.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/tests/test_irrigation.py` & `aquacrop-3.0.4/tests/test_irrigation.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/tests/test_model_exceptions.py` & `aquacrop-3.0.4/tests/test_model_exceptions.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/tests/test_model_not_running.py` & `aquacrop-3.0.4/tests/test_model_not_running.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/tests/test_model_step_finished.py` & `aquacrop-3.0.4/tests/test_model_step_finished.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/tests/test_model_step_less_than_1.py` & `aquacrop-3.0.4/tests/test_model_step_less_than_1.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/tests/test_model_step_not_finished.py` & `aquacrop-3.0.4/tests/test_model_step_not_finished.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/tests/test_model_till_termination.py` & `aquacrop-3.0.4/tests/test_model_till_termination.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/tests/test_speed.py` & `aquacrop-3.0.4/tests/test_speed.py`

 * *Files identical despite different names*

### Comparing `aquacrop-3.0.3/tests/test_v7.py` & `aquacrop-3.0.4/tests/test_v7.py`

 * *Files identical despite different names*


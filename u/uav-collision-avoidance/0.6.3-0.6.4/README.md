# Comparing `tmp/uav_collision_avoidance-0.6.3-py3-none-any.whl.zip` & `tmp/uav_collision_avoidance-0.6.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,38 @@
-Zip file size: 153144 bytes, number of entries: 111
+Zip file size: 176631 bytes, number of entries: 126
+-rw-r--r--  2.0 unx      107 b- defN 24-Apr-16 08:15 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py
+-rw-r--r--  2.0 unx      121 b- defN 24-Mar-28 17:13 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py
+-rw-r--r--  2.0 unx     2203 b- defN 24-Apr-15 19:36 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py
+-rw-r--r--  2.0 unx      238 b- defN 24-Apr-22 14:13 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/version.py
+-rw-r--r--  2.0 unx     1662 b- defN 24-Mar-28 17:17 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py
+-rw-r--r--  2.0 unx     9540 b- defN 24-Apr-11 18:19 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
+-rw-r--r--  2.0 unx     4195 b- defN 24-Apr-05 07:31 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py
+-rw-r--r--  2.0 unx     8671 b- defN 24-Apr-16 07:07 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py
+-rw-r--r--  2.0 unx     6057 b- defN 24-Apr-11 11:29 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py
+-rw-r--r--  2.0 unx     1979 b- defN 24-Mar-28 17:20 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py
+-rw-r--r--  2.0 unx     7112 b- defN 24-Apr-11 19:12 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py
+-rw-r--r--  2.0 unx     1041 b- defN 24-Mar-28 17:20 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py
+-rw-r--r--  2.0 unx      682 b- defN 24-Apr-06 09:52 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py
+-rw-r--r--  2.0 unx     6110 b- defN 24-Apr-11 12:04 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
+-rw-r--r--  2.0 unx    23164 b- defN 24-Apr-11 12:26 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
 -rw-r--r--  2.0 unx      107 b- defN 24-Apr-16 08:15 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py
 -rw-r--r--  2.0 unx      121 b- defN 24-Mar-28 17:13 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py
 -rw-r--r--  2.0 unx     2203 b- defN 24-Apr-15 19:36 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py
 -rw-r--r--  2.0 unx      238 b- defN 24-Apr-22 14:13 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/version.py
 -rw-r--r--  2.0 unx     1662 b- defN 24-Mar-28 17:17 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py
--rw-r--r--  2.0 unx     9540 b- defN 24-Apr-11 18:19 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
+-rw-r--r--  2.0 unx    11332 b- defN 24-Apr-22 13:54 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
 -rw-r--r--  2.0 unx     4195 b- defN 24-Apr-05 07:31 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py
--rw-r--r--  2.0 unx     8671 b- defN 24-Apr-16 07:07 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py
--rw-r--r--  2.0 unx     6057 b- defN 24-Apr-11 11:29 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py
+-rw-r--r--  2.0 unx     9028 b- defN 24-Apr-20 15:08 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py
+-rw-r--r--  2.0 unx     7108 b- defN 24-Apr-22 12:03 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py
 -rw-r--r--  2.0 unx     1979 b- defN 24-Mar-28 17:20 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py
--rw-r--r--  2.0 unx     7112 b- defN 24-Apr-11 19:12 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py
+-rw-r--r--  2.0 unx     6613 b- defN 24-Apr-21 14:26 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py
 -rw-r--r--  2.0 unx     1041 b- defN 24-Mar-28 17:20 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py
 -rw-r--r--  2.0 unx      682 b- defN 24-Apr-06 09:52 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py
--rw-r--r--  2.0 unx     6110 b- defN 24-Apr-11 12:04 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
--rw-r--r--  2.0 unx    23164 b- defN 24-Apr-11 12:26 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
+-rw-r--r--  2.0 unx     6290 b- defN 24-Apr-20 15:07 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
+-rw-r--r--  2.0 unx    23168 b- defN 24-Apr-18 21:19 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
 -rw-r--r--  2.0 unx      107 b- defN 24-Apr-16 08:15 build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py
 -rw-r--r--  2.0 unx      121 b- defN 24-Mar-28 17:13 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py
 -rw-r--r--  2.0 unx     2203 b- defN 24-Apr-15 19:36 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py
 -rw-r--r--  2.0 unx      238 b- defN 24-Apr-22 14:13 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/version.py
 -rw-r--r--  2.0 unx     1662 b- defN 24-Mar-28 17:17 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py
 -rw-r--r--  2.0 unx    11332 b- defN 24-Apr-22 13:54 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
 -rw-r--r--  2.0 unx     4195 b- defN 24-Apr-05 07:31 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py
@@ -60,54 +75,54 @@
 -rw-r--r--  2.0 unx     6290 b- defN 24-Apr-20 15:07 build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
 -rw-r--r--  2.0 unx    23168 b- defN 24-Apr-18 21:19 build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
 -rw-r--r--  2.0 unx      107 b- defN 24-Apr-16 08:15 build/lib/build/lib/tests/test_sample.py
 -rw-r--r--  2.0 unx      121 b- defN 24-Mar-28 17:13 build/lib/build/lib/uav_collision_avoidance/__init__.py
 -rw-r--r--  2.0 unx     2203 b- defN 24-Apr-15 19:36 build/lib/build/lib/uav_collision_avoidance/main.py
 -rw-r--r--  2.0 unx      238 b- defN 24-Apr-22 14:13 build/lib/build/lib/uav_collision_avoidance/version.py
 -rw-r--r--  2.0 unx     1662 b- defN 24-Mar-28 17:17 build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py
--rw-r--r--  2.0 unx    11332 b- defN 24-Apr-22 13:54 build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
+-rw-r--r--  2.0 unx    13017 b- defN 24-Apr-24 17:23 build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
 -rw-r--r--  2.0 unx     4195 b- defN 24-Apr-05 07:31 build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py
--rw-r--r--  2.0 unx     9028 b- defN 24-Apr-20 15:08 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py
--rw-r--r--  2.0 unx     7108 b- defN 24-Apr-22 12:03 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py
+-rw-r--r--  2.0 unx     9630 b- defN 24-Apr-24 17:35 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py
+-rw-r--r--  2.0 unx     7072 b- defN 24-Apr-24 14:39 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py
 -rw-r--r--  2.0 unx     1979 b- defN 24-Mar-28 17:20 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py
--rw-r--r--  2.0 unx     6613 b- defN 24-Apr-21 14:26 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py
+-rw-r--r--  2.0 unx     6613 b- defN 24-Apr-24 14:18 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py
 -rw-r--r--  2.0 unx     1041 b- defN 24-Mar-28 17:20 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py
 -rw-r--r--  2.0 unx      682 b- defN 24-Apr-06 09:52 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py
--rw-r--r--  2.0 unx     6290 b- defN 24-Apr-20 15:07 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
--rw-r--r--  2.0 unx    23168 b- defN 24-Apr-18 21:19 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
+-rw-r--r--  2.0 unx     6290 b- defN 24-Apr-24 14:18 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
+-rw-r--r--  2.0 unx    25822 b- defN 24-Apr-24 16:52 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
 -rw-r--r--  2.0 unx      107 b- defN 24-Apr-16 08:15 build/lib/tests/test_sample.py
 -rw-r--r--  2.0 unx      121 b- defN 24-Mar-28 17:13 build/lib/uav_collision_avoidance/__init__.py
 -rw-r--r--  2.0 unx     2203 b- defN 24-Apr-15 19:36 build/lib/uav_collision_avoidance/main.py
 -rw-r--r--  2.0 unx      238 b- defN 24-Apr-22 14:13 build/lib/uav_collision_avoidance/version.py
 -rw-r--r--  2.0 unx     1662 b- defN 24-Mar-28 17:17 build/lib/uav_collision_avoidance/src/aircraft/aircraft.py
--rw-r--r--  2.0 unx    13017 b- defN 24-Apr-24 17:23 build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
+-rw-r--r--  2.0 unx    14940 b- defN 24-Apr-25 10:35 build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
 -rw-r--r--  2.0 unx     4195 b- defN 24-Apr-05 07:31 build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py
--rw-r--r--  2.0 unx     9630 b- defN 24-Apr-24 17:35 build/lib/uav_collision_avoidance/src/simulation/simulation.py
--rw-r--r--  2.0 unx     7072 b- defN 24-Apr-24 14:39 build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py
+-rw-r--r--  2.0 unx     9632 b- defN 24-Apr-25 10:25 build/lib/uav_collision_avoidance/src/simulation/simulation.py
+-rw-r--r--  2.0 unx     8427 b- defN 24-Apr-24 20:23 build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py
 -rw-r--r--  2.0 unx     1979 b- defN 24-Mar-28 17:20 build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py
--rw-r--r--  2.0 unx     6613 b- defN 24-Apr-24 14:18 build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py
+-rw-r--r--  2.0 unx     8170 b- defN 24-Apr-25 10:23 build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py
 -rw-r--r--  2.0 unx     1041 b- defN 24-Mar-28 17:20 build/lib/uav_collision_avoidance/src/simulation/simulation_render.py
 -rw-r--r--  2.0 unx      682 b- defN 24-Apr-06 09:52 build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py
--rw-r--r--  2.0 unx     6290 b- defN 24-Apr-24 14:18 build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
--rw-r--r--  2.0 unx    25822 b- defN 24-Apr-24 16:52 build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
+-rw-r--r--  2.0 unx     6343 b- defN 24-Apr-25 10:24 build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
+-rw-r--r--  2.0 unx    26085 b- defN 24-Apr-25 10:19 build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
 -rw-r--r--  2.0 unx      107 b- defN 24-Apr-16 08:15 tests/test_sample.py
 -rw-r--r--  2.0 unx      121 b- defN 24-Mar-28 17:13 uav_collision_avoidance/__init__.py
 -rw-r--r--  2.0 unx     2203 b- defN 24-Apr-15 19:36 uav_collision_avoidance/main.py
 -rw-r--r--  2.0 unx      238 b- defN 24-Apr-22 14:13 uav_collision_avoidance/version.py
 -rw-r--r--  2.0 unx     1662 b- defN 24-Mar-28 17:17 uav_collision_avoidance/src/aircraft/aircraft.py
--rw-r--r--  2.0 unx    14940 b- defN 24-Apr-25 10:35 uav_collision_avoidance/src/aircraft/aircraft_fcc.py
+-rw-r--r--  2.0 unx    15437 b- defN 24-Apr-25 10:59 uav_collision_avoidance/src/aircraft/aircraft_fcc.py
 -rw-r--r--  2.0 unx     4195 b- defN 24-Apr-05 07:31 uav_collision_avoidance/src/aircraft/aircraft_vehicle.py
--rw-r--r--  2.0 unx     9632 b- defN 24-Apr-25 10:25 uav_collision_avoidance/src/simulation/simulation.py
+-rw-r--r--  2.0 unx     9632 b- defN 24-Apr-25 11:01 uav_collision_avoidance/src/simulation/simulation.py
 -rw-r--r--  2.0 unx     8427 b- defN 24-Apr-24 20:23 uav_collision_avoidance/src/simulation/simulation_adsb.py
 -rw-r--r--  2.0 unx     1979 b- defN 24-Mar-28 17:20 uav_collision_avoidance/src/simulation/simulation_fps.py
--rw-r--r--  2.0 unx     8170 b- defN 24-Apr-25 10:23 uav_collision_avoidance/src/simulation/simulation_physics.py
+-rw-r--r--  2.0 unx     8359 b- defN 24-Apr-25 10:56 uav_collision_avoidance/src/simulation/simulation_physics.py
 -rw-r--r--  2.0 unx     1041 b- defN 24-Mar-28 17:20 uav_collision_avoidance/src/simulation/simulation_render.py
 -rw-r--r--  2.0 unx      682 b- defN 24-Apr-06 09:52 uav_collision_avoidance/src/simulation/simulation_settings.py
 -rw-r--r--  2.0 unx     6343 b- defN 24-Apr-25 10:24 uav_collision_avoidance/src/simulation/simulation_state.py
 -rw-r--r--  2.0 unx    26085 b- defN 24-Apr-25 10:19 uav_collision_avoidance/src/simulation/simulation_widget.py
--rw-r--r--  2.0 unx     1075 b- defN 24-Apr-25 10:48 uav_collision_avoidance-0.6.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     7374 b- defN 24-Apr-25 10:48 uav_collision_avoidance-0.6.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 10:48 uav_collision_avoidance-0.6.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       73 b- defN 24-Apr-25 10:48 uav_collision_avoidance-0.6.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       58 b- defN 24-Apr-25 10:48 uav_collision_avoidance-0.6.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    14863 b- defN 24-Apr-25 10:48 uav_collision_avoidance-0.6.3.dist-info/RECORD
-111 files, 565982 bytes uncompressed, 127464 bytes compressed:  77.5%
+-rw-r--r--  2.0 unx     1075 b- defN 24-Apr-25 11:08 uav_collision_avoidance-0.6.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7374 b- defN 24-Apr-25 11:08 uav_collision_avoidance-0.6.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 11:08 uav_collision_avoidance-0.6.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       73 b- defN 24-Apr-25 11:08 uav_collision_avoidance-0.6.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       58 b- defN 24-Apr-25 11:08 uav_collision_avoidance-0.6.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    17504 b- defN 24-Apr-25 11:08 uav_collision_avoidance-0.6.4.dist-info/RECORD
+126 files, 655134 bytes uncompressed, 146235 bytes compressed:  77.7%
```

## zipnote {}

```diff
@@ -1,7 +1,52 @@
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/version.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
+Comment: 
+
 Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py
 Comment: 
 
 Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py
 Comment: 
 
 Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py
@@ -309,26 +354,26 @@
 
 Filename: uav_collision_avoidance/src/simulation/simulation_state.py
 Comment: 
 
 Filename: uav_collision_avoidance/src/simulation/simulation_widget.py
 Comment: 
 
-Filename: uav_collision_avoidance-0.6.3.dist-info/LICENSE
+Filename: uav_collision_avoidance-0.6.4.dist-info/LICENSE
 Comment: 
 
-Filename: uav_collision_avoidance-0.6.3.dist-info/METADATA
+Filename: uav_collision_avoidance-0.6.4.dist-info/METADATA
 Comment: 
 
-Filename: uav_collision_avoidance-0.6.3.dist-info/WHEEL
+Filename: uav_collision_avoidance-0.6.4.dist-info/WHEEL
 Comment: 
 
-Filename: uav_collision_avoidance-0.6.3.dist-info/entry_points.txt
+Filename: uav_collision_avoidance-0.6.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: uav_collision_avoidance-0.6.3.dist-info/top_level.txt
+Filename: uav_collision_avoidance-0.6.4.dist-info/top_level.txt
 Comment: 
 
-Filename: uav_collision_avoidance-0.6.3.dist-info/RECORD
+Filename: uav_collision_avoidance-0.6.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py

```diff
@@ -27,14 +27,16 @@
             self.target_yaw_angle : float = self.find_best_yaw_angle(aircraft.position, initial_target)
             self.add_first_destination(initial_target)
 
         self.initial_course : float = copy(self.target_yaw_angle)
         self.target_roll_angle : float = 0.0
         self.target_pitch_angle : float = 0.0
         self.__target_speed : float = self.aircraft.absolute_speed
+        self.__is_turning_right : bool = False
+        self.__is_turning_left : bool = False
 
         self.__evade_maneuver : bool = False
         self.vector_sharing_resolution : QVector3D | None = None
 
         self.destinations_history : List[QVector3D] = []
         self.visited : List[QVector3D] = []
     
@@ -44,37 +46,63 @@
         return self.__target_speed
     
     @target_speed.setter
     def target_speed(self, speed : float) -> None:
         """Sets target speed"""
         if speed > 0:
             self.__target_speed = speed
+    
+    @property
+    def is_turning_right(self) -> bool:
+        """Returns turning right state"""
+        return self.__is_turning_right
+    
+    @is_turning_right.setter
+    def is_turning_right(self, value : bool) -> None:
+        """Sets turning right state"""
+        self.__is_turning_right = value
+
+    @property
+    def is_turning_left(self) -> bool:
+        """Returns turning left state"""
+        return self.__is_turning_left
+    
+    @is_turning_left.setter
+    def is_turning_left(self, value : bool) -> None:
+        """Sets turning left state"""
+        self.__is_turning_left = value
 
     def add_last_destination(self, destination : QVector3D) -> None:
-        """Appends given location to the end of destinations list"""
-        assert isinstance(destination.x(), (int, float))
-        assert isinstance(destination.y(), (int, float))
-        assert isinstance(destination.z(), (int, float))
+        """Appends the given location (QVector3D) to the end of the destinations list."""
+        if not all(isinstance(coord, (int, float)) for coord in (destination.x(), destination.y(), destination.z())):
+            raise TypeError("Destination coordinates must be int or float.")
 
         self.destinations.append(destination)
 
     def add_first_destination(self, destination : QVector3D) -> None:
         """Pushes given location to the top of destinations list"""
-        assert isinstance(destination.x(), (int, float))
-        assert isinstance(destination.y(), (int, float))
-        assert isinstance(destination.z(), (int, float))
+        if not all(isinstance(coord, (int, float)) for coord in (destination.x(), destination.y(), destination.z())):
+            raise TypeError("Destination coordinates must be int or float.")
 
-        if len(self.destinations) > 0 and dist(destination.toTuple(), self.destinations[0].toTuple()) < 1:
+        if len(self.destinations) > 0 and dist(destination.toTuple(), self.destinations[0].toTuple()) < 1.0:
             print("Attempted to stack same destination")
-            logging.warning("Attempted to stack same destination")
+            logging.warning(f"Attempted to stack same destination: {destination}")
             return
 
         self.destinations.appendleft(destination)
         logging.info("Aircraft %s added new first destination: %s", self.aircraft.aircraft_id, destination.toTuple())
 
+    @property
+    def destination(self) -> QVector3D | None:
+        """Returns current destination"""
+        if len(self.destinations) > 0:
+            return self.destinations[0]
+        else:
+            return None
+
     def append_visited(self) -> None:
         """Appends current location to visited list"""
         self.visited.append(copy(self.aircraft.position))
 
     def normalize_angle(self, angle : float) -> float:
         """Normalizes -180-180 angle into 360 domain"""
         angle = angle % 360
@@ -121,19 +149,46 @@
     def reset_evade_maneuver(self) -> None:
         """Resets evade maneuver"""
         if self.__evade_maneuver:
             logging.info("Aircraft %s reset evade maneuver", self.aircraft.aircraft_id)
             self.__evade_maneuver = False
             #self.vector_sharing_resolution = None
 
-    def find_best_roll_angle(self, current_yaw_angle : float, target_yaw_angle : float) -> float:
+    def find_best_roll_angle(self, current_yaw_angle: float, target_yaw_angle: float) -> float:
         """Finds best roll angle for the targeted yaw angle"""
         difference = (target_yaw_angle - current_yaw_angle + 180) % 360 - 180
-        return 0.0 if abs(difference) < 0.01 else 30.0 if difference > 0 else -30.0
-
+        if abs(difference) < 0.001:
+            self.is_turning_right = False
+            self.is_turning_left = False
+            return 0.0
+        elif difference > 0:
+            self.is_turning_right = True
+            self.is_turning_left = False
+            if difference > 90:
+                return 30.0
+            elif difference > 45:
+                return 20.0
+            elif difference > 20:
+                return 10.0
+            else:
+                return 5.0
+        elif difference < 0:
+            self.is_turning_left = True
+            self.is_turning_right = False
+            if difference < -90:
+                return -30.0
+            elif difference < -45:
+                return -20.0
+            elif difference < -20:
+                return -10.0
+            else:
+                return -5.0
+        else:
+            return 0.0
+        
     def find_best_yaw_angle(self, position : QVector3D, destination : QVector3D) -> float:
         """Finds best yaw angle for the given destination"""
         target_yaw_angle : float  = degrees(atan2(
             destination.y() - position.y(),
             destination.x() - position.x()))
         target_yaw_angle += 90
         return self.format_angle(target_yaw_angle)
```

## build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py

```diff
@@ -23,38 +23,46 @@
 class Simulation(QMainWindow):
     """Main simulation App"""
 
     def __init__(self, aircrafts : List[Aircraft] | None = None, simulation_time : int = 100_000) -> None:
         super().__init__()
         SimulationSettings().__init__()
         if aircrafts is None:
-            self.aircrafts : List[Aircraft] = [
-                Aircraft( # detection test
-                    position = QVector3D(100, 1000, 1000),
-                    speed = QVector3D(50, -50, 0),
-                    initial_target = QVector3D(1_000_100, -1_001_000, 1000)),
-                Aircraft(
-                    position = QVector3D(900, 1300, 1000),
-                    speed = QVector3D(0, -70, 0),
-                    initial_target = QVector3D(900, -1_001_300, 1000)),
-                # Aircraft( # head on
-                #     position = QVector3D(100, 500, 1000),
-                #     speed = QVector3D(70, 0, 0)),
-                # Aircraft(
-                #     position = QVector3D(900, 500, 1000),
-                #     speed = QVector3D(-50, 0, 0)),
-                # Aircraft( # avoidance test
-                #     position = QVector3D(10, -10, 0),
-                #     speed = QVector3D(300, -300, 0),
-                #     initial_target = QVector3D(75000, -75000, 0)), # 75 km, -75 km
-                # Aircraft(
-                #     position = QVector3D(0, -100_000, 0),
-                #     speed = QVector3D(300, 290, 0),
-                #     initial_target = QVector3D(75000, -27500, 0)), # 75 km, -27.5 km
-            ]
+            test_case : int = 0
+            if test_case == 0:
+                self.aircrafts : List[Aircraft] = [
+                    Aircraft( # detection test
+                        position = QVector3D(-800, 4000, 1000),
+                        speed = QVector3D(60, -60, 0),
+                        initial_target = QVector3D(1_000_100, -1_001_000, 1000)),
+                    Aircraft(
+                        position = QVector3D(4000, 6000, 1000),
+                        speed = QVector3D(0, -85, 0),
+                        initial_target = QVector3D(900, -1_001_300, 1000)),
+                ]
+            elif test_case == 1:
+                self.aircrafts : List[Aircraft] = [
+                    Aircraft( # almost head on
+                        position = QVector3D(-3000, 500, 1000),
+                        speed = QVector3D(70, 0.1, 0)),
+                    Aircraft(
+                        position = QVector3D(5000, 500, 1000),
+                        speed = QVector3D(-50, 0, 0)),
+                ]
+            elif test_case == 2:
+                self.aircrafts : List[Aircraft] = [
+                    Aircraft( # avoidance test
+                        position = QVector3D(10, -10, 1000),
+                        speed = QVector3D(300, -300, 0),
+                        initial_target = QVector3D(75000, -75000, 0)), # 75 km, -75 km
+                    Aircraft(
+                        position = QVector3D(0, -100_000, 1000),
+                        speed = QVector3D(300, 290, 0),
+                        initial_target = QVector3D(75000, -27500, 0)), # 75 km, -27.5 km
+                ]
         else:
             self.aircrafts = aircrafts
         self.simulation_time : int = simulation_time
         self.state : SimulationState | None = None
 
     def run_realtime(self) -> None:
         """Executes realtime simulation"""
```

## build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py

```diff
@@ -40,14 +40,22 @@
             self.adsb_cycles += 1
             self.simulation_state.update_adsb_settings()
 
             relative_position = aircraft_vehicle_1.position - aircraft_vehicle_2.position
             speed_difference = aircraft_vehicle_1.speed - aircraft_vehicle_2.speed
             time_to_closest_approach = -(QVector3D.dotProduct(relative_position, speed_difference) / QVector3D.dotProduct(speed_difference, speed_difference))
             print("Time to closest approach: " + "{:.2f}".format(time_to_closest_approach) + "s")
+            
+            for aircraft in self.aircraft_vehicles:
+                # path
+                self.aircraft_fccs[aircraft.aircraft_id].append_visited()
+
+                # console output
+                if self.simulation_state.adsb_report and aircraft.aircraft_id == 0:
+                    self.print_adsb_report(aircraft)
 
             if not self.simulation_state.avoid_collisions:
                 return
 
             if time_to_closest_approach > 0:
                 # miss distance at closest approach
                 speed_difference_unit = speed_difference.normalized()
@@ -81,31 +89,43 @@
                 if collision_region > 0:
                     print("Collision detected")
             else:
                 for aircraft in self.aircraft_fccs:
                     if aircraft.evade_maneuver:
                         aircraft.reset_evade_maneuver()
 
-            for aircraft in self.aircraft_vehicles:
-                # path
-                self.aircraft_fccs[aircraft.aircraft_id].append_visited()
-
-                # console output
-                if self.simulation_state.adsb_report and aircraft.aircraft_id == 0:
-                    self.print_adsb_report(aircraft)
-
     def print_adsb_report(self, aircraft : AircraftVehicle) -> None:
         """Prints ADS-B report for the aircraft to the console"""
-        print("Aircraft id: " + str(aircraft.aircraft_id) +
+        fcc = self.aircraft_fccs[aircraft.aircraft_id]
+        turning_direction = "Not turning"
+        if fcc.is_turning_left:
+            turning_direction = "Turning left"
+        elif fcc.is_turning_right:
+            turning_direction = "Turning right"
+        print("- Aircraft id: " + str(aircraft.aircraft_id) +
             "; speed: " + "{:.2f}".format(aircraft.absolute_speed) +
-            "; target speed: " + "{:.2f}".format(self.aircraft_fccs[aircraft.aircraft_id].target_speed) +
+            "; turning: " + turning_direction +
+            "; roll angle: " + "{:.2f}".format(aircraft.roll_angle) +
+            "; target roll angle: " + "{:.2f}".format(fcc.target_roll_angle) +
+            "; yaw angle: " + "{:.2f}".format(aircraft.yaw_angle) +
+            "; target yaw angle: " + "{:.2f}".format(fcc.target_yaw_angle) +
             "; x: " + "{:.2f}".format(aircraft.position.x()) +
             "; y: " + "{:.2f}".format(aircraft.position.y()) +
-            "; yaw angle: " + "{:.2f}".format(aircraft.yaw_angle) +
-            "; target yaw angle: " + "{:.2f}".format(self.aircraft_fccs[aircraft.aircraft_id].target_yaw_angle) +
-            "; pitch angle: " + "{:.2f}".format(aircraft.pitch_angle) +
-            "; roll angle: " + "{:.2f}".format(aircraft.roll_angle) +
-            "; target roll angle: " + "{:.2f}".format(self.aircraft_fccs[aircraft.aircraft_id].target_roll_angle) +
-            "; distance covered: " + "{:.2f}".format(aircraft.distance_covered) +
-            "; fps: " + "{:.2f}".format(self.simulation_state.fps) +
-            "; t: " + str(self.adsb_cycles) +
-            "; phys: " + str(self.simulation_state.physics_cycles))
+            "; z: " + "{:.2f}".format(aircraft.position.z()))
+        if fcc.destination is not None:
+            print("target pitch angle: " + "{:.2f}".format(fcc.target_pitch_angle) +
+                "; pitch angle: " + "{:.2f}".format(aircraft.pitch_angle) +
+                "; dest x: " + "{:.2f}".format(fcc.destination.x()) +
+                "; dest y: " + "{:.2f}".format(fcc.destination.y()) +
+                "; dest z: " + "{:.2f}".format(fcc.destination.z()) +
+                "; distance covered: " + "{:.2f}".format(aircraft.distance_covered) +
+                "; fps: " + "{:.2f}".format(self.simulation_state.fps) +
+                "; t: " + str(self.adsb_cycles) +
+                "; phys: " + str(self.simulation_state.physics_cycles))
+        else:
+            print("target pitch angle: " + "{:.2f}".format(fcc.target_pitch_angle) +
+                "; pitch angle: " + "{:.2f}".format(aircraft.pitch_angle) +
+                "; distance covered: " + "{:.2f}".format(aircraft.distance_covered) +
+                "; fps: " + "{:.2f}".format(self.simulation_state.fps) +
+                "; t: " + str(self.adsb_cycles) +
+                "; phys: " + str(self.simulation_state.physics_cycles) +
+                "; no destination")
```

## build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py

```diff
@@ -117,34 +117,24 @@
             # pitch angle
 
             # yaw angle
             roll_angle : float = aircraft.roll_angle
 
             if roll_angle == 0.0:
                 continue
-            elif fcc.target_roll_angle > 0.0 and roll_angle < 0.0:
-                continue
-            elif fcc.target_roll_angle < 0.0 and roll_angle > 0.0:
-                continue
 
             current_yaw_angle : float = aircraft.yaw_angle
             target_yaw_angle : float = fcc.target_yaw_angle
             if abs(current_yaw_angle - target_yaw_angle) < 0.001:
                 continue
             current_horizontal_speed : float = aircraft.horizontal_speed
-            max_delta_yaw_angle : float = self.simulation_state.g_acceleration * tan(radians(roll_angle)) / (current_horizontal_speed / elapsed_time)
-            max_delta_yaw_angle = abs(max_delta_yaw_angle)
-            if roll_angle < 0.0:
-                max_delta_yaw_angle = -max_delta_yaw_angle
+            delta_yaw_angle : float = self.simulation_state.g_acceleration * tan(radians(roll_angle)) / (current_horizontal_speed / elapsed_time)
 
             new_yaw_angle : float = 0.0
-            if abs(current_yaw_angle - target_yaw_angle) < abs(max_delta_yaw_angle):
-                new_yaw_angle = target_yaw_angle
-            else:
-                new_yaw_angle = current_yaw_angle + max_delta_yaw_angle
+            new_yaw_angle = current_yaw_angle + delta_yaw_angle
 
             aircraft.speed.setX(sin(radians(new_yaw_angle)) * current_horizontal_speed)
             aircraft.speed.setY(-cos(radians(new_yaw_angle)) * current_horizontal_speed)
 
     def count_cycles(self) -> None:
         """Increments physics cycle counter"""
         self.cycles += 1
```

## build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py

```diff
@@ -23,28 +23,32 @@
         self.minimum_separation : float = 9260.0 # 5nmi
         self.physics_cycles : int = 0
         self.is_paused : bool = False
         self.is_running : bool = True
         self.__reset_demanded : bool = False
         self.pause_start_timestamp : QTime | None = None
         self.time_paused : int = 0 # ms
-        self.__adsb_report : bool = False
+        self.__adsb_report : bool = True
         self.__collision : bool = False
         self.__first_cause_collision : bool = False
         self.__second_cause_collision : bool = False
 
         if is_realtime:
             # render state
-            self.__gui_scale : float = 1.0 # define gui scaling
-            if SimulationSettings.screen_resolution.height() < 1440:
-                self.gui_scale = 0.75
-            elif SimulationSettings.screen_resolution.height() < 1080:
-                self.gui_scale = 0.5
-            elif SimulationSettings.screen_resolution.height() < 480:
-                self.gui_scale = 0.25
+            override_gui_scale : bool = True
+            if not override_gui_scale:
+                self.__gui_scale : float = 0.5 # define gui scaling
+                if SimulationSettings.screen_resolution.height() < 1440:
+                    self.gui_scale = 0.375
+                elif SimulationSettings.screen_resolution.height() < 1080:
+                    self.gui_scale = 0.25
+                elif SimulationSettings.screen_resolution.height() < 480:
+                    self.gui_scale = 0.125
+            else:
+                self.__gui_scale : float = 0.75
             self.fps : float = 0.0
             self.draw_fps : bool = True
             self.draw_aircraft : bool = True
             self.draw_grid : bool = False
             self.draw_path : bool = True
             self.draw_speed_vectors : bool = True
             self.draw_collision_detection : bool = True
```

## build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py

```diff
@@ -396,17 +396,17 @@
                 return super().keyPressEvent(event)
             self.simulation_state.toggle_pause()
         elif event.key() == Qt.Key.Key_R:
             if event.isAutoRepeat():
                 return super().keyPressEvent(event)
             self.simulation_state.reset()
         elif event.key() == Qt.Key.Key_Plus:
-            self.zoom(0.25)
+            self.zoom(0.0625)
         elif event.key() == Qt.Key.Key_Minus:
-            self.zoom(-0.25)
+            self.zoom(-0.0625)
         elif event.key() == Qt.Key.Key_F1:
             self.simulation_state.toggle_adsb_report()
         elif event.key() == Qt.Key.Key_F2:
             self.aircraft_fccs[0].target_speed -= 10.0
         elif event.key() == Qt.Key.Key_F3:
             self.aircraft_fccs[0].target_speed += 10.0
         elif event.key() == Qt.Key.Key_O:
```

## build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py

```diff
@@ -29,14 +29,15 @@
 
         self.initial_course : float = copy(self.target_yaw_angle)
         self.target_roll_angle : float = 0.0
         self.target_pitch_angle : float = 0.0
         self.__target_speed : float = self.aircraft.absolute_speed
         self.__is_turning_right : bool = False
         self.__is_turning_left : bool = False
+        self.ignore_destinations : bool = False
 
         self.__evade_maneuver : bool = False
         self.vector_sharing_resolution : QVector3D | None = None
 
         self.destinations_history : List[QVector3D] = []
         self.visited : List[QVector3D] = []
     
@@ -120,34 +121,49 @@
 
     def apply_evade_maneuver(self, opponent_speed : QVector3D, miss_distance_vector : QVector3D, unresolved_region : float, time_to_closest_approach : float) -> None:
         """Applies evade maneuver"""
         print(str(self.aircraft.aircraft_id) + ": opponent speed: " + "{:.2f}".format(opponent_speed.x()) + " " + "{:.2f}".format(opponent_speed.y()) + " " + "{:.2f}".format(opponent_speed.z()))
         print(str(self.aircraft.aircraft_id) + ": miss distance vector: " + "{:.2f}".format(miss_distance_vector.x()) + " " + "{:.2f}".format(miss_distance_vector.y()) + " " + "{:.2f}".format(miss_distance_vector.z()))
         print(str(self.aircraft.aircraft_id) + ": unresolved region: " + "{:.2f}".format(unresolved_region))
         print(str(self.aircraft.aircraft_id) + ": time to closest approach: " + "{:.2f}".format(time_to_closest_approach))
-        
-        if (miss_distance_vector.x() == 0 and miss_distance_vector.y() == 0 and miss_distance_vector.z() == 0):
-            return
 
         if self.__evade_maneuver:
             logging.warning("Another evade maneuver in progress")
         else:
             print(f"Aircraft {self.aircraft.aircraft_id} applying evade maneuver")
             logging.info("Aircraft %s applying evade maneuver", self.aircraft.aircraft_id)
             self.__evade_maneuver = True
-            self.vector_sharing_resolution : QVector3D | None = None
-            if self.aircraft_id == 0:
-                self.vector_sharing_resolution = (opponent_speed.length() * unresolved_region * -(miss_distance_vector)) / ((self.aircraft.speed.length() + opponent_speed.length()) * miss_distance_vector.length())
+
+            # this is temporal solution of the problem below
+            if miss_distance_vector.length() == 0:
+                miss_distance_vector = QVector3D(0.01, 0.01, 0.0)
+
+            target_avoiding : QVector3D = QVector3D()
+            if miss_distance_vector.length() == 0:
+                # todo: fix or just change height
+                # modified_speed_vector : QVector3D = self.aircraft.speed + 0.01 * (self.aircraft.speed.normalized().z() * self.aircraft.speed)
+                # modified_speed_vector : QVector3D = self.aircraft.speed + 0.01 * QVector3D.crossProduct(self.aircraft.speed.normalized(), self.aircraft.speed)
+                # modified_speed_vector : QVector3D = self.aircraft.speed + (QVector3D.crossProduct(QVector3D(0, 0, self.aircraft.speed.normalized().z()), self.aircraft.speed))
+                # print("Modified speed vector: " + "{:.2f}".format(modified_speed_vector.x()) + " " + "{:.2f}".format(modified_speed_vector.y()) + " " + "{:.2f}".format(modified_speed_vector.z()))
+                # unit_vector : QVector3D = modified_speed_vector.normalized()
+                # print("Unit vector: " + "{:.2f}".format(unit_vector.x()) + " " + "{:.2f}".format(unit_vector.y()) + " " + "{:.2f}".format(unit_vector.z()))
+                # target_avoiding = self.aircraft.position + (unit_vector * modified_speed_vector.length())
+                pass
             else:
-                self.vector_sharing_resolution = (opponent_speed.length() * unresolved_region * miss_distance_vector) / ((opponent_speed.length() + self.aircraft.speed.length()) * miss_distance_vector.length())
-            print("Vector sharing resolution: " + "{:.2f}".format(self.vector_sharing_resolution.x()) + " " + "{:.2f}".format(self.vector_sharing_resolution.y()) + " " + "{:.2f}".format(self.vector_sharing_resolution.z()))
+                self.vector_sharing_resolution : QVector3D | None = None
+                if self.aircraft_id == 0:
+                    self.vector_sharing_resolution = (opponent_speed.length() * unresolved_region * -(miss_distance_vector)) / ((self.aircraft.speed.length() + opponent_speed.length()) * miss_distance_vector.length())
+                elif self.aircraft_id == 1:
+                    self.vector_sharing_resolution = (opponent_speed.length() * unresolved_region * miss_distance_vector) / ((opponent_speed.length() + self.aircraft.speed.length()) * miss_distance_vector.length())
+                print("Vector sharing resolution: " + "{:.2f}".format(self.vector_sharing_resolution.x()) + " " + "{:.2f}".format(self.vector_sharing_resolution.y()) + " " + "{:.2f}".format(self.vector_sharing_resolution.z()))
+                modified_speed_vector : QVector3D = (self.aircraft.speed * time_to_closest_approach + self.vector_sharing_resolution)
+                unit_vector : QVector3D = modified_speed_vector.normalized()
+                target_avoiding = self.aircraft.position + (unit_vector * modified_speed_vector.length())
             
-            # self.vector_sharing_resolution *= 2
-
-            target_avoiding : QVector3D = self.aircraft.position + (self.aircraft.speed * time_to_closest_approach + self.vector_sharing_resolution)
+            print("Set target avoiding collision: " + "{:.2f}".format(target_avoiding.x()) + " " + "{:.2f}".format(target_avoiding.y()) + " " + "{:.2f}".format(target_avoiding.z()))
             self.add_first_destination(target_avoiding)
 
     def reset_evade_maneuver(self) -> None:
         """Resets evade maneuver"""
         if self.__evade_maneuver:
             logging.info("Aircraft %s reset evade maneuver", self.aircraft.aircraft_id)
             self.__evade_maneuver = False
@@ -191,15 +207,15 @@
             destination.y() - position.y(),
             destination.x() - position.x()))
         target_yaw_angle += 90
         return self.format_angle(target_yaw_angle)
 
     def update_target_yaw_angle(self) -> None:
         """Updates current yaw angle"""
-        if self.destinations:
+        if self.destinations and not self.ignore_destinations:
             destination = self.destinations[0]
             distance = dist(self.aircraft.position.toTuple(), destination.toTuple())
             if distance < self.aircraft.size / 2:
                 self.destinations_history.append(self.destinations.popleft())
                 if self.destinations:
                     destination = self.destinations[0]
                     logging.info("Aircraft %s visited destination and took next one", self.aircraft.aircraft_id)
```

## build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py

```diff
@@ -23,15 +23,15 @@
 class Simulation(QMainWindow):
     """Main simulation App"""
 
     def __init__(self, aircrafts : List[Aircraft] | None = None, simulation_time : int = 100_000) -> None:
         super().__init__()
         SimulationSettings().__init__()
         if aircrafts is None:
-            test_case : int = 0
+            test_case : int = 3
             if test_case == 0:
                 self.aircrafts : List[Aircraft] = [
                     Aircraft( # detection test
                         position = QVector3D(-800, 4000, 1000),
                         speed = QVector3D(60, -60, 0),
                         initial_target = QVector3D(1_000_100, -1_001_000, 1000)),
                     Aircraft(
@@ -47,21 +47,32 @@
                     Aircraft(
                         position = QVector3D(5000, 500, 1000),
                         speed = QVector3D(-50, 0, 0)),
                 ]
             elif test_case == 2:
                 self.aircrafts : List[Aircraft] = [
                     Aircraft( # avoidance test
-                        position = QVector3D(10, -10, 1000),
+                        position = QVector3D(0, 0, 1000),
+                        speed = QVector3D(30, -30, 0),
+                        initial_target = QVector3D(75000, -75000, 1000)), # 75 km, -75 km
+                    Aircraft(
+                        position = QVector3D(0, -100_000, 1000),
+                        speed = QVector3D(30, 29, 0),
+                        initial_target = QVector3D(75000, -27500, 1000)), # 75 km, -27.5 km
+                ]
+            elif test_case == 3:
+                self.aircrafts : List[Aircraft] = [
+                    Aircraft( # avoidance test fast
+                        position = QVector3D(0, 0, 1000),
                         speed = QVector3D(300, -300, 0),
-                        initial_target = QVector3D(75000, -75000, 0)), # 75 km, -75 km
+                        initial_target = QVector3D(75000, -75000, 1000)), # 75 km, -75 km
                     Aircraft(
                         position = QVector3D(0, -100_000, 1000),
                         speed = QVector3D(300, 290, 0),
-                        initial_target = QVector3D(75000, -27500, 0)), # 75 km, -27.5 km
+                        initial_target = QVector3D(75000, -27500, 1000)), # 75 km, -27.5 km
                 ]
         else:
             self.aircrafts = aircrafts
         self.simulation_time : int = simulation_time
         self.state : SimulationState | None = None
 
     def run_realtime(self) -> None:
```

## build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py

```diff
@@ -62,16 +62,15 @@
                 miss_distance_vector : QVector3D = QVector3D.crossProduct(
                     speed_difference_unit,
                     QVector3D.crossProduct(relative_position, speed_difference_unit))
                 print("Miss distance at closest approach: " + "{:.2f}".format(miss_distance_vector.length()) + "m")
 
                 if miss_distance_vector.length() == 0:
                     print("Head-on collision detected")
-                    # todo: height change maneuver
-                    # else other evade maneuver
+                    logging.info("Head-on collision detected")
 
                 # resolve confict condition
                 unresolved_region : float = self.simulation_state.minimum_separation - abs(miss_distance_vector.length())
                 if unresolved_region > 0.0:
                     print("Conflict condition detected")
                     for aircraft in self.aircraft_fccs:
                         if not aircraft.evade_maneuver:
```

## build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py

```diff
@@ -38,24 +38,42 @@
             SimulationSettings.screen_resolution.height() / 2 - self.window_height / 2 - 30,
             self.window_width,
             self.window_height)
         self.setStyleSheet("background-color: white;")
         self.setWindowTitle(QApplication.applicationName() + " " + QApplication.applicationVersion())
 
         self.icon = QIcon()
-        self.icon.addPixmap(self.simulation_state.aircraft_pixmap, QIcon.Mode.Normal, QIcon.State.Off)
+        self.icon.addPixmap(self.generate_icon(), QIcon.Mode.Normal, QIcon.State.Off)
         self.setWindowIcon(self.icon)
 
-        self.__moving_view_up = False
-        self.__moving_view_down = False
-        self.__moving_view_left = False
-        self.__moving_view_right = False
+        self.__moving_view_up : bool = False
+        self.__moving_view_down : bool = False
+        self.__moving_view_left : bool = False
+        self.__moving_view_right : bool = False
+        self.__steering_left : bool = False
+        self.__steering_right : bool = False
+        self.__steering_up : bool = False
+        self.__steering_down : bool = False
 
         self.center_offsets()
 
+    def generate_icon(self) -> QPixmap:
+        """Returns icon for the main window"""
+        pixmap = QPixmap(self.simulation_state.aircraft_pixmap)
+        painter = QPainter(pixmap)
+        painter.setBrush(QColor("white"))
+        painter.drawEllipse(self.simulation_state.aircraft_pixmap.rect())
+        painter.drawPixmap(
+            self.simulation_state.aircraft_pixmap.width() * 0.125,
+            self.simulation_state.aircraft_pixmap.height() * 0.125,
+            self.simulation_state.aircraft_pixmap.scaled(self.simulation_state.aircraft_pixmap.width() * 0.75,
+            self.simulation_state.aircraft_pixmap.height() * 0.75))
+        painter.end()
+        return pixmap
+
     def draw_aircraft(self, aircraft : AircraftVehicle, scale : float) -> None:
         """Draws given aircraft vehicle"""
         yaw_angle : float = aircraft.yaw_angle
         size : float = aircraft.size * scale
         pixmap : QPixmap
         if not self.simulation_state.aircraft_pixmap.isNull():
             pixmap = self.simulation_state.aircraft_pixmap.scaled(
@@ -272,14 +290,40 @@
         if self.__moving_view_down:
             self.screen_offset_y -= 10.0 / scale
         if self.__moving_view_left:
             self.screen_offset_x += 10.0 / scale
         if self.__moving_view_right:
             self.screen_offset_x -= 10.0 / scale
 
+    def update_steering(self) -> None:
+        """Updates aircraft steering based on current input"""
+        if self.aircrafts[0] and (self.__steering_up or self.__steering_down or self.__steering_left or self.__steering_right):
+            if sum([self.__steering_up, self.__steering_down, self.__steering_left, self.__steering_right]) >= 3:
+                return
+            self.aircraft_fccs[0].ignore_destinations = True
+            target_yaw_angle : float | None = None
+            if self.__steering_up and self.__steering_left:
+                target_yaw_angle = -45.0
+            elif self.__steering_up and self.__steering_right:
+                target_yaw_angle = 45.0
+            elif self.__steering_down and self.__steering_left:
+                target_yaw_angle = -135.0
+            elif self.__steering_down and self.__steering_right:
+                target_yaw_angle = 135.0
+            elif self.__steering_up:
+                target_yaw_angle = 0.0
+            elif self.__steering_down:
+                target_yaw_angle = 180.0
+            elif self.__steering_left:
+                target_yaw_angle = -90.0
+            elif self.__steering_right:
+                target_yaw_angle = 90.0
+            if target_yaw_angle is not None:
+                self.aircraft_fccs[0].target_yaw_angle = target_yaw_angle
+
     def center_offsets(self) -> None:
         """Updates screen offsets centering on selected aircraft"""
         scale : float = self.simulation_state.gui_scale
         id = self.simulation_state.focus_aircraft_id
         self.screen_offset_x = - self.aircraft_vehicles[id].position.x() + self.window_width / 2 / scale
         self.screen_offset_y = - self.aircraft_vehicles[id].position.y() + self.window_height / 2 / scale
 
@@ -291,21 +335,22 @@
     def zoom(self, factor : float) -> None:
         """Zooms in/out the simulation render"""
         if self.simulation_state.gui_scale + factor <= 0:
             return
         old_scale : float = self.simulation_state.gui_scale
         self.simulation_state.gui_scale += factor
         scale : float = self.simulation_state.gui_scale
-        self.screen_offset_x = self.screen_offset_x * old_scale / scale
-        self.screen_offset_y = self.screen_offset_y * old_scale / scale
+        self.screen_offset_x = self.screen_offset_x * (old_scale / scale)
+        self.screen_offset_y = self.screen_offset_y * (old_scale / scale)
 
     def paintEvent(self, event : QPaintEvent) -> None:
         """Qt method painting the aircrafts"""
         self.simulation_fps.count_frame()
         scale : float = self.simulation_state.gui_scale
+        self.update_steering()
         if not self.simulation_state.follow_aircraft:
             self.update_moving_offsets()
         else:
             self.center_offsets()
 
         if self.simulation_state.draw_fps:
             self.draw_text(QVector3D(10, 10, 0), 0, "FPS: " + "{:.2f}".format(self.simulation_state.fps))
@@ -395,14 +440,15 @@
             if event.isAutoRepeat():
                 return super().keyPressEvent(event)
             self.simulation_state.toggle_pause()
         elif event.key() == Qt.Key.Key_R:
             if event.isAutoRepeat():
                 return super().keyPressEvent(event)
             self.simulation_state.reset()
+            self.center_offsets()
         elif event.key() == Qt.Key.Key_Plus:
             self.zoom(0.0625)
         elif event.key() == Qt.Key.Key_Minus:
             self.zoom(-0.0625)
         elif event.key() == Qt.Key.Key_F1:
             self.simulation_state.toggle_adsb_report()
         elif event.key() == Qt.Key.Key_F2:
@@ -425,35 +471,45 @@
             self.__moving_view_right = True
         elif event.key() == Qt.Key.Key_Up:
             self.__moving_view_up = True
         elif event.key() == Qt.Key.Key_Down:
             self.__moving_view_down = True
         if self.aircrafts[0]:
             if event.key() == Qt.Key.Key_A:
-                self.aircraft_fccs[0].target_yaw_angle = -90.0
+                self.__steering_left = True
             elif event.key() == Qt.Key.Key_D:
-                self.aircraft_fccs[0].target_yaw_angle = 90.0
+                self.__steering_right = True
             elif event.key() == Qt.Key.Key_W:
-                self.aircraft_fccs[0].target_yaw_angle = 0.0
+                self.__steering_up = True
             elif event.key() == Qt.Key.Key_S:
-                self.aircraft_fccs[0].target_yaw_angle = 180.0
+                self.__steering_down = True
         return super().keyPressEvent(event)
     
     def keyReleaseEvent(self, event: QKeyEvent) -> None:
         """Qt method controlling keyboard input"""
         if event.key() == Qt.Key.Key_Slash and event.isAutoRepeat() and self.simulation_state.is_paused:
             self.simulation_state.toggle_pause()
         elif event.key() == Qt.Key.Key_Left:
             self.__moving_view_left = False
         elif event.key() == Qt.Key.Key_Right:
             self.__moving_view_right = False
         elif event.key() == Qt.Key.Key_Up:
             self.__moving_view_up = False
         elif event.key() == Qt.Key.Key_Down:
             self.__moving_view_down = False
+        if self.aircrafts[0]:
+            self.aircraft_fccs[0].ignore_destinations = False
+            if event.key() == Qt.Key.Key_A:
+                self.__steering_left = False
+            elif event.key() == Qt.Key.Key_D:
+                self.__steering_right = False
+            elif event.key() == Qt.Key.Key_W:
+                self.__steering_up = False
+            elif event.key() == Qt.Key.Key_S:
+                self.__steering_down = False
         return super().keyReleaseEvent(event)
     
     def resizeEvent(self, event: QPaintEvent) -> None:
         """Qt method controlling window resize event"""
         self.update_resolutions()
         return super().resizeEvent(event)
```

## build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py

```diff
@@ -31,14 +31,15 @@
         self.target_roll_angle : float = 0.0
         self.target_pitch_angle : float = 0.0
         self.__target_speed : float = self.aircraft.absolute_speed
         self.__is_turning_right : bool = False
         self.__is_turning_left : bool = False
         self.ignore_destinations : bool = False
 
+        self.__safe_zone_occupied : bool = False
         self.__evade_maneuver : bool = False
         self.vector_sharing_resolution : QVector3D | None = None
 
         self.destinations_history : List[QVector3D] = []
         self.visited : List[QVector3D] = []
     
     @property
@@ -68,33 +69,43 @@
         return self.__is_turning_left
     
     @is_turning_left.setter
     def is_turning_left(self, value : bool) -> None:
         """Sets turning left state"""
         self.__is_turning_left = value
 
-    def add_last_destination(self, destination : QVector3D) -> None:
-        """Appends the given location (QVector3D) to the end of the destinations list."""
+    def check_new_destination(self, destination : QVector3D, first : bool) -> QVector3D | None:
+        """Checks if the given destination is already in the destinations list"""
         if not all(isinstance(coord, (int, float)) for coord in (destination.x(), destination.y(), destination.z())):
             raise TypeError("Destination coordinates must be int or float.")
+        if len(self.destinations) > 0 and first:
+            if dist(destination.toTuple(), self.destinations[0].toTuple()) < 1.0:
+                print("Attempted to stack same destination")
+                logging.warning(f"Attempted to stack same destination: {destination}")
+                return None
+        elif len(self.destinations) > 0 and not first:
+            if dist(destination.toTuple(), self.destinations[len(self.destinations) - 1].toTuple()) < 1.0:
+                print("Attempted to stack same destination")
+                logging.warning(f"Attempted to stack same destination: {destination}")
+                return None
+        return destination
 
-        self.destinations.append(destination)
+    def add_last_destination(self, destination : QVector3D) -> None:
+        """Appends the given location (QVector3D) to the end of the destinations list."""
+        destination = self.check_new_destination(destination, False)
+        if destination is not None:
+            self.destinations.append(destination)
+            logging.info("Aircraft %s added new last destination: %s", self.aircraft.aircraft_id, destination.toTuple())
 
     def add_first_destination(self, destination : QVector3D) -> None:
         """Pushes given location to the top of destinations list"""
-        if not all(isinstance(coord, (int, float)) for coord in (destination.x(), destination.y(), destination.z())):
-            raise TypeError("Destination coordinates must be int or float.")
-
-        if len(self.destinations) > 0 and dist(destination.toTuple(), self.destinations[0].toTuple()) < 1.0:
-            print("Attempted to stack same destination")
-            logging.warning(f"Attempted to stack same destination: {destination}")
-            return
-
-        self.destinations.appendleft(destination)
-        logging.info("Aircraft %s added new first destination: %s", self.aircraft.aircraft_id, destination.toTuple())
+        destination = self.check_new_destination(destination, True)
+        if destination is not None:
+            self.destinations.appendleft(destination)
+            logging.info("Aircraft %s added new first destination: %s", self.aircraft.aircraft_id, destination.toTuple())
 
     @property
     def destination(self) -> QVector3D | None:
         """Returns current destination"""
         if len(self.destinations) > 0:
             return self.destinations[0]
         else:
@@ -105,20 +116,36 @@
         self.visited.append(copy(self.aircraft.position))
 
     def normalize_angle(self, angle : float) -> float:
         """Normalizes -180-180 angle into 360 domain"""
         angle = angle % 360
         return angle if angle >= 0 else angle + 360
 
-    def format_angle(self, angle : float) -> float:
+    def format_yaw_angle(self, angle : float) -> float:
         """Formats angle into -180-180 domain"""
         angle = self.normalize_angle(angle)
         return angle if angle <= 180 else -180 + (angle - 180)
     
     @property
+    def safe_zone_occupied(self) -> bool:
+        """Returns safe zone occupied state"""
+        return self.__safe_zone_occupied
+    
+    @safe_zone_occupied.setter
+    def safe_zone_occupied(self, value : bool) -> None:
+        """Sets safe zone occupied state"""
+        if self.__safe_zone_occupied and value:
+            print("Safe zone already occupied")
+            logging.warning("Safe zone already occupied")
+        if not self.__safe_zone_occupied and not value:
+            print("Safe zone already free")
+            logging.warning("Safe zone already free")
+        self.__safe_zone_occupied = value
+    
+    @property
     def evade_maneuver(self) -> bool:
         """Returns evade maneuver state"""
         return self.__evade_maneuver
 
     def apply_evade_maneuver(self, opponent_speed : QVector3D, miss_distance_vector : QVector3D, unresolved_region : float, time_to_closest_approach : float) -> None:
         """Applies evade maneuver"""
         print(str(self.aircraft.aircraft_id) + ": opponent speed: " + "{:.2f}".format(opponent_speed.x()) + " " + "{:.2f}".format(opponent_speed.y()) + " " + "{:.2f}".format(opponent_speed.z()))
@@ -203,17 +230,24 @@
         
     def find_best_yaw_angle(self, position : QVector3D, destination : QVector3D) -> float:
         """Finds best yaw angle for the given destination"""
         target_yaw_angle : float  = degrees(atan2(
             destination.y() - position.y(),
             destination.x() - position.x()))
         target_yaw_angle += 90
-        return self.format_angle(target_yaw_angle)
+        return self.format_yaw_angle(target_yaw_angle)
+    
+    def find_best_pitch_angle(self, position : QVector3D, destination : QVector3D) -> float:
+        """Finds best pitch angle for the given destination"""
+        target_pitch_angle : float = degrees(atan2(
+            destination.z() - position.z(),
+            dist(position.toTuple(), destination.toTuple())))
+        return target_pitch_angle
 
-    def update_target_yaw_angle(self) -> None:
+    def update_target_yaw_pitch_angles(self) -> None:
         """Updates current yaw angle"""
         if self.destinations and not self.ignore_destinations:
             destination = self.destinations[0]
             distance = dist(self.aircraft.position.toTuple(), destination.toTuple())
             if distance < self.aircraft.size / 2:
                 self.destinations_history.append(self.destinations.popleft())
                 if self.destinations:
@@ -223,14 +257,17 @@
                 else:
                     logging.info("Aircraft %s visited destination and is free now", self.aircraft.aircraft_id)
                     print(f"Aircraft {self.aircraft.aircraft_id} visited destination and is free now")
                     return
             self.target_yaw_angle = self.find_best_yaw_angle(
                 self.aircraft.position,
                 destination)
+            self.target_pitch_angle = self.find_best_pitch_angle(
+                self.aircraft.position,
+                destination)
             
     def update_target_roll_angle(self) -> None:
         """Updates target roll angle"""
         current_yaw_angle = self.normalize_angle(self.aircraft.yaw_angle)
         target_yaw_angle = self.normalize_angle(self.target_yaw_angle)
         self.target_roll_angle = self.find_best_roll_angle(current_yaw_angle, target_yaw_angle)
 
@@ -240,21 +277,21 @@
                 next_position = self.destinations[0]
                 next_destination = self.destinations[1]
                 next_target_yaw_angle : float = self.find_best_yaw_angle(next_position, next_destination)
                 self.target_roll_angle = self.find_best_roll_angle(current_yaw_angle, next_target_yaw_angle)
 
     def update(self) -> None:
         """Updates current targeted movement angles"""
-        self.update_target_yaw_angle()
+        self.update_target_yaw_pitch_angles()
         self.update_target_roll_angle()
 
     def update_target(self, target : QVector3D) -> None:
         """Updates target position"""
         self.target_yaw_angle = self.find_best_yaw_angle(self.aircraft.position, target)
-        self.update_target_roll_angle()    
+        self.update_target_roll_angle()      
 
     def reset(self) -> None:
         """Resets aircraft flight control computer"""
         self.destinations.clear()
         self.destinations_history.clear()
         self.visited.clear()
         self.target_yaw_angle = self.initial_course
```

## build/lib/uav_collision_avoidance/src/simulation/simulation.py

```diff
@@ -23,25 +23,25 @@
 class Simulation(QMainWindow):
     """Main simulation App"""
 
     def __init__(self, aircrafts : List[Aircraft] | None = None, simulation_time : int = 100_000) -> None:
         super().__init__()
         SimulationSettings().__init__()
         if aircrafts is None:
-            test_case : int = 3
+            test_case : int = 0
             if test_case == 0:
                 self.aircrafts : List[Aircraft] = [
                     Aircraft( # detection test
                         position = QVector3D(-800, 4000, 1000),
                         speed = QVector3D(60, -60, 0),
-                        initial_target = QVector3D(1_000_100, -1_001_000, 1000)),
+                        initial_target = QVector3D(1_000_100, -1_001_000, 10000)),
                     Aircraft(
                         position = QVector3D(4000, 6000, 1000),
                         speed = QVector3D(0, -85, 0),
-                        initial_target = QVector3D(900, -1_001_300, 1000)),
+                        initial_target = QVector3D(900, -1_001_300, 10000)),
                 ]
             elif test_case == 1:
                 self.aircrafts : List[Aircraft] = [
                     Aircraft( # almost head on
                         position = QVector3D(-3000, 500, 1000),
                         speed = QVector3D(70, 0.1, 0)),
                     Aircraft(
```

## build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py

```diff
@@ -42,21 +42,42 @@
 
             relative_position = aircraft_vehicle_1.position - aircraft_vehicle_2.position
             speed_difference = aircraft_vehicle_1.speed - aircraft_vehicle_2.speed
             time_to_closest_approach = -(QVector3D.dotProduct(relative_position, speed_difference) / QVector3D.dotProduct(speed_difference, speed_difference))
             print("Time to closest approach: " + "{:.2f}".format(time_to_closest_approach) + "s")
             
             for aircraft in self.aircraft_vehicles:
+                fcc : AircraftFCC = self.aircraft_fccs[aircraft.aircraft_id]
+
                 # path
-                self.aircraft_fccs[aircraft.aircraft_id].append_visited()
+                fcc.append_visited()
+
+                # console destination reach time
+                if fcc.destination and self.simulation_state.adsb_report:
+                    time_to_reaching_destination : float = (QVector3D.dotProduct(fcc.destination - aircraft.position, aircraft.speed) / QVector3D.dotProduct(aircraft.speed, aircraft.speed))
+                    print(f"Aircraft {aircraft.aircraft_id} will reach its destination in " + "{:.2f}".format(time_to_reaching_destination) + " (" + "{:.1f}".format(time_to_reaching_destination / 60) + " minutes or " + "{:.1f}".format(time_to_reaching_destination / 3600) + " hours)")
 
-                # console output
+                # console report output
                 if self.simulation_state.adsb_report and aircraft.aircraft_id == 0:
                     self.print_adsb_report(aircraft)
 
+                # safe zone occupancy check
+                if relative_position.length() < self.simulation_state.minimum_separation:
+                    if not fcc.safe_zone_occupied:
+                        fcc.safe_zone_occupied = True
+                        if not self.simulation_state.override_avoid_collisions:
+                            self.simulation_state.avoid_collisions = True
+                    print("Safe zone occupied")
+                else:
+                    if fcc.safe_zone_occupied:
+                        fcc.safe_zone_occupied = False
+                        self.simulation_state.avoid_collisions = False
+                    print("Safe zone free")
+                    return
+
             if not self.simulation_state.avoid_collisions:
                 return
 
             if time_to_closest_approach > 0:
                 # miss distance at closest approach
                 speed_difference_unit = speed_difference.normalized()
                 miss_distance_vector : QVector3D = QVector3D.crossProduct(
```

## build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py

```diff
@@ -1,12 +1,12 @@
 """Simulation physics thread module"""
 
 import logging
 from copy import copy
-from math import sin, cos, dist, tan, radians
+from math import sin, cos, dist, tan, radians, sqrt
 from typing import List
 
 from PySide6.QtCore import QThread, QTime
 from PySide6.QtGui import QVector3D
 from PySide6.QtWidgets import QApplication, QMainWindow
 
 from ..aircraft.aircraft import Aircraft
@@ -50,15 +50,15 @@
         if self.simulation_state.reset_demanded:
             self.reset_aircrafts()
         if not self.simulation_state.is_paused:
             self.count_cycles()
             self.simulation_state.update_simulation_settings()
             self.update_aircrafts_speed_angles(elapsed_time)
             if self.update_aircrafts_position(elapsed_time):
-                logging.warn("Aircrafts collided at coordinates: " + str(self.aircraft_vehicles[0].position.toTuple()) + " and " + str(self.aircraft_vehicles[1].position.toTuple()))
+                logging.warn("Collision Occured. Aircrafts coordinates: " + str(self.aircraft_vehicles[0].position.toTuple()) + " and " + str(self.aircraft_vehicles[1].position.toTuple()))
                 QApplication.beep()
                 self.simulation_state.register_collision()
                 if self.isRunning():
                     self.requestInterruption()
 
     def reset_aircrafts(self) -> None:
         """Resets aircrafts to initial state"""
@@ -67,17 +67,20 @@
         self.aircraft_fccs[0].reset()
         self.aircraft_fccs[1].reset()
         self.simulation_state.apply_reset()
 
     def update_aircrafts_position(self, elapsed_time : float) -> bool:
         """Updates aircrafts position, returns true on collision"""
         for aircraft in self.aircraft_vehicles:
+            if aircraft.position.z() <= 0.0:
+                print("Collision with ground")
+                return True
             relative_distance : float = dist(aircraft.position.toTuple(), self.aircraft_vehicles[1 - aircraft.aircraft_id].position.toTuple())
             if relative_distance <= aircraft.size:
-                print("Collision")
+                print("Collision with another aircraft")
                 return True
             old_pos : QVector3D = copy(aircraft.position)
             aircraft.move(
                 aircraft.speed.x() * elapsed_time / 1000.0,
                 aircraft.speed.y() * elapsed_time / 1000.0,
                 aircraft.speed.z() * elapsed_time / 1000.0)
             aircraft.distance_covered = dist(old_pos.toTuple(), aircraft.position.toTuple())
@@ -93,15 +96,15 @@
             cause_collision = self.simulation_state.first_cause_collision if id == 0 else self.simulation_state.second_cause_collision
             fcc.update() if not cause_collision else fcc.update_target(self.aircraft_vehicles[1 - id].position + self.aircraft_vehicles[1 - id].speed)
             
             # speed
             current_speed = aircraft.absolute_speed
             target_speed = fcc.target_speed
             speed_difference = abs(current_speed - target_speed)
-            if speed_difference > 0.001 and target_speed > 20.0:
+            if speed_difference > 0.001 and current_speed > 20.0 and current_speed < 340: # make drone subsonic
                 max_speed_delta = aircraft.max_acceleration / elapsed_time
                 if speed_difference < max_speed_delta:
                     pass # become target
                 elif current_speed < target_speed:
                     target_speed = current_speed + max_speed_delta
                 else:
                     target_speed = current_speed - max_speed_delta
@@ -111,31 +114,48 @@
                     aircraft.speed.y() * speed_scale_factor,
                     aircraft.speed.z() * speed_scale_factor)
 
             # roll angle
             aircraft.roll_angle = (1.0 / (aircraft.roll_dynamic_delay / elapsed_time)) * (fcc.target_roll_angle - aircraft.roll_angle)
 
             # pitch angle
+            current_pitch_angle : float = aircraft.pitch_angle
+            target_pitch_angle : float = copy(fcc.target_pitch_angle)
+            if not abs(current_pitch_angle - target_pitch_angle) < 0.001 and current_pitch_angle < 90.0 and current_pitch_angle > -90.0:
+                delta_pitch_angle : float = (1.0 / (aircraft.pitch_dynamic_delay / elapsed_time)) * (target_pitch_angle - aircraft.pitch_angle)
+                new_pitch_angle : float = current_pitch_angle
+                if target_pitch_angle > 0:
+                    if target_pitch_angle > current_pitch_angle:
+                        new_pitch_angle = current_pitch_angle + delta_pitch_angle
+                    else:
+                        new_pitch_angle = current_pitch_angle - delta_pitch_angle
+                else: # target_pitch_angle < 0
+                    if target_pitch_angle < current_pitch_angle:
+                        new_pitch_angle = current_pitch_angle + delta_pitch_angle
+                    else:
+                        new_pitch_angle = current_pitch_angle - delta_pitch_angle
 
+                current_speed : float = aircraft.absolute_speed
+                new_speed_z = current_speed * sin(radians(new_pitch_angle))
+                aircraft.speed = QVector3D(
+                    aircraft.speed.x(),
+                    aircraft.speed.y(),
+                    new_speed_z)
+                
             # yaw angle
             roll_angle : float = aircraft.roll_angle
-
-            if roll_angle == 0.0:
-                continue
-
             current_yaw_angle : float = aircraft.yaw_angle
             target_yaw_angle : float = fcc.target_yaw_angle
-            if abs(current_yaw_angle - target_yaw_angle) < 0.001:
-                continue
-            current_horizontal_speed : float = aircraft.horizontal_speed
-            delta_yaw_angle : float = self.simulation_state.g_acceleration * tan(radians(roll_angle)) / (current_horizontal_speed / elapsed_time)
+            if not (roll_angle == 0.0 or abs(current_yaw_angle - target_yaw_angle) < 0.001):
+                current_horizontal_speed : float = aircraft.horizontal_speed
+                delta_yaw_angle : float = self.simulation_state.g_acceleration * tan(radians(roll_angle)) / (current_horizontal_speed / elapsed_time)
 
-            new_yaw_angle : float = 0.0
-            new_yaw_angle = current_yaw_angle + delta_yaw_angle
+                new_yaw_angle : float = 0.0
+                new_yaw_angle = current_yaw_angle + delta_yaw_angle
 
-            aircraft.speed.setX(sin(radians(new_yaw_angle)) * current_horizontal_speed)
-            aircraft.speed.setY(-cos(radians(new_yaw_angle)) * current_horizontal_speed)
+                aircraft.speed.setX(sin(radians(new_yaw_angle)) * current_horizontal_speed)
+                aircraft.speed.setY(-cos(radians(new_yaw_angle)) * current_horizontal_speed)
 
     def count_cycles(self) -> None:
         """Increments physics cycle counter"""
         self.cycles += 1
         self.simulation_state.physics_cycles = self.cycles
```

## build/lib/uav_collision_avoidance/src/simulation/simulation_state.py

```diff
@@ -16,14 +16,15 @@
         self.__mutex : QMutex = QMutex()
 
         # simulation state
         self.simulation_settings = simulation_settings
         self.update_settings()
         self.is_realtime : bool = is_realtime
         self.avoid_collisions : bool = avoid_collisions
+        self.override_avoid_collisions : bool = True
         self.minimum_separation : float = 9260.0 # 5nmi
         self.physics_cycles : int = 0
         self.is_paused : bool = False
         self.is_running : bool = True
         self.__reset_demanded : bool = False
         self.pause_start_timestamp : QTime | None = None
         self.time_paused : int = 0 # ms
```

## build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py

```diff
@@ -217,15 +217,15 @@
         predicted_collision : bool = False
         time_to_closest_approach : float = 0.0
         if self.simulation_state.collision:
             self.draw_text(QVector3D(self.window_width - 70, 10, 0), 0, "COLLISION", QColor(255, 0, 0))
             return
         for aircraft in self.aircraft_vehicles:
             relative_position = aircraft.position - self.aircraft_vehicles[1 - aircraft.aircraft_id].position
-            speed_difference = aircraft.speed - self.aircraft_vehicles[1 - aircraft.aircraft_id].speed
+            speed_difference : QVector3D = aircraft.speed - self.aircraft_vehicles[1 - aircraft.aircraft_id].speed
             time_to_closest_approach = -(QVector3D.dotProduct(relative_position, speed_difference) / QVector3D.dotProduct(speed_difference, speed_difference))
             if time_to_closest_approach > 0:
                 speed_difference_unit = speed_difference.normalized()
                 miss_distance_vector : QVector3D = QVector3D.crossProduct(
                     speed_difference_unit,
                     QVector3D.crossProduct(relative_position, speed_difference_unit))
                 collision_distance = aircraft.size / 2 + self.aircraft_vehicles[1 - aircraft.aircraft_id].size / 2
@@ -320,26 +320,31 @@
             if target_yaw_angle is not None:
                 self.aircraft_fccs[0].target_yaw_angle = target_yaw_angle
 
     def center_offsets(self) -> None:
         """Updates screen offsets centering on selected aircraft"""
         scale : float = self.simulation_state.gui_scale
         id = self.simulation_state.focus_aircraft_id
-        self.screen_offset_x = - self.aircraft_vehicles[id].position.x() + self.window_width / 2 / scale
-        self.screen_offset_y = - self.aircraft_vehicles[id].position.y() + self.window_height / 2 / scale
+        self.screen_offset_x = (self.window_width / 2.0) / scale - self.aircraft_vehicles[id].position.x()
+        self.screen_offset_y = (self.window_height / 2.0) / scale - self.aircraft_vehicles[id].position.y()
 
     def update_resolutions(self) -> None:
         """Updates bounding box resolution"""
         self.window_width = self.width()
         self.window_height = self.height()
 
     def zoom(self, factor : float) -> None:
         """Zooms in/out the simulation render"""
-        if self.simulation_state.gui_scale + factor <= 0:
+        if self.simulation_state.gui_scale + factor >= 2:
+            self.simulation_state.gui_scale = 2
             return
+        while factor > 0 and factor > 2 * self.simulation_state.gui_scale:
+            factor /= 2
+        while factor < 0 and self.simulation_state.gui_scale + factor <= 0:
+            factor /= 2
         old_scale : float = self.simulation_state.gui_scale
         self.simulation_state.gui_scale += factor
         scale : float = self.simulation_state.gui_scale
         self.screen_offset_x = self.screen_offset_x * (old_scale / scale)
         self.screen_offset_y = self.screen_offset_y * (old_scale / scale)
 
     def paintEvent(self, event : QPaintEvent) -> None:
```

## uav_collision_avoidance/src/aircraft/aircraft_fcc.py

```diff
@@ -83,26 +83,34 @@
                 logging.warning(f"Attempted to stack same destination: {destination}")
                 return None
         elif len(self.destinations) > 0 and not first:
             if dist(destination.toTuple(), self.destinations[len(self.destinations) - 1].toTuple()) < 1.0:
                 print("Attempted to stack same destination")
                 logging.warning(f"Attempted to stack same destination: {destination}")
                 return None
+        if destination.z() < 500:
+            if destination.z() < 0:
+                print("Attempted to set destination below ground")
+                logging.warning(f"Attempted to set destination below ground: {destination}")
+            else:
+                print("Attempted to set destination too low")
+                logging.warning(f"Attempted to set destination too low: {destination}")
+            destination = QVector3D(destination.x(), destination.y(), 500)
         return destination
 
     def add_last_destination(self, destination : QVector3D) -> None:
         """Appends the given location (QVector3D) to the end of the destinations list."""
-        destination = self.check_new_destination(destination, False)
+        destination : QVector3D = self.check_new_destination(destination, False)
         if destination is not None:
             self.destinations.append(destination)
             logging.info("Aircraft %s added new last destination: %s", self.aircraft.aircraft_id, destination.toTuple())
 
     def add_first_destination(self, destination : QVector3D) -> None:
         """Pushes given location to the top of destinations list"""
-        destination = self.check_new_destination(destination, True)
+        destination : QVector3D = self.check_new_destination(destination, True)
         if destination is not None:
             self.destinations.appendleft(destination)
             logging.info("Aircraft %s added new first destination: %s", self.aircraft.aircraft_id, destination.toTuple())
 
     @property
     def destination(self) -> QVector3D | None:
         """Returns current destination"""
```

## uav_collision_avoidance/src/simulation/simulation_physics.py

```diff
@@ -50,15 +50,14 @@
         if self.simulation_state.reset_demanded:
             self.reset_aircrafts()
         if not self.simulation_state.is_paused:
             self.count_cycles()
             self.simulation_state.update_simulation_settings()
             self.update_aircrafts_speed_angles(elapsed_time)
             if self.update_aircrafts_position(elapsed_time):
-                logging.warn("Collision Occured. Aircrafts coordinates: " + str(self.aircraft_vehicles[0].position.toTuple()) + " and " + str(self.aircraft_vehicles[1].position.toTuple()))
                 QApplication.beep()
                 self.simulation_state.register_collision()
                 if self.isRunning():
                     self.requestInterruption()
 
     def reset_aircrafts(self) -> None:
         """Resets aircrafts to initial state"""
@@ -68,18 +67,20 @@
         self.aircraft_fccs[1].reset()
         self.simulation_state.apply_reset()
 
     def update_aircrafts_position(self, elapsed_time : float) -> bool:
         """Updates aircrafts position, returns true on collision"""
         for aircraft in self.aircraft_vehicles:
             if aircraft.position.z() <= 0.0:
+                logging.warn("Aircraft's " + str(aircraft.aircraft_id) + "collision with the ground. Coordinates: " + str(self.aircraft_vehicles[aircraft.aircraft_id].position.toTuple()))
                 print("Collision with ground")
                 return True
             relative_distance : float = dist(aircraft.position.toTuple(), self.aircraft_vehicles[1 - aircraft.aircraft_id].position.toTuple())
             if relative_distance <= aircraft.size:
+                logging.warn("Aircrafts' 0 and 1 collision. Coordinates: " + str(self.aircraft_vehicles[0].position.toTuple()) + " and " + str(self.aircraft_vehicles[1].position.toTuple()))
                 print("Collision with another aircraft")
                 return True
             old_pos : QVector3D = copy(aircraft.position)
             aircraft.move(
                 aircraft.speed.x() * elapsed_time / 1000.0,
                 aircraft.speed.y() * elapsed_time / 1000.0,
                 aircraft.speed.z() * elapsed_time / 1000.0)
```

## Comparing `uav_collision_avoidance-0.6.3.dist-info/LICENSE` & `uav_collision_avoidance-0.6.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `uav_collision_avoidance-0.6.3.dist-info/METADATA` & `uav_collision_avoidance-0.6.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uav-collision-avoidance
-Version: 0.6.3
+Version: 0.6.4
 Summary: UAV collision avoidance simulation
 Author-email: mldxo <miloszmaculewicz@gmail.com>
 Project-URL: Homepage, https://github.com/mldxo/uav-collision-avoidance
 Project-URL: Issues, https://github.com/mldxo/uav-collision-avoidance/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `uav_collision_avoidance-0.6.3.dist-info/RECORD` & `uav_collision_avoidance-0.6.4.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,37 @@
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py,sha256=iSdvIjN0pJhhnnrvTowieDMMnjU1HcZycfH0PK5lhEo,107
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py,sha256=fE4gQOSVcsNLjTsO_Efa39pHqkC6Fjj6nCMGp0twYDw,121
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py,sha256=kXX-REh00037lwvz5n2EAci-9f2nYYAAAkypW1lDpJU,2203
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/version.py,sha256=I6WvYCjHdTuOXOG8owwghajl8vOW_aevumGXnBl_sPk,238
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py,sha256=HbmkQi8lHpJHZL8KBCa3DTzw2q3ybdg7OTHz0eCXJAY,1662
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=7y-WaszHOstlbNzr3cAqYNZK4F94-lZqwtFX2M3pRQ8,9540
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py,sha256=Hdc1sQujBzdVMM5q5TsVDyJCyIxm7xi8S5FXD9WHJ8g,4195
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py,sha256=GakasXPXcBn-VBRsF2DxUGB_bQF4ngxRAa2KOdsj7kY,8671
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py,sha256=xF-IM-ljjJyc2GWSuiwVVcGzlzirrPhEAv3y8qAWobU,6057
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py,sha256=fBVukWmBt1md9Klep9J7_WqpzRIDWYHpdo4o8UZyvk0,1979
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py,sha256=6yf0nb_AfOsEmyaea5ywDy2q0N1tgfY_fimis4HG3YY,7112
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py,sha256=_Mb1k6Y1mRHtejgWByU-MmAIx4cSmwVBtaBqao0nrLk,1041
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py,sha256=gL0BI6DecE8MYBNex8-KMgNVqpUWuFoOo65chOypXi0,682
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py,sha256=lFwovBDK4mmX3Y6B34v--dv-2975e1va6aAtFQ70Ie4,6110
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py,sha256=XaPV0vLLQ0PrP1_r9dmJ8BlEkfaQ9dHJROGTjqv4t2Q,23164
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py,sha256=iSdvIjN0pJhhnnrvTowieDMMnjU1HcZycfH0PK5lhEo,107
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py,sha256=fE4gQOSVcsNLjTsO_Efa39pHqkC6Fjj6nCMGp0twYDw,121
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py,sha256=kXX-REh00037lwvz5n2EAci-9f2nYYAAAkypW1lDpJU,2203
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/version.py,sha256=I6WvYCjHdTuOXOG8owwghajl8vOW_aevumGXnBl_sPk,238
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py,sha256=HbmkQi8lHpJHZL8KBCa3DTzw2q3ybdg7OTHz0eCXJAY,1662
-build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=7y-WaszHOstlbNzr3cAqYNZK4F94-lZqwtFX2M3pRQ8,9540
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=XQOQjmXNAaX5aNeD0SPGLSSqU2dBksXdhOR1acALwgY,11332
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py,sha256=Hdc1sQujBzdVMM5q5TsVDyJCyIxm7xi8S5FXD9WHJ8g,4195
-build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py,sha256=GakasXPXcBn-VBRsF2DxUGB_bQF4ngxRAa2KOdsj7kY,8671
-build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py,sha256=xF-IM-ljjJyc2GWSuiwVVcGzlzirrPhEAv3y8qAWobU,6057
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py,sha256=E0SjNZiSmjte8UHPu9yebCFPjzg2-mF3Z7U45cd9KU8,9028
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py,sha256=Av5-ayC8GFdNFXplPsBr3CBhfc_7yoiz3AICrMVdShQ,7108
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py,sha256=fBVukWmBt1md9Klep9J7_WqpzRIDWYHpdo4o8UZyvk0,1979
-build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py,sha256=6yf0nb_AfOsEmyaea5ywDy2q0N1tgfY_fimis4HG3YY,7112
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py,sha256=0HVuLQl4q7-HkJWGd1dJkss-Dg3WXYVJZl3CkEAGvJI,6613
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py,sha256=_Mb1k6Y1mRHtejgWByU-MmAIx4cSmwVBtaBqao0nrLk,1041
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py,sha256=gL0BI6DecE8MYBNex8-KMgNVqpUWuFoOo65chOypXi0,682
-build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py,sha256=lFwovBDK4mmX3Y6B34v--dv-2975e1va6aAtFQ70Ie4,6110
-build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py,sha256=XaPV0vLLQ0PrP1_r9dmJ8BlEkfaQ9dHJROGTjqv4t2Q,23164
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py,sha256=OANRlZ5PlGypf36dXPaXbQTwQ7PLQ1BgnFXyWs0RpXg,6290
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py,sha256=f_Pa-mno9bDVRga2LhTAcoQ3jtVRLjuJlMVEFW5cnq4,23168
 build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py,sha256=iSdvIjN0pJhhnnrvTowieDMMnjU1HcZycfH0PK5lhEo,107
 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py,sha256=fE4gQOSVcsNLjTsO_Efa39pHqkC6Fjj6nCMGp0twYDw,121
 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py,sha256=kXX-REh00037lwvz5n2EAci-9f2nYYAAAkypW1lDpJU,2203
 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/version.py,sha256=I6WvYCjHdTuOXOG8owwghajl8vOW_aevumGXnBl_sPk,238
 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py,sha256=HbmkQi8lHpJHZL8KBCa3DTzw2q3ybdg7OTHz0eCXJAY,1662
 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=XQOQjmXNAaX5aNeD0SPGLSSqU2dBksXdhOR1acALwgY,11332
 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py,sha256=Hdc1sQujBzdVMM5q5TsVDyJCyIxm7xi8S5FXD9WHJ8g,4195
@@ -59,53 +74,53 @@
 build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py,sha256=OANRlZ5PlGypf36dXPaXbQTwQ7PLQ1BgnFXyWs0RpXg,6290
 build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py,sha256=f_Pa-mno9bDVRga2LhTAcoQ3jtVRLjuJlMVEFW5cnq4,23168
 build/lib/build/lib/tests/test_sample.py,sha256=iSdvIjN0pJhhnnrvTowieDMMnjU1HcZycfH0PK5lhEo,107
 build/lib/build/lib/uav_collision_avoidance/__init__.py,sha256=fE4gQOSVcsNLjTsO_Efa39pHqkC6Fjj6nCMGp0twYDw,121
 build/lib/build/lib/uav_collision_avoidance/main.py,sha256=kXX-REh00037lwvz5n2EAci-9f2nYYAAAkypW1lDpJU,2203
 build/lib/build/lib/uav_collision_avoidance/version.py,sha256=I6WvYCjHdTuOXOG8owwghajl8vOW_aevumGXnBl_sPk,238
 build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py,sha256=HbmkQi8lHpJHZL8KBCa3DTzw2q3ybdg7OTHz0eCXJAY,1662
-build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=XQOQjmXNAaX5aNeD0SPGLSSqU2dBksXdhOR1acALwgY,11332
+build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=tTvb9t_vO-ZwMivy5p1M66zx70oEigyd0sVsZQlgeu8,13017
 build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py,sha256=Hdc1sQujBzdVMM5q5TsVDyJCyIxm7xi8S5FXD9WHJ8g,4195
-build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py,sha256=E0SjNZiSmjte8UHPu9yebCFPjzg2-mF3Z7U45cd9KU8,9028
-build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py,sha256=Av5-ayC8GFdNFXplPsBr3CBhfc_7yoiz3AICrMVdShQ,7108
+build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py,sha256=PWU65G5kARp5A3saSLI01ieAe2JWgnY0ObmHTrfcF-Y,9630
+build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py,sha256=xsWQk4Z8GJWhvFC9LIoTznzYBHR88MwsJH50l96mbyE,7072
 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py,sha256=fBVukWmBt1md9Klep9J7_WqpzRIDWYHpdo4o8UZyvk0,1979
 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py,sha256=0HVuLQl4q7-HkJWGd1dJkss-Dg3WXYVJZl3CkEAGvJI,6613
 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py,sha256=_Mb1k6Y1mRHtejgWByU-MmAIx4cSmwVBtaBqao0nrLk,1041
 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py,sha256=gL0BI6DecE8MYBNex8-KMgNVqpUWuFoOo65chOypXi0,682
 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py,sha256=OANRlZ5PlGypf36dXPaXbQTwQ7PLQ1BgnFXyWs0RpXg,6290
-build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py,sha256=f_Pa-mno9bDVRga2LhTAcoQ3jtVRLjuJlMVEFW5cnq4,23168
+build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py,sha256=EkTPWUgSrPVfz19RQJAaT09kqYyrkES8P15xLEayVwQ,25822
 build/lib/tests/test_sample.py,sha256=iSdvIjN0pJhhnnrvTowieDMMnjU1HcZycfH0PK5lhEo,107
 build/lib/uav_collision_avoidance/__init__.py,sha256=fE4gQOSVcsNLjTsO_Efa39pHqkC6Fjj6nCMGp0twYDw,121
 build/lib/uav_collision_avoidance/main.py,sha256=kXX-REh00037lwvz5n2EAci-9f2nYYAAAkypW1lDpJU,2203
 build/lib/uav_collision_avoidance/version.py,sha256=I6WvYCjHdTuOXOG8owwghajl8vOW_aevumGXnBl_sPk,238
 build/lib/uav_collision_avoidance/src/aircraft/aircraft.py,sha256=HbmkQi8lHpJHZL8KBCa3DTzw2q3ybdg7OTHz0eCXJAY,1662
-build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=tTvb9t_vO-ZwMivy5p1M66zx70oEigyd0sVsZQlgeu8,13017
+build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=2SYsOuJQZRFbtfLe5-tIQUVcQahHFozmIfUAtK3atPY,14940
 build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py,sha256=Hdc1sQujBzdVMM5q5TsVDyJCyIxm7xi8S5FXD9WHJ8g,4195
-build/lib/uav_collision_avoidance/src/simulation/simulation.py,sha256=PWU65G5kARp5A3saSLI01ieAe2JWgnY0ObmHTrfcF-Y,9630
-build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py,sha256=xsWQk4Z8GJWhvFC9LIoTznzYBHR88MwsJH50l96mbyE,7072
+build/lib/uav_collision_avoidance/src/simulation/simulation.py,sha256=z1PxcQhD6echdvaDRu9O_gLhCvu7bb2ixqBbesHGrkA,9632
+build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py,sha256=t_5cGYVMpNkdY4751jeggRKQ_E5yqoRl8y_IBcz2BEw,8427
 build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py,sha256=fBVukWmBt1md9Klep9J7_WqpzRIDWYHpdo4o8UZyvk0,1979
-build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py,sha256=0HVuLQl4q7-HkJWGd1dJkss-Dg3WXYVJZl3CkEAGvJI,6613
+build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py,sha256=9sfCvqk7_KZPSC7VIzeDEURiHJDA2b9dUefJRTx5rkU,8170
 build/lib/uav_collision_avoidance/src/simulation/simulation_render.py,sha256=_Mb1k6Y1mRHtejgWByU-MmAIx4cSmwVBtaBqao0nrLk,1041
 build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py,sha256=gL0BI6DecE8MYBNex8-KMgNVqpUWuFoOo65chOypXi0,682
-build/lib/uav_collision_avoidance/src/simulation/simulation_state.py,sha256=OANRlZ5PlGypf36dXPaXbQTwQ7PLQ1BgnFXyWs0RpXg,6290
-build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py,sha256=EkTPWUgSrPVfz19RQJAaT09kqYyrkES8P15xLEayVwQ,25822
+build/lib/uav_collision_avoidance/src/simulation/simulation_state.py,sha256=TI-8V3DznKtmewZWuHKGYIzzZmAolaj89bPGdO1VyIg,6343
+build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py,sha256=BcH_2wSJsC_6ind9wDG7OGbciKPiQirR4WxPVdSUWsk,26085
 tests/test_sample.py,sha256=iSdvIjN0pJhhnnrvTowieDMMnjU1HcZycfH0PK5lhEo,107
 uav_collision_avoidance/__init__.py,sha256=fE4gQOSVcsNLjTsO_Efa39pHqkC6Fjj6nCMGp0twYDw,121
 uav_collision_avoidance/main.py,sha256=kXX-REh00037lwvz5n2EAci-9f2nYYAAAkypW1lDpJU,2203
 uav_collision_avoidance/version.py,sha256=I6WvYCjHdTuOXOG8owwghajl8vOW_aevumGXnBl_sPk,238
 uav_collision_avoidance/src/aircraft/aircraft.py,sha256=HbmkQi8lHpJHZL8KBCa3DTzw2q3ybdg7OTHz0eCXJAY,1662
-uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=2SYsOuJQZRFbtfLe5-tIQUVcQahHFozmIfUAtK3atPY,14940
+uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=Fkt_i2AGZcmsiitGbLyRqwLhbID-5eR8BdaOC6GgEVQ,15437
 uav_collision_avoidance/src/aircraft/aircraft_vehicle.py,sha256=Hdc1sQujBzdVMM5q5TsVDyJCyIxm7xi8S5FXD9WHJ8g,4195
 uav_collision_avoidance/src/simulation/simulation.py,sha256=z1PxcQhD6echdvaDRu9O_gLhCvu7bb2ixqBbesHGrkA,9632
 uav_collision_avoidance/src/simulation/simulation_adsb.py,sha256=t_5cGYVMpNkdY4751jeggRKQ_E5yqoRl8y_IBcz2BEw,8427
 uav_collision_avoidance/src/simulation/simulation_fps.py,sha256=fBVukWmBt1md9Klep9J7_WqpzRIDWYHpdo4o8UZyvk0,1979
-uav_collision_avoidance/src/simulation/simulation_physics.py,sha256=9sfCvqk7_KZPSC7VIzeDEURiHJDA2b9dUefJRTx5rkU,8170
+uav_collision_avoidance/src/simulation/simulation_physics.py,sha256=I88UTBnPqwmrZ8aZ-uUftF-28_7P14Dff8IjoiepR_A,8359
 uav_collision_avoidance/src/simulation/simulation_render.py,sha256=_Mb1k6Y1mRHtejgWByU-MmAIx4cSmwVBtaBqao0nrLk,1041
 uav_collision_avoidance/src/simulation/simulation_settings.py,sha256=gL0BI6DecE8MYBNex8-KMgNVqpUWuFoOo65chOypXi0,682
 uav_collision_avoidance/src/simulation/simulation_state.py,sha256=TI-8V3DznKtmewZWuHKGYIzzZmAolaj89bPGdO1VyIg,6343
 uav_collision_avoidance/src/simulation/simulation_widget.py,sha256=BcH_2wSJsC_6ind9wDG7OGbciKPiQirR4WxPVdSUWsk,26085
-uav_collision_avoidance-0.6.3.dist-info/LICENSE,sha256=VCiagDkTdM8_xItFjcyMl-mMsGbzL1CQEXpynU0QLxY,1075
-uav_collision_avoidance-0.6.3.dist-info/METADATA,sha256=CagmsKEd9QtcN20luW4LrCO8A7m38ssURRhBbfBgAak,7374
-uav_collision_avoidance-0.6.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-uav_collision_avoidance-0.6.3.dist-info/entry_points.txt,sha256=fcy0NnMoUjf7wZty5G169lvrCzHpWtJXyQuYsEGyg3k,73
-uav_collision_avoidance-0.6.3.dist-info/top_level.txt,sha256=miPZH4d_mAR-Tj76v8c0YFs_CNl1TTT4Yf7zwcPSuwY,58
-uav_collision_avoidance-0.6.3.dist-info/RECORD,,
+uav_collision_avoidance-0.6.4.dist-info/LICENSE,sha256=VCiagDkTdM8_xItFjcyMl-mMsGbzL1CQEXpynU0QLxY,1075
+uav_collision_avoidance-0.6.4.dist-info/METADATA,sha256=rXTCMrVyaaUh05zJSDcw0LYyHz0GCJ0-ZNR5t3HMf5s,7374
+uav_collision_avoidance-0.6.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+uav_collision_avoidance-0.6.4.dist-info/entry_points.txt,sha256=fcy0NnMoUjf7wZty5G169lvrCzHpWtJXyQuYsEGyg3k,73
+uav_collision_avoidance-0.6.4.dist-info/top_level.txt,sha256=miPZH4d_mAR-Tj76v8c0YFs_CNl1TTT4Yf7zwcPSuwY,58
+uav_collision_avoidance-0.6.4.dist-info/RECORD,,
```


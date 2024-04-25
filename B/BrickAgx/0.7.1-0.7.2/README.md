# Comparing `tmp/brickagx-0.7.1-cp39-cp39-win_amd64.whl.zip` & `tmp/brickagx-0.7.2-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 8657348 bytes, number of entries: 35
+Zip file size: 8657373 bytes, number of entries: 35
 -rw-r--r--  2.0 fat     1458 b- defN 80-Jan-01 00:00 rebrick/__init__.py
 -rw-r--r--  2.0 fat  5401600 b- defN 80-Jan-01 00:00 rebrick/_BrickAgxPyApi.cp39-win_amd64.pyd
 -rw-r--r--  2.0 fat  1504768 b- defN 80-Jan-01 00:00 rebrick/_CorePythonSwig.cp39-win_amd64.pyd
 -rw-r--r--  2.0 fat  2526208 b- defN 80-Jan-01 00:00 rebrick/_DriveTrainSwig.cp39-win_amd64.pyd
 -rw-r--r--  2.0 fat  1246208 b- defN 80-Jan-01 00:00 rebrick/_MathSwig.cp39-win_amd64.pyd
 -rw-r--r--  2.0 fat  2137600 b- defN 80-Jan-01 00:00 rebrick/_Physics1DSwig.cp39-win_amd64.pyd
 -rw-r--r--  2.0 fat 11220480 b- defN 80-Jan-01 00:00 rebrick/_Physics3DSwig.cp39-win_amd64.pyd
@@ -26,12 +26,12 @@
 -rw-r--r--  2.0 fat  2295209 b- defN 80-Jan-01 00:00 rebrick/Physics3D.py
 -rw-r--r--  2.0 fat   938547 b- defN 80-Jan-01 00:00 rebrick/Robotics.py
 -rw-r--r--  2.0 fat    46727 b- defN 80-Jan-01 00:00 rebrick/Simulation.py
 -rw-r--r--  2.0 fat    41484 b- defN 80-Jan-01 00:00 rebrick/Terrain.py
 -rw-r--r--  2.0 fat    23897 b- defN 80-Jan-01 00:00 rebrick/Urdf.py
 -rw-r--r--  2.0 fat   451249 b- defN 80-Jan-01 00:00 rebrick/Vehicles.py
 -rw-r--r--  2.0 fat   146491 b- defN 80-Jan-01 00:00 rebrick/Visuals.py
--rw-r--r--  2.0 fat      159 b- defN 80-Jan-01 00:00 brickagx-0.7.1.dist-info/entry_points.txt
--rw-r--r--  2.0 fat     7834 b- defN 80-Jan-01 00:00 brickagx-0.7.1.dist-info/METADATA
--rw-r--r--  2.0 fat       96 b- defN 80-Jan-01 00:00 brickagx-0.7.1.dist-info/WHEEL
-?rw-r--r--  2.0 fat     2989 b- defN 16-Jan-01 00:00 brickagx-0.7.1.dist-info/RECORD
-35 files, 48987653 bytes uncompressed, 8652684 bytes compressed:  82.3%
+-rw-r--r--  2.0 fat      159 b- defN 80-Jan-01 00:00 brickagx-0.7.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 fat     7834 b- defN 80-Jan-01 00:00 brickagx-0.7.2.dist-info/METADATA
+-rw-r--r--  2.0 fat       96 b- defN 80-Jan-01 00:00 brickagx-0.7.2.dist-info/WHEEL
+?rw-r--r--  2.0 fat     2989 b- defN 16-Jan-01 00:00 brickagx-0.7.2.dist-info/RECORD
+35 files, 48987653 bytes uncompressed, 8652709 bytes compressed:  82.3%
```

## zipnote {}

```diff
@@ -87,20 +87,20 @@
 
 Filename: rebrick/Vehicles.py
 Comment: 
 
 Filename: rebrick/Visuals.py
 Comment: 
 
-Filename: brickagx-0.7.1.dist-info/entry_points.txt
+Filename: brickagx-0.7.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: brickagx-0.7.1.dist-info/METADATA
+Filename: brickagx-0.7.2.dist-info/METADATA
 Comment: 
 
-Filename: brickagx-0.7.1.dist-info/WHEEL
+Filename: brickagx-0.7.2.dist-info/WHEEL
 Comment: 
 
-Filename: brickagx-0.7.1.dist-info/RECORD
+Filename: brickagx-0.7.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rebrick/__init__.py

```diff
@@ -1,10 +1,10 @@
 import os
 __AGXVERSION__ = "2.37.3.3"
-__version__ = "0.7.1"
+__version__ = "0.7.2"
 try:
     import agx
     if agx.__version__ != __AGXVERSION__:
         print(f"This version of brickagx is compiled for AGX {__AGXVERSION__} only and may crash with your {agx.__version__} version, upgrade brickagx or AGX to make sure the versions are suited for eachother")
 except:
     print("Failed finding AGX Dynamics, have you run setup_env?")
     exit(255)
```

## Comparing `brickagx-0.7.1.dist-info/METADATA` & `brickagx-0.7.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BrickAgx
-Version: 0.7.1
+Version: 0.7.2
 Summary: Brick.AGX python interface development
 Home-page: https://pub.algoryx.dev/brick/
 License: Apache 2.0
 Author: Algoryx
 Author-email: algoryx@algoryx.com
 Requires-Python: >=3.8
 Classifier: Intended Audience :: Manufacturing
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Dist: agx (==2.37.3.3)
-Requires-Dist: brickbundles (>=0.7.1,<0.8.0)
+Requires-Dist: brickbundles (>=0.7.2,<0.8.0)
 Requires-Dist: pclick (>=0.3.1,<0.4.0)
 Description-Content-Type: text/markdown
 
 # BRICK AGX
 
 The brickagx package implements all Brick bundles such as Physics, Robotics, DriveTrain and Simulation using [AGX Dynamics Real-time multi-body simulation](https://www.algoryx.se/agx-dynamics/).
 The package contains python bindings and native libraries needed to load and run .brick files.
```

## Comparing `brickagx-0.7.1.dist-info/RECORD` & `brickagx-0.7.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-rebrick/__init__.py,sha256=AUp_VrOffpu01syZ7V6SWRTIJzWfK2mPlNnlqbyzZxw,1458
-rebrick/_BrickAgxPyApi.cp39-win_amd64.pyd,sha256=iyVHfh0bw4DS-uGmIM7wXX92bco9OJHaN4CWAEhIXPI,5401600
-rebrick/_CorePythonSwig.cp39-win_amd64.pyd,sha256=TRYlnaKi3vpjx-DDyTmazSahNqAdwSKFGPaFcefbjRQ,1504768
-rebrick/_DriveTrainSwig.cp39-win_amd64.pyd,sha256=GrudLvr0YeehJGAK9K8JukEFM0ge38TkeBEIfw_ylrc,2526208
-rebrick/_MathSwig.cp39-win_amd64.pyd,sha256=4rAIWzETk_zoC2K2SAPlrUweUrFfDGfIPcCRPijkfjU,1246208
-rebrick/_Physics1DSwig.cp39-win_amd64.pyd,sha256=JQFA06WKcgOhffj6BUFDMKPCogrR3o2mbaIgAAEF1Zg,2137600
-rebrick/_Physics3DSwig.cp39-win_amd64.pyd,sha256=c_RiQiFR-iFF53w3PJTFLw2CnfW8hzibdQ4jLT_VeoQ,11220480
-rebrick/_PhysicsSwig.cp39-win_amd64.pyd,sha256=rx5MdjFpryDRSh8c3lRoZu99SnB9RIOJsiP8mB4B5iM,7019008
-rebrick/_RoboticsSwig.cp39-win_amd64.pyd,sha256=xDowL5n5r9lvyxfTi2M_371Ns--Pm7GU8g-F3pQMTyQ,5448192
-rebrick/_SimulationSwig.cp39-win_amd64.pyd,sha256=-MmUYYxRhuMxYspoNx8PK-jzHMMtoB9E7TDnc9gKQlU,704512
-rebrick/_TerrainSwig.cp39-win_amd64.pyd,sha256=Td7mxxdI20UIlYJ_hMCsnta97Q3AapUuXv8Tyns7kT0,728576
-rebrick/_UrdfSwig.cp39-win_amd64.pyd,sha256=KFx9k866vp8OhzEdWhVQYth63oo3s_7IkRn_vdxEXDo,631296
-rebrick/_VehiclesSwig.cp39-win_amd64.pyd,sha256=LagPUo82K8G5PzJNmIgRFKZN9Q3acCl3Z4LWk7a8Zw4,2861568
-rebrick/_VisualsSwig.cp39-win_amd64.pyd,sha256=5kYkiuwLKmIyhWUtA7jitgLFHtKVDD4jF08sNWCxOZM,997376
+rebrick/__init__.py,sha256=XwODHVKXS_08c1puu_5MVSKmlzF4agfUtqmOwTvFEts,1458
+rebrick/_BrickAgxPyApi.cp39-win_amd64.pyd,sha256=zjebrabWWpZ97ztOtngoCKIOdOzBuzaiRlvuI4pVyQ8,5401600
+rebrick/_CorePythonSwig.cp39-win_amd64.pyd,sha256=c2UFt5l2MO5Hu6dxzZbYMaiixaBK9C045agX6TL1KIw,1504768
+rebrick/_DriveTrainSwig.cp39-win_amd64.pyd,sha256=vvUVZwj9zP5hAELjuKvBux4NjiAMZIspY2Z3Zx8krkE,2526208
+rebrick/_MathSwig.cp39-win_amd64.pyd,sha256=U6Bh4ZYDqPQCr9Mp2XfPCuhdBOhqho-SkfV0rOoLpAI,1246208
+rebrick/_Physics1DSwig.cp39-win_amd64.pyd,sha256=gm__ge2caC_t5NeARim9InCMjl_vUjhFZuHhw_AOhCE,2137600
+rebrick/_Physics3DSwig.cp39-win_amd64.pyd,sha256=dlxbF0DJBVylp_6dshsUKuQ-qqd-b1O7kVtmMc9DKWQ,11220480
+rebrick/_PhysicsSwig.cp39-win_amd64.pyd,sha256=08IQOMKDBFJRXITwAGAwGbiMbyRQ7dC4o9ocyHNijVE,7019008
+rebrick/_RoboticsSwig.cp39-win_amd64.pyd,sha256=WTliZPZkSWqU3RJIDTtqmaEFeuI9G5mJ8P2TgruXW3k,5448192
+rebrick/_SimulationSwig.cp39-win_amd64.pyd,sha256=SW6nrQgY-vlCefb_WFVrnYBUq8cM02wfmO1GOxcIdSw,704512
+rebrick/_TerrainSwig.cp39-win_amd64.pyd,sha256=_V-E9b2Z-cwMG1PnxT14kcJRa_lgkEvEsGy8sBTUmeo,728576
+rebrick/_UrdfSwig.cp39-win_amd64.pyd,sha256=niWTk9WQpb4Kzl9h99cvaAePjJj3BguTKNIap_YpsQU,631296
+rebrick/_VehiclesSwig.cp39-win_amd64.pyd,sha256=FS5S4SymGKNozFH_GRhkF44At6tXNzAaYtX9meqMdYo,2861568
+rebrick/_VisualsSwig.cp39-win_amd64.pyd,sha256=hF7xyc1GxaO3uvKLTC_aZpiucPOlEQFMY6IbM1tQNpk,997376
 rebrick/agxtobrick.py,sha256=ww7fV5G2M5gABgE8jdaUdDqxKT9VhBAnRSzUOGFRLM4,2212
 rebrick/anytobrick.py,sha256=mZ8zVvHTRjgg-dMriwsSAunH6rfc3FYKvKdW2CvA8f4,2264
 rebrick/api.py,sha256=kU9C1KXK0PYEB4dono8xzcRhmdVTu7lFOTDJd-Zx2ok,39869
 rebrick/brickvalidate.py,sha256=mDRvBgYbQGiuh_YW4mxcCMg4nuAuo8Wb1lOwuvdf_wo,2013
 rebrick/brickview.py,sha256=PV-9zQnyUe_1CYOLe_bpX_xUtDlX9vlk3lRBlvNbSSU,5270
 rebrick/Core.py,sha256=HG5JzjuU75zRkbQoxnjDLpVHP6-QJplcP-UHZ4ybrn4,133079
 rebrick/DriveTrain.py,sha256=WTnbCvIVDErntjw-GqO4og2CsIm7jBu99hzB8bMKhgc,414656
@@ -25,11 +25,11 @@
 rebrick/Physics3D.py,sha256=FVduDB1lg3a7fepgRDO6lpaZXHGyhYGHXCZUpa0ZD-w,2295209
 rebrick/Robotics.py,sha256=94JwLNEF0sqjy2FWp-6Qui_O3dAMPuIwbBHVyVJn9nY,938547
 rebrick/Simulation.py,sha256=W613zVuHLbrwPeXjEttuOkyNShpD87qLnFL_Ufb2gE4,46727
 rebrick/Terrain.py,sha256=dO2rCRzw3F69T0-zF4zfbe4VE9yToiyeIkitwy7UIkY,41484
 rebrick/Urdf.py,sha256=Ze5Cq7gYUOclnhJoYP_h1owN4hJLONLWZmDXJ_k_o2g,23897
 rebrick/Vehicles.py,sha256=WTDFgjBU90y5wtj9oR4Obujnb4H1fc0kup9pYNJ6_XM,451249
 rebrick/Visuals.py,sha256=bDAB3cMVA4otGy1XZRreOW_u6g5LwAFxVhT1rDiVeqQ,146491
-brickagx-0.7.1.dist-info/entry_points.txt,sha256=8dPzLXD5RkYUaPkiAcnDTgJ0LO8XkcKz5bP51VVPIjs,159
-brickagx-0.7.1.dist-info/METADATA,sha256=kDS_Jqma4G9Y8HEuf6uRhHY31tV9GPTdXI3pQQziE1k,7834
-brickagx-0.7.1.dist-info/WHEEL,sha256=T7hzPzFWHJiWCVylm2UCj5payilA7ulisMC0IiBEe3o,96
-brickagx-0.7.1.dist-info/RECORD,,
+brickagx-0.7.2.dist-info/entry_points.txt,sha256=8dPzLXD5RkYUaPkiAcnDTgJ0LO8XkcKz5bP51VVPIjs,159
+brickagx-0.7.2.dist-info/METADATA,sha256=-5OezM3me2eMBP4RmN1XCx_JMtVfudpxT_9KGh7yBMk,7834
+brickagx-0.7.2.dist-info/WHEEL,sha256=T7hzPzFWHJiWCVylm2UCj5payilA7ulisMC0IiBEe3o,96
+brickagx-0.7.2.dist-info/RECORD,,
```


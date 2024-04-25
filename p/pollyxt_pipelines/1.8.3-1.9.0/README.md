# Comparing `tmp/pollyxt_pipelines-1.8.3.tar.gz` & `tmp/pollyxt_pipelines-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pollyxt_pipelines-1.8.3.tar", max compression
+gzip compressed data, was "pollyxt_pipelines-1.9.0.tar", max compression
```

## Comparing `pollyxt_pipelines-1.8.3.tar` & `pollyxt_pipelines-1.9.0.tar`

### file list

```diff
@@ -1,25 +1,29 @@
--rw-r--r--   0        0        0     1717 2021-10-14 13:06:26.743280 pollyxt_pipelines-1.8.3/pollyxt_pipelines/__init__.py
--rw-r--r--   0        0        0       51 2021-10-14 13:06:26.743280 pollyxt_pipelines-1.8.3/pollyxt_pipelines/__main__.py
--rw-r--r--   0        0        0     3133 2021-10-14 13:06:26.743280 pollyxt_pipelines-1.8.3/pollyxt_pipelines/config.py
--rw-r--r--   0        0        0      238 2021-10-14 13:06:26.743280 pollyxt_pipelines-1.8.3/pollyxt_pipelines/console.py
--rw-r--r--   0        0        0     7565 2021-10-14 13:06:26.743280 pollyxt_pipelines-1.8.3/pollyxt_pipelines/locations/__init__.py
--rw-r--r--   0        0        0     1241 2021-10-14 13:06:26.747280 pollyxt_pipelines-1.8.3/pollyxt_pipelines/locations/commands.py
--rw-r--r--   0        0        0     1355 2021-10-14 13:06:26.747280 pollyxt_pipelines-1.8.3/pollyxt_pipelines/locations/locations.ini
--rw-r--r--   0        0        0     7300 2021-10-14 13:06:26.747280 pollyxt_pipelines-1.8.3/pollyxt_pipelines/polly_to_scc/commands.py
--rw-r--r--   0        0        0     1541 2021-10-14 13:06:26.747280 pollyxt_pipelines-1.8.3/pollyxt_pipelines/polly_to_scc/exceptions.py
--rw-r--r--   0        0        0     9381 2021-10-14 13:06:26.747280 pollyxt_pipelines-1.8.3/pollyxt_pipelines/polly_to_scc/pollyxt.py
--rw-r--r--   0        0        0    17957 2021-10-14 13:06:26.747280 pollyxt_pipelines-1.8.3/pollyxt_pipelines/polly_to_scc/scc_netcdf.py
--rw-r--r--   0        0        0     2926 2021-10-14 13:06:26.747280 pollyxt_pipelines-1.8.3/pollyxt_pipelines/radiosondes/__init__.py
--rw-r--r--   0        0        0     2865 2021-10-14 13:06:26.747280 pollyxt_pipelines-1.8.3/pollyxt_pipelines/radiosondes/commands.py
--rw-r--r--   0        0        0     1393 2021-10-14 13:06:26.747280 pollyxt_pipelines-1.8.3/pollyxt_pipelines/radiosondes/exceptions.py
--rw-r--r--   0        0        0     3726 2021-10-14 13:06:26.747280 pollyxt_pipelines-1.8.3/pollyxt_pipelines/radiosondes/noa_wrf.py
--rw-r--r--   0        0        0    16770 2021-10-14 13:06:26.747280 pollyxt_pipelines-1.8.3/pollyxt_pipelines/scc_access/__init__.py
--rw-r--r--   0        0        0    25652 2021-10-14 13:06:26.747280 pollyxt_pipelines-1.8.3/pollyxt_pipelines/scc_access/commands.py
--rw-r--r--   0        0        0     2061 2021-10-14 13:06:26.747280 pollyxt_pipelines-1.8.3/pollyxt_pipelines/scc_access/constants.py
--rw-r--r--   0        0        0     1590 2021-10-14 13:06:26.747280 pollyxt_pipelines-1.8.3/pollyxt_pipelines/scc_access/exceptions.py
--rw-r--r--   0        0        0     8054 2021-10-14 13:06:26.747280 pollyxt_pipelines-1.8.3/pollyxt_pipelines/scc_access/types.py
--rw-r--r--   0        0        0     2801 2021-10-14 13:06:26.747280 pollyxt_pipelines-1.8.3/pollyxt_pipelines/test_utils.py
--rw-r--r--   0        0        0     3977 2021-10-14 13:06:26.747280 pollyxt_pipelines-1.8.3/pollyxt_pipelines/utils.py
--rw-r--r--   0        0        0      843 2021-10-14 13:06:26.747280 pollyxt_pipelines-1.8.3/pyproject.toml
--rw-r--r--   0        0        0     1088 2021-10-14 13:07:37.061648 pollyxt_pipelines-1.8.3/setup.py
--rw-r--r--   0        0        0      707 2021-10-14 13:07:37.061993 pollyxt_pipelines-1.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1870 2021-11-22 11:51:53.370072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/__init__.py
+-rw-r--r--   0        0        0       51 2021-11-22 11:51:53.370072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/__main__.py
+-rw-r--r--   0        0        0     3171 2021-11-22 11:51:53.370072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/config.py
+-rw-r--r--   0        0        0      238 2021-11-22 11:51:53.370072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/console.py
+-rw-r--r--   0        0        0     8309 2021-11-22 11:51:53.370072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/locations/__init__.py
+-rw-r--r--   0        0        0     1241 2021-11-22 11:51:53.370072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/locations/commands.py
+-rw-r--r--   0        0        0     1507 2021-11-22 11:51:53.370072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/locations/locations.ini
+-rw-r--r--   0        0        0     7681 2021-11-22 11:51:53.370072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/polly_to_scc/commands.py
+-rw-r--r--   0        0        0     1517 2021-11-22 11:51:53.370072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/polly_to_scc/exceptions.py
+-rw-r--r--   0        0        0    11261 2021-11-22 11:51:53.370072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/polly_to_scc/pollyxt.py
+-rw-r--r--   0        0        0    17416 2021-11-22 11:51:53.370072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/polly_to_scc/scc_netcdf.py
+-rw-r--r--   0        0        0     1248 2021-11-22 11:51:53.370072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/polly_to_scc/test_pollyxt.py
+-rw-r--r--   0        0        0     2255 2021-11-22 11:51:53.370072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/qc_eldec/commands.py
+-rw-r--r--   0        0        0     1671 2021-11-22 11:51:53.370072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/qc_eldec/constants.py
+-rw-r--r--   0        0        0    18550 2021-11-22 11:51:53.370072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/qc_eldec/qc_eldec_file.py
+-rw-r--r--   0        0        0     2926 2021-11-22 11:51:53.370072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/radiosondes/__init__.py
+-rw-r--r--   0        0        0     2925 2021-11-22 11:51:53.370072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/radiosondes/commands.py
+-rw-r--r--   0        0        0     1393 2021-11-22 11:51:53.370072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/radiosondes/exceptions.py
+-rw-r--r--   0        0        0     3801 2021-11-22 11:51:53.370072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/radiosondes/noa_wrf.py
+-rw-r--r--   0        0        0    17150 2021-11-22 11:51:53.374072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/scc_access/__init__.py
+-rw-r--r--   0        0        0    26396 2021-11-22 11:51:53.374072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/scc_access/commands.py
+-rw-r--r--   0        0        0     2085 2021-11-22 11:51:53.374072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/scc_access/constants.py
+-rw-r--r--   0        0        0     1590 2021-11-22 11:51:53.374072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/scc_access/exceptions.py
+-rw-r--r--   0        0        0     8204 2021-11-22 11:51:53.374072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/scc_access/types.py
+-rw-r--r--   0        0        0     2843 2021-11-22 11:51:53.374072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/test_utils.py
+-rw-r--r--   0        0        0     3992 2021-11-22 11:51:53.374072 pollyxt_pipelines-1.9.0/pollyxt_pipelines/utils.py
+-rw-r--r--   0        0        0      873 2021-11-22 11:51:53.374072 pollyxt_pipelines-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1151 2021-11-22 11:53:04.279890 pollyxt_pipelines-1.9.0/setup.py
+-rw-r--r--   0        0        0      753 2021-11-22 11:53:04.280261 pollyxt_pipelines-1.9.0/PKG-INFO
```

### Comparing `pollyxt_pipelines-1.8.3/pollyxt_pipelines/__init__.py` & `pollyxt_pipelines-1.9.0/pollyxt_pipelines/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     RerunSCC,
     SearchDownloadSCC,
     SearchSCC,
     UploadFiles,
     LidarConstantsSCC,
 )
 from pollyxt_pipelines.locations.commands import LocationPath, ShowLocations
+from pollyxt_pipelines.qc_eldec.commands import QCEldec, QCEldecDeleteHistory
 
 
 def get_package_version():
     """
     Returns the package version. If the package is not installed, it will
     return "Development Version".
     """
@@ -50,14 +51,16 @@
     application.add(DeleteSCC())
     application.add(RerunSCC())
     application.add(SearchSCC())
     application.add(SearchDownloadSCC())
     application.add(LidarConstantsSCC())
     application.add(ShowLocations())
     application.add(LocationPath())
+    application.add(QCEldec())
+    application.add(QCEldecDeleteHistory())
 
     return application
 
 
 def main():
     app = prepare_cli_application()
     app.run()
```

### Comparing `pollyxt_pipelines-1.8.3/pollyxt_pipelines/config.py` & `pollyxt_pipelines-1.9.0/pollyxt_pipelines/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,15 +86,17 @@
         config = Config()
         if value is None:
             # Read variable
             try:
                 value = config[group][name]
                 console.print(value)
             except KeyError:
-                console.print(f"[error]No config value with name[/error] {group}.{name}")
+                console.print(
+                    f"[error]No config value with name[/error] {group}.{name}"
+                )
                 console.print("Did you forget to define it?")
                 return 1
         else:
             config[group][name] = value
             config.write()
 
         return 0
```

### Comparing `pollyxt_pipelines-1.8.3/pollyxt_pipelines/locations/__init__.py` & `pollyxt_pipelines-1.9.0/pollyxt_pipelines/locations/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,14 +46,20 @@
 
     daytime_configuration: int
     """SCC Lidar Configuration ID - Daytime"""
 
     nighttime_configuration: int
     """SCC Lidar Configuration ID - Nightime"""
 
+    calibration_configuration_355nm: int
+    """SCC Lidar Configuration ID - Calibration (355 nm)"""
+
+    calibration_configuration_532nm: int
+    """SCC Lidar Configuration ID - Calibration (532 nm)"""
+
     channel_id: List[int]
     """List of channel IDs (for SCC `channel_ID` variable)"""
 
     background_low: List[int]
     """Value for the `Background_Low` variable"""
 
     background_high: List[int]
@@ -108,44 +114,54 @@
         table.add_column("Value")
 
         table.add_row("scc_code", self.scc_code)
         table.add_row("lat", str(self.lat))
         table.add_row("lon", str(self.lon))
         table.add_row("daytime_configuration", str(self.daytime_configuration))
         table.add_row("nighttime_configuration", str(self.nighttime_configuration))
+        table.add_row(
+            "calibration_configuration_355nm", str(self.calibration_configuration_355nm)
+        )
+        table.add_row(
+            "calibration_configuration_532nm", str(self.calibration_configuration_532nm)
+        )
         table.add_row("channel_id", ints_to_csv(self.channel_id))
         table.add_row("background_low", ints_to_csv(self.background_low))
         table.add_row("background_high", ints_to_csv(self.background_high))
         table.add_row("lr_input", ints_to_csv(self.lr_input))
         table.add_row("temperature", str(self.temperature))
         table.add_row("altitude_asl", str(self.altitude_asl))
         table.add_row("total_channel_355_nm", str(self.total_channel_355_nm))
         table.add_row("cross_channel_355_nm", str(self.cross_channel_355_nm))
         table.add_row("total_channel_532_nm", str(self.total_channel_532_nm))
         table.add_row("cross_channel_532_nm", str(self.cross_channel_532_nm))
         table.add_row(
-            "calibration_355nm_channel_ids", ints_to_csv(self.calibration_355nm_channel_ids)
+            "calibration_355nm_channel_ids",
+            ints_to_csv(self.calibration_355nm_channel_ids),
         )
         table.add_row(
-            "calibration_532nm_channel_ids", ints_to_csv(self.calibration_532nm_channel_ids)
+            "calibration_532nm_channel_ids",
+            ints_to_csv(self.calibration_532nm_channel_ids),
         )
         table.add_row("profile_name", self.profile_name)
         table.add_row("sounding_provider", self.sounding_provider)
 
         console.print(table)
 
 
 def location_from_section(name: str, section: SectionProxy) -> Location:
     """
     Create a Location from a ConfigParser Section (SectionProxy)
     """
 
     channel_id = [int(x.strip()) for x in section.get("channel_id").split(",")]
     background_low = [int(x.strip()) for x in section.get("background_low").split(",")]
-    background_high = [int(x.strip()) for x in section.get("background_high").split(",")]
+    background_high = [
+        int(x.strip()) for x in section.get("background_high").split(",")
+    ]
     lr_input = [int(x.strip()) for x in section.get("lr_input").split(",")]
 
     calibration_355nm_channel_ids = [
         int(x.strip()) for x in section.get("calibration_355nm_channel_ids").split(",")
     ]
     calibration_532nm_channel_ids = [
         int(x.strip()) for x in section.get("calibration_532nm_channel_ids").split(",")
@@ -155,14 +171,20 @@
         name=name,
         scc_code=section["scc_code"],
         lat=section.getfloat("lat"),
         lon=section.getfloat("lon"),
         altitude_asl=section.getfloat("altitude_asl"),
         daytime_configuration=section.getint("daytime_configuration"),
         nighttime_configuration=section.getint("nighttime_configuration"),
+        calibration_configuration_355nm=section.getint(
+            "calibration_configuration_355nm"
+        ),
+        calibration_configuration_532nm=section.getint(
+            "calibration_configuration_532nm"
+        ),
         channel_id=channel_id,
         background_low=background_low,
         background_high=background_high,
         lr_input=lr_input,
         temperature=section.getint("temperature"),
         pressure=section.getint("pressure"),
         total_channel_355_nm=section.getint("total_channel_355_nm"),
@@ -180,15 +202,17 @@
     """
     Reads all built-in and custom locations into a dictionary: name -> Location
     """
 
     locations = {}
 
     # Read built-in locations
-    locations_buffer = io.StringIO(read_text("pollyxt_pipelines.locations", "locations.ini"))
+    locations_buffer = io.StringIO(
+        read_text("pollyxt_pipelines.locations", "locations.ini")
+    )
     locations_config = ConfigParser()
     locations_config.read_file(locations_buffer)
 
     for name in locations_config.sections():
         section = locations_config[name]
         locations[name] = location_from_section(name, section)
 
@@ -220,12 +244,14 @@
 
 
 def unknown_location_error(name: str):
     """
     Prints an error message that the given location is not found, along with a
     list of known locations
     """
-    error = f"[error]Could not find location[/error]{name}[error]\nKnown locations:\n\n."
+    error = (
+        f"[error]Could not find location[/error]{name}[error]\nKnown locations:\n\n."
+    )
     for l in LOCATIONS:
         error += f"* {l.name}"
 
     console.print(Markdown(error))
```

### Comparing `pollyxt_pipelines-1.8.3/pollyxt_pipelines/locations/commands.py` & `pollyxt_pipelines-1.9.0/pollyxt_pipelines/locations/commands.py`

 * *Files identical despite different names*

### Comparing `pollyxt_pipelines-1.8.3/pollyxt_pipelines/locations/locations.ini` & `pollyxt_pipelines-1.9.0/pollyxt_pipelines/locations/locations.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [Antikythera]
 scc_code = aky
 lat = 23.3100
 lon = 35.8600
 altitude_asl = 0.1
 daytime_configuration = 437
 nighttime_configuration = 438
+calibration_configuration_355nm = 461
+calibration_configuration_532nm = 462
 channel_id = 493, 500, 497, 499, 494, 496, 498, 495, 501, 941, 940, 502
 background_low = 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0
 background_high = 249, 249, 249, 249, 249, 249, 249, 249, 249, 249, 249, 249
 lr_input = 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1
 temperature = 20
 pressure = 1008
 total_channel_355_nm = 0
@@ -24,14 +26,16 @@
 [Finokalia]
 scc_code = fik
 lat = 25.6698
 lon = 35.3377
 altitude_asl = 0.1
 daytime_configuration = 186
 nighttime_configuration = 302
+calibration_configuration_355nm = 461
+calibration_configuration_532nm = 462
 channel_id = 493, 500, 497, 499, 494, 496, 498, 495, 501, 941, 940, 502
 background_low = 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0
 background_high = 249, 249, 249, 249, 249, 249, 249, 249, 249, 249, 249, 249
 lr_input = 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1
 temperature = 20
 pressure = 1008
 total_channel_355_nm = 0
```

### Comparing `pollyxt_pipelines-1.8.3/pollyxt_pipelines/polly_to_scc/commands.py` & `pollyxt_pipelines-1.9.0/pollyxt_pipelines/polly_to_scc/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,29 +85,35 @@
             atmosphere = scc_netcdf.Atmosphere.from_string(atmosphere)
         if interval is None:
             interval = 60  # Default duration is 1 hour/60 minutes
         interval = timedelta(minutes=int(interval))
         start_time = self.option("start-time")
         end_time = self.option("end-time")
         if start_time is None and end_time is not None:
-            console.print("`--end-time` [error]can't be used without[/error] `--start-time`.")
+            console.print(
+                "`--end-time` [error]can't be used without[/error] `--start-time`."
+            )
             return 1
         system_id_day = self.option("system-id-day")
         if system_id_day is not None:
             try:
                 system_id_day = int(system_id_day)
             except ValueError:
-                console.print("[error]Value for system-id-day is not convertable to int![/error]")
+                console.print(
+                    "[error]Value for system-id-day is not convertable to int![/error]"
+                )
                 return 1
         system_id_night = self.option("system-id-night")
         if system_id_night is not None:
             try:
                 system_id_night = int(system_id_night)
             except ValueError:
-                console.print("[error]Value for system-id-night is not convertable to int![/error]")
+                console.print(
+                    "[error]Value for system-id-night is not convertable to int![/error]"
+                )
                 return 1
 
         # Try to get location
         location_name = self.argument("location")
         location = locations.LOCATIONS[location_name]
         if location is None:
             locations.unknown_location_error(location_name)
@@ -143,17 +149,22 @@
             atmosphere=atmosphere,
             start_time=start_time,
             end_time=end_time,
         )
         for id, path, timestamp_start, timestamp_end in converter:
             start_str = timestamp_start.strftime("%Y-%m-%d %H:%M")
             end_str = timestamp_end.strftime("%Y-%m-%d %H:%M")
-            console.print(
-                f"[info]Created file with measurement ID[/info] {id} [info]at[/info] {str(path)} [info]({start_str} - {end_str})[/info]"
-            )
+            if "calibration" in str(path):
+                console.print(
+                    f"[info]Created calibration file with measurement ID[/info] {id} [info]at[/info] {str(path)} [info]({start_str} - {end_str})[/info]"
+                )
+            else:
+                console.print(
+                    f"[info]Created file with measurement ID[/info] {id} [info]at[/info] {str(path)} [info]({start_str} - {end_str})[/info]"
+                )
 
             if atmosphere == scc_netcdf.Atmosphere.RADIOSONDE:
                 radiosondes.create_radiosonde_netcdf(
                     "wrf_noa",
                     location,
                     timestamp_start,
                     timestamp_start + interval,
```

### Comparing `pollyxt_pipelines-1.8.3/pollyxt_pipelines/polly_to_scc/exceptions.py` & `pollyxt_pipelines-1.9.0/pollyxt_pipelines/polly_to_scc/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,10 +49,8 @@
     def __init__(self, filename: str, value: Tuple[int, int]) -> None:
         super().__init__(filename, value)
 
         self.filename = filename
         self.value = value
 
     def __str__(self) -> str:
-        return (
-            f"Bad measurement time value was encountered in file {self.filename}: {str(self.value)}"
-        )
+        return f"Bad measurement time value was encountered in file {self.filename}: {str(self.value)}"
```

### Comparing `pollyxt_pipelines-1.8.3/pollyxt_pipelines/polly_to_scc/pollyxt.py` & `pollyxt_pipelines-1.9.0/pollyxt_pipelines/polly_to_scc/pollyxt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Routines related to PollyXT files
 """
 
 from pathlib import Path
-from typing import Tuple, Union
+from typing import Iterable, Tuple, Union
 from datetime import datetime, timedelta
 
 import numpy as np
 import pandas as pd
 from netCDF4 import Dataset
 
 from pollyxt_pipelines.polly_to_scc.exceptions import (
@@ -30,15 +30,17 @@
     day, seconds = timestamp
     day_str = str(day)
 
     date = datetime.strptime(day_str, "%Y%m%d")
     return date + timedelta(seconds=int(seconds))
 
 
-def get_measurement_period(input: Union[Path, Dataset, np.ndarray]) -> Tuple[datetime, datetime]:
+def get_measurement_period(
+    input: Union[Path, Dataset, np.ndarray]
+) -> Tuple[datetime, datetime]:
     """
     Return the measurement time (i.e. start and end times) from a PollyXT file.
 
     Parameters:
         input: Either a path to a PollyXT netCDF file, an opened netCDF dataset or the
             `measurement_time` variable.
 
@@ -125,63 +127,95 @@
         self.path = path
 
         if self.path.is_dir():
             self.files = list(self.path.glob("*.nc"))
         elif self.path.is_file():
             self.files = [self.path]
         else:
-            raise ValueError(f"Path {self.path} doesn't seem to be either a file or a directory")
+            raise ValueError(
+                f"Path {self.path} doesn't seem to be either a file or a directory"
+            )
 
         if len(self.files) == 0:
             raise NoFilesFound(self.path)
 
         # Create the index table
         rows = []
         for path in self.files:
             with Dataset(path, "r") as nc:
                 measurement_time = nc["measurement_time"][:]
-                for i, timestamp in enumerate(measurement_time):
+                depol_cal_angle = nc["depol_cal_angle"][:]
+                for i, (timestamp, dcv) in enumerate(
+                    zip(measurement_time, depol_cal_angle)
+                ):
                     # Parse date
                     try:
                         timestamp = polly_date_to_datetime(timestamp)
                     except ValueError:
                         raise BadMeasurementTime(path, timestamp)
 
-                    rows.append({"timestamp": timestamp, "index": i, "path": path})
+                    rows.append(
+                        {
+                            "timestamp": timestamp,
+                            "index": i,
+                            "path": path,
+                            "depol_cal_angle": dcv,
+                        }
+                    )
 
         self.index = pd.DataFrame(rows)
         self.index = self.index.sort_values("timestamp", ascending=True)
+        self.index["calibration"] = self.index["depol_cal_angle"] != 0
 
     def get_time_period(self) -> Tuple[datetime, datetime]:
         """
         Returns the time period available in this repository
 
         Returns:
             A tuple containing the first and last available timestamps
         """
 
         start = self.index.iloc[0]["timestamp"]
         end = self.index.iloc[-1]["timestamp"]
 
         return start, end
 
+    def get_calibration_periods(self) -> Iterable[Tuple[datetime, datetime]]:
+        """
+        Returns a list of periods that refer to calibration times.
+
+        This function checks when the `depol_cal_angle` variable is not 0 and returns
+        the time periods that this occures.
+
+        Returns:
+            List[Tuple[datetime, datetime]]: A list containing periods (ie. tuples of start-time and end-time)
+        """
+
+        groups = (self.index.calibration != self.index.calibration.shift()).cumsum()
+
+        for i, g in self.index.groupby(groups):
+            if g.depol_cal_angle.sum() != 0:
+                yield g.iloc[0]["timestamp"], g.iloc[-1]["timestamp"]
+
     def get_pollyxt_file(self, time_start: datetime, time_end: datetime):
         """
         Create a PollyXTFile for the given time range.
 
         Parameters:
             time_start: First measurement to include
             time_end: Last measurement to include
 
         Returns:
             The PollyXTFile file for the requested period.
         """
 
         # Filter index for given time range
-        mask = (self.index["timestamp"] >= time_start) & (self.index["timestamp"] <= time_end)
+        mask = (self.index["timestamp"] >= time_start) & (
+            self.index["timestamp"] <= time_end
+        )
         targets = self.index[mask]
         if targets.shape[0] == 0:
             raise NoMeasurementsInTimePeriod()
 
         # Read all files and concat into the requested
         polly_files = []
         for path in targets["path"].unique():
@@ -191,29 +225,52 @@
             end_index = targets_filtered["index"].max()
 
             polly_files.append(PollyXTFile(path, start=start_index, end=end_index))
 
         # Concatenate data into one file
         pollyxt_file = polly_files[0]
         pollyxt_file.raw_signal = np.concatenate([x.raw_signal for x in polly_files])
-        pollyxt_file.raw_signal_swap = np.concatenate([x.raw_signal_swap for x in polly_files])
-        pollyxt_file.measurement_time = np.concatenate([x.measurement_time for x in polly_files])
-        pollyxt_file.measurement_shots = np.concatenate([x.measurement_shots for x in polly_files])
+        pollyxt_file.raw_signal_swap = np.concatenate(
+            [x.raw_signal_swap for x in polly_files]
+        )
+        pollyxt_file.measurement_time = np.concatenate(
+            [x.measurement_time for x in polly_files]
+        )
+        pollyxt_file.measurement_shots = np.concatenate(
+            [x.measurement_shots for x in polly_files]
+        )
         try:
-            pollyxt_file.zenith_angle = np.concatenate([x.zenith_angle for x in polly_files])
+            pollyxt_file.zenith_angle = np.concatenate(
+                [x.zenith_angle for x in polly_files]
+            )
         except ValueError:
             # Sometimes these arrays are empty, this is not a problem
             pass
-        pollyxt_file.depol_cal_angle = np.concatenate([x.depol_cal_angle for x in polly_files])
+        pollyxt_file.depol_cal_angle = np.concatenate(
+            [x.depol_cal_angle for x in polly_files]
+        )
 
         pollyxt_file.end_date = polly_files[-1].end_date
 
         return pollyxt_file
 
 
+def make_nan_during_calibration(depol_cal_angle: np.ndarray, raw_signal: np.ndarray):
+    """
+    Given the depol_cal_angle and raw_signal arrays, set raw_signal to NaN during
+    calibrations. The raw_signal array is mutated.
+
+    Args:
+        depol_cal_angle: The depol_cal_angle array from a `PollyXTFile`
+        raw_signal: The raw_signal array from a `PollyXTFile`
+    """
+    depol_cal_time = depol_cal_angle != 0.0
+    raw_signal[depol_cal_time, :, :] = np.nan
+
+
 class PollyXTFile:
     """
     Reads the variables of interest from a PollyXT netCDF file.
     """
 
     start_date: datetime
     start_index: int
@@ -225,15 +282,17 @@
 
     measurement_time: np.ndarray
     measurement_shots: np.ndarray
     zenith_angle: np.ndarray
     location_coordinates: np.ndarray
     depol_cal_angle: np.ndarray
 
-    def __init__(self, input_path: Path, start: int = None, end: int = None, nan_calibration=True):
+    def __init__(
+        self, input_path: Path, start: int = None, end: int = None, nan_calibration=True
+    ):
         """
         Read a PollyXT netcdf file
 
         Parameters
             input_path: Which file to read
             start: Optionally, trim the file from this index
             end: Optionally, trim file until this index
@@ -249,28 +308,30 @@
             start = 0
         if end is None:
             end = self.measurement_time.shape[0]
 
         self.measurement_time = self.measurement_time[start : end + 1]
 
         # Read the rest of the variables
+        # raw_signal is converted to float64 for two reasons:
+        # 1. SCC requires it as float64
+        # 2. So we can set it to NaN during calibration
         self.raw_signal = nc["raw_signal"][start : end + 1, :, :]
+        self.raw_signal = np.array(self.raw_signal, dtype=np.float64)
         self.raw_signal_swap = np.swapaxes(self.raw_signal, 1, 2)
 
         self.measurement_shots = nc["measurement_shots"][start : end + 1, :]
         self.zenith_angle = nc["zenithangle"][:]
         self.location_coordinates = nc["location_coordinates"][:]
-        self.depol_cal_angle = nc["depol_cal_angle"][:]
+        self.depol_cal_angle = nc["depol_cal_angle"][start : end + 1]
 
         nc.close()
 
         # Optionally set calibration times to nan
         if nan_calibration:
-            depol_cal_time = np.where(self.depol_cal_angle != 0.0)[0]
-            if depol_cal_time.size != 0:
-                self.raw_signal[depol_cal_time[0] : depol_cal_time[-1], :, :] == np.nan
+            make_nan_during_calibration(self.depol_cal_angle, self.raw_signal)
 
         # Store some variables for easy access
         self.start_index = start
         self.end_index = end
         self.start_date = polly_date_to_datetime(self.measurement_time[0, :])
         self.end_date = polly_date_to_datetime(self.measurement_time[-1, :])
```

### Comparing `pollyxt_pipelines-1.8.3/pollyxt_pipelines/polly_to_scc/scc_netcdf.py` & `pollyxt_pipelines-1.9.0/pollyxt_pipelines/polly_to_scc/scc_netcdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 
 from netCDF4 import Dataset
 import numpy as np
 
 from pollyxt_pipelines.polly_to_scc import pollyxt
 from pollyxt_pipelines.locations import Location
 from pollyxt_pipelines import utils
-from pollyxt_pipelines.polly_to_scc.exceptions import NoMeasurementsInTimePeriod, TimeOutsideFile
+from pollyxt_pipelines.polly_to_scc.exceptions import (
+    NoMeasurementsInTimePeriod,
+    TimeOutsideFile,
+)
 
 
 class Wavelength(Enum):
     """Laser wavelength"""
 
     NM_355 = 355
     NM_532 = 532
@@ -44,35 +47,14 @@
             return Atmosphere.CLOUDNET
         if x == "standard":
             return Atmosphere.STANDARD_ATMOSPHERE
 
         raise ValueError(f"Unknown atmosphere {x}")
 
 
-"""When calibration takes place each day, in HH:MM-HH:MM format"""
-CALIBRATION_PERIODS = ["02:31-02:41", "17:31-17:41", "21:31-21:41"]
-
-
-def calibration_to_datetime(base: datetime, period: str) -> Tuple[datetime, datetime]:
-    """
-    Given a calibrarion period in HH:MM-HH:MM format (start-end), it converts it to a pair of `datetime`, the same day
-    as the given `base`.
-    """
-    base = base.replace(hour=0, minute=0, second=0)
-
-    start, end = period.split("-")
-    start = [int(x) for x in start.split(":")]
-    end = [int(x) for x in end.split(":")]
-
-    start = base + timedelta(hours=start[0], minutes=start[1])
-    end = base + timedelta(hours=end[0], minutes=end[1])
-
-    return start, end
-
-
 def create_scc_netcdf(
     pf: pollyxt.PollyXTFile,
     output_path: Path,
     location: Location,
     atmosphere=Atmosphere.STANDARD_ATMOSPHERE,
 ) -> Tuple[str, Path]:
     """
@@ -123,42 +105,52 @@
     # nc.Overlap_File_Name = 'ov_' + selected_start.strftime('%Y%m%daky%H') + '.nc'
 
     # Custom attribute for configuration ID
     # From 04:00 until 16:00 we use daytime configuration
     if pf.start_date.replace(
         hour=4, minute=0
     ) < pf.start_date and pf.start_date < pf.start_date.replace(hour=16, minute=0):
-        nc.NOAReACT_Configuration_ID = location.daytime_configuration
+        nc.X_PollyXTPipelines_Configuration_ID = location.daytime_configuration
     else:
-        nc.NOAReACT_Configuration_ID = location.nighttime_configuration
+        nc.X_PollyXTPipelines_Configuration_ID = location.nighttime_configuration
 
     # Create Variables. (mandatory)
     raw_data_start_time = nc.createVariable(
         "Raw_Data_Start_Time", "i4", dimensions=("time", "nb_of_time_scales"), zlib=True
     )
     raw_data_stop_time = nc.createVariable(
         "Raw_Data_Stop_Time", "i4", dimensions=("time", "nb_of_time_scales"), zlib=True
     )
     raw_lidar_data = nc.createVariable(
         "Raw_Lidar_Data", "f8", dimensions=("time", "channels", "points"), zlib=True
     )
-    channel_id = nc.createVariable("channel_ID", "i4", dimensions=("channels"), zlib=True)
-    id_timescale = nc.createVariable("id_timescale", "i4", dimensions=("channels"), zlib=True)
+    channel_id = nc.createVariable(
+        "channel_ID", "i4", dimensions=("channels"), zlib=True
+    )
+    id_timescale = nc.createVariable(
+        "id_timescale", "i4", dimensions=("channels"), zlib=True
+    )
     laser_pointing_angle = nc.createVariable(
         "Laser_Pointing_Angle", "f8", dimensions=("scan_angles"), zlib=True
     )
     laser_pointing_angle_of_profiles = nc.createVariable(
         "Laser_Pointing_Angle_of_Profiles",
         "i4",
         dimensions=("time", "nb_of_time_scales"),
         zlib=True,
     )
-    laser_shots = nc.createVariable("Laser_Shots", "i4", dimensions=("time", "channels"), zlib=True)
-    background_low = nc.createVariable("Background_Low", "f8", dimensions=("channels"), zlib=True)
-    background_high = nc.createVariable("Background_High", "f8", dimensions=("channels"), zlib=True)
+    laser_shots = nc.createVariable(
+        "Laser_Shots", "i4", dimensions=("time", "channels"), zlib=True
+    )
+    background_low = nc.createVariable(
+        "Background_Low", "f8", dimensions=("channels"), zlib=True
+    )
+    background_high = nc.createVariable(
+        "Background_High", "f8", dimensions=("channels"), zlib=True
+    )
     molecular_calc = nc.createVariable("Molecular_Calc", "i4", dimensions=(), zlib=True)
     nc.createVariable("Pol_Calib_Range_Min", "f8", dimensions=("channels"), zlib=True)
     nc.createVariable("Pol_Calib_Range_Max", "f8", dimensions=("channels"), zlib=True)
     pressure_at_lidar_station = nc.createVariable(
         "Pressure_at_Lidar_Station", "f8", dimensions=(), zlib=True
     )
     temperature_at_lidar_station = nc.createVariable(
@@ -252,28 +244,38 @@
     )
     raw_data_stop_time = nc.createVariable(
         "Raw_Data_Stop_Time", "i4", dimensions=("time", "nb_of_time_scales"), zlib=True
     )
     raw_lidar_data = nc.createVariable(
         "Raw_Lidar_Data", "f8", dimensions=("time", "channels", "points"), zlib=True
     )
-    channel_id = nc.createVariable("channel_ID", "i4", dimensions=("channels"), zlib=True)
-    id_timescale = nc.createVariable("id_timescale", "i4", dimensions=("channels"), zlib=True)
+    channel_id = nc.createVariable(
+        "channel_ID", "i4", dimensions=("channels"), zlib=True
+    )
+    id_timescale = nc.createVariable(
+        "id_timescale", "i4", dimensions=("channels"), zlib=True
+    )
     laser_pointing_angle = nc.createVariable(
         "Laser_Pointing_Angle", "f8", dimensions=("scan_angles"), zlib=True
     )
     laser_pointing_angle_of_profiles = nc.createVariable(
         "Laser_Pointing_Angle_of_Profiles",
         "i4",
         dimensions=("time", "nb_of_time_scales"),
         zlib=True,
     )
-    laser_shots = nc.createVariable("Laser_Shots", "i4", dimensions=("time", "channels"), zlib=True)
-    background_low = nc.createVariable("Background_Low", "f8", dimensions=("channels"), zlib=True)
-    background_high = nc.createVariable("Background_High", "f8", dimensions=("channels"), zlib=True)
+    laser_shots = nc.createVariable(
+        "Laser_Shots", "i4", dimensions=("time", "channels"), zlib=True
+    )
+    background_low = nc.createVariable(
+        "Background_Low", "f8", dimensions=("channels"), zlib=True
+    )
+    background_high = nc.createVariable(
+        "Background_High", "f8", dimensions=("channels"), zlib=True
+    )
     molecular_calc = nc.createVariable("Molecular_Calc", "i4", dimensions=(), zlib=True)
     pol_calib_range_min_var = nc.createVariable(
         "Pol_Calib_Range_Min", "f8", dimensions=("channels"), zlib=True
     )
     pol_calib_range_max_var = nc.createVariable(
         "Pol_Calib_Range_Max", "f8", dimensions=("channels"), zlib=True
     )
@@ -305,19 +307,25 @@
 
     # Define total and cross channels IDs from Polly
     if wavelength == Wavelength.NM_355:
         total_channel = location.total_channel_355_nm
         cross_channel = location.cross_channel_355_nm
         channel_id[:] = np.array(location.calibration_355nm_channel_ids)
         nc.Measurement_ID = measurement_id + "35"
+        nc.X_PollyXTPipelines_Configuration_ID = (
+            location.calibration_configuration_355nm
+        )
     elif wavelength == Wavelength.NM_532:
         total_channel = location.total_channel_532_nm
         cross_channel = location.cross_channel_532_nm
         channel_id[:] = np.array(location.calibration_532nm_channel_ids)
         nc.Measurement_ID = measurement_id + "53"
+        nc.X_PollyXTPipelines_Configuration_ID = (
+            location.calibration_configuration_532nm
+        )
     else:
         raise ValueError(f"Unknown wavelength {wavelength}")
 
     # Copy calibration cycles
     for meas_cycle in range(0, 3, 1):
         laser_shots[meas_cycle, :] = np.array([600, 600, 600, 600])
 
@@ -409,43 +417,37 @@
             interval_start = interval_start.replace(microsecond=0, second=0, minute=0)
 
         # Interval end
         interval_end = interval_start + interval
 
         # Open netCDF file and convert to SCC
         try:
-            pf = repo.get_pollyxt_file(interval_start, interval_end + timedelta(seconds=30))
+            pf = repo.get_pollyxt_file(
+                interval_start, interval_end + timedelta(seconds=30)
+            )
             id, path = create_scc_netcdf(pf, output_path, location, atmosphere)
 
             yield id, path, pf.start_date, pf.end_date
         except NoMeasurementsInTimePeriod as ex:
             # Go to next loop
             interval_start = interval_end
             continue
 
         # Set start of next interval to the end of this one
         interval_start = interval_end
 
     # Generate calibration files
-    # - 02:31 to 02:41
-    # - 17:31 to 17:41
-    # - 21:31 to 21:41
     if calibration:
         # Check for any valid calibration intervals
-        for period in CALIBRATION_PERIODS:
-            start, end = calibration_to_datetime(measurement_start, period)
-
+        for start, end in repo.get_calibration_periods():
             if start > measurement_start and end < measurement_end:
-                try:
-                    pf = repo.get_pollyxt_file(start, end)
+                pf = repo.get_pollyxt_file(start, end)
 
-                    id, path = create_scc_calibration_netcdf(
-                        pf, output_path, location, wavelength=Wavelength.NM_532
-                    )
-                    yield id, path, start, end
-
-                    id, path = create_scc_calibration_netcdf(
-                        pf, output_path, location, wavelength=Wavelength.NM_355
-                    )
-                    yield id, path, start, end
-                except NoMeasurementsInTimePeriod:
-                    pass
+                id, path = create_scc_calibration_netcdf(
+                    pf, output_path, location, wavelength=Wavelength.NM_532
+                )
+                yield id, path, start, end
+
+                id, path = create_scc_calibration_netcdf(
+                    pf, output_path, location, wavelength=Wavelength.NM_355
+                )
+                yield id, path, start, end
```

### Comparing `pollyxt_pipelines-1.8.3/pollyxt_pipelines/radiosondes/__init__.py` & `pollyxt_pipelines-1.9.0/pollyxt_pipelines/radiosondes/__init__.py`

 * *Files identical despite different names*

### Comparing `pollyxt_pipelines-1.8.3/pollyxt_pipelines/radiosondes/commands.py` & `pollyxt_pipelines-1.9.0/pollyxt_pipelines/radiosondes/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,17 @@
         {--to-scc= : Optionaly write the radiosonde data to a SCC-formatted netCDF file}
     """
 
     def handle(self):
         # Get requested provider
         provider = RadiosondeProviders.get(self.argument("provider"), None)
         if provider is None:
-            console.print(f"[error]Unknown provider[/error] {self.argument('provider')}")
+            console.print(
+                f"[error]Unknown provider[/error] {self.argument('provider')}"
+            )
             known_providers = "List of supported providers:\n\n"
             for key in RadiosondeProviders.keys():
                 known_providers += f"- {key}\n"
             console.print(Markdown(known_providers))
             return 1
 
         # Get location
@@ -69,9 +71,11 @@
         to_csv = self.option("to-csv")
         if to_csv is not None:
             console.print(f"[info]Writing profile as CSV file:[/info] {to_csv}")
             profile.to_csv(to_csv, index=False)
 
         to_scc = self.option("to-scc")
         if to_scc is not None:
-            console.print(f"[info]Writing profile as SCC radiosonde file:[/info] {to_scc}")
+            console.print(
+                f"[info]Writing profile as SCC radiosonde file:[/info] {to_scc}"
+            )
             write_radiosonde_netcdf(profile, location, profile_time, to_scc)
```

### Comparing `pollyxt_pipelines-1.8.3/pollyxt_pipelines/radiosondes/exceptions.py` & `pollyxt_pipelines-1.9.0/pollyxt_pipelines/radiosondes/exceptions.py`

 * *Files identical despite different names*

### Comparing `pollyxt_pipelines-1.8.3/pollyxt_pipelines/radiosondes/noa_wrf.py` & `pollyxt_pipelines-1.9.0/pollyxt_pipelines/radiosondes/noa_wrf.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,15 +49,17 @@
     """
 
     # Get radiosonde storage location
     try:
         config = Config()
         radiosonde_storage = config["wrf"]["path"]
     except KeyError:
-        raise ValueError(f"Config variable wrf.path is undefined. Can't locate radiosonde files")
+        raise ValueError(
+            f"Config variable wrf.path is undefined. Can't locate radiosonde files"
+        )
     radiosonde_storage = Path(radiosonde_storage)
 
     # Calculate file path
     filename = f'{location.upper()}_{date.strftime("%d%m%Y")}'
     file_path = radiosonde_storage / filename
 
     return file_path
@@ -90,23 +92,30 @@
     # Read the file and do some simple parsing
     columns = ["timestamp", "pressure", "temperature", "dew point", "rh", "altitude"]
     dtype = {col: float for col in columns}
     dtype["timestamp"] = str
 
     rs = pd.read_csv(path, header=0, names=columns, dtype=dtype)
 
-    rs["timestamp"] = pd.to_datetime(rs["timestamp"].str.strip(), format="%Y-%m-%d_%H:%M:%S")
+    rs["timestamp"] = pd.to_datetime(
+        rs["timestamp"].str.strip(), format="%Y-%m-%d_%H:%M:%S"
+    )
     rs = rs.rename(
         columns={
             "altitude": "Altitude",
             "temperature": "Temperature",
             "pressure": "Pressure",
             "rh": "RelativeHumidity",
         }
     )
 
     # Filter for the correct time
-    mask = (rs["timestamp"] >= time_start) & (rs["timestamp"] < time_start + timedelta(minutes=59))
+    mask = (rs["timestamp"] >= time_start) & (
+        rs["timestamp"] < time_start + timedelta(minutes=59)
+    )
     rs = rs.loc[mask]
 
     rs_timestamp = rs["timestamp"].iloc[0]
-    return rs_timestamp, rs.loc[:, ["Altitude", "Temperature", "Pressure", "RelativeHumidity"]]
+    return (
+        rs_timestamp,
+        rs.loc[:, ["Altitude", "Temperature", "Pressure", "RelativeHumidity"]],
+    )
```

### Comparing `pollyxt_pipelines-1.8.3/pollyxt_pipelines/scc_access/__init__.py` & `pollyxt_pipelines-1.9.0/pollyxt_pipelines/scc_access/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,20 +62,30 @@
         This function starts a session with the SCC backend, storing the authentication
         cookies so they can be used by the rest of the methods. Remember to call `logout()`!
         """
 
         # Get login form (for csrf token)
         login_page = self.session.get(constants.login_url)
         if not login_page.ok:
-            raise exceptions.PageNotAccessible(constants.login_url, login_page.status_code)
+            raise exceptions.PageNotAccessible(
+                constants.login_url, login_page.status_code
+            )
 
         # Submit login form
-        body = {"username": self.credentials.username, "password": self.credentials.password}
-        headers = {"X-CSRFToken": login_page.cookies["csrftoken"], "referer": constants.login_url}
-        logon_request = self.session.post(constants.login_url, data=body, headers=headers)
+        body = {
+            "username": self.credentials.username,
+            "password": self.credentials.password,
+        }
+        headers = {
+            "X-CSRFToken": login_page.cookies["csrftoken"],
+            "referer": constants.login_url,
+        }
+        logon_request = self.session.post(
+            constants.login_url, data=body, headers=headers
+        )
 
         # Do some basic checking on the response
         if "Wrong username or password" in logon_request.text:
             raise exceptions.WrongCredentialsException()
 
     def logout(self):
         """Logout of SCC"""
@@ -132,15 +142,16 @@
         last_page = pagination.find("a", class_="end")
         if last_page is None:
             pages = 1
         else:
             pages = int(last_page.text)
 
         measurements = [
-            Measurement.from_table_row(tr) for tr in body.findAll("tr", {"class": "grp-row"})
+            Measurement.from_table_row(tr)
+            for tr in body.findAll("tr", {"class": "grp-row"})
         ]
 
         return pages, measurements
 
     def download_products(
         self,
         measurement_id: str,
@@ -180,15 +191,17 @@
                     "url": constants.download_cloudmask_pattern.format(measurement_id),
                     "path": download_path / f"cloudmask_{measurement_id}.zip",
                 }
             )
         if elpp:
             to_download.append(
                 {
-                    "url": constants.download_preprocessed_pattern.format(measurement_id),
+                    "url": constants.download_preprocessed_pattern.format(
+                        measurement_id
+                    ),
                     "path": download_path / f"preprocessed_{measurement_id}.zip",
                 }
             )
         if optical:
             to_download.append(
                 {
                     "url": constants.download_optical_pattern.format(measurement_id),
@@ -235,15 +248,17 @@
         if file_type == "sounding":
             url = constants.api_sounding_search_pattern.format(file_id)
         elif file_type == "overlap":
             url = constants.api_overlap_search_pattern.format(file_id)
         elif file_type == "lidarratio":
             url = constants.api_lidarratio_search_pattern.format(file_id)
         else:
-            raise ValueError(f"File type should be one of: sounding, overlap, lidarratio")
+            raise ValueError(
+                f"File type should be one of: sounding, overlap, lidarratio"
+            )
 
         # Make request
         response = self.session.get(url)
         if not response.ok:
             raise exceptions.UnexpectedResponse("Could not get anchillary file info")
 
         # Parse body
@@ -307,28 +322,34 @@
 
         files["data"] = open(filename, "rb")
 
         # Get the form and submit it
         upload_page = self.session.get(constants.upload_url)
 
         body = {"system": system_id}
-        headers = {"X-CSRFToken": upload_page.cookies["csrftoken"], "referer": constants.upload_url}
+        headers = {
+            "X-CSRFToken": upload_page.cookies["csrftoken"],
+            "referer": constants.upload_url,
+        }
         upload_submit = self.session.post(
             constants.upload_url, data=body, files=files, headers=headers
         )
 
         # Check response
         response_body = BeautifulSoup(upload_submit.text, "html.parser")
         alerts = response_body.find_all("div", class_="alert-box")
         if len(alerts) > 0:
             errors = ", ".join([alert.p.text.strip() for alert in alerts])
             raise exceptions.SCCError(errors)
 
         # console.print(upload_submit.text)
-        if upload_submit.status_code != 200 or upload_submit.url == constants.upload_url:
+        if (
+            upload_submit.status_code != 200
+            or upload_submit.url == constants.upload_url
+        ):
             raise exceptions.UnexpectedResponse("Upload to SCC failed")
 
     def get_measurement(self, measurement_id: str) -> Union[Measurement, None]:
         """
         Fetches information about one measurement from SCC.
 
         Parameters:
@@ -359,15 +380,18 @@
 
         Parameters:
             measurement_id: Which measurement to delete
         """
 
         # Submit form
         url = constants.delete_measurement_pattern.format(measurement_id)
-        body = {"select_delete_related_measurements": "not_delete_related", "post": "yes"}
+        body = {
+            "select_delete_related_measurements": "not_delete_related",
+            "post": "yes",
+        }
         headers = {
             "referer": url,
             "X-CSRFToken": self.session.cookies["csrftoken"],
         }
         response = self.session.post(url, data=body, headers=headers)
 
         # Look for success banner
@@ -392,29 +416,33 @@
             "selected_across": "0",
             "index": 0,
         }
         headers = {
             "referer": url,
             "X-CSRFToken": self.session.cookies["csrftoken"],
         }
-        response = self.session.post(url, data=body, headers=headers, allow_redirects=False)
+        response = self.session.post(
+            url, data=body, headers=headers, allow_redirects=False
+        )
 
         # Look for success banner
         if response.status_code == 404:
             raise exceptions.MeasurementNotFound(measurement_id)
         if response.status_code != 302:
             raise exceptions.UnexpectedResponse("Response code is not 302")
 
         # Check for message in cookie
         messages_cookie = response.cookies["messages"]
         if messages_cookie is None:
             raise exceptions.UnexpectedResponse("`Messages` cookie not found")
 
         if "The processing chain was restarted" not in messages_cookie:
-            raise exceptions.UnexpectedResponse("Could not found restart message in cookie")
+            raise exceptions.UnexpectedResponse(
+                "Could not found restart message in cookie"
+            )
 
     def get_lidar_consants(
         self, date_start: date, date_end: date, location: Union[Location, None], page=1
     ) -> Tuple[int, List[Measurement]]:
         """
         Fetches the Lidar constants from SCC
 
@@ -450,15 +478,16 @@
         last_page = pagination.find("a", class_="end")
         if last_page is None:
             pages = 1
         else:
             pages = int(last_page.text)
 
         lidar_constants = [
-            LidarConstant.from_table_row(tr) for tr in body.findAll("tr", {"class": "grp-row"})
+            LidarConstant.from_table_row(tr)
+            for tr in body.findAll("tr", {"class": "grp-row"})
         ]
 
         return pages, lidar_constants
 
 
 @contextlib.contextmanager
 def scc_session(credentials: SCC_Credentials):
```

### Comparing `pollyxt_pipelines-1.8.3/pollyxt_pipelines/scc_access/commands.py` & `pollyxt_pipelines-1.9.0/pollyxt_pipelines/scc_access/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,26 +25,30 @@
 
     login
     """
 
     def handle(self):
         # Print warning!
         path = config_paths()[-1]
-        warning_md = "Your credentials will be stored as **PLAIN-TEXT** in the following file:\n"
+        warning_md = (
+            "Your credentials will be stored as **PLAIN-TEXT** in the following file:\n"
+        )
         warning_md += f"\n* {path}\n"
         warning_md += "\nPlease make sure you understand the security implications of this and keep the config files safe!"
         warning_md = Markdown(warning_md)
 
         console.print(Panel(warning_md))
 
         # Ask for the credentials
         console.print(
             "Please enter the HTTP authentication credentials (this is the first login popup when you access the website):"
         )
-        console.print("[warn]The password won't be visible while you are typing![/warn]")
+        console.print(
+            "[warn]The password won't be visible while you are typing![/warn]"
+        )
         http_username = input("Username: ")
         http_password = getpass.getpass("Password: ")
 
         console.print("Please enter your account login:")
         auth_username = input("Username: ")
         auth_password = getpass.getpass("Password: ")
 
@@ -78,26 +82,26 @@
 
 class UploadFiles(Command):
     """
     Batch upload files to SCC
 
     scc-upload
         {path : Path to SCC files. If it is a directory, all netCDF files inside will be uploaded.}
+        {--no-calibration : If uploading a directory, do not upload calibration files.}
         {list? : Optionally, store the uploaded file IDs in order to later download the products using scc-download}
     """
 
     def handle(self):
         # Parse arguments
         path = Path(self.argument("path"))
         if path.is_dir:
             files = path.glob("*.nc")
             files = filter(lambda x: not x.name.startswith("rs_"), files)
-            files = filter(
-                lambda x: not x.name.startswith("calibration_"), files
-            )  # TODO Handle calibration files
+            if self.option("no-calibration"):
+                files = filter(lambda x: not x.name.startswith("calibration_"), files)
         else:
             files = [path]
 
         files = list(files)
         if len(files) == 0:
             console.print("[error]No files found in given directory[/error]")
             return 1
@@ -118,15 +122,15 @@
                 # Read file to find radiosondes
                 nc = Dataset(file, "r")
                 try:
                     radiosonde_path = file.parent / nc.Sounding_File_Name
                 except AttributeError:
                     radiosonde_path = None
                 dataset_id = nc.Measurement_ID
-                configuration_id = nc.NOAReACT_Configuration_ID
+                configuration_id = nc.X_PollyXTPipelines_Configuration_ID
                 nc.close()
 
                 if radiosonde_path is not None and not radiosonde_path.exists():
                     console.print(
                         f"[error]Cannot find radiosonde file[/error] {radiosonde_path} [error] for measurement [/error] {file} [error]. Skipping file.[/error]"
                     )
                     continue
@@ -137,15 +141,17 @@
                     successful_files.append(file)
                     successful_ids.append(dataset_id)
                 except exceptions.SCCError as ex:
                     console.print(
                         f"[error]Error while uploading[/error] {file}[error]:[/error] {str(ex)}"
                     )
                 except Exception:
-                    console.print(f"[error]Unknown error while uploading[/error] {file}")
+                    console.print(
+                        f"[error]Unknown error while uploading[/error] {file}"
+                    )
                     console.print_exception()
 
         successful_count = len(successful_ids)
         if successful_count == 0:
             console.print("[warn]No files were uploaded successfully![/warn]")
             return 0
         else:
@@ -184,15 +190,17 @@
 
         # Check if list or IDs are defined
         id_frame = None
         id_list_file = self.argument("list")
         if id_list_file is None:
             ids = self.option("id")
             if ids is None or len(ids) == 0:
-                self.line_error("Either a list file or some measurement IDs must be provided!")
+                self.line_error(
+                    "Either a list file or some measurement IDs must be provided!"
+                )
                 return 1
         else:
             id_frame = pd.read_csv(id_list_file, index_col="id")
             ids = id_frame.index
 
         # Read application config
         config = Config()
@@ -204,15 +212,17 @@
 
         # Download files for each ID
         with scc_session(credentials) as scc:
             for id in track(ids, description="Downloading products", console=console):
                 # Check if processing is done
                 measurement = scc.get_measurement(id)
                 if measurement.is_processing:
-                    console.print(f"[warn]File[/warn] {id} [warn]is still processing.[/warn]")
+                    console.print(
+                        f"[warn]File[/warn] {id} [warn]is still processing.[/warn]"
+                    )
                     continue
 
                 for file in scc.download_products(id, output_directory):
                     console.print(f"[info]Downloaded[/info] {file}")
                 if id_frame is not None:
                     id_frame.loc[id, "Products_Downloaded"] = True
 
@@ -253,15 +263,17 @@
 
                 for id in ids:
                     try:
                         scc.delete_measurement(id)
                         console.print(f"[info]Deleted[/info] {id}")
                         successes.append(id)
                     except Exception as ex:
-                        console.print(f"-> [error]Could not delete:[/error] {id}", style="bold")
+                        console.print(
+                            f"-> [error]Could not delete:[/error] {id}", style="bold"
+                        )
                         console.print(f"[error]{type(ex).__name__}:[/error] {str(ex)}")
                         failures.append(id)
 
                     progress.advance(task)
 
         # Print a summary
         summary = "---\n"
@@ -306,15 +318,16 @@
                 for id in ids:
                     try:
                         scc.rerun_processing(id)
                         console.print(f"[info]Re-running[/info] {id}")
                         successes.append(id)
                     except Exception as ex:
                         console.print(
-                            f"-> [error]Could not make request:[/error] {id}", style="bold"
+                            f"-> [error]Could not make request:[/error] {id}",
+                            style="bold",
                         )
                         console.print(f"[error]{type(ex).__name__}:[/error] {str(ex)}")
                         failures.append(id)
 
                     progress.advance(task)
 
         # Print a summary
@@ -353,27 +366,33 @@
                 locations.unknown_location_error(location_name)
                 return 1
 
         try:
             date_start = self.argument("date-start")
             date_start = datetime.date.fromisoformat(date_start)
         except ValueError:
-            logging.error("Could not parse date-start! Please use the ISO format (YYYY-MM-DD)")
+            logging.error(
+                "Could not parse date-start! Please use the ISO format (YYYY-MM-DD)"
+            )
             return 1
 
         try:
             date_end = self.argument("date-end")
             date_end = datetime.date.fromisoformat(date_end)
         except ValueError:
-            logging.error("Could not parse date-start! Please use the ISO format (YYYY-MM-DD)")
+            logging.error(
+                "Could not parse date-start! Please use the ISO format (YYYY-MM-DD)"
+            )
             return 1
 
         detailed_status = self.option("detailed-status")
         if detailed_status and (self.option("to-csv") is None):
-            console.print("[error]Cannot use --detailed-status without --to-csv=[/error]")
+            console.print(
+                "[error]Cannot use --detailed-status without --to-csv=[/error]"
+            )
             return 1
 
         # Read application config
         config = Config()
         try:
             credentials = SCC_Credentials(config)
         except KeyError:
@@ -382,15 +401,17 @@
 
         # Login to SCC to make queries
         with scc_session(credentials) as scc:
             with Progress(console=console) as progress:
                 task = progress.add_task("Fetching results...", start=False, total=1)
 
                 # Query SCC for measurements
-                pages, measurements = scc.query_measurements(date_start, date_end, location)
+                pages, measurements = scc.query_measurements(
+                    date_start, date_end, location
+                )
                 if len(measurements) == 0:
                     progress.stop()
                     console.print("[warn]No measurements found![/warn]")
                     return 0
 
                 progress.start_task(task)
                 if pages > 1:
@@ -505,22 +526,26 @@
                 locations.unknown_location_error(location_name)
                 return 1
 
         try:
             date_start = self.argument("date-start")
             date_start = datetime.date.fromisoformat(date_start)
         except ValueError:
-            logging.error("Could not parse date-start! Please use the ISO format (YYYY-MM-DD)")
+            logging.error(
+                "Could not parse date-start! Please use the ISO format (YYYY-MM-DD)"
+            )
             return 1
 
         try:
             date_end = self.argument("date-end")
             date_end = datetime.date.fromisoformat(date_end)
         except ValueError:
-            logging.error("Could not parse date-start! Please use the ISO format (YYYY-MM-DD)")
+            logging.error(
+                "Could not parse date-start! Please use the ISO format (YYYY-MM-DD)"
+            )
             return 1
 
         hirelpp = option_to_bool(self.option("no-hirelpp"), True)
         cloudmask = option_to_bool(self.option("no-cloudmask"), True)
         elpp = option_to_bool(self.option("no-elpp"), True)
         optical = option_to_bool(self.option("no-optical"), True)
         elic = option_to_bool(self.option("no-elic"), True)
@@ -539,15 +564,17 @@
         # Login to SCC
         with scc_session(credentials) as scc:
             # Look up products
             with Progress(console=console) as progress:
                 task = progress.add_task("Fetching results...", start=False, total=1)
 
                 # Query SCC for measurements
-                pages, measurements = scc.query_measurements(date_start, date_end, location)
+                pages, measurements = scc.query_measurements(
+                    date_start, date_end, location
+                )
                 if len(measurements) == 0:
                     progress.stop()
                     console.print("[warn]No measurements found![/warn]")
                     return 0
 
                 if pages > 1:
                     progress.start_task(task)
@@ -559,28 +586,32 @@
                             date_start, date_end, location, page=current_page
                         )
                         measurements += more_measurements
 
                         current_page += 1
                         progress.advance(task)
 
-            console.log(f"[info]Found[/info] {len(measurements)} [info]measurements.[/info]")
+            console.log(
+                f"[info]Found[/info] {len(measurements)} [info]measurements.[/info]"
+            )
 
             # Download files
             measurement_count = len(measurements)
             file_count = 0
             i = 0
             with Progress(console=console) as progress:
                 task = progress.add_task(
-                    f"Downloading products (1/{measurement_count})...", total=measurement_count
+                    f"Downloading products (1/{measurement_count})...",
+                    total=measurement_count,
                 )
 
                 for m in measurements:
                     progress.update(
-                        task, description=f"Downloading products ({i}/{measurement_count})..."
+                        task,
+                        description=f"Downloading products ({i}/{measurement_count})...",
                     )
                     try:
                         for file in scc.download_products(
                             m.id,
                             download_path,
                             hirelpp and (m.hirelpp.status == ProductStatus.OK),
                             cloudmask and (m.cloudmask.status == ProductStatus.OK),
@@ -625,22 +656,26 @@
                 locations.unknown_location_error(location_name)
                 return 1
 
         try:
             date_start = self.argument("date-start")
             date_start = datetime.date.fromisoformat(date_start)
         except ValueError:
-            logging.error("Could not parse date-start! Please use the ISO format (YYYY-MM-DD)")
+            logging.error(
+                "Could not parse date-start! Please use the ISO format (YYYY-MM-DD)"
+            )
             return 1
 
         try:
             date_end = self.argument("date-end")
             date_end = datetime.date.fromisoformat(date_end)
         except ValueError:
-            logging.error("Could not parse date-start! Please use the ISO format (YYYY-MM-DD)")
+            logging.error(
+                "Could not parse date-start! Please use the ISO format (YYYY-MM-DD)"
+            )
             return 1
 
         # Read application config
         config = Config()
         try:
             credentials = SCC_Credentials(config)
         except KeyError:
@@ -649,15 +684,17 @@
 
         # Login to SCC to make queries
         with scc_session(credentials) as scc:
             with Progress(console=console) as progress:
                 task = progress.add_task("Fetching results...", start=False, total=1)
 
                 # Query SCC for measurements
-                pages, lidar_constants = scc.get_lidar_consants(date_start, date_end, location)
+                pages, lidar_constants = scc.get_lidar_consants(
+                    date_start, date_end, location
+                )
                 if len(lidar_constants) == 0:
                     progress.stop()
                     console.print("[warn]No data found![/warn]")
                     return 0
 
                 console.print(f"[info]Found {pages} pages[/info]")
                 progress.start_task(task)
```

### Comparing `pollyxt_pipelines-1.8.3/pollyxt_pipelines/scc_access/constants.py` & `pollyxt_pipelines-1.9.0/pollyxt_pipelines/scc_access/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 # Session management (login/logout)
 login_url = urlparse.urljoin(BASE_URL, "accounts/login/")
 logout_url = urlparse.urljoin(BASE_URL, "accounts/logout/")
 
 # Measurement mnagement
 list_measurements_url = urlparse.urljoin(BASE_URL, "admin/database/measurements/")
 upload_url = urlparse.urljoin(BASE_URL, "data_processing/measurements/quick/")
-delete_measurement_pattern = urlparse.urljoin(BASE_URL, "admin/database/measurements/{0}/delete/")
+delete_measurement_pattern = urlparse.urljoin(
+    BASE_URL, "admin/database/measurements/{0}/delete/"
+)
 rerun_measurement_url = urlparse.urljoin(BASE_URL, "/admin/database/measurements/")
 
 # Lidar constants
 lidar_constants_url = urlparse.urljoin(BASE_URL, "admin/database/lidarconstant/")
 
 # Downloading of products
 download_hirelpp_pattern = urlparse.urljoin(
@@ -42,10 +44,16 @@
     BASE_URL, "data_processing/measurements/{0}/download-elic/"
 )
 
 # API calls
 api_base_url = urlparse.urljoin(BASE_URL, "api/v1/")
 api_measurement_pattern = urlparse.urljoin(api_base_url, "measurements/{0}/")
 api_measurements_url = urlparse.urljoin(api_base_url, "measurements")
-api_sounding_search_pattern = urlparse.urljoin(api_base_url, "sounding_files/?filename={0}")
-api_lidarratio_search_pattern = urlparse.urljoin(api_base_url, "lidarratio_files/?filename={0}")
-api_overlap_search_pattern = urlparse.urljoin(api_base_url, "overlap_files/?filename={0}")
+api_sounding_search_pattern = urlparse.urljoin(
+    api_base_url, "sounding_files/?filename={0}"
+)
+api_lidarratio_search_pattern = urlparse.urljoin(
+    api_base_url, "lidarratio_files/?filename={0}"
+)
+api_overlap_search_pattern = urlparse.urljoin(
+    api_base_url, "overlap_files/?filename={0}"
+)
```

### Comparing `pollyxt_pipelines-1.8.3/pollyxt_pipelines/scc_access/exceptions.py` & `pollyxt_pipelines-1.9.0/pollyxt_pipelines/scc_access/exceptions.py`

 * *Files identical despite different names*

### Comparing `pollyxt_pipelines-1.8.3/pollyxt_pipelines/scc_access/types.py` & `pollyxt_pipelines-1.9.0/pollyxt_pipelines/scc_access/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,17 @@
             station_code=tr.find("th", class_="field-station_id").a.text,
             date_start=scc_date(tr.find("td", class_="field-start")),
             date_end=scc_date(tr.find("td", class_="field-stop")),
             date_creation=scc_date(tr.find("td", class_="field-creation_date")),
             date_updated=scc_date(tr.find("td", class_="field-updated_date")),
             is_uploaded=scc_product_status(tr.find("td", class_="field-upload_ok_evo")),
             hirelpp=scc_product_status(tr.find("td", class_="field-hirelpp_ok_evo")),
-            cloudmask=scc_product_status(tr.find("td", class_="field-cloudmask_ok_evo")),
+            cloudmask=scc_product_status(
+                tr.find("td", class_="field-cloudmask_ok_evo")
+            ),
             elpp=scc_product_status(tr.find("td", class_="field-elpp_ok_evo")),
             elda=scc_product_status(tr.find("td", class_="field-elda_ok_evo")),
             eldec=scc_product_status(tr.find("td", class_="field-eldec_ok_evo")),
             elic=scc_product_status(tr.find("td", class_="field-elic_ok_evo")),
             elquick=scc_product_status(tr.find("td", class_="field-elquick_ok_evo")),
             is_processing=scc_bool(tr.find("td", class_="field-is_being_processed")),
         )
@@ -201,20 +203,28 @@
         # print(tr.prettify())
 
         return LidarConstant(
             measurement_id=tr.find("td", class_="field-measurement_id_display").text,
             channel_id=tr.find("td", class_="field-channel_id_display").text,
             system_id=tr.find("td", class_="field-system_id_display").text,
             product_id=tr.find("td", class_="field-product_id_display").text,
-            detection_wavelength=tr.find("td", class_="field-detection_wavelength").text,
+            detection_wavelength=tr.find(
+                "td", class_="field-detection_wavelength"
+            ).text,
             lidar_constant=tr.find("td", class_="field-lidar_constant").text,
-            lidar_constant_stat_err=tr.find("td", class_="field-lidar_constant_stat_err").text,
-            profile_start_time=scc_date(tr.find("td", class_="field-profile_start_time")),
+            lidar_constant_stat_err=tr.find(
+                "td", class_="field-lidar_constant_stat_err"
+            ).text,
+            profile_start_time=scc_date(
+                tr.find("td", class_="field-profile_start_time")
+            ),
             profile_end_time=scc_date(tr.find("td", class_="field-profile_end_time")),
-            calibration_window_bottom=tr.find("td", class_="field-calibr_window_bottom").text,
+            calibration_window_bottom=tr.find(
+                "td", class_="field-calibr_window_bottom"
+            ).text,
             calibration_window_top=tr.find("td", class_="field-calibr_window_top").text,
             creation_date=scc_date(tr.find("td", class_="field-creation_date")),
             elda_version=tr.find("td", class_="field-elda_version").text,
         )
 
 
 class APIObject:
```

### Comparing `pollyxt_pipelines-1.8.3/pollyxt_pipelines/test_utils.py` & `pollyxt_pipelines-1.9.0/pollyxt_pipelines/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,33 +7,35 @@
 
 class TestDateOptionToDatetime:
     """
     Tests for the utils.date_option_to_datetime() function
     """
 
     def test_full_date_seconds(self):
-        measurement_start = datetime.strptime("2020-01-01_01:23:24", "%Y-%m-%d_%H:%M:%S")
+        measurement_start = datetime.strptime(
+            "2020-01-01_01:23:24", "%Y-%m-%d_%H:%M:%S"
+        )
         string = "2020-01-01_01:23:24"
 
         result = date_option_to_datetime(measurement_start, string)
 
         assert result == datetime.strptime(string, "%Y-%m-%d_%H:%M:%S")
 
-
     def test_full_date(self):
         measurement_start = datetime.strptime("2020-01-01_01:23", "%Y-%m-%d_%H:%M")
         string = "2022-02-10_10:34"
 
         result = date_option_to_datetime(measurement_start, string)
 
         assert result == datetime.strptime(string, "%Y-%m-%d_%H:%M")
 
-
     def test_hour_seconds(self):
-        measurement_start = datetime.strptime("2020-01-01_01:23:34", "%Y-%m-%d_%H:%M:%S")
+        measurement_start = datetime.strptime(
+            "2020-01-01_01:23:34", "%Y-%m-%d_%H:%M:%S"
+        )
         string = "12:00:34"
 
         result = date_option_to_datetime(measurement_start, string)
 
         assert result == measurement_start.replace(hour=12, minute=00, second=34)
 
     def test_hour(self):
```

### Comparing `pollyxt_pipelines-1.8.3/pollyxt_pipelines/utils.py` & `pollyxt_pipelines-1.9.0/pollyxt_pipelines/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,17 @@
         The string parsed as a datetime object
 
     Throws:
         ValueError: When the string is not in an acceptable format
     """
 
     # Try to determine the string's format
-    date_seconds_match = re.search(r"^\d{4}-[01]\d-[0123]\d_[012]\d:[0-5]\d:[0-5]\d", string)
+    date_seconds_match = re.search(
+        r"^\d{4}-[01]\d-[0123]\d_[012]\d:[0-5]\d:[0-5]\d", string
+    )
     if date_seconds_match is not None:
         # Strings seems to be in YYYY-mm-DD HH:MM:SS format
         return datetime.strptime(string, "%Y-%m-%d_%H:%M:%S")
 
     date_match = re.search(r"^\d{4}-[01]\d-[0123]\d_[012]\d:[0-5]\d", string)
     if date_match is not None:
         # String seems to be in YYYY-mm-DD HH:MM format
@@ -104,8 +106,8 @@
     if minutes_match is not None:
         minute = int(string[-2:])
         if today.replace(minute=minute) < today:
             return (today + timedelta(hours=1)).replace(minute=minute)
         else:
             return today.replace(minute=minute)
 
-    raise ValueError("`string` is neither in XX:MM, HH:MM nor YYYY-mm-DD HH:MM format!")
+    raise ValueError("`string` is neither in XX:MM, HH:MM nor YYYY-mm-DD HH:MM format!")
```

### Comparing `pollyxt_pipelines-1.8.3/pyproject.toml` & `pollyxt_pipelines-1.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [tool.poetry]
 name = "pollyxt_pipelines"
-version = "1.8.3"
+version = "1.9.0"
 description = "Tools and scripts related to the automated processing of PollyXT files"
 authors = ["Thanasis Georgiou <ageorgiou@noa.gr>"]
 
 [tool.poetry.scripts]
 pollyxt_pipelines = 'pollyxt_pipelines:main'
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.8,<3.11"
 cleo = "^0.8.1"
-netCDF4 = "^1.5.4"
-numpy = "^1.19.4"
-pandas = "^1.1.4"
-requests = "^2.24.0"
+netCDF4 = "^1.5.7"
+numpy = "^1.21.4"
+pandas = "^1.3.4"
+requests = "^2.26.0"
 beautifulsoup4 = "^4.9.3"
-rich = "^9.2.0"
+rich = "^10.14.0"
+matplotlib = "^3.4.3"
 
 [tool.poetry.dev-dependencies]
 pylint = "^2.6.0"
 Sphinx = "^3.3.1"
 sphinx-typlog-theme = "^0.8.0"
 sphinx-autodoc-typehints = "^1.11.1"
 black = "^20.8b1"
```

### Comparing `pollyxt_pipelines-1.8.3/setup.py` & `pollyxt_pipelines-1.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['pollyxt_pipelines',
  'pollyxt_pipelines.locations',
  'pollyxt_pipelines.polly_to_scc',
+ 'pollyxt_pipelines.qc_eldec',
  'pollyxt_pipelines.radiosondes',
  'pollyxt_pipelines.scc_access']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['beautifulsoup4>=4.9.3,<5.0.0',
  'cleo>=0.8.1,<0.9.0',
- 'netCDF4>=1.5.4,<2.0.0',
- 'numpy>=1.19.4,<2.0.0',
- 'pandas>=1.1.4,<2.0.0',
- 'requests>=2.24.0,<3.0.0',
- 'rich>=9.2.0,<10.0.0']
+ 'matplotlib>=3.4.3,<4.0.0',
+ 'netCDF4>=1.5.7,<2.0.0',
+ 'numpy>=1.21.4,<2.0.0',
+ 'pandas>=1.3.4,<2.0.0',
+ 'requests>=2.26.0,<3.0.0',
+ 'rich>=10.14.0,<11.0.0']
 
 entry_points = \
 {'console_scripts': ['pollyxt_pipelines = pollyxt_pipelines:main']}
 
 setup_kwargs = {
     'name': 'pollyxt-pipelines',
-    'version': '1.8.3',
+    'version': '1.9.0',
     'description': 'Tools and scripts related to the automated processing of PollyXT files',
     'long_description': None,
     'author': 'Thanasis Georgiou',
     'author_email': 'ageorgiou@noa.gr',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.8,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pollyxt_pipelines-1.8.3/PKG-INFO` & `pollyxt_pipelines-1.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pollyxt-pipelines
-Version: 1.8.3
+Version: 1.9.0
 Summary: Tools and scripts related to the automated processing of PollyXT files
 Author: Thanasis Georgiou
 Author-email: ageorgiou@noa.gr
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: beautifulsoup4 (>=4.9.3,<5.0.0)
 Requires-Dist: cleo (>=0.8.1,<0.9.0)
-Requires-Dist: netCDF4 (>=1.5.4,<2.0.0)
-Requires-Dist: numpy (>=1.19.4,<2.0.0)
-Requires-Dist: pandas (>=1.1.4,<2.0.0)
-Requires-Dist: requests (>=2.24.0,<3.0.0)
-Requires-Dist: rich (>=9.2.0,<10.0.0)
+Requires-Dist: matplotlib (>=3.4.3,<4.0.0)
+Requires-Dist: netCDF4 (>=1.5.7,<2.0.0)
+Requires-Dist: numpy (>=1.21.4,<2.0.0)
+Requires-Dist: pandas (>=1.3.4,<2.0.0)
+Requires-Dist: requests (>=2.26.0,<3.0.0)
+Requires-Dist: rich (>=10.14.0,<11.0.0)
```


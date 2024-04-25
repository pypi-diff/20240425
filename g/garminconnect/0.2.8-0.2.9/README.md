# Comparing `tmp/garminconnect-0.2.8.tar.gz` & `tmp/garminconnect-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garminconnect-0.2.8.tar", last modified: Sun Oct  1 08:10:19 2023, max compression
+gzip compressed data, was "garminconnect-0.2.9.tar", last modified: Sat Oct 28 21:43:39 2023, max compression
```

## Comparing `garminconnect-0.2.8.tar` & `garminconnect-0.2.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1074 2023-01-22 08:42:48.711930 garminconnect-0.2.8/LICENSE
--rw-r--r--   0        0        0     5077 2023-10-01 08:02:13.779794 garminconnect-0.2.8/README.md
--rw-r--r--   0        0        0    35118 2023-10-01 07:56:25.934578 garminconnect-0.2.8/garminconnect/__init__.py
--rw-r--r--   0        0        0       22 2023-10-01 08:06:16.866900 garminconnect-0.2.8/garminconnect/version.py
--rw-r--r--   0        0        0     1448 2023-10-01 08:10:19.326223 garminconnect-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     5289 2023-10-01 07:56:25.934578 garminconnect-0.2.8/tests/12129115726_ACTIVITY.fit
--rw-r--r--   0        0        0    37996 2023-09-21 19:38:18.990508 garminconnect-0.2.8/tests/cassettes/test_all_day_stress.yaml
--rw-r--r--   0        0        0     6363 2023-09-15 18:15:37.869821 garminconnect-0.2.8/tests/cassettes/test_body_battery.yaml
--rw-r--r--   0        0        0    11123 2023-09-15 18:15:37.869821 garminconnect-0.2.8/tests/cassettes/test_body_composition.yaml
--rw-r--r--   0        0        0     5952 2023-09-15 18:15:37.869821 garminconnect-0.2.8/tests/cassettes/test_daily_steps.yaml
--rw-r--r--   0        0        0  1270169 2023-09-15 18:15:37.873821 garminconnect-0.2.8/tests/cassettes/test_download_activity.yaml
--rw-r--r--   0        0        0    12169 2023-09-15 18:15:37.873821 garminconnect-0.2.8/tests/cassettes/test_floors.yaml
--rw-r--r--   0        0        0    27563 2023-09-15 18:15:37.873821 garminconnect-0.2.8/tests/cassettes/test_heart_rates.yaml
--rw-r--r--   0        0        0    18158 2023-09-15 18:15:37.873821 garminconnect-0.2.8/tests/cassettes/test_hrv_data.yaml
--rw-r--r--   0        0        0    11089 2023-09-15 18:15:37.873821 garminconnect-0.2.8/tests/cassettes/test_hydration_data.yaml
--rw-r--r--   0        0        0    30168 2023-09-15 18:15:37.873821 garminconnect-0.2.8/tests/cassettes/test_respiration_data.yaml
--rw-r--r--   0        0        0    12481 2023-09-15 18:15:37.873821 garminconnect-0.2.8/tests/cassettes/test_spo2_data.yaml
--rw-r--r--   0        0        0    17075 2023-09-15 18:15:37.873821 garminconnect-0.2.8/tests/cassettes/test_stats.yaml
--rw-r--r--   0        0        0    16380 2023-09-15 18:15:37.873821 garminconnect-0.2.8/tests/cassettes/test_stats_and_body.yaml
--rw-r--r--   0        0        0    23298 2023-09-15 18:15:37.877821 garminconnect-0.2.8/tests/cassettes/test_steps_data.yaml
--rw-r--r--   0        0        0    19356 2023-10-01 07:56:25.934578 garminconnect-0.2.8/tests/cassettes/test_upload.yaml
--rw-r--r--   0        0        0     9040 2023-09-15 18:15:37.877821 garminconnect-0.2.8/tests/cassettes/test_user_summary.yaml
--rw-r--r--   0        0        0     2137 2023-10-01 07:56:25.934578 garminconnect-0.2.8/tests/conftest.py
--rw-r--r--   0        0        0     3287 2023-10-01 07:56:25.934578 garminconnect-0.2.8/tests/test_garmin.py
--rw-r--r--   0        0        0     5755 1970-01-01 00:00:00.000000 garminconnect-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-10-28 20:37:59.074647 garminconnect-0.2.9/LICENSE
+-rw-r--r--   0        0        0     5228 2023-10-28 21:36:14.395308 garminconnect-0.2.9/README.md
+-rw-r--r--   0        0        0    38375 2023-10-28 21:35:49.190725 garminconnect-0.2.9/garminconnect/__init__.py
+-rw-r--r--   0        0        0       22 2023-10-28 20:42:00.512202 garminconnect-0.2.9/garminconnect/version.py
+-rw-r--r--   0        0        0     1503 2023-10-28 21:43:39.293576 garminconnect-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     5289 2023-10-28 20:37:59.074647 garminconnect-0.2.9/tests/12129115726_ACTIVITY.fit
+-rw-r--r--   0        0        0    37996 2023-10-28 20:37:59.074647 garminconnect-0.2.9/tests/cassettes/test_all_day_stress.yaml
+-rw-r--r--   0        0        0     6363 2023-10-28 20:37:59.074647 garminconnect-0.2.9/tests/cassettes/test_body_battery.yaml
+-rw-r--r--   0        0        0    11123 2023-10-28 20:37:59.074647 garminconnect-0.2.9/tests/cassettes/test_body_composition.yaml
+-rw-r--r--   0        0        0     5952 2023-10-28 20:37:59.074647 garminconnect-0.2.9/tests/cassettes/test_daily_steps.yaml
+-rw-r--r--   0        0        0  1270169 2023-10-28 20:37:59.078647 garminconnect-0.2.9/tests/cassettes/test_download_activity.yaml
+-rw-r--r--   0        0        0    12169 2023-10-28 20:37:59.078647 garminconnect-0.2.9/tests/cassettes/test_floors.yaml
+-rw-r--r--   0        0        0    27563 2023-10-28 20:37:59.078647 garminconnect-0.2.9/tests/cassettes/test_heart_rates.yaml
+-rw-r--r--   0        0        0    18158 2023-10-28 20:37:59.078647 garminconnect-0.2.9/tests/cassettes/test_hrv_data.yaml
+-rw-r--r--   0        0        0    11089 2023-10-28 20:37:59.078647 garminconnect-0.2.9/tests/cassettes/test_hydration_data.yaml
+-rw-r--r--   0        0        0    30168 2023-10-28 20:37:59.078647 garminconnect-0.2.9/tests/cassettes/test_respiration_data.yaml
+-rw-r--r--   0        0        0    12481 2023-10-28 20:37:59.078647 garminconnect-0.2.9/tests/cassettes/test_spo2_data.yaml
+-rw-r--r--   0        0        0    17075 2023-10-28 20:37:59.082647 garminconnect-0.2.9/tests/cassettes/test_stats.yaml
+-rw-r--r--   0        0        0    16380 2023-10-28 20:37:59.082647 garminconnect-0.2.9/tests/cassettes/test_stats_and_body.yaml
+-rw-r--r--   0        0        0    23298 2023-10-28 20:37:59.082647 garminconnect-0.2.9/tests/cassettes/test_steps_data.yaml
+-rw-r--r--   0        0        0    19356 2023-10-28 20:37:59.082647 garminconnect-0.2.9/tests/cassettes/test_upload.yaml
+-rw-r--r--   0        0        0     9040 2023-10-28 20:37:59.082647 garminconnect-0.2.9/tests/cassettes/test_user_summary.yaml
+-rw-r--r--   0        0        0     2137 2023-10-28 20:37:59.082647 garminconnect-0.2.9/tests/conftest.py
+-rw-r--r--   0        0        0     3287 2023-10-28 20:37:59.082647 garminconnect-0.2.9/tests/test_garmin.py
+-rw-r--r--   0        0        0     5966 1970-01-01 00:00:00.000000 garminconnect-0.2.9/PKG-INFO
```

### Comparing `garminconnect-0.2.8/LICENSE` & `garminconnect-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `garminconnect-0.2.8/README.md` & `garminconnect-0.2.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 Z -- Remove stored login tokens (logout)
 q -- Exit
 Make your selection: 
 ```
 
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.me/cyberjunkynl/)
 
-Python 3 API wrapper for Garmin Connect to get your statistics.
+Python 3 API wrapper for Garmin Connect.
 
 ## NOTE: For developers using this package
 From `version 0.2.1 onwards`, this package uses `garth` to authenticate and perform API calls.  
 This requires minor changes to your login code, look at the code in `example.py` or the `reference.ipynb` file how to do that.  
 It fixes a lot of stability issues, so it's well worth the effort!  
 
 ## About
@@ -100,14 +100,26 @@
 
 make install-test
 make test
 ```
 
 ## Development
 
+To create a development environment to commit code.
+
+```
+sudo apt install pdm
+snap install ruff
+pdm init
+
+sudo apt install pre-commit
+pip3 install pre-commit
+```
+
+## Example
 The tests provide examples of how to use the library.  
 There is a Jupyter notebook called `reference.ipynb` provided [here](https://github.com/cyberjunky/python-garminconnect/blob/master/reference.ipynb).  
 And you can check out the `example.py` code you can find [here](https://raw.githubusercontent.com/cyberjunky/python-garminconnect/master/example.py), you can run it like so:  
 ```
 pip3 install -r requirements-dev.txt
 ./example.py
 ```
```

### Comparing `garminconnect-0.2.8/garminconnect/__init__.py` & `garminconnect-0.2.9/garminconnect/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,33 @@
-"""Python 3 API wrapper for Garmin Connect to get your statistics."""
+"""Python 3 API wrapper for Garmin Connect."""
 
 import logging
 import os
 from datetime import datetime
 from enum import Enum, auto
 from typing import Any, Dict, List, Optional
 
 import garth
+from withings_sync import fit
 
 logger = logging.getLogger(__name__)
 
 
 class Garmin:
     """Class for fetching data from Garmin Connect."""
 
     def __init__(self, email=None, password=None, is_cn=False):
         """Create a new class instance."""
         self.username = email
         self.password = password
         self.is_cn = is_cn
 
+        self.garmin_connect_user_settings_url = (
+            "/userprofile-service/userprofile/user-settings"
+        )
         self.garmin_connect_devices_url = (
             "/device-service/deviceregistration/devices"
         )
         self.garmin_connect_device_url = "/device-service/deviceservice"
         self.garmin_connect_weight_url = "/weight-service"
         self.garmin_connect_daily_summary_url = (
             "/usersummary-service/usersummary/daily"
@@ -69,14 +73,19 @@
         self.garmin_connect_daily_body_battery_url = (
             "/wellness-service/wellness/bodyBattery/reports/daily"
         )
 
         self.garmin_connect_blood_pressure_endpoint = (
             "/bloodpressure-service/bloodpressure/range"
         )
+
+        self.garmin_connect_set_blood_pressure_endpoint = (
+            "/bloodpressure-service/bloodpressure"
+        )
+
         self.garmin_connect_endurance_score_url = (
             "/metrics-service/metrics/endurancescore"
         )
 
         self.garmin_connect_goals_url = "/goal-service/goal/goals"
 
         self.garmin_connect_rhr_url = "/userstats-service/wellness/daily"
@@ -164,17 +173,15 @@
             self.garth.load(tokenstore)
         else:
             self.garth.login(self.username, self.password)
 
         self.display_name = self.garth.profile["displayName"]
         self.full_name = self.garth.profile["fullName"]
 
-        settings = self.garth.connectapi(
-            "/userprofile-service/userprofile/user-settings"
-        )
+        settings = self.garth.connectapi(self.garmin_connect_user_settings_url)
         self.unit_system = settings["userData"]["measurementSystem"]
 
         return True
 
     def get_full_name(self):
         """Return full name."""
 
@@ -261,14 +268,58 @@
             enddate = startdate
         url = f"{self.garmin_connect_weight_url}/weight/dateRange"
         params = {"startDate": str(startdate), "endDate": str(enddate)}
         logger.debug("Requesting body composition")
 
         return self.connectapi(url, params=params)
 
+    def add_body_composition(
+        self,
+        timestamp: Optional[str],
+        weight: float,
+        percent_fat: Optional[float] = None,
+        percent_hydration: Optional[float] = None,
+        visceral_fat_mass: Optional[float] = None,
+        bone_mass: Optional[float] = None,
+        muscle_mass: Optional[float] = None,
+        basal_met: Optional[float] = None,
+        active_met: Optional[float] = None,
+        physique_rating: Optional[float] = None,
+        metabolic_age: Optional[float] = None,
+        visceral_fat_rating: Optional[float] = None,
+        bmi: Optional[float] = None,
+    ):
+        dt = datetime.fromisoformat(timestamp) if timestamp else datetime.now()
+        fitEncoder = fit.FitEncoderWeight()
+        fitEncoder.write_file_info()
+        fitEncoder.write_file_creator()
+        fitEncoder.write_device_info(dt)
+        fitEncoder.write_weight_scale(
+            dt,
+            weight=weight,
+            percent_fat=percent_fat,
+            percent_hydration=percent_hydration,
+            visceral_fat_mass=visceral_fat_mass,
+            bone_mass=bone_mass,
+            muscle_mass=muscle_mass,
+            basal_met=basal_met,
+            active_met=active_met,
+            physique_rating=physique_rating,
+            metabolic_age=metabolic_age,
+            visceral_fat_rating=visceral_fat_rating,
+            bmi=bmi,
+        )
+        fitEncoder.finish()
+
+        url = self.garmin_connect_upload
+        files = {
+            "file": ("body_composition.fit", fitEncoder.getvalue()),
+        }
+        return self.garth.post("connectapi", url, files=files, api=True)
+
     def add_weigh_in(
         self, weight: int, unitKey: str = "kg", timestamp: str = ""
     ):
         """Add a weigh-in (default to kg)"""
 
         url = f"{self.garmin_connect_weight_url}/user-weight"
         dt = datetime.fromisoformat(timestamp) if timestamp else datetime.now()
@@ -351,14 +402,44 @@
             enddate = startdate
         url = self.garmin_connect_daily_body_battery_url
         params = {"startDate": str(startdate), "endDate": str(enddate)}
         logger.debug("Requesting body battery data")
 
         return self.connectapi(url, params=params)
 
+    def set_blood_pressure(
+        self,
+        systolic: int,
+        diastolic: int,
+        pulse: int,
+        timestamp: str = "",
+        notes: str = "",
+    ):
+        """
+        Add blood pressure measurement
+        """
+
+        url = f"{self.garmin_connect_set_blood_pressure_endpoint}"
+        dt = datetime.fromisoformat(timestamp) if timestamp else datetime.now()
+        # Apply timezone offset to get UTC/GMT time
+        dtGMT = dt - dt.astimezone().tzinfo.utcoffset(dt)
+        payload = {
+            "measurementTimestampLocal": dt.isoformat()[:22] + ".00",
+            "measurementTimestampGMT": dtGMT.isoformat()[:22] + ".00",
+            "systolic": systolic,
+            "diastolic": diastolic,
+            "pulse": pulse,
+            "sourceType": "MANUAL",
+            "notes": notes,
+        }
+
+        logger.debug("Adding blood pressure")
+
+        return self.garth.post("connectapi", url, json=payload)
+
     def get_blood_pressure(
         self, startdate: str, enddate=None
     ) -> Dict[str, Any]:
         """
         Returns blood pressure by day for 'startdate' format
         'YYYY-MM-DD' through enddate 'YYYY-MM-DD'
         """
@@ -674,14 +755,22 @@
         """Return available activities for date."""
 
         url = f"{self.garmin_connect_activity_fordate}/{fordate}"
         logger.debug(f"Requesting activities for date {fordate}")
 
         return self.connectapi(url)
 
+    def set_activity_name(self, activity_id, title):
+        """Set name for activity with id."""
+
+        url = f"{self.garmin_connect_activity}/{activity_id}"
+        payload = {"activityId": activity_id, "activityName": title}
+
+        return self.garth.put("connectapi", url, json=payload, api=True)
+
     def get_last_activity(self):
         """Return last activity."""
 
         activities = self.get_activities(0, 1)
         if activities:
             return activities[-1]
 
@@ -840,17 +929,15 @@
     def set_gear_default(self, activityType, gearUUID, defaultGear=True):
         defaultGearString = "/default/true" if defaultGear else ""
         method_override = "PUT" if defaultGear else "DELETE"
         url = (
             f"{self.garmin_connect_gear_baseurl}{gearUUID}/"
             f"activityType/{activityType}{defaultGearString}"
         )
-        return self.garth.post(
-            "connectapi", url, {"x-http-method-override": method_override}
-        )
+        return self.garth.request(method_override, "connectapi", url, api=True)
 
     class ActivityDownloadFormat(Enum):
         """Activity variables."""
 
         ORIGINAL = auto()
         TCX = auto()
         GPX = auto()
@@ -969,14 +1056,22 @@
             "activityId": str(activity_id),
         }
         url = self.garmin_connect_gear
         logger.debug("Requesting gear for activity_id %s", activity_id)
 
         return self.connectapi(url, params=params)
 
+    def get_user_profile(self):
+        """Get all users settings."""
+
+        url = self.garmin_connect_user_settings_url
+        logger.debug("Requesting user profile.")
+
+        return self.connectapi(url)
+
     def logout(self):
         """Log user out of session."""
 
         logger.error(
             "Deprecated: Alternative is to delete login tokens to logout."
         )
```

### Comparing `garminconnect-0.2.8/pyproject.toml` & `garminconnect-0.2.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 dynamic = []
 description = "Python 3 API wrapper for Garmin Connect"
 authors = [
     { name = "Ron Klinkien", email = "ron@cyberjunky.nl" },
 ]
 dependencies = [
     "garth>=0.4.23",
+    "withings-sync>=4.1.0",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
 ]
 keywords = [
     "garmin connect",
     "api",
     "garmin",
 ]
-version = "0.2.8"
+requires-python = ">=3.10"
+version = "0.2.9"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/cyberjunky/python-garminconnect"
 "Bug Tracker" = "https://github.com/cyberjunky/python-garminconnect/issues"
```

### Comparing `garminconnect-0.2.8/tests/12129115726_ACTIVITY.fit` & `garminconnect-0.2.9/tests/12129115726_ACTIVITY.fit`

 * *Files identical despite different names*

### Comparing `garminconnect-0.2.8/tests/cassettes/test_all_day_stress.yaml` & `garminconnect-0.2.9/tests/cassettes/test_all_day_stress.yaml`

 * *Files identical despite different names*

### Comparing `garminconnect-0.2.8/tests/cassettes/test_body_battery.yaml` & `garminconnect-0.2.9/tests/cassettes/test_body_battery.yaml`

 * *Files identical despite different names*

### Comparing `garminconnect-0.2.8/tests/cassettes/test_body_composition.yaml` & `garminconnect-0.2.9/tests/cassettes/test_body_composition.yaml`

 * *Files identical despite different names*

### Comparing `garminconnect-0.2.8/tests/cassettes/test_daily_steps.yaml` & `garminconnect-0.2.9/tests/cassettes/test_daily_steps.yaml`

 * *Files identical despite different names*

### Comparing `garminconnect-0.2.8/tests/cassettes/test_download_activity.yaml` & `garminconnect-0.2.9/tests/cassettes/test_download_activity.yaml`

 * *Files identical despite different names*

### Comparing `garminconnect-0.2.8/tests/cassettes/test_floors.yaml` & `garminconnect-0.2.9/tests/cassettes/test_floors.yaml`

 * *Files identical despite different names*

### Comparing `garminconnect-0.2.8/tests/cassettes/test_heart_rates.yaml` & `garminconnect-0.2.9/tests/cassettes/test_heart_rates.yaml`

 * *Files identical despite different names*

### Comparing `garminconnect-0.2.8/tests/cassettes/test_hrv_data.yaml` & `garminconnect-0.2.9/tests/cassettes/test_hrv_data.yaml`

 * *Files identical despite different names*

### Comparing `garminconnect-0.2.8/tests/cassettes/test_hydration_data.yaml` & `garminconnect-0.2.9/tests/cassettes/test_hydration_data.yaml`

 * *Files identical despite different names*

### Comparing `garminconnect-0.2.8/tests/cassettes/test_respiration_data.yaml` & `garminconnect-0.2.9/tests/cassettes/test_respiration_data.yaml`

 * *Files identical despite different names*

### Comparing `garminconnect-0.2.8/tests/cassettes/test_spo2_data.yaml` & `garminconnect-0.2.9/tests/cassettes/test_spo2_data.yaml`

 * *Files identical despite different names*

### Comparing `garminconnect-0.2.8/tests/cassettes/test_stats.yaml` & `garminconnect-0.2.9/tests/cassettes/test_stats.yaml`

 * *Files identical despite different names*

### Comparing `garminconnect-0.2.8/tests/cassettes/test_stats_and_body.yaml` & `garminconnect-0.2.9/tests/cassettes/test_stats_and_body.yaml`

 * *Files identical despite different names*

### Comparing `garminconnect-0.2.8/tests/cassettes/test_steps_data.yaml` & `garminconnect-0.2.9/tests/cassettes/test_steps_data.yaml`

 * *Files identical despite different names*

### Comparing `garminconnect-0.2.8/tests/cassettes/test_upload.yaml` & `garminconnect-0.2.9/tests/cassettes/test_upload.yaml`

 * *Files identical despite different names*

### Comparing `garminconnect-0.2.8/tests/cassettes/test_user_summary.yaml` & `garminconnect-0.2.9/tests/cassettes/test_user_summary.yaml`

 * *Files identical despite different names*

### Comparing `garminconnect-0.2.8/tests/conftest.py` & `garminconnect-0.2.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `garminconnect-0.2.8/tests/test_garmin.py` & `garminconnect-0.2.9/tests/test_garmin.py`

 * *Files identical despite different names*

### Comparing `garminconnect-0.2.8/PKG-INFO` & `garminconnect-0.2.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: garminconnect
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python 3 API wrapper for Garmin Connect
 Keywords: garmin connect api garmin
 Author-Email: Ron Klinkien <ron@cyberjunky.nl>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Project-URL: Homepage, https://github.com/cyberjunky/python-garminconnect
 Project-URL: Bug tracker, https://github.com/cyberjunky/python-garminconnect/issues
+Requires-Python: >=3.10
 Requires-Dist: garth>=0.4.23
+Requires-Dist: withings-sync>=4.1.0
 Description-Content-Type: text/markdown
 
 # Python: Garmin Connect
 
 ```
 $ ./example.py 
 
@@ -78,15 +80,15 @@
 Z -- Remove stored login tokens (logout)
 q -- Exit
 Make your selection: 
 ```
 
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.me/cyberjunkynl/)
 
-Python 3 API wrapper for Garmin Connect to get your statistics.
+Python 3 API wrapper for Garmin Connect.
 
 ## NOTE: For developers using this package
 From `version 0.2.1 onwards`, this package uses `garth` to authenticate and perform API calls.  
 This requires minor changes to your login code, look at the code in `example.py` or the `reference.ipynb` file how to do that.  
 It fixes a lot of stability issues, so it's well worth the effort!  
 
 ## About
@@ -117,14 +119,26 @@
 
 make install-test
 make test
 ```
 
 ## Development
 
+To create a development environment to commit code.
+
+```
+sudo apt install pdm
+snap install ruff
+pdm init
+
+sudo apt install pre-commit
+pip3 install pre-commit
+```
+
+## Example
 The tests provide examples of how to use the library.  
 There is a Jupyter notebook called `reference.ipynb` provided [here](https://github.com/cyberjunky/python-garminconnect/blob/master/reference.ipynb).  
 And you can check out the `example.py` code you can find [here](https://raw.githubusercontent.com/cyberjunky/python-garminconnect/master/example.py), you can run it like so:  
 ```
 pip3 install -r requirements-dev.txt
 ./example.py
 ```
```


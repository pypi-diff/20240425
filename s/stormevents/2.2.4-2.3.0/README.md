# Comparing `tmp/stormevents-2.2.4-py3-none-any.whl.zip` & `tmp/stormevents-2.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,20 @@
-Zip file size: 68802 bytes, number of entries: 17
--rw-r--r--  2.0 unx       46 b- defN 24-Mar-14 18:26 stormevents/__init__.py
--rw-r--r--  2.0 unx    19991 b- defN 24-Mar-14 18:26 stormevents/stormevent.py
--rw-r--r--  2.0 unx     3862 b- defN 24-Mar-14 18:26 stormevents/utilities.py
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-14 18:26 stormevents/nhc/__init__.py
--rw-r--r--  2.0 unx    17928 b- defN 24-Mar-14 18:26 stormevents/nhc/atcf.py
--rw-r--r--  2.0 unx     8786 b- defN 24-Mar-14 18:26 stormevents/nhc/storms.py
--rw-r--r--  2.0 unx    51390 b- defN 24-Mar-14 18:26 stormevents/nhc/track.py
--rw-r--r--  2.0 unx      352 b- defN 24-Mar-14 18:26 stormevents/usgs/__init__.py
--rw-r--r--  2.0 unx      363 b- defN 24-Mar-14 18:26 stormevents/usgs/base.py
--rw-r--r--  2.0 unx    29697 b- defN 24-Mar-14 18:26 stormevents/usgs/events.py
--rw-r--r--  2.0 unx    15329 b- defN 24-Mar-14 18:26 stormevents/usgs/highwatermarks.py
--rw-r--r--  2.0 unx     5270 b- defN 24-Mar-14 18:26 stormevents/usgs/sensors.py
--rw-r--r--  2.0 unx    35145 b- defN 24-Mar-14 18:26 stormevents-2.2.4.dist-info/LICENSE
--rw-r--r--  2.0 unx    65188 b- defN 24-Mar-14 18:26 stormevents-2.2.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-14 18:26 stormevents-2.2.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-Mar-14 18:26 stormevents-2.2.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1401 b- defN 24-Mar-14 18:26 stormevents-2.2.4.dist-info/RECORD
-17 files, 254944 bytes uncompressed, 66510 bytes compressed:  73.9%
+Zip file size: 70658 bytes, number of entries: 18
+-rw-r--r--  2.0 unx       46 b- defN 24-Apr-25 11:50 stormevents/__init__.py
+-rw-r--r--  2.0 unx    19991 b- defN 24-Apr-25 11:50 stormevents/stormevent.py
+-rw-r--r--  2.0 unx     3862 b- defN 24-Apr-25 11:50 stormevents/utilities.py
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 11:50 stormevents/nhc/__init__.py
+-rw-r--r--  2.0 unx    17928 b- defN 24-Apr-25 11:50 stormevents/nhc/atcf.py
+-rw-r--r--  2.0 unx     2026 b- defN 24-Apr-25 11:50 stormevents/nhc/const.py
+-rw-r--r--  2.0 unx     8786 b- defN 24-Apr-25 11:50 stormevents/nhc/storms.py
+-rw-r--r--  2.0 unx    54570 b- defN 24-Apr-25 11:50 stormevents/nhc/track.py
+-rw-r--r--  2.0 unx      352 b- defN 24-Apr-25 11:50 stormevents/usgs/__init__.py
+-rw-r--r--  2.0 unx      363 b- defN 24-Apr-25 11:50 stormevents/usgs/base.py
+-rw-r--r--  2.0 unx    29697 b- defN 24-Apr-25 11:50 stormevents/usgs/events.py
+-rw-r--r--  2.0 unx    15329 b- defN 24-Apr-25 11:50 stormevents/usgs/highwatermarks.py
+-rw-r--r--  2.0 unx     5270 b- defN 24-Apr-25 11:50 stormevents/usgs/sensors.py
+-rw-r--r--  2.0 unx    35145 b- defN 24-Apr-25 11:50 stormevents-2.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    65188 b- defN 24-Apr-25 11:50 stormevents-2.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 11:50 stormevents-2.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-Apr-25 11:50 stormevents-2.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1482 b- defN 24-Apr-25 11:50 stormevents-2.3.0.dist-info/RECORD
+18 files, 260231 bytes uncompressed, 68242 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -9,14 +9,17 @@
 
 Filename: stormevents/nhc/__init__.py
 Comment: 
 
 Filename: stormevents/nhc/atcf.py
 Comment: 
 
+Filename: stormevents/nhc/const.py
+Comment: 
+
 Filename: stormevents/nhc/storms.py
 Comment: 
 
 Filename: stormevents/nhc/track.py
 Comment: 
 
 Filename: stormevents/usgs/__init__.py
@@ -30,23 +33,23 @@
 
 Filename: stormevents/usgs/highwatermarks.py
 Comment: 
 
 Filename: stormevents/usgs/sensors.py
 Comment: 
 
-Filename: stormevents-2.2.4.dist-info/LICENSE
+Filename: stormevents-2.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: stormevents-2.2.4.dist-info/METADATA
+Filename: stormevents-2.3.0.dist-info/METADATA
 Comment: 
 
-Filename: stormevents-2.2.4.dist-info/WHEEL
+Filename: stormevents-2.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: stormevents-2.2.4.dist-info/top_level.txt
+Filename: stormevents-2.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: stormevents-2.2.4.dist-info/RECORD
+Filename: stormevents-2.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## stormevents/nhc/track.py

```diff
@@ -29,14 +29,15 @@
 from stormevents.nhc.atcf import ATCF_FileDeck
 from stormevents.nhc.atcf import ATCF_Mode
 from stormevents.nhc.atcf import atcf_url
 from stormevents.nhc.atcf import EXTRA_ATCF_FIELDS
 from stormevents.nhc.atcf import get_atcf_entry
 from stormevents.nhc.atcf import read_atcf
 from stormevents.nhc.storms import nhc_storms
+from stormevents.nhc.const import get_RMW_regression_coefs
 from stormevents.utilities import subset_time_interval
 
 
 class VortexTrack:
     """
     interface to an ATCF vortex track (i.e. HURDAT, best track, HWRF, etc.)
     """
@@ -1200,15 +1201,15 @@
         for track_start_time in track_start_times:
             if advisory == "BEST":
                 track_data = advisory_data
             else:
                 track_data = advisory_data[
                     advisory_data["track_start_time"]
                     == pandas.to_datetime(track_start_time)
-                ].sort_values("forecast_hours")
+                ].sort_index()
 
             tracks[advisory][
                 f"{pandas.to_datetime(track_start_time):%Y%m%dT%H%M%S}"
             ] = track_data
 
     return tracks
 
@@ -1231,14 +1232,17 @@
     Correct official forecast using consensus track along with holland-b
     relation
 
     :param tracks: dictionary of forecasts for each advisory (aside from best track ``BEST``, which only has one hindcast)
     :return: dictionary of forecasts for each advisory (aside from best track ``BEST``, which only has one hindcast) with corrected OFCL
     """
 
+    def clamp(n, minn, maxn):
+        return max(min(maxn, n), minn)
+
     ofcl_tracks = tracks["OFCL"]
     carq_tracks = tracks["CARQ"]
 
     corr_ofcl_tracks = dict()
 
     for initial_time, forecast in ofcl_tracks.items():
         if initial_time in carq_tracks:
@@ -1265,18 +1269,83 @@
         columns_of_interest[columns_of_interest == 0] = pandas.NA
         missing = columns_of_interest.isna()
         # Order of columns is the same as columns_of_interest
         mrd_missing = missing.iloc[:, 0]
         mslp_missing = missing.iloc[:, 1]
         radp_missing = missing.iloc[:, 2]
 
-        # fill OFCL maximum wind radius with the first entry from 0-hr CARQ
-        forecast.loc[mrd_missing, "radius_of_maximum_winds"] = carq_ref[
-            "radius_of_maximum_winds"
+        # fill OFCL maximum wind radius based on regression method from
+        # Penny et al. (2023). https://doi.org/10.1175/WAF-D-22-0209.1
+        isotach_radii = forecast[
+            [
+                "isotach_radius_for_NEQ",
+                "isotach_radius_for_SEQ",
+                "isotach_radius_for_NWQ",
+                "isotach_radius_for_SWQ",
+            ]
         ]
+        isotach_radii[isotach_radii == 0] = pandas.NA
+        rmw0 = carq_ref["radius_of_maximum_winds"]
+        fcst_hrs = (forecast.loc[mrd_missing, "forecast_hours"]).unique()
+        rads = numpy.array([numpy.nan])  # initializing to make sure available
+        for fcst_hr in fcst_hrs:
+            fcst_index = forecast["forecast_hours"] == fcst_hr
+            if fcst_hr < 12:
+                rmw_ = rmw0
+            else:
+                vmax = forecast.loc[fcst_index, "max_sustained_wind_speed"].iloc[0]
+                if numpy.isnan(isotach_radii.loc[fcst_index].to_numpy()).all():
+                    # if no isotach's are found, preserve the isotach(s) if Vmax is greater
+                    if vmax > 50:
+                        rads = rads[0 : min(2, len(rads))]
+                    elif vmax > 34:
+                        rads = rads[[0]]
+                    else:
+                        rads = numpy.array([numpy.nan])
+                else:
+                    rads = numpy.nanmean(
+                        isotach_radii.loc[fcst_index].to_numpy(), axis=1
+                    )
+                coefs = get_RMW_regression_coefs(fcst_hr, rads)
+                lat = forecast.loc[fcst_index, "latitude"].iloc[0]
+                bases = numpy.hstack((1.0, rmw0, rads[~numpy.isnan(rads)], vmax, lat))
+                rmw_ = (bases[1:-1] ** coefs[1:-1]).prod() * numpy.exp(
+                    (coefs[[0, -1]] * bases[[0, -1]]).sum()
+                )  # bound RMW as per Penny et al. (2023)
+            forecast.loc[fcst_index, "radius_of_maximum_winds"] = clamp(
+                rmw_, 5.0, max(120.0, rmw0)
+            )
+        # apply 24-HR moving mean to unique datetimes
+        fcsthr_index = forecast["forecast_hours"].drop_duplicates().index
+        df_temp = forecast.loc[fcsthr_index].copy()
+        # make sure 60, 84, and 108 are added
+        fcsthrs_12hr = numpy.unique(
+            numpy.append(df_temp["forecast_hours"].values, [60, 84, 108])
+        )
+        rmw_12hr = numpy.interp(
+            fcsthrs_12hr, df_temp["forecast_hours"], df_temp["radius_of_maximum_winds"]
+        )
+        dt_12hr = pandas.to_datetime(
+            fcsthrs_12hr, unit="h", origin=df_temp["datetime"].iloc[0]
+        )
+        df_temp = DataFrame(
+            data={"forecast_hours": fcsthrs_12hr, "radius_of_maximum_winds": rmw_12hr},
+            index=dt_12hr,
+        )
+        rmw_rolling = df_temp.rolling(window="24.01 H", center=True, min_periods=1)[
+            "radius_of_maximum_winds"
+        ].mean()
+        for valid_time, rmw in rmw_rolling.items():
+            valid_index = forecast["datetime"] == valid_time
+            if (
+                valid_index.sum() == 0
+                or forecast.loc[valid_index, "forecast_hours"].iloc[0] == 0
+            ):
+                continue
+            forecast.loc[valid_index, "radius_of_maximum_winds"] = rmw
 
         # fill OFCL background pressure with the first entry from 0-hr CARQ background pressure (at sea level)
         forecast.loc[radp_missing, "background_pressure"] = carq_ref[
             "background_pressure"
         ]
 
         # fill OFCL central pressure (at sea level), preserving Holland B from 0-hr CARQ
```

## Comparing `stormevents-2.2.4.dist-info/LICENSE` & `stormevents-2.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `stormevents-2.2.4.dist-info/METADATA` & `stormevents-2.3.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stormevents
-Version: 2.2.4
+Version: 2.3.0
 Summary: Python interfaces for observational data surrounding named storm events
 Author-email: Zach Burnett <zachary.r.burnett@gmail.com>, Soroosh Mani <Soroosh.Mani@noaa.gov>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

## Comparing `stormevents-2.2.4.dist-info/RECORD` & `stormevents-2.3.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 stormevents/__init__.py,sha256=zALPV0qzr71s8hxsjVhVUIGCVWUWr8guIZrCO4Y73JY,46
 stormevents/stormevent.py,sha256=pABl_rUwYnd1isFpkKVlR5aG4HLvIq8ikr6hHRqd20o,19991
 stormevents/utilities.py,sha256=gezrmIB7vKoS4xOrDpi8AbOB-rYQMJ7IIGQuUbpP3SE,3862
 stormevents/nhc/__init__.py,sha256=zGOcaex85eGRuA4qfHtH5BHAQxERmx7WWSgLSa1pmPQ,92
 stormevents/nhc/atcf.py,sha256=L9zm98ibc05WXNbu_iOQolhguuRKIdEwVjzZoU5E4Xg,17928
+stormevents/nhc/const.py,sha256=bwsQeBEKU6ggMsTzZpU698Dy0jCETjDJjsDZhYmflyI,2026
 stormevents/nhc/storms.py,sha256=uBHyAzMZbsh8iAxVPSP8qryb95T4KGhLjdMzkUMREsY,8786
-stormevents/nhc/track.py,sha256=lp4SKaZSIX5kRRpWIMYwi4CXl_ICp6EAhqCmhDbx3pE,51390
+stormevents/nhc/track.py,sha256=l7MR8KrHP7tt06bGAmGEIXcQOSHJGYgAN7uKp2WuD6s,54570
 stormevents/usgs/__init__.py,sha256=nfJme6-5tEkjU8wBVCyv_W3Jm2TBU-AEgouc7r24nh4,352
 stormevents/usgs/base.py,sha256=hWIjBPNyTe12s_pUgLJsDIgZpX3k9dO1oRnUaIOM9XE,363
 stormevents/usgs/events.py,sha256=1XyjjTNfMjIukU6fI1maH7xdb8QGeI8I-jqLqGfop9g,29697
 stormevents/usgs/highwatermarks.py,sha256=UrS-zCCVy7LM_vBzpwRgneE5erGTxT2UBhJZXmtniUk,15329
 stormevents/usgs/sensors.py,sha256=NtOJs8JcBSh_bIBzoZesXARQhmdj78rkFtExn0htU9w,5270
-stormevents-2.2.4.dist-info/LICENSE,sha256=CsWICdCWFNMlGUJiXuxfrxFHw1uyVPns0jZJmzcWkjI,35145
-stormevents-2.2.4.dist-info/METADATA,sha256=C25ktSHNkOyKIYnXTXs4zGNFsA4acCWxeCwLi4G6we0,65188
-stormevents-2.2.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-stormevents-2.2.4.dist-info/top_level.txt,sha256=cBiPqoPys-7YaeBR0qnU5FB6RoglE5w_m0BVDHjoJiE,12
-stormevents-2.2.4.dist-info/RECORD,,
+stormevents-2.3.0.dist-info/LICENSE,sha256=CsWICdCWFNMlGUJiXuxfrxFHw1uyVPns0jZJmzcWkjI,35145
+stormevents-2.3.0.dist-info/METADATA,sha256=MsWilWEz6v358sueyzuswtr_xDisKpYheJJiqO0JZEs,65188
+stormevents-2.3.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+stormevents-2.3.0.dist-info/top_level.txt,sha256=cBiPqoPys-7YaeBR0qnU5FB6RoglE5w_m0BVDHjoJiE,12
+stormevents-2.3.0.dist-info/RECORD,,
```


# Comparing `tmp/lucidmotors-1.1.1.tar.gz` & `tmp/lucidmotors-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lucidmotors-1.1.1.tar", max compression
+gzip compressed data, was "lucidmotors-1.1.2.tar", max compression
```

## Comparing `lucidmotors-1.1.1.tar` & `lucidmotors-1.1.2.tar`

### file list

```diff
@@ -1,45 +1,51 @@
--rw-r--r--   0        0        0     1067 2023-11-10 23:30:11.736120 lucidmotors-1.1.1/LICENSE
--rw-r--r--   0        0        0      819 2024-01-25 06:44:35.584020 lucidmotors-1.1.1/README.md
--rw-r--r--   0        0        0    26594 2024-02-13 02:41:03.277826 lucidmotors-1.1.1/lucidmotors/__init__.py
--rw-r--r--   0        0        0        0 2023-11-10 22:03:32.369161 lucidmotors-1.1.1/lucidmotors/common.py
--rw-r--r--   0        0        0      840 2024-02-11 17:57:24.851184 lucidmotors-1.1.1/lucidmotors/const.py
--rw-r--r--   0        0        0      411 2024-01-25 05:45:20.514343 lucidmotors-1.1.1/lucidmotors/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-12 01:08:13.308130 lucidmotors-1.1.1/lucidmotors/gen/__init__.py
--rw-r--r--   0        0        0     9984 2024-01-28 00:24:52.947347 lucidmotors-1.1.1/lucidmotors/gen/charging_service_pb2.py
--rw-r--r--   0        0        0     9977 2024-01-28 00:24:52.930680 lucidmotors-1.1.1/lucidmotors/gen/charging_service_pb2.py.orig
--rw-r--r--   0        0        0    11097 2024-01-28 00:24:52.947347 lucidmotors-1.1.1/lucidmotors/gen/charging_service_pb2.pyi
--rw-r--r--   0        0        0    11090 2024-01-28 00:24:52.930680 lucidmotors-1.1.1/lucidmotors/gen/charging_service_pb2.pyi.orig
--rw-r--r--   0        0        0    14046 2024-01-28 00:24:52.947347 lucidmotors-1.1.1/lucidmotors/gen/charging_service_pb2_grpc.py
--rw-r--r--   0        0        0    14039 2024-01-28 00:24:52.930680 lucidmotors-1.1.1/lucidmotors/gen/charging_service_pb2_grpc.py.orig
--rw-r--r--   0        0        0     7775 2024-02-12 01:05:28.749681 lucidmotors-1.1.1/lucidmotors/gen/login_session_pb2.py
--rw-r--r--   0        0        0     7761 2024-02-12 01:05:28.723014 lucidmotors-1.1.1/lucidmotors/gen/login_session_pb2.py.orig
--rw-r--r--   0        0        0     7486 2024-02-12 01:05:28.749681 lucidmotors-1.1.1/lucidmotors/gen/login_session_pb2.pyi
--rw-r--r--   0        0        0     7472 2024-02-12 01:05:28.723014 lucidmotors-1.1.1/lucidmotors/gen/login_session_pb2.pyi.orig
--rw-r--r--   0        0        0    15656 2024-02-12 01:05:28.749681 lucidmotors-1.1.1/lucidmotors/gen/login_session_pb2_grpc.py
--rw-r--r--   0        0        0    15649 2024-02-12 01:05:28.723014 lucidmotors-1.1.1/lucidmotors/gen/login_session_pb2_grpc.py.orig
--rw-r--r--   0        0        0     1961 2024-01-28 00:24:53.067348 lucidmotors-1.1.1/lucidmotors/gen/salesforce_service_pb2.py
--rw-r--r--   0        0        0     1961 2024-01-28 00:24:53.050681 lucidmotors-1.1.1/lucidmotors/gen/salesforce_service_pb2.py.orig
--rw-r--r--   0        0        0     1091 2024-01-28 00:24:53.067348 lucidmotors-1.1.1/lucidmotors/gen/salesforce_service_pb2.pyi
--rw-r--r--   0        0        0     1091 2024-01-28 00:24:53.050681 lucidmotors-1.1.1/lucidmotors/gen/salesforce_service_pb2.pyi.orig
--rw-r--r--   0        0        0     2915 2024-01-28 00:24:53.067348 lucidmotors-1.1.1/lucidmotors/gen/salesforce_service_pb2_grpc.py
--rw-r--r--   0        0        0     2908 2024-01-28 00:24:53.050681 lucidmotors-1.1.1/lucidmotors/gen/salesforce_service_pb2_grpc.py.orig
--rw-r--r--   0        0        0     2659 2024-01-28 00:24:52.790679 lucidmotors-1.1.1/lucidmotors/gen/trip_service_pb2.py
--rw-r--r--   0        0        0     2659 2024-01-28 00:24:52.770679 lucidmotors-1.1.1/lucidmotors/gen/trip_service_pb2.py.orig
--rw-r--r--   0        0        0     2645 2024-01-28 00:24:52.790679 lucidmotors-1.1.1/lucidmotors/gen/trip_service_pb2.pyi
--rw-r--r--   0        0        0     2645 2024-01-28 00:24:52.770679 lucidmotors-1.1.1/lucidmotors/gen/trip_service_pb2.pyi.orig
--rw-r--r--   0        0        0     2526 2024-01-28 00:24:52.790679 lucidmotors-1.1.1/lucidmotors/gen/trip_service_pb2_grpc.py
--rw-r--r--   0        0        0     2519 2024-01-28 00:24:52.770679 lucidmotors-1.1.1/lucidmotors/gen/trip_service_pb2_grpc.py.orig
--rw-r--r--   0        0        0     3643 2024-02-12 01:08:13.488132 lucidmotors-1.1.1/lucidmotors/gen/user_profile_service_pb2.py
--rw-r--r--   0        0        0     3643 2024-02-12 01:08:13.461465 lucidmotors-1.1.1/lucidmotors/gen/user_profile_service_pb2.py.orig
--rw-r--r--   0        0        0     3046 2024-02-12 01:08:13.488132 lucidmotors-1.1.1/lucidmotors/gen/user_profile_service_pb2.pyi
--rw-r--r--   0        0        0     3046 2024-02-12 01:08:13.461465 lucidmotors-1.1.1/lucidmotors/gen/user_profile_service_pb2.pyi.orig
--rw-r--r--   0        0        0     6217 2024-02-12 01:08:13.488132 lucidmotors-1.1.1/lucidmotors/gen/user_profile_service_pb2_grpc.py
--rw-r--r--   0        0        0     6210 2024-02-12 01:08:13.461465 lucidmotors-1.1.1/lucidmotors/gen/user_profile_service_pb2_grpc.py.orig
--rw-r--r--   0        0        0    35802 2024-02-12 01:02:10.754117 lucidmotors-1.1.1/lucidmotors/gen/vehicle_state_service_pb2.py
--rw-r--r--   0        0        0    35802 2024-02-12 01:02:10.727450 lucidmotors-1.1.1/lucidmotors/gen/vehicle_state_service_pb2.py.orig
--rw-r--r--   0        0        0    49206 2024-02-12 01:02:10.754117 lucidmotors-1.1.1/lucidmotors/gen/vehicle_state_service_pb2.pyi
--rw-r--r--   0        0        0    49206 2024-02-12 01:02:10.730783 lucidmotors-1.1.1/lucidmotors/gen/vehicle_state_service_pb2.pyi.orig
--rw-r--r--   0        0        0    28751 2024-02-12 01:02:10.754117 lucidmotors-1.1.1/lucidmotors/gen/vehicle_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    28744 2024-02-12 01:02:10.730783 lucidmotors-1.1.1/lucidmotors/gen/vehicle_state_service_pb2_grpc.py.orig
--rw-r--r--   0        0        0      800 2024-02-13 02:41:12.267918 lucidmotors-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1280 1970-01-01 00:00:00.000000 lucidmotors-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-11-10 23:30:11.736120 lucidmotors-1.1.2/LICENSE
+-rw-r--r--   0        0        0      819 2024-01-25 06:44:35.584020 lucidmotors-1.1.2/README.md
+-rw-r--r--   0        0        0    28876 2024-03-01 23:03:33.779918 lucidmotors-1.1.2/lucidmotors/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-10 22:03:32.369161 lucidmotors-1.1.2/lucidmotors/common.py
+-rw-r--r--   0        0        0     1139 2024-03-01 23:24:22.184801 lucidmotors-1.1.2/lucidmotors/const.py
+-rw-r--r--   0        0        0      625 2024-03-01 00:25:14.499378 lucidmotors-1.1.2/lucidmotors/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-25 02:25:24.647414 lucidmotors-1.1.2/lucidmotors/gen/__init__.py
+-rw-r--r--   0        0        0    10570 2024-02-28 23:57:45.296091 lucidmotors-1.1.2/lucidmotors/gen/charging_service_pb2.py
+-rw-r--r--   0        0        0    10563 2024-02-28 23:57:45.272757 lucidmotors-1.1.2/lucidmotors/gen/charging_service_pb2.py.orig
+-rw-r--r--   0        0        0    12246 2024-02-28 23:57:45.296091 lucidmotors-1.1.2/lucidmotors/gen/charging_service_pb2.pyi
+-rw-r--r--   0        0        0    12239 2024-02-28 23:57:45.272757 lucidmotors-1.1.2/lucidmotors/gen/charging_service_pb2.pyi.orig
+-rw-r--r--   0        0        0    14046 2024-02-28 23:57:45.296091 lucidmotors-1.1.2/lucidmotors/gen/charging_service_pb2_grpc.py
+-rw-r--r--   0        0        0    14039 2024-02-28 23:57:45.272757 lucidmotors-1.1.2/lucidmotors/gen/charging_service_pb2_grpc.py.orig
+-rw-r--r--   0        0        0     7855 2024-02-28 23:57:45.096089 lucidmotors-1.1.2/lucidmotors/gen/login_session_pb2.py
+-rw-r--r--   0        0        0     7841 2024-02-28 23:57:45.072755 lucidmotors-1.1.2/lucidmotors/gen/login_session_pb2.py.orig
+-rw-r--r--   0        0        0     7693 2024-02-28 23:57:45.099422 lucidmotors-1.1.2/lucidmotors/gen/login_session_pb2.pyi
+-rw-r--r--   0        0        0     7679 2024-02-28 23:57:45.072755 lucidmotors-1.1.2/lucidmotors/gen/login_session_pb2.pyi.orig
+-rw-r--r--   0        0        0    15656 2024-02-28 23:57:45.099422 lucidmotors-1.1.2/lucidmotors/gen/login_session_pb2_grpc.py
+-rw-r--r--   0        0        0    15649 2024-02-28 23:57:45.072755 lucidmotors-1.1.2/lucidmotors/gen/login_session_pb2_grpc.py.orig
+-rw-r--r--   0        0        0     4139 2024-03-10 15:27:15.191015 lucidmotors-1.1.2/lucidmotors/gen/salesforce_service_pb2.py
+-rw-r--r--   0        0        0     4139 2024-03-10 15:27:15.164348 lucidmotors-1.1.2/lucidmotors/gen/salesforce_service_pb2.py.orig
+-rw-r--r--   0        0        0     4676 2024-03-10 15:27:15.191015 lucidmotors-1.1.2/lucidmotors/gen/salesforce_service_pb2.pyi
+-rw-r--r--   0        0        0     4676 2024-03-10 15:27:15.164348 lucidmotors-1.1.2/lucidmotors/gen/salesforce_service_pb2.pyi.orig
+-rw-r--r--   0        0        0     6199 2024-03-10 15:27:15.191015 lucidmotors-1.1.2/lucidmotors/gen/salesforce_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6192 2024-03-10 15:27:15.164348 lucidmotors-1.1.2/lucidmotors/gen/salesforce_service_pb2_grpc.py.orig
+-rw-r--r--   0        0        0     1484 2024-03-01 00:22:09.487647 lucidmotors-1.1.2/lucidmotors/gen/sentry_service_pb2.py
+-rw-r--r--   0        0        0     1484 2024-03-01 00:22:09.464314 lucidmotors-1.1.2/lucidmotors/gen/sentry_service_pb2.py.orig
+-rw-r--r--   0        0        0      605 2024-03-01 00:22:09.487647 lucidmotors-1.1.2/lucidmotors/gen/sentry_service_pb2.pyi
+-rw-r--r--   0        0        0      605 2024-03-01 00:22:09.464314 lucidmotors-1.1.2/lucidmotors/gen/sentry_service_pb2.pyi.orig
+-rw-r--r--   0        0        0     2556 2024-03-01 00:22:09.487647 lucidmotors-1.1.2/lucidmotors/gen/sentry_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2549 2024-03-01 00:22:09.464314 lucidmotors-1.1.2/lucidmotors/gen/sentry_service_pb2_grpc.py.orig
+-rw-r--r--   0        0        0     2659 2024-01-28 00:24:52.790679 lucidmotors-1.1.2/lucidmotors/gen/trip_service_pb2.py
+-rw-r--r--   0        0        0     2659 2024-01-28 00:24:52.770679 lucidmotors-1.1.2/lucidmotors/gen/trip_service_pb2.py.orig
+-rw-r--r--   0        0        0     2645 2024-01-28 00:24:52.790679 lucidmotors-1.1.2/lucidmotors/gen/trip_service_pb2.pyi
+-rw-r--r--   0        0        0     2645 2024-01-28 00:24:52.770679 lucidmotors-1.1.2/lucidmotors/gen/trip_service_pb2.pyi.orig
+-rw-r--r--   0        0        0     2526 2024-01-28 00:24:52.790679 lucidmotors-1.1.2/lucidmotors/gen/trip_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2519 2024-01-28 00:24:52.770679 lucidmotors-1.1.2/lucidmotors/gen/trip_service_pb2_grpc.py.orig
+-rw-r--r--   0        0        0     3718 2024-02-28 23:57:10.672470 lucidmotors-1.1.2/lucidmotors/gen/user_profile_service_pb2.py
+-rw-r--r--   0        0        0     3718 2024-02-28 23:57:10.672470 lucidmotors-1.1.2/lucidmotors/gen/user_profile_service_pb2.py.orig
+-rw-r--r--   0        0        0     3268 2024-02-28 23:57:10.672470 lucidmotors-1.1.2/lucidmotors/gen/user_profile_service_pb2.pyi
+-rw-r--r--   0        0        0     3268 2024-02-28 23:57:10.672470 lucidmotors-1.1.2/lucidmotors/gen/user_profile_service_pb2.pyi.orig
+-rw-r--r--   0        0        0     6217 2024-02-28 23:57:10.672470 lucidmotors-1.1.2/lucidmotors/gen/user_profile_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6210 2024-02-28 23:57:10.672470 lucidmotors-1.1.2/lucidmotors/gen/user_profile_service_pb2_grpc.py.orig
+-rw-r--r--   0        0        0    36975 2024-04-25 02:25:24.884084 lucidmotors-1.1.2/lucidmotors/gen/vehicle_state_service_pb2.py
+-rw-r--r--   0        0        0    36975 2024-04-25 02:25:24.854083 lucidmotors-1.1.2/lucidmotors/gen/vehicle_state_service_pb2.py.orig
+-rw-r--r--   0        0        0    51054 2024-04-25 02:25:24.887417 lucidmotors-1.1.2/lucidmotors/gen/vehicle_state_service_pb2.pyi
+-rw-r--r--   0        0        0    51054 2024-04-25 02:25:24.854083 lucidmotors-1.1.2/lucidmotors/gen/vehicle_state_service_pb2.pyi.orig
+-rw-r--r--   0        0        0    28751 2024-04-25 02:25:24.884084 lucidmotors-1.1.2/lucidmotors/gen/vehicle_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    28744 2024-04-25 02:25:24.854083 lucidmotors-1.1.2/lucidmotors/gen/vehicle_state_service_pb2_grpc.py.orig
+-rw-r--r--   0        0        0      800 2024-04-25 02:27:25.022442 lucidmotors-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1280 1970-01-01 00:00:00.000000 lucidmotors-1.1.2/PKG-INFO
```

### Comparing `lucidmotors-1.1.1/LICENSE` & `lucidmotors-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lucidmotors-1.1.1/README.md` & `lucidmotors-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `lucidmotors-1.1.1/lucidmotors/__init__.py` & `lucidmotors-1.1.2/lucidmotors/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 """The Lucid Motors mobile app API"""
 from __future__ import annotations
 from typing import Optional, Any, Callable, TypeVar, Awaitable
 from datetime import datetime, timezone, timedelta
 from grpc.aio import ClientCallDetails, UnaryUnaryCall
 from google.protobuf.internal.enum_type_wrapper import EnumTypeWrapper
+from base64 import b64encode
 
 import uuid
 import grpc
 import grpc.aio
 import logging
 
-from .const import MOBILE_API
-from .exceptions import APIError, StatusCode
+from .const import MOBILE_API_REGIONS, Region
+from .exceptions import APIError, APIValueError, StatusCode
 
 from .gen import (
     login_session_pb2,
     login_session_pb2_grpc,
+    user_profile_service_pb2,
+    user_profile_service_pb2_grpc,
     trip_service_pb2,
     trip_service_pb2_grpc,
     vehicle_state_service_pb2,
     vehicle_state_service_pb2 as VSS,
     vehicle_state_service_pb2_grpc,
     charging_service_pb2,
     charging_service_pb2_grpc,
+    salesforce_service_pb2,
+    salesforce_service_pb2_grpc,
 )
 from .gen.login_session_pb2 import NotificationChannelType
 from .gen.user_profile_service_pb2 import UserProfile
 from .gen.vehicle_state_service_pb2 import (
     AccessLevel,
     Model,
     ModelVariant,
@@ -112,16 +117,21 @@
     Cdr,
 )
 from .gen.trip_service_pb2 import (
     WaypointType,
     Waypoint,
     Trip,
 )
+from .gen.salesforce_service_pb2 import (
+    ReferralHistory,
+    MemberAttributes,
+    ReferralData,
+)
 
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 _LOGGER = logging.getLogger(__name__)
 
 
 T = TypeVar('T')
 
 
@@ -230,19 +240,21 @@
             return "AC"
         case (VSS.EnergyType, EnergyType.ENERGY_TYPE_DC):
             return "DC"
         case (VSS.EnergyType, EnergyType.ENERGY_TYPE_V2V):
             return "V2V"
 
         case (VSS.DriveMode, DriveMode.DRIVE_MODE_COMFORT):
-            return "Comfort"
+            return "Smooth"
         case (VSS.DriveMode, DriveMode.DRIVE_MODE_SWIFT):
             return "Swift"
         case (VSS.DriveMode, DriveMode.DRIVE_MODE_SPORT_PLUS):
             return "Sprint"
+        case (VSS.DriveMode, DriveMode.DRIVE_MODE_SERVICE):
+            return "Service"
 
         case (VSS.GearPosition, GearPosition.GEAR_PARK):
             return "Park"
         case (VSS.GearPosition, GearPosition.GEAR_REVERSE):
             return "Reverse"
         case (VSS.GearPosition, GearPosition.GEAR_NEUTRAL):
             return "Neutral"
@@ -296,61 +308,73 @@
     # Expiration time of our current authentication token, or None if we do not
     # have a valid one yet (call .login()).
     _token_expiry_time: Optional[datetime]
 
     # Refresh token for our session
     _refresh_token: Optional[str]
 
+    # Gigya JWT token used for some other authentication?
+    _gigya_jwt: Optional[str]
+
     # User profile data from most recent login request, or None if not logged
     # in yet.
     _user_profile: Optional[UserProfile]
 
     # List of user vehicles
     _vehicles: list[Vehicle]
 
     # RPC call interceptor
     _interceptor: LucidAPIInterceptor
 
     # Service stubs generated from the gRPC Service definitions
     _login_service: login_session_pb2_grpc.LoginSessionStub
+    _user_profile_service: user_profile_service_pb2_grpc.UserProfileServiceStub
     _trip_service: trip_service_pb2_grpc.TripServiceStub
     _vehicle_service: vehicle_state_service_pb2_grpc.VehicleStateServiceStub
     _charging_service: charging_service_pb2_grpc.ChargingServiceStub
+    _salesforce_service: salesforce_service_pb2_grpc.SalesforceServiceStub
 
     # Automatically wake sleeping vehicle along with commands?
     _auto_wake: bool
 
-    def __init__(self, auto_wake: bool = False) -> None:
+    def __init__(self, auto_wake: bool = False, region: Region = Region.US) -> None:
         """Initialize the API client
 
         :param auto_wake: Automatically send a wake request with commands that
         require it if the vehicle is sleeping.
         """
 
         # We start with a channel secured with "SSL credentials," i.e. normal
         # SSL/TLS certificate verification. Once we log in we can upgrade to
         # "token" credentials to keep an authenticated session.
         ssl_creds = grpc.ssl_channel_credentials()
         self._interceptor = LucidAPIInterceptor()
         # Typing ignored due to "_PartialStubMustCastOrIgnore" insanity in
         # grpc-stubs package.
         self._channel = grpc.aio.secure_channel(
-            MOBILE_API,
+            MOBILE_API_REGIONS[region],
             credentials=ssl_creds,
             interceptors=[self._interceptor],  # type: ignore
         )
         self._login_service = login_session_pb2_grpc.LoginSessionStub(self._channel)
+        self._user_profile_service = (
+            user_profile_service_pb2_grpc.UserProfileServiceStub(self._channel)
+        )
         self._trip_service = trip_service_pb2_grpc.TripServiceStub(self._channel)
         self._vehicle_service = vehicle_state_service_pb2_grpc.VehicleStateServiceStub(
             self._channel
         )
         self._charging_service = charging_service_pb2_grpc.ChargingServiceStub(
             self._channel
         )
+        self._salesforce_service = salesforce_service_pb2_grpc.SalesforceServiceStub(
+            self._channel
+        )
         self._refresh_token = None
+        self._gigya_jwt = None
         self._token_expiry_time = None
         self._user_profile = None
         self._vehicles = []
         self._auto_wake = auto_wake
 
     async def __aenter__(self) -> "LucidAPI":
         await self._channel.__aenter__()
@@ -360,14 +384,15 @@
         await self._channel.__aexit__(*exc)
 
     def _save_session(self, sess: login_session_pb2.SessionInfo) -> None:
         self._token_expiry_time = datetime.fromtimestamp(
             sess.expiry_time_sec, timezone.utc
         )
         self._refresh_token = sess.refresh_token
+        self._gigya_jwt = sess.gigya_jwt
 
         _LOGGER.debug(
             "API authentication succeeded. Token expires at %s (%s from now)",
             self._token_expiry_time,
             self._token_expiry_time - datetime.now(timezone.utc),
         )
 
@@ -417,14 +442,53 @@
         reply = await _check_for_api_error(self._login_service.Login(request))
 
         self._save_session(reply.session_info)
 
         self._user_profile = reply.user_profile
         self._vehicles = reply.user_vehicle_data
 
+    async def set_profile_photo(self, photo_bytes: bytes) -> Optional[str]:
+        """Set the logged-in user's profile photo.
+
+        Returns the uploaded photo URL on success."""
+
+        request = user_profile_service_pb2.UploadUserProfilePhotoRequest(
+            photo_bytes=b64encode(photo_bytes).decode('utf-8'),
+        )
+
+        reply = await _check_for_api_error(
+            self._user_profile_service.UploadUserProfilePhoto(request)
+        )
+
+        return reply.photo_url
+
+    async def get_referral_history(self) -> ReferralData:
+        """Fetch the logged-in user's referral history."""
+
+        if self._gigya_jwt is None:
+            raise APIValueError('API did not provide a Gigya JWT token')
+        if self._user_profile is None:
+            raise APIValueError('User profile is missing')
+
+        request = salesforce_service_pb2.ReferralHistoryRequest(
+            email=self._user_profile.email,
+        )
+
+        reply = await _check_for_api_error(
+            self._salesforce_service.ReferralHistory(
+                request,
+                metadata=[('gigyajwt', self._gigya_jwt)],
+            )
+        )
+
+        if reply.statusCode != 200:
+            raise APIValueError(f'Fetching referral history failed: {reply.message}')
+
+        return reply.data
+
     async def authentication_refresh(self) -> None:
         """Get a fresh new token by using the refresh token."""
         request = login_session_pb2.GetNewJWTTokenRequest(
             refresh_token=self._refresh_token
         )
         reply = await _check_for_api_error(self._login_service.GetNewJWTToken(request))
```

### Comparing `lucidmotors-1.1.1/lucidmotors/const.py` & `lucidmotors-1.1.2/lucidmotors/const.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,29 @@
 """Constants for the Lucid Motors API."""
 
+from enum import Enum
+
+
+class Region(Enum):
+    US = 'us'
+    SA = 'sa'
+    EU = 'eu'
+
+    @property
+    def api_domain(self) -> str:
+        return MOBILE_API_REGIONS[self]
+
+
 # Before Lucid was Lucid, it was Atieva. They still use their old domain in
 # their mobile apps for now.
-MOBILE_API = "mobile.deneb.prod.infotainment.pdx.atieva.com"
+MOBILE_API_REGIONS = {
+    Region.US: "mobile.deneb.prod.infotainment.pdx.atieva.com",
+    Region.SA: "mobile.ksap.prod.do.lucidcars.io",
+    Region.EU: "mobile.do.prod.eu.lcid.io",
+}
 
 # Min/max temperatures for HVAC preconditioning. The API rejects anything
 # outside of this range. Values are in Celsius.
 # StatusCode.INVALID_ARGUMENT:
 # SetCabinTemperature failed
 # temperature [15.0 <= x <= 30.0] is required with HVAC_PRECONDITION in
 # SetCabinTemperatureRequest
```

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/charging_service_pb2.py` & `lucidmotors-1.1.2/lucidmotors/gen/charging_service_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,83 +11,85 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from . import vehicle_state_service_pb2 as vehicle__state__service__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x63harging_service.proto\x12\x14mobilegateway.protos\x1a\x1bvehicle_state_service.proto\"\x1b\n\x08\x44\x61teTime\x12\x0f\n\x07seconds\x18\x01 \x01(\x04\"\t\n\x07Unknown\"Y\n\x05Image\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x35\n\x08\x63\x61tegory\x18\x03 \x01(\x0e\x32#.mobilegateway.protos.ImageCategory\x12\x0c\n\x04type\x18\x04 \x01(\t\"C\n\x08Operator\x12\x0c\n\x04name\x18\x01 \x01(\t\x12)\n\x04logo\x18\x03 \x01(\x0b\x32\x1b.mobilegateway.protos.Image\"\x97\x02\n\tConnector\x12\n\n\x02id\x18\x01 \x01(\t\x12\x39\n\x08standard\x18\x02 \x01(\x0e\x32\'.mobilegateway.protos.ConnectorStandard\x12\x35\n\x06\x66ormat\x18\x03 \x01(\x0e\x32%.mobilegateway.protos.ConnectorFormat\x12\x33\n\npower_type\x18\x04 \x01(\x0e\x32\x1f.mobilegateway.protos.PowerType\x12\x0f\n\x07voltage\x18\x05 \x01(\r\x12\x10\n\x08\x61mperage\x18\x06 \x01(\r\x12\x34\n\x06status\x18\x0b \x01(\x0e\x32$.mobilegateway.protos.ChargingStatus\"\xeb\x01\n\x0f\x43hargingSession\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12\x0f\n\x07\x65vse_id\x18\x02 \x01(\t\x12\x34\n\x06status\x18\x03 \x01(\x0e\x32$.mobilegateway.protos.ChargingStatus\x12\x33\n\nconnectors\x18\x06 \x03(\x0b\x32\x1f.mobilegateway.protos.Connector\x12\x33\n\x0b\x63oordinates\x18\x08 \x01(\x0b\x32\x1e.mobilegateway.protos.Location\x12\x1a\n\x12physical_reference\x18\t \x01(\t\"\'\n\x0cOpeningTimes\x12\x17\n\x0ftwentyfourseven\x18\x01 \x01(\x08\"\xa1\x03\n\x10\x43hargingLocation\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\x04 \x01(\t\x12\x0c\n\x04\x63ity\x18\x05 \x01(\t\x12\x13\n\x0bpostal_code\x18\x06 \x01(\t\x12\r\n\x05state\x18\x07 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x08 \x01(\t\x12\x33\n\x0b\x63oordinates\x18\t \x01(\x0b\x32\x1e.mobilegateway.protos.Location\x12\x36\n\x07session\x18\x0b \x01(\x0b\x32%.mobilegateway.protos.ChargingSession\x12\x30\n\x08operator\x18\r \x01(\x0b\x32\x1e.mobilegateway.protos.Operator\x12\x33\n\x0bsuboperator\x18\x0e \x01(\x0b\x32\x1e.mobilegateway.protos.Operator\x12\x10\n\x08timezone\x18\x11 \x01(\t\x12\x39\n\ropening_times\x18\x12 \x01(\x0b\x32\".mobilegateway.protos.OpeningTimes\"t\n\x03\x46\x65\x65\x12+\n\x04name\x18\x01 \x01(\x0e\x32\x1d.mobilegateway.protos.FeeName\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12+\n\x04type\x18\x04 \x01(\x0e\x32\x1d.mobilegateway.protos.FeeType\"\xfa\x02\n\x03\x43\x64r\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x0estart_datetime\x18\x02 \x01(\x0b\x32\x1e.mobilegateway.protos.DateTime\x12\x35\n\rstop_datetime\x18\x03 \x01(\x0b\x32\x1e.mobilegateway.protos.DateTime\x12\x0f\n\x07\x61uth_id\x18\x04 \x01(\t\x12\x14\n\x0ctotal_energy\x18\x06 \x01(\x01\x12\x1a\n\x12total_parking_time\x18\x07 \x01(\x01\x12\x38\n\x08location\x18\n \x01(\x0b\x32&.mobilegateway.protos.ChargingLocation\x12\x12\n\ntotal_time\x18\x0b \x01(\x01\x12-\n\nadd_on_fee\x18\x0e \x03(\x0b\x32\x19.mobilegateway.protos.Fee\x12\x13\n\x0b\x63harge_time\x18\x0f \x01(\x01\x12\x11\n\tidle_time\x18\x11 \x01(\x01\x12\x10\n\x08\x63urrency\x18\x15 \x01(\t\"\x0f\n\rGetCdrRequest\"\x10\n\x0eGetCdrResponse\"/\n\x0eGetCdrsRequest\x12\x0e\n\x06\x65ma_id\x18\x01 \x01(\t\x12\r\n\x05limit\x18\x03 \x01(\r\"9\n\x0fGetCdrsResponse\x12&\n\x03\x63\x64r\x18\x01 \x03(\x0b\x32\x19.mobilegateway.protos.Cdr\"\x18\n\x16GetLocationsBoxRequest\"\x19\n\x17GetLocationsBoxResponse\"\x1d\n\x1bGetLocationsByRadiusRequest\"\x1e\n\x1cGetLocationsByRadiusResponse\"\x12\n\x10GetTariffRequest\"\x13\n\x11GetTariffResponse\"\x15\n\x13RegisterRFIDRequest\"\x16\n\x14RegisterRFIDResponse\"\x15\n\x13StartSessionRequest\"\x16\n\x14StartSessionResponse\"\x14\n\x12StopSessionRequest\"\x15\n\x13StopSessionResponse*H\n\rImageCategory\x12\x1a\n\x16IMAGE_CATEGORY_UNKNOWN\x10\x00\x12\x1b\n\x17IMAGE_CATEGORY_OPERATOR\x10\x05*K\n\x0e\x43hargingStatus\x12\x1b\n\x17\x43HARGING_STATUS_UNKNOWN\x10\x00\x12\x1c\n\x18\x43HARGING_STATUS_CHARGING\x10\x03*^\n\x11\x43onnectorStandard\x12\x1e\n\x1a\x43ONNECTOR_STANDARD_UNKNOWN\x10\x00\x12)\n%CONNECTOR_STANDARD_IEC_62196_T1_COMBO\x10\x13*K\n\x0f\x43onnectorFormat\x12\x1c\n\x18\x43ONNECTOR_FORMAT_UNKNOWN\x10\x00\x12\x1a\n\x16\x43ONNECTOR_FORMAT_CABLE\x10\x02*6\n\tPowerType\x12\x16\n\x12POWER_TYPE_UNKNOWN\x10\x00\x12\x11\n\rPOWER_TYPE_DC\x10\x03*K\n\x07\x46\x65\x65Name\x12\x14\n\x10\x46\x45\x45_NAME_UNKNOWN\x10\x00\x12\x10\n\x0c\x46\x45\x45_NAME_TAX\x10\x01\x12\x18\n\x14\x46\x45\x45_NAME_PARKING_FEE\x10\x04*=\n\x07\x46\x65\x65Type\x12\x14\n\x10\x46\x45\x45_TYPE_UNKNOWN\x10\x00\x12\x1c\n\x18\x46\x45\x45_TYPE_ADD_ON_FEE_FLAT\x10\x01\x32\xcd\x06\n\x0f\x43hargingService\x12U\n\x06GetCdr\x12#.mobilegateway.protos.GetCdrRequest\x1a$.mobilegateway.protos.GetCdrResponse\"\x00\x12X\n\x07GetCdrs\x12$.mobilegateway.protos.GetCdrsRequest\x1a%.mobilegateway.protos.GetCdrsResponse\"\x00\x12p\n\x0fGetLocationsBox\x12,.mobilegateway.protos.GetLocationsBoxRequest\x1a-.mobilegateway.protos.GetLocationsBoxResponse\"\x00\x12\x7f\n\x14GetLocationsByRadius\x12\x31.mobilegateway.protos.GetLocationsByRadiusRequest\x1a\x32.mobilegateway.protos.GetLocationsByRadiusResponse\"\x00\x12^\n\tGetTariff\x12&.mobilegateway.protos.GetTariffRequest\x1a\'.mobilegateway.protos.GetTariffResponse\"\x00\x12g\n\x0cRegisterRFID\x12).mobilegateway.protos.RegisterRFIDRequest\x1a*.mobilegateway.protos.RegisterRFIDResponse\"\x00\x12g\n\x0cStartSession\x12).mobilegateway.protos.StartSessionRequest\x1a*.mobilegateway.protos.StartSessionResponse\"\x00\x12\x64\n\x0bStopSession\x12(.mobilegateway.protos.StopSessionRequest\x1a).mobilegateway.protos.StopSessionResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x63harging_service.proto\x12\x14mobilegateway.protos\x1a\x1bvehicle_state_service.proto\"\x1b\n\x08\x44\x61teTime\x12\x0f\n\x07seconds\x18\x01 \x01(\x04\"\t\n\x07Unknown\"Y\n\x05Image\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x35\n\x08\x63\x61tegory\x18\x03 \x01(\x0e\x32#.mobilegateway.protos.ImageCategory\x12\x0c\n\x04type\x18\x04 \x01(\t\"C\n\x08Operator\x12\x0c\n\x04name\x18\x01 \x01(\t\x12)\n\x04logo\x18\x03 \x01(\x0b\x32\x1b.mobilegateway.protos.Image\"\xa6\x02\n\tConnector\x12\n\n\x02id\x18\x01 \x01(\t\x12\x39\n\x08standard\x18\x02 \x01(\x0e\x32\'.mobilegateway.protos.ConnectorStandard\x12\x35\n\x06\x66ormat\x18\x03 \x01(\x0e\x32%.mobilegateway.protos.ConnectorFormat\x12\x33\n\npower_type\x18\x04 \x01(\x0e\x32\x1f.mobilegateway.protos.PowerType\x12\x0f\n\x07voltage\x18\x05 \x01(\r\x12\x10\n\x08\x61mperage\x18\x06 \x01(\r\x12\x34\n\x06status\x18\x0b \x01(\x0e\x32$.mobilegateway.protos.ChargingStatus\x12\r\n\x05power\x18\x0c \x01(\r\"\xeb\x01\n\x0f\x43hargingSession\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12\x0f\n\x07\x65vse_id\x18\x02 \x01(\t\x12\x34\n\x06status\x18\x03 \x01(\x0e\x32$.mobilegateway.protos.ChargingStatus\x12\x33\n\nconnectors\x18\x06 \x03(\x0b\x32\x1f.mobilegateway.protos.Connector\x12\x33\n\x0b\x63oordinates\x18\x08 \x01(\x0b\x32\x1e.mobilegateway.protos.Location\x12\x1a\n\x12physical_reference\x18\t \x01(\t\"\'\n\x0cOpeningTimes\x12\x17\n\x0ftwentyfourseven\x18\x01 \x01(\x08\"\xa1\x03\n\x10\x43hargingLocation\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\x04 \x01(\t\x12\x0c\n\x04\x63ity\x18\x05 \x01(\t\x12\x13\n\x0bpostal_code\x18\x06 \x01(\t\x12\r\n\x05state\x18\x07 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x08 \x01(\t\x12\x33\n\x0b\x63oordinates\x18\t \x01(\x0b\x32\x1e.mobilegateway.protos.Location\x12\x36\n\x07session\x18\x0b \x01(\x0b\x32%.mobilegateway.protos.ChargingSession\x12\x30\n\x08operator\x18\r \x01(\x0b\x32\x1e.mobilegateway.protos.Operator\x12\x33\n\x0bsuboperator\x18\x0e \x01(\x0b\x32\x1e.mobilegateway.protos.Operator\x12\x10\n\x08timezone\x18\x11 \x01(\t\x12\x39\n\ropening_times\x18\x12 \x01(\x0b\x32\".mobilegateway.protos.OpeningTimes\"t\n\x03\x46\x65\x65\x12+\n\x04name\x18\x01 \x01(\x0e\x32\x1d.mobilegateway.protos.FeeName\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12+\n\x04type\x18\x04 \x01(\x0e\x32\x1d.mobilegateway.protos.FeeType\"\xfa\x02\n\x03\x43\x64r\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x0estart_datetime\x18\x02 \x01(\x0b\x32\x1e.mobilegateway.protos.DateTime\x12\x35\n\rstop_datetime\x18\x03 \x01(\x0b\x32\x1e.mobilegateway.protos.DateTime\x12\x0f\n\x07\x61uth_id\x18\x04 \x01(\t\x12\x14\n\x0ctotal_energy\x18\x06 \x01(\x01\x12\x1a\n\x12total_parking_time\x18\x07 \x01(\x01\x12\x38\n\x08location\x18\n \x01(\x0b\x32&.mobilegateway.protos.ChargingLocation\x12\x12\n\ntotal_time\x18\x0b \x01(\x01\x12-\n\nadd_on_fee\x18\x0e \x03(\x0b\x32\x19.mobilegateway.protos.Fee\x12\x13\n\x0b\x63harge_time\x18\x0f \x01(\x01\x12\x11\n\tidle_time\x18\x11 \x01(\x01\x12\x10\n\x08\x63urrency\x18\x15 \x01(\t\"\x0f\n\rGetCdrRequest\"\x10\n\x0eGetCdrResponse\"/\n\x0eGetCdrsRequest\x12\x0e\n\x06\x65ma_id\x18\x01 \x01(\t\x12\r\n\x05limit\x18\x03 \x01(\r\"9\n\x0fGetCdrsResponse\x12&\n\x03\x63\x64r\x18\x01 \x03(\x0b\x32\x19.mobilegateway.protos.Cdr\"\x18\n\x16GetLocationsBoxRequest\"\x19\n\x17GetLocationsBoxResponse\"f\n\x18\x43hargingLocationDistance\x12\x38\n\x08location\x18\x01 \x01(\x0b\x32&.mobilegateway.protos.ChargingLocation\x12\x10\n\x08\x64istance\x18\x02 \x01(\x04\"]\n\x1bGetLocationsByRadiusRequest\x12.\n\x06origin\x18\x01 \x01(\x0b\x32\x1e.mobilegateway.protos.Location\x12\x0e\n\x06radius\x18\x02 \x01(\r\"a\n\x1cGetLocationsByRadiusResponse\x12\x41\n\tlocations\x18\x01 \x03(\x0b\x32..mobilegateway.protos.ChargingLocationDistance\"\x12\n\x10GetTariffRequest\"\x13\n\x11GetTariffResponse\"9\n\x13RegisterRFIDRequest\x12\x0e\n\x06\x65ma_id\x18\x01 \x01(\t\x12\x12\n\nrfid_token\x18\x02 \x01(\t\"\x16\n\x14RegisterRFIDResponse\"\x15\n\x13StartSessionRequest\"\x16\n\x14StartSessionResponse\"\x14\n\x12StopSessionRequest\"\x15\n\x13StopSessionResponse*H\n\rImageCategory\x12\x1a\n\x16IMAGE_CATEGORY_UNKNOWN\x10\x00\x12\x1b\n\x17IMAGE_CATEGORY_OPERATOR\x10\x05*K\n\x0e\x43hargingStatus\x12\x1b\n\x17\x43HARGING_STATUS_UNKNOWN\x10\x00\x12\x1c\n\x18\x43HARGING_STATUS_CHARGING\x10\x03*^\n\x11\x43onnectorStandard\x12\x1e\n\x1a\x43ONNECTOR_STANDARD_UNKNOWN\x10\x00\x12)\n%CONNECTOR_STANDARD_IEC_62196_T1_COMBO\x10\x13*K\n\x0f\x43onnectorFormat\x12\x1c\n\x18\x43ONNECTOR_FORMAT_UNKNOWN\x10\x00\x12\x1a\n\x16\x43ONNECTOR_FORMAT_CABLE\x10\x02*6\n\tPowerType\x12\x16\n\x12POWER_TYPE_UNKNOWN\x10\x00\x12\x11\n\rPOWER_TYPE_DC\x10\x03*K\n\x07\x46\x65\x65Name\x12\x14\n\x10\x46\x45\x45_NAME_UNKNOWN\x10\x00\x12\x10\n\x0c\x46\x45\x45_NAME_TAX\x10\x01\x12\x18\n\x14\x46\x45\x45_NAME_PARKING_FEE\x10\x04*=\n\x07\x46\x65\x65Type\x12\x14\n\x10\x46\x45\x45_TYPE_UNKNOWN\x10\x00\x12\x1c\n\x18\x46\x45\x45_TYPE_ADD_ON_FEE_FLAT\x10\x01\x32\xcd\x06\n\x0f\x43hargingService\x12U\n\x06GetCdr\x12#.mobilegateway.protos.GetCdrRequest\x1a$.mobilegateway.protos.GetCdrResponse\"\x00\x12X\n\x07GetCdrs\x12$.mobilegateway.protos.GetCdrsRequest\x1a%.mobilegateway.protos.GetCdrsResponse\"\x00\x12p\n\x0fGetLocationsBox\x12,.mobilegateway.protos.GetLocationsBoxRequest\x1a-.mobilegateway.protos.GetLocationsBoxResponse\"\x00\x12\x7f\n\x14GetLocationsByRadius\x12\x31.mobilegateway.protos.GetLocationsByRadiusRequest\x1a\x32.mobilegateway.protos.GetLocationsByRadiusResponse\"\x00\x12^\n\tGetTariff\x12&.mobilegateway.protos.GetTariffRequest\x1a\'.mobilegateway.protos.GetTariffResponse\"\x00\x12g\n\x0cRegisterRFID\x12).mobilegateway.protos.RegisterRFIDRequest\x1a*.mobilegateway.protos.RegisterRFIDResponse\"\x00\x12g\n\x0cStartSession\x12).mobilegateway.protos.StartSessionRequest\x1a*.mobilegateway.protos.StartSessionResponse\"\x00\x12\x64\n\x0bStopSession\x12(.mobilegateway.protos.StopSessionRequest\x1a).mobilegateway.protos.StopSessionResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'charging_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
-  _globals['_IMAGECATEGORY']._serialized_start=2196
-  _globals['_IMAGECATEGORY']._serialized_end=2268
-  _globals['_CHARGINGSTATUS']._serialized_start=2270
-  _globals['_CHARGINGSTATUS']._serialized_end=2345
-  _globals['_CONNECTORSTANDARD']._serialized_start=2347
-  _globals['_CONNECTORSTANDARD']._serialized_end=2441
-  _globals['_CONNECTORFORMAT']._serialized_start=2443
-  _globals['_CONNECTORFORMAT']._serialized_end=2518
-  _globals['_POWERTYPE']._serialized_start=2520
-  _globals['_POWERTYPE']._serialized_end=2574
-  _globals['_FEENAME']._serialized_start=2576
-  _globals['_FEENAME']._serialized_end=2651
-  _globals['_FEETYPE']._serialized_start=2653
-  _globals['_FEETYPE']._serialized_end=2714
+  _globals['_IMAGECATEGORY']._serialized_start=2482
+  _globals['_IMAGECATEGORY']._serialized_end=2554
+  _globals['_CHARGINGSTATUS']._serialized_start=2556
+  _globals['_CHARGINGSTATUS']._serialized_end=2631
+  _globals['_CONNECTORSTANDARD']._serialized_start=2633
+  _globals['_CONNECTORSTANDARD']._serialized_end=2727
+  _globals['_CONNECTORFORMAT']._serialized_start=2729
+  _globals['_CONNECTORFORMAT']._serialized_end=2804
+  _globals['_POWERTYPE']._serialized_start=2806
+  _globals['_POWERTYPE']._serialized_end=2860
+  _globals['_FEENAME']._serialized_start=2862
+  _globals['_FEENAME']._serialized_end=2937
+  _globals['_FEETYPE']._serialized_start=2939
+  _globals['_FEETYPE']._serialized_end=3000
   _globals['_DATETIME']._serialized_start=77
   _globals['_DATETIME']._serialized_end=104
   _globals['_UNKNOWN']._serialized_start=106
   _globals['_UNKNOWN']._serialized_end=115
   _globals['_IMAGE']._serialized_start=117
   _globals['_IMAGE']._serialized_end=206
   _globals['_OPERATOR']._serialized_start=208
   _globals['_OPERATOR']._serialized_end=275
   _globals['_CONNECTOR']._serialized_start=278
-  _globals['_CONNECTOR']._serialized_end=557
-  _globals['_CHARGINGSESSION']._serialized_start=560
-  _globals['_CHARGINGSESSION']._serialized_end=795
-  _globals['_OPENINGTIMES']._serialized_start=797
-  _globals['_OPENINGTIMES']._serialized_end=836
-  _globals['_CHARGINGLOCATION']._serialized_start=839
-  _globals['_CHARGINGLOCATION']._serialized_end=1256
-  _globals['_FEE']._serialized_start=1258
-  _globals['_FEE']._serialized_end=1374
-  _globals['_CDR']._serialized_start=1377
-  _globals['_CDR']._serialized_end=1755
-  _globals['_GETCDRREQUEST']._serialized_start=1757
-  _globals['_GETCDRREQUEST']._serialized_end=1772
-  _globals['_GETCDRRESPONSE']._serialized_start=1774
-  _globals['_GETCDRRESPONSE']._serialized_end=1790
-  _globals['_GETCDRSREQUEST']._serialized_start=1792
-  _globals['_GETCDRSREQUEST']._serialized_end=1839
-  _globals['_GETCDRSRESPONSE']._serialized_start=1841
-  _globals['_GETCDRSRESPONSE']._serialized_end=1898
-  _globals['_GETLOCATIONSBOXREQUEST']._serialized_start=1900
-  _globals['_GETLOCATIONSBOXREQUEST']._serialized_end=1924
-  _globals['_GETLOCATIONSBOXRESPONSE']._serialized_start=1926
-  _globals['_GETLOCATIONSBOXRESPONSE']._serialized_end=1951
-  _globals['_GETLOCATIONSBYRADIUSREQUEST']._serialized_start=1953
-  _globals['_GETLOCATIONSBYRADIUSREQUEST']._serialized_end=1982
-  _globals['_GETLOCATIONSBYRADIUSRESPONSE']._serialized_start=1984
-  _globals['_GETLOCATIONSBYRADIUSRESPONSE']._serialized_end=2014
-  _globals['_GETTARIFFREQUEST']._serialized_start=2016
-  _globals['_GETTARIFFREQUEST']._serialized_end=2034
-  _globals['_GETTARIFFRESPONSE']._serialized_start=2036
-  _globals['_GETTARIFFRESPONSE']._serialized_end=2055
-  _globals['_REGISTERRFIDREQUEST']._serialized_start=2057
-  _globals['_REGISTERRFIDREQUEST']._serialized_end=2078
-  _globals['_REGISTERRFIDRESPONSE']._serialized_start=2080
-  _globals['_REGISTERRFIDRESPONSE']._serialized_end=2102
-  _globals['_STARTSESSIONREQUEST']._serialized_start=2104
-  _globals['_STARTSESSIONREQUEST']._serialized_end=2125
-  _globals['_STARTSESSIONRESPONSE']._serialized_start=2127
-  _globals['_STARTSESSIONRESPONSE']._serialized_end=2149
-  _globals['_STOPSESSIONREQUEST']._serialized_start=2151
-  _globals['_STOPSESSIONREQUEST']._serialized_end=2171
-  _globals['_STOPSESSIONRESPONSE']._serialized_start=2173
-  _globals['_STOPSESSIONRESPONSE']._serialized_end=2194
-  _globals['_CHARGINGSERVICE']._serialized_start=2717
-  _globals['_CHARGINGSERVICE']._serialized_end=3562
+  _globals['_CONNECTOR']._serialized_end=572
+  _globals['_CHARGINGSESSION']._serialized_start=575
+  _globals['_CHARGINGSESSION']._serialized_end=810
+  _globals['_OPENINGTIMES']._serialized_start=812
+  _globals['_OPENINGTIMES']._serialized_end=851
+  _globals['_CHARGINGLOCATION']._serialized_start=854
+  _globals['_CHARGINGLOCATION']._serialized_end=1271
+  _globals['_FEE']._serialized_start=1273
+  _globals['_FEE']._serialized_end=1389
+  _globals['_CDR']._serialized_start=1392
+  _globals['_CDR']._serialized_end=1770
+  _globals['_GETCDRREQUEST']._serialized_start=1772
+  _globals['_GETCDRREQUEST']._serialized_end=1787
+  _globals['_GETCDRRESPONSE']._serialized_start=1789
+  _globals['_GETCDRRESPONSE']._serialized_end=1805
+  _globals['_GETCDRSREQUEST']._serialized_start=1807
+  _globals['_GETCDRSREQUEST']._serialized_end=1854
+  _globals['_GETCDRSRESPONSE']._serialized_start=1856
+  _globals['_GETCDRSRESPONSE']._serialized_end=1913
+  _globals['_GETLOCATIONSBOXREQUEST']._serialized_start=1915
+  _globals['_GETLOCATIONSBOXREQUEST']._serialized_end=1939
+  _globals['_GETLOCATIONSBOXRESPONSE']._serialized_start=1941
+  _globals['_GETLOCATIONSBOXRESPONSE']._serialized_end=1966
+  _globals['_CHARGINGLOCATIONDISTANCE']._serialized_start=1968
+  _globals['_CHARGINGLOCATIONDISTANCE']._serialized_end=2070
+  _globals['_GETLOCATIONSBYRADIUSREQUEST']._serialized_start=2072
+  _globals['_GETLOCATIONSBYRADIUSREQUEST']._serialized_end=2165
+  _globals['_GETLOCATIONSBYRADIUSRESPONSE']._serialized_start=2167
+  _globals['_GETLOCATIONSBYRADIUSRESPONSE']._serialized_end=2264
+  _globals['_GETTARIFFREQUEST']._serialized_start=2266
+  _globals['_GETTARIFFREQUEST']._serialized_end=2284
+  _globals['_GETTARIFFRESPONSE']._serialized_start=2286
+  _globals['_GETTARIFFRESPONSE']._serialized_end=2305
+  _globals['_REGISTERRFIDREQUEST']._serialized_start=2307
+  _globals['_REGISTERRFIDREQUEST']._serialized_end=2364
+  _globals['_REGISTERRFIDRESPONSE']._serialized_start=2366
+  _globals['_REGISTERRFIDRESPONSE']._serialized_end=2388
+  _globals['_STARTSESSIONREQUEST']._serialized_start=2390
+  _globals['_STARTSESSIONREQUEST']._serialized_end=2411
+  _globals['_STARTSESSIONRESPONSE']._serialized_start=2413
+  _globals['_STARTSESSIONRESPONSE']._serialized_end=2435
+  _globals['_STOPSESSIONREQUEST']._serialized_start=2437
+  _globals['_STOPSESSIONREQUEST']._serialized_end=2457
+  _globals['_STOPSESSIONRESPONSE']._serialized_start=2459
+  _globals['_STOPSESSIONRESPONSE']._serialized_end=2480
+  _globals['_CHARGINGSERVICE']._serialized_start=3003
+  _globals['_CHARGINGSERVICE']._serialized_end=3848
 # @@protoc_insertion_point(module_scope)
```

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/charging_service_pb2.py.orig` & `lucidmotors-1.1.2/lucidmotors/gen/charging_service_pb2.py.orig`

 * *Files 2% similar despite different names*

```diff
@@ -11,83 +11,85 @@
 
 _sym_db = _symbol_database.Default()
 
 
 import vehicle_state_service_pb2 as vehicle__state__service__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x63harging_service.proto\x12\x14mobilegateway.protos\x1a\x1bvehicle_state_service.proto\"\x1b\n\x08\x44\x61teTime\x12\x0f\n\x07seconds\x18\x01 \x01(\x04\"\t\n\x07Unknown\"Y\n\x05Image\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x35\n\x08\x63\x61tegory\x18\x03 \x01(\x0e\x32#.mobilegateway.protos.ImageCategory\x12\x0c\n\x04type\x18\x04 \x01(\t\"C\n\x08Operator\x12\x0c\n\x04name\x18\x01 \x01(\t\x12)\n\x04logo\x18\x03 \x01(\x0b\x32\x1b.mobilegateway.protos.Image\"\x97\x02\n\tConnector\x12\n\n\x02id\x18\x01 \x01(\t\x12\x39\n\x08standard\x18\x02 \x01(\x0e\x32\'.mobilegateway.protos.ConnectorStandard\x12\x35\n\x06\x66ormat\x18\x03 \x01(\x0e\x32%.mobilegateway.protos.ConnectorFormat\x12\x33\n\npower_type\x18\x04 \x01(\x0e\x32\x1f.mobilegateway.protos.PowerType\x12\x0f\n\x07voltage\x18\x05 \x01(\r\x12\x10\n\x08\x61mperage\x18\x06 \x01(\r\x12\x34\n\x06status\x18\x0b \x01(\x0e\x32$.mobilegateway.protos.ChargingStatus\"\xeb\x01\n\x0f\x43hargingSession\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12\x0f\n\x07\x65vse_id\x18\x02 \x01(\t\x12\x34\n\x06status\x18\x03 \x01(\x0e\x32$.mobilegateway.protos.ChargingStatus\x12\x33\n\nconnectors\x18\x06 \x03(\x0b\x32\x1f.mobilegateway.protos.Connector\x12\x33\n\x0b\x63oordinates\x18\x08 \x01(\x0b\x32\x1e.mobilegateway.protos.Location\x12\x1a\n\x12physical_reference\x18\t \x01(\t\"\'\n\x0cOpeningTimes\x12\x17\n\x0ftwentyfourseven\x18\x01 \x01(\x08\"\xa1\x03\n\x10\x43hargingLocation\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\x04 \x01(\t\x12\x0c\n\x04\x63ity\x18\x05 \x01(\t\x12\x13\n\x0bpostal_code\x18\x06 \x01(\t\x12\r\n\x05state\x18\x07 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x08 \x01(\t\x12\x33\n\x0b\x63oordinates\x18\t \x01(\x0b\x32\x1e.mobilegateway.protos.Location\x12\x36\n\x07session\x18\x0b \x01(\x0b\x32%.mobilegateway.protos.ChargingSession\x12\x30\n\x08operator\x18\r \x01(\x0b\x32\x1e.mobilegateway.protos.Operator\x12\x33\n\x0bsuboperator\x18\x0e \x01(\x0b\x32\x1e.mobilegateway.protos.Operator\x12\x10\n\x08timezone\x18\x11 \x01(\t\x12\x39\n\ropening_times\x18\x12 \x01(\x0b\x32\".mobilegateway.protos.OpeningTimes\"t\n\x03\x46\x65\x65\x12+\n\x04name\x18\x01 \x01(\x0e\x32\x1d.mobilegateway.protos.FeeName\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12+\n\x04type\x18\x04 \x01(\x0e\x32\x1d.mobilegateway.protos.FeeType\"\xfa\x02\n\x03\x43\x64r\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x0estart_datetime\x18\x02 \x01(\x0b\x32\x1e.mobilegateway.protos.DateTime\x12\x35\n\rstop_datetime\x18\x03 \x01(\x0b\x32\x1e.mobilegateway.protos.DateTime\x12\x0f\n\x07\x61uth_id\x18\x04 \x01(\t\x12\x14\n\x0ctotal_energy\x18\x06 \x01(\x01\x12\x1a\n\x12total_parking_time\x18\x07 \x01(\x01\x12\x38\n\x08location\x18\n \x01(\x0b\x32&.mobilegateway.protos.ChargingLocation\x12\x12\n\ntotal_time\x18\x0b \x01(\x01\x12-\n\nadd_on_fee\x18\x0e \x03(\x0b\x32\x19.mobilegateway.protos.Fee\x12\x13\n\x0b\x63harge_time\x18\x0f \x01(\x01\x12\x11\n\tidle_time\x18\x11 \x01(\x01\x12\x10\n\x08\x63urrency\x18\x15 \x01(\t\"\x0f\n\rGetCdrRequest\"\x10\n\x0eGetCdrResponse\"/\n\x0eGetCdrsRequest\x12\x0e\n\x06\x65ma_id\x18\x01 \x01(\t\x12\r\n\x05limit\x18\x03 \x01(\r\"9\n\x0fGetCdrsResponse\x12&\n\x03\x63\x64r\x18\x01 \x03(\x0b\x32\x19.mobilegateway.protos.Cdr\"\x18\n\x16GetLocationsBoxRequest\"\x19\n\x17GetLocationsBoxResponse\"\x1d\n\x1bGetLocationsByRadiusRequest\"\x1e\n\x1cGetLocationsByRadiusResponse\"\x12\n\x10GetTariffRequest\"\x13\n\x11GetTariffResponse\"\x15\n\x13RegisterRFIDRequest\"\x16\n\x14RegisterRFIDResponse\"\x15\n\x13StartSessionRequest\"\x16\n\x14StartSessionResponse\"\x14\n\x12StopSessionRequest\"\x15\n\x13StopSessionResponse*H\n\rImageCategory\x12\x1a\n\x16IMAGE_CATEGORY_UNKNOWN\x10\x00\x12\x1b\n\x17IMAGE_CATEGORY_OPERATOR\x10\x05*K\n\x0e\x43hargingStatus\x12\x1b\n\x17\x43HARGING_STATUS_UNKNOWN\x10\x00\x12\x1c\n\x18\x43HARGING_STATUS_CHARGING\x10\x03*^\n\x11\x43onnectorStandard\x12\x1e\n\x1a\x43ONNECTOR_STANDARD_UNKNOWN\x10\x00\x12)\n%CONNECTOR_STANDARD_IEC_62196_T1_COMBO\x10\x13*K\n\x0f\x43onnectorFormat\x12\x1c\n\x18\x43ONNECTOR_FORMAT_UNKNOWN\x10\x00\x12\x1a\n\x16\x43ONNECTOR_FORMAT_CABLE\x10\x02*6\n\tPowerType\x12\x16\n\x12POWER_TYPE_UNKNOWN\x10\x00\x12\x11\n\rPOWER_TYPE_DC\x10\x03*K\n\x07\x46\x65\x65Name\x12\x14\n\x10\x46\x45\x45_NAME_UNKNOWN\x10\x00\x12\x10\n\x0c\x46\x45\x45_NAME_TAX\x10\x01\x12\x18\n\x14\x46\x45\x45_NAME_PARKING_FEE\x10\x04*=\n\x07\x46\x65\x65Type\x12\x14\n\x10\x46\x45\x45_TYPE_UNKNOWN\x10\x00\x12\x1c\n\x18\x46\x45\x45_TYPE_ADD_ON_FEE_FLAT\x10\x01\x32\xcd\x06\n\x0f\x43hargingService\x12U\n\x06GetCdr\x12#.mobilegateway.protos.GetCdrRequest\x1a$.mobilegateway.protos.GetCdrResponse\"\x00\x12X\n\x07GetCdrs\x12$.mobilegateway.protos.GetCdrsRequest\x1a%.mobilegateway.protos.GetCdrsResponse\"\x00\x12p\n\x0fGetLocationsBox\x12,.mobilegateway.protos.GetLocationsBoxRequest\x1a-.mobilegateway.protos.GetLocationsBoxResponse\"\x00\x12\x7f\n\x14GetLocationsByRadius\x12\x31.mobilegateway.protos.GetLocationsByRadiusRequest\x1a\x32.mobilegateway.protos.GetLocationsByRadiusResponse\"\x00\x12^\n\tGetTariff\x12&.mobilegateway.protos.GetTariffRequest\x1a\'.mobilegateway.protos.GetTariffResponse\"\x00\x12g\n\x0cRegisterRFID\x12).mobilegateway.protos.RegisterRFIDRequest\x1a*.mobilegateway.protos.RegisterRFIDResponse\"\x00\x12g\n\x0cStartSession\x12).mobilegateway.protos.StartSessionRequest\x1a*.mobilegateway.protos.StartSessionResponse\"\x00\x12\x64\n\x0bStopSession\x12(.mobilegateway.protos.StopSessionRequest\x1a).mobilegateway.protos.StopSessionResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x63harging_service.proto\x12\x14mobilegateway.protos\x1a\x1bvehicle_state_service.proto\"\x1b\n\x08\x44\x61teTime\x12\x0f\n\x07seconds\x18\x01 \x01(\x04\"\t\n\x07Unknown\"Y\n\x05Image\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x35\n\x08\x63\x61tegory\x18\x03 \x01(\x0e\x32#.mobilegateway.protos.ImageCategory\x12\x0c\n\x04type\x18\x04 \x01(\t\"C\n\x08Operator\x12\x0c\n\x04name\x18\x01 \x01(\t\x12)\n\x04logo\x18\x03 \x01(\x0b\x32\x1b.mobilegateway.protos.Image\"\xa6\x02\n\tConnector\x12\n\n\x02id\x18\x01 \x01(\t\x12\x39\n\x08standard\x18\x02 \x01(\x0e\x32\'.mobilegateway.protos.ConnectorStandard\x12\x35\n\x06\x66ormat\x18\x03 \x01(\x0e\x32%.mobilegateway.protos.ConnectorFormat\x12\x33\n\npower_type\x18\x04 \x01(\x0e\x32\x1f.mobilegateway.protos.PowerType\x12\x0f\n\x07voltage\x18\x05 \x01(\r\x12\x10\n\x08\x61mperage\x18\x06 \x01(\r\x12\x34\n\x06status\x18\x0b \x01(\x0e\x32$.mobilegateway.protos.ChargingStatus\x12\r\n\x05power\x18\x0c \x01(\r\"\xeb\x01\n\x0f\x43hargingSession\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12\x0f\n\x07\x65vse_id\x18\x02 \x01(\t\x12\x34\n\x06status\x18\x03 \x01(\x0e\x32$.mobilegateway.protos.ChargingStatus\x12\x33\n\nconnectors\x18\x06 \x03(\x0b\x32\x1f.mobilegateway.protos.Connector\x12\x33\n\x0b\x63oordinates\x18\x08 \x01(\x0b\x32\x1e.mobilegateway.protos.Location\x12\x1a\n\x12physical_reference\x18\t \x01(\t\"\'\n\x0cOpeningTimes\x12\x17\n\x0ftwentyfourseven\x18\x01 \x01(\x08\"\xa1\x03\n\x10\x43hargingLocation\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\x04 \x01(\t\x12\x0c\n\x04\x63ity\x18\x05 \x01(\t\x12\x13\n\x0bpostal_code\x18\x06 \x01(\t\x12\r\n\x05state\x18\x07 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x08 \x01(\t\x12\x33\n\x0b\x63oordinates\x18\t \x01(\x0b\x32\x1e.mobilegateway.protos.Location\x12\x36\n\x07session\x18\x0b \x01(\x0b\x32%.mobilegateway.protos.ChargingSession\x12\x30\n\x08operator\x18\r \x01(\x0b\x32\x1e.mobilegateway.protos.Operator\x12\x33\n\x0bsuboperator\x18\x0e \x01(\x0b\x32\x1e.mobilegateway.protos.Operator\x12\x10\n\x08timezone\x18\x11 \x01(\t\x12\x39\n\ropening_times\x18\x12 \x01(\x0b\x32\".mobilegateway.protos.OpeningTimes\"t\n\x03\x46\x65\x65\x12+\n\x04name\x18\x01 \x01(\x0e\x32\x1d.mobilegateway.protos.FeeName\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12+\n\x04type\x18\x04 \x01(\x0e\x32\x1d.mobilegateway.protos.FeeType\"\xfa\x02\n\x03\x43\x64r\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x0estart_datetime\x18\x02 \x01(\x0b\x32\x1e.mobilegateway.protos.DateTime\x12\x35\n\rstop_datetime\x18\x03 \x01(\x0b\x32\x1e.mobilegateway.protos.DateTime\x12\x0f\n\x07\x61uth_id\x18\x04 \x01(\t\x12\x14\n\x0ctotal_energy\x18\x06 \x01(\x01\x12\x1a\n\x12total_parking_time\x18\x07 \x01(\x01\x12\x38\n\x08location\x18\n \x01(\x0b\x32&.mobilegateway.protos.ChargingLocation\x12\x12\n\ntotal_time\x18\x0b \x01(\x01\x12-\n\nadd_on_fee\x18\x0e \x03(\x0b\x32\x19.mobilegateway.protos.Fee\x12\x13\n\x0b\x63harge_time\x18\x0f \x01(\x01\x12\x11\n\tidle_time\x18\x11 \x01(\x01\x12\x10\n\x08\x63urrency\x18\x15 \x01(\t\"\x0f\n\rGetCdrRequest\"\x10\n\x0eGetCdrResponse\"/\n\x0eGetCdrsRequest\x12\x0e\n\x06\x65ma_id\x18\x01 \x01(\t\x12\r\n\x05limit\x18\x03 \x01(\r\"9\n\x0fGetCdrsResponse\x12&\n\x03\x63\x64r\x18\x01 \x03(\x0b\x32\x19.mobilegateway.protos.Cdr\"\x18\n\x16GetLocationsBoxRequest\"\x19\n\x17GetLocationsBoxResponse\"f\n\x18\x43hargingLocationDistance\x12\x38\n\x08location\x18\x01 \x01(\x0b\x32&.mobilegateway.protos.ChargingLocation\x12\x10\n\x08\x64istance\x18\x02 \x01(\x04\"]\n\x1bGetLocationsByRadiusRequest\x12.\n\x06origin\x18\x01 \x01(\x0b\x32\x1e.mobilegateway.protos.Location\x12\x0e\n\x06radius\x18\x02 \x01(\r\"a\n\x1cGetLocationsByRadiusResponse\x12\x41\n\tlocations\x18\x01 \x03(\x0b\x32..mobilegateway.protos.ChargingLocationDistance\"\x12\n\x10GetTariffRequest\"\x13\n\x11GetTariffResponse\"9\n\x13RegisterRFIDRequest\x12\x0e\n\x06\x65ma_id\x18\x01 \x01(\t\x12\x12\n\nrfid_token\x18\x02 \x01(\t\"\x16\n\x14RegisterRFIDResponse\"\x15\n\x13StartSessionRequest\"\x16\n\x14StartSessionResponse\"\x14\n\x12StopSessionRequest\"\x15\n\x13StopSessionResponse*H\n\rImageCategory\x12\x1a\n\x16IMAGE_CATEGORY_UNKNOWN\x10\x00\x12\x1b\n\x17IMAGE_CATEGORY_OPERATOR\x10\x05*K\n\x0e\x43hargingStatus\x12\x1b\n\x17\x43HARGING_STATUS_UNKNOWN\x10\x00\x12\x1c\n\x18\x43HARGING_STATUS_CHARGING\x10\x03*^\n\x11\x43onnectorStandard\x12\x1e\n\x1a\x43ONNECTOR_STANDARD_UNKNOWN\x10\x00\x12)\n%CONNECTOR_STANDARD_IEC_62196_T1_COMBO\x10\x13*K\n\x0f\x43onnectorFormat\x12\x1c\n\x18\x43ONNECTOR_FORMAT_UNKNOWN\x10\x00\x12\x1a\n\x16\x43ONNECTOR_FORMAT_CABLE\x10\x02*6\n\tPowerType\x12\x16\n\x12POWER_TYPE_UNKNOWN\x10\x00\x12\x11\n\rPOWER_TYPE_DC\x10\x03*K\n\x07\x46\x65\x65Name\x12\x14\n\x10\x46\x45\x45_NAME_UNKNOWN\x10\x00\x12\x10\n\x0c\x46\x45\x45_NAME_TAX\x10\x01\x12\x18\n\x14\x46\x45\x45_NAME_PARKING_FEE\x10\x04*=\n\x07\x46\x65\x65Type\x12\x14\n\x10\x46\x45\x45_TYPE_UNKNOWN\x10\x00\x12\x1c\n\x18\x46\x45\x45_TYPE_ADD_ON_FEE_FLAT\x10\x01\x32\xcd\x06\n\x0f\x43hargingService\x12U\n\x06GetCdr\x12#.mobilegateway.protos.GetCdrRequest\x1a$.mobilegateway.protos.GetCdrResponse\"\x00\x12X\n\x07GetCdrs\x12$.mobilegateway.protos.GetCdrsRequest\x1a%.mobilegateway.protos.GetCdrsResponse\"\x00\x12p\n\x0fGetLocationsBox\x12,.mobilegateway.protos.GetLocationsBoxRequest\x1a-.mobilegateway.protos.GetLocationsBoxResponse\"\x00\x12\x7f\n\x14GetLocationsByRadius\x12\x31.mobilegateway.protos.GetLocationsByRadiusRequest\x1a\x32.mobilegateway.protos.GetLocationsByRadiusResponse\"\x00\x12^\n\tGetTariff\x12&.mobilegateway.protos.GetTariffRequest\x1a\'.mobilegateway.protos.GetTariffResponse\"\x00\x12g\n\x0cRegisterRFID\x12).mobilegateway.protos.RegisterRFIDRequest\x1a*.mobilegateway.protos.RegisterRFIDResponse\"\x00\x12g\n\x0cStartSession\x12).mobilegateway.protos.StartSessionRequest\x1a*.mobilegateway.protos.StartSessionResponse\"\x00\x12\x64\n\x0bStopSession\x12(.mobilegateway.protos.StopSessionRequest\x1a).mobilegateway.protos.StopSessionResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'charging_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
-  _globals['_IMAGECATEGORY']._serialized_start=2196
-  _globals['_IMAGECATEGORY']._serialized_end=2268
-  _globals['_CHARGINGSTATUS']._serialized_start=2270
-  _globals['_CHARGINGSTATUS']._serialized_end=2345
-  _globals['_CONNECTORSTANDARD']._serialized_start=2347
-  _globals['_CONNECTORSTANDARD']._serialized_end=2441
-  _globals['_CONNECTORFORMAT']._serialized_start=2443
-  _globals['_CONNECTORFORMAT']._serialized_end=2518
-  _globals['_POWERTYPE']._serialized_start=2520
-  _globals['_POWERTYPE']._serialized_end=2574
-  _globals['_FEENAME']._serialized_start=2576
-  _globals['_FEENAME']._serialized_end=2651
-  _globals['_FEETYPE']._serialized_start=2653
-  _globals['_FEETYPE']._serialized_end=2714
+  _globals['_IMAGECATEGORY']._serialized_start=2482
+  _globals['_IMAGECATEGORY']._serialized_end=2554
+  _globals['_CHARGINGSTATUS']._serialized_start=2556
+  _globals['_CHARGINGSTATUS']._serialized_end=2631
+  _globals['_CONNECTORSTANDARD']._serialized_start=2633
+  _globals['_CONNECTORSTANDARD']._serialized_end=2727
+  _globals['_CONNECTORFORMAT']._serialized_start=2729
+  _globals['_CONNECTORFORMAT']._serialized_end=2804
+  _globals['_POWERTYPE']._serialized_start=2806
+  _globals['_POWERTYPE']._serialized_end=2860
+  _globals['_FEENAME']._serialized_start=2862
+  _globals['_FEENAME']._serialized_end=2937
+  _globals['_FEETYPE']._serialized_start=2939
+  _globals['_FEETYPE']._serialized_end=3000
   _globals['_DATETIME']._serialized_start=77
   _globals['_DATETIME']._serialized_end=104
   _globals['_UNKNOWN']._serialized_start=106
   _globals['_UNKNOWN']._serialized_end=115
   _globals['_IMAGE']._serialized_start=117
   _globals['_IMAGE']._serialized_end=206
   _globals['_OPERATOR']._serialized_start=208
   _globals['_OPERATOR']._serialized_end=275
   _globals['_CONNECTOR']._serialized_start=278
-  _globals['_CONNECTOR']._serialized_end=557
-  _globals['_CHARGINGSESSION']._serialized_start=560
-  _globals['_CHARGINGSESSION']._serialized_end=795
-  _globals['_OPENINGTIMES']._serialized_start=797
-  _globals['_OPENINGTIMES']._serialized_end=836
-  _globals['_CHARGINGLOCATION']._serialized_start=839
-  _globals['_CHARGINGLOCATION']._serialized_end=1256
-  _globals['_FEE']._serialized_start=1258
-  _globals['_FEE']._serialized_end=1374
-  _globals['_CDR']._serialized_start=1377
-  _globals['_CDR']._serialized_end=1755
-  _globals['_GETCDRREQUEST']._serialized_start=1757
-  _globals['_GETCDRREQUEST']._serialized_end=1772
-  _globals['_GETCDRRESPONSE']._serialized_start=1774
-  _globals['_GETCDRRESPONSE']._serialized_end=1790
-  _globals['_GETCDRSREQUEST']._serialized_start=1792
-  _globals['_GETCDRSREQUEST']._serialized_end=1839
-  _globals['_GETCDRSRESPONSE']._serialized_start=1841
-  _globals['_GETCDRSRESPONSE']._serialized_end=1898
-  _globals['_GETLOCATIONSBOXREQUEST']._serialized_start=1900
-  _globals['_GETLOCATIONSBOXREQUEST']._serialized_end=1924
-  _globals['_GETLOCATIONSBOXRESPONSE']._serialized_start=1926
-  _globals['_GETLOCATIONSBOXRESPONSE']._serialized_end=1951
-  _globals['_GETLOCATIONSBYRADIUSREQUEST']._serialized_start=1953
-  _globals['_GETLOCATIONSBYRADIUSREQUEST']._serialized_end=1982
-  _globals['_GETLOCATIONSBYRADIUSRESPONSE']._serialized_start=1984
-  _globals['_GETLOCATIONSBYRADIUSRESPONSE']._serialized_end=2014
-  _globals['_GETTARIFFREQUEST']._serialized_start=2016
-  _globals['_GETTARIFFREQUEST']._serialized_end=2034
-  _globals['_GETTARIFFRESPONSE']._serialized_start=2036
-  _globals['_GETTARIFFRESPONSE']._serialized_end=2055
-  _globals['_REGISTERRFIDREQUEST']._serialized_start=2057
-  _globals['_REGISTERRFIDREQUEST']._serialized_end=2078
-  _globals['_REGISTERRFIDRESPONSE']._serialized_start=2080
-  _globals['_REGISTERRFIDRESPONSE']._serialized_end=2102
-  _globals['_STARTSESSIONREQUEST']._serialized_start=2104
-  _globals['_STARTSESSIONREQUEST']._serialized_end=2125
-  _globals['_STARTSESSIONRESPONSE']._serialized_start=2127
-  _globals['_STARTSESSIONRESPONSE']._serialized_end=2149
-  _globals['_STOPSESSIONREQUEST']._serialized_start=2151
-  _globals['_STOPSESSIONREQUEST']._serialized_end=2171
-  _globals['_STOPSESSIONRESPONSE']._serialized_start=2173
-  _globals['_STOPSESSIONRESPONSE']._serialized_end=2194
-  _globals['_CHARGINGSERVICE']._serialized_start=2717
-  _globals['_CHARGINGSERVICE']._serialized_end=3562
+  _globals['_CONNECTOR']._serialized_end=572
+  _globals['_CHARGINGSESSION']._serialized_start=575
+  _globals['_CHARGINGSESSION']._serialized_end=810
+  _globals['_OPENINGTIMES']._serialized_start=812
+  _globals['_OPENINGTIMES']._serialized_end=851
+  _globals['_CHARGINGLOCATION']._serialized_start=854
+  _globals['_CHARGINGLOCATION']._serialized_end=1271
+  _globals['_FEE']._serialized_start=1273
+  _globals['_FEE']._serialized_end=1389
+  _globals['_CDR']._serialized_start=1392
+  _globals['_CDR']._serialized_end=1770
+  _globals['_GETCDRREQUEST']._serialized_start=1772
+  _globals['_GETCDRREQUEST']._serialized_end=1787
+  _globals['_GETCDRRESPONSE']._serialized_start=1789
+  _globals['_GETCDRRESPONSE']._serialized_end=1805
+  _globals['_GETCDRSREQUEST']._serialized_start=1807
+  _globals['_GETCDRSREQUEST']._serialized_end=1854
+  _globals['_GETCDRSRESPONSE']._serialized_start=1856
+  _globals['_GETCDRSRESPONSE']._serialized_end=1913
+  _globals['_GETLOCATIONSBOXREQUEST']._serialized_start=1915
+  _globals['_GETLOCATIONSBOXREQUEST']._serialized_end=1939
+  _globals['_GETLOCATIONSBOXRESPONSE']._serialized_start=1941
+  _globals['_GETLOCATIONSBOXRESPONSE']._serialized_end=1966
+  _globals['_CHARGINGLOCATIONDISTANCE']._serialized_start=1968
+  _globals['_CHARGINGLOCATIONDISTANCE']._serialized_end=2070
+  _globals['_GETLOCATIONSBYRADIUSREQUEST']._serialized_start=2072
+  _globals['_GETLOCATIONSBYRADIUSREQUEST']._serialized_end=2165
+  _globals['_GETLOCATIONSBYRADIUSRESPONSE']._serialized_start=2167
+  _globals['_GETLOCATIONSBYRADIUSRESPONSE']._serialized_end=2264
+  _globals['_GETTARIFFREQUEST']._serialized_start=2266
+  _globals['_GETTARIFFREQUEST']._serialized_end=2284
+  _globals['_GETTARIFFRESPONSE']._serialized_start=2286
+  _globals['_GETTARIFFRESPONSE']._serialized_end=2305
+  _globals['_REGISTERRFIDREQUEST']._serialized_start=2307
+  _globals['_REGISTERRFIDREQUEST']._serialized_end=2364
+  _globals['_REGISTERRFIDRESPONSE']._serialized_start=2366
+  _globals['_REGISTERRFIDRESPONSE']._serialized_end=2388
+  _globals['_STARTSESSIONREQUEST']._serialized_start=2390
+  _globals['_STARTSESSIONREQUEST']._serialized_end=2411
+  _globals['_STARTSESSIONRESPONSE']._serialized_start=2413
+  _globals['_STARTSESSIONRESPONSE']._serialized_end=2435
+  _globals['_STOPSESSIONREQUEST']._serialized_start=2437
+  _globals['_STOPSESSIONREQUEST']._serialized_end=2457
+  _globals['_STOPSESSIONRESPONSE']._serialized_start=2459
+  _globals['_STOPSESSIONRESPONSE']._serialized_end=2480
+  _globals['_CHARGINGSERVICE']._serialized_start=3003
+  _globals['_CHARGINGSERVICE']._serialized_end=3848
 # @@protoc_insertion_point(module_scope)
```

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/charging_service_pb2.pyi` & `lucidmotors-1.1.2/lucidmotors/gen/charging_service_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -83,30 +83,32 @@
     NAME_FIELD_NUMBER: _ClassVar[int]
     LOGO_FIELD_NUMBER: _ClassVar[int]
     name: str
     logo: Image
     def __init__(self, name: _Optional[str] = ..., logo: _Optional[_Union[Image, _Mapping]] = ...) -> None: ...
 
 class Connector(_message.Message):
-    __slots__ = ("id", "standard", "format", "power_type", "voltage", "amperage", "status")
+    __slots__ = ("id", "standard", "format", "power_type", "voltage", "amperage", "status", "power")
     ID_FIELD_NUMBER: _ClassVar[int]
     STANDARD_FIELD_NUMBER: _ClassVar[int]
     FORMAT_FIELD_NUMBER: _ClassVar[int]
     POWER_TYPE_FIELD_NUMBER: _ClassVar[int]
     VOLTAGE_FIELD_NUMBER: _ClassVar[int]
     AMPERAGE_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
+    POWER_FIELD_NUMBER: _ClassVar[int]
     id: str
     standard: ConnectorStandard
     format: ConnectorFormat
     power_type: PowerType
     voltage: int
     amperage: int
     status: ChargingStatus
-    def __init__(self, id: _Optional[str] = ..., standard: _Optional[_Union[ConnectorStandard, str]] = ..., format: _Optional[_Union[ConnectorFormat, str]] = ..., power_type: _Optional[_Union[PowerType, str]] = ..., voltage: _Optional[int] = ..., amperage: _Optional[int] = ..., status: _Optional[_Union[ChargingStatus, str]] = ...) -> None: ...
+    power: int
+    def __init__(self, id: _Optional[str] = ..., standard: _Optional[_Union[ConnectorStandard, str]] = ..., format: _Optional[_Union[ConnectorFormat, str]] = ..., power_type: _Optional[_Union[PowerType, str]] = ..., voltage: _Optional[int] = ..., amperage: _Optional[int] = ..., status: _Optional[_Union[ChargingStatus, str]] = ..., power: _Optional[int] = ...) -> None: ...
 
 class ChargingSession(_message.Message):
     __slots__ = ("uid", "evse_id", "status", "connectors", "coordinates", "physical_reference")
     UID_FIELD_NUMBER: _ClassVar[int]
     EVSE_ID_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
     CONNECTORS_FIELD_NUMBER: _ClassVar[int]
@@ -220,33 +222,51 @@
     __slots__ = ()
     def __init__(self) -> None: ...
 
 class GetLocationsBoxResponse(_message.Message):
     __slots__ = ()
     def __init__(self) -> None: ...
 
+class ChargingLocationDistance(_message.Message):
+    __slots__ = ("location", "distance")
+    LOCATION_FIELD_NUMBER: _ClassVar[int]
+    DISTANCE_FIELD_NUMBER: _ClassVar[int]
+    location: ChargingLocation
+    distance: int
+    def __init__(self, location: _Optional[_Union[ChargingLocation, _Mapping]] = ..., distance: _Optional[int] = ...) -> None: ...
+
 class GetLocationsByRadiusRequest(_message.Message):
-    __slots__ = ()
-    def __init__(self) -> None: ...
+    __slots__ = ("origin", "radius")
+    ORIGIN_FIELD_NUMBER: _ClassVar[int]
+    RADIUS_FIELD_NUMBER: _ClassVar[int]
+    origin: _vehicle_state_service_pb2.Location
+    radius: int
+    def __init__(self, origin: _Optional[_Union[_vehicle_state_service_pb2.Location, _Mapping]] = ..., radius: _Optional[int] = ...) -> None: ...
 
 class GetLocationsByRadiusResponse(_message.Message):
-    __slots__ = ()
-    def __init__(self) -> None: ...
+    __slots__ = ("locations",)
+    LOCATIONS_FIELD_NUMBER: _ClassVar[int]
+    locations: _containers.RepeatedCompositeFieldContainer[ChargingLocationDistance]
+    def __init__(self, locations: _Optional[_Iterable[_Union[ChargingLocationDistance, _Mapping]]] = ...) -> None: ...
 
 class GetTariffRequest(_message.Message):
     __slots__ = ()
     def __init__(self) -> None: ...
 
 class GetTariffResponse(_message.Message):
     __slots__ = ()
     def __init__(self) -> None: ...
 
 class RegisterRFIDRequest(_message.Message):
-    __slots__ = ()
-    def __init__(self) -> None: ...
+    __slots__ = ("ema_id", "rfid_token")
+    EMA_ID_FIELD_NUMBER: _ClassVar[int]
+    RFID_TOKEN_FIELD_NUMBER: _ClassVar[int]
+    ema_id: str
+    rfid_token: str
+    def __init__(self, ema_id: _Optional[str] = ..., rfid_token: _Optional[str] = ...) -> None: ...
 
 class RegisterRFIDResponse(_message.Message):
     __slots__ = ()
     def __init__(self) -> None: ...
 
 class StartSessionRequest(_message.Message):
     __slots__ = ()
```

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/charging_service_pb2.pyi.orig` & `lucidmotors-1.1.2/lucidmotors/gen/charging_service_pb2.pyi.orig`

 * *Files 6% similar despite different names*

```diff
@@ -83,30 +83,32 @@
     NAME_FIELD_NUMBER: _ClassVar[int]
     LOGO_FIELD_NUMBER: _ClassVar[int]
     name: str
     logo: Image
     def __init__(self, name: _Optional[str] = ..., logo: _Optional[_Union[Image, _Mapping]] = ...) -> None: ...
 
 class Connector(_message.Message):
-    __slots__ = ("id", "standard", "format", "power_type", "voltage", "amperage", "status")
+    __slots__ = ("id", "standard", "format", "power_type", "voltage", "amperage", "status", "power")
     ID_FIELD_NUMBER: _ClassVar[int]
     STANDARD_FIELD_NUMBER: _ClassVar[int]
     FORMAT_FIELD_NUMBER: _ClassVar[int]
     POWER_TYPE_FIELD_NUMBER: _ClassVar[int]
     VOLTAGE_FIELD_NUMBER: _ClassVar[int]
     AMPERAGE_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
+    POWER_FIELD_NUMBER: _ClassVar[int]
     id: str
     standard: ConnectorStandard
     format: ConnectorFormat
     power_type: PowerType
     voltage: int
     amperage: int
     status: ChargingStatus
-    def __init__(self, id: _Optional[str] = ..., standard: _Optional[_Union[ConnectorStandard, str]] = ..., format: _Optional[_Union[ConnectorFormat, str]] = ..., power_type: _Optional[_Union[PowerType, str]] = ..., voltage: _Optional[int] = ..., amperage: _Optional[int] = ..., status: _Optional[_Union[ChargingStatus, str]] = ...) -> None: ...
+    power: int
+    def __init__(self, id: _Optional[str] = ..., standard: _Optional[_Union[ConnectorStandard, str]] = ..., format: _Optional[_Union[ConnectorFormat, str]] = ..., power_type: _Optional[_Union[PowerType, str]] = ..., voltage: _Optional[int] = ..., amperage: _Optional[int] = ..., status: _Optional[_Union[ChargingStatus, str]] = ..., power: _Optional[int] = ...) -> None: ...
 
 class ChargingSession(_message.Message):
     __slots__ = ("uid", "evse_id", "status", "connectors", "coordinates", "physical_reference")
     UID_FIELD_NUMBER: _ClassVar[int]
     EVSE_ID_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
     CONNECTORS_FIELD_NUMBER: _ClassVar[int]
@@ -220,33 +222,51 @@
     __slots__ = ()
     def __init__(self) -> None: ...
 
 class GetLocationsBoxResponse(_message.Message):
     __slots__ = ()
     def __init__(self) -> None: ...
 
+class ChargingLocationDistance(_message.Message):
+    __slots__ = ("location", "distance")
+    LOCATION_FIELD_NUMBER: _ClassVar[int]
+    DISTANCE_FIELD_NUMBER: _ClassVar[int]
+    location: ChargingLocation
+    distance: int
+    def __init__(self, location: _Optional[_Union[ChargingLocation, _Mapping]] = ..., distance: _Optional[int] = ...) -> None: ...
+
 class GetLocationsByRadiusRequest(_message.Message):
-    __slots__ = ()
-    def __init__(self) -> None: ...
+    __slots__ = ("origin", "radius")
+    ORIGIN_FIELD_NUMBER: _ClassVar[int]
+    RADIUS_FIELD_NUMBER: _ClassVar[int]
+    origin: _vehicle_state_service_pb2.Location
+    radius: int
+    def __init__(self, origin: _Optional[_Union[_vehicle_state_service_pb2.Location, _Mapping]] = ..., radius: _Optional[int] = ...) -> None: ...
 
 class GetLocationsByRadiusResponse(_message.Message):
-    __slots__ = ()
-    def __init__(self) -> None: ...
+    __slots__ = ("locations",)
+    LOCATIONS_FIELD_NUMBER: _ClassVar[int]
+    locations: _containers.RepeatedCompositeFieldContainer[ChargingLocationDistance]
+    def __init__(self, locations: _Optional[_Iterable[_Union[ChargingLocationDistance, _Mapping]]] = ...) -> None: ...
 
 class GetTariffRequest(_message.Message):
     __slots__ = ()
     def __init__(self) -> None: ...
 
 class GetTariffResponse(_message.Message):
     __slots__ = ()
     def __init__(self) -> None: ...
 
 class RegisterRFIDRequest(_message.Message):
-    __slots__ = ()
-    def __init__(self) -> None: ...
+    __slots__ = ("ema_id", "rfid_token")
+    EMA_ID_FIELD_NUMBER: _ClassVar[int]
+    RFID_TOKEN_FIELD_NUMBER: _ClassVar[int]
+    ema_id: str
+    rfid_token: str
+    def __init__(self, ema_id: _Optional[str] = ..., rfid_token: _Optional[str] = ...) -> None: ...
 
 class RegisterRFIDResponse(_message.Message):
     __slots__ = ()
     def __init__(self) -> None: ...
 
 class StartSessionRequest(_message.Message):
     __slots__ = ()
```

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/charging_service_pb2_grpc.py` & `lucidmotors-1.1.2/lucidmotors/gen/charging_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/charging_service_pb2_grpc.py.orig` & `lucidmotors-1.1.2/lucidmotors/gen/charging_service_pb2_grpc.py.orig`

 * *Files identical despite different names*

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/login_session_pb2.py` & `lucidmotors-1.1.2/lucidmotors/gen/login_session_pb2.py.orig`

 * *Files 4% similar despite different names*

```diff
@@ -8,33 +8,33 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from . import user_profile_service_pb2 as user__profile__service__pb2
-from . import vehicle_state_service_pb2 as vehicle__state__service__pb2
+import user_profile_service_pb2 as user__profile__service__pb2
+import vehicle_state_service_pb2 as vehicle__state__service__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13login_session.proto\x12\x14mobilegateway.protos\x1a\x1auser_profile_service.proto\x1a\x1bvehicle_state_service.proto\"\xad\x02\n\x0cLoginRequest\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12P\n\x19notification_channel_type\x18\x03 \x01(\x0e\x32-.mobilegateway.protos.NotificationChannelType\x12$\n\x02os\x18\x04 \x01(\x0e\x32\x18.mobilegateway.protos.Os\x12!\n\x19notification_device_token\x18\x05 \x01(\t\x12\x0e\n\x06locale\x18\x06 \x01(\t\x12\x16\n\tdevice_id\x18\x07 \x01(\tH\x00\x88\x01\x01\x12\x18\n\x0b\x63lient_name\x18\x08 \x01(\tH\x01\x88\x01\x01\x42\x0c\n\n_device_idB\x0e\n\x0c_client_name\"y\n\x0bSessionInfo\x12\x10\n\x08id_token\x18\x01 \x01(\t\x12\x17\n\x0f\x65xpiry_time_sec\x18\x02 \x01(\x05\x12\x1a\n\rrefresh_token\x18\x03 \x01(\tH\x00\x88\x01\x01\x12\x11\n\tgigya_jwt\x18\x04 \x01(\tB\x10\n\x0e_refresh_token\"\xb9\x02\n\rLoginResponse\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12\x37\n\x0csession_info\x18\x02 \x01(\x0b\x32!.mobilegateway.protos.SessionInfo\x12\x37\n\x0cuser_profile\x18\x03 \x01(\x0b\x32!.mobilegateway.protos.UserProfile\x12\x38\n\x11user_vehicle_data\x18\x04 \x03(\x0b\x32\x1d.mobilegateway.protos.Vehicle\x12\x39\n\rsubscriptions\x18\x05 \x03(\x0e\x32\".mobilegateway.protos.Subscription\x12\x34\n\nencryption\x18\x06 \x01(\x0e\x32 .mobilegateway.protos.Encryption\".\n\x15GetNewJWTTokenRequest\x12\x15\n\rrefresh_token\x18\x01 \x01(\t\"Q\n\x16GetNewJWTTokenResponse\x12\x37\n\x0csession_info\x18\x01 \x01(\x0b\x32!.mobilegateway.protos.SessionInfo\"\x18\n\x16\x43onfirmResetPinRequest\"\x19\n\x17\x43onfirmResetPinResponse\"\x18\n\x16GetSubscriptionRequest\"\x19\n\x17GetSubscriptionResponse\"\x18\n\x16GetUserVehiclesRequest\"S\n\x17GetUserVehiclesResponse\x12\x38\n\x11user_vehicle_data\x18\x01 \x03(\x0b\x32\x1d.mobilegateway.protos.Vehicle\"\x0f\n\rLogoutRequest\"\x10\n\x0eLogoutResponse\"!\n\x1fRefreshNotificationTokenRequest\"\"\n RefreshNotificationTokenResponse\":\n\x12SetNickNameRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\x12\x10\n\x08nickname\x18\x02 \x01(\t\"\x15\n\x13SetNickNameResponse\"\x18\n\x16SetSubscriptionRequest\"\x19\n\x17SetSubscriptionResponse*w\n\x17NotificationChannelType\x12 \n\x1cNOTIFICATION_CHANNEL_UNKNOWN\x10\x00\x12\x1c\n\x18NOTIFICATION_CHANNEL_ONE\x10\x01\x12\x1c\n\x18NOTIFICATION_CHANNEL_TWO\x10\x02*0\n\x02Os\x12\x0e\n\nOS_UNKNOWN\x10\x00\x12\n\n\x06OS_IOS\x10\x01\x12\x0e\n\nOS_ANDROID\x10\x02*\xe4\x01\n\x0cSubscription\x12\x18\n\x14SUBSCRIPTION_UNKNOWN\x10\x00\x12\x17\n\x13SUBSCRIPTION_CHARGE\x10\x01\x12\x19\n\x15SUBSCRIPTION_SECURITY\x10\x02\x12\x19\n\x15SUBSCRIPTION_SOFTWARE\x10\x03\x12\x15\n\x11SUBSCRIPTION_HVAC\x10\x04\x12\x19\n\x15SUBSCRIPTION_REQUIRED\x10\x05\x12\x1a\n\x16SUBSCRIPTION_CDR_EMAIL\x10\x06\x12\x1d\n\x19SUBSCRIPTION_SUBSCRIPTION\x10\x07*;\n\nEncryption\x12\x16\n\x12\x45NCRYPTION_UNKNOWN\x10\x00\x12\x15\n\x11\x45NCRYPTION_SINGLE\x10\x01\x32\xe4\x07\n\x0cLoginSession\x12p\n\x0f\x43onfirmResetPin\x12,.mobilegateway.protos.ConfirmResetPinRequest\x1a-.mobilegateway.protos.ConfirmResetPinResponse\"\x00\x12m\n\x0eGetNewJWTToken\x12+.mobilegateway.protos.GetNewJWTTokenRequest\x1a,.mobilegateway.protos.GetNewJWTTokenResponse\"\x00\x12p\n\x0fGetSubscription\x12,.mobilegateway.protos.GetSubscriptionRequest\x1a-.mobilegateway.protos.GetSubscriptionResponse\"\x00\x12p\n\x0fGetUserVehicles\x12,.mobilegateway.protos.GetUserVehiclesRequest\x1a-.mobilegateway.protos.GetUserVehiclesResponse\"\x00\x12R\n\x05Login\x12\".mobilegateway.protos.LoginRequest\x1a#.mobilegateway.protos.LoginResponse\"\x00\x12U\n\x06Logout\x12#.mobilegateway.protos.LogoutRequest\x1a$.mobilegateway.protos.LogoutResponse\"\x00\x12\x8b\x01\n\x18RefreshNotificationToken\x12\x35.mobilegateway.protos.RefreshNotificationTokenRequest\x1a\x36.mobilegateway.protos.RefreshNotificationTokenResponse\"\x00\x12\x64\n\x0bSetNickName\x12(.mobilegateway.protos.SetNickNameRequest\x1a).mobilegateway.protos.SetNickNameResponse\"\x00\x12p\n\x0fSetSubscription\x12,.mobilegateway.protos.SetSubscriptionRequest\x1a-.mobilegateway.protos.SetSubscriptionResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13login_session.proto\x12\x14mobilegateway.protos\x1a\x1auser_profile_service.proto\x1a\x1bvehicle_state_service.proto\"\xad\x02\n\x0cLoginRequest\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12P\n\x19notification_channel_type\x18\x03 \x01(\x0e\x32-.mobilegateway.protos.NotificationChannelType\x12$\n\x02os\x18\x04 \x01(\x0e\x32\x18.mobilegateway.protos.Os\x12!\n\x19notification_device_token\x18\x05 \x01(\t\x12\x0e\n\x06locale\x18\x06 \x01(\t\x12\x16\n\tdevice_id\x18\x07 \x01(\tH\x00\x88\x01\x01\x12\x18\n\x0b\x63lient_name\x18\x08 \x01(\tH\x01\x88\x01\x01\x42\x0c\n\n_device_idB\x0e\n\x0c_client_name\"y\n\x0bSessionInfo\x12\x10\n\x08id_token\x18\x01 \x01(\t\x12\x17\n\x0f\x65xpiry_time_sec\x18\x02 \x01(\x05\x12\x1a\n\rrefresh_token\x18\x03 \x01(\tH\x00\x88\x01\x01\x12\x11\n\tgigya_jwt\x18\x04 \x01(\tB\x10\n\x0e_refresh_token\"\xb9\x02\n\rLoginResponse\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12\x37\n\x0csession_info\x18\x02 \x01(\x0b\x32!.mobilegateway.protos.SessionInfo\x12\x37\n\x0cuser_profile\x18\x03 \x01(\x0b\x32!.mobilegateway.protos.UserProfile\x12\x38\n\x11user_vehicle_data\x18\x04 \x03(\x0b\x32\x1d.mobilegateway.protos.Vehicle\x12\x39\n\rsubscriptions\x18\x05 \x03(\x0e\x32\".mobilegateway.protos.Subscription\x12\x34\n\nencryption\x18\x06 \x01(\x0e\x32 .mobilegateway.protos.Encryption\".\n\x15GetNewJWTTokenRequest\x12\x15\n\rrefresh_token\x18\x01 \x01(\t\"Q\n\x16GetNewJWTTokenResponse\x12\x37\n\x0csession_info\x18\x01 \x01(\x0b\x32!.mobilegateway.protos.SessionInfo\"\x18\n\x16\x43onfirmResetPinRequest\"\x19\n\x17\x43onfirmResetPinResponse\"\x18\n\x16GetSubscriptionRequest\"T\n\x17GetSubscriptionResponse\x12\x39\n\rsubscriptions\x18\x01 \x03(\x0e\x32\".mobilegateway.protos.Subscription\"\x18\n\x16GetUserVehiclesRequest\"S\n\x17GetUserVehiclesResponse\x12\x38\n\x11user_vehicle_data\x18\x01 \x03(\x0b\x32\x1d.mobilegateway.protos.Vehicle\"\x0f\n\rLogoutRequest\"\x10\n\x0eLogoutResponse\"!\n\x1fRefreshNotificationTokenRequest\"\"\n RefreshNotificationTokenResponse\":\n\x12SetNickNameRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\x12\x10\n\x08nickname\x18\x02 \x01(\t\"\x15\n\x13SetNickNameResponse\"\x18\n\x16SetSubscriptionRequest\"\x19\n\x17SetSubscriptionResponse*w\n\x17NotificationChannelType\x12 \n\x1cNOTIFICATION_CHANNEL_UNKNOWN\x10\x00\x12\x1c\n\x18NOTIFICATION_CHANNEL_ONE\x10\x01\x12\x1c\n\x18NOTIFICATION_CHANNEL_TWO\x10\x02*0\n\x02Os\x12\x0e\n\nOS_UNKNOWN\x10\x00\x12\n\n\x06OS_IOS\x10\x01\x12\x0e\n\nOS_ANDROID\x10\x02*\xe4\x01\n\x0cSubscription\x12\x18\n\x14SUBSCRIPTION_UNKNOWN\x10\x00\x12\x17\n\x13SUBSCRIPTION_CHARGE\x10\x01\x12\x19\n\x15SUBSCRIPTION_SECURITY\x10\x02\x12\x19\n\x15SUBSCRIPTION_SOFTWARE\x10\x03\x12\x15\n\x11SUBSCRIPTION_HVAC\x10\x04\x12\x19\n\x15SUBSCRIPTION_REQUIRED\x10\x05\x12\x1a\n\x16SUBSCRIPTION_CDR_EMAIL\x10\x06\x12\x1d\n\x19SUBSCRIPTION_SUBSCRIPTION\x10\x07*;\n\nEncryption\x12\x16\n\x12\x45NCRYPTION_UNKNOWN\x10\x00\x12\x15\n\x11\x45NCRYPTION_SINGLE\x10\x01\x32\xe4\x07\n\x0cLoginSession\x12p\n\x0f\x43onfirmResetPin\x12,.mobilegateway.protos.ConfirmResetPinRequest\x1a-.mobilegateway.protos.ConfirmResetPinResponse\"\x00\x12m\n\x0eGetNewJWTToken\x12+.mobilegateway.protos.GetNewJWTTokenRequest\x1a,.mobilegateway.protos.GetNewJWTTokenResponse\"\x00\x12p\n\x0fGetSubscription\x12,.mobilegateway.protos.GetSubscriptionRequest\x1a-.mobilegateway.protos.GetSubscriptionResponse\"\x00\x12p\n\x0fGetUserVehicles\x12,.mobilegateway.protos.GetUserVehiclesRequest\x1a-.mobilegateway.protos.GetUserVehiclesResponse\"\x00\x12R\n\x05Login\x12\".mobilegateway.protos.LoginRequest\x1a#.mobilegateway.protos.LoginResponse\"\x00\x12U\n\x06Logout\x12#.mobilegateway.protos.LogoutRequest\x1a$.mobilegateway.protos.LogoutResponse\"\x00\x12\x8b\x01\n\x18RefreshNotificationToken\x12\x35.mobilegateway.protos.RefreshNotificationTokenRequest\x1a\x36.mobilegateway.protos.RefreshNotificationTokenResponse\"\x00\x12\x64\n\x0bSetNickName\x12(.mobilegateway.protos.SetNickNameRequest\x1a).mobilegateway.protos.SetNickNameResponse\"\x00\x12p\n\x0fSetSubscription\x12,.mobilegateway.protos.SetSubscriptionRequest\x1a-.mobilegateway.protos.SetSubscriptionResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'login_session_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
-  _globals['_NOTIFICATIONCHANNELTYPE']._serialized_start=1435
-  _globals['_NOTIFICATIONCHANNELTYPE']._serialized_end=1554
-  _globals['_OS']._serialized_start=1556
-  _globals['_OS']._serialized_end=1604
-  _globals['_SUBSCRIPTION']._serialized_start=1607
-  _globals['_SUBSCRIPTION']._serialized_end=1835
-  _globals['_ENCRYPTION']._serialized_start=1837
-  _globals['_ENCRYPTION']._serialized_end=1896
+  _globals['_NOTIFICATIONCHANNELTYPE']._serialized_start=1494
+  _globals['_NOTIFICATIONCHANNELTYPE']._serialized_end=1613
+  _globals['_OS']._serialized_start=1615
+  _globals['_OS']._serialized_end=1663
+  _globals['_SUBSCRIPTION']._serialized_start=1666
+  _globals['_SUBSCRIPTION']._serialized_end=1894
+  _globals['_ENCRYPTION']._serialized_start=1896
+  _globals['_ENCRYPTION']._serialized_end=1955
   _globals['_LOGINREQUEST']._serialized_start=103
   _globals['_LOGINREQUEST']._serialized_end=404
   _globals['_SESSIONINFO']._serialized_start=406
   _globals['_SESSIONINFO']._serialized_end=527
   _globals['_LOGINRESPONSE']._serialized_start=530
   _globals['_LOGINRESPONSE']._serialized_end=843
   _globals['_GETNEWJWTTOKENREQUEST']._serialized_start=845
@@ -44,31 +44,31 @@
   _globals['_CONFIRMRESETPINREQUEST']._serialized_start=976
   _globals['_CONFIRMRESETPINREQUEST']._serialized_end=1000
   _globals['_CONFIRMRESETPINRESPONSE']._serialized_start=1002
   _globals['_CONFIRMRESETPINRESPONSE']._serialized_end=1027
   _globals['_GETSUBSCRIPTIONREQUEST']._serialized_start=1029
   _globals['_GETSUBSCRIPTIONREQUEST']._serialized_end=1053
   _globals['_GETSUBSCRIPTIONRESPONSE']._serialized_start=1055
-  _globals['_GETSUBSCRIPTIONRESPONSE']._serialized_end=1080
-  _globals['_GETUSERVEHICLESREQUEST']._serialized_start=1082
-  _globals['_GETUSERVEHICLESREQUEST']._serialized_end=1106
-  _globals['_GETUSERVEHICLESRESPONSE']._serialized_start=1108
-  _globals['_GETUSERVEHICLESRESPONSE']._serialized_end=1191
-  _globals['_LOGOUTREQUEST']._serialized_start=1193
-  _globals['_LOGOUTREQUEST']._serialized_end=1208
-  _globals['_LOGOUTRESPONSE']._serialized_start=1210
-  _globals['_LOGOUTRESPONSE']._serialized_end=1226
-  _globals['_REFRESHNOTIFICATIONTOKENREQUEST']._serialized_start=1228
-  _globals['_REFRESHNOTIFICATIONTOKENREQUEST']._serialized_end=1261
-  _globals['_REFRESHNOTIFICATIONTOKENRESPONSE']._serialized_start=1263
-  _globals['_REFRESHNOTIFICATIONTOKENRESPONSE']._serialized_end=1297
-  _globals['_SETNICKNAMEREQUEST']._serialized_start=1299
-  _globals['_SETNICKNAMEREQUEST']._serialized_end=1357
-  _globals['_SETNICKNAMERESPONSE']._serialized_start=1359
-  _globals['_SETNICKNAMERESPONSE']._serialized_end=1380
-  _globals['_SETSUBSCRIPTIONREQUEST']._serialized_start=1382
-  _globals['_SETSUBSCRIPTIONREQUEST']._serialized_end=1406
-  _globals['_SETSUBSCRIPTIONRESPONSE']._serialized_start=1408
-  _globals['_SETSUBSCRIPTIONRESPONSE']._serialized_end=1433
-  _globals['_LOGINSESSION']._serialized_start=1899
-  _globals['_LOGINSESSION']._serialized_end=2895
+  _globals['_GETSUBSCRIPTIONRESPONSE']._serialized_end=1139
+  _globals['_GETUSERVEHICLESREQUEST']._serialized_start=1141
+  _globals['_GETUSERVEHICLESREQUEST']._serialized_end=1165
+  _globals['_GETUSERVEHICLESRESPONSE']._serialized_start=1167
+  _globals['_GETUSERVEHICLESRESPONSE']._serialized_end=1250
+  _globals['_LOGOUTREQUEST']._serialized_start=1252
+  _globals['_LOGOUTREQUEST']._serialized_end=1267
+  _globals['_LOGOUTRESPONSE']._serialized_start=1269
+  _globals['_LOGOUTRESPONSE']._serialized_end=1285
+  _globals['_REFRESHNOTIFICATIONTOKENREQUEST']._serialized_start=1287
+  _globals['_REFRESHNOTIFICATIONTOKENREQUEST']._serialized_end=1320
+  _globals['_REFRESHNOTIFICATIONTOKENRESPONSE']._serialized_start=1322
+  _globals['_REFRESHNOTIFICATIONTOKENRESPONSE']._serialized_end=1356
+  _globals['_SETNICKNAMEREQUEST']._serialized_start=1358
+  _globals['_SETNICKNAMEREQUEST']._serialized_end=1416
+  _globals['_SETNICKNAMERESPONSE']._serialized_start=1418
+  _globals['_SETNICKNAMERESPONSE']._serialized_end=1439
+  _globals['_SETSUBSCRIPTIONREQUEST']._serialized_start=1441
+  _globals['_SETSUBSCRIPTIONREQUEST']._serialized_end=1465
+  _globals['_SETSUBSCRIPTIONRESPONSE']._serialized_start=1467
+  _globals['_SETSUBSCRIPTIONRESPONSE']._serialized_end=1492
+  _globals['_LOGINSESSION']._serialized_start=1958
+  _globals['_LOGINSESSION']._serialized_end=2954
 # @@protoc_insertion_point(module_scope)
```

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/login_session_pb2.py.orig` & `lucidmotors-1.1.2/lucidmotors/gen/login_session_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,33 +8,33 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-import user_profile_service_pb2 as user__profile__service__pb2
-import vehicle_state_service_pb2 as vehicle__state__service__pb2
+from . import user_profile_service_pb2 as user__profile__service__pb2
+from . import vehicle_state_service_pb2 as vehicle__state__service__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13login_session.proto\x12\x14mobilegateway.protos\x1a\x1auser_profile_service.proto\x1a\x1bvehicle_state_service.proto\"\xad\x02\n\x0cLoginRequest\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12P\n\x19notification_channel_type\x18\x03 \x01(\x0e\x32-.mobilegateway.protos.NotificationChannelType\x12$\n\x02os\x18\x04 \x01(\x0e\x32\x18.mobilegateway.protos.Os\x12!\n\x19notification_device_token\x18\x05 \x01(\t\x12\x0e\n\x06locale\x18\x06 \x01(\t\x12\x16\n\tdevice_id\x18\x07 \x01(\tH\x00\x88\x01\x01\x12\x18\n\x0b\x63lient_name\x18\x08 \x01(\tH\x01\x88\x01\x01\x42\x0c\n\n_device_idB\x0e\n\x0c_client_name\"y\n\x0bSessionInfo\x12\x10\n\x08id_token\x18\x01 \x01(\t\x12\x17\n\x0f\x65xpiry_time_sec\x18\x02 \x01(\x05\x12\x1a\n\rrefresh_token\x18\x03 \x01(\tH\x00\x88\x01\x01\x12\x11\n\tgigya_jwt\x18\x04 \x01(\tB\x10\n\x0e_refresh_token\"\xb9\x02\n\rLoginResponse\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12\x37\n\x0csession_info\x18\x02 \x01(\x0b\x32!.mobilegateway.protos.SessionInfo\x12\x37\n\x0cuser_profile\x18\x03 \x01(\x0b\x32!.mobilegateway.protos.UserProfile\x12\x38\n\x11user_vehicle_data\x18\x04 \x03(\x0b\x32\x1d.mobilegateway.protos.Vehicle\x12\x39\n\rsubscriptions\x18\x05 \x03(\x0e\x32\".mobilegateway.protos.Subscription\x12\x34\n\nencryption\x18\x06 \x01(\x0e\x32 .mobilegateway.protos.Encryption\".\n\x15GetNewJWTTokenRequest\x12\x15\n\rrefresh_token\x18\x01 \x01(\t\"Q\n\x16GetNewJWTTokenResponse\x12\x37\n\x0csession_info\x18\x01 \x01(\x0b\x32!.mobilegateway.protos.SessionInfo\"\x18\n\x16\x43onfirmResetPinRequest\"\x19\n\x17\x43onfirmResetPinResponse\"\x18\n\x16GetSubscriptionRequest\"\x19\n\x17GetSubscriptionResponse\"\x18\n\x16GetUserVehiclesRequest\"S\n\x17GetUserVehiclesResponse\x12\x38\n\x11user_vehicle_data\x18\x01 \x03(\x0b\x32\x1d.mobilegateway.protos.Vehicle\"\x0f\n\rLogoutRequest\"\x10\n\x0eLogoutResponse\"!\n\x1fRefreshNotificationTokenRequest\"\"\n RefreshNotificationTokenResponse\":\n\x12SetNickNameRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\x12\x10\n\x08nickname\x18\x02 \x01(\t\"\x15\n\x13SetNickNameResponse\"\x18\n\x16SetSubscriptionRequest\"\x19\n\x17SetSubscriptionResponse*w\n\x17NotificationChannelType\x12 \n\x1cNOTIFICATION_CHANNEL_UNKNOWN\x10\x00\x12\x1c\n\x18NOTIFICATION_CHANNEL_ONE\x10\x01\x12\x1c\n\x18NOTIFICATION_CHANNEL_TWO\x10\x02*0\n\x02Os\x12\x0e\n\nOS_UNKNOWN\x10\x00\x12\n\n\x06OS_IOS\x10\x01\x12\x0e\n\nOS_ANDROID\x10\x02*\xe4\x01\n\x0cSubscription\x12\x18\n\x14SUBSCRIPTION_UNKNOWN\x10\x00\x12\x17\n\x13SUBSCRIPTION_CHARGE\x10\x01\x12\x19\n\x15SUBSCRIPTION_SECURITY\x10\x02\x12\x19\n\x15SUBSCRIPTION_SOFTWARE\x10\x03\x12\x15\n\x11SUBSCRIPTION_HVAC\x10\x04\x12\x19\n\x15SUBSCRIPTION_REQUIRED\x10\x05\x12\x1a\n\x16SUBSCRIPTION_CDR_EMAIL\x10\x06\x12\x1d\n\x19SUBSCRIPTION_SUBSCRIPTION\x10\x07*;\n\nEncryption\x12\x16\n\x12\x45NCRYPTION_UNKNOWN\x10\x00\x12\x15\n\x11\x45NCRYPTION_SINGLE\x10\x01\x32\xe4\x07\n\x0cLoginSession\x12p\n\x0f\x43onfirmResetPin\x12,.mobilegateway.protos.ConfirmResetPinRequest\x1a-.mobilegateway.protos.ConfirmResetPinResponse\"\x00\x12m\n\x0eGetNewJWTToken\x12+.mobilegateway.protos.GetNewJWTTokenRequest\x1a,.mobilegateway.protos.GetNewJWTTokenResponse\"\x00\x12p\n\x0fGetSubscription\x12,.mobilegateway.protos.GetSubscriptionRequest\x1a-.mobilegateway.protos.GetSubscriptionResponse\"\x00\x12p\n\x0fGetUserVehicles\x12,.mobilegateway.protos.GetUserVehiclesRequest\x1a-.mobilegateway.protos.GetUserVehiclesResponse\"\x00\x12R\n\x05Login\x12\".mobilegateway.protos.LoginRequest\x1a#.mobilegateway.protos.LoginResponse\"\x00\x12U\n\x06Logout\x12#.mobilegateway.protos.LogoutRequest\x1a$.mobilegateway.protos.LogoutResponse\"\x00\x12\x8b\x01\n\x18RefreshNotificationToken\x12\x35.mobilegateway.protos.RefreshNotificationTokenRequest\x1a\x36.mobilegateway.protos.RefreshNotificationTokenResponse\"\x00\x12\x64\n\x0bSetNickName\x12(.mobilegateway.protos.SetNickNameRequest\x1a).mobilegateway.protos.SetNickNameResponse\"\x00\x12p\n\x0fSetSubscription\x12,.mobilegateway.protos.SetSubscriptionRequest\x1a-.mobilegateway.protos.SetSubscriptionResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13login_session.proto\x12\x14mobilegateway.protos\x1a\x1auser_profile_service.proto\x1a\x1bvehicle_state_service.proto\"\xad\x02\n\x0cLoginRequest\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12P\n\x19notification_channel_type\x18\x03 \x01(\x0e\x32-.mobilegateway.protos.NotificationChannelType\x12$\n\x02os\x18\x04 \x01(\x0e\x32\x18.mobilegateway.protos.Os\x12!\n\x19notification_device_token\x18\x05 \x01(\t\x12\x0e\n\x06locale\x18\x06 \x01(\t\x12\x16\n\tdevice_id\x18\x07 \x01(\tH\x00\x88\x01\x01\x12\x18\n\x0b\x63lient_name\x18\x08 \x01(\tH\x01\x88\x01\x01\x42\x0c\n\n_device_idB\x0e\n\x0c_client_name\"y\n\x0bSessionInfo\x12\x10\n\x08id_token\x18\x01 \x01(\t\x12\x17\n\x0f\x65xpiry_time_sec\x18\x02 \x01(\x05\x12\x1a\n\rrefresh_token\x18\x03 \x01(\tH\x00\x88\x01\x01\x12\x11\n\tgigya_jwt\x18\x04 \x01(\tB\x10\n\x0e_refresh_token\"\xb9\x02\n\rLoginResponse\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12\x37\n\x0csession_info\x18\x02 \x01(\x0b\x32!.mobilegateway.protos.SessionInfo\x12\x37\n\x0cuser_profile\x18\x03 \x01(\x0b\x32!.mobilegateway.protos.UserProfile\x12\x38\n\x11user_vehicle_data\x18\x04 \x03(\x0b\x32\x1d.mobilegateway.protos.Vehicle\x12\x39\n\rsubscriptions\x18\x05 \x03(\x0e\x32\".mobilegateway.protos.Subscription\x12\x34\n\nencryption\x18\x06 \x01(\x0e\x32 .mobilegateway.protos.Encryption\".\n\x15GetNewJWTTokenRequest\x12\x15\n\rrefresh_token\x18\x01 \x01(\t\"Q\n\x16GetNewJWTTokenResponse\x12\x37\n\x0csession_info\x18\x01 \x01(\x0b\x32!.mobilegateway.protos.SessionInfo\"\x18\n\x16\x43onfirmResetPinRequest\"\x19\n\x17\x43onfirmResetPinResponse\"\x18\n\x16GetSubscriptionRequest\"T\n\x17GetSubscriptionResponse\x12\x39\n\rsubscriptions\x18\x01 \x03(\x0e\x32\".mobilegateway.protos.Subscription\"\x18\n\x16GetUserVehiclesRequest\"S\n\x17GetUserVehiclesResponse\x12\x38\n\x11user_vehicle_data\x18\x01 \x03(\x0b\x32\x1d.mobilegateway.protos.Vehicle\"\x0f\n\rLogoutRequest\"\x10\n\x0eLogoutResponse\"!\n\x1fRefreshNotificationTokenRequest\"\"\n RefreshNotificationTokenResponse\":\n\x12SetNickNameRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\x12\x10\n\x08nickname\x18\x02 \x01(\t\"\x15\n\x13SetNickNameResponse\"\x18\n\x16SetSubscriptionRequest\"\x19\n\x17SetSubscriptionResponse*w\n\x17NotificationChannelType\x12 \n\x1cNOTIFICATION_CHANNEL_UNKNOWN\x10\x00\x12\x1c\n\x18NOTIFICATION_CHANNEL_ONE\x10\x01\x12\x1c\n\x18NOTIFICATION_CHANNEL_TWO\x10\x02*0\n\x02Os\x12\x0e\n\nOS_UNKNOWN\x10\x00\x12\n\n\x06OS_IOS\x10\x01\x12\x0e\n\nOS_ANDROID\x10\x02*\xe4\x01\n\x0cSubscription\x12\x18\n\x14SUBSCRIPTION_UNKNOWN\x10\x00\x12\x17\n\x13SUBSCRIPTION_CHARGE\x10\x01\x12\x19\n\x15SUBSCRIPTION_SECURITY\x10\x02\x12\x19\n\x15SUBSCRIPTION_SOFTWARE\x10\x03\x12\x15\n\x11SUBSCRIPTION_HVAC\x10\x04\x12\x19\n\x15SUBSCRIPTION_REQUIRED\x10\x05\x12\x1a\n\x16SUBSCRIPTION_CDR_EMAIL\x10\x06\x12\x1d\n\x19SUBSCRIPTION_SUBSCRIPTION\x10\x07*;\n\nEncryption\x12\x16\n\x12\x45NCRYPTION_UNKNOWN\x10\x00\x12\x15\n\x11\x45NCRYPTION_SINGLE\x10\x01\x32\xe4\x07\n\x0cLoginSession\x12p\n\x0f\x43onfirmResetPin\x12,.mobilegateway.protos.ConfirmResetPinRequest\x1a-.mobilegateway.protos.ConfirmResetPinResponse\"\x00\x12m\n\x0eGetNewJWTToken\x12+.mobilegateway.protos.GetNewJWTTokenRequest\x1a,.mobilegateway.protos.GetNewJWTTokenResponse\"\x00\x12p\n\x0fGetSubscription\x12,.mobilegateway.protos.GetSubscriptionRequest\x1a-.mobilegateway.protos.GetSubscriptionResponse\"\x00\x12p\n\x0fGetUserVehicles\x12,.mobilegateway.protos.GetUserVehiclesRequest\x1a-.mobilegateway.protos.GetUserVehiclesResponse\"\x00\x12R\n\x05Login\x12\".mobilegateway.protos.LoginRequest\x1a#.mobilegateway.protos.LoginResponse\"\x00\x12U\n\x06Logout\x12#.mobilegateway.protos.LogoutRequest\x1a$.mobilegateway.protos.LogoutResponse\"\x00\x12\x8b\x01\n\x18RefreshNotificationToken\x12\x35.mobilegateway.protos.RefreshNotificationTokenRequest\x1a\x36.mobilegateway.protos.RefreshNotificationTokenResponse\"\x00\x12\x64\n\x0bSetNickName\x12(.mobilegateway.protos.SetNickNameRequest\x1a).mobilegateway.protos.SetNickNameResponse\"\x00\x12p\n\x0fSetSubscription\x12,.mobilegateway.protos.SetSubscriptionRequest\x1a-.mobilegateway.protos.SetSubscriptionResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'login_session_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
-  _globals['_NOTIFICATIONCHANNELTYPE']._serialized_start=1435
-  _globals['_NOTIFICATIONCHANNELTYPE']._serialized_end=1554
-  _globals['_OS']._serialized_start=1556
-  _globals['_OS']._serialized_end=1604
-  _globals['_SUBSCRIPTION']._serialized_start=1607
-  _globals['_SUBSCRIPTION']._serialized_end=1835
-  _globals['_ENCRYPTION']._serialized_start=1837
-  _globals['_ENCRYPTION']._serialized_end=1896
+  _globals['_NOTIFICATIONCHANNELTYPE']._serialized_start=1494
+  _globals['_NOTIFICATIONCHANNELTYPE']._serialized_end=1613
+  _globals['_OS']._serialized_start=1615
+  _globals['_OS']._serialized_end=1663
+  _globals['_SUBSCRIPTION']._serialized_start=1666
+  _globals['_SUBSCRIPTION']._serialized_end=1894
+  _globals['_ENCRYPTION']._serialized_start=1896
+  _globals['_ENCRYPTION']._serialized_end=1955
   _globals['_LOGINREQUEST']._serialized_start=103
   _globals['_LOGINREQUEST']._serialized_end=404
   _globals['_SESSIONINFO']._serialized_start=406
   _globals['_SESSIONINFO']._serialized_end=527
   _globals['_LOGINRESPONSE']._serialized_start=530
   _globals['_LOGINRESPONSE']._serialized_end=843
   _globals['_GETNEWJWTTOKENREQUEST']._serialized_start=845
@@ -44,31 +44,31 @@
   _globals['_CONFIRMRESETPINREQUEST']._serialized_start=976
   _globals['_CONFIRMRESETPINREQUEST']._serialized_end=1000
   _globals['_CONFIRMRESETPINRESPONSE']._serialized_start=1002
   _globals['_CONFIRMRESETPINRESPONSE']._serialized_end=1027
   _globals['_GETSUBSCRIPTIONREQUEST']._serialized_start=1029
   _globals['_GETSUBSCRIPTIONREQUEST']._serialized_end=1053
   _globals['_GETSUBSCRIPTIONRESPONSE']._serialized_start=1055
-  _globals['_GETSUBSCRIPTIONRESPONSE']._serialized_end=1080
-  _globals['_GETUSERVEHICLESREQUEST']._serialized_start=1082
-  _globals['_GETUSERVEHICLESREQUEST']._serialized_end=1106
-  _globals['_GETUSERVEHICLESRESPONSE']._serialized_start=1108
-  _globals['_GETUSERVEHICLESRESPONSE']._serialized_end=1191
-  _globals['_LOGOUTREQUEST']._serialized_start=1193
-  _globals['_LOGOUTREQUEST']._serialized_end=1208
-  _globals['_LOGOUTRESPONSE']._serialized_start=1210
-  _globals['_LOGOUTRESPONSE']._serialized_end=1226
-  _globals['_REFRESHNOTIFICATIONTOKENREQUEST']._serialized_start=1228
-  _globals['_REFRESHNOTIFICATIONTOKENREQUEST']._serialized_end=1261
-  _globals['_REFRESHNOTIFICATIONTOKENRESPONSE']._serialized_start=1263
-  _globals['_REFRESHNOTIFICATIONTOKENRESPONSE']._serialized_end=1297
-  _globals['_SETNICKNAMEREQUEST']._serialized_start=1299
-  _globals['_SETNICKNAMEREQUEST']._serialized_end=1357
-  _globals['_SETNICKNAMERESPONSE']._serialized_start=1359
-  _globals['_SETNICKNAMERESPONSE']._serialized_end=1380
-  _globals['_SETSUBSCRIPTIONREQUEST']._serialized_start=1382
-  _globals['_SETSUBSCRIPTIONREQUEST']._serialized_end=1406
-  _globals['_SETSUBSCRIPTIONRESPONSE']._serialized_start=1408
-  _globals['_SETSUBSCRIPTIONRESPONSE']._serialized_end=1433
-  _globals['_LOGINSESSION']._serialized_start=1899
-  _globals['_LOGINSESSION']._serialized_end=2895
+  _globals['_GETSUBSCRIPTIONRESPONSE']._serialized_end=1139
+  _globals['_GETUSERVEHICLESREQUEST']._serialized_start=1141
+  _globals['_GETUSERVEHICLESREQUEST']._serialized_end=1165
+  _globals['_GETUSERVEHICLESRESPONSE']._serialized_start=1167
+  _globals['_GETUSERVEHICLESRESPONSE']._serialized_end=1250
+  _globals['_LOGOUTREQUEST']._serialized_start=1252
+  _globals['_LOGOUTREQUEST']._serialized_end=1267
+  _globals['_LOGOUTRESPONSE']._serialized_start=1269
+  _globals['_LOGOUTRESPONSE']._serialized_end=1285
+  _globals['_REFRESHNOTIFICATIONTOKENREQUEST']._serialized_start=1287
+  _globals['_REFRESHNOTIFICATIONTOKENREQUEST']._serialized_end=1320
+  _globals['_REFRESHNOTIFICATIONTOKENRESPONSE']._serialized_start=1322
+  _globals['_REFRESHNOTIFICATIONTOKENRESPONSE']._serialized_end=1356
+  _globals['_SETNICKNAMEREQUEST']._serialized_start=1358
+  _globals['_SETNICKNAMEREQUEST']._serialized_end=1416
+  _globals['_SETNICKNAMERESPONSE']._serialized_start=1418
+  _globals['_SETNICKNAMERESPONSE']._serialized_end=1439
+  _globals['_SETSUBSCRIPTIONREQUEST']._serialized_start=1441
+  _globals['_SETSUBSCRIPTIONREQUEST']._serialized_end=1465
+  _globals['_SETSUBSCRIPTIONRESPONSE']._serialized_start=1467
+  _globals['_SETSUBSCRIPTIONRESPONSE']._serialized_end=1492
+  _globals['_LOGINSESSION']._serialized_start=1958
+  _globals['_LOGINSESSION']._serialized_end=2954
 # @@protoc_insertion_point(module_scope)
```

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/login_session_pb2.pyi` & `lucidmotors-1.1.2/lucidmotors/gen/login_session_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -121,16 +121,18 @@
     def __init__(self) -> None: ...
 
 class GetSubscriptionRequest(_message.Message):
     __slots__ = ()
     def __init__(self) -> None: ...
 
 class GetSubscriptionResponse(_message.Message):
-    __slots__ = ()
-    def __init__(self) -> None: ...
+    __slots__ = ("subscriptions",)
+    SUBSCRIPTIONS_FIELD_NUMBER: _ClassVar[int]
+    subscriptions: _containers.RepeatedScalarFieldContainer[Subscription]
+    def __init__(self, subscriptions: _Optional[_Iterable[_Union[Subscription, str]]] = ...) -> None: ...
 
 class GetUserVehiclesRequest(_message.Message):
     __slots__ = ()
     def __init__(self) -> None: ...
 
 class GetUserVehiclesResponse(_message.Message):
     __slots__ = ("user_vehicle_data",)
```

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/login_session_pb2.pyi.orig` & `lucidmotors-1.1.2/lucidmotors/gen/login_session_pb2.pyi.orig`

 * *Files 1% similar despite different names*

```diff
@@ -121,16 +121,18 @@
     def __init__(self) -> None: ...
 
 class GetSubscriptionRequest(_message.Message):
     __slots__ = ()
     def __init__(self) -> None: ...
 
 class GetSubscriptionResponse(_message.Message):
-    __slots__ = ()
-    def __init__(self) -> None: ...
+    __slots__ = ("subscriptions",)
+    SUBSCRIPTIONS_FIELD_NUMBER: _ClassVar[int]
+    subscriptions: _containers.RepeatedScalarFieldContainer[Subscription]
+    def __init__(self, subscriptions: _Optional[_Iterable[_Union[Subscription, str]]] = ...) -> None: ...
 
 class GetUserVehiclesRequest(_message.Message):
     __slots__ = ()
     def __init__(self) -> None: ...
 
 class GetUserVehiclesResponse(_message.Message):
     __slots__ = ("user_vehicle_data",)
```

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/login_session_pb2_grpc.py` & `lucidmotors-1.1.2/lucidmotors/gen/login_session_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/login_session_pb2_grpc.py.orig` & `lucidmotors-1.1.2/lucidmotors/gen/login_session_pb2_grpc.py.orig`

 * *Files identical despite different names*

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/salesforce_service_pb2.py` & `lucidmotors-1.1.2/lucidmotors/gen/sentry_service_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: salesforce_service.proto
+# source: sentry_service.proto
 # Protobuf Python Version: 4.25.0
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18salesforce_service.proto\x12\x14mobilegateway.protos\"\x14\n\x12ServiceAppointment\")\n\'GetSalesForceServiceAppointmentsRequest\"\x8b\x01\n(GetSalesForceServiceAppointmentsResponse\x12\x0e\n\x06status\x18\x01 \x01(\t\x12>\n\x0c\x61ppointments\x18\x02 \x03(\x0b\x32(.mobilegateway.protos.ServiceAppointment\x12\x0f\n\x07\x63omment\x18\x03 \x01(\t2\xb9\x01\n\x11SalesforceService\x12\xa3\x01\n GetSalesForceServiceAppointments\x12=.mobilegateway.protos.GetSalesForceServiceAppointmentsRequest\x1a>.mobilegateway.protos.GetSalesForceServiceAppointmentsResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14sentry_service.proto\x12\x14mobilegateway.protos\"5\n\x10GetEventsRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\x12\r\n\x05limit\x18\x02 \x01(\r\"\x13\n\x11GetEventsResponse2o\n\rSentryService\x12^\n\tGetEvents\x12&.mobilegateway.protos.GetEventsRequest\x1a\'.mobilegateway.protos.GetEventsResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'salesforce_service_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sentry_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
-  _globals['_SERVICEAPPOINTMENT']._serialized_start=50
-  _globals['_SERVICEAPPOINTMENT']._serialized_end=70
-  _globals['_GETSALESFORCESERVICEAPPOINTMENTSREQUEST']._serialized_start=72
-  _globals['_GETSALESFORCESERVICEAPPOINTMENTSREQUEST']._serialized_end=113
-  _globals['_GETSALESFORCESERVICEAPPOINTMENTSRESPONSE']._serialized_start=116
-  _globals['_GETSALESFORCESERVICEAPPOINTMENTSRESPONSE']._serialized_end=255
-  _globals['_SALESFORCESERVICE']._serialized_start=258
-  _globals['_SALESFORCESERVICE']._serialized_end=443
+  _globals['_GETEVENTSREQUEST']._serialized_start=46
+  _globals['_GETEVENTSREQUEST']._serialized_end=99
+  _globals['_GETEVENTSRESPONSE']._serialized_start=101
+  _globals['_GETEVENTSRESPONSE']._serialized_end=120
+  _globals['_SENTRYSERVICE']._serialized_start=122
+  _globals['_SENTRYSERVICE']._serialized_end=233
 # @@protoc_insertion_point(module_scope)
```

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/salesforce_service_pb2.py.orig` & `lucidmotors-1.1.2/lucidmotors/gen/sentry_service_pb2.py.orig`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: salesforce_service.proto
+# source: sentry_service.proto
 # Protobuf Python Version: 4.25.0
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18salesforce_service.proto\x12\x14mobilegateway.protos\"\x14\n\x12ServiceAppointment\")\n\'GetSalesForceServiceAppointmentsRequest\"\x8b\x01\n(GetSalesForceServiceAppointmentsResponse\x12\x0e\n\x06status\x18\x01 \x01(\t\x12>\n\x0c\x61ppointments\x18\x02 \x03(\x0b\x32(.mobilegateway.protos.ServiceAppointment\x12\x0f\n\x07\x63omment\x18\x03 \x01(\t2\xb9\x01\n\x11SalesforceService\x12\xa3\x01\n GetSalesForceServiceAppointments\x12=.mobilegateway.protos.GetSalesForceServiceAppointmentsRequest\x1a>.mobilegateway.protos.GetSalesForceServiceAppointmentsResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14sentry_service.proto\x12\x14mobilegateway.protos\"5\n\x10GetEventsRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\x12\r\n\x05limit\x18\x02 \x01(\r\"\x13\n\x11GetEventsResponse2o\n\rSentryService\x12^\n\tGetEvents\x12&.mobilegateway.protos.GetEventsRequest\x1a\'.mobilegateway.protos.GetEventsResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'salesforce_service_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sentry_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
-  _globals['_SERVICEAPPOINTMENT']._serialized_start=50
-  _globals['_SERVICEAPPOINTMENT']._serialized_end=70
-  _globals['_GETSALESFORCESERVICEAPPOINTMENTSREQUEST']._serialized_start=72
-  _globals['_GETSALESFORCESERVICEAPPOINTMENTSREQUEST']._serialized_end=113
-  _globals['_GETSALESFORCESERVICEAPPOINTMENTSRESPONSE']._serialized_start=116
-  _globals['_GETSALESFORCESERVICEAPPOINTMENTSRESPONSE']._serialized_end=255
-  _globals['_SALESFORCESERVICE']._serialized_start=258
-  _globals['_SALESFORCESERVICE']._serialized_end=443
+  _globals['_GETEVENTSREQUEST']._serialized_start=46
+  _globals['_GETEVENTSREQUEST']._serialized_end=99
+  _globals['_GETEVENTSRESPONSE']._serialized_start=101
+  _globals['_GETEVENTSRESPONSE']._serialized_end=120
+  _globals['_SENTRYSERVICE']._serialized_start=122
+  _globals['_SENTRYSERVICE']._serialized_end=233
 # @@protoc_insertion_point(module_scope)
```

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/trip_service_pb2.py` & `lucidmotors-1.1.2/lucidmotors/gen/trip_service_pb2.py`

 * *Files identical despite different names*

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/trip_service_pb2.py.orig` & `lucidmotors-1.1.2/lucidmotors/gen/trip_service_pb2.py.orig`

 * *Files identical despite different names*

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/trip_service_pb2.pyi` & `lucidmotors-1.1.2/lucidmotors/gen/trip_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/trip_service_pb2.pyi.orig` & `lucidmotors-1.1.2/lucidmotors/gen/trip_service_pb2.pyi.orig`

 * *Files identical despite different names*

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/trip_service_pb2_grpc.py` & `lucidmotors-1.1.2/lucidmotors/gen/trip_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/trip_service_pb2_grpc.py.orig` & `lucidmotors-1.1.2/lucidmotors/gen/trip_service_pb2_grpc.py.orig`

 * *Files identical despite different names*

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/user_profile_service_pb2.py` & `lucidmotors-1.1.2/lucidmotors/gen/user_profile_service_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1auser_profile_service.proto\x12\x14mobilegateway.protos\"\x9b\x01\n\x0bUserProfile\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x13\n\x06locale\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x10\n\x08username\x18\x03 \x01(\t\x12\x16\n\tphoto_url\x18\x04 \x01(\tH\x01\x88\x01\x01\x12\x12\n\nfirst_name\x18\x05 \x01(\t\x12\x11\n\tlast_name\x18\x06 \x01(\tB\t\n\x07_localeB\x0c\n\n_photo_url\"\x1d\n\x0bPhoneNumber\x12\x0e\n\x06number\x18\x02 \x01(\t\"\xdd\x01\n\x0fUserProfileData\x12\x12\n\nfirst_name\x18\x01 \x01(\t\x12\x11\n\tlast_name\x18\x02 \x01(\t\x12\r\n\x05\x65mail\x18\x03 \x01(\t\x12\x0e\n\x06locale\x18\x04 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\x06 \x01(\t\x12\x0c\n\x04\x63ity\x18\x07 \x01(\t\x12\r\n\x05state\x18\x08 \x01(\t\x12\x13\n\x0bpostal_code\x18\t \x01(\t\x12\x0f\n\x07\x63ountry\x18\n \x01(\t\x12\x30\n\x05phone\x18\x0b \x01(\x0b\x32!.mobilegateway.protos.PhoneNumber\"\x17\n\x15SetUserProfileRequest\"\x18\n\x16SetUserProfileResponse\"\x17\n\x15GetUserProfileRequest\"P\n\x16GetUserProfileResponse\x12\x36\n\x07profile\x18\x01 \x01(\x0b\x32%.mobilegateway.protos.UserProfileData\"\x1f\n\x1dUploadUserProfilePhotoRequest\" \n\x1eUploadUserProfilePhotoResponse2\xfa\x02\n\x12UserProfileService\x12m\n\x0eGetUserProfile\x12+.mobilegateway.protos.GetUserProfileRequest\x1a,.mobilegateway.protos.GetUserProfileResponse\"\x00\x12m\n\x0eSetUserProfile\x12+.mobilegateway.protos.SetUserProfileRequest\x1a,.mobilegateway.protos.SetUserProfileResponse\"\x00\x12\x85\x01\n\x16UploadUserProfilePhoto\x12\x33.mobilegateway.protos.UploadUserProfilePhotoRequest\x1a\x34.mobilegateway.protos.UploadUserProfilePhotoResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1auser_profile_service.proto\x12\x14mobilegateway.protos\"\x9b\x01\n\x0bUserProfile\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x13\n\x06locale\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x10\n\x08username\x18\x03 \x01(\t\x12\x16\n\tphoto_url\x18\x04 \x01(\tH\x01\x88\x01\x01\x12\x12\n\nfirst_name\x18\x05 \x01(\t\x12\x11\n\tlast_name\x18\x06 \x01(\tB\t\n\x07_localeB\x0c\n\n_photo_url\"\x1d\n\x0bPhoneNumber\x12\x0e\n\x06number\x18\x02 \x01(\t\"\xdd\x01\n\x0fUserProfileData\x12\x12\n\nfirst_name\x18\x01 \x01(\t\x12\x11\n\tlast_name\x18\x02 \x01(\t\x12\r\n\x05\x65mail\x18\x03 \x01(\t\x12\x0e\n\x06locale\x18\x04 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\x06 \x01(\t\x12\x0c\n\x04\x63ity\x18\x07 \x01(\t\x12\r\n\x05state\x18\x08 \x01(\t\x12\x13\n\x0bpostal_code\x18\t \x01(\t\x12\x0f\n\x07\x63ountry\x18\n \x01(\t\x12\x30\n\x05phone\x18\x0b \x01(\x0b\x32!.mobilegateway.protos.PhoneNumber\"\x17\n\x15SetUserProfileRequest\"\x18\n\x16SetUserProfileResponse\"\x17\n\x15GetUserProfileRequest\"P\n\x16GetUserProfileResponse\x12\x36\n\x07profile\x18\x01 \x01(\x0b\x32%.mobilegateway.protos.UserProfileData\"4\n\x1dUploadUserProfilePhotoRequest\x12\x13\n\x0bphoto_bytes\x18\x01 \x01(\t\"3\n\x1eUploadUserProfilePhotoResponse\x12\x11\n\tphoto_url\x18\x01 \x01(\t2\xfa\x02\n\x12UserProfileService\x12m\n\x0eGetUserProfile\x12+.mobilegateway.protos.GetUserProfileRequest\x1a,.mobilegateway.protos.GetUserProfileResponse\"\x00\x12m\n\x0eSetUserProfile\x12+.mobilegateway.protos.SetUserProfileRequest\x1a,.mobilegateway.protos.SetUserProfileResponse\"\x00\x12\x85\x01\n\x16UploadUserProfilePhoto\x12\x33.mobilegateway.protos.UploadUserProfilePhotoRequest\x1a\x34.mobilegateway.protos.UploadUserProfilePhotoResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'user_profile_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_USERPROFILE']._serialized_start=53
@@ -32,13 +32,13 @@
   _globals['_SETUSERPROFILERESPONSE']._serialized_start=490
   _globals['_SETUSERPROFILERESPONSE']._serialized_end=514
   _globals['_GETUSERPROFILEREQUEST']._serialized_start=516
   _globals['_GETUSERPROFILEREQUEST']._serialized_end=539
   _globals['_GETUSERPROFILERESPONSE']._serialized_start=541
   _globals['_GETUSERPROFILERESPONSE']._serialized_end=621
   _globals['_UPLOADUSERPROFILEPHOTOREQUEST']._serialized_start=623
-  _globals['_UPLOADUSERPROFILEPHOTOREQUEST']._serialized_end=654
-  _globals['_UPLOADUSERPROFILEPHOTORESPONSE']._serialized_start=656
-  _globals['_UPLOADUSERPROFILEPHOTORESPONSE']._serialized_end=688
-  _globals['_USERPROFILESERVICE']._serialized_start=691
-  _globals['_USERPROFILESERVICE']._serialized_end=1069
+  _globals['_UPLOADUSERPROFILEPHOTOREQUEST']._serialized_end=675
+  _globals['_UPLOADUSERPROFILEPHOTORESPONSE']._serialized_start=677
+  _globals['_UPLOADUSERPROFILEPHOTORESPONSE']._serialized_end=728
+  _globals['_USERPROFILESERVICE']._serialized_start=731
+  _globals['_USERPROFILESERVICE']._serialized_end=1109
 # @@protoc_insertion_point(module_scope)
```

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/user_profile_service_pb2.py.orig` & `lucidmotors-1.1.2/lucidmotors/gen/user_profile_service_pb2.py.orig`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1auser_profile_service.proto\x12\x14mobilegateway.protos\"\x9b\x01\n\x0bUserProfile\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x13\n\x06locale\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x10\n\x08username\x18\x03 \x01(\t\x12\x16\n\tphoto_url\x18\x04 \x01(\tH\x01\x88\x01\x01\x12\x12\n\nfirst_name\x18\x05 \x01(\t\x12\x11\n\tlast_name\x18\x06 \x01(\tB\t\n\x07_localeB\x0c\n\n_photo_url\"\x1d\n\x0bPhoneNumber\x12\x0e\n\x06number\x18\x02 \x01(\t\"\xdd\x01\n\x0fUserProfileData\x12\x12\n\nfirst_name\x18\x01 \x01(\t\x12\x11\n\tlast_name\x18\x02 \x01(\t\x12\r\n\x05\x65mail\x18\x03 \x01(\t\x12\x0e\n\x06locale\x18\x04 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\x06 \x01(\t\x12\x0c\n\x04\x63ity\x18\x07 \x01(\t\x12\r\n\x05state\x18\x08 \x01(\t\x12\x13\n\x0bpostal_code\x18\t \x01(\t\x12\x0f\n\x07\x63ountry\x18\n \x01(\t\x12\x30\n\x05phone\x18\x0b \x01(\x0b\x32!.mobilegateway.protos.PhoneNumber\"\x17\n\x15SetUserProfileRequest\"\x18\n\x16SetUserProfileResponse\"\x17\n\x15GetUserProfileRequest\"P\n\x16GetUserProfileResponse\x12\x36\n\x07profile\x18\x01 \x01(\x0b\x32%.mobilegateway.protos.UserProfileData\"\x1f\n\x1dUploadUserProfilePhotoRequest\" \n\x1eUploadUserProfilePhotoResponse2\xfa\x02\n\x12UserProfileService\x12m\n\x0eGetUserProfile\x12+.mobilegateway.protos.GetUserProfileRequest\x1a,.mobilegateway.protos.GetUserProfileResponse\"\x00\x12m\n\x0eSetUserProfile\x12+.mobilegateway.protos.SetUserProfileRequest\x1a,.mobilegateway.protos.SetUserProfileResponse\"\x00\x12\x85\x01\n\x16UploadUserProfilePhoto\x12\x33.mobilegateway.protos.UploadUserProfilePhotoRequest\x1a\x34.mobilegateway.protos.UploadUserProfilePhotoResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1auser_profile_service.proto\x12\x14mobilegateway.protos\"\x9b\x01\n\x0bUserProfile\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x13\n\x06locale\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x10\n\x08username\x18\x03 \x01(\t\x12\x16\n\tphoto_url\x18\x04 \x01(\tH\x01\x88\x01\x01\x12\x12\n\nfirst_name\x18\x05 \x01(\t\x12\x11\n\tlast_name\x18\x06 \x01(\tB\t\n\x07_localeB\x0c\n\n_photo_url\"\x1d\n\x0bPhoneNumber\x12\x0e\n\x06number\x18\x02 \x01(\t\"\xdd\x01\n\x0fUserProfileData\x12\x12\n\nfirst_name\x18\x01 \x01(\t\x12\x11\n\tlast_name\x18\x02 \x01(\t\x12\r\n\x05\x65mail\x18\x03 \x01(\t\x12\x0e\n\x06locale\x18\x04 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\x06 \x01(\t\x12\x0c\n\x04\x63ity\x18\x07 \x01(\t\x12\r\n\x05state\x18\x08 \x01(\t\x12\x13\n\x0bpostal_code\x18\t \x01(\t\x12\x0f\n\x07\x63ountry\x18\n \x01(\t\x12\x30\n\x05phone\x18\x0b \x01(\x0b\x32!.mobilegateway.protos.PhoneNumber\"\x17\n\x15SetUserProfileRequest\"\x18\n\x16SetUserProfileResponse\"\x17\n\x15GetUserProfileRequest\"P\n\x16GetUserProfileResponse\x12\x36\n\x07profile\x18\x01 \x01(\x0b\x32%.mobilegateway.protos.UserProfileData\"4\n\x1dUploadUserProfilePhotoRequest\x12\x13\n\x0bphoto_bytes\x18\x01 \x01(\t\"3\n\x1eUploadUserProfilePhotoResponse\x12\x11\n\tphoto_url\x18\x01 \x01(\t2\xfa\x02\n\x12UserProfileService\x12m\n\x0eGetUserProfile\x12+.mobilegateway.protos.GetUserProfileRequest\x1a,.mobilegateway.protos.GetUserProfileResponse\"\x00\x12m\n\x0eSetUserProfile\x12+.mobilegateway.protos.SetUserProfileRequest\x1a,.mobilegateway.protos.SetUserProfileResponse\"\x00\x12\x85\x01\n\x16UploadUserProfilePhoto\x12\x33.mobilegateway.protos.UploadUserProfilePhotoRequest\x1a\x34.mobilegateway.protos.UploadUserProfilePhotoResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'user_profile_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_USERPROFILE']._serialized_start=53
@@ -32,13 +32,13 @@
   _globals['_SETUSERPROFILERESPONSE']._serialized_start=490
   _globals['_SETUSERPROFILERESPONSE']._serialized_end=514
   _globals['_GETUSERPROFILEREQUEST']._serialized_start=516
   _globals['_GETUSERPROFILEREQUEST']._serialized_end=539
   _globals['_GETUSERPROFILERESPONSE']._serialized_start=541
   _globals['_GETUSERPROFILERESPONSE']._serialized_end=621
   _globals['_UPLOADUSERPROFILEPHOTOREQUEST']._serialized_start=623
-  _globals['_UPLOADUSERPROFILEPHOTOREQUEST']._serialized_end=654
-  _globals['_UPLOADUSERPROFILEPHOTORESPONSE']._serialized_start=656
-  _globals['_UPLOADUSERPROFILEPHOTORESPONSE']._serialized_end=688
-  _globals['_USERPROFILESERVICE']._serialized_start=691
-  _globals['_USERPROFILESERVICE']._serialized_end=1069
+  _globals['_UPLOADUSERPROFILEPHOTOREQUEST']._serialized_end=675
+  _globals['_UPLOADUSERPROFILEPHOTORESPONSE']._serialized_start=677
+  _globals['_UPLOADUSERPROFILEPHOTORESPONSE']._serialized_end=728
+  _globals['_USERPROFILESERVICE']._serialized_start=731
+  _globals['_USERPROFILESERVICE']._serialized_end=1109
 # @@protoc_insertion_point(module_scope)
```

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/user_profile_service_pb2.pyi` & `lucidmotors-1.1.2/lucidmotors/gen/user_profile_service_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -65,13 +65,17 @@
 class GetUserProfileResponse(_message.Message):
     __slots__ = ("profile",)
     PROFILE_FIELD_NUMBER: _ClassVar[int]
     profile: UserProfileData
     def __init__(self, profile: _Optional[_Union[UserProfileData, _Mapping]] = ...) -> None: ...
 
 class UploadUserProfilePhotoRequest(_message.Message):
-    __slots__ = ()
-    def __init__(self) -> None: ...
+    __slots__ = ("photo_bytes",)
+    PHOTO_BYTES_FIELD_NUMBER: _ClassVar[int]
+    photo_bytes: str
+    def __init__(self, photo_bytes: _Optional[str] = ...) -> None: ...
 
 class UploadUserProfilePhotoResponse(_message.Message):
-    __slots__ = ()
-    def __init__(self) -> None: ...
+    __slots__ = ("photo_url",)
+    PHOTO_URL_FIELD_NUMBER: _ClassVar[int]
+    photo_url: str
+    def __init__(self, photo_url: _Optional[str] = ...) -> None: ...
```

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/user_profile_service_pb2.pyi.orig` & `lucidmotors-1.1.2/lucidmotors/gen/user_profile_service_pb2.pyi.orig`

 * *Files 12% similar despite different names*

```diff
@@ -65,13 +65,17 @@
 class GetUserProfileResponse(_message.Message):
     __slots__ = ("profile",)
     PROFILE_FIELD_NUMBER: _ClassVar[int]
     profile: UserProfileData
     def __init__(self, profile: _Optional[_Union[UserProfileData, _Mapping]] = ...) -> None: ...
 
 class UploadUserProfilePhotoRequest(_message.Message):
-    __slots__ = ()
-    def __init__(self) -> None: ...
+    __slots__ = ("photo_bytes",)
+    PHOTO_BYTES_FIELD_NUMBER: _ClassVar[int]
+    photo_bytes: str
+    def __init__(self, photo_bytes: _Optional[str] = ...) -> None: ...
 
 class UploadUserProfilePhotoResponse(_message.Message):
-    __slots__ = ()
-    def __init__(self) -> None: ...
+    __slots__ = ("photo_url",)
+    PHOTO_URL_FIELD_NUMBER: _ClassVar[int]
+    photo_url: str
+    def __init__(self, photo_url: _Optional[str] = ...) -> None: ...
```

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/user_profile_service_pb2_grpc.py` & `lucidmotors-1.1.2/lucidmotors/gen/user_profile_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/user_profile_service_pb2_grpc.py.orig` & `lucidmotors-1.1.2/lucidmotors/gen/user_profile_service_pb2_grpc.py.orig`

 * *Files identical despite different names*

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/vehicle_state_service_pb2.py` & `lucidmotors-1.1.2/lucidmotors/gen/vehicle_state_service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,111 +10,117 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bvehicle_state_service.proto\x12\x14mobilegateway.protos\"\x8b\x01\n\x14\x43hargingSubscription\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x17\n\x0f\x65xpiration_date\x18\x02 \x01(\x04\x12\x12\n\nstart_date\x18\x03 \x01(\x04\x12\x38\n\x06status\x18\x04 \x01(\x0e\x32(.mobilegateway.protos.SubscriptionStatus\"\xe8\x01\n\x0f\x43hargingAccount\x12\x0e\n\x06\x65ma_id\x18\x01 \x01(\t\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\x12;\n\x06status\x18\x03 \x01(\x0e\x32+.mobilegateway.protos.ChargingAccountStatus\x12\x1c\n\x14\x63reated_at_epoch_sec\x18\x04 \x01(\x04\x12\x1b\n\x13\x65xpiry_on_epoch_sec\x18\x05 \x01(\x04\x12\x39\n\x0bvendor_name\x18\x06 \x01(\x0e\x32$.mobilegateway.protos.ChargingVendor\"(\n\x12SpecialIdentifiers\x12\x12\n\ndoor_plate\x18\x01 \x01(\t\"\x1b\n\x0bReservation\x12\x0c\n\x04\x64\x61te\x18\x01 \x01(\x04\"\x93\x07\n\rVehicleConfig\x12\x0b\n\x03vin\x18\x01 \x01(\t\x12*\n\x05model\x18\x02 \x01(\x0e\x32\x1b.mobilegateway.protos.Model\x12\x33\n\x07variant\x18\x03 \x01(\x0e\x32\".mobilegateway.protos.ModelVariant\x12\x10\n\x08nickname\x18\x05 \x01(\t\x12\x35\n\x0bpaint_color\x18\x06 \x01(\x0e\x32 .mobilegateway.protos.PaintColor\x12\x0e\n\x06\x65ma_id\x18\x07 \x01(\t\x12,\n\x06wheels\x18\x08 \x01(\x0e\x32\x1c.mobilegateway.protos.Wheels\x12\x43\n\x0f\x65\x61_subscription\x18\t \x01(\x0b\x32*.mobilegateway.protos.ChargingSubscription\x12@\n\x11\x63harging_accounts\x18\n \x03(\x0b\x32%.mobilegateway.protos.ChargingAccount\x12\x14\n\x0c\x63ountry_code\x18\x0b \x01(\t\x12\x13\n\x0bregion_code\x18\x0c \x01(\t\x12.\n\x07\x65\x64ition\x18\r \x01(\x0e\x32\x1d.mobilegateway.protos.Edition\x12\x32\n\x07\x62\x61ttery\x18\x0e \x01(\x0e\x32!.mobilegateway.protos.BatteryType\x12\x30\n\x08interior\x18\x0f \x01(\x0e\x32\x1e.mobilegateway.protos.Interior\x12\x45\n\x13special_identifiers\x18\x10 \x01(\x0b\x32(.mobilegateway.protos.SpecialIdentifiers\x12(\n\x04look\x18\x11 \x01(\x0e\x32\x1a.mobilegateway.protos.Look\x12\x1b\n\x13\x65xterior_color_code\x18\x12 \x01(\t\x12\x1b\n\x13interior_color_code\x18\x13 \x01(\t\x12\x34\n\x0b\x66runk_strut\x18\x14 \x01(\x0e\x32\x1f.mobilegateway.protos.StrutType\x12\x36\n\x0breservation\x18\x15 \x01(\x0b\x32!.mobilegateway.protos.Reservation\x12,\n\x04roof\x18\x16 \x01(\x0e\x32\x1e.mobilegateway.protos.RoofType\"\xaf\x03\n\x0c\x42\x61tteryState\x12\x17\n\x0fremaining_range\x18\x01 \x01(\x01\x12\x16\n\x0e\x63harge_percent\x18\x02 \x01(\x01\x12\x0c\n\x04kwhr\x18\x03 \x01(\x01\x12\x15\n\rcapacity_kwhr\x18\x04 \x01(\x01\x12:\n\x0e\x62\x61ttery_health\x18\x05 \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12<\n\x10low_charge_level\x18\x06 \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12\x41\n\x15\x63ritical_charge_level\x18\x07 \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12\x19\n\x11unavailable_range\x18\x08 \x01(\x01\x12I\n\x16preconditioning_status\x18\t \x01(\x0e\x32).mobilegateway.protos.BatteryPreconStatus\x12&\n\x1epreconditioning_time_remaining\x18\n \x01(\r\":\n\nCabinState\x12\x15\n\rinterior_temp\x18\x01 \x01(\x01\x12\x15\n\rexterior_temp\x18\x02 \x01(\x01\"\xc6\x04\n\tBodyState\x12\x33\n\ndoor_locks\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.LockState\x12\x34\n\x0b\x66ront_cargo\x18\x02 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x33\n\nrear_cargo\x18\x03 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x38\n\x0f\x66ront_left_door\x18\x04 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x39\n\x10\x66ront_right_door\x18\x05 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x37\n\x0erear_left_door\x18\x06 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x38\n\x0frear_right_door\x18\x07 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x34\n\x0b\x63harge_port\x18\x08 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12:\n\rwalkaway_lock\x18\t \x01(\x0e\x32#.mobilegateway.protos.WalkawayState\x12?\n\x12\x61\x63\x63\x65ss_type_status\x18\n \x01(\x0e\x32#.mobilegateway.protos.AccessRequest\"\x9b\x06\n\x0c\x43hassisState\x12\x13\n\x0bodometer_km\x18\x01 \x01(\x01\x12$\n\x1c\x66ront_left_tire_pressure_bar\x18\x02 \x01(\x01\x12%\n\x1d\x66ront_right_tire_pressure_bar\x18\x03 \x01(\x01\x12#\n\x1brear_left_tire_pressure_bar\x18\x04 \x01(\x01\x12$\n\x1crear_right_tire_pressure_bar\x18\x05 \x01(\x01\x12\x34\n\nheadlights\x18\x06 \x01(\x0e\x32 .mobilegateway.protos.LightState\x12@\n\x14hard_warn_left_front\x18\x08 \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12?\n\x13hard_warn_left_rear\x18\t \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12\x41\n\x15hard_warn_right_front\x18\n \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12@\n\x14hard_warn_right_rear\x18\x0b \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12@\n\x14soft_warn_left_front\x18\x0c \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12?\n\x13soft_warn_left_rear\x18\r \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12\x41\n\x15soft_warn_right_front\x18\x0e \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12@\n\x14soft_warn_right_rear\x18\x0f \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12\x18\n\x10software_version\x18\x10 \x01(\t\"\xed\x04\n\rChargingState\x12\x37\n\x0c\x63harge_state\x18\x01 \x01(\x0e\x32!.mobilegateway.protos.ChargeState\x12\x35\n\x0b\x65nergy_type\x18\x02 \x01(\x0e\x32 .mobilegateway.protos.EnergyType\x12\x19\n\x11\x63harge_session_mi\x18\x05 \x01(\x01\x12\x1a\n\x12\x63harge_session_kwh\x18\x06 \x01(\x01\x12!\n\x19session_minutes_remaining\x18\x07 \x01(\r\x12\x14\n\x0c\x63harge_limit\x18\x08 \x01(\r\x12\x33\n\ncable_lock\x18\n \x01(\x0e\x32\x1f.mobilegateway.protos.LockState\x12\x1f\n\x17\x63harge_rate_kwh_precise\x18\x0b \x01(\x01\x12\x1f\n\x17\x63harge_rate_mph_precise\x18\x0c \x01(\x01\x12%\n\x1d\x63harge_rate_miles_min_precise\x18\r \x01(\x01\x12\x1c\n\x14\x63harge_limit_percent\x18\x0e \x01(\x01\x12\x1d\n\x15\x63harge_scheduled_time\x18\x10 \x01(\r\x12\x44\n\x10scheduled_charge\x18\x11 \x01(\x0e\x32*.mobilegateway.protos.ScheduledChargeState\x12[\n\x1cscheduled_charge_unavailable\x18\x12 \x01(\x0e\x32\x35.mobilegateway.protos.ScheduledChargeUnavailableState\"/\n\x08Location\x12\x10\n\x08latitude\x18\x01 \x01(\x01\x12\x11\n\tlongitude\x18\x02 \x01(\x01\"z\n\x03Gps\x12\x30\n\x08location\x18\x01 \x01(\x0b\x32\x1e.mobilegateway.protos.Location\x12\x11\n\televation\x18\x02 \x01(\x05\x12\x15\n\rposition_time\x18\x04 \x01(\x04\x12\x17\n\x0fheading_precise\x18\x05 \x01(\x01\"\x9e\x02\n\x0eSoftwareUpdate\x12\x19\n\x11version_available\x18\x01 \x01(\t\x12 \n\x18install_duration_minutes\x18\x02 \x01(\r\x12\x18\n\x10percent_complete\x18\x04 \x01(\r\x12\x30\n\x05state\x18\x05 \x01(\x0e\x32!.mobilegateway.protos.UpdateState\x12\x1d\n\x15version_available_raw\x18\x08 \x01(\r\x12\x42\n\x10update_available\x18\t \x01(\x0e\x32(.mobilegateway.protos.UpdateAvailability\x12 \n\x18scheduled_start_time_sec\x18\n \x01(\x04\"n\n\nAlarmState\x12\x31\n\x06status\x18\x01 \x01(\x0e\x32!.mobilegateway.protos.AlarmStatus\x12-\n\x04mode\x18\x02 \x01(\x0e\x32\x1f.mobilegateway.protos.AlarmMode\"\xbb\x01\n\tHvacState\x12.\n\x05power\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.HvacPower\x12\x33\n\x07\x64\x65\x66rost\x18\x02 \x01(\x0e\x32\".mobilegateway.protos.DefrostState\x12I\n\x13precondition_status\x18\x03 \x01(\x0e\x32,.mobilegateway.protos.HvacPreconditionStatus\"\x82\x04\n\x11MobileAppReqState\x12<\n\x13\x63harge_port_request\x18\x02 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12<\n\x13\x66runk_cargo_request\x18\t \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x38\n\x0chvac_defrost\x18\x0b \x01(\x0e\x32\".mobilegateway.protos.DefrostState\x12:\n\x11hvac_precondition\x18\x0c \x01(\x0e\x32\x1f.mobilegateway.protos.HvacPower\x12\x38\n\rlight_request\x18\r \x01(\x0e\x32!.mobilegateway.protos.LightAction\x12\x42\n\x13shared_trip_request\x18\x0f \x01(\x0e\x32%.mobilegateway.protos.SharedTripState\x12<\n\x13trunk_cargo_request\x18\x10 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12?\n\x16vehicle_unlock_request\x18\x11 \x01(\x0e\x32\x1f.mobilegateway.protos.LockState\"\x82\x02\n\x10TcuInternetState\x12/\n\x08lte_type\x18\x01 \x01(\x0e\x32\x1d.mobilegateway.protos.LteType\x12\x38\n\nlte_status\x18\x02 \x01(\x0e\x32$.mobilegateway.protos.InternetStatus\x12\x39\n\x0bwifi_status\x18\x03 \x01(\x0e\x32$.mobilegateway.protos.InternetStatus\x12\x15\n\x08lte_rssi\x18\x04 \x01(\x05H\x00\x88\x01\x01\x12\x16\n\twifi_rssi\x18\x05 \x01(\x05H\x01\x88\x01\x01\x42\x0b\n\t_lte_rssiB\x0c\n\n_wifi_rssi\"\x83\x08\n\x0cVehicleState\x12\x33\n\x07\x62\x61ttery\x18\x01 \x01(\x0b\x32\".mobilegateway.protos.BatteryState\x12/\n\x05power\x18\x02 \x01(\x0e\x32 .mobilegateway.protos.PowerState\x12/\n\x05\x63\x61\x62in\x18\x03 \x01(\x0b\x32 .mobilegateway.protos.CabinState\x12-\n\x04\x62ody\x18\x04 \x01(\x0b\x32\x1f.mobilegateway.protos.BodyState\x12\x17\n\x0flast_updated_ms\x18\x05 \x01(\x04\x12\x33\n\x07\x63hassis\x18\x06 \x01(\x0b\x32\".mobilegateway.protos.ChassisState\x12\x35\n\x08\x63harging\x18\x08 \x01(\x0b\x32#.mobilegateway.protos.ChargingState\x12&\n\x03gps\x18\x0b \x01(\x0b\x32\x19.mobilegateway.protos.Gps\x12=\n\x0fsoftware_update\x18\x0c \x01(\x0b\x32$.mobilegateway.protos.SoftwareUpdate\x12/\n\x05\x61larm\x18\r \x01(\x0b\x32 .mobilegateway.protos.AlarmState\x12\x44\n\x10\x63loud_connection\x18\x0f \x01(\x0e\x32*.mobilegateway.protos.CloudConnectionState\x12\x42\n\x0fkeyless_driving\x18\x10 \x01(\x0e\x32).mobilegateway.protos.KeylessDrivingState\x12-\n\x04hvac\x18\x11 \x01(\x0b\x32\x1f.mobilegateway.protos.HvacState\x12\x33\n\ndrive_mode\x18\x12 \x01(\x0e\x32\x1f.mobilegateway.protos.DriveMode\x12\x37\n\x0cprivacy_mode\x18\x13 \x01(\x0e\x32!.mobilegateway.protos.PrivacyMode\x12\x39\n\rgear_position\x18\x14 \x01(\x0e\x32\".mobilegateway.protos.GearPosition\x12\x43\n\x12mobile_app_request\x18\x15 \x01(\x0b\x32\'.mobilegateway.protos.MobileAppReqState\x12+\n\x03tcu\x18\x16 \x01(\x0e\x32\x1e.mobilegateway.protos.TcuState\x12<\n\x0ctcu_internet\x18\x17 \x01(\x0b\x32&.mobilegateway.protos.TcuInternetState\"\xbe\x01\n\x07Vehicle\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\x12\x37\n\x0c\x61\x63\x63\x65ss_level\x18\x02 \x01(\x0e\x32!.mobilegateway.protos.AccessLevel\x12\x33\n\x06\x63onfig\x18\x03 \x01(\x0b\x32#.mobilegateway.protos.VehicleConfig\x12\x31\n\x05state\x18\x04 \x01(\x0b\x32\".mobilegateway.protos.VehicleState\"0\n\x1a\x41pplySoftwareUpdateRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\"\x1d\n\x1b\x41pplySoftwareUpdateResponse\"2\n\x1c\x43\x61ncelScheduledUpdateRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\"\x1f\n\x1d\x43\x61ncelScheduledUpdateResponse\"^\n\x14\x43hargeControlRequest\x12\x32\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32\".mobilegateway.protos.ChargeAction\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x17\n\x15\x43hargeControlResponse\"f\n\x18\x43ontrolChargePortRequest\x12\x36\n\rclosure_state\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x1b\n\x19\x43ontrolChargePortResponse\"y\n\x17\x44oorLocksControlRequest\x12\x15\n\rdoor_location\x18\x01 \x03(\x05\x12\x33\n\nlock_state\x18\x02 \x01(\x0e\x32\x1f.mobilegateway.protos.LockState\x12\x12\n\nvehicle_id\x18\x03 \x01(\t\"\x1a\n\x18\x44oorLocksControlResponse\"f\n\x18\x46rontCargoControlRequest\x12\x36\n\rclosure_state\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x1b\n\x19\x46rontCargoControlResponse\"(\n\x13\x44ocumentInfoUnknown\x12\x11\n\ttimestamp\x18\x01 \x01(\x04\"\xa2\x01\n\x0c\x44ocumentInfo\x12\x30\n\x04type\x18\x01 \x01(\x0e\x32\".mobilegateway.protos.DocumentType\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12:\n\x07unknown\x18\x05 \x01(\x0b\x32).mobilegateway.protos.DocumentInfoUnknown\"d\n\x16GetDocumentInfoRequest\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x39\n\rdocument_type\x18\x04 \x01(\x0e\x32\".mobilegateway.protos.DocumentType\"X\n\x17GetDocumentInfoResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x30\n\x04info\x18\x02 \x01(\x0b\x32\".mobilegateway.protos.DocumentInfo\",\n\x16GetVehicleStateRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\"`\n\x17GetVehicleStateResponse\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\x12\x31\n\x05state\x18\x02 \x01(\x0b\x32\".mobilegateway.protos.VehicleState\"%\n\x0fHonkHornRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\"\x12\n\x10HonkHornResponse\"i\n\x19HvacDefrostControlRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\x12\x38\n\x0chvac_defrost\x18\x02 \x01(\x0e\x32\".mobilegateway.protos.DefrostState\"\x1c\n\x1aHvacDefrostControlResponse\"]\n\x14LightsControlRequest\x12\x31\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32!.mobilegateway.protos.LightAction\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x17\n\x15LightsControlResponse\"e\n\x17RearCargoControlRequest\x12\x36\n\rclosure_state\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x1a\n\x18RearCargoControlResponse\"`\n\x1bSecurityAlarmControlRequest\x12-\n\x04mode\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.AlarmMode\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x1e\n\x1cSecurityAlarmControlResponse\"u\n\x1aSetCabinTemperatureRequest\x12\x13\n\x0btemperature\x18\x01 \x01(\x01\x12.\n\x05state\x18\x02 \x01(\x0e\x32\x1f.mobilegateway.protos.HvacPower\x12\x12\n\nvehicle_id\x18\x03 \x01(\t\"\x1d\n\x1bSetCabinTemperatureResponse\"B\n\x15SetChargeLimitRequest\x12\x15\n\rlimit_percent\x18\x01 \x01(\r\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x18\n\x16SetChargeLimitResponse\"*\n\x14WakeupVehicleRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\"\x17\n\x15WakeupVehicleResponse*k\n\x0b\x41\x63\x63\x65ssLevel\x12\x18\n\x14\x41\x43\x43\x45SS_LEVEL_UNKNOWN\x10\x00\x12\"\n\x1e\x41\x43\x43\x45SS_LEVEL_PREDELIVERY_OWNER\x10\x01\x12\x1e\n\x1a\x41\x43\x43\x45SS_LEVEL_PRIMARY_OWNER\x10\x02*<\n\x05Model\x12\x11\n\rMODEL_UNKNOWN\x10\x00\x12\r\n\tMODEL_AIR\x10\x01\x12\x11\n\rMODEL_GRAVITY\x10\x02*\x9e\x01\n\x0cModelVariant\x12\x19\n\x15MODEL_VARIANT_UNKNOWN\x10\x00\x12\x1f\n\x1bMODEL_VARIANT_DREAM_EDITION\x10\x01\x12\x1f\n\x1bMODEL_VARIANT_GRAND_TOURING\x10\x02\x12\x19\n\x15MODEL_VARIANT_TOURING\x10\x03\x12\x16\n\x12MODEL_VARIANT_PURE\x10\x04*\xf7\x01\n\nPaintColor\x12\x17\n\x13PAINT_COLOR_UNKNOWN\x10\x00\x12\x1b\n\x17PAINT_COLOR_EUREKA_GOLD\x10\x01\x12\x1d\n\x19PAINT_COLOR_STELLAR_WHITE\x10\x02\x12\x1e\n\x1aPAINT_COLOR_INFINITE_BLACK\x10\x03\x12\x1d\n\x19PAINT_COLOR_COSMOS_SILVER\x10\x04\x12\x1c\n\x18PAINT_COLOR_QUANTUM_GREY\x10\x05\x12\x1a\n\x16PAINT_COLOR_ZENITH_RED\x10\x06\x12\x1b\n\x17PAINT_COLOR_FATHOM_BLUE\x10\x07*=\n\x04Look\x12\x10\n\x0cLOOK_UNKNOWN\x10\x00\x12\x11\n\rLOOK_PLATINUM\x10\x01\x12\x10\n\x0cLOOK_STEALTH\x10\x02*|\n\x06Wheels\x12\x12\n\x0eWHEELS_UNKNOWN\x10\x00\x12\x10\n\x0cWHEELS_DREAM\x10\x01\x12\x10\n\x0cWHEELS_BLADE\x10\x02\x12\x0f\n\x0bWHEELS_LITE\x10\x03\x12\x10\n\x0cWHEELS_RANGE\x10\x04\x12\x17\n\x13WHEELS_LITE_STEALTH\x10\x08*V\n\x12SubscriptionStatus\x12\x1f\n\x1bSUBSCRIPTION_STATUS_UNKNOWN\x10\x00\x12\x1f\n\x1bSUBSCRIPTION_STATUS_CURRENT\x10\x01*b\n\x15\x43hargingAccountStatus\x12#\n\x1f\x43HARGING_ACCOUNT_STATUS_UNKNOWN\x10\x00\x12$\n CHARGING_ACCOUNT_STATUS_ENROLLED\x10\x02*T\n\x0e\x43hargingVendor\x12\x1b\n\x17\x43HARGING_VENDOR_UNKNOWN\x10\x00\x12%\n!CHARGING_VENDOR_ELECTRIFY_AMERICA\x10\x01*`\n\x07\x45\x64ition\x12\x13\n\x0f\x45\x44ITION_UNKNOWN\x10\x00\x12\x17\n\x13\x45\x44ITION_PERFORMANCE\x10\x01\x12\x11\n\rEDITION_RANGE\x10\x02\x12\x14\n\x10\x45\x44ITION_STANDARD\x10\x03*\xe4\x01\n\x0b\x42\x61tteryType\x12\x18\n\x14\x42\x41TTERY_TYPE_UNKNOWN\x10\x00\x12\x13\n\x0f\x42\x41TTERY_TYPE_01\x10\x01\x12\x13\n\x0f\x42\x41TTERY_TYPE_02\x10\x02\x12\x13\n\x0f\x42\x41TTERY_TYPE_03\x10\x03\x12\x13\n\x0f\x42\x41TTERY_TYPE_04\x10\x04\x12\x13\n\x0f\x42\x41TTERY_TYPE_05\x10\x05\x12\x13\n\x0f\x42\x41TTERY_TYPE_06\x10\x06\x12\x13\n\x0f\x42\x41TTERY_TYPE_07\x10\x07\x12\x13\n\x0f\x42\x41TTERY_TYPE_08\x10\x08\x12\x13\n\x0f\x42\x41TTERY_TYPE_09\x10\t*}\n\x08Interior\x12\x14\n\x10INTERIOR_UNKNOWN\x10\x00\x12\x17\n\x13INTERIOR_SANTA_CRUZ\x10\x01\x12\x12\n\x0eINTERIOR_TAHOE\x10\x02\x12\x13\n\x0fINTERIOR_MOJAVE\x10\x03\x12\x19\n\x15INTERIOR_SANTA_MONICA\x10\x05*M\n\tStrutType\x12\x16\n\x12STRUT_TYPE_UNKNOWN\x10\x00\x12\x12\n\x0eSTRUT_TYPE_GAS\x10\x01\x12\x14\n\x10STRUT_TYPE_POWER\x10\x02*R\n\x08RoofType\x12\x15\n\x11ROOF_TYPE_UNKNOWN\x10\x00\x12\x1a\n\x16ROOF_TYPE_GLASS_CANOPY\x10\x01\x12\x13\n\x0fROOF_TYPE_METAL\x10\x02*D\n\x0cWarningState\x12\x13\n\x0fWARNING_UNKNOWN\x10\x00\x12\x0f\n\x0bWARNING_OFF\x10\x01\x12\x0e\n\nWARNING_ON\x10\x02*\x80\x01\n\x13\x42\x61tteryPreconStatus\x12\x1a\n\x16\x42\x41TTERY_PRECON_UNKNOWN\x10\x00\x12\x16\n\x12\x42\x41TTERY_PRECON_OFF\x10\x01\x12\x15\n\x11\x42\x41TTERY_PRECON_ON\x10\x02\x12\x1e\n\x1a\x42\x41TTERY_PRECON_UNAVAILABLE\x10\x03*\x8e\x02\n\nPowerState\x12\x17\n\x13POWER_STATE_UNKNOWN\x10\x00\x12\x15\n\x11POWER_STATE_SLEEP\x10\x01\x12\x14\n\x10POWER_STATE_WINK\x10\x02\x12\x19\n\x15POWER_STATE_ACCESSORY\x10\x03\x12\x15\n\x11POWER_STATE_DRIVE\x10\x04\x12\x1b\n\x17POWER_STATE_LIVE_CHARGE\x10\x05\x12\x1c\n\x18POWER_STATE_SLEEP_CHARGE\x10\x06\x12\x1b\n\x17POWER_STATE_LIVE_UPDATE\x10\x07\x12\x17\n\x13POWER_STATE_CLOUD_2\x10\n\x12\x17\n\x13POWER_STATE_MONITOR\x10\x0b*S\n\tLockState\x12\x16\n\x12LOCK_STATE_UNKNOWN\x10\x00\x12\x17\n\x13LOCK_STATE_UNLOCKED\x10\x01\x12\x15\n\x11LOCK_STATE_LOCKED\x10\x02*d\n\tDoorState\x12\x16\n\x12\x44OOR_STATE_UNKNOWN\x10\x00\x12\x13\n\x0f\x44OOR_STATE_OPEN\x10\x01\x12\x15\n\x11\x44OOR_STATE_CLOSED\x10\x02\x12\x13\n\x0f\x44OOR_STATE_AJAR\x10\x03*P\n\rWalkawayState\x12\x14\n\x10WALKAWAY_UNKNOWN\x10\x00\x12\x13\n\x0fWALKAWAY_ACTIVE\x10\x02\x12\x14\n\x10WALKAWAY_DISABLE\x10\x03*b\n\rAccessRequest\x12\x1a\n\x16\x41\x43\x43\x45SS_REQUEST_UNKNOWN\x10\x00\x12\x19\n\x15\x41\x43\x43\x45SS_REQUEST_ACTIVE\x10\x01\x12\x1a\n\x16\x41\x43\x43\x45SS_REQUEST_PASSIVE\x10\x02*n\n\nLightState\x12\x1e\n\x1aLIGHT_STATE_REALLY_UNKNOWN\x10\x00\x12\x13\n\x0fLIGHT_STATE_OFF\x10\x01\x12\x12\n\x0eLIGHT_STATE_ON\x10\x02\x12\x17\n\x13LIGHT_STATE_UNKNOWN\x10\x03*j\n\x0bLightAction\x12\x18\n\x14LIGHT_ACTION_UNKNOWN\x10\x00\x12\x16\n\x12LIGHT_ACTION_FLASH\x10\x01\x12\x13\n\x0fLIGHT_ACTION_ON\x10\x02\x12\x14\n\x10LIGHT_ACTION_OFF\x10\x03*\xc4\x01\n\x0b\x43hargeState\x12\x18\n\x14\x43HARGE_STATE_UNKNOWN\x10\x00\x12\x1e\n\x1a\x43HARGE_STATE_NOT_CONNECTED\x10\x01\x12 \n\x1c\x43HARGE_STATE_CABLE_CONNECTED\x10\x02\x12\x19\n\x15\x43HARGE_STATE_CHARGING\x10\x08\x12 \n\x1c\x43HARGE_STATE_CHARGING_END_OK\x10\t\x12\x1c\n\x18\x43HARGE_STATE_DISCHARGING\x10\x13*\xb9\x01\n\x14ScheduledChargeState\x12\"\n\x1eSCHEDULED_CHARGE_STATE_UNKNOWN\x10\x00\x12\x1f\n\x1bSCHEDULED_CHARGE_STATE_IDLE\x10\x01\x12.\n*SCHEDULED_CHARGE_STATE_SCHEDULED_TO_CHARGE\x10\x02\x12,\n(SCHEDULED_CHARGE_STATE_REQUEST_TO_CHARGE\x10\x03*x\n\x1fScheduledChargeUnavailableState\x12(\n$SCHEDULED_CHARGE_UNAVAILABLE_UNKNOWN\x10\x00\x12+\n\'SCHEDULED_CHARGE_UNAVAILABLE_NO_REQUEST\x10\x01*b\n\nEnergyType\x12\x17\n\x13\x45NERGY_TYPE_UNKNOWN\x10\x00\x12\x12\n\x0e\x45NERGY_TYPE_AC\x10\x01\x12\x12\n\x0e\x45NERGY_TYPE_DC\x10\x02\x12\x13\n\x0f\x45NERGY_TYPE_V2V\x10\x04*\xbb\x01\n\x0bUpdateState\x12\x18\n\x14UPDATE_STATE_UNKNOWN\x10\x00\x12\x1c\n\x18UPDATE_STATE_IN_PROGRESS\x10\x01\x12\x18\n\x14UPDATE_STATE_SUCCESS\x10\x02\x12\x17\n\x13UPDATE_STATE_FAILED\x10\x03\x12\x1f\n\x1bUPDATE_FAILED_DRIVE_ALLOWED\x10\x05\x12 \n\x1cUPDATE_SUCCESS_WITH_WARNINGS\x10\x07*K\n\x12UpdateAvailability\x12\x1f\n\x1bUPDATE_AVAILABILITY_UNKNOWN\x10\x00\x12\x14\n\x10UPDATE_AVAILABLE\x10\x01*Z\n\x0b\x41larmStatus\x12\x18\n\x14\x41LARM_STATUS_UNKNOWN\x10\x00\x12\x19\n\x15\x41LARM_STATUS_DISARMED\x10\x01\x12\x16\n\x12\x41LARM_STATUS_ARMED\x10\x02*a\n\tAlarmMode\x12\x16\n\x12\x41LARM_MODE_UNKNOWN\x10\x00\x12\x12\n\x0e\x41LARM_MODE_OFF\x10\x01\x12\x11\n\rALARM_MODE_ON\x10\x02\x12\x15\n\x11\x41LARM_MODE_SILENT\x10\x03*w\n\x14\x43loudConnectionState\x12\x1c\n\x18\x43LOUD_CONNECTION_UNKNOWN\x10\x00\x12\x1e\n\x1a\x43LOUD_CONNECTION_CONNECTED\x10\x01\x12!\n\x1d\x43LOUD_CONNECTION_DISCONNECTED\x10\x02*c\n\x13KeylessDrivingState\x12\x1b\n\x17KEYLESS_DRIVING_UNKNOWN\x10\x00\x12\x16\n\x12KEYLESS_DRIVING_ON\x10\x01\x12\x17\n\x13KEYLESS_DRIVING_OFF\x10\x02*U\n\tHvacPower\x12\x16\n\x12HVAC_POWER_UNKNOWN\x10\x00\x12\x0b\n\x07HVAC_ON\x10\x01\x12\x0c\n\x08HVAC_OFF\x10\x02\x12\x15\n\x11HVAC_PRECONDITION\x10\x03*J\n\x0c\x44\x65\x66rostState\x12\x19\n\x15\x44\x45\x46ROST_STATE_UNKNOWN\x10\x00\x12\x0e\n\nDEFROST_ON\x10\x01\x12\x0f\n\x0b\x44\x45\x46ROST_OFF\x10\x02*\x92\x01\n\x16HvacPreconditionStatus\x12$\n HVAC_PRECONDITION_STATUS_UNKNOWN\x10\x00\x12)\n%HVAC_PRECONDITION_STATUS_STILL_ACTIVE\x10\x01\x12\'\n#HVAC_PRECONDITION_STATUS_USER_INPUT\x10\x04*l\n\tDriveMode\x12\x16\n\x12\x44RIVE_MODE_UNKNOWN\x10\x00\x12\x16\n\x12\x44RIVE_MODE_COMFORT\x10\x01\x12\x14\n\x10\x44RIVE_MODE_SWIFT\x10\x02\x12\x19\n\x15\x44RIVE_MODE_SPORT_PLUS\x10\x05*v\n\x0bPrivacyMode\x12\x18\n\x14PRIVACY_MODE_UNKNOWN\x10\x00\x12%\n!PRIVACY_MODE_CONNECTIVITY_ENABLED\x10\x01\x12&\n\"PRIVACY_MODE_CONNECTIVITY_DISABLED\x10\x02*c\n\x0cGearPosition\x12\x10\n\x0cGEAR_UNKNOWN\x10\x00\x12\r\n\tGEAR_PARK\x10\x01\x12\x10\n\x0cGEAR_REVERSE\x10\x02\x12\x10\n\x0cGEAR_NEUTRAL\x10\x03\x12\x0e\n\nGEAR_DRIVE\x10\x04*E\n\x0fSharedTripState\x12\x17\n\x13SHARED_TRIP_UNKNOWN\x10\x00\x12\x19\n\x15SHARED_TRIP_AVAILABLE\x10\x01*Y\n\x08TcuState\x12\x0f\n\x0bTCU_UNKNOWN\x10\x00\x12\r\n\tTCU_SLEEP\x10\x01\x12\x0e\n\nTCU_DROWSY\x10\x02\x12\x0c\n\x08TCU_FULL\x10\x04\x12\x0f\n\x0bTCU_FACTORY\x10\x05*A\n\x07LteType\x12\x14\n\x10LTE_TYPE_UNKNOWN\x10\x00\x12\x0f\n\x0bLTE_TYPE_3G\x10\x01\x12\x0f\n\x0bLTE_TYPE_4G\x10\x02*`\n\x0eInternetStatus\x12\x1b\n\x17INTERNET_STATUS_UNKNOWN\x10\x00\x12\x19\n\x15INTERNET_DISCONNECTED\x10\x01\x12\x16\n\x12INTERNET_CONNECTED\x10\x02*Z\n\x0c\x43hargeAction\x12\x19\n\x15\x43HARGE_ACTION_UNKNOWN\x10\x00\x12\x17\n\x13\x43HARGE_ACTION_START\x10\x01\x12\x16\n\x12\x43HARGE_ACTION_STOP\x10\x02*\x95\x01\n\x0c\x44ocumentType\x12\x19\n\x15\x44OCUMENT_TYPE_UNKNOWN\x10\x00\x12#\n\x1f\x44OCUMENT_TYPE_RELEASE_NOTES_PRE\x10\x01\x12$\n DOCUMENT_TYPE_RELEASE_NOTES_POST\x10\x02\x12\x1f\n\x1b\x44OCUMENT_TYPE_OWNERS_MANUAL\x10\x03\x32\xe0\x0e\n\x13VehicleStateService\x12|\n\x13\x41pplySoftwareUpdate\x12\x30.mobilegateway.protos.ApplySoftwareUpdateRequest\x1a\x31.mobilegateway.protos.ApplySoftwareUpdateResponse\"\x00\x12\x82\x01\n\x15\x43\x61ncelScheduledUpdate\x12\x32.mobilegateway.protos.CancelScheduledUpdateRequest\x1a\x33.mobilegateway.protos.CancelScheduledUpdateResponse\"\x00\x12j\n\rChargeControl\x12*.mobilegateway.protos.ChargeControlRequest\x1a+.mobilegateway.protos.ChargeControlResponse\"\x00\x12v\n\x11\x43ontrolChargePort\x12..mobilegateway.protos.ControlChargePortRequest\x1a/.mobilegateway.protos.ControlChargePortResponse\"\x00\x12s\n\x10\x44oorLocksControl\x12-.mobilegateway.protos.DoorLocksControlRequest\x1a..mobilegateway.protos.DoorLocksControlResponse\"\x00\x12v\n\x11\x46rontCargoControl\x12..mobilegateway.protos.FrontCargoControlRequest\x1a/.mobilegateway.protos.FrontCargoControlResponse\"\x00\x12p\n\x0fGetDocumentInfo\x12,.mobilegateway.protos.GetDocumentInfoRequest\x1a-.mobilegateway.protos.GetDocumentInfoResponse\"\x00\x12p\n\x0fGetVehicleState\x12,.mobilegateway.protos.GetVehicleStateRequest\x1a-.mobilegateway.protos.GetVehicleStateResponse\"\x00\x12[\n\x08HonkHorn\x12%.mobilegateway.protos.HonkHornRequest\x1a&.mobilegateway.protos.HonkHornResponse\"\x00\x12y\n\x12HvacDefrostControl\x12/.mobilegateway.protos.HvacDefrostControlRequest\x1a\x30.mobilegateway.protos.HvacDefrostControlResponse\"\x00\x12j\n\rLightsControl\x12*.mobilegateway.protos.LightsControlRequest\x1a+.mobilegateway.protos.LightsControlResponse\"\x00\x12s\n\x10RearCargoControl\x12-.mobilegateway.protos.RearCargoControlRequest\x1a..mobilegateway.protos.RearCargoControlResponse\"\x00\x12\x7f\n\x14SecurityAlarmControl\x12\x31.mobilegateway.protos.SecurityAlarmControlRequest\x1a\x32.mobilegateway.protos.SecurityAlarmControlResponse\"\x00\x12|\n\x13SetCabinTemperature\x12\x30.mobilegateway.protos.SetCabinTemperatureRequest\x1a\x31.mobilegateway.protos.SetCabinTemperatureResponse\"\x00\x12m\n\x0eSetChargeLimit\x12+.mobilegateway.protos.SetChargeLimitRequest\x1a,.mobilegateway.protos.SetChargeLimitResponse\"\x00\x12j\n\rWakeupVehicle\x12*.mobilegateway.protos.WakeupVehicleRequest\x1a+.mobilegateway.protos.WakeupVehicleResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bvehicle_state_service.proto\x12\x14mobilegateway.protos\"\x8b\x01\n\x14\x43hargingSubscription\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x17\n\x0f\x65xpiration_date\x18\x02 \x01(\x04\x12\x12\n\nstart_date\x18\x03 \x01(\x04\x12\x38\n\x06status\x18\x04 \x01(\x0e\x32(.mobilegateway.protos.SubscriptionStatus\"\xe8\x01\n\x0f\x43hargingAccount\x12\x0e\n\x06\x65ma_id\x18\x01 \x01(\t\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\x12;\n\x06status\x18\x03 \x01(\x0e\x32+.mobilegateway.protos.ChargingAccountStatus\x12\x1c\n\x14\x63reated_at_epoch_sec\x18\x04 \x01(\x04\x12\x1b\n\x13\x65xpiry_on_epoch_sec\x18\x05 \x01(\x04\x12\x39\n\x0bvendor_name\x18\x06 \x01(\x0e\x32$.mobilegateway.protos.ChargingVendor\"(\n\x12SpecialIdentifiers\x12\x12\n\ndoor_plate\x18\x01 \x01(\t\"\x1b\n\x0bReservation\x12\x0c\n\x04\x64\x61te\x18\x01 \x01(\x04\"\x93\x07\n\rVehicleConfig\x12\x0b\n\x03vin\x18\x01 \x01(\t\x12*\n\x05model\x18\x02 \x01(\x0e\x32\x1b.mobilegateway.protos.Model\x12\x33\n\x07variant\x18\x03 \x01(\x0e\x32\".mobilegateway.protos.ModelVariant\x12\x10\n\x08nickname\x18\x05 \x01(\t\x12\x35\n\x0bpaint_color\x18\x06 \x01(\x0e\x32 .mobilegateway.protos.PaintColor\x12\x0e\n\x06\x65ma_id\x18\x07 \x01(\t\x12,\n\x06wheels\x18\x08 \x01(\x0e\x32\x1c.mobilegateway.protos.Wheels\x12\x43\n\x0f\x65\x61_subscription\x18\t \x01(\x0b\x32*.mobilegateway.protos.ChargingSubscription\x12@\n\x11\x63harging_accounts\x18\n \x03(\x0b\x32%.mobilegateway.protos.ChargingAccount\x12\x14\n\x0c\x63ountry_code\x18\x0b \x01(\t\x12\x13\n\x0bregion_code\x18\x0c \x01(\t\x12.\n\x07\x65\x64ition\x18\r \x01(\x0e\x32\x1d.mobilegateway.protos.Edition\x12\x32\n\x07\x62\x61ttery\x18\x0e \x01(\x0e\x32!.mobilegateway.protos.BatteryType\x12\x30\n\x08interior\x18\x0f \x01(\x0e\x32\x1e.mobilegateway.protos.Interior\x12\x45\n\x13special_identifiers\x18\x10 \x01(\x0b\x32(.mobilegateway.protos.SpecialIdentifiers\x12(\n\x04look\x18\x11 \x01(\x0e\x32\x1a.mobilegateway.protos.Look\x12\x1b\n\x13\x65xterior_color_code\x18\x12 \x01(\t\x12\x1b\n\x13interior_color_code\x18\x13 \x01(\t\x12\x34\n\x0b\x66runk_strut\x18\x14 \x01(\x0e\x32\x1f.mobilegateway.protos.StrutType\x12\x36\n\x0breservation\x18\x15 \x01(\x0b\x32!.mobilegateway.protos.Reservation\x12,\n\x04roof\x18\x16 \x01(\x0e\x32\x1e.mobilegateway.protos.RoofType\"\xaf\x03\n\x0c\x42\x61tteryState\x12\x17\n\x0fremaining_range\x18\x01 \x01(\x01\x12\x16\n\x0e\x63harge_percent\x18\x02 \x01(\x01\x12\x0c\n\x04kwhr\x18\x03 \x01(\x01\x12\x15\n\rcapacity_kwhr\x18\x04 \x01(\x01\x12:\n\x0e\x62\x61ttery_health\x18\x05 \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12<\n\x10low_charge_level\x18\x06 \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12\x41\n\x15\x63ritical_charge_level\x18\x07 \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12\x19\n\x11unavailable_range\x18\x08 \x01(\x01\x12I\n\x16preconditioning_status\x18\t \x01(\x0e\x32).mobilegateway.protos.BatteryPreconStatus\x12&\n\x1epreconditioning_time_remaining\x18\n \x01(\r\":\n\nCabinState\x12\x15\n\rinterior_temp\x18\x01 \x01(\x01\x12\x15\n\rexterior_temp\x18\x02 \x01(\x01\"\xc6\x04\n\tBodyState\x12\x33\n\ndoor_locks\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.LockState\x12\x34\n\x0b\x66ront_cargo\x18\x02 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x33\n\nrear_cargo\x18\x03 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x38\n\x0f\x66ront_left_door\x18\x04 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x39\n\x10\x66ront_right_door\x18\x05 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x37\n\x0erear_left_door\x18\x06 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x38\n\x0frear_right_door\x18\x07 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x34\n\x0b\x63harge_port\x18\x08 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12:\n\rwalkaway_lock\x18\t \x01(\x0e\x32#.mobilegateway.protos.WalkawayState\x12?\n\x12\x61\x63\x63\x65ss_type_status\x18\n \x01(\x0e\x32#.mobilegateway.protos.AccessRequest\"\x9b\x06\n\x0c\x43hassisState\x12\x13\n\x0bodometer_km\x18\x01 \x01(\x01\x12$\n\x1c\x66ront_left_tire_pressure_bar\x18\x02 \x01(\x01\x12%\n\x1d\x66ront_right_tire_pressure_bar\x18\x03 \x01(\x01\x12#\n\x1brear_left_tire_pressure_bar\x18\x04 \x01(\x01\x12$\n\x1crear_right_tire_pressure_bar\x18\x05 \x01(\x01\x12\x34\n\nheadlights\x18\x06 \x01(\x0e\x32 .mobilegateway.protos.LightState\x12@\n\x14hard_warn_left_front\x18\x08 \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12?\n\x13hard_warn_left_rear\x18\t \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12\x41\n\x15hard_warn_right_front\x18\n \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12@\n\x14hard_warn_right_rear\x18\x0b \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12@\n\x14soft_warn_left_front\x18\x0c \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12?\n\x13soft_warn_left_rear\x18\r \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12\x41\n\x15soft_warn_right_front\x18\x0e \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12@\n\x14soft_warn_right_rear\x18\x0f \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12\x18\n\x10software_version\x18\x10 \x01(\t\"\xed\x04\n\rChargingState\x12\x37\n\x0c\x63harge_state\x18\x01 \x01(\x0e\x32!.mobilegateway.protos.ChargeState\x12\x35\n\x0b\x65nergy_type\x18\x02 \x01(\x0e\x32 .mobilegateway.protos.EnergyType\x12\x19\n\x11\x63harge_session_mi\x18\x05 \x01(\x01\x12\x1a\n\x12\x63harge_session_kwh\x18\x06 \x01(\x01\x12!\n\x19session_minutes_remaining\x18\x07 \x01(\r\x12\x14\n\x0c\x63harge_limit\x18\x08 \x01(\r\x12\x33\n\ncable_lock\x18\n \x01(\x0e\x32\x1f.mobilegateway.protos.LockState\x12\x1f\n\x17\x63harge_rate_kwh_precise\x18\x0b \x01(\x01\x12\x1f\n\x17\x63harge_rate_mph_precise\x18\x0c \x01(\x01\x12%\n\x1d\x63harge_rate_miles_min_precise\x18\r \x01(\x01\x12\x1c\n\x14\x63harge_limit_percent\x18\x0e \x01(\x01\x12\x1d\n\x15\x63harge_scheduled_time\x18\x10 \x01(\r\x12\x44\n\x10scheduled_charge\x18\x11 \x01(\x0e\x32*.mobilegateway.protos.ScheduledChargeState\x12[\n\x1cscheduled_charge_unavailable\x18\x12 \x01(\x0e\x32\x35.mobilegateway.protos.ScheduledChargeUnavailableState\"/\n\x08Location\x12\x10\n\x08latitude\x18\x01 \x01(\x01\x12\x11\n\tlongitude\x18\x02 \x01(\x01\"z\n\x03Gps\x12\x30\n\x08location\x18\x01 \x01(\x0b\x32\x1e.mobilegateway.protos.Location\x12\x11\n\televation\x18\x02 \x01(\x05\x12\x15\n\rposition_time\x18\x04 \x01(\x04\x12\x17\n\x0fheading_precise\x18\x05 \x01(\x01\"\x9e\x02\n\x0eSoftwareUpdate\x12\x19\n\x11version_available\x18\x01 \x01(\t\x12 \n\x18install_duration_minutes\x18\x02 \x01(\r\x12\x18\n\x10percent_complete\x18\x04 \x01(\r\x12\x30\n\x05state\x18\x05 \x01(\x0e\x32!.mobilegateway.protos.UpdateState\x12\x1d\n\x15version_available_raw\x18\x08 \x01(\r\x12\x42\n\x10update_available\x18\t \x01(\x0e\x32(.mobilegateway.protos.UpdateAvailability\x12 \n\x18scheduled_start_time_sec\x18\n \x01(\x04\"n\n\nAlarmState\x12\x31\n\x06status\x18\x01 \x01(\x0e\x32!.mobilegateway.protos.AlarmStatus\x12-\n\x04mode\x18\x02 \x01(\x0e\x32\x1f.mobilegateway.protos.AlarmMode\"\x81\x02\n\tHvacState\x12.\n\x05power\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.HvacPower\x12\x33\n\x07\x64\x65\x66rost\x18\x02 \x01(\x0e\x32\".mobilegateway.protos.DefrostState\x12I\n\x13precondition_status\x18\x03 \x01(\x0e\x32,.mobilegateway.protos.HvacPreconditionStatus\x12\x44\n\x13keep_climate_status\x18\x05 \x01(\x0e\x32\'.mobilegateway.protos.KeepClimateStatus\"\xf7\x04\n\x11MobileAppReqState\x12:\n\x11\x61larm_set_request\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.AlarmMode\x12<\n\x13\x63harge_port_request\x18\x02 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12<\n\x13\x66runk_cargo_request\x18\t \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x38\n\x0chvac_defrost\x18\x0b \x01(\x0e\x32\".mobilegateway.protos.DefrostState\x12:\n\x11hvac_precondition\x18\x0c \x01(\x0e\x32\x1f.mobilegateway.protos.HvacPower\x12\x38\n\rlight_request\x18\r \x01(\x0e\x32!.mobilegateway.protos.LightAction\x12\x37\n\rpanic_request\x18\x0e \x01(\x0e\x32 .mobilegateway.protos.PanicState\x12\x42\n\x13shared_trip_request\x18\x0f \x01(\x0e\x32%.mobilegateway.protos.SharedTripState\x12<\n\x13trunk_cargo_request\x18\x10 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12?\n\x16vehicle_unlock_request\x18\x11 \x01(\x0e\x32\x1f.mobilegateway.protos.LockState\"\x82\x02\n\x10TcuInternetState\x12/\n\x08lte_type\x18\x01 \x01(\x0e\x32\x1d.mobilegateway.protos.LteType\x12\x38\n\nlte_status\x18\x02 \x01(\x0e\x32$.mobilegateway.protos.InternetStatus\x12\x39\n\x0bwifi_status\x18\x03 \x01(\x0e\x32$.mobilegateway.protos.InternetStatus\x12\x15\n\x08lte_rssi\x18\x04 \x01(\x05H\x00\x88\x01\x01\x12\x16\n\twifi_rssi\x18\x05 \x01(\x05H\x01\x88\x01\x01\x42\x0b\n\t_lte_rssiB\x0c\n\n_wifi_rssi\"\x83\x08\n\x0cVehicleState\x12\x33\n\x07\x62\x61ttery\x18\x01 \x01(\x0b\x32\".mobilegateway.protos.BatteryState\x12/\n\x05power\x18\x02 \x01(\x0e\x32 .mobilegateway.protos.PowerState\x12/\n\x05\x63\x61\x62in\x18\x03 \x01(\x0b\x32 .mobilegateway.protos.CabinState\x12-\n\x04\x62ody\x18\x04 \x01(\x0b\x32\x1f.mobilegateway.protos.BodyState\x12\x17\n\x0flast_updated_ms\x18\x05 \x01(\x04\x12\x33\n\x07\x63hassis\x18\x06 \x01(\x0b\x32\".mobilegateway.protos.ChassisState\x12\x35\n\x08\x63harging\x18\x08 \x01(\x0b\x32#.mobilegateway.protos.ChargingState\x12&\n\x03gps\x18\x0b \x01(\x0b\x32\x19.mobilegateway.protos.Gps\x12=\n\x0fsoftware_update\x18\x0c \x01(\x0b\x32$.mobilegateway.protos.SoftwareUpdate\x12/\n\x05\x61larm\x18\r \x01(\x0b\x32 .mobilegateway.protos.AlarmState\x12\x44\n\x10\x63loud_connection\x18\x0f \x01(\x0e\x32*.mobilegateway.protos.CloudConnectionState\x12\x42\n\x0fkeyless_driving\x18\x10 \x01(\x0e\x32).mobilegateway.protos.KeylessDrivingState\x12-\n\x04hvac\x18\x11 \x01(\x0b\x32\x1f.mobilegateway.protos.HvacState\x12\x33\n\ndrive_mode\x18\x12 \x01(\x0e\x32\x1f.mobilegateway.protos.DriveMode\x12\x37\n\x0cprivacy_mode\x18\x13 \x01(\x0e\x32!.mobilegateway.protos.PrivacyMode\x12\x39\n\rgear_position\x18\x14 \x01(\x0e\x32\".mobilegateway.protos.GearPosition\x12\x43\n\x12mobile_app_request\x18\x15 \x01(\x0b\x32\'.mobilegateway.protos.MobileAppReqState\x12+\n\x03tcu\x18\x16 \x01(\x0e\x32\x1e.mobilegateway.protos.TcuState\x12<\n\x0ctcu_internet\x18\x17 \x01(\x0b\x32&.mobilegateway.protos.TcuInternetState\"\xbe\x01\n\x07Vehicle\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\x12\x37\n\x0c\x61\x63\x63\x65ss_level\x18\x02 \x01(\x0e\x32!.mobilegateway.protos.AccessLevel\x12\x33\n\x06\x63onfig\x18\x03 \x01(\x0b\x32#.mobilegateway.protos.VehicleConfig\x12\x31\n\x05state\x18\x04 \x01(\x0b\x32\".mobilegateway.protos.VehicleState\"0\n\x1a\x41pplySoftwareUpdateRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\"\x1d\n\x1b\x41pplySoftwareUpdateResponse\"2\n\x1c\x43\x61ncelScheduledUpdateRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\"\x1f\n\x1d\x43\x61ncelScheduledUpdateResponse\"^\n\x14\x43hargeControlRequest\x12\x32\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32\".mobilegateway.protos.ChargeAction\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x17\n\x15\x43hargeControlResponse\"f\n\x18\x43ontrolChargePortRequest\x12\x36\n\rclosure_state\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x1b\n\x19\x43ontrolChargePortResponse\"y\n\x17\x44oorLocksControlRequest\x12\x15\n\rdoor_location\x18\x01 \x03(\x05\x12\x33\n\nlock_state\x18\x02 \x01(\x0e\x32\x1f.mobilegateway.protos.LockState\x12\x12\n\nvehicle_id\x18\x03 \x01(\t\"\x1a\n\x18\x44oorLocksControlResponse\"f\n\x18\x46rontCargoControlRequest\x12\x36\n\rclosure_state\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x1b\n\x19\x46rontCargoControlResponse\"(\n\x13\x44ocumentInfoUnknown\x12\x11\n\ttimestamp\x18\x01 \x01(\x04\"\xa2\x01\n\x0c\x44ocumentInfo\x12\x30\n\x04type\x18\x01 \x01(\x0e\x32\".mobilegateway.protos.DocumentType\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12:\n\x07unknown\x18\x05 \x01(\x0b\x32).mobilegateway.protos.DocumentInfoUnknown\"d\n\x16GetDocumentInfoRequest\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x39\n\rdocument_type\x18\x04 \x01(\x0e\x32\".mobilegateway.protos.DocumentType\"X\n\x17GetDocumentInfoResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x30\n\x04info\x18\x02 \x01(\x0b\x32\".mobilegateway.protos.DocumentInfo\",\n\x16GetVehicleStateRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\"`\n\x17GetVehicleStateResponse\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\x12\x31\n\x05state\x18\x02 \x01(\x0b\x32\".mobilegateway.protos.VehicleState\"%\n\x0fHonkHornRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\"\x12\n\x10HonkHornResponse\"i\n\x19HvacDefrostControlRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\x12\x38\n\x0chvac_defrost\x18\x02 \x01(\x0e\x32\".mobilegateway.protos.DefrostState\"\x1c\n\x1aHvacDefrostControlResponse\"]\n\x14LightsControlRequest\x12\x31\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32!.mobilegateway.protos.LightAction\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x17\n\x15LightsControlResponse\"e\n\x17RearCargoControlRequest\x12\x36\n\rclosure_state\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x1a\n\x18RearCargoControlResponse\"`\n\x1bSecurityAlarmControlRequest\x12-\n\x04mode\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.AlarmMode\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x1e\n\x1cSecurityAlarmControlResponse\"u\n\x1aSetCabinTemperatureRequest\x12\x13\n\x0btemperature\x18\x01 \x01(\x01\x12.\n\x05state\x18\x02 \x01(\x0e\x32\x1f.mobilegateway.protos.HvacPower\x12\x12\n\nvehicle_id\x18\x03 \x01(\t\"\x1d\n\x1bSetCabinTemperatureResponse\"B\n\x15SetChargeLimitRequest\x12\x15\n\rlimit_percent\x18\x01 \x01(\r\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x18\n\x16SetChargeLimitResponse\"*\n\x14WakeupVehicleRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\"\x17\n\x15WakeupVehicleResponse*k\n\x0b\x41\x63\x63\x65ssLevel\x12\x18\n\x14\x41\x43\x43\x45SS_LEVEL_UNKNOWN\x10\x00\x12\"\n\x1e\x41\x43\x43\x45SS_LEVEL_PREDELIVERY_OWNER\x10\x01\x12\x1e\n\x1a\x41\x43\x43\x45SS_LEVEL_PRIMARY_OWNER\x10\x02*<\n\x05Model\x12\x11\n\rMODEL_UNKNOWN\x10\x00\x12\r\n\tMODEL_AIR\x10\x01\x12\x11\n\rMODEL_GRAVITY\x10\x02*\x9e\x01\n\x0cModelVariant\x12\x19\n\x15MODEL_VARIANT_UNKNOWN\x10\x00\x12\x1f\n\x1bMODEL_VARIANT_DREAM_EDITION\x10\x01\x12\x1f\n\x1bMODEL_VARIANT_GRAND_TOURING\x10\x02\x12\x19\n\x15MODEL_VARIANT_TOURING\x10\x03\x12\x16\n\x12MODEL_VARIANT_PURE\x10\x04*\xf7\x01\n\nPaintColor\x12\x17\n\x13PAINT_COLOR_UNKNOWN\x10\x00\x12\x1b\n\x17PAINT_COLOR_EUREKA_GOLD\x10\x01\x12\x1d\n\x19PAINT_COLOR_STELLAR_WHITE\x10\x02\x12\x1e\n\x1aPAINT_COLOR_INFINITE_BLACK\x10\x03\x12\x1d\n\x19PAINT_COLOR_COSMOS_SILVER\x10\x04\x12\x1c\n\x18PAINT_COLOR_QUANTUM_GREY\x10\x05\x12\x1a\n\x16PAINT_COLOR_ZENITH_RED\x10\x06\x12\x1b\n\x17PAINT_COLOR_FATHOM_BLUE\x10\x07*=\n\x04Look\x12\x10\n\x0cLOOK_UNKNOWN\x10\x00\x12\x11\n\rLOOK_PLATINUM\x10\x01\x12\x10\n\x0cLOOK_STEALTH\x10\x02*|\n\x06Wheels\x12\x12\n\x0eWHEELS_UNKNOWN\x10\x00\x12\x10\n\x0cWHEELS_DREAM\x10\x01\x12\x10\n\x0cWHEELS_BLADE\x10\x02\x12\x0f\n\x0bWHEELS_LITE\x10\x03\x12\x10\n\x0cWHEELS_RANGE\x10\x04\x12\x17\n\x13WHEELS_LITE_STEALTH\x10\x08*V\n\x12SubscriptionStatus\x12\x1f\n\x1bSUBSCRIPTION_STATUS_UNKNOWN\x10\x00\x12\x1f\n\x1bSUBSCRIPTION_STATUS_CURRENT\x10\x01*b\n\x15\x43hargingAccountStatus\x12#\n\x1f\x43HARGING_ACCOUNT_STATUS_UNKNOWN\x10\x00\x12$\n CHARGING_ACCOUNT_STATUS_ENROLLED\x10\x02*o\n\x0e\x43hargingVendor\x12\x1b\n\x17\x43HARGING_VENDOR_UNKNOWN\x10\x00\x12%\n!CHARGING_VENDOR_ELECTRIFY_AMERICA\x10\x01\x12\x19\n\x15\x43HARGING_VENDOR_BOSCH\x10\x03*`\n\x07\x45\x64ition\x12\x13\n\x0f\x45\x44ITION_UNKNOWN\x10\x00\x12\x17\n\x13\x45\x44ITION_PERFORMANCE\x10\x01\x12\x11\n\rEDITION_RANGE\x10\x02\x12\x14\n\x10\x45\x44ITION_STANDARD\x10\x03*\xe4\x01\n\x0b\x42\x61tteryType\x12\x18\n\x14\x42\x41TTERY_TYPE_UNKNOWN\x10\x00\x12\x13\n\x0f\x42\x41TTERY_TYPE_01\x10\x01\x12\x13\n\x0f\x42\x41TTERY_TYPE_02\x10\x02\x12\x13\n\x0f\x42\x41TTERY_TYPE_03\x10\x03\x12\x13\n\x0f\x42\x41TTERY_TYPE_04\x10\x04\x12\x13\n\x0f\x42\x41TTERY_TYPE_05\x10\x05\x12\x13\n\x0f\x42\x41TTERY_TYPE_06\x10\x06\x12\x13\n\x0f\x42\x41TTERY_TYPE_07\x10\x07\x12\x13\n\x0f\x42\x41TTERY_TYPE_08\x10\x08\x12\x13\n\x0f\x42\x41TTERY_TYPE_09\x10\t*}\n\x08Interior\x12\x14\n\x10INTERIOR_UNKNOWN\x10\x00\x12\x17\n\x13INTERIOR_SANTA_CRUZ\x10\x01\x12\x12\n\x0eINTERIOR_TAHOE\x10\x02\x12\x13\n\x0fINTERIOR_MOJAVE\x10\x03\x12\x19\n\x15INTERIOR_SANTA_MONICA\x10\x05*M\n\tStrutType\x12\x16\n\x12STRUT_TYPE_UNKNOWN\x10\x00\x12\x12\n\x0eSTRUT_TYPE_GAS\x10\x01\x12\x14\n\x10STRUT_TYPE_POWER\x10\x02*R\n\x08RoofType\x12\x15\n\x11ROOF_TYPE_UNKNOWN\x10\x00\x12\x1a\n\x16ROOF_TYPE_GLASS_CANOPY\x10\x01\x12\x13\n\x0fROOF_TYPE_METAL\x10\x02*D\n\x0cWarningState\x12\x13\n\x0fWARNING_UNKNOWN\x10\x00\x12\x0f\n\x0bWARNING_OFF\x10\x01\x12\x0e\n\nWARNING_ON\x10\x02*\x80\x01\n\x13\x42\x61tteryPreconStatus\x12\x1a\n\x16\x42\x41TTERY_PRECON_UNKNOWN\x10\x00\x12\x16\n\x12\x42\x41TTERY_PRECON_OFF\x10\x01\x12\x15\n\x11\x42\x41TTERY_PRECON_ON\x10\x02\x12\x1e\n\x1a\x42\x41TTERY_PRECON_UNAVAILABLE\x10\x03*\x8e\x02\n\nPowerState\x12\x17\n\x13POWER_STATE_UNKNOWN\x10\x00\x12\x15\n\x11POWER_STATE_SLEEP\x10\x01\x12\x14\n\x10POWER_STATE_WINK\x10\x02\x12\x19\n\x15POWER_STATE_ACCESSORY\x10\x03\x12\x15\n\x11POWER_STATE_DRIVE\x10\x04\x12\x1b\n\x17POWER_STATE_LIVE_CHARGE\x10\x05\x12\x1c\n\x18POWER_STATE_SLEEP_CHARGE\x10\x06\x12\x1b\n\x17POWER_STATE_LIVE_UPDATE\x10\x07\x12\x17\n\x13POWER_STATE_CLOUD_2\x10\n\x12\x17\n\x13POWER_STATE_MONITOR\x10\x0b*S\n\tLockState\x12\x16\n\x12LOCK_STATE_UNKNOWN\x10\x00\x12\x17\n\x13LOCK_STATE_UNLOCKED\x10\x01\x12\x15\n\x11LOCK_STATE_LOCKED\x10\x02*d\n\tDoorState\x12\x16\n\x12\x44OOR_STATE_UNKNOWN\x10\x00\x12\x13\n\x0f\x44OOR_STATE_OPEN\x10\x01\x12\x15\n\x11\x44OOR_STATE_CLOSED\x10\x02\x12\x13\n\x0f\x44OOR_STATE_AJAR\x10\x03*P\n\rWalkawayState\x12\x14\n\x10WALKAWAY_UNKNOWN\x10\x00\x12\x13\n\x0fWALKAWAY_ACTIVE\x10\x02\x12\x14\n\x10WALKAWAY_DISABLE\x10\x03*b\n\rAccessRequest\x12\x1a\n\x16\x41\x43\x43\x45SS_REQUEST_UNKNOWN\x10\x00\x12\x19\n\x15\x41\x43\x43\x45SS_REQUEST_ACTIVE\x10\x01\x12\x1a\n\x16\x41\x43\x43\x45SS_REQUEST_PASSIVE\x10\x02*n\n\nLightState\x12\x1e\n\x1aLIGHT_STATE_REALLY_UNKNOWN\x10\x00\x12\x13\n\x0fLIGHT_STATE_OFF\x10\x01\x12\x12\n\x0eLIGHT_STATE_ON\x10\x02\x12\x17\n\x13LIGHT_STATE_UNKNOWN\x10\x03*j\n\x0bLightAction\x12\x18\n\x14LIGHT_ACTION_UNKNOWN\x10\x00\x12\x16\n\x12LIGHT_ACTION_FLASH\x10\x01\x12\x13\n\x0fLIGHT_ACTION_ON\x10\x02\x12\x14\n\x10LIGHT_ACTION_OFF\x10\x03*\xc4\x01\n\x0b\x43hargeState\x12\x18\n\x14\x43HARGE_STATE_UNKNOWN\x10\x00\x12\x1e\n\x1a\x43HARGE_STATE_NOT_CONNECTED\x10\x01\x12 \n\x1c\x43HARGE_STATE_CABLE_CONNECTED\x10\x02\x12\x19\n\x15\x43HARGE_STATE_CHARGING\x10\x08\x12 \n\x1c\x43HARGE_STATE_CHARGING_END_OK\x10\t\x12\x1c\n\x18\x43HARGE_STATE_DISCHARGING\x10\x13*\xb9\x01\n\x14ScheduledChargeState\x12\"\n\x1eSCHEDULED_CHARGE_STATE_UNKNOWN\x10\x00\x12\x1f\n\x1bSCHEDULED_CHARGE_STATE_IDLE\x10\x01\x12.\n*SCHEDULED_CHARGE_STATE_SCHEDULED_TO_CHARGE\x10\x02\x12,\n(SCHEDULED_CHARGE_STATE_REQUEST_TO_CHARGE\x10\x03*x\n\x1fScheduledChargeUnavailableState\x12(\n$SCHEDULED_CHARGE_UNAVAILABLE_UNKNOWN\x10\x00\x12+\n\'SCHEDULED_CHARGE_UNAVAILABLE_NO_REQUEST\x10\x01*b\n\nEnergyType\x12\x17\n\x13\x45NERGY_TYPE_UNKNOWN\x10\x00\x12\x12\n\x0e\x45NERGY_TYPE_AC\x10\x01\x12\x12\n\x0e\x45NERGY_TYPE_DC\x10\x02\x12\x13\n\x0f\x45NERGY_TYPE_V2V\x10\x04*\xbb\x01\n\x0bUpdateState\x12\x18\n\x14UPDATE_STATE_UNKNOWN\x10\x00\x12\x1c\n\x18UPDATE_STATE_IN_PROGRESS\x10\x01\x12\x18\n\x14UPDATE_STATE_SUCCESS\x10\x02\x12\x17\n\x13UPDATE_STATE_FAILED\x10\x03\x12\x1f\n\x1bUPDATE_FAILED_DRIVE_ALLOWED\x10\x05\x12 \n\x1cUPDATE_SUCCESS_WITH_WARNINGS\x10\x07*K\n\x12UpdateAvailability\x12\x1f\n\x1bUPDATE_AVAILABILITY_UNKNOWN\x10\x00\x12\x14\n\x10UPDATE_AVAILABLE\x10\x01*Z\n\x0b\x41larmStatus\x12\x18\n\x14\x41LARM_STATUS_UNKNOWN\x10\x00\x12\x19\n\x15\x41LARM_STATUS_DISARMED\x10\x01\x12\x16\n\x12\x41LARM_STATUS_ARMED\x10\x02*a\n\tAlarmMode\x12\x16\n\x12\x41LARM_MODE_UNKNOWN\x10\x00\x12\x12\n\x0e\x41LARM_MODE_OFF\x10\x01\x12\x11\n\rALARM_MODE_ON\x10\x02\x12\x15\n\x11\x41LARM_MODE_SILENT\x10\x03*w\n\x14\x43loudConnectionState\x12\x1c\n\x18\x43LOUD_CONNECTION_UNKNOWN\x10\x00\x12\x1e\n\x1a\x43LOUD_CONNECTION_CONNECTED\x10\x01\x12!\n\x1d\x43LOUD_CONNECTION_DISCONNECTED\x10\x02*c\n\x13KeylessDrivingState\x12\x1b\n\x17KEYLESS_DRIVING_UNKNOWN\x10\x00\x12\x16\n\x12KEYLESS_DRIVING_ON\x10\x01\x12\x17\n\x13KEYLESS_DRIVING_OFF\x10\x02*i\n\tHvacPower\x12\x16\n\x12HVAC_POWER_UNKNOWN\x10\x00\x12\x0b\n\x07HVAC_ON\x10\x01\x12\x0c\n\x08HVAC_OFF\x10\x02\x12\x15\n\x11HVAC_PRECONDITION\x10\x03\x12\x12\n\x0eHVAC_KEEP_TEMP\x10\x06*J\n\x0c\x44\x65\x66rostState\x12\x19\n\x15\x44\x45\x46ROST_STATE_UNKNOWN\x10\x00\x12\x0e\n\nDEFROST_ON\x10\x01\x12\x0f\n\x0b\x44\x45\x46ROST_OFF\x10\x02*\x92\x01\n\x16HvacPreconditionStatus\x12$\n HVAC_PRECONDITION_STATUS_UNKNOWN\x10\x00\x12)\n%HVAC_PRECONDITION_STATUS_STILL_ACTIVE\x10\x01\x12\'\n#HVAC_PRECONDITION_STATUS_USER_INPUT\x10\x04*\xbe\x01\n\x11KeepClimateStatus\x12\x1f\n\x1bKEEP_CLIMATE_STATUS_UNKNOWN\x10\x00\x12 \n\x1cKEEP_CLIMATE_STATUS_INACTIVE\x10\x01\x12\x1f\n\x1bKEEP_CLIMATE_STATUS_ENABLED\x10\x02\x12 \n\x1cKEEP_CLIMATE_STATUS_CANCELED\x10\x03\x12#\n\x1fKEEP_CLIMATE_STATUS_PET_MODE_ON\x10\x04*:\n\x14KeepClimateCondition\x12\"\n\x1eKEEP_CLIMATE_CONDITION_UNKNOWN\x10\x00*\x84\x01\n\tDriveMode\x12\x16\n\x12\x44RIVE_MODE_UNKNOWN\x10\x00\x12\x16\n\x12\x44RIVE_MODE_COMFORT\x10\x01\x12\x14\n\x10\x44RIVE_MODE_SWIFT\x10\x02\x12\x19\n\x15\x44RIVE_MODE_SPORT_PLUS\x10\x05\x12\x16\n\x12\x44RIVE_MODE_SERVICE\x10\x08*v\n\x0bPrivacyMode\x12\x18\n\x14PRIVACY_MODE_UNKNOWN\x10\x00\x12%\n!PRIVACY_MODE_CONNECTIVITY_ENABLED\x10\x01\x12&\n\"PRIVACY_MODE_CONNECTIVITY_DISABLED\x10\x02*c\n\x0cGearPosition\x12\x10\n\x0cGEAR_UNKNOWN\x10\x00\x12\r\n\tGEAR_PARK\x10\x01\x12\x10\n\x0cGEAR_REVERSE\x10\x02\x12\x10\n\x0cGEAR_NEUTRAL\x10\x03\x12\x0e\n\nGEAR_DRIVE\x10\x04*E\n\x0fSharedTripState\x12\x17\n\x13SHARED_TRIP_UNKNOWN\x10\x00\x12\x19\n\x15SHARED_TRIP_AVAILABLE\x10\x01*9\n\nPanicState\x12\x17\n\x13PANIC_ALARM_UNKNOWN\x10\x00\x12\x12\n\x0ePANIC_ALARM_ON\x10\x01*Y\n\x08TcuState\x12\x0f\n\x0bTCU_UNKNOWN\x10\x00\x12\r\n\tTCU_SLEEP\x10\x01\x12\x0e\n\nTCU_DROWSY\x10\x02\x12\x0c\n\x08TCU_FULL\x10\x04\x12\x0f\n\x0bTCU_FACTORY\x10\x05*A\n\x07LteType\x12\x14\n\x10LTE_TYPE_UNKNOWN\x10\x00\x12\x0f\n\x0bLTE_TYPE_3G\x10\x01\x12\x0f\n\x0bLTE_TYPE_4G\x10\x02*`\n\x0eInternetStatus\x12\x1b\n\x17INTERNET_STATUS_UNKNOWN\x10\x00\x12\x19\n\x15INTERNET_DISCONNECTED\x10\x01\x12\x16\n\x12INTERNET_CONNECTED\x10\x02*Z\n\x0c\x43hargeAction\x12\x19\n\x15\x43HARGE_ACTION_UNKNOWN\x10\x00\x12\x17\n\x13\x43HARGE_ACTION_START\x10\x01\x12\x16\n\x12\x43HARGE_ACTION_STOP\x10\x02*\x95\x01\n\x0c\x44ocumentType\x12\x19\n\x15\x44OCUMENT_TYPE_UNKNOWN\x10\x00\x12#\n\x1f\x44OCUMENT_TYPE_RELEASE_NOTES_PRE\x10\x01\x12$\n DOCUMENT_TYPE_RELEASE_NOTES_POST\x10\x02\x12\x1f\n\x1b\x44OCUMENT_TYPE_OWNERS_MANUAL\x10\x03\x32\xe0\x0e\n\x13VehicleStateService\x12|\n\x13\x41pplySoftwareUpdate\x12\x30.mobilegateway.protos.ApplySoftwareUpdateRequest\x1a\x31.mobilegateway.protos.ApplySoftwareUpdateResponse\"\x00\x12\x82\x01\n\x15\x43\x61ncelScheduledUpdate\x12\x32.mobilegateway.protos.CancelScheduledUpdateRequest\x1a\x33.mobilegateway.protos.CancelScheduledUpdateResponse\"\x00\x12j\n\rChargeControl\x12*.mobilegateway.protos.ChargeControlRequest\x1a+.mobilegateway.protos.ChargeControlResponse\"\x00\x12v\n\x11\x43ontrolChargePort\x12..mobilegateway.protos.ControlChargePortRequest\x1a/.mobilegateway.protos.ControlChargePortResponse\"\x00\x12s\n\x10\x44oorLocksControl\x12-.mobilegateway.protos.DoorLocksControlRequest\x1a..mobilegateway.protos.DoorLocksControlResponse\"\x00\x12v\n\x11\x46rontCargoControl\x12..mobilegateway.protos.FrontCargoControlRequest\x1a/.mobilegateway.protos.FrontCargoControlResponse\"\x00\x12p\n\x0fGetDocumentInfo\x12,.mobilegateway.protos.GetDocumentInfoRequest\x1a-.mobilegateway.protos.GetDocumentInfoResponse\"\x00\x12p\n\x0fGetVehicleState\x12,.mobilegateway.protos.GetVehicleStateRequest\x1a-.mobilegateway.protos.GetVehicleStateResponse\"\x00\x12[\n\x08HonkHorn\x12%.mobilegateway.protos.HonkHornRequest\x1a&.mobilegateway.protos.HonkHornResponse\"\x00\x12y\n\x12HvacDefrostControl\x12/.mobilegateway.protos.HvacDefrostControlRequest\x1a\x30.mobilegateway.protos.HvacDefrostControlResponse\"\x00\x12j\n\rLightsControl\x12*.mobilegateway.protos.LightsControlRequest\x1a+.mobilegateway.protos.LightsControlResponse\"\x00\x12s\n\x10RearCargoControl\x12-.mobilegateway.protos.RearCargoControlRequest\x1a..mobilegateway.protos.RearCargoControlResponse\"\x00\x12\x7f\n\x14SecurityAlarmControl\x12\x31.mobilegateway.protos.SecurityAlarmControlRequest\x1a\x32.mobilegateway.protos.SecurityAlarmControlResponse\"\x00\x12|\n\x13SetCabinTemperature\x12\x30.mobilegateway.protos.SetCabinTemperatureRequest\x1a\x31.mobilegateway.protos.SetCabinTemperatureResponse\"\x00\x12m\n\x0eSetChargeLimit\x12+.mobilegateway.protos.SetChargeLimitRequest\x1a,.mobilegateway.protos.SetChargeLimitResponse\"\x00\x12j\n\rWakeupVehicle\x12*.mobilegateway.protos.WakeupVehicleRequest\x1a+.mobilegateway.protos.WakeupVehicleResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'vehicle_state_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
-  _globals['_ACCESSLEVEL']._serialized_start=8822
-  _globals['_ACCESSLEVEL']._serialized_end=8929
-  _globals['_MODEL']._serialized_start=8931
-  _globals['_MODEL']._serialized_end=8991
-  _globals['_MODELVARIANT']._serialized_start=8994
-  _globals['_MODELVARIANT']._serialized_end=9152
-  _globals['_PAINTCOLOR']._serialized_start=9155
-  _globals['_PAINTCOLOR']._serialized_end=9402
-  _globals['_LOOK']._serialized_start=9404
-  _globals['_LOOK']._serialized_end=9465
-  _globals['_WHEELS']._serialized_start=9467
-  _globals['_WHEELS']._serialized_end=9591
-  _globals['_SUBSCRIPTIONSTATUS']._serialized_start=9593
-  _globals['_SUBSCRIPTIONSTATUS']._serialized_end=9679
-  _globals['_CHARGINGACCOUNTSTATUS']._serialized_start=9681
-  _globals['_CHARGINGACCOUNTSTATUS']._serialized_end=9779
-  _globals['_CHARGINGVENDOR']._serialized_start=9781
-  _globals['_CHARGINGVENDOR']._serialized_end=9865
-  _globals['_EDITION']._serialized_start=9867
-  _globals['_EDITION']._serialized_end=9963
-  _globals['_BATTERYTYPE']._serialized_start=9966
-  _globals['_BATTERYTYPE']._serialized_end=10194
-  _globals['_INTERIOR']._serialized_start=10196
-  _globals['_INTERIOR']._serialized_end=10321
-  _globals['_STRUTTYPE']._serialized_start=10323
-  _globals['_STRUTTYPE']._serialized_end=10400
-  _globals['_ROOFTYPE']._serialized_start=10402
-  _globals['_ROOFTYPE']._serialized_end=10484
-  _globals['_WARNINGSTATE']._serialized_start=10486
-  _globals['_WARNINGSTATE']._serialized_end=10554
-  _globals['_BATTERYPRECONSTATUS']._serialized_start=10557
-  _globals['_BATTERYPRECONSTATUS']._serialized_end=10685
-  _globals['_POWERSTATE']._serialized_start=10688
-  _globals['_POWERSTATE']._serialized_end=10958
-  _globals['_LOCKSTATE']._serialized_start=10960
-  _globals['_LOCKSTATE']._serialized_end=11043
-  _globals['_DOORSTATE']._serialized_start=11045
-  _globals['_DOORSTATE']._serialized_end=11145
-  _globals['_WALKAWAYSTATE']._serialized_start=11147
-  _globals['_WALKAWAYSTATE']._serialized_end=11227
-  _globals['_ACCESSREQUEST']._serialized_start=11229
-  _globals['_ACCESSREQUEST']._serialized_end=11327
-  _globals['_LIGHTSTATE']._serialized_start=11329
-  _globals['_LIGHTSTATE']._serialized_end=11439
-  _globals['_LIGHTACTION']._serialized_start=11441
-  _globals['_LIGHTACTION']._serialized_end=11547
-  _globals['_CHARGESTATE']._serialized_start=11550
-  _globals['_CHARGESTATE']._serialized_end=11746
-  _globals['_SCHEDULEDCHARGESTATE']._serialized_start=11749
-  _globals['_SCHEDULEDCHARGESTATE']._serialized_end=11934
-  _globals['_SCHEDULEDCHARGEUNAVAILABLESTATE']._serialized_start=11936
-  _globals['_SCHEDULEDCHARGEUNAVAILABLESTATE']._serialized_end=12056
-  _globals['_ENERGYTYPE']._serialized_start=12058
-  _globals['_ENERGYTYPE']._serialized_end=12156
-  _globals['_UPDATESTATE']._serialized_start=12159
-  _globals['_UPDATESTATE']._serialized_end=12346
-  _globals['_UPDATEAVAILABILITY']._serialized_start=12348
-  _globals['_UPDATEAVAILABILITY']._serialized_end=12423
-  _globals['_ALARMSTATUS']._serialized_start=12425
-  _globals['_ALARMSTATUS']._serialized_end=12515
-  _globals['_ALARMMODE']._serialized_start=12517
-  _globals['_ALARMMODE']._serialized_end=12614
-  _globals['_CLOUDCONNECTIONSTATE']._serialized_start=12616
-  _globals['_CLOUDCONNECTIONSTATE']._serialized_end=12735
-  _globals['_KEYLESSDRIVINGSTATE']._serialized_start=12737
-  _globals['_KEYLESSDRIVINGSTATE']._serialized_end=12836
-  _globals['_HVACPOWER']._serialized_start=12838
-  _globals['_HVACPOWER']._serialized_end=12923
-  _globals['_DEFROSTSTATE']._serialized_start=12925
-  _globals['_DEFROSTSTATE']._serialized_end=12999
-  _globals['_HVACPRECONDITIONSTATUS']._serialized_start=13002
-  _globals['_HVACPRECONDITIONSTATUS']._serialized_end=13148
-  _globals['_DRIVEMODE']._serialized_start=13150
-  _globals['_DRIVEMODE']._serialized_end=13258
-  _globals['_PRIVACYMODE']._serialized_start=13260
-  _globals['_PRIVACYMODE']._serialized_end=13378
-  _globals['_GEARPOSITION']._serialized_start=13380
-  _globals['_GEARPOSITION']._serialized_end=13479
-  _globals['_SHAREDTRIPSTATE']._serialized_start=13481
-  _globals['_SHAREDTRIPSTATE']._serialized_end=13550
-  _globals['_TCUSTATE']._serialized_start=13552
-  _globals['_TCUSTATE']._serialized_end=13641
-  _globals['_LTETYPE']._serialized_start=13643
-  _globals['_LTETYPE']._serialized_end=13708
-  _globals['_INTERNETSTATUS']._serialized_start=13710
-  _globals['_INTERNETSTATUS']._serialized_end=13806
-  _globals['_CHARGEACTION']._serialized_start=13808
-  _globals['_CHARGEACTION']._serialized_end=13898
-  _globals['_DOCUMENTTYPE']._serialized_start=13901
-  _globals['_DOCUMENTTYPE']._serialized_end=14050
+  _globals['_ACCESSLEVEL']._serialized_start=9009
+  _globals['_ACCESSLEVEL']._serialized_end=9116
+  _globals['_MODEL']._serialized_start=9118
+  _globals['_MODEL']._serialized_end=9178
+  _globals['_MODELVARIANT']._serialized_start=9181
+  _globals['_MODELVARIANT']._serialized_end=9339
+  _globals['_PAINTCOLOR']._serialized_start=9342
+  _globals['_PAINTCOLOR']._serialized_end=9589
+  _globals['_LOOK']._serialized_start=9591
+  _globals['_LOOK']._serialized_end=9652
+  _globals['_WHEELS']._serialized_start=9654
+  _globals['_WHEELS']._serialized_end=9778
+  _globals['_SUBSCRIPTIONSTATUS']._serialized_start=9780
+  _globals['_SUBSCRIPTIONSTATUS']._serialized_end=9866
+  _globals['_CHARGINGACCOUNTSTATUS']._serialized_start=9868
+  _globals['_CHARGINGACCOUNTSTATUS']._serialized_end=9966
+  _globals['_CHARGINGVENDOR']._serialized_start=9968
+  _globals['_CHARGINGVENDOR']._serialized_end=10079
+  _globals['_EDITION']._serialized_start=10081
+  _globals['_EDITION']._serialized_end=10177
+  _globals['_BATTERYTYPE']._serialized_start=10180
+  _globals['_BATTERYTYPE']._serialized_end=10408
+  _globals['_INTERIOR']._serialized_start=10410
+  _globals['_INTERIOR']._serialized_end=10535
+  _globals['_STRUTTYPE']._serialized_start=10537
+  _globals['_STRUTTYPE']._serialized_end=10614
+  _globals['_ROOFTYPE']._serialized_start=10616
+  _globals['_ROOFTYPE']._serialized_end=10698
+  _globals['_WARNINGSTATE']._serialized_start=10700
+  _globals['_WARNINGSTATE']._serialized_end=10768
+  _globals['_BATTERYPRECONSTATUS']._serialized_start=10771
+  _globals['_BATTERYPRECONSTATUS']._serialized_end=10899
+  _globals['_POWERSTATE']._serialized_start=10902
+  _globals['_POWERSTATE']._serialized_end=11172
+  _globals['_LOCKSTATE']._serialized_start=11174
+  _globals['_LOCKSTATE']._serialized_end=11257
+  _globals['_DOORSTATE']._serialized_start=11259
+  _globals['_DOORSTATE']._serialized_end=11359
+  _globals['_WALKAWAYSTATE']._serialized_start=11361
+  _globals['_WALKAWAYSTATE']._serialized_end=11441
+  _globals['_ACCESSREQUEST']._serialized_start=11443
+  _globals['_ACCESSREQUEST']._serialized_end=11541
+  _globals['_LIGHTSTATE']._serialized_start=11543
+  _globals['_LIGHTSTATE']._serialized_end=11653
+  _globals['_LIGHTACTION']._serialized_start=11655
+  _globals['_LIGHTACTION']._serialized_end=11761
+  _globals['_CHARGESTATE']._serialized_start=11764
+  _globals['_CHARGESTATE']._serialized_end=11960
+  _globals['_SCHEDULEDCHARGESTATE']._serialized_start=11963
+  _globals['_SCHEDULEDCHARGESTATE']._serialized_end=12148
+  _globals['_SCHEDULEDCHARGEUNAVAILABLESTATE']._serialized_start=12150
+  _globals['_SCHEDULEDCHARGEUNAVAILABLESTATE']._serialized_end=12270
+  _globals['_ENERGYTYPE']._serialized_start=12272
+  _globals['_ENERGYTYPE']._serialized_end=12370
+  _globals['_UPDATESTATE']._serialized_start=12373
+  _globals['_UPDATESTATE']._serialized_end=12560
+  _globals['_UPDATEAVAILABILITY']._serialized_start=12562
+  _globals['_UPDATEAVAILABILITY']._serialized_end=12637
+  _globals['_ALARMSTATUS']._serialized_start=12639
+  _globals['_ALARMSTATUS']._serialized_end=12729
+  _globals['_ALARMMODE']._serialized_start=12731
+  _globals['_ALARMMODE']._serialized_end=12828
+  _globals['_CLOUDCONNECTIONSTATE']._serialized_start=12830
+  _globals['_CLOUDCONNECTIONSTATE']._serialized_end=12949
+  _globals['_KEYLESSDRIVINGSTATE']._serialized_start=12951
+  _globals['_KEYLESSDRIVINGSTATE']._serialized_end=13050
+  _globals['_HVACPOWER']._serialized_start=13052
+  _globals['_HVACPOWER']._serialized_end=13157
+  _globals['_DEFROSTSTATE']._serialized_start=13159
+  _globals['_DEFROSTSTATE']._serialized_end=13233
+  _globals['_HVACPRECONDITIONSTATUS']._serialized_start=13236
+  _globals['_HVACPRECONDITIONSTATUS']._serialized_end=13382
+  _globals['_KEEPCLIMATESTATUS']._serialized_start=13385
+  _globals['_KEEPCLIMATESTATUS']._serialized_end=13575
+  _globals['_KEEPCLIMATECONDITION']._serialized_start=13577
+  _globals['_KEEPCLIMATECONDITION']._serialized_end=13635
+  _globals['_DRIVEMODE']._serialized_start=13638
+  _globals['_DRIVEMODE']._serialized_end=13770
+  _globals['_PRIVACYMODE']._serialized_start=13772
+  _globals['_PRIVACYMODE']._serialized_end=13890
+  _globals['_GEARPOSITION']._serialized_start=13892
+  _globals['_GEARPOSITION']._serialized_end=13991
+  _globals['_SHAREDTRIPSTATE']._serialized_start=13993
+  _globals['_SHAREDTRIPSTATE']._serialized_end=14062
+  _globals['_PANICSTATE']._serialized_start=14064
+  _globals['_PANICSTATE']._serialized_end=14121
+  _globals['_TCUSTATE']._serialized_start=14123
+  _globals['_TCUSTATE']._serialized_end=14212
+  _globals['_LTETYPE']._serialized_start=14214
+  _globals['_LTETYPE']._serialized_end=14279
+  _globals['_INTERNETSTATUS']._serialized_start=14281
+  _globals['_INTERNETSTATUS']._serialized_end=14377
+  _globals['_CHARGEACTION']._serialized_start=14379
+  _globals['_CHARGEACTION']._serialized_end=14469
+  _globals['_DOCUMENTTYPE']._serialized_start=14472
+  _globals['_DOCUMENTTYPE']._serialized_end=14621
   _globals['_CHARGINGSUBSCRIPTION']._serialized_start=54
   _globals['_CHARGINGSUBSCRIPTION']._serialized_end=193
   _globals['_CHARGINGACCOUNT']._serialized_start=196
   _globals['_CHARGINGACCOUNT']._serialized_end=428
   _globals['_SPECIALIDENTIFIERS']._serialized_start=430
   _globals['_SPECIALIDENTIFIERS']._serialized_end=470
   _globals['_RESERVATION']._serialized_start=472
@@ -136,87 +142,87 @@
   _globals['_GPS']._serialized_start=3969
   _globals['_GPS']._serialized_end=4091
   _globals['_SOFTWAREUPDATE']._serialized_start=4094
   _globals['_SOFTWAREUPDATE']._serialized_end=4380
   _globals['_ALARMSTATE']._serialized_start=4382
   _globals['_ALARMSTATE']._serialized_end=4492
   _globals['_HVACSTATE']._serialized_start=4495
-  _globals['_HVACSTATE']._serialized_end=4682
-  _globals['_MOBILEAPPREQSTATE']._serialized_start=4685
-  _globals['_MOBILEAPPREQSTATE']._serialized_end=5199
-  _globals['_TCUINTERNETSTATE']._serialized_start=5202
-  _globals['_TCUINTERNETSTATE']._serialized_end=5460
-  _globals['_VEHICLESTATE']._serialized_start=5463
-  _globals['_VEHICLESTATE']._serialized_end=6490
-  _globals['_VEHICLE']._serialized_start=6493
-  _globals['_VEHICLE']._serialized_end=6683
-  _globals['_APPLYSOFTWAREUPDATEREQUEST']._serialized_start=6685
-  _globals['_APPLYSOFTWAREUPDATEREQUEST']._serialized_end=6733
-  _globals['_APPLYSOFTWAREUPDATERESPONSE']._serialized_start=6735
-  _globals['_APPLYSOFTWAREUPDATERESPONSE']._serialized_end=6764
-  _globals['_CANCELSCHEDULEDUPDATEREQUEST']._serialized_start=6766
-  _globals['_CANCELSCHEDULEDUPDATEREQUEST']._serialized_end=6816
-  _globals['_CANCELSCHEDULEDUPDATERESPONSE']._serialized_start=6818
-  _globals['_CANCELSCHEDULEDUPDATERESPONSE']._serialized_end=6849
-  _globals['_CHARGECONTROLREQUEST']._serialized_start=6851
-  _globals['_CHARGECONTROLREQUEST']._serialized_end=6945
-  _globals['_CHARGECONTROLRESPONSE']._serialized_start=6947
-  _globals['_CHARGECONTROLRESPONSE']._serialized_end=6970
-  _globals['_CONTROLCHARGEPORTREQUEST']._serialized_start=6972
-  _globals['_CONTROLCHARGEPORTREQUEST']._serialized_end=7074
-  _globals['_CONTROLCHARGEPORTRESPONSE']._serialized_start=7076
-  _globals['_CONTROLCHARGEPORTRESPONSE']._serialized_end=7103
-  _globals['_DOORLOCKSCONTROLREQUEST']._serialized_start=7105
-  _globals['_DOORLOCKSCONTROLREQUEST']._serialized_end=7226
-  _globals['_DOORLOCKSCONTROLRESPONSE']._serialized_start=7228
-  _globals['_DOORLOCKSCONTROLRESPONSE']._serialized_end=7254
-  _globals['_FRONTCARGOCONTROLREQUEST']._serialized_start=7256
-  _globals['_FRONTCARGOCONTROLREQUEST']._serialized_end=7358
-  _globals['_FRONTCARGOCONTROLRESPONSE']._serialized_start=7360
-  _globals['_FRONTCARGOCONTROLRESPONSE']._serialized_end=7387
-  _globals['_DOCUMENTINFOUNKNOWN']._serialized_start=7389
-  _globals['_DOCUMENTINFOUNKNOWN']._serialized_end=7429
-  _globals['_DOCUMENTINFO']._serialized_start=7432
-  _globals['_DOCUMENTINFO']._serialized_end=7594
-  _globals['_GETDOCUMENTINFOREQUEST']._serialized_start=7596
-  _globals['_GETDOCUMENTINFOREQUEST']._serialized_end=7696
-  _globals['_GETDOCUMENTINFORESPONSE']._serialized_start=7698
-  _globals['_GETDOCUMENTINFORESPONSE']._serialized_end=7786
-  _globals['_GETVEHICLESTATEREQUEST']._serialized_start=7788
-  _globals['_GETVEHICLESTATEREQUEST']._serialized_end=7832
-  _globals['_GETVEHICLESTATERESPONSE']._serialized_start=7834
-  _globals['_GETVEHICLESTATERESPONSE']._serialized_end=7930
-  _globals['_HONKHORNREQUEST']._serialized_start=7932
-  _globals['_HONKHORNREQUEST']._serialized_end=7969
-  _globals['_HONKHORNRESPONSE']._serialized_start=7971
-  _globals['_HONKHORNRESPONSE']._serialized_end=7989
-  _globals['_HVACDEFROSTCONTROLREQUEST']._serialized_start=7991
-  _globals['_HVACDEFROSTCONTROLREQUEST']._serialized_end=8096
-  _globals['_HVACDEFROSTCONTROLRESPONSE']._serialized_start=8098
-  _globals['_HVACDEFROSTCONTROLRESPONSE']._serialized_end=8126
-  _globals['_LIGHTSCONTROLREQUEST']._serialized_start=8128
-  _globals['_LIGHTSCONTROLREQUEST']._serialized_end=8221
-  _globals['_LIGHTSCONTROLRESPONSE']._serialized_start=8223
-  _globals['_LIGHTSCONTROLRESPONSE']._serialized_end=8246
-  _globals['_REARCARGOCONTROLREQUEST']._serialized_start=8248
-  _globals['_REARCARGOCONTROLREQUEST']._serialized_end=8349
-  _globals['_REARCARGOCONTROLRESPONSE']._serialized_start=8351
-  _globals['_REARCARGOCONTROLRESPONSE']._serialized_end=8377
-  _globals['_SECURITYALARMCONTROLREQUEST']._serialized_start=8379
-  _globals['_SECURITYALARMCONTROLREQUEST']._serialized_end=8475
-  _globals['_SECURITYALARMCONTROLRESPONSE']._serialized_start=8477
-  _globals['_SECURITYALARMCONTROLRESPONSE']._serialized_end=8507
-  _globals['_SETCABINTEMPERATUREREQUEST']._serialized_start=8509
-  _globals['_SETCABINTEMPERATUREREQUEST']._serialized_end=8626
-  _globals['_SETCABINTEMPERATURERESPONSE']._serialized_start=8628
-  _globals['_SETCABINTEMPERATURERESPONSE']._serialized_end=8657
-  _globals['_SETCHARGELIMITREQUEST']._serialized_start=8659
-  _globals['_SETCHARGELIMITREQUEST']._serialized_end=8725
-  _globals['_SETCHARGELIMITRESPONSE']._serialized_start=8727
-  _globals['_SETCHARGELIMITRESPONSE']._serialized_end=8751
-  _globals['_WAKEUPVEHICLEREQUEST']._serialized_start=8753
-  _globals['_WAKEUPVEHICLEREQUEST']._serialized_end=8795
-  _globals['_WAKEUPVEHICLERESPONSE']._serialized_start=8797
-  _globals['_WAKEUPVEHICLERESPONSE']._serialized_end=8820
-  _globals['_VEHICLESTATESERVICE']._serialized_start=14053
-  _globals['_VEHICLESTATESERVICE']._serialized_end=15941
+  _globals['_HVACSTATE']._serialized_end=4752
+  _globals['_MOBILEAPPREQSTATE']._serialized_start=4755
+  _globals['_MOBILEAPPREQSTATE']._serialized_end=5386
+  _globals['_TCUINTERNETSTATE']._serialized_start=5389
+  _globals['_TCUINTERNETSTATE']._serialized_end=5647
+  _globals['_VEHICLESTATE']._serialized_start=5650
+  _globals['_VEHICLESTATE']._serialized_end=6677
+  _globals['_VEHICLE']._serialized_start=6680
+  _globals['_VEHICLE']._serialized_end=6870
+  _globals['_APPLYSOFTWAREUPDATEREQUEST']._serialized_start=6872
+  _globals['_APPLYSOFTWAREUPDATEREQUEST']._serialized_end=6920
+  _globals['_APPLYSOFTWAREUPDATERESPONSE']._serialized_start=6922
+  _globals['_APPLYSOFTWAREUPDATERESPONSE']._serialized_end=6951
+  _globals['_CANCELSCHEDULEDUPDATEREQUEST']._serialized_start=6953
+  _globals['_CANCELSCHEDULEDUPDATEREQUEST']._serialized_end=7003
+  _globals['_CANCELSCHEDULEDUPDATERESPONSE']._serialized_start=7005
+  _globals['_CANCELSCHEDULEDUPDATERESPONSE']._serialized_end=7036
+  _globals['_CHARGECONTROLREQUEST']._serialized_start=7038
+  _globals['_CHARGECONTROLREQUEST']._serialized_end=7132
+  _globals['_CHARGECONTROLRESPONSE']._serialized_start=7134
+  _globals['_CHARGECONTROLRESPONSE']._serialized_end=7157
+  _globals['_CONTROLCHARGEPORTREQUEST']._serialized_start=7159
+  _globals['_CONTROLCHARGEPORTREQUEST']._serialized_end=7261
+  _globals['_CONTROLCHARGEPORTRESPONSE']._serialized_start=7263
+  _globals['_CONTROLCHARGEPORTRESPONSE']._serialized_end=7290
+  _globals['_DOORLOCKSCONTROLREQUEST']._serialized_start=7292
+  _globals['_DOORLOCKSCONTROLREQUEST']._serialized_end=7413
+  _globals['_DOORLOCKSCONTROLRESPONSE']._serialized_start=7415
+  _globals['_DOORLOCKSCONTROLRESPONSE']._serialized_end=7441
+  _globals['_FRONTCARGOCONTROLREQUEST']._serialized_start=7443
+  _globals['_FRONTCARGOCONTROLREQUEST']._serialized_end=7545
+  _globals['_FRONTCARGOCONTROLRESPONSE']._serialized_start=7547
+  _globals['_FRONTCARGOCONTROLRESPONSE']._serialized_end=7574
+  _globals['_DOCUMENTINFOUNKNOWN']._serialized_start=7576
+  _globals['_DOCUMENTINFOUNKNOWN']._serialized_end=7616
+  _globals['_DOCUMENTINFO']._serialized_start=7619
+  _globals['_DOCUMENTINFO']._serialized_end=7781
+  _globals['_GETDOCUMENTINFOREQUEST']._serialized_start=7783
+  _globals['_GETDOCUMENTINFOREQUEST']._serialized_end=7883
+  _globals['_GETDOCUMENTINFORESPONSE']._serialized_start=7885
+  _globals['_GETDOCUMENTINFORESPONSE']._serialized_end=7973
+  _globals['_GETVEHICLESTATEREQUEST']._serialized_start=7975
+  _globals['_GETVEHICLESTATEREQUEST']._serialized_end=8019
+  _globals['_GETVEHICLESTATERESPONSE']._serialized_start=8021
+  _globals['_GETVEHICLESTATERESPONSE']._serialized_end=8117
+  _globals['_HONKHORNREQUEST']._serialized_start=8119
+  _globals['_HONKHORNREQUEST']._serialized_end=8156
+  _globals['_HONKHORNRESPONSE']._serialized_start=8158
+  _globals['_HONKHORNRESPONSE']._serialized_end=8176
+  _globals['_HVACDEFROSTCONTROLREQUEST']._serialized_start=8178
+  _globals['_HVACDEFROSTCONTROLREQUEST']._serialized_end=8283
+  _globals['_HVACDEFROSTCONTROLRESPONSE']._serialized_start=8285
+  _globals['_HVACDEFROSTCONTROLRESPONSE']._serialized_end=8313
+  _globals['_LIGHTSCONTROLREQUEST']._serialized_start=8315
+  _globals['_LIGHTSCONTROLREQUEST']._serialized_end=8408
+  _globals['_LIGHTSCONTROLRESPONSE']._serialized_start=8410
+  _globals['_LIGHTSCONTROLRESPONSE']._serialized_end=8433
+  _globals['_REARCARGOCONTROLREQUEST']._serialized_start=8435
+  _globals['_REARCARGOCONTROLREQUEST']._serialized_end=8536
+  _globals['_REARCARGOCONTROLRESPONSE']._serialized_start=8538
+  _globals['_REARCARGOCONTROLRESPONSE']._serialized_end=8564
+  _globals['_SECURITYALARMCONTROLREQUEST']._serialized_start=8566
+  _globals['_SECURITYALARMCONTROLREQUEST']._serialized_end=8662
+  _globals['_SECURITYALARMCONTROLRESPONSE']._serialized_start=8664
+  _globals['_SECURITYALARMCONTROLRESPONSE']._serialized_end=8694
+  _globals['_SETCABINTEMPERATUREREQUEST']._serialized_start=8696
+  _globals['_SETCABINTEMPERATUREREQUEST']._serialized_end=8813
+  _globals['_SETCABINTEMPERATURERESPONSE']._serialized_start=8815
+  _globals['_SETCABINTEMPERATURERESPONSE']._serialized_end=8844
+  _globals['_SETCHARGELIMITREQUEST']._serialized_start=8846
+  _globals['_SETCHARGELIMITREQUEST']._serialized_end=8912
+  _globals['_SETCHARGELIMITRESPONSE']._serialized_start=8914
+  _globals['_SETCHARGELIMITRESPONSE']._serialized_end=8938
+  _globals['_WAKEUPVEHICLEREQUEST']._serialized_start=8940
+  _globals['_WAKEUPVEHICLEREQUEST']._serialized_end=8982
+  _globals['_WAKEUPVEHICLERESPONSE']._serialized_start=8984
+  _globals['_WAKEUPVEHICLERESPONSE']._serialized_end=9007
+  _globals['_VEHICLESTATESERVICE']._serialized_start=14624
+  _globals['_VEHICLESTATESERVICE']._serialized_end=16512
 # @@protoc_insertion_point(module_scope)
```

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/vehicle_state_service_pb2.py.orig` & `lucidmotors-1.1.2/lucidmotors/gen/vehicle_state_service_pb2.py.orig`

 * *Files 1% similar despite different names*

```diff
@@ -10,111 +10,117 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bvehicle_state_service.proto\x12\x14mobilegateway.protos\"\x8b\x01\n\x14\x43hargingSubscription\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x17\n\x0f\x65xpiration_date\x18\x02 \x01(\x04\x12\x12\n\nstart_date\x18\x03 \x01(\x04\x12\x38\n\x06status\x18\x04 \x01(\x0e\x32(.mobilegateway.protos.SubscriptionStatus\"\xe8\x01\n\x0f\x43hargingAccount\x12\x0e\n\x06\x65ma_id\x18\x01 \x01(\t\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\x12;\n\x06status\x18\x03 \x01(\x0e\x32+.mobilegateway.protos.ChargingAccountStatus\x12\x1c\n\x14\x63reated_at_epoch_sec\x18\x04 \x01(\x04\x12\x1b\n\x13\x65xpiry_on_epoch_sec\x18\x05 \x01(\x04\x12\x39\n\x0bvendor_name\x18\x06 \x01(\x0e\x32$.mobilegateway.protos.ChargingVendor\"(\n\x12SpecialIdentifiers\x12\x12\n\ndoor_plate\x18\x01 \x01(\t\"\x1b\n\x0bReservation\x12\x0c\n\x04\x64\x61te\x18\x01 \x01(\x04\"\x93\x07\n\rVehicleConfig\x12\x0b\n\x03vin\x18\x01 \x01(\t\x12*\n\x05model\x18\x02 \x01(\x0e\x32\x1b.mobilegateway.protos.Model\x12\x33\n\x07variant\x18\x03 \x01(\x0e\x32\".mobilegateway.protos.ModelVariant\x12\x10\n\x08nickname\x18\x05 \x01(\t\x12\x35\n\x0bpaint_color\x18\x06 \x01(\x0e\x32 .mobilegateway.protos.PaintColor\x12\x0e\n\x06\x65ma_id\x18\x07 \x01(\t\x12,\n\x06wheels\x18\x08 \x01(\x0e\x32\x1c.mobilegateway.protos.Wheels\x12\x43\n\x0f\x65\x61_subscription\x18\t \x01(\x0b\x32*.mobilegateway.protos.ChargingSubscription\x12@\n\x11\x63harging_accounts\x18\n \x03(\x0b\x32%.mobilegateway.protos.ChargingAccount\x12\x14\n\x0c\x63ountry_code\x18\x0b \x01(\t\x12\x13\n\x0bregion_code\x18\x0c \x01(\t\x12.\n\x07\x65\x64ition\x18\r \x01(\x0e\x32\x1d.mobilegateway.protos.Edition\x12\x32\n\x07\x62\x61ttery\x18\x0e \x01(\x0e\x32!.mobilegateway.protos.BatteryType\x12\x30\n\x08interior\x18\x0f \x01(\x0e\x32\x1e.mobilegateway.protos.Interior\x12\x45\n\x13special_identifiers\x18\x10 \x01(\x0b\x32(.mobilegateway.protos.SpecialIdentifiers\x12(\n\x04look\x18\x11 \x01(\x0e\x32\x1a.mobilegateway.protos.Look\x12\x1b\n\x13\x65xterior_color_code\x18\x12 \x01(\t\x12\x1b\n\x13interior_color_code\x18\x13 \x01(\t\x12\x34\n\x0b\x66runk_strut\x18\x14 \x01(\x0e\x32\x1f.mobilegateway.protos.StrutType\x12\x36\n\x0breservation\x18\x15 \x01(\x0b\x32!.mobilegateway.protos.Reservation\x12,\n\x04roof\x18\x16 \x01(\x0e\x32\x1e.mobilegateway.protos.RoofType\"\xaf\x03\n\x0c\x42\x61tteryState\x12\x17\n\x0fremaining_range\x18\x01 \x01(\x01\x12\x16\n\x0e\x63harge_percent\x18\x02 \x01(\x01\x12\x0c\n\x04kwhr\x18\x03 \x01(\x01\x12\x15\n\rcapacity_kwhr\x18\x04 \x01(\x01\x12:\n\x0e\x62\x61ttery_health\x18\x05 \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12<\n\x10low_charge_level\x18\x06 \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12\x41\n\x15\x63ritical_charge_level\x18\x07 \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12\x19\n\x11unavailable_range\x18\x08 \x01(\x01\x12I\n\x16preconditioning_status\x18\t \x01(\x0e\x32).mobilegateway.protos.BatteryPreconStatus\x12&\n\x1epreconditioning_time_remaining\x18\n \x01(\r\":\n\nCabinState\x12\x15\n\rinterior_temp\x18\x01 \x01(\x01\x12\x15\n\rexterior_temp\x18\x02 \x01(\x01\"\xc6\x04\n\tBodyState\x12\x33\n\ndoor_locks\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.LockState\x12\x34\n\x0b\x66ront_cargo\x18\x02 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x33\n\nrear_cargo\x18\x03 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x38\n\x0f\x66ront_left_door\x18\x04 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x39\n\x10\x66ront_right_door\x18\x05 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x37\n\x0erear_left_door\x18\x06 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x38\n\x0frear_right_door\x18\x07 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x34\n\x0b\x63harge_port\x18\x08 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12:\n\rwalkaway_lock\x18\t \x01(\x0e\x32#.mobilegateway.protos.WalkawayState\x12?\n\x12\x61\x63\x63\x65ss_type_status\x18\n \x01(\x0e\x32#.mobilegateway.protos.AccessRequest\"\x9b\x06\n\x0c\x43hassisState\x12\x13\n\x0bodometer_km\x18\x01 \x01(\x01\x12$\n\x1c\x66ront_left_tire_pressure_bar\x18\x02 \x01(\x01\x12%\n\x1d\x66ront_right_tire_pressure_bar\x18\x03 \x01(\x01\x12#\n\x1brear_left_tire_pressure_bar\x18\x04 \x01(\x01\x12$\n\x1crear_right_tire_pressure_bar\x18\x05 \x01(\x01\x12\x34\n\nheadlights\x18\x06 \x01(\x0e\x32 .mobilegateway.protos.LightState\x12@\n\x14hard_warn_left_front\x18\x08 \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12?\n\x13hard_warn_left_rear\x18\t \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12\x41\n\x15hard_warn_right_front\x18\n \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12@\n\x14hard_warn_right_rear\x18\x0b \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12@\n\x14soft_warn_left_front\x18\x0c \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12?\n\x13soft_warn_left_rear\x18\r \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12\x41\n\x15soft_warn_right_front\x18\x0e \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12@\n\x14soft_warn_right_rear\x18\x0f \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12\x18\n\x10software_version\x18\x10 \x01(\t\"\xed\x04\n\rChargingState\x12\x37\n\x0c\x63harge_state\x18\x01 \x01(\x0e\x32!.mobilegateway.protos.ChargeState\x12\x35\n\x0b\x65nergy_type\x18\x02 \x01(\x0e\x32 .mobilegateway.protos.EnergyType\x12\x19\n\x11\x63harge_session_mi\x18\x05 \x01(\x01\x12\x1a\n\x12\x63harge_session_kwh\x18\x06 \x01(\x01\x12!\n\x19session_minutes_remaining\x18\x07 \x01(\r\x12\x14\n\x0c\x63harge_limit\x18\x08 \x01(\r\x12\x33\n\ncable_lock\x18\n \x01(\x0e\x32\x1f.mobilegateway.protos.LockState\x12\x1f\n\x17\x63harge_rate_kwh_precise\x18\x0b \x01(\x01\x12\x1f\n\x17\x63harge_rate_mph_precise\x18\x0c \x01(\x01\x12%\n\x1d\x63harge_rate_miles_min_precise\x18\r \x01(\x01\x12\x1c\n\x14\x63harge_limit_percent\x18\x0e \x01(\x01\x12\x1d\n\x15\x63harge_scheduled_time\x18\x10 \x01(\r\x12\x44\n\x10scheduled_charge\x18\x11 \x01(\x0e\x32*.mobilegateway.protos.ScheduledChargeState\x12[\n\x1cscheduled_charge_unavailable\x18\x12 \x01(\x0e\x32\x35.mobilegateway.protos.ScheduledChargeUnavailableState\"/\n\x08Location\x12\x10\n\x08latitude\x18\x01 \x01(\x01\x12\x11\n\tlongitude\x18\x02 \x01(\x01\"z\n\x03Gps\x12\x30\n\x08location\x18\x01 \x01(\x0b\x32\x1e.mobilegateway.protos.Location\x12\x11\n\televation\x18\x02 \x01(\x05\x12\x15\n\rposition_time\x18\x04 \x01(\x04\x12\x17\n\x0fheading_precise\x18\x05 \x01(\x01\"\x9e\x02\n\x0eSoftwareUpdate\x12\x19\n\x11version_available\x18\x01 \x01(\t\x12 \n\x18install_duration_minutes\x18\x02 \x01(\r\x12\x18\n\x10percent_complete\x18\x04 \x01(\r\x12\x30\n\x05state\x18\x05 \x01(\x0e\x32!.mobilegateway.protos.UpdateState\x12\x1d\n\x15version_available_raw\x18\x08 \x01(\r\x12\x42\n\x10update_available\x18\t \x01(\x0e\x32(.mobilegateway.protos.UpdateAvailability\x12 \n\x18scheduled_start_time_sec\x18\n \x01(\x04\"n\n\nAlarmState\x12\x31\n\x06status\x18\x01 \x01(\x0e\x32!.mobilegateway.protos.AlarmStatus\x12-\n\x04mode\x18\x02 \x01(\x0e\x32\x1f.mobilegateway.protos.AlarmMode\"\xbb\x01\n\tHvacState\x12.\n\x05power\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.HvacPower\x12\x33\n\x07\x64\x65\x66rost\x18\x02 \x01(\x0e\x32\".mobilegateway.protos.DefrostState\x12I\n\x13precondition_status\x18\x03 \x01(\x0e\x32,.mobilegateway.protos.HvacPreconditionStatus\"\x82\x04\n\x11MobileAppReqState\x12<\n\x13\x63harge_port_request\x18\x02 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12<\n\x13\x66runk_cargo_request\x18\t \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x38\n\x0chvac_defrost\x18\x0b \x01(\x0e\x32\".mobilegateway.protos.DefrostState\x12:\n\x11hvac_precondition\x18\x0c \x01(\x0e\x32\x1f.mobilegateway.protos.HvacPower\x12\x38\n\rlight_request\x18\r \x01(\x0e\x32!.mobilegateway.protos.LightAction\x12\x42\n\x13shared_trip_request\x18\x0f \x01(\x0e\x32%.mobilegateway.protos.SharedTripState\x12<\n\x13trunk_cargo_request\x18\x10 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12?\n\x16vehicle_unlock_request\x18\x11 \x01(\x0e\x32\x1f.mobilegateway.protos.LockState\"\x82\x02\n\x10TcuInternetState\x12/\n\x08lte_type\x18\x01 \x01(\x0e\x32\x1d.mobilegateway.protos.LteType\x12\x38\n\nlte_status\x18\x02 \x01(\x0e\x32$.mobilegateway.protos.InternetStatus\x12\x39\n\x0bwifi_status\x18\x03 \x01(\x0e\x32$.mobilegateway.protos.InternetStatus\x12\x15\n\x08lte_rssi\x18\x04 \x01(\x05H\x00\x88\x01\x01\x12\x16\n\twifi_rssi\x18\x05 \x01(\x05H\x01\x88\x01\x01\x42\x0b\n\t_lte_rssiB\x0c\n\n_wifi_rssi\"\x83\x08\n\x0cVehicleState\x12\x33\n\x07\x62\x61ttery\x18\x01 \x01(\x0b\x32\".mobilegateway.protos.BatteryState\x12/\n\x05power\x18\x02 \x01(\x0e\x32 .mobilegateway.protos.PowerState\x12/\n\x05\x63\x61\x62in\x18\x03 \x01(\x0b\x32 .mobilegateway.protos.CabinState\x12-\n\x04\x62ody\x18\x04 \x01(\x0b\x32\x1f.mobilegateway.protos.BodyState\x12\x17\n\x0flast_updated_ms\x18\x05 \x01(\x04\x12\x33\n\x07\x63hassis\x18\x06 \x01(\x0b\x32\".mobilegateway.protos.ChassisState\x12\x35\n\x08\x63harging\x18\x08 \x01(\x0b\x32#.mobilegateway.protos.ChargingState\x12&\n\x03gps\x18\x0b \x01(\x0b\x32\x19.mobilegateway.protos.Gps\x12=\n\x0fsoftware_update\x18\x0c \x01(\x0b\x32$.mobilegateway.protos.SoftwareUpdate\x12/\n\x05\x61larm\x18\r \x01(\x0b\x32 .mobilegateway.protos.AlarmState\x12\x44\n\x10\x63loud_connection\x18\x0f \x01(\x0e\x32*.mobilegateway.protos.CloudConnectionState\x12\x42\n\x0fkeyless_driving\x18\x10 \x01(\x0e\x32).mobilegateway.protos.KeylessDrivingState\x12-\n\x04hvac\x18\x11 \x01(\x0b\x32\x1f.mobilegateway.protos.HvacState\x12\x33\n\ndrive_mode\x18\x12 \x01(\x0e\x32\x1f.mobilegateway.protos.DriveMode\x12\x37\n\x0cprivacy_mode\x18\x13 \x01(\x0e\x32!.mobilegateway.protos.PrivacyMode\x12\x39\n\rgear_position\x18\x14 \x01(\x0e\x32\".mobilegateway.protos.GearPosition\x12\x43\n\x12mobile_app_request\x18\x15 \x01(\x0b\x32\'.mobilegateway.protos.MobileAppReqState\x12+\n\x03tcu\x18\x16 \x01(\x0e\x32\x1e.mobilegateway.protos.TcuState\x12<\n\x0ctcu_internet\x18\x17 \x01(\x0b\x32&.mobilegateway.protos.TcuInternetState\"\xbe\x01\n\x07Vehicle\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\x12\x37\n\x0c\x61\x63\x63\x65ss_level\x18\x02 \x01(\x0e\x32!.mobilegateway.protos.AccessLevel\x12\x33\n\x06\x63onfig\x18\x03 \x01(\x0b\x32#.mobilegateway.protos.VehicleConfig\x12\x31\n\x05state\x18\x04 \x01(\x0b\x32\".mobilegateway.protos.VehicleState\"0\n\x1a\x41pplySoftwareUpdateRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\"\x1d\n\x1b\x41pplySoftwareUpdateResponse\"2\n\x1c\x43\x61ncelScheduledUpdateRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\"\x1f\n\x1d\x43\x61ncelScheduledUpdateResponse\"^\n\x14\x43hargeControlRequest\x12\x32\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32\".mobilegateway.protos.ChargeAction\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x17\n\x15\x43hargeControlResponse\"f\n\x18\x43ontrolChargePortRequest\x12\x36\n\rclosure_state\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x1b\n\x19\x43ontrolChargePortResponse\"y\n\x17\x44oorLocksControlRequest\x12\x15\n\rdoor_location\x18\x01 \x03(\x05\x12\x33\n\nlock_state\x18\x02 \x01(\x0e\x32\x1f.mobilegateway.protos.LockState\x12\x12\n\nvehicle_id\x18\x03 \x01(\t\"\x1a\n\x18\x44oorLocksControlResponse\"f\n\x18\x46rontCargoControlRequest\x12\x36\n\rclosure_state\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x1b\n\x19\x46rontCargoControlResponse\"(\n\x13\x44ocumentInfoUnknown\x12\x11\n\ttimestamp\x18\x01 \x01(\x04\"\xa2\x01\n\x0c\x44ocumentInfo\x12\x30\n\x04type\x18\x01 \x01(\x0e\x32\".mobilegateway.protos.DocumentType\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12:\n\x07unknown\x18\x05 \x01(\x0b\x32).mobilegateway.protos.DocumentInfoUnknown\"d\n\x16GetDocumentInfoRequest\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x39\n\rdocument_type\x18\x04 \x01(\x0e\x32\".mobilegateway.protos.DocumentType\"X\n\x17GetDocumentInfoResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x30\n\x04info\x18\x02 \x01(\x0b\x32\".mobilegateway.protos.DocumentInfo\",\n\x16GetVehicleStateRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\"`\n\x17GetVehicleStateResponse\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\x12\x31\n\x05state\x18\x02 \x01(\x0b\x32\".mobilegateway.protos.VehicleState\"%\n\x0fHonkHornRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\"\x12\n\x10HonkHornResponse\"i\n\x19HvacDefrostControlRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\x12\x38\n\x0chvac_defrost\x18\x02 \x01(\x0e\x32\".mobilegateway.protos.DefrostState\"\x1c\n\x1aHvacDefrostControlResponse\"]\n\x14LightsControlRequest\x12\x31\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32!.mobilegateway.protos.LightAction\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x17\n\x15LightsControlResponse\"e\n\x17RearCargoControlRequest\x12\x36\n\rclosure_state\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x1a\n\x18RearCargoControlResponse\"`\n\x1bSecurityAlarmControlRequest\x12-\n\x04mode\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.AlarmMode\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x1e\n\x1cSecurityAlarmControlResponse\"u\n\x1aSetCabinTemperatureRequest\x12\x13\n\x0btemperature\x18\x01 \x01(\x01\x12.\n\x05state\x18\x02 \x01(\x0e\x32\x1f.mobilegateway.protos.HvacPower\x12\x12\n\nvehicle_id\x18\x03 \x01(\t\"\x1d\n\x1bSetCabinTemperatureResponse\"B\n\x15SetChargeLimitRequest\x12\x15\n\rlimit_percent\x18\x01 \x01(\r\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x18\n\x16SetChargeLimitResponse\"*\n\x14WakeupVehicleRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\"\x17\n\x15WakeupVehicleResponse*k\n\x0b\x41\x63\x63\x65ssLevel\x12\x18\n\x14\x41\x43\x43\x45SS_LEVEL_UNKNOWN\x10\x00\x12\"\n\x1e\x41\x43\x43\x45SS_LEVEL_PREDELIVERY_OWNER\x10\x01\x12\x1e\n\x1a\x41\x43\x43\x45SS_LEVEL_PRIMARY_OWNER\x10\x02*<\n\x05Model\x12\x11\n\rMODEL_UNKNOWN\x10\x00\x12\r\n\tMODEL_AIR\x10\x01\x12\x11\n\rMODEL_GRAVITY\x10\x02*\x9e\x01\n\x0cModelVariant\x12\x19\n\x15MODEL_VARIANT_UNKNOWN\x10\x00\x12\x1f\n\x1bMODEL_VARIANT_DREAM_EDITION\x10\x01\x12\x1f\n\x1bMODEL_VARIANT_GRAND_TOURING\x10\x02\x12\x19\n\x15MODEL_VARIANT_TOURING\x10\x03\x12\x16\n\x12MODEL_VARIANT_PURE\x10\x04*\xf7\x01\n\nPaintColor\x12\x17\n\x13PAINT_COLOR_UNKNOWN\x10\x00\x12\x1b\n\x17PAINT_COLOR_EUREKA_GOLD\x10\x01\x12\x1d\n\x19PAINT_COLOR_STELLAR_WHITE\x10\x02\x12\x1e\n\x1aPAINT_COLOR_INFINITE_BLACK\x10\x03\x12\x1d\n\x19PAINT_COLOR_COSMOS_SILVER\x10\x04\x12\x1c\n\x18PAINT_COLOR_QUANTUM_GREY\x10\x05\x12\x1a\n\x16PAINT_COLOR_ZENITH_RED\x10\x06\x12\x1b\n\x17PAINT_COLOR_FATHOM_BLUE\x10\x07*=\n\x04Look\x12\x10\n\x0cLOOK_UNKNOWN\x10\x00\x12\x11\n\rLOOK_PLATINUM\x10\x01\x12\x10\n\x0cLOOK_STEALTH\x10\x02*|\n\x06Wheels\x12\x12\n\x0eWHEELS_UNKNOWN\x10\x00\x12\x10\n\x0cWHEELS_DREAM\x10\x01\x12\x10\n\x0cWHEELS_BLADE\x10\x02\x12\x0f\n\x0bWHEELS_LITE\x10\x03\x12\x10\n\x0cWHEELS_RANGE\x10\x04\x12\x17\n\x13WHEELS_LITE_STEALTH\x10\x08*V\n\x12SubscriptionStatus\x12\x1f\n\x1bSUBSCRIPTION_STATUS_UNKNOWN\x10\x00\x12\x1f\n\x1bSUBSCRIPTION_STATUS_CURRENT\x10\x01*b\n\x15\x43hargingAccountStatus\x12#\n\x1f\x43HARGING_ACCOUNT_STATUS_UNKNOWN\x10\x00\x12$\n CHARGING_ACCOUNT_STATUS_ENROLLED\x10\x02*T\n\x0e\x43hargingVendor\x12\x1b\n\x17\x43HARGING_VENDOR_UNKNOWN\x10\x00\x12%\n!CHARGING_VENDOR_ELECTRIFY_AMERICA\x10\x01*`\n\x07\x45\x64ition\x12\x13\n\x0f\x45\x44ITION_UNKNOWN\x10\x00\x12\x17\n\x13\x45\x44ITION_PERFORMANCE\x10\x01\x12\x11\n\rEDITION_RANGE\x10\x02\x12\x14\n\x10\x45\x44ITION_STANDARD\x10\x03*\xe4\x01\n\x0b\x42\x61tteryType\x12\x18\n\x14\x42\x41TTERY_TYPE_UNKNOWN\x10\x00\x12\x13\n\x0f\x42\x41TTERY_TYPE_01\x10\x01\x12\x13\n\x0f\x42\x41TTERY_TYPE_02\x10\x02\x12\x13\n\x0f\x42\x41TTERY_TYPE_03\x10\x03\x12\x13\n\x0f\x42\x41TTERY_TYPE_04\x10\x04\x12\x13\n\x0f\x42\x41TTERY_TYPE_05\x10\x05\x12\x13\n\x0f\x42\x41TTERY_TYPE_06\x10\x06\x12\x13\n\x0f\x42\x41TTERY_TYPE_07\x10\x07\x12\x13\n\x0f\x42\x41TTERY_TYPE_08\x10\x08\x12\x13\n\x0f\x42\x41TTERY_TYPE_09\x10\t*}\n\x08Interior\x12\x14\n\x10INTERIOR_UNKNOWN\x10\x00\x12\x17\n\x13INTERIOR_SANTA_CRUZ\x10\x01\x12\x12\n\x0eINTERIOR_TAHOE\x10\x02\x12\x13\n\x0fINTERIOR_MOJAVE\x10\x03\x12\x19\n\x15INTERIOR_SANTA_MONICA\x10\x05*M\n\tStrutType\x12\x16\n\x12STRUT_TYPE_UNKNOWN\x10\x00\x12\x12\n\x0eSTRUT_TYPE_GAS\x10\x01\x12\x14\n\x10STRUT_TYPE_POWER\x10\x02*R\n\x08RoofType\x12\x15\n\x11ROOF_TYPE_UNKNOWN\x10\x00\x12\x1a\n\x16ROOF_TYPE_GLASS_CANOPY\x10\x01\x12\x13\n\x0fROOF_TYPE_METAL\x10\x02*D\n\x0cWarningState\x12\x13\n\x0fWARNING_UNKNOWN\x10\x00\x12\x0f\n\x0bWARNING_OFF\x10\x01\x12\x0e\n\nWARNING_ON\x10\x02*\x80\x01\n\x13\x42\x61tteryPreconStatus\x12\x1a\n\x16\x42\x41TTERY_PRECON_UNKNOWN\x10\x00\x12\x16\n\x12\x42\x41TTERY_PRECON_OFF\x10\x01\x12\x15\n\x11\x42\x41TTERY_PRECON_ON\x10\x02\x12\x1e\n\x1a\x42\x41TTERY_PRECON_UNAVAILABLE\x10\x03*\x8e\x02\n\nPowerState\x12\x17\n\x13POWER_STATE_UNKNOWN\x10\x00\x12\x15\n\x11POWER_STATE_SLEEP\x10\x01\x12\x14\n\x10POWER_STATE_WINK\x10\x02\x12\x19\n\x15POWER_STATE_ACCESSORY\x10\x03\x12\x15\n\x11POWER_STATE_DRIVE\x10\x04\x12\x1b\n\x17POWER_STATE_LIVE_CHARGE\x10\x05\x12\x1c\n\x18POWER_STATE_SLEEP_CHARGE\x10\x06\x12\x1b\n\x17POWER_STATE_LIVE_UPDATE\x10\x07\x12\x17\n\x13POWER_STATE_CLOUD_2\x10\n\x12\x17\n\x13POWER_STATE_MONITOR\x10\x0b*S\n\tLockState\x12\x16\n\x12LOCK_STATE_UNKNOWN\x10\x00\x12\x17\n\x13LOCK_STATE_UNLOCKED\x10\x01\x12\x15\n\x11LOCK_STATE_LOCKED\x10\x02*d\n\tDoorState\x12\x16\n\x12\x44OOR_STATE_UNKNOWN\x10\x00\x12\x13\n\x0f\x44OOR_STATE_OPEN\x10\x01\x12\x15\n\x11\x44OOR_STATE_CLOSED\x10\x02\x12\x13\n\x0f\x44OOR_STATE_AJAR\x10\x03*P\n\rWalkawayState\x12\x14\n\x10WALKAWAY_UNKNOWN\x10\x00\x12\x13\n\x0fWALKAWAY_ACTIVE\x10\x02\x12\x14\n\x10WALKAWAY_DISABLE\x10\x03*b\n\rAccessRequest\x12\x1a\n\x16\x41\x43\x43\x45SS_REQUEST_UNKNOWN\x10\x00\x12\x19\n\x15\x41\x43\x43\x45SS_REQUEST_ACTIVE\x10\x01\x12\x1a\n\x16\x41\x43\x43\x45SS_REQUEST_PASSIVE\x10\x02*n\n\nLightState\x12\x1e\n\x1aLIGHT_STATE_REALLY_UNKNOWN\x10\x00\x12\x13\n\x0fLIGHT_STATE_OFF\x10\x01\x12\x12\n\x0eLIGHT_STATE_ON\x10\x02\x12\x17\n\x13LIGHT_STATE_UNKNOWN\x10\x03*j\n\x0bLightAction\x12\x18\n\x14LIGHT_ACTION_UNKNOWN\x10\x00\x12\x16\n\x12LIGHT_ACTION_FLASH\x10\x01\x12\x13\n\x0fLIGHT_ACTION_ON\x10\x02\x12\x14\n\x10LIGHT_ACTION_OFF\x10\x03*\xc4\x01\n\x0b\x43hargeState\x12\x18\n\x14\x43HARGE_STATE_UNKNOWN\x10\x00\x12\x1e\n\x1a\x43HARGE_STATE_NOT_CONNECTED\x10\x01\x12 \n\x1c\x43HARGE_STATE_CABLE_CONNECTED\x10\x02\x12\x19\n\x15\x43HARGE_STATE_CHARGING\x10\x08\x12 \n\x1c\x43HARGE_STATE_CHARGING_END_OK\x10\t\x12\x1c\n\x18\x43HARGE_STATE_DISCHARGING\x10\x13*\xb9\x01\n\x14ScheduledChargeState\x12\"\n\x1eSCHEDULED_CHARGE_STATE_UNKNOWN\x10\x00\x12\x1f\n\x1bSCHEDULED_CHARGE_STATE_IDLE\x10\x01\x12.\n*SCHEDULED_CHARGE_STATE_SCHEDULED_TO_CHARGE\x10\x02\x12,\n(SCHEDULED_CHARGE_STATE_REQUEST_TO_CHARGE\x10\x03*x\n\x1fScheduledChargeUnavailableState\x12(\n$SCHEDULED_CHARGE_UNAVAILABLE_UNKNOWN\x10\x00\x12+\n\'SCHEDULED_CHARGE_UNAVAILABLE_NO_REQUEST\x10\x01*b\n\nEnergyType\x12\x17\n\x13\x45NERGY_TYPE_UNKNOWN\x10\x00\x12\x12\n\x0e\x45NERGY_TYPE_AC\x10\x01\x12\x12\n\x0e\x45NERGY_TYPE_DC\x10\x02\x12\x13\n\x0f\x45NERGY_TYPE_V2V\x10\x04*\xbb\x01\n\x0bUpdateState\x12\x18\n\x14UPDATE_STATE_UNKNOWN\x10\x00\x12\x1c\n\x18UPDATE_STATE_IN_PROGRESS\x10\x01\x12\x18\n\x14UPDATE_STATE_SUCCESS\x10\x02\x12\x17\n\x13UPDATE_STATE_FAILED\x10\x03\x12\x1f\n\x1bUPDATE_FAILED_DRIVE_ALLOWED\x10\x05\x12 \n\x1cUPDATE_SUCCESS_WITH_WARNINGS\x10\x07*K\n\x12UpdateAvailability\x12\x1f\n\x1bUPDATE_AVAILABILITY_UNKNOWN\x10\x00\x12\x14\n\x10UPDATE_AVAILABLE\x10\x01*Z\n\x0b\x41larmStatus\x12\x18\n\x14\x41LARM_STATUS_UNKNOWN\x10\x00\x12\x19\n\x15\x41LARM_STATUS_DISARMED\x10\x01\x12\x16\n\x12\x41LARM_STATUS_ARMED\x10\x02*a\n\tAlarmMode\x12\x16\n\x12\x41LARM_MODE_UNKNOWN\x10\x00\x12\x12\n\x0e\x41LARM_MODE_OFF\x10\x01\x12\x11\n\rALARM_MODE_ON\x10\x02\x12\x15\n\x11\x41LARM_MODE_SILENT\x10\x03*w\n\x14\x43loudConnectionState\x12\x1c\n\x18\x43LOUD_CONNECTION_UNKNOWN\x10\x00\x12\x1e\n\x1a\x43LOUD_CONNECTION_CONNECTED\x10\x01\x12!\n\x1d\x43LOUD_CONNECTION_DISCONNECTED\x10\x02*c\n\x13KeylessDrivingState\x12\x1b\n\x17KEYLESS_DRIVING_UNKNOWN\x10\x00\x12\x16\n\x12KEYLESS_DRIVING_ON\x10\x01\x12\x17\n\x13KEYLESS_DRIVING_OFF\x10\x02*U\n\tHvacPower\x12\x16\n\x12HVAC_POWER_UNKNOWN\x10\x00\x12\x0b\n\x07HVAC_ON\x10\x01\x12\x0c\n\x08HVAC_OFF\x10\x02\x12\x15\n\x11HVAC_PRECONDITION\x10\x03*J\n\x0c\x44\x65\x66rostState\x12\x19\n\x15\x44\x45\x46ROST_STATE_UNKNOWN\x10\x00\x12\x0e\n\nDEFROST_ON\x10\x01\x12\x0f\n\x0b\x44\x45\x46ROST_OFF\x10\x02*\x92\x01\n\x16HvacPreconditionStatus\x12$\n HVAC_PRECONDITION_STATUS_UNKNOWN\x10\x00\x12)\n%HVAC_PRECONDITION_STATUS_STILL_ACTIVE\x10\x01\x12\'\n#HVAC_PRECONDITION_STATUS_USER_INPUT\x10\x04*l\n\tDriveMode\x12\x16\n\x12\x44RIVE_MODE_UNKNOWN\x10\x00\x12\x16\n\x12\x44RIVE_MODE_COMFORT\x10\x01\x12\x14\n\x10\x44RIVE_MODE_SWIFT\x10\x02\x12\x19\n\x15\x44RIVE_MODE_SPORT_PLUS\x10\x05*v\n\x0bPrivacyMode\x12\x18\n\x14PRIVACY_MODE_UNKNOWN\x10\x00\x12%\n!PRIVACY_MODE_CONNECTIVITY_ENABLED\x10\x01\x12&\n\"PRIVACY_MODE_CONNECTIVITY_DISABLED\x10\x02*c\n\x0cGearPosition\x12\x10\n\x0cGEAR_UNKNOWN\x10\x00\x12\r\n\tGEAR_PARK\x10\x01\x12\x10\n\x0cGEAR_REVERSE\x10\x02\x12\x10\n\x0cGEAR_NEUTRAL\x10\x03\x12\x0e\n\nGEAR_DRIVE\x10\x04*E\n\x0fSharedTripState\x12\x17\n\x13SHARED_TRIP_UNKNOWN\x10\x00\x12\x19\n\x15SHARED_TRIP_AVAILABLE\x10\x01*Y\n\x08TcuState\x12\x0f\n\x0bTCU_UNKNOWN\x10\x00\x12\r\n\tTCU_SLEEP\x10\x01\x12\x0e\n\nTCU_DROWSY\x10\x02\x12\x0c\n\x08TCU_FULL\x10\x04\x12\x0f\n\x0bTCU_FACTORY\x10\x05*A\n\x07LteType\x12\x14\n\x10LTE_TYPE_UNKNOWN\x10\x00\x12\x0f\n\x0bLTE_TYPE_3G\x10\x01\x12\x0f\n\x0bLTE_TYPE_4G\x10\x02*`\n\x0eInternetStatus\x12\x1b\n\x17INTERNET_STATUS_UNKNOWN\x10\x00\x12\x19\n\x15INTERNET_DISCONNECTED\x10\x01\x12\x16\n\x12INTERNET_CONNECTED\x10\x02*Z\n\x0c\x43hargeAction\x12\x19\n\x15\x43HARGE_ACTION_UNKNOWN\x10\x00\x12\x17\n\x13\x43HARGE_ACTION_START\x10\x01\x12\x16\n\x12\x43HARGE_ACTION_STOP\x10\x02*\x95\x01\n\x0c\x44ocumentType\x12\x19\n\x15\x44OCUMENT_TYPE_UNKNOWN\x10\x00\x12#\n\x1f\x44OCUMENT_TYPE_RELEASE_NOTES_PRE\x10\x01\x12$\n DOCUMENT_TYPE_RELEASE_NOTES_POST\x10\x02\x12\x1f\n\x1b\x44OCUMENT_TYPE_OWNERS_MANUAL\x10\x03\x32\xe0\x0e\n\x13VehicleStateService\x12|\n\x13\x41pplySoftwareUpdate\x12\x30.mobilegateway.protos.ApplySoftwareUpdateRequest\x1a\x31.mobilegateway.protos.ApplySoftwareUpdateResponse\"\x00\x12\x82\x01\n\x15\x43\x61ncelScheduledUpdate\x12\x32.mobilegateway.protos.CancelScheduledUpdateRequest\x1a\x33.mobilegateway.protos.CancelScheduledUpdateResponse\"\x00\x12j\n\rChargeControl\x12*.mobilegateway.protos.ChargeControlRequest\x1a+.mobilegateway.protos.ChargeControlResponse\"\x00\x12v\n\x11\x43ontrolChargePort\x12..mobilegateway.protos.ControlChargePortRequest\x1a/.mobilegateway.protos.ControlChargePortResponse\"\x00\x12s\n\x10\x44oorLocksControl\x12-.mobilegateway.protos.DoorLocksControlRequest\x1a..mobilegateway.protos.DoorLocksControlResponse\"\x00\x12v\n\x11\x46rontCargoControl\x12..mobilegateway.protos.FrontCargoControlRequest\x1a/.mobilegateway.protos.FrontCargoControlResponse\"\x00\x12p\n\x0fGetDocumentInfo\x12,.mobilegateway.protos.GetDocumentInfoRequest\x1a-.mobilegateway.protos.GetDocumentInfoResponse\"\x00\x12p\n\x0fGetVehicleState\x12,.mobilegateway.protos.GetVehicleStateRequest\x1a-.mobilegateway.protos.GetVehicleStateResponse\"\x00\x12[\n\x08HonkHorn\x12%.mobilegateway.protos.HonkHornRequest\x1a&.mobilegateway.protos.HonkHornResponse\"\x00\x12y\n\x12HvacDefrostControl\x12/.mobilegateway.protos.HvacDefrostControlRequest\x1a\x30.mobilegateway.protos.HvacDefrostControlResponse\"\x00\x12j\n\rLightsControl\x12*.mobilegateway.protos.LightsControlRequest\x1a+.mobilegateway.protos.LightsControlResponse\"\x00\x12s\n\x10RearCargoControl\x12-.mobilegateway.protos.RearCargoControlRequest\x1a..mobilegateway.protos.RearCargoControlResponse\"\x00\x12\x7f\n\x14SecurityAlarmControl\x12\x31.mobilegateway.protos.SecurityAlarmControlRequest\x1a\x32.mobilegateway.protos.SecurityAlarmControlResponse\"\x00\x12|\n\x13SetCabinTemperature\x12\x30.mobilegateway.protos.SetCabinTemperatureRequest\x1a\x31.mobilegateway.protos.SetCabinTemperatureResponse\"\x00\x12m\n\x0eSetChargeLimit\x12+.mobilegateway.protos.SetChargeLimitRequest\x1a,.mobilegateway.protos.SetChargeLimitResponse\"\x00\x12j\n\rWakeupVehicle\x12*.mobilegateway.protos.WakeupVehicleRequest\x1a+.mobilegateway.protos.WakeupVehicleResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bvehicle_state_service.proto\x12\x14mobilegateway.protos\"\x8b\x01\n\x14\x43hargingSubscription\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x17\n\x0f\x65xpiration_date\x18\x02 \x01(\x04\x12\x12\n\nstart_date\x18\x03 \x01(\x04\x12\x38\n\x06status\x18\x04 \x01(\x0e\x32(.mobilegateway.protos.SubscriptionStatus\"\xe8\x01\n\x0f\x43hargingAccount\x12\x0e\n\x06\x65ma_id\x18\x01 \x01(\t\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\x12;\n\x06status\x18\x03 \x01(\x0e\x32+.mobilegateway.protos.ChargingAccountStatus\x12\x1c\n\x14\x63reated_at_epoch_sec\x18\x04 \x01(\x04\x12\x1b\n\x13\x65xpiry_on_epoch_sec\x18\x05 \x01(\x04\x12\x39\n\x0bvendor_name\x18\x06 \x01(\x0e\x32$.mobilegateway.protos.ChargingVendor\"(\n\x12SpecialIdentifiers\x12\x12\n\ndoor_plate\x18\x01 \x01(\t\"\x1b\n\x0bReservation\x12\x0c\n\x04\x64\x61te\x18\x01 \x01(\x04\"\x93\x07\n\rVehicleConfig\x12\x0b\n\x03vin\x18\x01 \x01(\t\x12*\n\x05model\x18\x02 \x01(\x0e\x32\x1b.mobilegateway.protos.Model\x12\x33\n\x07variant\x18\x03 \x01(\x0e\x32\".mobilegateway.protos.ModelVariant\x12\x10\n\x08nickname\x18\x05 \x01(\t\x12\x35\n\x0bpaint_color\x18\x06 \x01(\x0e\x32 .mobilegateway.protos.PaintColor\x12\x0e\n\x06\x65ma_id\x18\x07 \x01(\t\x12,\n\x06wheels\x18\x08 \x01(\x0e\x32\x1c.mobilegateway.protos.Wheels\x12\x43\n\x0f\x65\x61_subscription\x18\t \x01(\x0b\x32*.mobilegateway.protos.ChargingSubscription\x12@\n\x11\x63harging_accounts\x18\n \x03(\x0b\x32%.mobilegateway.protos.ChargingAccount\x12\x14\n\x0c\x63ountry_code\x18\x0b \x01(\t\x12\x13\n\x0bregion_code\x18\x0c \x01(\t\x12.\n\x07\x65\x64ition\x18\r \x01(\x0e\x32\x1d.mobilegateway.protos.Edition\x12\x32\n\x07\x62\x61ttery\x18\x0e \x01(\x0e\x32!.mobilegateway.protos.BatteryType\x12\x30\n\x08interior\x18\x0f \x01(\x0e\x32\x1e.mobilegateway.protos.Interior\x12\x45\n\x13special_identifiers\x18\x10 \x01(\x0b\x32(.mobilegateway.protos.SpecialIdentifiers\x12(\n\x04look\x18\x11 \x01(\x0e\x32\x1a.mobilegateway.protos.Look\x12\x1b\n\x13\x65xterior_color_code\x18\x12 \x01(\t\x12\x1b\n\x13interior_color_code\x18\x13 \x01(\t\x12\x34\n\x0b\x66runk_strut\x18\x14 \x01(\x0e\x32\x1f.mobilegateway.protos.StrutType\x12\x36\n\x0breservation\x18\x15 \x01(\x0b\x32!.mobilegateway.protos.Reservation\x12,\n\x04roof\x18\x16 \x01(\x0e\x32\x1e.mobilegateway.protos.RoofType\"\xaf\x03\n\x0c\x42\x61tteryState\x12\x17\n\x0fremaining_range\x18\x01 \x01(\x01\x12\x16\n\x0e\x63harge_percent\x18\x02 \x01(\x01\x12\x0c\n\x04kwhr\x18\x03 \x01(\x01\x12\x15\n\rcapacity_kwhr\x18\x04 \x01(\x01\x12:\n\x0e\x62\x61ttery_health\x18\x05 \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12<\n\x10low_charge_level\x18\x06 \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12\x41\n\x15\x63ritical_charge_level\x18\x07 \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12\x19\n\x11unavailable_range\x18\x08 \x01(\x01\x12I\n\x16preconditioning_status\x18\t \x01(\x0e\x32).mobilegateway.protos.BatteryPreconStatus\x12&\n\x1epreconditioning_time_remaining\x18\n \x01(\r\":\n\nCabinState\x12\x15\n\rinterior_temp\x18\x01 \x01(\x01\x12\x15\n\rexterior_temp\x18\x02 \x01(\x01\"\xc6\x04\n\tBodyState\x12\x33\n\ndoor_locks\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.LockState\x12\x34\n\x0b\x66ront_cargo\x18\x02 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x33\n\nrear_cargo\x18\x03 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x38\n\x0f\x66ront_left_door\x18\x04 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x39\n\x10\x66ront_right_door\x18\x05 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x37\n\x0erear_left_door\x18\x06 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x38\n\x0frear_right_door\x18\x07 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x34\n\x0b\x63harge_port\x18\x08 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12:\n\rwalkaway_lock\x18\t \x01(\x0e\x32#.mobilegateway.protos.WalkawayState\x12?\n\x12\x61\x63\x63\x65ss_type_status\x18\n \x01(\x0e\x32#.mobilegateway.protos.AccessRequest\"\x9b\x06\n\x0c\x43hassisState\x12\x13\n\x0bodometer_km\x18\x01 \x01(\x01\x12$\n\x1c\x66ront_left_tire_pressure_bar\x18\x02 \x01(\x01\x12%\n\x1d\x66ront_right_tire_pressure_bar\x18\x03 \x01(\x01\x12#\n\x1brear_left_tire_pressure_bar\x18\x04 \x01(\x01\x12$\n\x1crear_right_tire_pressure_bar\x18\x05 \x01(\x01\x12\x34\n\nheadlights\x18\x06 \x01(\x0e\x32 .mobilegateway.protos.LightState\x12@\n\x14hard_warn_left_front\x18\x08 \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12?\n\x13hard_warn_left_rear\x18\t \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12\x41\n\x15hard_warn_right_front\x18\n \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12@\n\x14hard_warn_right_rear\x18\x0b \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12@\n\x14soft_warn_left_front\x18\x0c \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12?\n\x13soft_warn_left_rear\x18\r \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12\x41\n\x15soft_warn_right_front\x18\x0e \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12@\n\x14soft_warn_right_rear\x18\x0f \x01(\x0e\x32\".mobilegateway.protos.WarningState\x12\x18\n\x10software_version\x18\x10 \x01(\t\"\xed\x04\n\rChargingState\x12\x37\n\x0c\x63harge_state\x18\x01 \x01(\x0e\x32!.mobilegateway.protos.ChargeState\x12\x35\n\x0b\x65nergy_type\x18\x02 \x01(\x0e\x32 .mobilegateway.protos.EnergyType\x12\x19\n\x11\x63harge_session_mi\x18\x05 \x01(\x01\x12\x1a\n\x12\x63harge_session_kwh\x18\x06 \x01(\x01\x12!\n\x19session_minutes_remaining\x18\x07 \x01(\r\x12\x14\n\x0c\x63harge_limit\x18\x08 \x01(\r\x12\x33\n\ncable_lock\x18\n \x01(\x0e\x32\x1f.mobilegateway.protos.LockState\x12\x1f\n\x17\x63harge_rate_kwh_precise\x18\x0b \x01(\x01\x12\x1f\n\x17\x63harge_rate_mph_precise\x18\x0c \x01(\x01\x12%\n\x1d\x63harge_rate_miles_min_precise\x18\r \x01(\x01\x12\x1c\n\x14\x63harge_limit_percent\x18\x0e \x01(\x01\x12\x1d\n\x15\x63harge_scheduled_time\x18\x10 \x01(\r\x12\x44\n\x10scheduled_charge\x18\x11 \x01(\x0e\x32*.mobilegateway.protos.ScheduledChargeState\x12[\n\x1cscheduled_charge_unavailable\x18\x12 \x01(\x0e\x32\x35.mobilegateway.protos.ScheduledChargeUnavailableState\"/\n\x08Location\x12\x10\n\x08latitude\x18\x01 \x01(\x01\x12\x11\n\tlongitude\x18\x02 \x01(\x01\"z\n\x03Gps\x12\x30\n\x08location\x18\x01 \x01(\x0b\x32\x1e.mobilegateway.protos.Location\x12\x11\n\televation\x18\x02 \x01(\x05\x12\x15\n\rposition_time\x18\x04 \x01(\x04\x12\x17\n\x0fheading_precise\x18\x05 \x01(\x01\"\x9e\x02\n\x0eSoftwareUpdate\x12\x19\n\x11version_available\x18\x01 \x01(\t\x12 \n\x18install_duration_minutes\x18\x02 \x01(\r\x12\x18\n\x10percent_complete\x18\x04 \x01(\r\x12\x30\n\x05state\x18\x05 \x01(\x0e\x32!.mobilegateway.protos.UpdateState\x12\x1d\n\x15version_available_raw\x18\x08 \x01(\r\x12\x42\n\x10update_available\x18\t \x01(\x0e\x32(.mobilegateway.protos.UpdateAvailability\x12 \n\x18scheduled_start_time_sec\x18\n \x01(\x04\"n\n\nAlarmState\x12\x31\n\x06status\x18\x01 \x01(\x0e\x32!.mobilegateway.protos.AlarmStatus\x12-\n\x04mode\x18\x02 \x01(\x0e\x32\x1f.mobilegateway.protos.AlarmMode\"\x81\x02\n\tHvacState\x12.\n\x05power\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.HvacPower\x12\x33\n\x07\x64\x65\x66rost\x18\x02 \x01(\x0e\x32\".mobilegateway.protos.DefrostState\x12I\n\x13precondition_status\x18\x03 \x01(\x0e\x32,.mobilegateway.protos.HvacPreconditionStatus\x12\x44\n\x13keep_climate_status\x18\x05 \x01(\x0e\x32\'.mobilegateway.protos.KeepClimateStatus\"\xf7\x04\n\x11MobileAppReqState\x12:\n\x11\x61larm_set_request\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.AlarmMode\x12<\n\x13\x63harge_port_request\x18\x02 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12<\n\x13\x66runk_cargo_request\x18\t \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x38\n\x0chvac_defrost\x18\x0b \x01(\x0e\x32\".mobilegateway.protos.DefrostState\x12:\n\x11hvac_precondition\x18\x0c \x01(\x0e\x32\x1f.mobilegateway.protos.HvacPower\x12\x38\n\rlight_request\x18\r \x01(\x0e\x32!.mobilegateway.protos.LightAction\x12\x37\n\rpanic_request\x18\x0e \x01(\x0e\x32 .mobilegateway.protos.PanicState\x12\x42\n\x13shared_trip_request\x18\x0f \x01(\x0e\x32%.mobilegateway.protos.SharedTripState\x12<\n\x13trunk_cargo_request\x18\x10 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12?\n\x16vehicle_unlock_request\x18\x11 \x01(\x0e\x32\x1f.mobilegateway.protos.LockState\"\x82\x02\n\x10TcuInternetState\x12/\n\x08lte_type\x18\x01 \x01(\x0e\x32\x1d.mobilegateway.protos.LteType\x12\x38\n\nlte_status\x18\x02 \x01(\x0e\x32$.mobilegateway.protos.InternetStatus\x12\x39\n\x0bwifi_status\x18\x03 \x01(\x0e\x32$.mobilegateway.protos.InternetStatus\x12\x15\n\x08lte_rssi\x18\x04 \x01(\x05H\x00\x88\x01\x01\x12\x16\n\twifi_rssi\x18\x05 \x01(\x05H\x01\x88\x01\x01\x42\x0b\n\t_lte_rssiB\x0c\n\n_wifi_rssi\"\x83\x08\n\x0cVehicleState\x12\x33\n\x07\x62\x61ttery\x18\x01 \x01(\x0b\x32\".mobilegateway.protos.BatteryState\x12/\n\x05power\x18\x02 \x01(\x0e\x32 .mobilegateway.protos.PowerState\x12/\n\x05\x63\x61\x62in\x18\x03 \x01(\x0b\x32 .mobilegateway.protos.CabinState\x12-\n\x04\x62ody\x18\x04 \x01(\x0b\x32\x1f.mobilegateway.protos.BodyState\x12\x17\n\x0flast_updated_ms\x18\x05 \x01(\x04\x12\x33\n\x07\x63hassis\x18\x06 \x01(\x0b\x32\".mobilegateway.protos.ChassisState\x12\x35\n\x08\x63harging\x18\x08 \x01(\x0b\x32#.mobilegateway.protos.ChargingState\x12&\n\x03gps\x18\x0b \x01(\x0b\x32\x19.mobilegateway.protos.Gps\x12=\n\x0fsoftware_update\x18\x0c \x01(\x0b\x32$.mobilegateway.protos.SoftwareUpdate\x12/\n\x05\x61larm\x18\r \x01(\x0b\x32 .mobilegateway.protos.AlarmState\x12\x44\n\x10\x63loud_connection\x18\x0f \x01(\x0e\x32*.mobilegateway.protos.CloudConnectionState\x12\x42\n\x0fkeyless_driving\x18\x10 \x01(\x0e\x32).mobilegateway.protos.KeylessDrivingState\x12-\n\x04hvac\x18\x11 \x01(\x0b\x32\x1f.mobilegateway.protos.HvacState\x12\x33\n\ndrive_mode\x18\x12 \x01(\x0e\x32\x1f.mobilegateway.protos.DriveMode\x12\x37\n\x0cprivacy_mode\x18\x13 \x01(\x0e\x32!.mobilegateway.protos.PrivacyMode\x12\x39\n\rgear_position\x18\x14 \x01(\x0e\x32\".mobilegateway.protos.GearPosition\x12\x43\n\x12mobile_app_request\x18\x15 \x01(\x0b\x32\'.mobilegateway.protos.MobileAppReqState\x12+\n\x03tcu\x18\x16 \x01(\x0e\x32\x1e.mobilegateway.protos.TcuState\x12<\n\x0ctcu_internet\x18\x17 \x01(\x0b\x32&.mobilegateway.protos.TcuInternetState\"\xbe\x01\n\x07Vehicle\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\x12\x37\n\x0c\x61\x63\x63\x65ss_level\x18\x02 \x01(\x0e\x32!.mobilegateway.protos.AccessLevel\x12\x33\n\x06\x63onfig\x18\x03 \x01(\x0b\x32#.mobilegateway.protos.VehicleConfig\x12\x31\n\x05state\x18\x04 \x01(\x0b\x32\".mobilegateway.protos.VehicleState\"0\n\x1a\x41pplySoftwareUpdateRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\"\x1d\n\x1b\x41pplySoftwareUpdateResponse\"2\n\x1c\x43\x61ncelScheduledUpdateRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\"\x1f\n\x1d\x43\x61ncelScheduledUpdateResponse\"^\n\x14\x43hargeControlRequest\x12\x32\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32\".mobilegateway.protos.ChargeAction\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x17\n\x15\x43hargeControlResponse\"f\n\x18\x43ontrolChargePortRequest\x12\x36\n\rclosure_state\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x1b\n\x19\x43ontrolChargePortResponse\"y\n\x17\x44oorLocksControlRequest\x12\x15\n\rdoor_location\x18\x01 \x03(\x05\x12\x33\n\nlock_state\x18\x02 \x01(\x0e\x32\x1f.mobilegateway.protos.LockState\x12\x12\n\nvehicle_id\x18\x03 \x01(\t\"\x1a\n\x18\x44oorLocksControlResponse\"f\n\x18\x46rontCargoControlRequest\x12\x36\n\rclosure_state\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x1b\n\x19\x46rontCargoControlResponse\"(\n\x13\x44ocumentInfoUnknown\x12\x11\n\ttimestamp\x18\x01 \x01(\x04\"\xa2\x01\n\x0c\x44ocumentInfo\x12\x30\n\x04type\x18\x01 \x01(\x0e\x32\".mobilegateway.protos.DocumentType\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12:\n\x07unknown\x18\x05 \x01(\x0b\x32).mobilegateway.protos.DocumentInfoUnknown\"d\n\x16GetDocumentInfoRequest\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x39\n\rdocument_type\x18\x04 \x01(\x0e\x32\".mobilegateway.protos.DocumentType\"X\n\x17GetDocumentInfoResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x30\n\x04info\x18\x02 \x01(\x0b\x32\".mobilegateway.protos.DocumentInfo\",\n\x16GetVehicleStateRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\"`\n\x17GetVehicleStateResponse\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\x12\x31\n\x05state\x18\x02 \x01(\x0b\x32\".mobilegateway.protos.VehicleState\"%\n\x0fHonkHornRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\"\x12\n\x10HonkHornResponse\"i\n\x19HvacDefrostControlRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\x12\x38\n\x0chvac_defrost\x18\x02 \x01(\x0e\x32\".mobilegateway.protos.DefrostState\"\x1c\n\x1aHvacDefrostControlResponse\"]\n\x14LightsControlRequest\x12\x31\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32!.mobilegateway.protos.LightAction\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x17\n\x15LightsControlResponse\"e\n\x17RearCargoControlRequest\x12\x36\n\rclosure_state\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.DoorState\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x1a\n\x18RearCargoControlResponse\"`\n\x1bSecurityAlarmControlRequest\x12-\n\x04mode\x18\x01 \x01(\x0e\x32\x1f.mobilegateway.protos.AlarmMode\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x1e\n\x1cSecurityAlarmControlResponse\"u\n\x1aSetCabinTemperatureRequest\x12\x13\n\x0btemperature\x18\x01 \x01(\x01\x12.\n\x05state\x18\x02 \x01(\x0e\x32\x1f.mobilegateway.protos.HvacPower\x12\x12\n\nvehicle_id\x18\x03 \x01(\t\"\x1d\n\x1bSetCabinTemperatureResponse\"B\n\x15SetChargeLimitRequest\x12\x15\n\rlimit_percent\x18\x01 \x01(\r\x12\x12\n\nvehicle_id\x18\x02 \x01(\t\"\x18\n\x16SetChargeLimitResponse\"*\n\x14WakeupVehicleRequest\x12\x12\n\nvehicle_id\x18\x01 \x01(\t\"\x17\n\x15WakeupVehicleResponse*k\n\x0b\x41\x63\x63\x65ssLevel\x12\x18\n\x14\x41\x43\x43\x45SS_LEVEL_UNKNOWN\x10\x00\x12\"\n\x1e\x41\x43\x43\x45SS_LEVEL_PREDELIVERY_OWNER\x10\x01\x12\x1e\n\x1a\x41\x43\x43\x45SS_LEVEL_PRIMARY_OWNER\x10\x02*<\n\x05Model\x12\x11\n\rMODEL_UNKNOWN\x10\x00\x12\r\n\tMODEL_AIR\x10\x01\x12\x11\n\rMODEL_GRAVITY\x10\x02*\x9e\x01\n\x0cModelVariant\x12\x19\n\x15MODEL_VARIANT_UNKNOWN\x10\x00\x12\x1f\n\x1bMODEL_VARIANT_DREAM_EDITION\x10\x01\x12\x1f\n\x1bMODEL_VARIANT_GRAND_TOURING\x10\x02\x12\x19\n\x15MODEL_VARIANT_TOURING\x10\x03\x12\x16\n\x12MODEL_VARIANT_PURE\x10\x04*\xf7\x01\n\nPaintColor\x12\x17\n\x13PAINT_COLOR_UNKNOWN\x10\x00\x12\x1b\n\x17PAINT_COLOR_EUREKA_GOLD\x10\x01\x12\x1d\n\x19PAINT_COLOR_STELLAR_WHITE\x10\x02\x12\x1e\n\x1aPAINT_COLOR_INFINITE_BLACK\x10\x03\x12\x1d\n\x19PAINT_COLOR_COSMOS_SILVER\x10\x04\x12\x1c\n\x18PAINT_COLOR_QUANTUM_GREY\x10\x05\x12\x1a\n\x16PAINT_COLOR_ZENITH_RED\x10\x06\x12\x1b\n\x17PAINT_COLOR_FATHOM_BLUE\x10\x07*=\n\x04Look\x12\x10\n\x0cLOOK_UNKNOWN\x10\x00\x12\x11\n\rLOOK_PLATINUM\x10\x01\x12\x10\n\x0cLOOK_STEALTH\x10\x02*|\n\x06Wheels\x12\x12\n\x0eWHEELS_UNKNOWN\x10\x00\x12\x10\n\x0cWHEELS_DREAM\x10\x01\x12\x10\n\x0cWHEELS_BLADE\x10\x02\x12\x0f\n\x0bWHEELS_LITE\x10\x03\x12\x10\n\x0cWHEELS_RANGE\x10\x04\x12\x17\n\x13WHEELS_LITE_STEALTH\x10\x08*V\n\x12SubscriptionStatus\x12\x1f\n\x1bSUBSCRIPTION_STATUS_UNKNOWN\x10\x00\x12\x1f\n\x1bSUBSCRIPTION_STATUS_CURRENT\x10\x01*b\n\x15\x43hargingAccountStatus\x12#\n\x1f\x43HARGING_ACCOUNT_STATUS_UNKNOWN\x10\x00\x12$\n CHARGING_ACCOUNT_STATUS_ENROLLED\x10\x02*o\n\x0e\x43hargingVendor\x12\x1b\n\x17\x43HARGING_VENDOR_UNKNOWN\x10\x00\x12%\n!CHARGING_VENDOR_ELECTRIFY_AMERICA\x10\x01\x12\x19\n\x15\x43HARGING_VENDOR_BOSCH\x10\x03*`\n\x07\x45\x64ition\x12\x13\n\x0f\x45\x44ITION_UNKNOWN\x10\x00\x12\x17\n\x13\x45\x44ITION_PERFORMANCE\x10\x01\x12\x11\n\rEDITION_RANGE\x10\x02\x12\x14\n\x10\x45\x44ITION_STANDARD\x10\x03*\xe4\x01\n\x0b\x42\x61tteryType\x12\x18\n\x14\x42\x41TTERY_TYPE_UNKNOWN\x10\x00\x12\x13\n\x0f\x42\x41TTERY_TYPE_01\x10\x01\x12\x13\n\x0f\x42\x41TTERY_TYPE_02\x10\x02\x12\x13\n\x0f\x42\x41TTERY_TYPE_03\x10\x03\x12\x13\n\x0f\x42\x41TTERY_TYPE_04\x10\x04\x12\x13\n\x0f\x42\x41TTERY_TYPE_05\x10\x05\x12\x13\n\x0f\x42\x41TTERY_TYPE_06\x10\x06\x12\x13\n\x0f\x42\x41TTERY_TYPE_07\x10\x07\x12\x13\n\x0f\x42\x41TTERY_TYPE_08\x10\x08\x12\x13\n\x0f\x42\x41TTERY_TYPE_09\x10\t*}\n\x08Interior\x12\x14\n\x10INTERIOR_UNKNOWN\x10\x00\x12\x17\n\x13INTERIOR_SANTA_CRUZ\x10\x01\x12\x12\n\x0eINTERIOR_TAHOE\x10\x02\x12\x13\n\x0fINTERIOR_MOJAVE\x10\x03\x12\x19\n\x15INTERIOR_SANTA_MONICA\x10\x05*M\n\tStrutType\x12\x16\n\x12STRUT_TYPE_UNKNOWN\x10\x00\x12\x12\n\x0eSTRUT_TYPE_GAS\x10\x01\x12\x14\n\x10STRUT_TYPE_POWER\x10\x02*R\n\x08RoofType\x12\x15\n\x11ROOF_TYPE_UNKNOWN\x10\x00\x12\x1a\n\x16ROOF_TYPE_GLASS_CANOPY\x10\x01\x12\x13\n\x0fROOF_TYPE_METAL\x10\x02*D\n\x0cWarningState\x12\x13\n\x0fWARNING_UNKNOWN\x10\x00\x12\x0f\n\x0bWARNING_OFF\x10\x01\x12\x0e\n\nWARNING_ON\x10\x02*\x80\x01\n\x13\x42\x61tteryPreconStatus\x12\x1a\n\x16\x42\x41TTERY_PRECON_UNKNOWN\x10\x00\x12\x16\n\x12\x42\x41TTERY_PRECON_OFF\x10\x01\x12\x15\n\x11\x42\x41TTERY_PRECON_ON\x10\x02\x12\x1e\n\x1a\x42\x41TTERY_PRECON_UNAVAILABLE\x10\x03*\x8e\x02\n\nPowerState\x12\x17\n\x13POWER_STATE_UNKNOWN\x10\x00\x12\x15\n\x11POWER_STATE_SLEEP\x10\x01\x12\x14\n\x10POWER_STATE_WINK\x10\x02\x12\x19\n\x15POWER_STATE_ACCESSORY\x10\x03\x12\x15\n\x11POWER_STATE_DRIVE\x10\x04\x12\x1b\n\x17POWER_STATE_LIVE_CHARGE\x10\x05\x12\x1c\n\x18POWER_STATE_SLEEP_CHARGE\x10\x06\x12\x1b\n\x17POWER_STATE_LIVE_UPDATE\x10\x07\x12\x17\n\x13POWER_STATE_CLOUD_2\x10\n\x12\x17\n\x13POWER_STATE_MONITOR\x10\x0b*S\n\tLockState\x12\x16\n\x12LOCK_STATE_UNKNOWN\x10\x00\x12\x17\n\x13LOCK_STATE_UNLOCKED\x10\x01\x12\x15\n\x11LOCK_STATE_LOCKED\x10\x02*d\n\tDoorState\x12\x16\n\x12\x44OOR_STATE_UNKNOWN\x10\x00\x12\x13\n\x0f\x44OOR_STATE_OPEN\x10\x01\x12\x15\n\x11\x44OOR_STATE_CLOSED\x10\x02\x12\x13\n\x0f\x44OOR_STATE_AJAR\x10\x03*P\n\rWalkawayState\x12\x14\n\x10WALKAWAY_UNKNOWN\x10\x00\x12\x13\n\x0fWALKAWAY_ACTIVE\x10\x02\x12\x14\n\x10WALKAWAY_DISABLE\x10\x03*b\n\rAccessRequest\x12\x1a\n\x16\x41\x43\x43\x45SS_REQUEST_UNKNOWN\x10\x00\x12\x19\n\x15\x41\x43\x43\x45SS_REQUEST_ACTIVE\x10\x01\x12\x1a\n\x16\x41\x43\x43\x45SS_REQUEST_PASSIVE\x10\x02*n\n\nLightState\x12\x1e\n\x1aLIGHT_STATE_REALLY_UNKNOWN\x10\x00\x12\x13\n\x0fLIGHT_STATE_OFF\x10\x01\x12\x12\n\x0eLIGHT_STATE_ON\x10\x02\x12\x17\n\x13LIGHT_STATE_UNKNOWN\x10\x03*j\n\x0bLightAction\x12\x18\n\x14LIGHT_ACTION_UNKNOWN\x10\x00\x12\x16\n\x12LIGHT_ACTION_FLASH\x10\x01\x12\x13\n\x0fLIGHT_ACTION_ON\x10\x02\x12\x14\n\x10LIGHT_ACTION_OFF\x10\x03*\xc4\x01\n\x0b\x43hargeState\x12\x18\n\x14\x43HARGE_STATE_UNKNOWN\x10\x00\x12\x1e\n\x1a\x43HARGE_STATE_NOT_CONNECTED\x10\x01\x12 \n\x1c\x43HARGE_STATE_CABLE_CONNECTED\x10\x02\x12\x19\n\x15\x43HARGE_STATE_CHARGING\x10\x08\x12 \n\x1c\x43HARGE_STATE_CHARGING_END_OK\x10\t\x12\x1c\n\x18\x43HARGE_STATE_DISCHARGING\x10\x13*\xb9\x01\n\x14ScheduledChargeState\x12\"\n\x1eSCHEDULED_CHARGE_STATE_UNKNOWN\x10\x00\x12\x1f\n\x1bSCHEDULED_CHARGE_STATE_IDLE\x10\x01\x12.\n*SCHEDULED_CHARGE_STATE_SCHEDULED_TO_CHARGE\x10\x02\x12,\n(SCHEDULED_CHARGE_STATE_REQUEST_TO_CHARGE\x10\x03*x\n\x1fScheduledChargeUnavailableState\x12(\n$SCHEDULED_CHARGE_UNAVAILABLE_UNKNOWN\x10\x00\x12+\n\'SCHEDULED_CHARGE_UNAVAILABLE_NO_REQUEST\x10\x01*b\n\nEnergyType\x12\x17\n\x13\x45NERGY_TYPE_UNKNOWN\x10\x00\x12\x12\n\x0e\x45NERGY_TYPE_AC\x10\x01\x12\x12\n\x0e\x45NERGY_TYPE_DC\x10\x02\x12\x13\n\x0f\x45NERGY_TYPE_V2V\x10\x04*\xbb\x01\n\x0bUpdateState\x12\x18\n\x14UPDATE_STATE_UNKNOWN\x10\x00\x12\x1c\n\x18UPDATE_STATE_IN_PROGRESS\x10\x01\x12\x18\n\x14UPDATE_STATE_SUCCESS\x10\x02\x12\x17\n\x13UPDATE_STATE_FAILED\x10\x03\x12\x1f\n\x1bUPDATE_FAILED_DRIVE_ALLOWED\x10\x05\x12 \n\x1cUPDATE_SUCCESS_WITH_WARNINGS\x10\x07*K\n\x12UpdateAvailability\x12\x1f\n\x1bUPDATE_AVAILABILITY_UNKNOWN\x10\x00\x12\x14\n\x10UPDATE_AVAILABLE\x10\x01*Z\n\x0b\x41larmStatus\x12\x18\n\x14\x41LARM_STATUS_UNKNOWN\x10\x00\x12\x19\n\x15\x41LARM_STATUS_DISARMED\x10\x01\x12\x16\n\x12\x41LARM_STATUS_ARMED\x10\x02*a\n\tAlarmMode\x12\x16\n\x12\x41LARM_MODE_UNKNOWN\x10\x00\x12\x12\n\x0e\x41LARM_MODE_OFF\x10\x01\x12\x11\n\rALARM_MODE_ON\x10\x02\x12\x15\n\x11\x41LARM_MODE_SILENT\x10\x03*w\n\x14\x43loudConnectionState\x12\x1c\n\x18\x43LOUD_CONNECTION_UNKNOWN\x10\x00\x12\x1e\n\x1a\x43LOUD_CONNECTION_CONNECTED\x10\x01\x12!\n\x1d\x43LOUD_CONNECTION_DISCONNECTED\x10\x02*c\n\x13KeylessDrivingState\x12\x1b\n\x17KEYLESS_DRIVING_UNKNOWN\x10\x00\x12\x16\n\x12KEYLESS_DRIVING_ON\x10\x01\x12\x17\n\x13KEYLESS_DRIVING_OFF\x10\x02*i\n\tHvacPower\x12\x16\n\x12HVAC_POWER_UNKNOWN\x10\x00\x12\x0b\n\x07HVAC_ON\x10\x01\x12\x0c\n\x08HVAC_OFF\x10\x02\x12\x15\n\x11HVAC_PRECONDITION\x10\x03\x12\x12\n\x0eHVAC_KEEP_TEMP\x10\x06*J\n\x0c\x44\x65\x66rostState\x12\x19\n\x15\x44\x45\x46ROST_STATE_UNKNOWN\x10\x00\x12\x0e\n\nDEFROST_ON\x10\x01\x12\x0f\n\x0b\x44\x45\x46ROST_OFF\x10\x02*\x92\x01\n\x16HvacPreconditionStatus\x12$\n HVAC_PRECONDITION_STATUS_UNKNOWN\x10\x00\x12)\n%HVAC_PRECONDITION_STATUS_STILL_ACTIVE\x10\x01\x12\'\n#HVAC_PRECONDITION_STATUS_USER_INPUT\x10\x04*\xbe\x01\n\x11KeepClimateStatus\x12\x1f\n\x1bKEEP_CLIMATE_STATUS_UNKNOWN\x10\x00\x12 \n\x1cKEEP_CLIMATE_STATUS_INACTIVE\x10\x01\x12\x1f\n\x1bKEEP_CLIMATE_STATUS_ENABLED\x10\x02\x12 \n\x1cKEEP_CLIMATE_STATUS_CANCELED\x10\x03\x12#\n\x1fKEEP_CLIMATE_STATUS_PET_MODE_ON\x10\x04*:\n\x14KeepClimateCondition\x12\"\n\x1eKEEP_CLIMATE_CONDITION_UNKNOWN\x10\x00*\x84\x01\n\tDriveMode\x12\x16\n\x12\x44RIVE_MODE_UNKNOWN\x10\x00\x12\x16\n\x12\x44RIVE_MODE_COMFORT\x10\x01\x12\x14\n\x10\x44RIVE_MODE_SWIFT\x10\x02\x12\x19\n\x15\x44RIVE_MODE_SPORT_PLUS\x10\x05\x12\x16\n\x12\x44RIVE_MODE_SERVICE\x10\x08*v\n\x0bPrivacyMode\x12\x18\n\x14PRIVACY_MODE_UNKNOWN\x10\x00\x12%\n!PRIVACY_MODE_CONNECTIVITY_ENABLED\x10\x01\x12&\n\"PRIVACY_MODE_CONNECTIVITY_DISABLED\x10\x02*c\n\x0cGearPosition\x12\x10\n\x0cGEAR_UNKNOWN\x10\x00\x12\r\n\tGEAR_PARK\x10\x01\x12\x10\n\x0cGEAR_REVERSE\x10\x02\x12\x10\n\x0cGEAR_NEUTRAL\x10\x03\x12\x0e\n\nGEAR_DRIVE\x10\x04*E\n\x0fSharedTripState\x12\x17\n\x13SHARED_TRIP_UNKNOWN\x10\x00\x12\x19\n\x15SHARED_TRIP_AVAILABLE\x10\x01*9\n\nPanicState\x12\x17\n\x13PANIC_ALARM_UNKNOWN\x10\x00\x12\x12\n\x0ePANIC_ALARM_ON\x10\x01*Y\n\x08TcuState\x12\x0f\n\x0bTCU_UNKNOWN\x10\x00\x12\r\n\tTCU_SLEEP\x10\x01\x12\x0e\n\nTCU_DROWSY\x10\x02\x12\x0c\n\x08TCU_FULL\x10\x04\x12\x0f\n\x0bTCU_FACTORY\x10\x05*A\n\x07LteType\x12\x14\n\x10LTE_TYPE_UNKNOWN\x10\x00\x12\x0f\n\x0bLTE_TYPE_3G\x10\x01\x12\x0f\n\x0bLTE_TYPE_4G\x10\x02*`\n\x0eInternetStatus\x12\x1b\n\x17INTERNET_STATUS_UNKNOWN\x10\x00\x12\x19\n\x15INTERNET_DISCONNECTED\x10\x01\x12\x16\n\x12INTERNET_CONNECTED\x10\x02*Z\n\x0c\x43hargeAction\x12\x19\n\x15\x43HARGE_ACTION_UNKNOWN\x10\x00\x12\x17\n\x13\x43HARGE_ACTION_START\x10\x01\x12\x16\n\x12\x43HARGE_ACTION_STOP\x10\x02*\x95\x01\n\x0c\x44ocumentType\x12\x19\n\x15\x44OCUMENT_TYPE_UNKNOWN\x10\x00\x12#\n\x1f\x44OCUMENT_TYPE_RELEASE_NOTES_PRE\x10\x01\x12$\n DOCUMENT_TYPE_RELEASE_NOTES_POST\x10\x02\x12\x1f\n\x1b\x44OCUMENT_TYPE_OWNERS_MANUAL\x10\x03\x32\xe0\x0e\n\x13VehicleStateService\x12|\n\x13\x41pplySoftwareUpdate\x12\x30.mobilegateway.protos.ApplySoftwareUpdateRequest\x1a\x31.mobilegateway.protos.ApplySoftwareUpdateResponse\"\x00\x12\x82\x01\n\x15\x43\x61ncelScheduledUpdate\x12\x32.mobilegateway.protos.CancelScheduledUpdateRequest\x1a\x33.mobilegateway.protos.CancelScheduledUpdateResponse\"\x00\x12j\n\rChargeControl\x12*.mobilegateway.protos.ChargeControlRequest\x1a+.mobilegateway.protos.ChargeControlResponse\"\x00\x12v\n\x11\x43ontrolChargePort\x12..mobilegateway.protos.ControlChargePortRequest\x1a/.mobilegateway.protos.ControlChargePortResponse\"\x00\x12s\n\x10\x44oorLocksControl\x12-.mobilegateway.protos.DoorLocksControlRequest\x1a..mobilegateway.protos.DoorLocksControlResponse\"\x00\x12v\n\x11\x46rontCargoControl\x12..mobilegateway.protos.FrontCargoControlRequest\x1a/.mobilegateway.protos.FrontCargoControlResponse\"\x00\x12p\n\x0fGetDocumentInfo\x12,.mobilegateway.protos.GetDocumentInfoRequest\x1a-.mobilegateway.protos.GetDocumentInfoResponse\"\x00\x12p\n\x0fGetVehicleState\x12,.mobilegateway.protos.GetVehicleStateRequest\x1a-.mobilegateway.protos.GetVehicleStateResponse\"\x00\x12[\n\x08HonkHorn\x12%.mobilegateway.protos.HonkHornRequest\x1a&.mobilegateway.protos.HonkHornResponse\"\x00\x12y\n\x12HvacDefrostControl\x12/.mobilegateway.protos.HvacDefrostControlRequest\x1a\x30.mobilegateway.protos.HvacDefrostControlResponse\"\x00\x12j\n\rLightsControl\x12*.mobilegateway.protos.LightsControlRequest\x1a+.mobilegateway.protos.LightsControlResponse\"\x00\x12s\n\x10RearCargoControl\x12-.mobilegateway.protos.RearCargoControlRequest\x1a..mobilegateway.protos.RearCargoControlResponse\"\x00\x12\x7f\n\x14SecurityAlarmControl\x12\x31.mobilegateway.protos.SecurityAlarmControlRequest\x1a\x32.mobilegateway.protos.SecurityAlarmControlResponse\"\x00\x12|\n\x13SetCabinTemperature\x12\x30.mobilegateway.protos.SetCabinTemperatureRequest\x1a\x31.mobilegateway.protos.SetCabinTemperatureResponse\"\x00\x12m\n\x0eSetChargeLimit\x12+.mobilegateway.protos.SetChargeLimitRequest\x1a,.mobilegateway.protos.SetChargeLimitResponse\"\x00\x12j\n\rWakeupVehicle\x12*.mobilegateway.protos.WakeupVehicleRequest\x1a+.mobilegateway.protos.WakeupVehicleResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'vehicle_state_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
-  _globals['_ACCESSLEVEL']._serialized_start=8822
-  _globals['_ACCESSLEVEL']._serialized_end=8929
-  _globals['_MODEL']._serialized_start=8931
-  _globals['_MODEL']._serialized_end=8991
-  _globals['_MODELVARIANT']._serialized_start=8994
-  _globals['_MODELVARIANT']._serialized_end=9152
-  _globals['_PAINTCOLOR']._serialized_start=9155
-  _globals['_PAINTCOLOR']._serialized_end=9402
-  _globals['_LOOK']._serialized_start=9404
-  _globals['_LOOK']._serialized_end=9465
-  _globals['_WHEELS']._serialized_start=9467
-  _globals['_WHEELS']._serialized_end=9591
-  _globals['_SUBSCRIPTIONSTATUS']._serialized_start=9593
-  _globals['_SUBSCRIPTIONSTATUS']._serialized_end=9679
-  _globals['_CHARGINGACCOUNTSTATUS']._serialized_start=9681
-  _globals['_CHARGINGACCOUNTSTATUS']._serialized_end=9779
-  _globals['_CHARGINGVENDOR']._serialized_start=9781
-  _globals['_CHARGINGVENDOR']._serialized_end=9865
-  _globals['_EDITION']._serialized_start=9867
-  _globals['_EDITION']._serialized_end=9963
-  _globals['_BATTERYTYPE']._serialized_start=9966
-  _globals['_BATTERYTYPE']._serialized_end=10194
-  _globals['_INTERIOR']._serialized_start=10196
-  _globals['_INTERIOR']._serialized_end=10321
-  _globals['_STRUTTYPE']._serialized_start=10323
-  _globals['_STRUTTYPE']._serialized_end=10400
-  _globals['_ROOFTYPE']._serialized_start=10402
-  _globals['_ROOFTYPE']._serialized_end=10484
-  _globals['_WARNINGSTATE']._serialized_start=10486
-  _globals['_WARNINGSTATE']._serialized_end=10554
-  _globals['_BATTERYPRECONSTATUS']._serialized_start=10557
-  _globals['_BATTERYPRECONSTATUS']._serialized_end=10685
-  _globals['_POWERSTATE']._serialized_start=10688
-  _globals['_POWERSTATE']._serialized_end=10958
-  _globals['_LOCKSTATE']._serialized_start=10960
-  _globals['_LOCKSTATE']._serialized_end=11043
-  _globals['_DOORSTATE']._serialized_start=11045
-  _globals['_DOORSTATE']._serialized_end=11145
-  _globals['_WALKAWAYSTATE']._serialized_start=11147
-  _globals['_WALKAWAYSTATE']._serialized_end=11227
-  _globals['_ACCESSREQUEST']._serialized_start=11229
-  _globals['_ACCESSREQUEST']._serialized_end=11327
-  _globals['_LIGHTSTATE']._serialized_start=11329
-  _globals['_LIGHTSTATE']._serialized_end=11439
-  _globals['_LIGHTACTION']._serialized_start=11441
-  _globals['_LIGHTACTION']._serialized_end=11547
-  _globals['_CHARGESTATE']._serialized_start=11550
-  _globals['_CHARGESTATE']._serialized_end=11746
-  _globals['_SCHEDULEDCHARGESTATE']._serialized_start=11749
-  _globals['_SCHEDULEDCHARGESTATE']._serialized_end=11934
-  _globals['_SCHEDULEDCHARGEUNAVAILABLESTATE']._serialized_start=11936
-  _globals['_SCHEDULEDCHARGEUNAVAILABLESTATE']._serialized_end=12056
-  _globals['_ENERGYTYPE']._serialized_start=12058
-  _globals['_ENERGYTYPE']._serialized_end=12156
-  _globals['_UPDATESTATE']._serialized_start=12159
-  _globals['_UPDATESTATE']._serialized_end=12346
-  _globals['_UPDATEAVAILABILITY']._serialized_start=12348
-  _globals['_UPDATEAVAILABILITY']._serialized_end=12423
-  _globals['_ALARMSTATUS']._serialized_start=12425
-  _globals['_ALARMSTATUS']._serialized_end=12515
-  _globals['_ALARMMODE']._serialized_start=12517
-  _globals['_ALARMMODE']._serialized_end=12614
-  _globals['_CLOUDCONNECTIONSTATE']._serialized_start=12616
-  _globals['_CLOUDCONNECTIONSTATE']._serialized_end=12735
-  _globals['_KEYLESSDRIVINGSTATE']._serialized_start=12737
-  _globals['_KEYLESSDRIVINGSTATE']._serialized_end=12836
-  _globals['_HVACPOWER']._serialized_start=12838
-  _globals['_HVACPOWER']._serialized_end=12923
-  _globals['_DEFROSTSTATE']._serialized_start=12925
-  _globals['_DEFROSTSTATE']._serialized_end=12999
-  _globals['_HVACPRECONDITIONSTATUS']._serialized_start=13002
-  _globals['_HVACPRECONDITIONSTATUS']._serialized_end=13148
-  _globals['_DRIVEMODE']._serialized_start=13150
-  _globals['_DRIVEMODE']._serialized_end=13258
-  _globals['_PRIVACYMODE']._serialized_start=13260
-  _globals['_PRIVACYMODE']._serialized_end=13378
-  _globals['_GEARPOSITION']._serialized_start=13380
-  _globals['_GEARPOSITION']._serialized_end=13479
-  _globals['_SHAREDTRIPSTATE']._serialized_start=13481
-  _globals['_SHAREDTRIPSTATE']._serialized_end=13550
-  _globals['_TCUSTATE']._serialized_start=13552
-  _globals['_TCUSTATE']._serialized_end=13641
-  _globals['_LTETYPE']._serialized_start=13643
-  _globals['_LTETYPE']._serialized_end=13708
-  _globals['_INTERNETSTATUS']._serialized_start=13710
-  _globals['_INTERNETSTATUS']._serialized_end=13806
-  _globals['_CHARGEACTION']._serialized_start=13808
-  _globals['_CHARGEACTION']._serialized_end=13898
-  _globals['_DOCUMENTTYPE']._serialized_start=13901
-  _globals['_DOCUMENTTYPE']._serialized_end=14050
+  _globals['_ACCESSLEVEL']._serialized_start=9009
+  _globals['_ACCESSLEVEL']._serialized_end=9116
+  _globals['_MODEL']._serialized_start=9118
+  _globals['_MODEL']._serialized_end=9178
+  _globals['_MODELVARIANT']._serialized_start=9181
+  _globals['_MODELVARIANT']._serialized_end=9339
+  _globals['_PAINTCOLOR']._serialized_start=9342
+  _globals['_PAINTCOLOR']._serialized_end=9589
+  _globals['_LOOK']._serialized_start=9591
+  _globals['_LOOK']._serialized_end=9652
+  _globals['_WHEELS']._serialized_start=9654
+  _globals['_WHEELS']._serialized_end=9778
+  _globals['_SUBSCRIPTIONSTATUS']._serialized_start=9780
+  _globals['_SUBSCRIPTIONSTATUS']._serialized_end=9866
+  _globals['_CHARGINGACCOUNTSTATUS']._serialized_start=9868
+  _globals['_CHARGINGACCOUNTSTATUS']._serialized_end=9966
+  _globals['_CHARGINGVENDOR']._serialized_start=9968
+  _globals['_CHARGINGVENDOR']._serialized_end=10079
+  _globals['_EDITION']._serialized_start=10081
+  _globals['_EDITION']._serialized_end=10177
+  _globals['_BATTERYTYPE']._serialized_start=10180
+  _globals['_BATTERYTYPE']._serialized_end=10408
+  _globals['_INTERIOR']._serialized_start=10410
+  _globals['_INTERIOR']._serialized_end=10535
+  _globals['_STRUTTYPE']._serialized_start=10537
+  _globals['_STRUTTYPE']._serialized_end=10614
+  _globals['_ROOFTYPE']._serialized_start=10616
+  _globals['_ROOFTYPE']._serialized_end=10698
+  _globals['_WARNINGSTATE']._serialized_start=10700
+  _globals['_WARNINGSTATE']._serialized_end=10768
+  _globals['_BATTERYPRECONSTATUS']._serialized_start=10771
+  _globals['_BATTERYPRECONSTATUS']._serialized_end=10899
+  _globals['_POWERSTATE']._serialized_start=10902
+  _globals['_POWERSTATE']._serialized_end=11172
+  _globals['_LOCKSTATE']._serialized_start=11174
+  _globals['_LOCKSTATE']._serialized_end=11257
+  _globals['_DOORSTATE']._serialized_start=11259
+  _globals['_DOORSTATE']._serialized_end=11359
+  _globals['_WALKAWAYSTATE']._serialized_start=11361
+  _globals['_WALKAWAYSTATE']._serialized_end=11441
+  _globals['_ACCESSREQUEST']._serialized_start=11443
+  _globals['_ACCESSREQUEST']._serialized_end=11541
+  _globals['_LIGHTSTATE']._serialized_start=11543
+  _globals['_LIGHTSTATE']._serialized_end=11653
+  _globals['_LIGHTACTION']._serialized_start=11655
+  _globals['_LIGHTACTION']._serialized_end=11761
+  _globals['_CHARGESTATE']._serialized_start=11764
+  _globals['_CHARGESTATE']._serialized_end=11960
+  _globals['_SCHEDULEDCHARGESTATE']._serialized_start=11963
+  _globals['_SCHEDULEDCHARGESTATE']._serialized_end=12148
+  _globals['_SCHEDULEDCHARGEUNAVAILABLESTATE']._serialized_start=12150
+  _globals['_SCHEDULEDCHARGEUNAVAILABLESTATE']._serialized_end=12270
+  _globals['_ENERGYTYPE']._serialized_start=12272
+  _globals['_ENERGYTYPE']._serialized_end=12370
+  _globals['_UPDATESTATE']._serialized_start=12373
+  _globals['_UPDATESTATE']._serialized_end=12560
+  _globals['_UPDATEAVAILABILITY']._serialized_start=12562
+  _globals['_UPDATEAVAILABILITY']._serialized_end=12637
+  _globals['_ALARMSTATUS']._serialized_start=12639
+  _globals['_ALARMSTATUS']._serialized_end=12729
+  _globals['_ALARMMODE']._serialized_start=12731
+  _globals['_ALARMMODE']._serialized_end=12828
+  _globals['_CLOUDCONNECTIONSTATE']._serialized_start=12830
+  _globals['_CLOUDCONNECTIONSTATE']._serialized_end=12949
+  _globals['_KEYLESSDRIVINGSTATE']._serialized_start=12951
+  _globals['_KEYLESSDRIVINGSTATE']._serialized_end=13050
+  _globals['_HVACPOWER']._serialized_start=13052
+  _globals['_HVACPOWER']._serialized_end=13157
+  _globals['_DEFROSTSTATE']._serialized_start=13159
+  _globals['_DEFROSTSTATE']._serialized_end=13233
+  _globals['_HVACPRECONDITIONSTATUS']._serialized_start=13236
+  _globals['_HVACPRECONDITIONSTATUS']._serialized_end=13382
+  _globals['_KEEPCLIMATESTATUS']._serialized_start=13385
+  _globals['_KEEPCLIMATESTATUS']._serialized_end=13575
+  _globals['_KEEPCLIMATECONDITION']._serialized_start=13577
+  _globals['_KEEPCLIMATECONDITION']._serialized_end=13635
+  _globals['_DRIVEMODE']._serialized_start=13638
+  _globals['_DRIVEMODE']._serialized_end=13770
+  _globals['_PRIVACYMODE']._serialized_start=13772
+  _globals['_PRIVACYMODE']._serialized_end=13890
+  _globals['_GEARPOSITION']._serialized_start=13892
+  _globals['_GEARPOSITION']._serialized_end=13991
+  _globals['_SHAREDTRIPSTATE']._serialized_start=13993
+  _globals['_SHAREDTRIPSTATE']._serialized_end=14062
+  _globals['_PANICSTATE']._serialized_start=14064
+  _globals['_PANICSTATE']._serialized_end=14121
+  _globals['_TCUSTATE']._serialized_start=14123
+  _globals['_TCUSTATE']._serialized_end=14212
+  _globals['_LTETYPE']._serialized_start=14214
+  _globals['_LTETYPE']._serialized_end=14279
+  _globals['_INTERNETSTATUS']._serialized_start=14281
+  _globals['_INTERNETSTATUS']._serialized_end=14377
+  _globals['_CHARGEACTION']._serialized_start=14379
+  _globals['_CHARGEACTION']._serialized_end=14469
+  _globals['_DOCUMENTTYPE']._serialized_start=14472
+  _globals['_DOCUMENTTYPE']._serialized_end=14621
   _globals['_CHARGINGSUBSCRIPTION']._serialized_start=54
   _globals['_CHARGINGSUBSCRIPTION']._serialized_end=193
   _globals['_CHARGINGACCOUNT']._serialized_start=196
   _globals['_CHARGINGACCOUNT']._serialized_end=428
   _globals['_SPECIALIDENTIFIERS']._serialized_start=430
   _globals['_SPECIALIDENTIFIERS']._serialized_end=470
   _globals['_RESERVATION']._serialized_start=472
@@ -136,87 +142,87 @@
   _globals['_GPS']._serialized_start=3969
   _globals['_GPS']._serialized_end=4091
   _globals['_SOFTWAREUPDATE']._serialized_start=4094
   _globals['_SOFTWAREUPDATE']._serialized_end=4380
   _globals['_ALARMSTATE']._serialized_start=4382
   _globals['_ALARMSTATE']._serialized_end=4492
   _globals['_HVACSTATE']._serialized_start=4495
-  _globals['_HVACSTATE']._serialized_end=4682
-  _globals['_MOBILEAPPREQSTATE']._serialized_start=4685
-  _globals['_MOBILEAPPREQSTATE']._serialized_end=5199
-  _globals['_TCUINTERNETSTATE']._serialized_start=5202
-  _globals['_TCUINTERNETSTATE']._serialized_end=5460
-  _globals['_VEHICLESTATE']._serialized_start=5463
-  _globals['_VEHICLESTATE']._serialized_end=6490
-  _globals['_VEHICLE']._serialized_start=6493
-  _globals['_VEHICLE']._serialized_end=6683
-  _globals['_APPLYSOFTWAREUPDATEREQUEST']._serialized_start=6685
-  _globals['_APPLYSOFTWAREUPDATEREQUEST']._serialized_end=6733
-  _globals['_APPLYSOFTWAREUPDATERESPONSE']._serialized_start=6735
-  _globals['_APPLYSOFTWAREUPDATERESPONSE']._serialized_end=6764
-  _globals['_CANCELSCHEDULEDUPDATEREQUEST']._serialized_start=6766
-  _globals['_CANCELSCHEDULEDUPDATEREQUEST']._serialized_end=6816
-  _globals['_CANCELSCHEDULEDUPDATERESPONSE']._serialized_start=6818
-  _globals['_CANCELSCHEDULEDUPDATERESPONSE']._serialized_end=6849
-  _globals['_CHARGECONTROLREQUEST']._serialized_start=6851
-  _globals['_CHARGECONTROLREQUEST']._serialized_end=6945
-  _globals['_CHARGECONTROLRESPONSE']._serialized_start=6947
-  _globals['_CHARGECONTROLRESPONSE']._serialized_end=6970
-  _globals['_CONTROLCHARGEPORTREQUEST']._serialized_start=6972
-  _globals['_CONTROLCHARGEPORTREQUEST']._serialized_end=7074
-  _globals['_CONTROLCHARGEPORTRESPONSE']._serialized_start=7076
-  _globals['_CONTROLCHARGEPORTRESPONSE']._serialized_end=7103
-  _globals['_DOORLOCKSCONTROLREQUEST']._serialized_start=7105
-  _globals['_DOORLOCKSCONTROLREQUEST']._serialized_end=7226
-  _globals['_DOORLOCKSCONTROLRESPONSE']._serialized_start=7228
-  _globals['_DOORLOCKSCONTROLRESPONSE']._serialized_end=7254
-  _globals['_FRONTCARGOCONTROLREQUEST']._serialized_start=7256
-  _globals['_FRONTCARGOCONTROLREQUEST']._serialized_end=7358
-  _globals['_FRONTCARGOCONTROLRESPONSE']._serialized_start=7360
-  _globals['_FRONTCARGOCONTROLRESPONSE']._serialized_end=7387
-  _globals['_DOCUMENTINFOUNKNOWN']._serialized_start=7389
-  _globals['_DOCUMENTINFOUNKNOWN']._serialized_end=7429
-  _globals['_DOCUMENTINFO']._serialized_start=7432
-  _globals['_DOCUMENTINFO']._serialized_end=7594
-  _globals['_GETDOCUMENTINFOREQUEST']._serialized_start=7596
-  _globals['_GETDOCUMENTINFOREQUEST']._serialized_end=7696
-  _globals['_GETDOCUMENTINFORESPONSE']._serialized_start=7698
-  _globals['_GETDOCUMENTINFORESPONSE']._serialized_end=7786
-  _globals['_GETVEHICLESTATEREQUEST']._serialized_start=7788
-  _globals['_GETVEHICLESTATEREQUEST']._serialized_end=7832
-  _globals['_GETVEHICLESTATERESPONSE']._serialized_start=7834
-  _globals['_GETVEHICLESTATERESPONSE']._serialized_end=7930
-  _globals['_HONKHORNREQUEST']._serialized_start=7932
-  _globals['_HONKHORNREQUEST']._serialized_end=7969
-  _globals['_HONKHORNRESPONSE']._serialized_start=7971
-  _globals['_HONKHORNRESPONSE']._serialized_end=7989
-  _globals['_HVACDEFROSTCONTROLREQUEST']._serialized_start=7991
-  _globals['_HVACDEFROSTCONTROLREQUEST']._serialized_end=8096
-  _globals['_HVACDEFROSTCONTROLRESPONSE']._serialized_start=8098
-  _globals['_HVACDEFROSTCONTROLRESPONSE']._serialized_end=8126
-  _globals['_LIGHTSCONTROLREQUEST']._serialized_start=8128
-  _globals['_LIGHTSCONTROLREQUEST']._serialized_end=8221
-  _globals['_LIGHTSCONTROLRESPONSE']._serialized_start=8223
-  _globals['_LIGHTSCONTROLRESPONSE']._serialized_end=8246
-  _globals['_REARCARGOCONTROLREQUEST']._serialized_start=8248
-  _globals['_REARCARGOCONTROLREQUEST']._serialized_end=8349
-  _globals['_REARCARGOCONTROLRESPONSE']._serialized_start=8351
-  _globals['_REARCARGOCONTROLRESPONSE']._serialized_end=8377
-  _globals['_SECURITYALARMCONTROLREQUEST']._serialized_start=8379
-  _globals['_SECURITYALARMCONTROLREQUEST']._serialized_end=8475
-  _globals['_SECURITYALARMCONTROLRESPONSE']._serialized_start=8477
-  _globals['_SECURITYALARMCONTROLRESPONSE']._serialized_end=8507
-  _globals['_SETCABINTEMPERATUREREQUEST']._serialized_start=8509
-  _globals['_SETCABINTEMPERATUREREQUEST']._serialized_end=8626
-  _globals['_SETCABINTEMPERATURERESPONSE']._serialized_start=8628
-  _globals['_SETCABINTEMPERATURERESPONSE']._serialized_end=8657
-  _globals['_SETCHARGELIMITREQUEST']._serialized_start=8659
-  _globals['_SETCHARGELIMITREQUEST']._serialized_end=8725
-  _globals['_SETCHARGELIMITRESPONSE']._serialized_start=8727
-  _globals['_SETCHARGELIMITRESPONSE']._serialized_end=8751
-  _globals['_WAKEUPVEHICLEREQUEST']._serialized_start=8753
-  _globals['_WAKEUPVEHICLEREQUEST']._serialized_end=8795
-  _globals['_WAKEUPVEHICLERESPONSE']._serialized_start=8797
-  _globals['_WAKEUPVEHICLERESPONSE']._serialized_end=8820
-  _globals['_VEHICLESTATESERVICE']._serialized_start=14053
-  _globals['_VEHICLESTATESERVICE']._serialized_end=15941
+  _globals['_HVACSTATE']._serialized_end=4752
+  _globals['_MOBILEAPPREQSTATE']._serialized_start=4755
+  _globals['_MOBILEAPPREQSTATE']._serialized_end=5386
+  _globals['_TCUINTERNETSTATE']._serialized_start=5389
+  _globals['_TCUINTERNETSTATE']._serialized_end=5647
+  _globals['_VEHICLESTATE']._serialized_start=5650
+  _globals['_VEHICLESTATE']._serialized_end=6677
+  _globals['_VEHICLE']._serialized_start=6680
+  _globals['_VEHICLE']._serialized_end=6870
+  _globals['_APPLYSOFTWAREUPDATEREQUEST']._serialized_start=6872
+  _globals['_APPLYSOFTWAREUPDATEREQUEST']._serialized_end=6920
+  _globals['_APPLYSOFTWAREUPDATERESPONSE']._serialized_start=6922
+  _globals['_APPLYSOFTWAREUPDATERESPONSE']._serialized_end=6951
+  _globals['_CANCELSCHEDULEDUPDATEREQUEST']._serialized_start=6953
+  _globals['_CANCELSCHEDULEDUPDATEREQUEST']._serialized_end=7003
+  _globals['_CANCELSCHEDULEDUPDATERESPONSE']._serialized_start=7005
+  _globals['_CANCELSCHEDULEDUPDATERESPONSE']._serialized_end=7036
+  _globals['_CHARGECONTROLREQUEST']._serialized_start=7038
+  _globals['_CHARGECONTROLREQUEST']._serialized_end=7132
+  _globals['_CHARGECONTROLRESPONSE']._serialized_start=7134
+  _globals['_CHARGECONTROLRESPONSE']._serialized_end=7157
+  _globals['_CONTROLCHARGEPORTREQUEST']._serialized_start=7159
+  _globals['_CONTROLCHARGEPORTREQUEST']._serialized_end=7261
+  _globals['_CONTROLCHARGEPORTRESPONSE']._serialized_start=7263
+  _globals['_CONTROLCHARGEPORTRESPONSE']._serialized_end=7290
+  _globals['_DOORLOCKSCONTROLREQUEST']._serialized_start=7292
+  _globals['_DOORLOCKSCONTROLREQUEST']._serialized_end=7413
+  _globals['_DOORLOCKSCONTROLRESPONSE']._serialized_start=7415
+  _globals['_DOORLOCKSCONTROLRESPONSE']._serialized_end=7441
+  _globals['_FRONTCARGOCONTROLREQUEST']._serialized_start=7443
+  _globals['_FRONTCARGOCONTROLREQUEST']._serialized_end=7545
+  _globals['_FRONTCARGOCONTROLRESPONSE']._serialized_start=7547
+  _globals['_FRONTCARGOCONTROLRESPONSE']._serialized_end=7574
+  _globals['_DOCUMENTINFOUNKNOWN']._serialized_start=7576
+  _globals['_DOCUMENTINFOUNKNOWN']._serialized_end=7616
+  _globals['_DOCUMENTINFO']._serialized_start=7619
+  _globals['_DOCUMENTINFO']._serialized_end=7781
+  _globals['_GETDOCUMENTINFOREQUEST']._serialized_start=7783
+  _globals['_GETDOCUMENTINFOREQUEST']._serialized_end=7883
+  _globals['_GETDOCUMENTINFORESPONSE']._serialized_start=7885
+  _globals['_GETDOCUMENTINFORESPONSE']._serialized_end=7973
+  _globals['_GETVEHICLESTATEREQUEST']._serialized_start=7975
+  _globals['_GETVEHICLESTATEREQUEST']._serialized_end=8019
+  _globals['_GETVEHICLESTATERESPONSE']._serialized_start=8021
+  _globals['_GETVEHICLESTATERESPONSE']._serialized_end=8117
+  _globals['_HONKHORNREQUEST']._serialized_start=8119
+  _globals['_HONKHORNREQUEST']._serialized_end=8156
+  _globals['_HONKHORNRESPONSE']._serialized_start=8158
+  _globals['_HONKHORNRESPONSE']._serialized_end=8176
+  _globals['_HVACDEFROSTCONTROLREQUEST']._serialized_start=8178
+  _globals['_HVACDEFROSTCONTROLREQUEST']._serialized_end=8283
+  _globals['_HVACDEFROSTCONTROLRESPONSE']._serialized_start=8285
+  _globals['_HVACDEFROSTCONTROLRESPONSE']._serialized_end=8313
+  _globals['_LIGHTSCONTROLREQUEST']._serialized_start=8315
+  _globals['_LIGHTSCONTROLREQUEST']._serialized_end=8408
+  _globals['_LIGHTSCONTROLRESPONSE']._serialized_start=8410
+  _globals['_LIGHTSCONTROLRESPONSE']._serialized_end=8433
+  _globals['_REARCARGOCONTROLREQUEST']._serialized_start=8435
+  _globals['_REARCARGOCONTROLREQUEST']._serialized_end=8536
+  _globals['_REARCARGOCONTROLRESPONSE']._serialized_start=8538
+  _globals['_REARCARGOCONTROLRESPONSE']._serialized_end=8564
+  _globals['_SECURITYALARMCONTROLREQUEST']._serialized_start=8566
+  _globals['_SECURITYALARMCONTROLREQUEST']._serialized_end=8662
+  _globals['_SECURITYALARMCONTROLRESPONSE']._serialized_start=8664
+  _globals['_SECURITYALARMCONTROLRESPONSE']._serialized_end=8694
+  _globals['_SETCABINTEMPERATUREREQUEST']._serialized_start=8696
+  _globals['_SETCABINTEMPERATUREREQUEST']._serialized_end=8813
+  _globals['_SETCABINTEMPERATURERESPONSE']._serialized_start=8815
+  _globals['_SETCABINTEMPERATURERESPONSE']._serialized_end=8844
+  _globals['_SETCHARGELIMITREQUEST']._serialized_start=8846
+  _globals['_SETCHARGELIMITREQUEST']._serialized_end=8912
+  _globals['_SETCHARGELIMITRESPONSE']._serialized_start=8914
+  _globals['_SETCHARGELIMITRESPONSE']._serialized_end=8938
+  _globals['_WAKEUPVEHICLEREQUEST']._serialized_start=8940
+  _globals['_WAKEUPVEHICLEREQUEST']._serialized_end=8982
+  _globals['_WAKEUPVEHICLERESPONSE']._serialized_start=8984
+  _globals['_WAKEUPVEHICLERESPONSE']._serialized_end=9007
+  _globals['_VEHICLESTATESERVICE']._serialized_start=14624
+  _globals['_VEHICLESTATESERVICE']._serialized_end=16512
 # @@protoc_insertion_point(module_scope)
```

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/vehicle_state_service_pb2.pyi` & `lucidmotors-1.1.2/lucidmotors/gen/vehicle_state_service_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     CHARGING_ACCOUNT_STATUS_UNKNOWN: _ClassVar[ChargingAccountStatus]
     CHARGING_ACCOUNT_STATUS_ENROLLED: _ClassVar[ChargingAccountStatus]
 
 class ChargingVendor(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     CHARGING_VENDOR_UNKNOWN: _ClassVar[ChargingVendor]
     CHARGING_VENDOR_ELECTRIFY_AMERICA: _ClassVar[ChargingVendor]
+    CHARGING_VENDOR_BOSCH: _ClassVar[ChargingVendor]
 
 class Edition(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     EDITION_UNKNOWN: _ClassVar[Edition]
     EDITION_PERFORMANCE: _ClassVar[Edition]
     EDITION_RANGE: _ClassVar[Edition]
     EDITION_STANDARD: _ClassVar[Edition]
@@ -241,33 +242,47 @@
 
 class HvacPower(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     HVAC_POWER_UNKNOWN: _ClassVar[HvacPower]
     HVAC_ON: _ClassVar[HvacPower]
     HVAC_OFF: _ClassVar[HvacPower]
     HVAC_PRECONDITION: _ClassVar[HvacPower]
+    HVAC_KEEP_TEMP: _ClassVar[HvacPower]
 
 class DefrostState(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     DEFROST_STATE_UNKNOWN: _ClassVar[DefrostState]
     DEFROST_ON: _ClassVar[DefrostState]
     DEFROST_OFF: _ClassVar[DefrostState]
 
 class HvacPreconditionStatus(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     HVAC_PRECONDITION_STATUS_UNKNOWN: _ClassVar[HvacPreconditionStatus]
     HVAC_PRECONDITION_STATUS_STILL_ACTIVE: _ClassVar[HvacPreconditionStatus]
     HVAC_PRECONDITION_STATUS_USER_INPUT: _ClassVar[HvacPreconditionStatus]
 
+class KeepClimateStatus(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = ()
+    KEEP_CLIMATE_STATUS_UNKNOWN: _ClassVar[KeepClimateStatus]
+    KEEP_CLIMATE_STATUS_INACTIVE: _ClassVar[KeepClimateStatus]
+    KEEP_CLIMATE_STATUS_ENABLED: _ClassVar[KeepClimateStatus]
+    KEEP_CLIMATE_STATUS_CANCELED: _ClassVar[KeepClimateStatus]
+    KEEP_CLIMATE_STATUS_PET_MODE_ON: _ClassVar[KeepClimateStatus]
+
+class KeepClimateCondition(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = ()
+    KEEP_CLIMATE_CONDITION_UNKNOWN: _ClassVar[KeepClimateCondition]
+
 class DriveMode(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     DRIVE_MODE_UNKNOWN: _ClassVar[DriveMode]
     DRIVE_MODE_COMFORT: _ClassVar[DriveMode]
     DRIVE_MODE_SWIFT: _ClassVar[DriveMode]
     DRIVE_MODE_SPORT_PLUS: _ClassVar[DriveMode]
+    DRIVE_MODE_SERVICE: _ClassVar[DriveMode]
 
 class PrivacyMode(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     PRIVACY_MODE_UNKNOWN: _ClassVar[PrivacyMode]
     PRIVACY_MODE_CONNECTIVITY_ENABLED: _ClassVar[PrivacyMode]
     PRIVACY_MODE_CONNECTIVITY_DISABLED: _ClassVar[PrivacyMode]
 
@@ -280,14 +295,19 @@
     GEAR_DRIVE: _ClassVar[GearPosition]
 
 class SharedTripState(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     SHARED_TRIP_UNKNOWN: _ClassVar[SharedTripState]
     SHARED_TRIP_AVAILABLE: _ClassVar[SharedTripState]
 
+class PanicState(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = ()
+    PANIC_ALARM_UNKNOWN: _ClassVar[PanicState]
+    PANIC_ALARM_ON: _ClassVar[PanicState]
+
 class TcuState(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     TCU_UNKNOWN: _ClassVar[TcuState]
     TCU_SLEEP: _ClassVar[TcuState]
     TCU_DROWSY: _ClassVar[TcuState]
     TCU_FULL: _ClassVar[TcuState]
     TCU_FACTORY: _ClassVar[TcuState]
@@ -346,14 +366,15 @@
 WHEELS_LITE_STEALTH: Wheels
 SUBSCRIPTION_STATUS_UNKNOWN: SubscriptionStatus
 SUBSCRIPTION_STATUS_CURRENT: SubscriptionStatus
 CHARGING_ACCOUNT_STATUS_UNKNOWN: ChargingAccountStatus
 CHARGING_ACCOUNT_STATUS_ENROLLED: ChargingAccountStatus
 CHARGING_VENDOR_UNKNOWN: ChargingVendor
 CHARGING_VENDOR_ELECTRIFY_AMERICA: ChargingVendor
+CHARGING_VENDOR_BOSCH: ChargingVendor
 EDITION_UNKNOWN: Edition
 EDITION_PERFORMANCE: Edition
 EDITION_RANGE: Edition
 EDITION_STANDARD: Edition
 BATTERY_TYPE_UNKNOWN: BatteryType
 BATTERY_TYPE_01: BatteryType
 BATTERY_TYPE_02: BatteryType
@@ -450,34 +471,44 @@
 KEYLESS_DRIVING_UNKNOWN: KeylessDrivingState
 KEYLESS_DRIVING_ON: KeylessDrivingState
 KEYLESS_DRIVING_OFF: KeylessDrivingState
 HVAC_POWER_UNKNOWN: HvacPower
 HVAC_ON: HvacPower
 HVAC_OFF: HvacPower
 HVAC_PRECONDITION: HvacPower
+HVAC_KEEP_TEMP: HvacPower
 DEFROST_STATE_UNKNOWN: DefrostState
 DEFROST_ON: DefrostState
 DEFROST_OFF: DefrostState
 HVAC_PRECONDITION_STATUS_UNKNOWN: HvacPreconditionStatus
 HVAC_PRECONDITION_STATUS_STILL_ACTIVE: HvacPreconditionStatus
 HVAC_PRECONDITION_STATUS_USER_INPUT: HvacPreconditionStatus
+KEEP_CLIMATE_STATUS_UNKNOWN: KeepClimateStatus
+KEEP_CLIMATE_STATUS_INACTIVE: KeepClimateStatus
+KEEP_CLIMATE_STATUS_ENABLED: KeepClimateStatus
+KEEP_CLIMATE_STATUS_CANCELED: KeepClimateStatus
+KEEP_CLIMATE_STATUS_PET_MODE_ON: KeepClimateStatus
+KEEP_CLIMATE_CONDITION_UNKNOWN: KeepClimateCondition
 DRIVE_MODE_UNKNOWN: DriveMode
 DRIVE_MODE_COMFORT: DriveMode
 DRIVE_MODE_SWIFT: DriveMode
 DRIVE_MODE_SPORT_PLUS: DriveMode
+DRIVE_MODE_SERVICE: DriveMode
 PRIVACY_MODE_UNKNOWN: PrivacyMode
 PRIVACY_MODE_CONNECTIVITY_ENABLED: PrivacyMode
 PRIVACY_MODE_CONNECTIVITY_DISABLED: PrivacyMode
 GEAR_UNKNOWN: GearPosition
 GEAR_PARK: GearPosition
 GEAR_REVERSE: GearPosition
 GEAR_NEUTRAL: GearPosition
 GEAR_DRIVE: GearPosition
 SHARED_TRIP_UNKNOWN: SharedTripState
 SHARED_TRIP_AVAILABLE: SharedTripState
+PANIC_ALARM_UNKNOWN: PanicState
+PANIC_ALARM_ON: PanicState
 TCU_UNKNOWN: TcuState
 TCU_SLEEP: TcuState
 TCU_DROWSY: TcuState
 TCU_FULL: TcuState
 TCU_FACTORY: TcuState
 LTE_TYPE_UNKNOWN: LteType
 LTE_TYPE_3G: LteType
@@ -744,42 +775,48 @@
     STATUS_FIELD_NUMBER: _ClassVar[int]
     MODE_FIELD_NUMBER: _ClassVar[int]
     status: AlarmStatus
     mode: AlarmMode
     def __init__(self, status: _Optional[_Union[AlarmStatus, str]] = ..., mode: _Optional[_Union[AlarmMode, str]] = ...) -> None: ...
 
 class HvacState(_message.Message):
-    __slots__ = ("power", "defrost", "precondition_status")
+    __slots__ = ("power", "defrost", "precondition_status", "keep_climate_status")
     POWER_FIELD_NUMBER: _ClassVar[int]
     DEFROST_FIELD_NUMBER: _ClassVar[int]
     PRECONDITION_STATUS_FIELD_NUMBER: _ClassVar[int]
+    KEEP_CLIMATE_STATUS_FIELD_NUMBER: _ClassVar[int]
     power: HvacPower
     defrost: DefrostState
     precondition_status: HvacPreconditionStatus
-    def __init__(self, power: _Optional[_Union[HvacPower, str]] = ..., defrost: _Optional[_Union[DefrostState, str]] = ..., precondition_status: _Optional[_Union[HvacPreconditionStatus, str]] = ...) -> None: ...
+    keep_climate_status: KeepClimateStatus
+    def __init__(self, power: _Optional[_Union[HvacPower, str]] = ..., defrost: _Optional[_Union[DefrostState, str]] = ..., precondition_status: _Optional[_Union[HvacPreconditionStatus, str]] = ..., keep_climate_status: _Optional[_Union[KeepClimateStatus, str]] = ...) -> None: ...
 
 class MobileAppReqState(_message.Message):
-    __slots__ = ("charge_port_request", "frunk_cargo_request", "hvac_defrost", "hvac_precondition", "light_request", "shared_trip_request", "trunk_cargo_request", "vehicle_unlock_request")
+    __slots__ = ("alarm_set_request", "charge_port_request", "frunk_cargo_request", "hvac_defrost", "hvac_precondition", "light_request", "panic_request", "shared_trip_request", "trunk_cargo_request", "vehicle_unlock_request")
+    ALARM_SET_REQUEST_FIELD_NUMBER: _ClassVar[int]
     CHARGE_PORT_REQUEST_FIELD_NUMBER: _ClassVar[int]
     FRUNK_CARGO_REQUEST_FIELD_NUMBER: _ClassVar[int]
     HVAC_DEFROST_FIELD_NUMBER: _ClassVar[int]
     HVAC_PRECONDITION_FIELD_NUMBER: _ClassVar[int]
     LIGHT_REQUEST_FIELD_NUMBER: _ClassVar[int]
+    PANIC_REQUEST_FIELD_NUMBER: _ClassVar[int]
     SHARED_TRIP_REQUEST_FIELD_NUMBER: _ClassVar[int]
     TRUNK_CARGO_REQUEST_FIELD_NUMBER: _ClassVar[int]
     VEHICLE_UNLOCK_REQUEST_FIELD_NUMBER: _ClassVar[int]
+    alarm_set_request: AlarmMode
     charge_port_request: DoorState
     frunk_cargo_request: DoorState
     hvac_defrost: DefrostState
     hvac_precondition: HvacPower
     light_request: LightAction
+    panic_request: PanicState
     shared_trip_request: SharedTripState
     trunk_cargo_request: DoorState
     vehicle_unlock_request: LockState
-    def __init__(self, charge_port_request: _Optional[_Union[DoorState, str]] = ..., frunk_cargo_request: _Optional[_Union[DoorState, str]] = ..., hvac_defrost: _Optional[_Union[DefrostState, str]] = ..., hvac_precondition: _Optional[_Union[HvacPower, str]] = ..., light_request: _Optional[_Union[LightAction, str]] = ..., shared_trip_request: _Optional[_Union[SharedTripState, str]] = ..., trunk_cargo_request: _Optional[_Union[DoorState, str]] = ..., vehicle_unlock_request: _Optional[_Union[LockState, str]] = ...) -> None: ...
+    def __init__(self, alarm_set_request: _Optional[_Union[AlarmMode, str]] = ..., charge_port_request: _Optional[_Union[DoorState, str]] = ..., frunk_cargo_request: _Optional[_Union[DoorState, str]] = ..., hvac_defrost: _Optional[_Union[DefrostState, str]] = ..., hvac_precondition: _Optional[_Union[HvacPower, str]] = ..., light_request: _Optional[_Union[LightAction, str]] = ..., panic_request: _Optional[_Union[PanicState, str]] = ..., shared_trip_request: _Optional[_Union[SharedTripState, str]] = ..., trunk_cargo_request: _Optional[_Union[DoorState, str]] = ..., vehicle_unlock_request: _Optional[_Union[LockState, str]] = ...) -> None: ...
 
 class TcuInternetState(_message.Message):
     __slots__ = ("lte_type", "lte_status", "wifi_status", "lte_rssi", "wifi_rssi")
     LTE_TYPE_FIELD_NUMBER: _ClassVar[int]
     LTE_STATUS_FIELD_NUMBER: _ClassVar[int]
     WIFI_STATUS_FIELD_NUMBER: _ClassVar[int]
     LTE_RSSI_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/vehicle_state_service_pb2.pyi.orig` & `lucidmotors-1.1.2/lucidmotors/gen/vehicle_state_service_pb2.pyi.orig`

 * *Files 7% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     CHARGING_ACCOUNT_STATUS_UNKNOWN: _ClassVar[ChargingAccountStatus]
     CHARGING_ACCOUNT_STATUS_ENROLLED: _ClassVar[ChargingAccountStatus]
 
 class ChargingVendor(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     CHARGING_VENDOR_UNKNOWN: _ClassVar[ChargingVendor]
     CHARGING_VENDOR_ELECTRIFY_AMERICA: _ClassVar[ChargingVendor]
+    CHARGING_VENDOR_BOSCH: _ClassVar[ChargingVendor]
 
 class Edition(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     EDITION_UNKNOWN: _ClassVar[Edition]
     EDITION_PERFORMANCE: _ClassVar[Edition]
     EDITION_RANGE: _ClassVar[Edition]
     EDITION_STANDARD: _ClassVar[Edition]
@@ -241,33 +242,47 @@
 
 class HvacPower(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     HVAC_POWER_UNKNOWN: _ClassVar[HvacPower]
     HVAC_ON: _ClassVar[HvacPower]
     HVAC_OFF: _ClassVar[HvacPower]
     HVAC_PRECONDITION: _ClassVar[HvacPower]
+    HVAC_KEEP_TEMP: _ClassVar[HvacPower]
 
 class DefrostState(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     DEFROST_STATE_UNKNOWN: _ClassVar[DefrostState]
     DEFROST_ON: _ClassVar[DefrostState]
     DEFROST_OFF: _ClassVar[DefrostState]
 
 class HvacPreconditionStatus(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     HVAC_PRECONDITION_STATUS_UNKNOWN: _ClassVar[HvacPreconditionStatus]
     HVAC_PRECONDITION_STATUS_STILL_ACTIVE: _ClassVar[HvacPreconditionStatus]
     HVAC_PRECONDITION_STATUS_USER_INPUT: _ClassVar[HvacPreconditionStatus]
 
+class KeepClimateStatus(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = ()
+    KEEP_CLIMATE_STATUS_UNKNOWN: _ClassVar[KeepClimateStatus]
+    KEEP_CLIMATE_STATUS_INACTIVE: _ClassVar[KeepClimateStatus]
+    KEEP_CLIMATE_STATUS_ENABLED: _ClassVar[KeepClimateStatus]
+    KEEP_CLIMATE_STATUS_CANCELED: _ClassVar[KeepClimateStatus]
+    KEEP_CLIMATE_STATUS_PET_MODE_ON: _ClassVar[KeepClimateStatus]
+
+class KeepClimateCondition(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = ()
+    KEEP_CLIMATE_CONDITION_UNKNOWN: _ClassVar[KeepClimateCondition]
+
 class DriveMode(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     DRIVE_MODE_UNKNOWN: _ClassVar[DriveMode]
     DRIVE_MODE_COMFORT: _ClassVar[DriveMode]
     DRIVE_MODE_SWIFT: _ClassVar[DriveMode]
     DRIVE_MODE_SPORT_PLUS: _ClassVar[DriveMode]
+    DRIVE_MODE_SERVICE: _ClassVar[DriveMode]
 
 class PrivacyMode(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     PRIVACY_MODE_UNKNOWN: _ClassVar[PrivacyMode]
     PRIVACY_MODE_CONNECTIVITY_ENABLED: _ClassVar[PrivacyMode]
     PRIVACY_MODE_CONNECTIVITY_DISABLED: _ClassVar[PrivacyMode]
 
@@ -280,14 +295,19 @@
     GEAR_DRIVE: _ClassVar[GearPosition]
 
 class SharedTripState(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     SHARED_TRIP_UNKNOWN: _ClassVar[SharedTripState]
     SHARED_TRIP_AVAILABLE: _ClassVar[SharedTripState]
 
+class PanicState(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = ()
+    PANIC_ALARM_UNKNOWN: _ClassVar[PanicState]
+    PANIC_ALARM_ON: _ClassVar[PanicState]
+
 class TcuState(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     TCU_UNKNOWN: _ClassVar[TcuState]
     TCU_SLEEP: _ClassVar[TcuState]
     TCU_DROWSY: _ClassVar[TcuState]
     TCU_FULL: _ClassVar[TcuState]
     TCU_FACTORY: _ClassVar[TcuState]
@@ -346,14 +366,15 @@
 WHEELS_LITE_STEALTH: Wheels
 SUBSCRIPTION_STATUS_UNKNOWN: SubscriptionStatus
 SUBSCRIPTION_STATUS_CURRENT: SubscriptionStatus
 CHARGING_ACCOUNT_STATUS_UNKNOWN: ChargingAccountStatus
 CHARGING_ACCOUNT_STATUS_ENROLLED: ChargingAccountStatus
 CHARGING_VENDOR_UNKNOWN: ChargingVendor
 CHARGING_VENDOR_ELECTRIFY_AMERICA: ChargingVendor
+CHARGING_VENDOR_BOSCH: ChargingVendor
 EDITION_UNKNOWN: Edition
 EDITION_PERFORMANCE: Edition
 EDITION_RANGE: Edition
 EDITION_STANDARD: Edition
 BATTERY_TYPE_UNKNOWN: BatteryType
 BATTERY_TYPE_01: BatteryType
 BATTERY_TYPE_02: BatteryType
@@ -450,34 +471,44 @@
 KEYLESS_DRIVING_UNKNOWN: KeylessDrivingState
 KEYLESS_DRIVING_ON: KeylessDrivingState
 KEYLESS_DRIVING_OFF: KeylessDrivingState
 HVAC_POWER_UNKNOWN: HvacPower
 HVAC_ON: HvacPower
 HVAC_OFF: HvacPower
 HVAC_PRECONDITION: HvacPower
+HVAC_KEEP_TEMP: HvacPower
 DEFROST_STATE_UNKNOWN: DefrostState
 DEFROST_ON: DefrostState
 DEFROST_OFF: DefrostState
 HVAC_PRECONDITION_STATUS_UNKNOWN: HvacPreconditionStatus
 HVAC_PRECONDITION_STATUS_STILL_ACTIVE: HvacPreconditionStatus
 HVAC_PRECONDITION_STATUS_USER_INPUT: HvacPreconditionStatus
+KEEP_CLIMATE_STATUS_UNKNOWN: KeepClimateStatus
+KEEP_CLIMATE_STATUS_INACTIVE: KeepClimateStatus
+KEEP_CLIMATE_STATUS_ENABLED: KeepClimateStatus
+KEEP_CLIMATE_STATUS_CANCELED: KeepClimateStatus
+KEEP_CLIMATE_STATUS_PET_MODE_ON: KeepClimateStatus
+KEEP_CLIMATE_CONDITION_UNKNOWN: KeepClimateCondition
 DRIVE_MODE_UNKNOWN: DriveMode
 DRIVE_MODE_COMFORT: DriveMode
 DRIVE_MODE_SWIFT: DriveMode
 DRIVE_MODE_SPORT_PLUS: DriveMode
+DRIVE_MODE_SERVICE: DriveMode
 PRIVACY_MODE_UNKNOWN: PrivacyMode
 PRIVACY_MODE_CONNECTIVITY_ENABLED: PrivacyMode
 PRIVACY_MODE_CONNECTIVITY_DISABLED: PrivacyMode
 GEAR_UNKNOWN: GearPosition
 GEAR_PARK: GearPosition
 GEAR_REVERSE: GearPosition
 GEAR_NEUTRAL: GearPosition
 GEAR_DRIVE: GearPosition
 SHARED_TRIP_UNKNOWN: SharedTripState
 SHARED_TRIP_AVAILABLE: SharedTripState
+PANIC_ALARM_UNKNOWN: PanicState
+PANIC_ALARM_ON: PanicState
 TCU_UNKNOWN: TcuState
 TCU_SLEEP: TcuState
 TCU_DROWSY: TcuState
 TCU_FULL: TcuState
 TCU_FACTORY: TcuState
 LTE_TYPE_UNKNOWN: LteType
 LTE_TYPE_3G: LteType
@@ -744,42 +775,48 @@
     STATUS_FIELD_NUMBER: _ClassVar[int]
     MODE_FIELD_NUMBER: _ClassVar[int]
     status: AlarmStatus
     mode: AlarmMode
     def __init__(self, status: _Optional[_Union[AlarmStatus, str]] = ..., mode: _Optional[_Union[AlarmMode, str]] = ...) -> None: ...
 
 class HvacState(_message.Message):
-    __slots__ = ("power", "defrost", "precondition_status")
+    __slots__ = ("power", "defrost", "precondition_status", "keep_climate_status")
     POWER_FIELD_NUMBER: _ClassVar[int]
     DEFROST_FIELD_NUMBER: _ClassVar[int]
     PRECONDITION_STATUS_FIELD_NUMBER: _ClassVar[int]
+    KEEP_CLIMATE_STATUS_FIELD_NUMBER: _ClassVar[int]
     power: HvacPower
     defrost: DefrostState
     precondition_status: HvacPreconditionStatus
-    def __init__(self, power: _Optional[_Union[HvacPower, str]] = ..., defrost: _Optional[_Union[DefrostState, str]] = ..., precondition_status: _Optional[_Union[HvacPreconditionStatus, str]] = ...) -> None: ...
+    keep_climate_status: KeepClimateStatus
+    def __init__(self, power: _Optional[_Union[HvacPower, str]] = ..., defrost: _Optional[_Union[DefrostState, str]] = ..., precondition_status: _Optional[_Union[HvacPreconditionStatus, str]] = ..., keep_climate_status: _Optional[_Union[KeepClimateStatus, str]] = ...) -> None: ...
 
 class MobileAppReqState(_message.Message):
-    __slots__ = ("charge_port_request", "frunk_cargo_request", "hvac_defrost", "hvac_precondition", "light_request", "shared_trip_request", "trunk_cargo_request", "vehicle_unlock_request")
+    __slots__ = ("alarm_set_request", "charge_port_request", "frunk_cargo_request", "hvac_defrost", "hvac_precondition", "light_request", "panic_request", "shared_trip_request", "trunk_cargo_request", "vehicle_unlock_request")
+    ALARM_SET_REQUEST_FIELD_NUMBER: _ClassVar[int]
     CHARGE_PORT_REQUEST_FIELD_NUMBER: _ClassVar[int]
     FRUNK_CARGO_REQUEST_FIELD_NUMBER: _ClassVar[int]
     HVAC_DEFROST_FIELD_NUMBER: _ClassVar[int]
     HVAC_PRECONDITION_FIELD_NUMBER: _ClassVar[int]
     LIGHT_REQUEST_FIELD_NUMBER: _ClassVar[int]
+    PANIC_REQUEST_FIELD_NUMBER: _ClassVar[int]
     SHARED_TRIP_REQUEST_FIELD_NUMBER: _ClassVar[int]
     TRUNK_CARGO_REQUEST_FIELD_NUMBER: _ClassVar[int]
     VEHICLE_UNLOCK_REQUEST_FIELD_NUMBER: _ClassVar[int]
+    alarm_set_request: AlarmMode
     charge_port_request: DoorState
     frunk_cargo_request: DoorState
     hvac_defrost: DefrostState
     hvac_precondition: HvacPower
     light_request: LightAction
+    panic_request: PanicState
     shared_trip_request: SharedTripState
     trunk_cargo_request: DoorState
     vehicle_unlock_request: LockState
-    def __init__(self, charge_port_request: _Optional[_Union[DoorState, str]] = ..., frunk_cargo_request: _Optional[_Union[DoorState, str]] = ..., hvac_defrost: _Optional[_Union[DefrostState, str]] = ..., hvac_precondition: _Optional[_Union[HvacPower, str]] = ..., light_request: _Optional[_Union[LightAction, str]] = ..., shared_trip_request: _Optional[_Union[SharedTripState, str]] = ..., trunk_cargo_request: _Optional[_Union[DoorState, str]] = ..., vehicle_unlock_request: _Optional[_Union[LockState, str]] = ...) -> None: ...
+    def __init__(self, alarm_set_request: _Optional[_Union[AlarmMode, str]] = ..., charge_port_request: _Optional[_Union[DoorState, str]] = ..., frunk_cargo_request: _Optional[_Union[DoorState, str]] = ..., hvac_defrost: _Optional[_Union[DefrostState, str]] = ..., hvac_precondition: _Optional[_Union[HvacPower, str]] = ..., light_request: _Optional[_Union[LightAction, str]] = ..., panic_request: _Optional[_Union[PanicState, str]] = ..., shared_trip_request: _Optional[_Union[SharedTripState, str]] = ..., trunk_cargo_request: _Optional[_Union[DoorState, str]] = ..., vehicle_unlock_request: _Optional[_Union[LockState, str]] = ...) -> None: ...
 
 class TcuInternetState(_message.Message):
     __slots__ = ("lte_type", "lte_status", "wifi_status", "lte_rssi", "wifi_rssi")
     LTE_TYPE_FIELD_NUMBER: _ClassVar[int]
     LTE_STATUS_FIELD_NUMBER: _ClassVar[int]
     WIFI_STATUS_FIELD_NUMBER: _ClassVar[int]
     LTE_RSSI_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/vehicle_state_service_pb2_grpc.py` & `lucidmotors-1.1.2/lucidmotors/gen/vehicle_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lucidmotors-1.1.1/lucidmotors/gen/vehicle_state_service_pb2_grpc.py.orig` & `lucidmotors-1.1.2/lucidmotors/gen/vehicle_state_service_pb2_grpc.py.orig`

 * *Files identical despite different names*

### Comparing `lucidmotors-1.1.1/pyproject.toml` & `lucidmotors-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lucidmotors"
-version = "1.1.1"
+version = "1.1.2"
 description = ""
 authors = ["Nick Shipp <git@segbrk.com>", "Michael Borohovski <borski@owlpost.lol>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = "^3.8.5"
```

### Comparing `lucidmotors-1.1.1/PKG-INFO` & `lucidmotors-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lucidmotors
-Version: 1.1.1
+Version: 1.1.2
 Summary: 
 Author: Nick Shipp
 Author-email: git@segbrk.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


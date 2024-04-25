# Comparing `tmp/pybrams-0.0.8.tar.gz` & `tmp/pybrams-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybrams-0.0.8.tar", last modified: Thu Nov  2 18:23:13 2023, max compression
+gzip compressed data, was "pybrams-0.0.9.tar", max compression
```

## Comparing `pybrams-0.0.8.tar` & `pybrams-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,18 @@
-drwxr-sr-x   0 antoinec  (1000) antoinec  (1000)        0 2023-11-02 18:23:13.947876 pybrams-0.0.8/
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)     1069 2023-10-05 12:35:27.000000 pybrams-0.0.8/LICENSE.txt
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)     2342 2023-11-02 18:23:13.947876 pybrams-0.0.8/PKG-INFO
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)     1728 2023-10-17 18:46:59.000000 pybrams-0.0.8/README.md
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)      737 2023-10-24 08:45:51.000000 pybrams-0.0.8/pyproject.toml
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)       38 2023-11-02 18:23:13.947876 pybrams-0.0.8/setup.cfg
-drwxr-sr-x   0 antoinec  (1000) antoinec  (1000)        0 2023-11-02 18:23:13.944876 pybrams-0.0.8/src/
-drwxr-sr-x   0 antoinec  (1000) antoinec  (1000)        0 2023-11-02 18:23:13.946876 pybrams-0.0.8/src/brams/
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)      358 2023-10-18 14:17:54.000000 pybrams-0.0.8/src/brams/__init__.py
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)      217 2023-10-24 09:01:27.000000 pybrams-0.0.8/src/brams/api.py
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)     2337 2023-10-27 14:29:44.000000 pybrams-0.0.8/src/brams/cache.py
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)     3694 2023-10-21 14:09:13.000000 pybrams-0.0.8/src/brams/coordinates.py
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)    11299 2023-11-02 18:14:47.000000 pybrams-0.0.8/src/brams/files.py
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)      840 2023-10-27 14:30:10.000000 pybrams-0.0.8/src/brams/http.py
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)      554 2023-10-26 11:13:08.000000 pybrams-0.0.8/src/brams/interval.py
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)     2728 2023-10-22 19:33:17.000000 pybrams-0.0.8/src/brams/locations.py
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)     1113 2023-10-21 15:11:21.000000 pybrams-0.0.8/src/brams/pps.py
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)    12754 2023-11-02 18:22:21.000000 pybrams-0.0.8/src/brams/signal.py
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)     4233 2023-10-26 23:19:11.000000 pybrams-0.0.8/src/brams/systems.py
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)      528 2023-10-12 10:45:52.000000 pybrams-0.0.8/src/brams/timestamps.py
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)     6047 2023-11-02 11:25:26.000000 pybrams-0.0.8/src/brams/wav.py
-drwxr-sr-x   0 antoinec  (1000) antoinec  (1000)        0 2023-11-02 18:23:13.946876 pybrams-0.0.8/src/pybrams.egg-info/
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)     2342 2023-11-02 18:23:13.000000 pybrams-0.0.8/src/pybrams.egg-info/PKG-INFO
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)      552 2023-11-02 18:23:13.000000 pybrams-0.0.8/src/pybrams.egg-info/SOURCES.txt
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)        1 2023-11-02 18:23:13.000000 pybrams-0.0.8/src/pybrams.egg-info/dependency_links.txt
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)       41 2023-11-02 18:23:13.000000 pybrams-0.0.8/src/pybrams.egg-info/requires.txt
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)       11 2023-11-02 18:23:13.000000 pybrams-0.0.8/src/pybrams.egg-info/top_level.txt
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)     4007 2023-11-02 11:22:43.000000 pybrams-0.0.8/src/test.py
-drwxr-sr-x   0 antoinec  (1000) antoinec  (1000)        0 2023-11-02 18:23:13.947876 pybrams-0.0.8/tests/
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)     3121 2023-10-30 13:21:04.000000 pybrams-0.0.8/tests/test_files.py
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)     1257 2023-10-21 13:16:43.000000 pybrams-0.0.8/tests/test_locations.py
--rw-r--r--   0 antoinec  (1000) antoinec  (1000)     1903 2023-10-23 13:21:04.000000 pybrams-0.0.8/tests/test_systems.py
+-rw-r--r--   0        0        0     1069 2023-10-05 12:35:27.666981 pybrams-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0     1728 2023-10-17 18:46:59.755455 pybrams-0.0.9/README.md
+-rw-r--r--   0        0        0      685 2023-11-08 15:23:25.111325 pybrams-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      555 2023-11-08 12:05:41.740623 pybrams-0.0.9/src/brams/__init__.py
+-rw-r--r--   0        0        0      230 2023-11-08 12:31:03.091251 pybrams-0.0.9/src/brams/api.py
+-rw-r--r--   0        0        0       48 2023-11-08 12:06:55.343084 pybrams-0.0.9/src/brams/archive.py
+-rw-r--r--   0        0        0     2373 2023-11-08 12:32:27.393793 pybrams-0.0.9/src/brams/cache.py
+-rw-r--r--   0        0        0     4572 2023-11-08 12:32:53.513961 pybrams-0.0.9/src/brams/coordinates.py
+-rw-r--r--   0        0        0    11354 2023-11-08 12:35:05.810812 pybrams-0.0.9/src/brams/files.py
+-rw-r--r--   0        0        0      840 2023-10-27 14:30:10.691479 pybrams-0.0.9/src/brams/http.py
+-rw-r--r--   0        0        0      554 2023-10-26 11:13:08.794666 pybrams-0.0.9/src/brams/interval.py
+-rw-r--r--   0        0        0     2741 2023-11-08 12:35:25.540938 pybrams-0.0.9/src/brams/locations.py
+-rw-r--r--   0        0        0     1113 2023-10-21 15:11:21.081538 pybrams-0.0.9/src/brams/pps.py
+-rw-r--r--   0        0        0    12754 2023-11-02 18:22:21.298646 pybrams-0.0.9/src/brams/signal.py
+-rw-r--r--   0        0        0     4239 2023-11-08 12:35:37.005012 pybrams-0.0.9/src/brams/systems.py
+-rw-r--r--   0        0        0      528 2023-10-12 10:45:52.425269 pybrams-0.0.9/src/brams/timestamps.py
+-rw-r--r--   0        0        0     6078 2023-11-08 12:35:57.863146 pybrams-0.0.9/src/brams/wav.py
+-rw-r--r--   0        0        0     2693 1970-01-01 00:00:00.000000 pybrams-0.0.9/PKG-INFO
```

### Comparing `pybrams-0.0.8/LICENSE.txt` & `pybrams-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pybrams-0.0.8/PKG-INFO` & `pybrams-0.0.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: pybrams
-Version: 0.0.8
-Summary: BRAMS
-Author-email: Antoine Calegaro <antoine.calegaro@aeronomie.be>, Joachim Balis <joachim.balis@aeronomie.be>
-Project-URL: Homepage, https://brams.aeronomie.be
-Project-URL: Git, https://gitlab.aeronomie.be/ae/brams/pybrams
-Keywords: brams,meteor
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: requests
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: json-fix
-Requires-Dist: matplotlib
-
 # pybrams
 
 **pybrams** is a Python package that allows you to access information and data from the BRAMS (Belgian RAdio Meteor Stations) project. BRAMS is a network of radio receiving stations that use forward scattering techniques to study the meteoroid population. This project, coordinated by the Belgian Institute for Space Aeronomy (BISA), provides a valuable source of data for researchers, amateur astronomers, and meteor enthusiasts.
 
 ## Features
 
 - Fetch detailed information about BRAMS stations, including their location, name, number of antennas, and more.
```

### Comparing `pybrams-0.0.8/pyproject.toml` & `pybrams-0.0.9/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-[build-system]
-requires      = ["setuptools>=61.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[project]
+[tool.poetry]
 name = "pybrams"
-version = "0.0.8"
+version = "0.0.9"
 description = "BRAMS"
+authors = [
+    "Antoine Calegaro <antoine.calegaro@aeronomie.be>",
+    "Joachim Balis <joachim.balis@aeronomie.be>",
+]
+license = "MIT"
 readme = "README.md"
-authors = [{ name = "Antoine Calegaro", email = "antoine.calegaro@aeronomie.be" }, { name = "Joachim Balis", email = "joachim.balis@aeronomie.be" } ]
-license = { file = "LICENSE" }
+homepage = "https://brams.aeronomie.be"
+repository= "https://gitlab.aeronomie.be/ae/brams/pybrams"
+keywords = ["brams", "meteor"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
-keywords = ["brams", "meteor"]
-dependencies = [
-    "requests",
-    "numpy",
-    "scipy",
-	"json-fix",
-    "matplotlib"
+packages = [
+    { include = "brams", from = "src" },
 ]
-requires-python = ">=3.6"
 
-[project.urls]
-Homepage = "https://brams.aeronomie.be"
-Git = "https://gitlab.aeronomie.be/ae/brams/pybrams"
+[tool.poetry.dependencies]
+python = ">=3.6"
+requests = "*"
+numpy = "*"
+scipy = "*"
+json-fix = "*"
+matplotlib = "*"
+dataclasses = { version = "*", python = "3.6"}
+
```

### Comparing `pybrams-0.0.8/src/brams/cache.py` & `pybrams-0.0.9/src/brams/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import shutil
 import glob
-from typing import Any, List, Literal, Optional
+from typing import Any, List, Literal, Optional, Union
 
 class Cache:
 
     root = os.path.join(".", ".cache")
     use_cache = False
     data = {}
 
@@ -49,14 +49,16 @@
                     
                     cls.remove(file)     
                 
         else:
 
             shutil.rmtree(cls.root, ignore_errors=True)
 
+        cls.data = {}
+
     @classmethod
     def cache(cls, key: str, data: Any, json: bool = True) -> None:
 
         if cls.use_cache:
 
             if not os.path.exists(cls.root):
 
@@ -71,15 +73,15 @@
             
             if json:
 
                 cls.data[key] = data
 
 
     @classmethod
-    def get(cls, key: str, json: bool = True) -> Any | Literal[False]:
+    def get(cls, key: str, json: bool = True) -> Union[Any, Literal[False]]:
 
         if cls.use_cache:
 
             path = f"{key}.json" if json else key
             mode = "r" if json else "rb"
 
             if json and key in cls.data:
```

### Comparing `pybrams-0.0.8/src/brams/coordinates.py` & `pybrams-0.0.9/src/brams/coordinates.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from dataclasses import dataclass
 from math import cos, radians, sin, sqrt
-from typing import Any, Dict
+from typing import Any, Dict, Union
 import numpy as np
 import json_fix # type: ignore
 
 GRS80 = 6378.137, 298.257222100882711
 WGS84 = 6378.137, 298.257223563
 
 
@@ -24,14 +24,26 @@
 
         return GeodeticCoordinates(self.latitude + o.latitude, self.longitude + o.longitude, self.altitude + o.altitude)
 
     def __sub__(self, o: GeodeticCoordinates) -> GeodeticCoordinates:
 
         return GeodeticCoordinates(self.latitude - o.latitude, self.longitude - o.longitude, self.altitude - o.altitude)
 
+    def __eq__(self, other: object) -> bool:
+
+        if isinstance(other, GeodeticCoordinates):
+
+            return (
+                self.latitude == other.latitude and
+                self.longitude == other.longitude and
+                self.altitude == other.altitude
+            )
+
+        return False
+
 
 @dataclass
 class CartesianCoordinates:
 
     x: float
     y: float
     z: float
@@ -44,29 +56,53 @@
 
         return CartesianCoordinates(self.x + o.x, self.y + o.y, self.z + o.z)
 
     def __sub__(self, o: CartesianCoordinates) -> CartesianCoordinates:
 
         return CartesianCoordinates(self.x - o.x, self.y - o.y, self.z - o.z)
 
+    def __eq__(self, other: object) -> bool:
+
+        if isinstance(other, CartesianCoordinates):
+
+            return (
+                self.x == other.x and
+                self.y == other.y and
+                self.z == other.z
+            )
+
+        return False
+
 
 DOURBES_GEODETIC_COORDINATES = GeodeticCoordinates(50.097569, 4.588487, 0.167)
 
 
 @dataclass
 class Coordinates:
 
     geodetic: GeodeticCoordinates
     geocentric: CartesianCoordinates
     dourbocentric: CartesianCoordinates
 
-    def __json__(self) -> Dict[str, GeodeticCoordinates | CartesianCoordinates]:
+    def __json__(self) -> Dict[str, Union[GeodeticCoordinates, CartesianCoordinates]]:
 
         return self.__dict__
 
+    def __eq__(self, other: object) -> bool:
+
+        if isinstance(other, Coordinates):
+
+            return (
+                self.geodetic == other.geodetic and
+                self.geocentric == other.geocentric and
+                self.dourbocentric == other.dourbocentric
+            )
+
+        return False
+
     @staticmethod
     def geodetic2Geocentric(coordinates: GeodeticCoordinates) -> CartesianCoordinates:
 
         φ = radians(coordinates.latitude)
         λ = radians(coordinates.longitude)
         sin_φ = sin(φ)
         a, rf = WGS84           # semi-major axis, reciprocal flattening
@@ -111,14 +147,12 @@
         C3 = RotMatPhi @ C2
 
         return CartesianCoordinates(C3[1], C3[2], C3[0])
 
     @classmethod
     def fromGeodetic(cls, latitude: float, longitude: float, altitude: float) -> Coordinates:
 
-        geodeticCoordinates = GeodeticCoordinates(
-            latitude, longitude, altitude)
+        geodeticCoordinates = GeodeticCoordinates(latitude, longitude, altitude)
         geocentricCoordinates = cls.geodetic2Geocentric(geodeticCoordinates)
-        dourbocentricCoordinates = cls.geodetic2Dourbocentric(
-            geodeticCoordinates)
+        dourbocentricCoordinates = cls.geodetic2Dourbocentric(geodeticCoordinates)
 
         return cls(geodeticCoordinates, geocentricCoordinates, dourbocentricCoordinates)
```

### Comparing `pybrams-0.0.8/src/brams/files.py` & `pybrams-0.0.9/src/brams/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from __future__ import annotations
 from types import NoneType
-from typing import Any, Dict, Literal, Optional, Union, List
+from typing import Any, Dict, Optional, Union, List
 import json_fix # type: ignore
 import os
 import json
 from . import locations
 from . import systems
 from .wav import Wav
 from .signal import Signal
 from .pps import PPS
 from .api import request as api_request
 from .http import get as get_request
 from .cache import Cache
 from .interval import parse
 
+use_brams_archive = False
 api_endpoint = "file.php"
 
 class File:
 
     def __init__(self, year: int, month: int, day: int, hours: int, minutes: int, samplerate: float,
                  pps_count: int, duration: int, precise_start: int, precise_end: int, system_code: str,
                  location_code: str, location_url: str, system_url: str, wav_url: str, wav_name: str, png_url: str,
@@ -69,30 +70,32 @@
             "wav_url": self.wav_url,
             "wav_name": self.wav_name,
             "png_url": self.png_url,
             "png_name": self.png_name,
             "beacon_frequency": self.signal.beacon_frequency if self.signal else None
         }
     
-    def system(self) -> systems.System | None:
+    def system(self) -> Union[systems.System, None]:
 
         return systems.get(self.system_code) 
 
 
-    def location(self) -> locations.Location | None:
+    def location(self) -> Union[locations.Location, None]:
 
         return locations.get(self.location_code) 
 
 
     def load(self) -> None:
 
         wav_content = Cache.get(self.wav_name, False)
 
         if not wav_content:
 
+            
+
             while not wav_content or not len(wav_content):
 
                 response = get_request(self.wav_url)
                 wav_content = response.content
 
             Cache.cache(self.wav_name, wav_content, False)
 
@@ -140,15 +143,15 @@
 
 
     def json_string(self) -> str:
 
         return f"{self.system_code}.{str(self.year).zfill(4)}{str(self.month).zfill(2)}{str(self.day).zfill(2)}_{str(self.hours).zfill(2)}{str(self.minutes).zfill(2)}"
 
 
-    def __add__(self, other: File) -> File | None:
+    def __add__(self, other: File) -> Union[File, None]:
 
         # WIP
 
         if self.system_code == other.system_code and self.type == other.type:
 
             import numpy as np
 
@@ -188,15 +191,15 @@
                 self.type == other.type and
                 self.signal == other.signal
             )
 
         return False
 
 
-def get(interval: str, system: Union[str, systems.System, List[Union[str, systems.System]], Dict[str, systems.System], None] = None) -> Union[File, Dict[str, File], Dict[str, List[File]] | None]:
+def get(interval: str, system: Union[str, systems.System, List[Union[str, systems.System]], Dict[str, systems.System], None] = None) -> Union[File, Dict[str, File], Union[Dict[str, List[File]], None]]:
 
     def get_file(system_code, key: str):
 
         cached_file = Cache.get(key)
         
         if cached_file:
```

### Comparing `pybrams-0.0.8/src/brams/http.py` & `pybrams-0.0.9/src/brams/http.py`

 * *Files identical despite different names*

### Comparing `pybrams-0.0.8/src/brams/interval.py` & `pybrams-0.0.9/src/brams/interval.py`

 * *Files identical despite different names*

### Comparing `pybrams-0.0.8/src/brams/locations.py` & `pybrams-0.0.9/src/brams/locations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict
+from typing import Any, Dict, Union
 import json_fix # type: ignore
 from dataclasses import dataclass
 from .coordinates import Coordinates
 import json
 import datetime
 from .cache import Cache
 from .api import request as api_request
@@ -38,15 +38,15 @@
 
     def systems(self):
 
         from .systems import get as get_system
         return get_system(location=self)
         
 
-def get(location_code: str) -> Location | None:
+def get(location_code: str) -> Union[Location, None]:
 
     location = None
 
     for key in [location_code, "locations"]:
 
         json_location = Cache.get(key)
```

### Comparing `pybrams-0.0.8/src/brams/pps.py` & `pybrams-0.0.9/src/brams/pps.py`

 * *Files identical despite different names*

### Comparing `pybrams-0.0.8/src/brams/signal.py` & `pybrams-0.0.9/src/brams/signal.py`

 * *Files identical despite different names*

### Comparing `pybrams-0.0.8/src/brams/systems.py` & `pybrams-0.0.9/src/brams/systems.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             "start": self.start,
             "end": self.end,
             "antenna": self.antenna,
             "location_url": self.location_url,
             "location_code": self.location_code
         }
 
-    def location(self) -> Location | None:
+    def location(self) -> Union[Location, None]:
 
         from .locations import get as get_location
         return get_location(self.location_code) 
         
 
 def get(system_code: Optional[str] = None, location: Optional[Union[str, Location]] = None) -> Union[System, Dict[str, System], None]:
```

### Comparing `pybrams-0.0.8/src/brams/timestamps.py` & `pybrams-0.0.9/src/brams/timestamps.py`

 * *Files identical despite different names*

### Comparing `pybrams-0.0.8/src/brams/wav.py` & `pybrams-0.0.9/src/brams/wav.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import struct
+from typing import Union
 import numpy as np
 import io
 from .signal import Signal
 
 class Header:
 
     fmt_main = "<H 2d 2Q 5d 2H 5d 6s 6s 6s 234s"
@@ -85,15 +86,15 @@
     def pack(self):
 
         return struct.pack(self.fmt * int(len(self.pps) / (struct.calcsize(self.fmt) / 8)), *self.pps)
 
 
 class Data:
 
-    def __init__(self, buffer, dtype: np.int16 | np.float64):
+    def __init__(self, buffer, dtype: Union[np.int16, np.float64]):
 
         self.dtype = dtype
         self.fmt = "h" if self.dtype == np.int16 else "d"
         self.npoints = int(len(buffer) / struct.calcsize(self.fmt))
         self.signal = np.array(struct.unpack("<" + self.fmt * self.npoints, buffer))
 
     def set(self, signal: Signal):
```


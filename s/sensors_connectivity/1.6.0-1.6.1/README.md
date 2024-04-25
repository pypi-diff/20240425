# Comparing `tmp/sensors_connectivity-1.6.0.tar.gz` & `tmp/sensors_connectivity-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sensors_connectivity-1.6.0.tar", max compression
+gzip compressed data, was "sensors_connectivity-1.6.1.tar", max compression
```

## Comparing `sensors_connectivity-1.6.0.tar` & `sensors_connectivity-1.6.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1507 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/LICENSE
--rw-r--r--   0        0        0     4549 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/README.md
--rw-r--r--   0        0        0       24 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/__init__.py
--rw-r--r--   0        0        0     9099 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/config/README.md
--rw-r--r--   0        0        0       36 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/config/__init__.py
--rw-r--r--   0        0        0     1006 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/config/default.json
--rw-r--r--   0        0        0      938 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/config/logging.py
--rw-r--r--   0        0        0      824 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/config/logging_template.py
--rw-r--r--   0        0        0       94 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/constants.py
--rw-r--r--   0        0        0     5975 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/main.py
--rw-r--r--   0        0        0       51 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/src/drivers/__init__.py
--rw-r--r--   0        0        0      477 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/src/drivers/ping.py
--rw-r--r--   0        0        0     5754 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/src/drivers/sds011.py
--rw-r--r--   0        0        0      189 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/src/feeders/__init__.py
--rw-r--r--   0        0        0    10475 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/src/feeders/datalog_feeder.py
--rw-r--r--   0        0        0     1280 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/src/feeders/frontier_datalog.py
--rw-r--r--   0        0        0     1088 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/src/feeders/ifeeder.py
--rw-r--r--   0        0        0     3205 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/src/feeders/robonomics_feeder.py
--rw-r--r--   0        0        0      224 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/src/sensors/__init__.py
--rw-r--r--   0        0        0     1592 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/src/sensors/base.py
--rw-r--r--   0        0        0     2149 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/src/sensors/environmental_box.py
--rw-r--r--   0        0        0      684 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/src/sensors/lora_sensors.py
--rw-r--r--   0        0        0     1483 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/src/sensors/mobile_lab.py
--rw-r--r--   0        0        0     1467 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/src/sensors/sensor_sds011.py
--rw-r--r--   0        0        0      811 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/src/sensors/sensor_template.py
--rw-r--r--   0        0        0     2612 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/src/sensors/trackagro_sensor.py
--rw-r--r--   0        0        0      212 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/src/stations/__init__.py
--rw-r--r--   0        0        0     2238 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/src/stations/comstation.py
--rw-r--r--   0        0        0     4380 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/src/stations/httpstation.py
--rw-r--r--   0        0        0     1639 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/src/stations/istation.py
--rw-r--r--   0        0        0     4111 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/src/stations/mqttstation.py
--rw-r--r--   0        0        0     3089 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/src/stations/trackargostation.py
--rw-r--r--   0        0        0       55 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/utils/__init__.py
--rw-r--r--   0        0        0     2705 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/utils/database.py
--rwxr-xr-x   0        0        0     3207 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/utils/flash_firmware.py
--rwxr-xr-x   0        0        0     1825 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/utils/generate_secrets.py
--rw-r--r--   0        0        0      391 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/utils/get_mac.py
--rwxr-xr-x   0        0        0      553 2023-09-18 10:40:55.305430 sensors_connectivity-1.6.0/connectivity/utils/py_generate_secrets.py
--rwxr-xr-x   0        0        0     2502 2023-09-18 10:40:55.309430 sensors_connectivity-1.6.0/connectivity/utils/virtual-sensor.py
--rw-r--r--   0        0        0     1258 2023-09-18 10:40:55.309430 sensors_connectivity-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     5830 1970-01-01 00:00:00.000000 sensors_connectivity-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1507 2024-04-25 10:36:17.947303 sensors_connectivity-1.6.1/LICENSE
+-rw-r--r--   0        0        0     4549 2024-04-25 10:36:17.947303 sensors_connectivity-1.6.1/README.md
+-rw-r--r--   0        0        0       24 2024-04-25 10:36:17.947303 sensors_connectivity-1.6.1/connectivity/__init__.py
+-rw-r--r--   0        0        0     9099 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/config/README.md
+-rw-r--r--   0        0        0       36 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/config/__init__.py
+-rw-r--r--   0        0        0     1006 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/config/default.json
+-rw-r--r--   0        0        0      938 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/config/logging.py
+-rw-r--r--   0        0        0      824 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/config/logging_template.py
+-rw-r--r--   0        0        0       94 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/constants.py
+-rw-r--r--   0        0        0     5975 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/main.py
+-rw-r--r--   0        0        0       51 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/src/drivers/__init__.py
+-rw-r--r--   0        0        0      477 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/src/drivers/ping.py
+-rw-r--r--   0        0        0     5754 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/src/drivers/sds011.py
+-rw-r--r--   0        0        0      189 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/src/feeders/__init__.py
+-rw-r--r--   0        0        0    10475 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/src/feeders/datalog_feeder.py
+-rw-r--r--   0        0        0     1280 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/src/feeders/frontier_datalog.py
+-rw-r--r--   0        0        0     1088 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/src/feeders/ifeeder.py
+-rw-r--r--   0        0        0     3205 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/src/feeders/robonomics_feeder.py
+-rw-r--r--   0        0        0      224 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/src/sensors/__init__.py
+-rw-r--r--   0        0        0     1592 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/src/sensors/base.py
+-rw-r--r--   0        0        0     2173 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/src/sensors/environmental_box.py
+-rw-r--r--   0        0        0      684 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/src/sensors/lora_sensors.py
+-rw-r--r--   0        0        0     1483 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/src/sensors/mobile_lab.py
+-rw-r--r--   0        0        0     1467 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/src/sensors/sensor_sds011.py
+-rw-r--r--   0        0        0      811 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/src/sensors/sensor_template.py
+-rw-r--r--   0        0        0     2612 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/src/sensors/trackagro_sensor.py
+-rw-r--r--   0        0        0      212 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/src/stations/__init__.py
+-rw-r--r--   0        0        0     2238 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/src/stations/comstation.py
+-rw-r--r--   0        0        0     4380 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/src/stations/httpstation.py
+-rw-r--r--   0        0        0     1639 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/src/stations/istation.py
+-rw-r--r--   0        0        0     4111 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/src/stations/mqttstation.py
+-rw-r--r--   0        0        0     3089 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/src/stations/trackargostation.py
+-rw-r--r--   0        0        0       55 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/utils/__init__.py
+-rw-r--r--   0        0        0     2705 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/utils/database.py
+-rwxr-xr-x   0        0        0     3207 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/utils/flash_firmware.py
+-rwxr-xr-x   0        0        0     1825 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/utils/generate_secrets.py
+-rw-r--r--   0        0        0      391 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/utils/get_mac.py
+-rwxr-xr-x   0        0        0      553 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/utils/py_generate_secrets.py
+-rwxr-xr-x   0        0        0     2502 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/connectivity/utils/virtual-sensor.py
+-rw-r--r--   0        0        0     1305 2024-04-25 10:36:17.951303 sensors_connectivity-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     5881 1970-01-01 00:00:00.000000 sensors_connectivity-1.6.1/PKG-INFO
```

### Comparing `sensors_connectivity-1.6.0/LICENSE` & `sensors_connectivity-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/README.md` & `sensors_connectivity-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/config/README.md` & `sensors_connectivity-1.6.1/connectivity/config/README.md`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/config/default.json` & `sensors_connectivity-1.6.1/connectivity/config/default.json`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/config/logging.py` & `sensors_connectivity-1.6.1/connectivity/config/logging.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/config/logging_template.py` & `sensors_connectivity-1.6.1/connectivity/config/logging_template.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/main.py` & `sensors_connectivity-1.6.1/connectivity/main.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/src/drivers/sds011.py` & `sensors_connectivity-1.6.1/connectivity/src/drivers/sds011.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/src/feeders/datalog_feeder.py` & `sensors_connectivity-1.6.1/connectivity/src/feeders/datalog_feeder.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/src/feeders/frontier_datalog.py` & `sensors_connectivity-1.6.1/connectivity/src/feeders/frontier_datalog.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/src/feeders/ifeeder.py` & `sensors_connectivity-1.6.1/connectivity/src/feeders/ifeeder.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/src/feeders/robonomics_feeder.py` & `sensors_connectivity-1.6.1/connectivity/src/feeders/robonomics_feeder.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/src/sensors/base.py` & `sensors_connectivity-1.6.1/connectivity/src/sensors/base.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/src/sensors/environmental_box.py` & `sensors_connectivity-1.6.1/connectivity/src/sensors/environmental_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     data: dict = field(repr=False)
 
     def __post_init__(self) -> None:
         """Parse data from sensor and store into the corresponding variables."""
         
         super().__post_init__()
         self.id = str(self.data["esp8266id"])
-        self.model = SDS011_MODEL
+        self.model = self.data.get("model", SDS011_MODEL)
         self.public = self.generate_pubkey(str(self.id))
         self.donated_by = str(self.data.get("donated_by", ""))
         sensors_data = self.data["sensordatavalues"]
         for d in sensors_data:
             if d["value_type"] == "GPS_lat":
                 self.geo_lat = d["value"]
             if d["value_type"] == "GPS_lon":
```

### Comparing `sensors_connectivity-1.6.0/connectivity/src/sensors/lora_sensors.py` & `sensors_connectivity-1.6.1/connectivity/src/sensors/lora_sensors.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/src/sensors/mobile_lab.py` & `sensors_connectivity-1.6.1/connectivity/src/sensors/mobile_lab.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/src/sensors/sensor_sds011.py` & `sensors_connectivity-1.6.1/connectivity/src/sensors/sensor_sds011.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/src/sensors/sensor_template.py` & `sensors_connectivity-1.6.1/connectivity/src/sensors/sensor_template.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/src/sensors/trackagro_sensor.py` & `sensors_connectivity-1.6.1/connectivity/src/sensors/trackagro_sensor.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/src/stations/comstation.py` & `sensors_connectivity-1.6.1/connectivity/src/stations/comstation.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/src/stations/httpstation.py` & `sensors_connectivity-1.6.1/connectivity/src/stations/httpstation.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/src/stations/istation.py` & `sensors_connectivity-1.6.1/connectivity/src/stations/istation.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/src/stations/mqttstation.py` & `sensors_connectivity-1.6.1/connectivity/src/stations/mqttstation.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/src/stations/trackargostation.py` & `sensors_connectivity-1.6.1/connectivity/src/stations/trackargostation.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/utils/database.py` & `sensors_connectivity-1.6.1/connectivity/utils/database.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/utils/flash_firmware.py` & `sensors_connectivity-1.6.1/connectivity/utils/flash_firmware.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/utils/generate_secrets.py` & `sensors_connectivity-1.6.1/connectivity/utils/generate_secrets.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/utils/py_generate_secrets.py` & `sensors_connectivity-1.6.1/connectivity/utils/py_generate_secrets.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/connectivity/utils/virtual-sensor.py` & `sensors_connectivity-1.6.1/connectivity/utils/virtual-sensor.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.6.0/pyproject.toml` & `sensors_connectivity-1.6.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sensors_connectivity"
-version = "1.6.0"
+version = "1.6.1"
 description = "Robonomics package to read data from sensors and publish to different output channels"
 authors = [
     "Vadim Manaenko <vadim.razorq@gmail.com>",
     "Mariia Bystramovich <m.bystramovich@gmail.com>",
 ]
 license = "BSD 3-Clause License"
 
@@ -38,11 +38,12 @@
 
 [tool.poetry.scripts]
 sensors_connectivity = "connectivity.main:run"
 test_environmental_box = "tests.environmental_box_test:main"
 test_mobile_lab = "tests.mobile_lab_test:main"
 test_many_sensors = "tests.many_environmental_boxes:main"
 test_lora_sensors = "tests.lora_sensor_test:main"
+test_gps_sensor = "tests.gps_sensor_test:main"
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sensors_connectivity-1.6.0/PKG-INFO` & `sensors_connectivity-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: sensors_connectivity
-Version: 1.6.0
+Version: 1.6.1
 Summary: Robonomics package to read data from sensors and publish to different output channels
 Home-page: https://github.com/airalab/sensors-connectivity
 License: BSD 3-Clause License
 Author: Vadim Manaenko
 Author-email: vadim.razorq@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: IPFS-Toolkit (>=0.4.4,<0.5.0)
 Requires-Dist: crust-interface-patara (>=0.1.1,<0.2.0)
 Requires-Dist: ipfshttpclient (==0.8.0a2)
 Requires-Dist: netifaces (>=0.11.0,<0.12.0)
 Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
 Requires-Dist: pinatapy-vourhey (>=0.1.3,<0.2.0)
 Requires-Dist: prometheus-client (>=0.13.1,<0.14.0)
```


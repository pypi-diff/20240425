# Comparing `tmp/accessi-0.0.2.tar.gz` & `tmp/accessi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accessi-0.0.2.tar", last modified: Sat Feb 17 12:10:23 2024, max compression
+gzip compressed data, was "accessi-0.0.5.tar", last modified: Thu Apr 25 19:12:46 2024, max compression
```

## Comparing `accessi-0.0.2.tar` & `accessi-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 12:10:23.356568 accessi-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-17 12:10:07.000000 accessi-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-02-17 12:10:23.356568 accessi-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-02-17 12:10:07.000000 accessi-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-02-17 12:10:07.000000 accessi-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-17 12:10:23.356568 accessi-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 12:10:23.356568 accessi-0.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-17 12:10:07.000000 accessi-0.0.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 12:10:23.356568 accessi-0.0.2/src/accessi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-02-17 12:10:23.000000 accessi-0.0.2/src/accessi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-02-17 12:10:23.000000 accessi-0.0.2/src/accessi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-17 12:10:23.000000 accessi-0.0.2/src/accessi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-17 12:10:23.000000 accessi-0.0.2/src/accessi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    26145 2024-02-17 12:10:07.000000 accessi-0.0.2/src/accessi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 12:10:23.356568 accessi-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-02-17 12:10:07.000000 accessi-0.0.2/tests/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:12:46.061027 accessi-0.0.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2024-04-25 18:49:29.000000 accessi-0.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1477 2024-04-25 19:12:46.061027 accessi-0.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      889 2024-04-25 18:49:29.000000 accessi-0.0.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      570 2024-04-25 19:12:13.000000 accessi-0.0.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 19:12:46.061027 accessi-0.0.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:12:46.057027 accessi-0.0.5/src/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 19:12:13.000000 accessi-0.0.5/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:12:46.057027 accessi-0.0.5/src/accessi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1477 2024-04-25 19:12:46.000000 accessi-0.0.5/src/accessi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      218 2024-04-25 19:12:46.000000 accessi-0.0.5/src/accessi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 19:12:46.000000 accessi-0.0.5/src/accessi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-25 19:12:46.000000 accessi-0.0.5/src/accessi.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    35905 2024-04-25 18:49:29.000000 accessi-0.0.5/src/accessi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:12:46.057027 accessi-0.0.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     6311 2024-04-25 18:49:29.000000 accessi-0.0.5/tests/tests.py
```

### Comparing `accessi-0.0.2/LICENSE` & `accessi-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `accessi-0.0.2/PKG-INFO` & `accessi-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accessi
-Version: 0.0.2
+Version: 0.0.5
 Summary: Library for Siemens Access-i MR Scanner Interface to integrate and control the MR Scanner.
 Author-email: Martin Reinok <m.reinok@student.utwente.nl>
 Project-URL: Homepage, https://github.com/martinreinok/accessi-library
 Project-URL: Issues, https://github.com/martinreinok/accessi-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `accessi-0.0.2/README.md` & `accessi-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `accessi-0.0.2/pyproject.toml` & `accessi-0.0.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "accessi"
-version = "0.0.2"
+version = "0.0.5"
 authors = [
   { name="Martin Reinok", email="m.reinok@student.utwente.nl" },
 ]
 description = "Library for Siemens Access-i MR Scanner Interface to integrate and control the MR Scanner."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/martinreinok/accessi-library"
-Issues = "https://github.com/martinreinok/accessi-library/issues"
+Issues = "https://github.com/martinreinok/accessi-library/issues"
```

### Comparing `accessi-0.0.2/src/accessi.egg-info/PKG-INFO` & `accessi-0.0.5/src/accessi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accessi
-Version: 0.0.2
+Version: 0.0.5
 Summary: Library for Siemens Access-i MR Scanner Interface to integrate and control the MR Scanner.
 Author-email: Martin Reinok <m.reinok@student.utwente.nl>
 Project-URL: Homepage, https://github.com/martinreinok/accessi-library
 Project-URL: Issues, https://github.com/martinreinok/accessi-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `accessi-0.0.2/src/accessi.py` & `accessi-0.0.5/src/accessi.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 # TODO: Table Service Not implemented.
 # TODO: Tracking Service Not implemented.
 # TODO: Issue Service Not implemented.
 # TODO: Adjustment Service Not implemented.
 # TODO: Debugging Service Not implemented.
 
 from types import SimpleNamespace
+from math import atan2, degrees
 from typing import Literal
+import numpy as np
 import websockets
 import requests
 import urllib3
-import math
+import asyncio
 import json
 import ssl
-import sys
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
 class config:
     """
     User-configurable variables for establishing a connection with the MR host.
@@ -43,14 +44,18 @@
     def base_url():
         return f"{config.protocol}://{config.ip_address}:{config.port}/SRC/{config.version}/product"
 
     @staticmethod
     def base_url_remote():
         return f"{config.protocol}://{config.ip_address}:{config.port}/SRC/product/remote"
 
+    @staticmethod
+    def websocket_default_url():
+        return f"wss://{config.ip_address}:{config.websocket_port}/SRC?sessionId={config.session_id}"
+
 
 class Remote:
     """
     The remote service provides the RC with options to check whether and which version of the SRC is up and running
     on the MR host. This service requires no prior authorization of the RC.
     """
 
@@ -77,15 +82,15 @@
 
 
 class Authorization:
     """
     The Authorization service (authorization) ensures that only RCs with a valid authentication key
     can communicate with the Access-i server.
     Before any of the services described in this document can be used,
-    a RC must register providing a valid authentication key (provided by your point of contact at Siemens Healthineers),
+    an RC must register providing a valid authentication key (provided by your point of contact at Siemens Healthineers),
     which also encodes the scope of functionality that can be used by the RC.
     """
 
     @staticmethod
     def register(name="Access_i SDK", comment=None, start_date="20180115", warn_date="20391215",
                  expire_date="20400115", system_id="99999999999999", is_read_option_available=True,
                  is_execute_option_available=True, is_advanced_option_available=True, version="1.0",
@@ -141,15 +146,15 @@
 
 class HostControl:
     """
     The Host Control Service allows changing the entity that is controlling
     the MR host which is either the MR host itself or an RC.
     At a given point in time only one entity can actively control the host, i.e.
     has the mastership with respect to controlling the workflow.
-    As soon as a RC releases the control, the MR host is automatically in charge.
+    As soon as an RC releases the control, the MR host is automatically in charge.
     The RC can only retrieve the mastership if a patient is registered and no sequence is running or open.
     """
 
     @staticmethod
     def get_state():
         """
         Response example:
@@ -410,26 +415,26 @@
          - "value":{"x":10.0,"y":10.0,"z":20.0}
         """
         url = f"{config.base_url()}/parameter/standard/getSlicePositionDcs"
         data = {"sessionId": config.session_id}
         return send_request(url, data, "GET")
 
     @staticmethod
-    def set_slice_position_dcs(index=0, x=None, y=None, z=None, allow_side_effects=True):
+    def set_slice_position_dcs(x=None, y=None, z=None, allow_side_effects=True, index=0):
         """
         Response example:
          - "result":{"success":true,"reason":"ok","time":"20170608T143325.423"},
          - "valueSet":{"x":10.0,"y":-10.0,"z":-20.0}
         """
         url = f"{config.base_url()}/parameter/standard/setSlicePositionDcs"
         data = {"sessionId": config.session_id,
                 "index": index,
                 "value": {"x": x, "y": y, "z": z},
                 "allowSideEffects": allow_side_effects}
-        return send_request(url, data)
+        return send_request(url, data, "POST")
 
     @staticmethod
     def get_slice_orientation_dcs():
         """
         Response example:
          - "result":{"success":true,"reason":"ok","time":"20170608T143325.423"},
          - "normal":{"x":0,"y":0,"z":-1.0},
@@ -437,18 +442,16 @@
          - "read":{"x":-1.0,"y":0,"z":0}
         """
         url = f"{config.base_url()}/parameter/standard/getSliceOrientationDcs"
         data = {"sessionId": config.session_id}
         return send_request(url, data, "GET")
 
     @staticmethod
-    def set_slice_orientation_dcs(index=0, allow_side_effects=True,
-                                  normal: tuple = (0, 0, 0),
-                                  phase: tuple = (0, 0, 0),
-                                  read: tuple = (0, 0, 0)):
+    def set_slice_orientation_dcs(normal: tuple = (0, 0, 0), phase: tuple = (0, 0, 0), read: tuple = (0, 0, 0),
+                                  allow_side_effects=True, index=0):
         """
         Response example:
          - "result":{"success":true,"reason":"ok","time":"20170608T143325.423"},
          - "normalSet":{"x":0,"y":0,"z":-1.0},
          - "phaseSet":{"x":0,"y":-1.0,"z":0},
          - "readSet":{"x":-1.0,"y":0,"z":0}
         """
@@ -458,37 +461,274 @@
                 "normal": {"x": normal[0], "y": normal[1], "z": normal[2]},
                 "phase": {"x": phase[0], "y": phase[1], "z": phase[2]},
                 "read": {"x": read[0], "y": read[1], "z": read[2]},
                 "allowSideEffects": allow_side_effects}
         return send_request(url, data, "POST")
 
     @staticmethod
+    def set_slice_orientation_pcs(normal: tuple = (0, 0, 0), phase: tuple = (0, 0, 0), read: tuple = (0, 0, 0),
+                                  allow_side_effects=True, index=0):
+        """
+        Response example:
+         - "result":{"success":true,"reason":"ok","time":"20170608T143325.423"},
+         - "normalSet":{"x":0,"y":0,"z":-1.0},
+         - "phaseSet":{"x":0,"y":-1.0,"z":0},
+         - "readSet":{"x":-1.0,"y":0,"z":0}
+        """
+        url = f"{config.base_url()}/parameter/standard/setSliceOrientationPcs"
+        data = {"sessionId": config.session_id,
+                "index": index,
+                "normal": {"sag": float(normal[0]), "cor": float(normal[1]), "tra": float(normal[2])},
+                "phase": {"sag": float(phase[0]), "cor": float(phase[1]), "tra": float(phase[2])},
+                "read": {"sag": float(read[0]), "cor": float(read[1]), "tra": float(read[2])},
+                "allowSideEffects": allow_side_effects}
+        return send_request(url, data, "POST")
+
+    @staticmethod
+    def get_slice_orientation_pcs():
+        """
+        Response example:
+         - "result":{"success":true,"reason":"ok","time":"20170608T143325.423"},
+         - "normal":{"x":0,"y":0,"z":-1.0},
+         - "phase":{"x":0,"y":-1.0,"z":0},
+         - "read":{"x":-1.0,"y":0,"z":0}
+        """
+        url = f"{config.base_url()}/parameter/standard/getSliceOrientationPcs"
+        data = {"sessionId": config.session_id}
+        return send_request(url, data, "GET")
+
+    @staticmethod
+    def get_number_of_slice_groups():
+        """
+        Response example:
+         - "result":{"success":true,"reason":"ok","time":"20170608T143325.423"},
+         - "value":2
+        """
+        url = f"{config.base_url()}/parameter/standard/getNumberOfSliceGroups"
+        data = {"sessionId": config.session_id}
+        return send_request(url, data, "GET")
+
+    @staticmethod
+    def get_number_of_slices():
+        """
+        Response example:
+         - "result":{"success":true,"reason":"ok","time":"20170608T143325.423"},
+         - "value":2
+        """
+        url = f"{config.base_url()}/parameter/standard/getNumberOfSlices"
+        data = {"sessionId": config.session_id}
+        return send_request(url, data, "GET")
+
+    @staticmethod
+    def set_slice_orientation_degrees_dcs(roll_degrees, pitch_degrees, yaw_degrees, allow_side_effects=True, index=0):
+        """
+        This math is not completely verified but seems to work.
+        Response example:
+         - "result":{"success":true,"reason":"ok","time":"20170608T143325.423"},
+         - "normalSet":{"x":0,"y":0,"z":-1.0},
+         - "phaseSet":{"x":0,"y":-1.0,"z":0},
+         - "readSet":{"x":-1.0,"y":0,"z":0}
+        """
+        rotation_matrix = ParameterStandard.euler_to_rotation_matrix((roll_degrees, pitch_degrees, yaw_degrees))
+        basis_vectors = np.eye(3)
+        rotated_vectors = np.dot(rotation_matrix, basis_vectors.T).T
+        normalized_vectors = rotated_vectors / np.linalg.norm(rotated_vectors, axis=1, keepdims=True)
+
+        for vector in normalized_vectors:
+            if vector[2] < 0:  # Ensure the largest component is positive
+                vector *= -1
+
+        normal = np.array([rotation_matrix[0, 0], rotation_matrix[0, 1], rotation_matrix[0, 2]])
+        phase = np.array([rotation_matrix[1, 0], rotation_matrix[1, 1], rotation_matrix[1, 2]])
+        read = np.array([rotation_matrix[2, 0], rotation_matrix[2, 1], rotation_matrix[2, 2]])
+
+        # Set the slice orientation using the RAS coordinate system
+        return ParameterStandard.set_slice_orientation_dcs(normal, phase, read, allow_side_effects, index)
+
+    @staticmethod
+    def euler_to_rotation_matrix(angles=(0, 0, 0)):
+        phi, theta, psi = np.radians(angles)
+        R_x = np.array([[1, 0, 0],
+                        [0, np.cos(phi), -np.sin(phi)],
+                        [0, np.sin(phi), np.cos(phi)]])
+        R_y = np.array([[np.cos(theta), 0, np.sin(theta)],
+                        [0, 1, 0],
+                        [-np.sin(theta), 0, np.cos(theta)]])
+        R_z = np.array([[np.cos(psi), -np.sin(psi), 0],
+                        [np.sin(psi), np.cos(psi), 0],
+                        [0, 0, 1]])
+        return np.dot(R_z, np.dot(R_y, R_x))
+
+    @staticmethod
+    def get_slice_orientation_degrees_dcs():
+        """
+        This math is not completely verified but seems to work.
+        Response example:
+         - "result":{"success":true,"reason":"ok","time":"20170608T143325.423"},
+         - "normal":{180},
+         - "phase":{0},
+         - "read":{180}
+        """
+        answer = ParameterStandard.get_slice_orientation_dcs()
+        if not answer.result.success:
+            return answer.result.reason
+
+        normal = np.array([answer.normal.x, answer.normal.y, answer.normal.z])
+        phase = np.array([answer.phase.x, answer.phase.y, answer.phase.z])
+        read = np.array([answer.read.x, answer.read.y, answer.read.z])
+
+        rotation_matrix = np.array([normal, phase, read])
+
+        theta = -np.arcsin(rotation_matrix[0, 2])  # pitch
+        psi = np.arctan2(rotation_matrix[0, 1], rotation_matrix[0, 0])  # yaw
+        phi = np.arctan2(rotation_matrix[1, 2], rotation_matrix[2, 2])  # roll
+
+        # Convert unit vectors to angles (in degrees)
+        answer.normal = np.degrees(phi)
+        answer.phase = np.degrees(theta)
+        answer.read = np.degrees(psi)
+        return answer
+
+    @staticmethod
     def get_slice_thickness():
         """
         Unit:mm
         Response example:
          - "result":{"success":true,"reason":"ok","time":"20170608T143325.423"},
          - "value":2.5
         """
         url = f"{config.base_url()}/parameter/standard/getSliceThickness"
         data = {"sessionId": config.session_id}
         return send_request(url, data, "GET")
 
     @staticmethod
+    def get_field_of_view_read():
+        """
+        Unit:mm
+        Response example:
+         - "result":{"success":true,"reason":"ok","time":"20170608T143325.423"},
+         - "value": 400.0
+        """
+        url = f"{config.base_url()}/parameter/standard/getFieldOfViewRead"
+        data = {"sessionId": config.session_id}
+        return send_request(url, data, "GET")
+
+    @staticmethod
+    def set_field_of_view_read(value, allow_side_effects=True):
+        """
+        Unit:mm
+        Response example:
+         - "result":{"success":true,"reason":"ok","time":"20170608T143325.423"},
+         - "valueSet":350.0
+        """
+        url = f"{config.base_url()}/parameter/standard/setFieldOfViewRead"
+        data = {"sessionId": config.session_id,
+                "value": value,
+                "allowSideEffects": allow_side_effects}
+        return send_request(url, data, "POST")
+
+    @staticmethod
     def set_slice_thickness(value, allow_side_effects=True):
         """
         Unit:mm
         Response example:
          - "result":{"success":true,"reason":"ok","time":"20170608T143325.423"},
          - "valueSet":3.5
         """
         url = f"{config.base_url()}/parameter/standard/setSliceThickness"
         data = {"sessionId": config.session_id, "value": float(value), "allowSideEffects": allow_side_effects}
         return send_request(url, data, "POST")
 
+    @staticmethod
+    def get_base_resolution():
+        """
+        Unit:mm
+        Response example:
+         - "result":{"success":true,"reason":"ok","time":"20170608T143325.423"},
+         - "value":128
+        """
+        url = f"{config.base_url()}/parameter/standard/getBaseResolution"
+        data = {"sessionId": config.session_id}
+        return send_request(url, data, "GET")
+
+    @staticmethod
+    def set_base_resolution(value, allow_side_effects=True):
+        """
+        Unit:mm
+        Response example:
+         - "result":{"success":true,"reason":"ok","time":"20170608T143325.423"},
+         - "valueSet":192
+        """
+        url = f"{config.base_url()}/parameter/standard/setBaseResolution"
+        data = {"sessionId": config.session_id, "value": value, "allowSideEffects": allow_side_effects}
+        return send_request(url, data, "POST")
+
+
+class Table:
+    """
+    The table service was newly introduced in version 2 of the Access-i interface,
+     to reflect the new / changed table positioning modes that are available for the Numaris X Sola / Vida systems.
+     In contrast to Access-i version 1, the table positioning mode is set globally for the whole workflow,
+     i.e. not template-/protocol-specific. Therefore a dedicated service was introduced for this purpose.
+    """
+
+    @staticmethod
+    def get_current_table_position():
+        """
+        Response example:
+         - "result":{"success":true,"reason":"ok","time":"20170608T143325.423"},
+         - "value":120
+        """
+        url = f"{config.base_url()}/table/getCurrentTablePosition"
+        data = {"sessionId": config.session_id}
+        return send_request(url, data, "GET")
+
+    @staticmethod
+    def get_table_positioning_mode():
+        """
+        Response example:
+         - "result":{"success":true,"reason":"ok","time":"20170608T143325.423"},
+         - "value":"fix"
+        """
+        url = f"{config.base_url()}/table/getTablePositioningMode"
+        data = {"sessionId": config.session_id}
+        return send_request(url, data, "GET")
+
+    @staticmethod
+    def set_table_positioning_mode(value: Literal["isoCenter", "localRange", "fix"] = "isoCenter"):
+        """
+        Response example:
+         - "result":{"success":true,"reason":"ok","time":"20170608T143325.423"},
+         - "value":"fix"
+        """
+        url = f"{config.base_url()}/table/setTablePositioningMode"
+        data = {"sessionId": config.session_id, "value": value}
+        return send_request(url, data, "POST")
+
+    @staticmethod
+    def get_fix_table_position():
+        """
+        Response example:
+         - "result":{"success":true,"reason":"ok","time":"20170608T143325.423"},
+         - "value":123
+        """
+        url = f"{config.base_url()}/table/getFixTablePosition"
+        data = {"sessionId": config.session_id}
+        return send_request(url, data, "GET")
+
+    @staticmethod
+    def set_fix_table_position(value: int):
+        """
+        Response example:
+         - "result":{"success":true,"reason":"ok","time":"20170608T143325.423"}
+        """
+        url = f"{config.base_url()}/table/setFixTablePosition"
+        data = {"sessionId": config.session_id, "value": value}
+        return send_request(url, data, "POST")
+
 
 class Image:
     """
     Via the websocket functionality the client can automatically receive images that are reconstructed on the MR host.
     """
 
     @staticmethod
@@ -653,34 +893,37 @@
 def handle_websocket_message(data):
     service, request, response, message = None, None, None, None
     try:
         message = json.loads(data)
         service = message.get('service', '')
         request = message.get('request', '')
         response = message.get('response', '')
-        print("Service:", service)
-        print("Request:", request)
     except json.JSONDecodeError as e:
         print("Error decoding JSON:", e)
     return [service, request, response, message]
 
 
-async def connect_websocket(config, callback_function):
-    url = f"wss://{config.ip_address}:{config.websocket_port}/SRC?sessionId={config.session_id}"
-    if not config.ssl_verify:
-        ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
-        ssl_context.check_hostname = False
-        ssl_context.verify_mode = ssl.CERT_NONE
-    else:
-        raise SystemExit("SSL verification no supported yet")
-    async with websockets.connect(url, ssl=ssl_context) as websocket:
-        while True:
-            message = await websocket.recv()
-            decoded_message = handle_websocket_message(message)
-            await callback_function(decoded_message)
+async def connect_websocket():
+    """
+    Connects to the websocket server and returns the connected websocket object.
+    Returns websockets.legacy.client.Connect object
+    """
+    try:
+        url = config.websocket_default_url()
+        if not config.ssl_verify:
+            ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
+            ssl_context.check_hostname = False
+            ssl_context.verify_mode = ssl.CERT_NONE
+        else:
+            raise SystemExit("SSL verification not supported yet")
+        return websockets.connect(url, ssl=ssl_context)
+    except (websockets.ConnectionClosed, asyncio.TimeoutError) as e:
+        raise ConnectionError("Connection failed: " + str(e)) from e
+    except Exception as e:
+        raise e
 
 
 def response_to_object(json_response):
     return json.loads(json.dumps(json_response.json()), object_hook=lambda d: SimpleNamespace(**d))
 
 
 def send_request(url, data, request_type: Literal["GET", "POST"] = "POST"):
```

### Comparing `accessi-0.0.2/tests/tests.py` & `accessi-0.0.5/tests/tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """
 Usage example and tests to make sure the library works.
 Siemens Access-i simulator should be running for this to work (or real MRI system with appropriate IP-address).
 """
 import json
+from asyncio import LifoQueue
 from types import SimpleNamespace
-
-import src as Access
+from src import accessi as Access
 import threading
 import asyncio
 import time
 
-
 Access.config.ip_address = "127.0.0.1"
 Access.config.version = "v2"
 
 """
 Remote Service
 """
 output = Access.Remote.get_is_active().result.success
@@ -83,16 +82,21 @@
 output = Access.SystemInformation.get_serial_number().value
 print(f"get_serial_number: {output}")
 assert output is not None
 
 """
 Template Execution Service
 """
-template = Access.TemplateExecution.get_templates().value[0]
-print(f"get_template [0]: {template.label}")
+# Find interactive template
+i = 0
+template = Access.TemplateExecution.get_templates().value[i]
+while not template.isInteractive:
+    i += 1
+    template = Access.TemplateExecution.get_templates().value[i]
+print(f"get_template [{i}]: {template.label}")
 template_id = template.id
 assert template_id is not None
 
 output = Access.TemplateExecution.get_state().value.canStart
 print(f"get_state can start template: {output}")
 assert output is True
 
@@ -164,48 +168,46 @@
 Image Service
 """
 output = Access.Image.set_image_format("raw16bit").result.success
 print(f"set_image_format: {output}")
 assert output is True
 
 
-async def demo_callback_function(image_data):
-    if "imageStream" in image_data:
-        image_data = json.loads(json.dumps(image_data), object_hook=lambda d: SimpleNamespace(**d))
-        print(f"Websocket callback image dimensions: "
-              f"{image_data[2].value.image.dimensions.columns},"
-              f"{image_data[2].value.image.dimensions.rows} ")
-
-
-def run_websocket_in_thread(config, callback_function):
-    loop = asyncio.new_event_loop()
-    asyncio.set_event_loop(loop)
-    try:
-        loop.run_until_complete(Access.connect_websocket(config, callback_function))
-    except Exception as error:
-        print(f"Websocket was unexpectedly closed (this is fine), {error}")
-
-
-thread = threading.Thread(target=run_websocket_in_thread, args=(Access.config, demo_callback_function))
-thread.start()
-
-websocket = Access.Image.connect_to_default_web_socket()
-print(f"connect_to_default_web_socket: {websocket}")
-assert websocket.result.success is True
-
-output = Access.TemplateExecution.start(template_id).result.success
-print(f"start: {output}")
-assert output is True
+async def main():
+    # Run websocket
+    async with await Access.connect_websocket() as websocket:
+
+        # Connect the image service to websocket
+        websocket_connection = Access.Image.connect_to_default_web_socket()
+        print(f"connect_to_default_web_socket: {websocket_connection}")
+        assert websocket_connection.result.success is True
+
+        # Start template
+        output = Access.TemplateExecution.start(template_id).result.success
+        print(f"start: {output}")
+        assert output is True
+
+        # Receive one image and quit
+        while True:
+            image_data = await websocket.recv()
+            if '"imageStream"' in image_data:
+                image_data = json.dumps(Access.handle_websocket_message(image_data))
+                image_data = json.loads(image_data, object_hook=lambda d: SimpleNamespace(**d))
+                print(f"Websocket callback image dimensions: "
+                      f"{image_data[2].value.image.dimensions.columns},"
+                      f"{image_data[2].value.image.dimensions.rows} ")
+                break
+
+        """
+        Done, cleanup
+        """
+        print("Tests done, cleaning up")
+        Access.TemplateExecution.stop()
+        Access.TemplateModification.close()
+        Access.HostControl.release_host_control()
+        Access.Authorization.deregister()
+        print("It works!")
+        raise SystemExit
 
-print("Sleeping 5 seconds")
-time.sleep(5)
 
-"""
-Done, cleanup
-"""
-
-Access.TemplateExecution.stop()
-Access.TemplateModification.close()
-Access.HostControl.release_host_control()
-Access.Authorization.deregister()
-print("It works!")
-SystemExit()
+print("Running websocket for 1 image")
+asyncio.run(main())
```


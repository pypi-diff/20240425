# Comparing `tmp/can-j1939-ttpsc-1.0.2.tar.gz` & `tmp/can-j1939-ttpsc-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "can-j1939-ttpsc-1.0.2.tar", last modified: Wed Oct 25 12:37:34 2023, max compression
+gzip compressed data, was "can-j1939-ttpsc-1.0.3.tar", last modified: Thu Apr 25 08:54:04 2024, max compression
```

## Comparing `can-j1939-ttpsc-1.0.2.tar` & `can-j1939-ttpsc-1.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 molinaf   (1000) molinaf   (1000)        0 2023-10-25 12:37:34.985403 can-j1939-ttpsc-1.0.2/
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     1148 2023-10-25 10:48:29.000000 can-j1939-ttpsc-1.0.2/LICENSE
--rw-r--r--   0 molinaf   (1000) molinaf   (1000)     8173 2023-10-25 12:37:34.985403 can-j1939-ttpsc-1.0.2/PKG-INFO
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     7496 2023-10-25 12:36:45.000000 can-j1939-ttpsc-1.0.2/README.rst
-drwxrwxr-x   0 molinaf   (1000) molinaf   (1000)        0 2023-10-25 12:37:34.981403 can-j1939-ttpsc-1.0.2/can_j1939_ttpsc.egg-info/
--rw-r--r--   0 molinaf   (1000) molinaf   (1000)     8173 2023-10-25 12:37:34.000000 can-j1939-ttpsc-1.0.2/can_j1939_ttpsc.egg-info/PKG-INFO
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)      618 2023-10-25 12:37:34.000000 can-j1939-ttpsc-1.0.2/can_j1939_ttpsc.egg-info/SOURCES.txt
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)        1 2023-10-25 12:37:34.000000 can-j1939-ttpsc-1.0.2/can_j1939_ttpsc.egg-info/dependency_links.txt
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)       46 2023-10-25 12:37:34.000000 can-j1939-ttpsc-1.0.2/can_j1939_ttpsc.egg-info/requires.txt
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)       19 2023-10-25 12:37:34.000000 can-j1939-ttpsc-1.0.2/can_j1939_ttpsc.egg-info/top_level.txt
-drwxrwxr-x   0 molinaf   (1000) molinaf   (1000)        0 2023-10-25 12:37:34.985403 can-j1939-ttpsc-1.0.2/j1939/
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)      327 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.2/j1939/__init__.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)    14753 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.2/j1939/controller_application.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)    11844 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.2/j1939/diagnostic_messages.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)    14995 2023-09-28 10:57:27.000000 can-j1939-ttpsc-1.0.2/j1939/electronic_control_unit.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)    31187 2023-09-28 11:33:28.000000 can-j1939-ttpsc-1.0.2/j1939/j1939_21.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)    48909 2023-09-28 11:16:49.000000 can-j1939-ttpsc-1.0.2/j1939/j1939_22.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     6776 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.2/j1939/memory_access.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     1839 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.2/j1939/message_id.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)    10322 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.2/j1939/name.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     5323 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.2/j1939/parameter_group_number.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)       22 2023-10-25 12:37:26.000000 can-j1939-ttpsc-1.0.2/j1939/version.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)       67 2023-10-25 12:37:34.985403 can-j1939-ttpsc-1.0.2/setup.cfg
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     1216 2023-10-25 12:10:42.000000 can-j1939-ttpsc-1.0.2/setup.py
-drwxrwxr-x   0 molinaf   (1000) molinaf   (1000)        0 2023-10-25 12:37:34.985403 can-j1939-ttpsc-1.0.2/test/
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     3786 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.2/test/test_ca.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     6705 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.2/test/test_ecu.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     4278 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.2/test/test_memory_access.py
-drwxrwxr-x   0 molinaf   (1000) molinaf   (1000)        0 2023-10-25 12:37:34.985403 can-j1939-ttpsc-1.0.2/test_helpers/
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)        0 2023-10-25 11:46:34.000000 can-j1939-ttpsc-1.0.2/test_helpers/__init__.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)      168 2023-10-25 11:46:34.000000 can-j1939-ttpsc-1.0.2/test_helpers/conftest.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     5279 2023-10-25 11:46:34.000000 can-j1939-ttpsc-1.0.2/test_helpers/feeder.py
+drwxrwxr-x   0 molinaf   (1000) molinaf   (1000)        0 2024-04-25 08:54:04.260985 can-j1939-ttpsc-1.0.3/
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     1148 2023-10-25 10:48:29.000000 can-j1939-ttpsc-1.0.3/LICENSE
+-rw-r--r--   0 molinaf   (1000) molinaf   (1000)     8173 2024-04-25 08:54:04.260985 can-j1939-ttpsc-1.0.3/PKG-INFO
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     7496 2023-10-25 12:36:45.000000 can-j1939-ttpsc-1.0.3/README.rst
+drwxrwxr-x   0 molinaf   (1000) molinaf   (1000)        0 2024-04-25 08:54:04.248985 can-j1939-ttpsc-1.0.3/can_j1939_ttpsc.egg-info/
+-rw-r--r--   0 molinaf   (1000) molinaf   (1000)     8173 2024-04-25 08:54:04.000000 can-j1939-ttpsc-1.0.3/can_j1939_ttpsc.egg-info/PKG-INFO
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)      618 2024-04-25 08:54:04.000000 can-j1939-ttpsc-1.0.3/can_j1939_ttpsc.egg-info/SOURCES.txt
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)        1 2024-04-25 08:54:04.000000 can-j1939-ttpsc-1.0.3/can_j1939_ttpsc.egg-info/dependency_links.txt
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)       46 2024-04-25 08:54:04.000000 can-j1939-ttpsc-1.0.3/can_j1939_ttpsc.egg-info/requires.txt
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)       19 2024-04-25 08:54:04.000000 can-j1939-ttpsc-1.0.3/can_j1939_ttpsc.egg-info/top_level.txt
+drwxrwxr-x   0 molinaf   (1000) molinaf   (1000)        0 2024-04-25 08:54:04.256985 can-j1939-ttpsc-1.0.3/j1939/
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)      327 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.3/j1939/__init__.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)    14753 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.3/j1939/controller_application.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)    11844 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.3/j1939/diagnostic_messages.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)    14995 2023-09-28 10:57:27.000000 can-j1939-ttpsc-1.0.3/j1939/electronic_control_unit.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)    28786 2024-04-13 10:34:02.000000 can-j1939-ttpsc-1.0.3/j1939/j1939_21.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)    46754 2024-04-13 10:34:43.000000 can-j1939-ttpsc-1.0.3/j1939/j1939_22.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     6776 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.3/j1939/memory_access.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     1839 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.3/j1939/message_id.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)    10322 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.3/j1939/name.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     5323 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.3/j1939/parameter_group_number.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)       22 2024-04-25 08:53:45.000000 can-j1939-ttpsc-1.0.3/j1939/version.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)       67 2024-04-25 08:54:04.260985 can-j1939-ttpsc-1.0.3/setup.cfg
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     1216 2023-10-25 12:10:42.000000 can-j1939-ttpsc-1.0.3/setup.py
+drwxrwxr-x   0 molinaf   (1000) molinaf   (1000)        0 2024-04-25 08:54:04.256985 can-j1939-ttpsc-1.0.3/test/
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     3786 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.3/test/test_ca.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     6705 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.3/test/test_ecu.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     4278 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.3/test/test_memory_access.py
+drwxrwxr-x   0 molinaf   (1000) molinaf   (1000)        0 2024-04-25 08:54:04.260985 can-j1939-ttpsc-1.0.3/test_helpers/
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)        0 2023-10-25 11:46:34.000000 can-j1939-ttpsc-1.0.3/test_helpers/__init__.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)      168 2023-10-25 11:46:34.000000 can-j1939-ttpsc-1.0.3/test_helpers/conftest.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     5279 2023-10-25 11:46:34.000000 can-j1939-ttpsc-1.0.3/test_helpers/feeder.py
```

### Comparing `can-j1939-ttpsc-1.0.2/LICENSE` & `can-j1939-ttpsc-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.2/PKG-INFO` & `can-j1939-ttpsc-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: can-j1939-ttpsc
-Version: 1.0.2
+Version: 1.0.3
 Summary: Fork of SAE J1939 stack implementation, originally created by Juergen Heilgemeir
 Home-page: https://github.com/ttpscmolinaf/python-can-j1939
 Author: TTPSC
 License: MIT
 Keywords: CAN SAE J1939 J1939-FD J1939-22
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `can-j1939-ttpsc-1.0.2/README.rst` & `can-j1939-ttpsc-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.2/can_j1939_ttpsc.egg-info/PKG-INFO` & `can-j1939-ttpsc-1.0.3/can_j1939_ttpsc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: can-j1939-ttpsc
-Version: 1.0.2
+Version: 1.0.3
 Summary: Fork of SAE J1939 stack implementation, originally created by Juergen Heilgemeir
 Home-page: https://github.com/ttpscmolinaf/python-can-j1939
 Author: TTPSC
 License: MIT
 Keywords: CAN SAE J1939 J1939-FD J1939-22
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `can-j1939-ttpsc-1.0.2/can_j1939_ttpsc.egg-info/SOURCES.txt` & `can-j1939-ttpsc-1.0.3/can_j1939_ttpsc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.2/j1939/controller_application.py` & `can-j1939-ttpsc-1.0.3/j1939/controller_application.py`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.2/j1939/diagnostic_messages.py` & `can-j1939-ttpsc-1.0.3/j1939/diagnostic_messages.py`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.2/j1939/electronic_control_unit.py` & `can-j1939-ttpsc-1.0.3/j1939/electronic_control_unit.py`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.2/j1939/j1939_21.py` & `can-j1939-ttpsc-1.0.3/j1939/j1939_21.py`

 * *Files 5% similar despite different names*

```diff
@@ -708,79 +708,24 @@
             seconds.
             Where possible this will be timestamped in hardware.
         """
 
         mid = MessageId(can_id=can_id)
         pgn = ParameterGroupNumber()
         pgn.from_message_id(mid)
-
-        if pgn.is_pdu2_format:
-            # direct broadcast
-            """
-            As of commit https://github.com/juergenH87/python-can-j1939/commit/739c1c0baf24c07cdf32e96289595954200782b9
-            It was added the channel parameter for the notifier.
-            """
-            # Added channel param
-            self.__notify_subscribers(
-                mid.priority,
-                pgn.value,
-                mid.source_address,
-                ParameterGroupNumber.Address.GLOBAL,
-                timestamp,
-                data,
-                channel,
-            )
-            return
-
-        # peer to peer
-        # pdu_specific is destination Address
-        pgn_value = pgn.value & 0x1FF00
-        dest_address = pgn.pdu_specific  # may be Address.GLOBAL
-
-        # iterate all CAs to check if we have to handle this destination address
-        if dest_address != ParameterGroupNumber.Address.GLOBAL:
-            if not self.__ecu_is_message_acceptable(
-                dest_address
-            ):  # simple peer-to-peer reception without adding a controller-application
-                reject = True
-                for ca in self._cas:
-                    if ca.message_acceptable(dest_address):
-                        reject = False
-                        break
-                if reject == True:
-                    return
-
-        if pgn_value == ParameterGroupNumber.PGN.ADDRESSCLAIM:
-            for ca in self._cas:
-                ca._process_addressclaim(mid, data, timestamp)
-        elif pgn_value == ParameterGroupNumber.PGN.REQUEST:
-            for ca in self._cas:
-                if ca.message_acceptable(dest_address):
-                    ca._process_request(mid, dest_address, data, timestamp)
-        elif pgn_value == ParameterGroupNumber.PGN.TP_CM:
-            """
-            As of commit https://github.com/juergenH87/python-can-j1939/commit/739c1c0baf24c07cdf32e96289595954200782b9
-            It was added the channel parameter for the notifier.
-            """
-            self._process_tp_cm(mid, dest_address, data, timestamp, channel)
-        elif pgn_value == ParameterGroupNumber.PGN.DATATRANSFER:
-            """
-            As of commit https://github.com/juergenH87/python-can-j1939/commit/739c1c0baf24c07cdf32e96289595954200782b9
-            It was added the channel parameter for the notifier.
-            """
-            self._process_tp_dt(mid, dest_address, data, timestamp, channel)
-        else:
-            """
-            As of commit https://github.com/juergenH87/python-can-j1939/commit/739c1c0baf24c07cdf32e96289595954200782b9
-            It was added the channel parameter for the notifier.
-            """
-            # Added channel param
-            self.__notify_subscribers(
-                mid.priority,
-                pgn_value,
-                mid.source_address,
-                dest_address,
-                timestamp,
-                data,
-                channel,
-            )
-            return
+        # Direct broadcast
+        # Removed peer to peer logic, we are interested in sniffing only.
+        """
+        As of commit https://github.com/juergenH87/python-can-j1939/commit/739c1c0baf24c07cdf32e96289595954200782b9
+        It was added the channel parameter for the notifier.
+        """
+        # Added channel param
+        self.__notify_subscribers(
+            mid.priority,
+            pgn.value,
+            mid.source_address,
+            ParameterGroupNumber.Address.GLOBAL,
+            timestamp,
+            data,
+            channel,
+        )
+        return
```

### Comparing `can-j1939-ttpsc-1.0.2/j1939/j1939_22.py` & `can-j1939-ttpsc-1.0.3/j1939/j1939_22.py`

 * *Files 3% similar despite different names*

```diff
@@ -1190,67 +1190,18 @@
             seconds.
             Where possible this will be timestamped in hardware.
         """
         mid = MessageId(can_id=can_id)
         pgn = ParameterGroupNumber()
         pgn.from_message_id(mid)
 
-        # peer to peer
-        # pdu_specific is destination Address
-        pgn_value = pgn.value & 0x1FF00
-        dest_address = pgn.pdu_specific  # may be Address.GLOBAL
-
-        # iterate all CAs to check if we have to handle this destination address
-        if dest_address != ParameterGroupNumber.Address.GLOBAL:
-            if not self.__ecu_is_message_acceptable(
-                dest_address
-            ):  # simple peer-to-peer reception without adding a controller-application
-                reject = True
-                for ca in self._cas:
-                    if ca.message_acceptable(dest_address):
-                        reject = False
-                        break
-                if reject == True:
-                    return
-
-        if pgn_value == ParameterGroupNumber.PGN.FEFF_MULTI_PG:
-            self._process_multi_pg(mid, dest_address, data, timestamp)
-        elif pgn_value == ParameterGroupNumber.PGN.ADDRESSCLAIM:
-            for ca in self._cas:
-                ca._process_addressclaim(mid, data, timestamp)
-        elif pgn_value == ParameterGroupNumber.PGN.REQUEST:
-            for ca in self._cas:
-                if ca.message_acceptable(dest_address):
-                    ca._process_request(mid, dest_address, data, timestamp)
-        elif pgn_value == ParameterGroupNumber.PGN.FD_TP_CM:
-            self._process_tp_cm(mid, dest_address, data, timestamp)
-        elif pgn_value == ParameterGroupNumber.PGN.FD_TP_DT:
-            self._process_tp_dt(mid, dest_address, data, timestamp)
-        elif pgn_value == ParameterGroupNumber.PGN.TP_CM:
-            logger.info(
-                "j1939-21 transport protocol cm not allowed in j1939-22 network"
-            )
-        elif pgn_value == ParameterGroupNumber.PGN.DATATRANSFER:
-            logger.info(
-                "j1939-21 transport protocol dt not allowed in j1939-22 network"
-            )
-        elif pgn.is_pdu2_format:
-            # direct broadcast
-            self.__notify_subscribers(
-                mid.priority,
-                pgn.value,
-                mid.source_address,
-                ParameterGroupNumber.Address.GLOBAL,
-                timestamp,
-                data,
-                channel,
-            )
-        else:
-            self.__notify_subscribers(
-                mid.priority,
-                pgn_value,
-                mid.source_address,
-                dest_address,
-                timestamp,
-                data,
-                channel,
-            )
+        # Direct broadcast
+        # Removed peer to peer logic, we are interested in sniffing only
+        self.__notify_subscribers(
+            mid.priority,
+            pgn.value,
+            mid.source_address,
+            ParameterGroupNumber.Address.GLOBAL,
+            timestamp,
+            data,
+            channel,
+        )
```

### Comparing `can-j1939-ttpsc-1.0.2/j1939/memory_access.py` & `can-j1939-ttpsc-1.0.3/j1939/memory_access.py`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.2/j1939/message_id.py` & `can-j1939-ttpsc-1.0.3/j1939/message_id.py`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.2/j1939/name.py` & `can-j1939-ttpsc-1.0.3/j1939/name.py`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.2/j1939/parameter_group_number.py` & `can-j1939-ttpsc-1.0.3/j1939/parameter_group_number.py`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.2/setup.py` & `can-j1939-ttpsc-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.2/test/test_ca.py` & `can-j1939-ttpsc-1.0.3/test/test_ca.py`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.2/test/test_ecu.py` & `can-j1939-ttpsc-1.0.3/test/test_ecu.py`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.2/test/test_memory_access.py` & `can-j1939-ttpsc-1.0.3/test/test_memory_access.py`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.2/test_helpers/feeder.py` & `can-j1939-ttpsc-1.0.3/test_helpers/feeder.py`

 * *Files identical despite different names*


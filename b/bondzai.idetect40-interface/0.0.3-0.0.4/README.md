# Comparing `tmp/bondzai.idetect40-interface-0.0.3.tar.gz` & `tmp/bondzai.idetect40-interface-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.idetect40-interface-0.0.3.tar", last modified: Wed Apr 24 16:03:10 2024, max compression
+gzip compressed data, was "bondzai.idetect40-interface-0.0.4.tar", last modified: Wed Apr 24 18:01:32 2024, max compression
```

## Comparing `bondzai.idetect40-interface-0.0.3.tar` & `bondzai.idetect40-interface-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 16:03:10.488548 bondzai.idetect40-interface-0.0.3/
--rw-rw-rw-   0        0        0      547 2023-10-17 12:30:45.000000 bondzai.idetect40-interface-0.0.3/NOTICE
--rw-rw-rw-   0        0        0      805 2024-04-24 16:03:10.488548 bondzai.idetect40-interface-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      360 2024-04-24 10:47:45.000000 bondzai.idetect40-interface-0.0.3/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-24 16:03:10.471052 bondzai.idetect40-interface-0.0.3/bondzai/
-drwxrwxrwx   0        0        0        0 2024-04-24 16:03:10.479230 bondzai.idetect40-interface-0.0.3/bondzai/idetect40_interface/
--rw-rw-rw-   0        0        0       22 2024-04-24 16:02:46.000000 bondzai.idetect40-interface-0.0.3/bondzai/idetect40_interface/__init__.py
--rw-rw-rw-   0        0        0     2429 2024-04-24 10:29:44.000000 bondzai.idetect40-interface-0.0.3/bondzai/idetect40_interface/dict.py
--rw-rw-rw-   0        0        0    13464 2024-04-24 14:26:44.000000 bondzai.idetect40-interface-0.0.3/bondzai/idetect40_interface/exchange_table.py
--rw-rw-rw-   0        0        0    11553 2024-04-22 15:43:39.000000 bondzai.idetect40-interface-0.0.3/bondzai/idetect40_interface/socket.py
-drwxrwxrwx   0        0        0        0 2024-04-24 16:03:10.487485 bondzai.idetect40-interface-0.0.3/bondzai.idetect40_interface.egg-info/
--rw-rw-rw-   0        0        0      805 2024-04-24 16:03:10.000000 bondzai.idetect40-interface-0.0.3/bondzai.idetect40_interface.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      883 2024-04-24 16:03:10.000000 bondzai.idetect40-interface-0.0.3/bondzai.idetect40_interface.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 16:03:10.000000 bondzai.idetect40-interface-0.0.3/bondzai.idetect40_interface.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-24 16:03:10.000000 bondzai.idetect40-interface-0.0.3/bondzai.idetect40_interface.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0       28 2024-04-24 16:03:10.000000 bondzai.idetect40-interface-0.0.3/bondzai.idetect40_interface.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-24 16:03:10.000000 bondzai.idetect40-interface-0.0.3/bondzai.idetect40_interface.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-24 16:03:10.000000 bondzai.idetect40-interface-0.0.3/bondzai.idetect40_interface.egg-info/zip-safe
--rw-rw-rw-   0        0        0       71 2023-10-17 12:30:45.000000 bondzai.idetect40-interface-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      733 2024-04-24 16:03:10.490719 bondzai.idetect40-interface-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0       36 2023-10-17 12:30:45.000000 bondzai.idetect40-interface-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 16:03:10.480878 bondzai.idetect40-interface-0.0.3/tests/
--rw-rw-rw-   0        0        0     2383 2024-04-24 10:29:44.000000 bondzai.idetect40-interface-0.0.3/tests/test_dict.py
--rw-rw-rw-   0        0        0     4578 2024-04-24 14:26:44.000000 bondzai.idetect40-interface-0.0.3/tests/test_exchange_table.py
--rw-rw-rw-   0        0        0     5998 2024-04-24 10:33:37.000000 bondzai.idetect40-interface-0.0.3/tests/test_socket.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:01:32.140940 bondzai.idetect40-interface-0.0.4/
+-rw-rw-rw-   0        0        0      547 2023-10-17 12:30:45.000000 bondzai.idetect40-interface-0.0.4/NOTICE
+-rw-rw-rw-   0        0        0      805 2024-04-24 18:01:32.140940 bondzai.idetect40-interface-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2024-04-24 10:47:45.000000 bondzai.idetect40-interface-0.0.4/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-24 18:01:32.101301 bondzai.idetect40-interface-0.0.4/bondzai/
+drwxrwxrwx   0        0        0        0 2024-04-24 18:01:32.111033 bondzai.idetect40-interface-0.0.4/bondzai/idetect40_interface/
+-rw-rw-rw-   0        0        0       22 2024-04-24 18:01:24.000000 bondzai.idetect40-interface-0.0.4/bondzai/idetect40_interface/__init__.py
+-rw-rw-rw-   0        0        0    12704 2024-04-24 16:59:21.000000 bondzai.idetect40-interface-0.0.4/bondzai/idetect40_interface/exchange_table.py
+-rw-rw-rw-   0        0        0    11553 2024-04-22 15:43:39.000000 bondzai.idetect40-interface-0.0.4/bondzai/idetect40_interface/socket.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:01:32.139942 bondzai.idetect40-interface-0.0.4/bondzai.idetect40_interface.egg-info/
+-rw-rw-rw-   0        0        0      805 2024-04-24 18:01:32.000000 bondzai.idetect40-interface-0.0.4/bondzai.idetect40_interface.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      769 2024-04-24 18:01:32.000000 bondzai.idetect40-interface-0.0.4/bondzai.idetect40_interface.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 18:01:32.000000 bondzai.idetect40-interface-0.0.4/bondzai.idetect40_interface.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-24 18:01:32.000000 bondzai.idetect40-interface-0.0.4/bondzai.idetect40_interface.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0       28 2024-04-24 18:01:32.000000 bondzai.idetect40-interface-0.0.4/bondzai.idetect40_interface.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-24 18:01:32.000000 bondzai.idetect40-interface-0.0.4/bondzai.idetect40_interface.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-24 18:01:31.000000 bondzai.idetect40-interface-0.0.4/bondzai.idetect40_interface.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       71 2023-10-17 12:30:45.000000 bondzai.idetect40-interface-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      733 2024-04-24 18:01:32.144039 bondzai.idetect40-interface-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0       36 2023-10-17 12:30:45.000000 bondzai.idetect40-interface-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:01:32.116052 bondzai.idetect40-interface-0.0.4/tests/
+-rw-rw-rw-   0        0        0     4578 2024-04-24 14:26:44.000000 bondzai.idetect40-interface-0.0.4/tests/test_exchange_table.py
+-rw-rw-rw-   0        0        0     5998 2024-04-24 10:33:37.000000 bondzai.idetect40-interface-0.0.4/tests/test_socket.py
```

### Comparing `bondzai.idetect40-interface-0.0.3/NOTICE` & `bondzai.idetect40-interface-0.0.4/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.idetect40-interface-0.0.3/PKG-INFO` & `bondzai.idetect40-interface-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.idetect40-interface
-Version: 0.0.3
+Version: 0.0.4
 Summary: Bondzai iDetect 4.0 interface
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,idetect40
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.idetect40-interface-0.0.3/bondzai/idetect40_interface/exchange_table.py` & `bondzai.idetect40-interface-0.0.4/bondzai/idetect40_interface/exchange_table.py`

 * *Files 5% similar despite different names*

```diff
@@ -257,28 +257,14 @@
             elif attribute.type ==  AttributeDataType.FLOAT:
                 value_array = struct.pack('f',value)
             elif attribute.type ==  AttributeDataType.BOOL:
                 value_array = struct.pack("?", value)
             byte_array += bytearray(value_array) + int(0).to_bytes(byte_nb - len(value_array), byteorder="little")
         return byte_array
     
-    # def to_dict(self) -> dict:
-    #     input_table = {
-    #     "system": {"running": True, "process_ongoing": False, "heart_beat": False, 
-    #                "ack_result": True, "ack_exception": True},
-    #     "agents": {
-    #         1: {"active": True, "sources": {1: True, 2: False, 3: True, 4: False}},
-    #         2: {"active": True, "sources": {1: False, 2: False, 3: True, 4: False}},
-    #         3: {"active": False, "sources": {1: True, 2: True, 3: True, 4: False}},
-    #         4: {"active": False, "sources": {1: True, 2: False, 3: True, 4: True}}
-    #     },
-    #     "attributes": {"serial number": 12, "vehicule type": "abc", "temperature": 48.70000076293945, 
-    #                    "over pressure": False}
-    #     }
-    
     def __eq__(self, other):
         eq = self.system_running == other.system_running
         eq = eq and self.process_ongoing == other.process_ongoing
         eq = eq and self.heartbeat == other.heartbeat
         for agent_id, agent in self.agents.items():
             eq = eq and other.agents[agent_id] == agent
         for idx, attribute in enumerate(self.attributes):
```

### Comparing `bondzai.idetect40-interface-0.0.3/bondzai/idetect40_interface/socket.py` & `bondzai.idetect40-interface-0.0.4/bondzai/idetect40_interface/socket.py`

 * *Files identical despite different names*

### Comparing `bondzai.idetect40-interface-0.0.3/bondzai.idetect40_interface.egg-info/PKG-INFO` & `bondzai.idetect40-interface-0.0.4/bondzai.idetect40_interface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.idetect40-interface
-Version: 0.0.3
+Version: 0.0.4
 Summary: Bondzai iDetect 4.0 interface
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,idetect40
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.idetect40-interface-0.0.3/bondzai.idetect40_interface.egg-info/SOURCES.txt` & `bondzai.idetect40-interface-0.0.4/bondzai.idetect40_interface.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 NOTICE
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 ./bondzai/idetect40_interface/__init__.py
-./bondzai/idetect40_interface/dict.py
 ./bondzai/idetect40_interface/exchange_table.py
 ./bondzai/idetect40_interface/socket.py
-./tests/test_dict.py
 ./tests/test_exchange_table.py
 ./tests/test_socket.py
 bondzai.idetect40_interface.egg-info/PKG-INFO
 bondzai.idetect40_interface.egg-info/SOURCES.txt
 bondzai.idetect40_interface.egg-info/dependency_links.txt
 bondzai.idetect40_interface.egg-info/namespace_packages.txt
 bondzai.idetect40_interface.egg-info/requires.txt
 bondzai.idetect40_interface.egg-info/top_level.txt
 bondzai.idetect40_interface.egg-info/zip-safe
 bondzai/idetect40_interface/__init__.py
-bondzai/idetect40_interface/dict.py
 bondzai/idetect40_interface/exchange_table.py
 bondzai/idetect40_interface/socket.py
-tests/test_dict.py
 tests/test_exchange_table.py
 tests/test_socket.py
```

### Comparing `bondzai.idetect40-interface-0.0.3/setup.cfg` & `bondzai.idetect40-interface-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `bondzai.idetect40-interface-0.0.3/tests/test_exchange_table.py` & `bondzai.idetect40-interface-0.0.4/tests/test_exchange_table.py`

 * *Files identical despite different names*

### Comparing `bondzai.idetect40-interface-0.0.3/tests/test_socket.py` & `bondzai.idetect40-interface-0.0.4/tests/test_socket.py`

 * *Files identical despite different names*


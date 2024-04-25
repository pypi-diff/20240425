# Comparing `tmp/eve2cml-0.1.0b2.tar.gz` & `tmp/eve2cml-0.1.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eve2cml-0.1.0b2.tar", last modified: Thu Apr 11 10:50:48 2024, max compression
+gzip compressed data, was "eve2cml-0.1.0b4.tar", last modified: Thu Apr 25 07:03:29 2024, max compression
```

## Comparing `eve2cml-0.1.0b2.tar` & `eve2cml-0.1.0b4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1088 2024-03-12 12:50:05.022091 eve2cml-0.1.0b2/LICENSE
--rw-r--r--   0        0        0     6176 2024-04-11 10:48:57.012784 eve2cml-0.1.0b2/README.md
--rw-r--r--   0        0        0     1279 2024-04-11 10:50:48.724868 eve2cml-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-08 09:09:17.161399 eve2cml-0.1.0b2/src/eve2cml/__init__.py
--rw-r--r--   0        0        0       23 2024-04-11 10:50:48.720868 eve2cml-0.1.0b2/src/eve2cml/_version.py
--rw-r--r--   0        0        0      446 2024-03-12 10:40:45.713918 eve2cml-0.1.0b2/src/eve2cml/eve/__init__.py
--rw-r--r--   0        0        0      805 2024-03-08 12:06:50.314821 eve2cml-0.1.0b2/src/eve2cml/eve/config.py
--rw-r--r--   0        0        0      854 2024-03-08 12:06:46.366807 eve2cml-0.1.0b2/src/eve2cml/eve/configset.py
--rw-r--r--   0        0        0      367 2024-03-08 10:48:43.230941 eve2cml-0.1.0b2/src/eve2cml/eve/decode.py
--rw-r--r--   0        0        0     2534 2024-04-11 10:48:57.012784 eve2cml-0.1.0b2/src/eve2cml/eve/interface.py
--rw-r--r--   0        0        0     7874 2024-03-13 11:26:23.429205 eve2cml-0.1.0b2/src/eve2cml/eve/lab.py
--rw-r--r--   0        0        0     1179 2024-03-08 12:06:46.370807 eve2cml-0.1.0b2/src/eve2cml/eve/network.py
--rw-r--r--   0        0        0     6107 2024-04-11 10:48:57.012784 eve2cml-0.1.0b2/src/eve2cml/eve/node.py
--rw-r--r--   0        0        0     2107 2024-03-12 08:36:10.681337 eve2cml-0.1.0b2/src/eve2cml/eve/objects.py
--rw-r--r--   0        0        0     1077 2024-03-08 16:31:50.754881 eve2cml-0.1.0b2/src/eve2cml/eve/task.py
--rw-r--r--   0        0        0     9961 2024-03-12 08:40:57.396562 eve2cml-0.1.0b2/src/eve2cml/eve/textobject.py
--rw-r--r--   0        0        0      417 2024-03-08 14:08:19.532357 eve2cml-0.1.0b2/src/eve2cml/eve/topology.py
--rw-r--r--   0        0        0     1674 2024-03-12 07:59:30.375216 eve2cml-0.1.0b2/src/eve2cml/log.py
--rw-r--r--   0        0        0     7301 2024-03-13 10:42:16.954687 eve2cml-0.1.0b2/src/eve2cml/main.py
--rw-r--r--   0        0        0        0 2024-03-11 11:57:30.331045 eve2cml-0.1.0b2/src/eve2cml/map_data/__init__.py
--rw-r--r--   0        0        0     5803 2024-04-11 10:48:57.012784 eve2cml-0.1.0b2/src/eve2cml/map_data/default.yaml
--rw-r--r--   0        0        0     3275 2024-03-13 10:17:07.238473 eve2cml-0.1.0b2/src/eve2cml/mapper.py
--rw-r--r--   0        0        0        0 2024-03-05 09:48:58.793209 eve2cml-0.1.0b2/tests/__init__.py
--rw-r--r--   0        0        0      516 2024-03-13 11:35:39.763285 eve2cml-0.1.0b2/tests/requirements.txt
--rw-r--r--   0        0        0      447 2024-03-12 09:36:41.602131 eve2cml-0.1.0b2/tests/test_decode.py
--rw-r--r--   0        0        0     1845 2024-03-13 11:14:11.862480 eve2cml-0.1.0b2/tests/test_integration.py
--rw-r--r--   0        0        0     1058 2024-03-12 09:37:55.879401 eve2cml-0.1.0b2/tests/test_logging.py
--rw-r--r--   0        0        0     1043 2024-03-12 09:25:02.378964 eve2cml-0.1.0b2/tests/test_rgb_to_hex.py
--rw-r--r--   0        0        0     1961 2024-03-12 09:08:23.088301 eve2cml-0.1.0b2/tests/testdata/hub.unl
--rw-r--r--   0        0        0     1291 2024-03-13 11:25:57.501109 eve2cml-0.1.0b2/tests/testdata/nat.unl
--rw-r--r--   0        0        0     1036 2024-03-13 10:05:43.853858 eve2cml-0.1.0b2/tests/testdata/pnet.unl
--rw-r--r--   0        0        0     3405 2024-03-13 10:03:13.597125 eve2cml-0.1.0b2/tests/testdata/test.unl
--rw-r--r--   0        0        0     1494 2024-03-12 10:13:29.869315 eve2cml-0.1.0b2/tests/testdata/test.zip
--rw-r--r--   0        0        0     6512 1970-01-01 00:00:00.000000 eve2cml-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1088 2024-04-10 17:00:34.893286 eve2cml-0.1.0b4/LICENSE
+-rw-r--r--   0        0        0     8689 2024-04-25 06:54:18.415588 eve2cml-0.1.0b4/README.md
+-rw-r--r--   0        0        0     2087 2024-04-25 07:03:29.419555 eve2cml-0.1.0b4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-10 17:00:34.894803 eve2cml-0.1.0b4/src/eve2cml/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-25 07:03:29.416157 eve2cml-0.1.0b4/src/eve2cml/_version.py
+-rw-r--r--   0        0        0      446 2024-04-10 17:00:34.895071 eve2cml-0.1.0b4/src/eve2cml/eve/__init__.py
+-rw-r--r--   0        0        0      805 2024-04-10 17:00:34.895169 eve2cml-0.1.0b4/src/eve2cml/eve/config.py
+-rw-r--r--   0        0        0      854 2024-04-10 17:00:34.895270 eve2cml-0.1.0b4/src/eve2cml/eve/configset.py
+-rw-r--r--   0        0        0      367 2024-04-10 17:00:34.895363 eve2cml-0.1.0b4/src/eve2cml/eve/decode.py
+-rw-r--r--   0        0        0     2654 2024-04-25 06:54:18.416351 eve2cml-0.1.0b4/src/eve2cml/eve/interface.py
+-rw-r--r--   0        0        0     7874 2024-04-10 17:00:34.895592 eve2cml-0.1.0b4/src/eve2cml/eve/lab.py
+-rw-r--r--   0        0        0     1179 2024-04-10 17:00:34.895686 eve2cml-0.1.0b4/src/eve2cml/eve/network.py
+-rw-r--r--   0        0        0     6414 2024-04-25 06:54:18.416840 eve2cml-0.1.0b4/src/eve2cml/eve/node.py
+-rw-r--r--   0        0        0     2107 2024-04-10 17:00:34.895896 eve2cml-0.1.0b4/src/eve2cml/eve/objects.py
+-rw-r--r--   0        0        0     1077 2024-04-10 17:00:34.896005 eve2cml-0.1.0b4/src/eve2cml/eve/task.py
+-rw-r--r--   0        0        0     9961 2024-04-10 17:00:34.896137 eve2cml-0.1.0b4/src/eve2cml/eve/textobject.py
+-rw-r--r--   0        0        0      417 2024-04-10 17:00:34.896232 eve2cml-0.1.0b4/src/eve2cml/eve/topology.py
+-rw-r--r--   0        0        0     1674 2024-04-10 17:00:34.896327 eve2cml-0.1.0b4/src/eve2cml/log.py
+-rw-r--r--   0        0        0     7301 2024-04-10 17:00:34.896448 eve2cml-0.1.0b4/src/eve2cml/main.py
+-rw-r--r--   0        0        0        0 2024-04-10 17:00:34.896546 eve2cml-0.1.0b4/src/eve2cml/map_data/__init__.py
+-rw-r--r--   0        0        0     5803 2024-04-11 11:06:40.393445 eve2cml-0.1.0b4/src/eve2cml/map_data/default.yaml
+-rw-r--r--   0        0        0     3374 2024-04-23 09:56:23.970162 eve2cml-0.1.0b4/src/eve2cml/mapper.py
+-rw-r--r--   0        0        0        0 2024-04-10 17:00:34.896861 eve2cml-0.1.0b4/tests/__init__.py
+-rw-r--r--   0        0        0      516 2024-04-23 09:56:23.970483 eve2cml-0.1.0b4/tests/requirements.txt
+-rw-r--r--   0        0        0      447 2024-04-10 17:00:34.897052 eve2cml-0.1.0b4/tests/test_decode.py
+-rw-r--r--   0        0        0     1845 2024-04-10 17:00:34.897150 eve2cml-0.1.0b4/tests/test_integration.py
+-rw-r--r--   0        0        0     1058 2024-04-10 17:00:34.897235 eve2cml-0.1.0b4/tests/test_logging.py
+-rw-r--r--   0        0        0     1043 2024-04-10 17:00:34.897327 eve2cml-0.1.0b4/tests/test_rgb_to_hex.py
+-rw-r--r--   0        0        0     1961 2024-04-10 17:00:34.897462 eve2cml-0.1.0b4/tests/testdata/hub.unl
+-rw-r--r--   0        0        0     1291 2024-04-10 17:00:34.897560 eve2cml-0.1.0b4/tests/testdata/nat.unl
+-rw-r--r--   0        0        0     1036 2024-04-10 17:00:34.897640 eve2cml-0.1.0b4/tests/testdata/pnet.unl
+-rw-r--r--   0        0        0     3405 2024-04-10 17:00:34.897720 eve2cml-0.1.0b4/tests/testdata/test.unl
+-rw-r--r--   0        0        0     1494 2024-04-10 17:00:34.897807 eve2cml-0.1.0b4/tests/testdata/test.zip
+-rw-r--r--   0        0        0     9849 1970-01-01 00:00:00.000000 eve2cml-0.1.0b4/PKG-INFO
```

### Comparing `eve2cml-0.1.0b2/LICENSE` & `eve2cml-0.1.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b2/pyproject.toml` & `eve2cml-0.1.0b4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -7,19 +7,44 @@
 ]
 dependencies = [
     "beautifulsoup4>=4.12.3",
     "pyyaml>=6.0.1",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "0.1.0b2"
+keywords = [
+    "automation",
+    "tools",
+    "simulation",
+    "virtualization",
+    "network-programming",
+]
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Environment :: Console",
+    "Intended Audience :: Telecommunications Industry",
+    "Topic :: Internet",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+]
+version = "0.1.0b4"
 
 [project.license]
 text = "MIT"
 
+[project.urls]
+Homepage = "https://developer.cisco.com/modeling-labs"
+Repository = "https://github.com/ciscodevnet/eve2cml"
+Issues = "https://github.com/ciscodevnet/eve2cml/issues"
+Changelog = "https://github.com/ciscodevnet/eve2cml/blob/master/CHANGELOG.md"
+
 [project.scripts]
 eve2cml = "eve2cml.main:main"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
```

### Comparing `eve2cml-0.1.0b2/src/eve2cml/eve/config.py` & `eve2cml-0.1.0b4/src/eve2cml/eve/config.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b2/src/eve2cml/eve/configset.py` & `eve2cml-0.1.0b4/src/eve2cml/eve/configset.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b2/src/eve2cml/eve/interface.py` & `eve2cml-0.1.0b4/src/eve2cml/eve/interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,40 +38,43 @@
     def __str__(self):
         return f"ID: {self.id}, Name: {self.name}, Type: {self.obj_type}, NetID: {self.network_id}"
 
     def __repr__(self):
         return f"{self.__class__.__name__}(id={self.id}, slot={self.slot})"
 
     def as_cml_dict(self, idx, node_def, lab):
+        # can likely remove the idx arg as the id should match the idx!
+        assert self.id == idx
         return {
+            # "id": f"i{self.id}",
             "id": f"i{idx}",
             "label": lab.mapper.cml_iface_label(self.slot, node_def, self.name),
             "slot": self.slot,
             "type": "physical",
         }
 
     @classmethod
     def parse(
         cls, node_id: int, obj_type: str, elem: List[Element]
     ) -> List["Interface"]:
         # special treatment for slots when type is IOL
         no_iol = obj_type != "iol"
 
         interfaces: List[Interface] = []
-        for idx, interface_elem in enumerate(elem):
+        for interface_elem in elem:
             id = int(interface_elem.attrib.get("id", "unknown"))
             interface = Interface(
                 id=id,
                 name=interface_elem.attrib.get("name", "unknown"),
                 obj_type=interface_elem.attrib.get("type", "unknown"),
                 network_id=int(interface_elem.attrib.get("network_id", 0)),
                 labelpos=interface_elem.attrib.get("labelpos", ""),
                 curviness=interface_elem.attrib.get("curviness", ""),
                 beziercurviness=interface_elem.attrib.get("beziercurviness", ""),
                 midpoint=interface_elem.attrib.get("midpoint", ""),
                 srcpos=interface_elem.attrib.get("srcpos", ""),
                 dstpos=interface_elem.attrib.get("dstpos", ""),
                 node_id=node_id,
-                slot=idx if no_iol else ((id & 0xF) * 4) + (id >> 4),
+                slot=id if no_iol else ((id & 0xF) * 4) + (id >> 4),
             )
             interfaces.append(interface)
         return interfaces
```

### Comparing `eve2cml-0.1.0b2/src/eve2cml/eve/lab.py` & `eve2cml-0.1.0b4/src/eve2cml/eve/lab.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b2/src/eve2cml/eve/network.py` & `eve2cml-0.1.0b4/src/eve2cml/eve/network.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b2/src/eve2cml/eve/node.py` & `eve2cml-0.1.0b4/src/eve2cml/eve/node.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,32 +67,40 @@
     def __str__(self):
         return f"ID: {self.id}, Name: {self.name}, Type: {self.obj_type}, X: {self.left}, Y: {self.top}, Template: {self.template}, Image: {self.image}, Ethernet: {self.ethernet}"
 
     def as_cml_dict(self, node_id: int, lab: "Lab"):
         nd_map = lab.mapper.node_def(self.obj_type, self.template, self.image)
 
         temp_list: List[Interface] = []
-        prev = 0
+        prev_idx = 0
+        prev_slot = 0
+        _LOGGER.debug(self.interfaces)
         for idx, iface in enumerate(self.interfaces):
-            delta = iface.slot - prev
+            delta = iface.slot - prev_slot
             _LOGGER.debug(
-                "idx, slot, prev, delta %d/%d/%d/%d", idx, iface.slot, prev, delta
+                "idx, slot, prev, delta %d/%d/%d/%d", idx, iface.slot, prev_slot, delta
             )
             for idx2 in range(delta):
+                _LOGGER.debug(
+                    "prepending filler interface id %d/%d", prev_idx, prev_slot + idx2
+                )
                 temp_list.append(
                     Interface(
-                        id=idx + idx2,
+                        id=prev_idx,
                         obj_type=self.obj_type,
                         network_id=999999,
                         name="filler",
-                        slot=prev + idx2,
+                        slot=prev_slot + idx2,
                     )
                 )
+                prev_idx += 1
+            iface.id = prev_idx
             temp_list.append(iface)
-            prev = iface.slot + 1
+            prev_slot = iface.slot + 1
+            prev_idx += 1
 
         _LOGGER.debug("list %s", temp_list)
 
         iface_count = len(temp_list)
         iface_diff = int(self.ethernet) - iface_count
         if iface_diff > 0:
             _LOGGER.info(
```

### Comparing `eve2cml-0.1.0b2/src/eve2cml/eve/objects.py` & `eve2cml-0.1.0b4/src/eve2cml/eve/objects.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b2/src/eve2cml/eve/task.py` & `eve2cml-0.1.0b4/src/eve2cml/eve/task.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b2/src/eve2cml/eve/textobject.py` & `eve2cml-0.1.0b4/src/eve2cml/eve/textobject.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b2/src/eve2cml/log.py` & `eve2cml-0.1.0b4/src/eve2cml/log.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b2/src/eve2cml/main.py` & `eve2cml-0.1.0b4/src/eve2cml/main.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b2/src/eve2cml/map_data/default.yaml` & `eve2cml-0.1.0b4/src/eve2cml/map_data/default.yaml`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b2/src/eve2cml/mapper.py` & `eve2cml-0.1.0b4/src/eve2cml/mapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -73,24 +73,25 @@
         return mapper
 
     def node_def(self, obj_type: str, template: str, image: str) -> CMLdef:
         lookup = f"{obj_type}:{template}:{image}"
         found = self.map.get(lookup)
         if not found:
             # special case for non-template images like IOL or Docker
-            if image and template == obj_type:
-                for key, cmldef in self.map.items():
-                    if lookup.startswith(key):
-                        return cmldef
-            found = self.map.get(f"{obj_type}:{template}")
-            if not found:
-                _LOGGER.warning(
-                    "Unmapped node type %s %s %s", obj_type, template, image
-                )
-                return CMLdef(self.unknown_type, None, True)
+            longest_prefix = ""
+            longest_cmldef = None
+            for key, cmldef in self.map.items():
+                if lookup.startswith(key) and len(key) > len(longest_prefix):
+                    longest_prefix = key
+                    longest_cmldef = cmldef
+            if longest_cmldef:
+                _LOGGER.info("mapped node type %s", longest_cmldef)
+                return longest_cmldef
+            _LOGGER.warning("Unmapped node type %s %s %s", obj_type, template, image)
+            return CMLdef(self.unknown_type, None, True)
         return found
 
     def cml_iface_label(self, slot: int, node_def: str, label: str) -> str:
         interfaces = self.interface_lists.get(node_def)
         if interfaces is None:
             _LOGGER.warning("No mapping: %s %d", node_def, slot)
             return label
```

### Comparing `eve2cml-0.1.0b2/tests/requirements.txt` & `eve2cml-0.1.0b4/tests/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 exceptiongroup==1.2.0; python_version < "3.11"
 iniconfig==2.0.0
 mypy==1.9.0
 mypy-extensions==1.0.0
 packaging==23.2
 pluggy==1.4.0
 pytest==8.1.1
-pytest-cov==4.1.0
+pytest-cov==5.0.0
 pyyaml==6.0.1
-ruff==0.3.2
+ruff==0.4.1
 soupsieve==2.5
 tomli==2.0.1; python_version < "3.11"
 types-beautifulsoup4==4.12.0.20240229
 types-html5lib==1.1.11.20240228
 types-pyyaml==6.0.12.20240311
 typing-extensions==4.10.0
```

### Comparing `eve2cml-0.1.0b2/tests/test_integration.py` & `eve2cml-0.1.0b4/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b2/tests/test_logging.py` & `eve2cml-0.1.0b4/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b2/tests/test_rgb_to_hex.py` & `eve2cml-0.1.0b4/tests/test_rgb_to_hex.py`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b2/tests/testdata/hub.unl` & `eve2cml-0.1.0b4/tests/testdata/hub.unl`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b2/tests/testdata/nat.unl` & `eve2cml-0.1.0b4/tests/testdata/nat.unl`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b2/tests/testdata/pnet.unl` & `eve2cml-0.1.0b4/tests/testdata/pnet.unl`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b2/tests/testdata/test.unl` & `eve2cml-0.1.0b4/tests/testdata/test.unl`

 * *Files identical despite different names*

### Comparing `eve2cml-0.1.0b2/tests/testdata/test.zip` & `eve2cml-0.1.0b4/tests/testdata/test.zip`

 * *Files identical despite different names*


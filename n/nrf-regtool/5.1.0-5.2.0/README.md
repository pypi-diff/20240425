# Comparing `tmp/nrf-regtool-5.1.0.tar.gz` & `tmp/nrf_regtool-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrf-regtool-5.1.0.tar", last modified: Tue Feb 27 12:42:46 2024, max compression
+gzip compressed data, was "nrf_regtool-5.2.0.tar", last modified: Thu Apr 25 14:51:38 2024, max compression
```

## Comparing `nrf-regtool-5.1.0.tar` & `nrf_regtool-5.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 joni-l    (1000) joni-l    (1000)        0 2024-02-27 12:42:46.485592 nrf-regtool-5.1.0/
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)    11358 2022-12-07 09:09:13.000000 nrf-regtool-5.1.0/LICENSE
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)    13630 2024-02-27 12:42:46.485592 nrf-regtool-5.1.0/PKG-INFO
-drwxr-xr-x   0 joni-l    (1000) joni-l    (1000)        0 2024-02-27 12:42:46.485592 nrf-regtool-5.1.0/nrf_regtool.egg-info/
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)    13630 2024-02-27 12:42:46.000000 nrf-regtool-5.1.0/nrf_regtool.egg-info/PKG-INFO
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)      520 2024-02-27 12:42:46.000000 nrf-regtool-5.1.0/nrf_regtool.egg-info/SOURCES.txt
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)        1 2024-02-27 12:42:46.000000 nrf-regtool-5.1.0/nrf_regtool.egg-info/dependency_links.txt
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)       65 2024-02-27 12:42:46.000000 nrf-regtool-5.1.0/nrf_regtool.egg-info/entry_points.txt
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)       74 2024-02-27 12:42:46.000000 nrf-regtool-5.1.0/nrf_regtool.egg-info/requires.txt
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)       11 2024-02-27 12:42:46.000000 nrf-regtool-5.1.0/nrf_regtool.egg-info/top_level.txt
-drwxr-xr-x   0 joni-l    (1000) joni-l    (1000)        0 2024-02-27 12:42:46.485592 nrf-regtool-5.1.0/nrfregtool/
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)     1565 2024-02-27 12:19:53.000000 nrf-regtool-5.1.0/nrfregtool/__init__.py
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)      626 2023-06-15 07:04:14.000000 nrf-regtool-5.1.0/nrfregtool/__main__.py
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)    17162 2024-02-27 12:19:53.000000 nrf-regtool-5.1.0/nrfregtool/bicr.py
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)    18606 2024-02-27 12:19:53.000000 nrf-regtool-5.1.0/nrfregtool/cli.py
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)     8302 2024-02-27 12:19:53.000000 nrf-regtool-5.1.0/nrfregtool/common.py
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)    25372 2024-02-27 12:19:53.000000 nrf-regtool-5.1.0/nrfregtool/core.py
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)      906 2024-02-15 12:17:33.000000 nrf-regtool-5.1.0/nrfregtool/main.py
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)    15680 2024-02-27 12:19:53.000000 nrf-regtool-5.1.0/nrfregtool/parsed_dt.py
-drwxr-xr-x   0 joni-l    (1000) joni-l    (1000)        0 2024-02-27 12:42:46.485592 nrf-regtool-5.1.0/nrfregtool/resources/
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)        0 2024-02-15 12:17:33.000000 nrf-regtool-5.1.0/nrfregtool/resources/__init__.py
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)    24086 2023-06-14 07:15:13.000000 nrf-regtool-5.1.0/nrfregtool/resources/uicrextended.svd
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)    73321 2024-02-27 12:19:53.000000 nrf-regtool-5.1.0/nrfregtool/uicr.py
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)      987 2024-02-27 12:19:53.000000 nrf-regtool-5.1.0/pyproject.toml
-drwxr-xr-x   0 joni-l    (1000) joni-l    (1000)        0 2024-02-27 12:42:46.485592 nrf-regtool-5.1.0/scripts/
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)       74 2024-02-22 15:16:08.000000 nrf-regtool-5.1.0/scripts/requirements-base.txt
--rw-r--r--   0 joni-l    (1000) joni-l    (1000)       38 2024-02-27 12:42:46.485592 nrf-regtool-5.1.0/setup.cfg
+drwxrwxr-x   0 local-joni  (1000) local-joni  (1000)        0 2024-04-25 14:51:38.461704 nrf_regtool-5.2.0/
+-rw-rw-r--   0 local-joni  (1000) local-joni  (1000)    11358 2024-04-25 14:47:07.000000 nrf_regtool-5.2.0/LICENSE
+-rw-r--r--   0 local-joni  (1000) local-joni  (1000)    13630 2024-04-25 14:51:38.461704 nrf_regtool-5.2.0/PKG-INFO
+drwxrwxr-x   0 local-joni  (1000) local-joni  (1000)        0 2024-04-25 14:51:38.461704 nrf_regtool-5.2.0/nrf_regtool.egg-info/
+-rw-r--r--   0 local-joni  (1000) local-joni  (1000)    13630 2024-04-25 14:51:38.000000 nrf_regtool-5.2.0/nrf_regtool.egg-info/PKG-INFO
+-rw-rw-r--   0 local-joni  (1000) local-joni  (1000)      520 2024-04-25 14:51:38.000000 nrf_regtool-5.2.0/nrf_regtool.egg-info/SOURCES.txt
+-rw-rw-r--   0 local-joni  (1000) local-joni  (1000)        1 2024-04-25 14:51:38.000000 nrf_regtool-5.2.0/nrf_regtool.egg-info/dependency_links.txt
+-rw-rw-r--   0 local-joni  (1000) local-joni  (1000)       65 2024-04-25 14:51:38.000000 nrf_regtool-5.2.0/nrf_regtool.egg-info/entry_points.txt
+-rw-rw-r--   0 local-joni  (1000) local-joni  (1000)       74 2024-04-25 14:51:38.000000 nrf_regtool-5.2.0/nrf_regtool.egg-info/requires.txt
+-rw-rw-r--   0 local-joni  (1000) local-joni  (1000)       11 2024-04-25 14:51:38.000000 nrf_regtool-5.2.0/nrf_regtool.egg-info/top_level.txt
+drwxrwxr-x   0 local-joni  (1000) local-joni  (1000)        0 2024-04-25 14:51:38.461704 nrf_regtool-5.2.0/nrfregtool/
+-rw-rw-r--   0 local-joni  (1000) local-joni  (1000)     1565 2024-04-25 14:49:49.000000 nrf_regtool-5.2.0/nrfregtool/__init__.py
+-rw-rw-r--   0 local-joni  (1000) local-joni  (1000)      626 2024-04-25 14:47:07.000000 nrf_regtool-5.2.0/nrfregtool/__main__.py
+-rw-rw-r--   0 local-joni  (1000) local-joni  (1000)    17162 2024-04-25 14:49:49.000000 nrf_regtool-5.2.0/nrfregtool/bicr.py
+-rw-rw-r--   0 local-joni  (1000) local-joni  (1000)    18606 2024-04-25 14:49:49.000000 nrf_regtool-5.2.0/nrfregtool/cli.py
+-rw-rw-r--   0 local-joni  (1000) local-joni  (1000)     9370 2024-04-25 14:49:49.000000 nrf_regtool-5.2.0/nrfregtool/common.py
+-rw-rw-r--   0 local-joni  (1000) local-joni  (1000)    25372 2024-04-25 14:49:49.000000 nrf_regtool-5.2.0/nrfregtool/core.py
+-rw-rw-r--   0 local-joni  (1000) local-joni  (1000)      906 2024-04-25 14:49:49.000000 nrf_regtool-5.2.0/nrfregtool/main.py
+-rw-rw-r--   0 local-joni  (1000) local-joni  (1000)    15737 2024-04-25 14:49:49.000000 nrf_regtool-5.2.0/nrfregtool/parsed_dt.py
+drwxrwxr-x   0 local-joni  (1000) local-joni  (1000)        0 2024-04-25 14:51:38.461704 nrf_regtool-5.2.0/nrfregtool/resources/
+-rw-rw-r--   0 local-joni  (1000) local-joni  (1000)        0 2024-04-25 14:47:07.000000 nrf_regtool-5.2.0/nrfregtool/resources/__init__.py
+-rw-rw-r--   0 local-joni  (1000) local-joni  (1000)    24086 2024-04-25 14:47:07.000000 nrf_regtool-5.2.0/nrfregtool/resources/uicrextended.svd
+-rw-rw-r--   0 local-joni  (1000) local-joni  (1000)    72635 2024-04-25 14:49:49.000000 nrf_regtool-5.2.0/nrfregtool/uicr.py
+-rw-rw-r--   0 local-joni  (1000) local-joni  (1000)      987 2024-04-25 14:49:49.000000 nrf_regtool-5.2.0/pyproject.toml
+drwxrwxr-x   0 local-joni  (1000) local-joni  (1000)        0 2024-04-25 14:51:38.461704 nrf_regtool-5.2.0/scripts/
+-rw-rw-r--   0 local-joni  (1000) local-joni  (1000)       74 2024-04-25 14:47:07.000000 nrf_regtool-5.2.0/scripts/requirements-base.txt
+-rw-rw-r--   0 local-joni  (1000) local-joni  (1000)       38 2024-04-25 14:51:38.461704 nrf_regtool-5.2.0/setup.cfg
```

### Comparing `nrf-regtool-5.1.0/LICENSE` & `nrf_regtool-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nrf-regtool-5.1.0/PKG-INFO` & `nrf_regtool-5.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrf-regtool
-Version: 5.1.0
+Version: 5.2.0
 Summary: Generate files of register content for memory-mapped peripherals.
 Author: Nordic Semiconductor ASA
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `nrf-regtool-5.1.0/nrf_regtool.egg-info/PKG-INFO` & `nrf_regtool-5.2.0/nrf_regtool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrf-regtool
-Version: 5.1.0
+Version: 5.2.0
 Summary: Generate files of register content for memory-mapped peripherals.
 Author: Nordic Semiconductor ASA
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `nrf-regtool-5.1.0/nrf_regtool.egg-info/SOURCES.txt` & `nrf_regtool-5.2.0/nrf_regtool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nrf-regtool-5.1.0/nrfregtool/__init__.py` & `nrf_regtool-5.2.0/nrfregtool/__init__.py`

 * *Files identical despite different names*

### Comparing `nrf-regtool-5.1.0/nrfregtool/__main__.py` & `nrf_regtool-5.2.0/nrfregtool/__main__.py`

 * *Files identical despite different names*

### Comparing `nrf-regtool-5.1.0/nrfregtool/bicr.py` & `nrf_regtool-5.2.0/nrfregtool/bicr.py`

 * *Files identical despite different names*

### Comparing `nrf-regtool-5.1.0/nrfregtool/cli.py` & `nrf_regtool-5.2.0/nrfregtool/cli.py`

 * *Files identical despite different names*

### Comparing `nrf-regtool-5.1.0/nrfregtool/common.py` & `nrf_regtool-5.2.0/nrfregtool/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -140,14 +140,23 @@
             DomainID.SECURE.value: cls.SECURE,
             DomainID.APPLICATION.value: cls.APPLICATION,
             DomainID.RADIOCORE.value: cls.RADIOCORE,
             DomainID.GLOBAL_FAST.value: cls.SYSCTRL,
         }
         return domain_owner.get(int(domain))
 
+    @classmethod
+    def from_processor(cls, processor: Union[ProcessorID, int]):
+        """
+        Helper method to extract an enumerated owner ID from a processor ID.
+        """
+        if (domain := DomainID.from_processor(processor)) is not None:
+            return cls.from_domain(domain)
+        return None
+
 
 @enum.unique
 class ProcessorID(_HaltiumID):
     """
     Enumeration of processor IDs in haltium products.
     """
 
@@ -158,26 +167,49 @@
     SYSCTRL = 12
     PPR = 13
     FLPR = 14
 
     @classmethod
     def from_domain(cls, domain: DomainID):
         """
-        Helper method to extract an enumerated domain ID from a processor ID.
+        Helper method to extract an enumerated processor ID from a domain ID.
         """
         domain_processor = {
             DomainID.SECURE.value: cls.SECURE,
             DomainID.APPLICATION.value: cls.APPLICATION,
             DomainID.RADIOCORE.value: cls.RADIOCORE,
             DomainID.GLOBAL_FAST.value: cls.SYSCTRL,
             DomainID.GLOBAL_SLOW.value: cls.PPR,
             DomainID.GLOBAL_.value: cls.FLPR,
         }
         return domain_processor.get(int(domain))
 
+    @classmethod
+    def from_nodelabels(cls, labels: List[str]):
+        """
+        Helper method to extract an enumerated processor ID from a list of devicetree nodelabels.
+        """
+        substring_processor = {
+            "cpusec": cls.SECURE,
+            "cpuapp": cls.APPLICATION,
+            "cpurad": cls.RADIOCORE,
+            "cpubbpr": cls.BBPR,
+            "cpusys": cls.SYSCTRL,
+            "cpuppr": cls.PPR,
+            "cpuflpr": cls.FLPR,
+        }
+        processors = {
+            processor_id
+            for substring, processor_id in substring_processor.items()
+            if any(substring in label for label in labels)
+        }
+        if len(processors) == 1:
+            return processors.pop()
+        return None
+
 
 class Record(Dict[str, Dict[str, Union[str, int]]]):
     """
     A transcript of the contents of any number of registers and their fields.
     A basic Record is one that is not complete with register instance information, while a complete
     Record is one that also carries instance information.
```

### Comparing `nrf-regtool-5.1.0/nrfregtool/core.py` & `nrf_regtool-5.2.0/nrfregtool/core.py`

 * *Files identical despite different names*

### Comparing `nrf-regtool-5.1.0/nrfregtool/main.py` & `nrf_regtool-5.2.0/nrfregtool/main.py`

 * *Files identical despite different names*

### Comparing `nrf-regtool-5.1.0/nrfregtool/parsed_dt.py` & `nrf_regtool-5.2.0/nrfregtool/parsed_dt.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,21 +360,25 @@
     """
     Get processor information from a domain's devicetree.
 
     :param devicetree: Devicetree
 
     :return: Tuple of processor information of the devicetree's domain
     """
-    cpus = devicetree.get_node("/cpus")
-    if len(cpus.children) != 1:
+    cpus = [
+        node
+        for node in devicetree.get_node("/cpus").children.values()
+        if node.name.startswith("cpu@")
+    ]
+    if len(cpus) != 1:
         raise RuntimeError(
-            f"Expected exactly 1 'cpu' node, but devicetree contained {len(cpus.children)} nodes"
+            f"Expected exactly 1 'cpu' node, but devicetree contained {len(cpus)} nodes"
         )
 
-    cpu = list(cpus.children.values())[0]
+    cpu = cpus[0]
     try:
         compatible = cpu.compats[0]
     except IndexError:
         raise RuntimeError("Devicetree 'cpu' node has no compatible")
 
     processor_id = ProcessorID.from_value(cpu.regs[0].addr)
     if processor_id is None:
```

### Comparing `nrf-regtool-5.1.0/nrfregtool/resources/uicrextended.svd` & `nrf_regtool-5.2.0/nrfregtool/resources/uicrextended.svd`

 * *Files identical despite different names*

### Comparing `nrf-regtool-5.1.0/nrfregtool/uicr.py` & `nrf_regtool-5.2.0/nrfregtool/uicr.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,22 @@
         "nordic,nrf-bellboard",
         [
             DomainID.GLOBAL_FAST,
             DomainID.APPLICATION,
             DomainID.RADIOCORE,
         ],
     ),
-    ("nordic,nrf-vevif", [DomainID.GLOBAL_FAST]),
+    (
+        "nordic,nrf-vevif",
+        [
+            DomainID.GLOBAL_FAST,
+            DomainID.APPLICATION,
+            DomainID.RADIOCORE,
+        ],
+    ),
     ("nordic,nrf-clic", [DomainID.GLOBAL_FAST]),
     (
         "nordic,nrf-gpio",
         [
             DomainID.GLOBAL_FAST,
             DomainID.APPLICATION,
             DomainID.RADIOCORE,
@@ -1263,26 +1270,16 @@
     :param default: Processor ID of the domain CPU, which is used by default
     """
 
     current_processor_id = None
 
     for irq in node.node.interrupts:
         irq_ctrl = ParsedDTNode(irq.controller)
-        if irq_ctrl.compatibles_contain(ResourceCompatible.CLIC.value):
-            # Interrupt controller is a VPR CLIC.
-            # Map the interrupt to the associated VPR coprocessor.
-            vpr = irq_ctrl.parent
-            try:
-                processor_id = ProcessorID(vpr.properties.get_val("cpu"))
-            except ValueError:
-                raise RuntimeError(
-                    f"Missing or invalid 'cpu' property in node {vpr.path}"
-                )
-        else:
-            # Assume the interrupt will be mapped to the domain processor.
+        processor_id = ProcessorID.from_nodelabels(irq_ctrl.labels)
+        if processor_id is None:
             processor_id = default
 
         if current_processor_id is None:
             current_processor_id = processor_id
         elif current_processor_id != processor_id:
             raise RuntimeError(
                 f"Peripheral node {node.path} has IRQs mapped to multiple processors "
@@ -1817,28 +1814,21 @@
     Get the owner ID associated with the remote mbox.
 
     :param mbox_nodes: Dictionary of mbox nodes
 
     :return: remote Owner ID.
     """
 
-    if any("cpusec" in label for label in mbox_nodes["tx"].labels):
-        domain_id = DomainID.SECURE
-    elif any("cpuapp" in label for label in mbox_nodes["tx"].labels):
-        domain_id = DomainID.APPLICATION
-    elif any("cpurad" in label for label in mbox_nodes["tx"].labels):
-        domain_id = DomainID.RADIOCORE
-    elif any("cpuppr" in label for label in mbox_nodes["tx"].labels):
-        domain_id = DomainID.GLOBAL_SLOW
-    else:
+    processor_id = ProcessorID.from_nodelabels(mbox_nodes["tx"].labels)
+    if processor_id is None:
         raise RuntimeError(
-            f"Unable to determine domain for {mbox_nodes['tx'].path}, {mbox_nodes['tx'].labels}"
+            f"Unable to determine processor for {mbox_nodes['tx'].path}, {mbox_nodes['tx'].labels}"
         )
 
-    return OwnerID.from_domain(domain_id)
+    return OwnerID.from_processor(processor_id)
 
 
 def _shmem_is_secure(shmem_node: ParsedDTNode) -> bool:
     """
     Check if a memory node is secure. That is, it has an ancestor
     with owned memory compatible and perm-secure property.
     It stops at the first node with compatible owned memory.
```

### Comparing `nrf-regtool-5.1.0/pyproject.toml` & `nrf_regtool-5.2.0/pyproject.toml`

 * *Files identical despite different names*


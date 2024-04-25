# Comparing `tmp/vmware-cloud-foundation-health-monitoring-2.1.1.1001.tar.gz` & `tmp/vmware_cloud_foundation_health_monitoring-2.1.2.1001.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmware-cloud-foundation-health-monitoring-2.1.1.1001.tar", last modified: Thu Apr  4 18:46:16 2024, max compression
+gzip compressed data, was "vmware_cloud_foundation_health_monitoring-2.1.2.1001.tar", last modified: Thu Apr 25 19:11:12 2024, max compression
```

## Comparing `vmware-cloud-foundation-health-monitoring-2.1.1.1001.tar` & `vmware_cloud_foundation_health_monitoring-2.1.2.1001.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 18:46:16.717364 vmware-cloud-foundation-health-monitoring-2.1.1.1001/
--rw-rw-rw-   0        0        0     1368 2024-04-04 18:15:00.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/LICENSE
--rw-rw-rw-   0        0        0      434 2024-04-04 18:15:00.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/NOTICE
--rw-rw-rw-   0        0        0    19547 2024-04-04 18:46:16.717364 vmware-cloud-foundation-health-monitoring-2.1.1.1001/PKG-INFO
--rw-rw-rw-   0        0        0    18670 2024-04-04 18:35:16.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/README.md
--rw-rw-rw-   0        0        0       86 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/pyproject.toml
--rw-rw-rw-   0        0        0     1078 2024-04-04 18:46:16.732992 vmware-cloud-foundation-health-monitoring-2.1.1.1001/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-04 18:46:16.561116 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/
-drwxrwxrwx   0        0        0        0 2024-04-04 18:46:16.576737 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/artifacts/
--rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/artifacts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 18:46:16.592365 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/artifacts/vSAN/
--rw-rw-rw-   0        0        0   160429 2024-01-24 16:35:38.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/artifacts/vSAN/Alert_Definitions.xml
--rw-rw-rw-   0        0        0    31502 2024-04-04 18:39:57.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/artifacts/vSAN/Dashboards.zip
--rw-rw-rw-   0        0        0    17918 2024-04-04 18:37:03.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/artifacts/vSAN/Supermetrics.json
--rw-rw-rw-   0        0        0    18400 2024-04-04 18:22:11.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/artifacts/vSAN/Views.zip
--rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/artifacts/vSAN/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 18:46:16.592365 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/examples/
--rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/examples/__init__.py
--rwxrwxrwx   0        0        0       55 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/examples/run_send-data-to-vrops.bat
-drwxrwxrwx   0        0        0        0 2024-04-04 18:46:16.654866 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/
--rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/__init__.py
--rw-rw-rw-   0        0        0     2693 2024-01-10 20:39:28.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/encrypt-passwords.py
-drwxrwxrwx   0        0        0        0 2024-04-04 18:46:16.654866 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/encrypted_files/
--rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/encrypted_files/__init__.py
--rw-rw-rw-   0        0        0     1655 2024-01-10 20:39:28.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/env.json
--rw-rw-rw-   0        0        0   129113 2024-01-24 16:35:38.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/notifications-template.json
--rw-rw-rw-   0        0        0     4381 2024-01-10 20:39:28.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/notifications.py
--rw-rw-rw-   0        0        0    82701 2024-04-04 18:17:29.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/send-data-to-vrops.py
-drwxrwxrwx   0        0        0        0 2024-04-04 18:46:16.686115 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/utils/
--rw-rw-rw-   0        0        0     5364 2024-01-24 16:35:38.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/utils/FolderUtility.py
--rw-rw-rw-   0        0        0     3929 2024-01-24 16:35:38.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/utils/LogUtility.py
--rw-rw-rw-   0        0        0     2528 2024-01-24 16:35:38.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/utils/PSUtility.py
--rw-rw-rw-   0        0        0     6886 2024-01-24 16:35:38.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/utils/SosRest.py
--rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 18:46:16.717364 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/vmware_cloud_foundation_health_monitoring.egg-info/
--rw-rw-rw-   0        0        0    19547 2024-04-04 18:46:16.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/vmware_cloud_foundation_health_monitoring.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1002 2024-04-04 18:46:16.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/vmware_cloud_foundation_health_monitoring.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 18:46:16.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/vmware_cloud_foundation_health_monitoring.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-04 18:46:16.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/vmware_cloud_foundation_health_monitoring.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 19:11:12.912591 vmware_cloud_foundation_health_monitoring-2.1.2.1001/
+-rw-rw-rw-   0        0        0     1368 2024-04-25 19:06:05.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/LICENSE
+-rw-rw-rw-   0        0        0      434 2024-04-25 19:06:05.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/NOTICE
+-rw-rw-rw-   0        0        0    19547 2024-04-25 19:11:12.912591 vmware_cloud_foundation_health_monitoring-2.1.2.1001/PKG-INFO
+-rw-rw-rw-   0        0        0    18670 2024-04-25 19:06:05.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/README.md
+-rw-rw-rw-   0        0        0       86 2023-08-25 20:53:55.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/pyproject.toml
+-rw-rw-rw-   0        0        0     1078 2024-04-25 19:11:12.912591 vmware_cloud_foundation_health_monitoring-2.1.2.1001/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-25 19:11:12.771963 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/
+drwxrwxrwx   0        0        0        0 2024-04-25 19:11:12.771963 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/artifacts/
+-rw-rw-rw-   0        0        0        0 2023-08-25 20:53:55.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/artifacts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 19:11:12.771963 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/artifacts/vSAN/
+-rw-rw-rw-   0        0        0   162075 2024-04-25 19:06:05.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/artifacts/vSAN/Alert_Definitions.xml
+-rw-rw-rw-   0        0        0    31891 2024-04-25 19:06:05.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/artifacts/vSAN/Dashboards.zip
+-rw-rw-rw-   0        0        0    18465 2024-04-25 19:06:05.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/artifacts/vSAN/Supermetrics.json
+-rw-rw-rw-   0        0        0    18783 2024-04-25 19:06:05.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/artifacts/vSAN/Views.zip
+-rw-rw-rw-   0        0        0        0 2023-08-25 20:53:55.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/artifacts/vSAN/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 19:11:12.787588 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/examples/
+-rw-rw-rw-   0        0        0        0 2023-08-25 20:53:55.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/examples/__init__.py
+-rwxrwxrwx   0        0        0       55 2023-08-25 20:53:55.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/examples/run_send-data-to-vrops.bat
+drwxrwxrwx   0        0        0        0 2024-04-25 19:11:12.834463 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/main/
+-rw-rw-rw-   0        0        0        0 2023-08-25 20:53:55.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/main/__init__.py
+-rw-rw-rw-   0        0        0     2693 2024-01-09 00:47:14.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/main/encrypt-passwords.py
+drwxrwxrwx   0        0        0        0 2024-04-25 19:11:12.834463 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/main/encrypted_files/
+-rw-rw-rw-   0        0        0        0 2023-08-25 20:53:55.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/main/encrypted_files/__init__.py
+-rw-rw-rw-   0        0        0     1655 2024-01-09 00:47:14.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/main/env.json
+-rw-rw-rw-   0        0        0   130855 2024-04-25 19:06:05.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/main/notifications-template.json
+-rw-rw-rw-   0        0        0     4381 2024-01-09 00:47:14.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/main/notifications.py
+-rw-rw-rw-   0        0        0    82701 2024-04-25 19:06:05.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/main/send-data-to-vrops.py
+drwxrwxrwx   0        0        0        0 2024-04-25 19:11:12.881341 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/main/utils/
+-rw-rw-rw-   0        0        0     5364 2024-01-18 21:29:57.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/main/utils/FolderUtility.py
+-rw-rw-rw-   0        0        0     3929 2024-01-18 21:29:57.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/main/utils/LogUtility.py
+-rw-rw-rw-   0        0        0     2528 2024-01-18 21:29:57.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/main/utils/PSUtility.py
+-rw-rw-rw-   0        0        0     6886 2024-01-18 21:29:57.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/main/utils/SosRest.py
+-rw-rw-rw-   0        0        0        0 2023-08-25 20:53:55.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/main/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 19:11:12.912591 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/vmware_cloud_foundation_health_monitoring.egg-info/
+-rw-rw-rw-   0        0        0    19547 2024-04-25 19:11:12.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/vmware_cloud_foundation_health_monitoring.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1002 2024-04-25 19:11:12.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/vmware_cloud_foundation_health_monitoring.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 19:11:12.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/vmware_cloud_foundation_health_monitoring.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-25 19:11:12.000000 vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/vmware_cloud_foundation_health_monitoring.egg-info/top_level.txt
```

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.1.1001/LICENSE` & `vmware_cloud_foundation_health_monitoring-2.1.2.1001/LICENSE`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.1.1001/PKG-INFO` & `vmware_cloud_foundation_health_monitoring-2.1.2.1001/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmware-cloud-foundation-health-monitoring
-Version: 2.1.1.1001
+Version: 2.1.2.1001
 Summary: Python Module for VMware Cloud Foundation Health Monitoring in VMware Aria Operations
 Home-page: https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
 Author: Broadcom
 Author-email: bhumitra.nagar@broadcom.com, olga.efremov@broadcom.com
 License: BSD-2-Clause
 Project-URL: Issues, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues
 Project-URL: Source, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
```

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.1.1001/README.md` & `vmware_cloud_foundation_health_monitoring-2.1.2.1001/README.md`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.1.1001/setup.cfg` & `vmware_cloud_foundation_health_monitoring-2.1.2.1001/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6d77 6172 652d 636c 6f75 642d   = vmware-cloud-
 00000020: 666f 756e 6461 7469 6f6e 2d68 6561 6c74  foundation-healt
 00000030: 682d 6d6f 6e69 746f 7269 6e67 0d0a 7665  h-monitoring..ve
-00000040: 7273 696f 6e20 3d20 322e 312e 312e 3130  rsion = 2.1.1.10
+00000040: 7273 696f 6e20 3d20 322e 312e 322e 3130  rsion = 2.1.2.10
 00000050: 3031 0d0a 6175 7468 6f72 203d 2042 726f  01..author = Bro
 00000060: 6164 636f 6d0d 0a61 7574 686f 725f 656d  adcom..author_em
 00000070: 6169 6c20 3d20 6268 756d 6974 7261 2e6e  ail = bhumitra.n
 00000080: 6167 6172 4062 726f 6164 636f 6d2e 636f  agar@broadcom.co
 00000090: 6d2c 206f 6c67 612e 6566 7265 6d6f 7640  m, olga.efremov@
 000000a0: 6272 6f61 6463 6f6d 2e63 6f6d 0d0a 6465  broadcom.com..de
 000000b0: 7363 7269 7074 696f 6e20 3d20 5079 7468  scription = Pyth
```

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/artifacts/vSAN/Alert_Definitions.xml` & `vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/artifacts/vSAN/Alert_Definitions.xml`

 * *Files 0% similar despite different names*

#### Comparing `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/artifacts/vSAN/Alert_Definitions.xml` & `vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/artifacts/vSAN/Alert_Definitions.xml`

```diff
@@ -10,14 +10,23 @@
         </SymptomSet>
         <Impact key="health" type="badge"/>
         <Recommendations>
           <Recommendation priority="1" ref="Recommendation-ud-98bae8b0-b328-4520-adc8-62dbb373a266"/>
         </Recommendations>
       </State>
     </AlertDefinition>
+    <AlertDefinition adapterKind="VMWARE" disableInBasePolicy="true" id="AlertDefinition-dc36105e-a766-4a73-ac9f-8356f9ae9ed7" name="SoS: PSC Ring Topology Status" resourceKind="VirtualMachine" subType="19" type="15">
+      <State severity="automatic">
+        <SymptomSet applyOn="self" operator="or">
+          <Symptom ref="SymptomDefinition-25725a2a-c727-49b4-bace-b4e11881feca"/>
+          <Symptom ref="SymptomDefinition-a6d6e4d3-fadb-4e0a-9d20-32a4a9cd1789"/>
+        </SymptomSet>
+        <Impact key="health" type="badge"/>
+      </State>
+    </AlertDefinition>
     <AlertDefinition adapterKind="NSXTAdapter" disableInBasePolicy="true" id="AlertDefinition-7b8b9d51-8c9c-4e3e-99c5-34eea2e9a2ce" name="HRM: NSX Local Manager Cluster backup is more than 3 days old." resourceKind="NSXTAdapterInstance" subType="18" type="20">
       <State severity="automatic">
         <SymptomSet applyOn="self" operator="and">
           <Symptom ref="SymptomDefinition-c31a0966-e487-4aa9-8308-381f98de631f"/>
           <Symptom ref="SymptomDefinition-8af4441e-32a4-4bc8-9b36-f3d18f59c447"/>
           <Symptom ref="SymptomDefinition-1571cd09-8d54-4eb3-a3c2-e31a90696cfe"/>
         </SymptomSet>
@@ -857,14 +866,24 @@
           <Symptom ref="SymptomDefinition-b79e651e-153d-4eb3-a71b-fa1821409e92"/>
         </SymptomSet>
         <Impact key="health" type="badge"/>
       </State>
     </AlertDefinition>
   </AlertDefinitions>
   <SymptomDefinitions>
+    <SymptomDefinition adapterKind="VMWARE" disableInBasePolicy="true" id="SymptomDefinition-a6d6e4d3-fadb-4e0a-9d20-32a4a9cd1789" name="Condition_541b2319-a359-4b7e-bc7d-fd41375460c3" resourceKind="VirtualMachine" symptomDefType="condition_self">
+      <State severity="warning">
+        <Condition key="SOS General|Ring Health Status|alert_code" operator="=" thresholdType="static" type="metric" value="1.0" valueType="numeric"/>
+      </State>
+    </SymptomDefinition>
+    <SymptomDefinition adapterKind="VMWARE" disableInBasePolicy="true" id="SymptomDefinition-25725a2a-c727-49b4-bace-b4e11881feca" name="Condition_12be692e-dfe1-401a-83aa-99ad94397dba" resourceKind="VirtualMachine" symptomDefType="condition_self">
+      <State severity="critical">
+        <Condition key="SOS General|Ring Health Status|alert_code" operator="=" thresholdType="static" type="metric" value="2.0" valueType="numeric"/>
+      </State>
+    </SymptomDefinition>
     <SymptomDefinition adapterKind="VMWARE" disableInBasePolicy="true" id="SymptomDefinition-3d956b76-0fe4-47cd-8261-002107e66e89" name="Condition_18bf90fc-c5d2-4da2-bad4-706e93a98107" resourceKind="HostSystem" symptomDefType="condition_self">
       <State severity="warning">
         <Condition key="HRM ESXi Connection Health Status|alert_code" operator="=" thresholdType="static" type="metric" value="1.0" valueType="numeric"/>
       </State>
     </SymptomDefinition>
     <SymptomDefinition adapterKind="VMWARE" disableInBasePolicy="true" id="SymptomDefinition-2d1e2b7e-284e-431e-87d7-e44540600d1c" name="Condition_c6b77c8a-966d-43e7-ac35-5a9b50292e16" resourceKind="VirtualMachine" symptomDefType="condition_self">
       <State severity="warning">
```

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/encrypt-passwords.py` & `vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/main/encrypt-passwords.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/env.json` & `vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/main/env.json`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/notifications-template.json` & `vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/main/notifications-template.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9983108108108107%*

 * *Differences: {"'NotificationRules'": "{'notificationRules': {0: {'NotificationRule': {insert: [(0, "*

 * *                        "OrderedDict([('id', OrderedDict([('@UUID', "*

 * *                        "'e792d731-e09a-43e8-afbe-dea385681d10'), ('@ObjectType', "*

 * *                        "'NOTIFICATION_RULE')])), ('Name', 'PSC Ring Topology health status'), "*

 * *                        "('Description', ''), ('PluginID', OrderedDict([('@pluginType', ''), "*

 * *                        "('@pluginName', '')])), ('PluginType', ''), ('entry', […]*

```diff
@@ -2,14 +2,57 @@
     "NotificationRules": {
         "notificationRules": [
             {
                 "NotificationRule": [
                     {
                         "Description": "",
                         "Disabled": false,
+                        "Name": "PSC Ring Topology health status",
+                        "PluginID": {
+                            "@pluginName": "",
+                            "@pluginType": ""
+                        },
+                        "PluginNotificationProperty": {
+                            "PropertyName": "",
+                            "PropertyValue": ""
+                        },
+                        "PluginType": "",
+                        "entry": [
+                            {
+                                "ConditionType": "RESOURCEKIND",
+                                "NotificationRuleResourceKindCondition": {
+                                    "ResourceKindKeys": [
+                                        {
+                                            "ResourceKindKey": {
+                                                "@adapterKind": "VMWARE",
+                                                "@resourceKind": "VirtualMachine"
+                                            }
+                                        }
+                                    ]
+                                }
+                            },
+                            {
+                                "ConditionType": "ALERT_DEFINITION_ID",
+                                "NotificationRuleAlertDefinitionCondition": {
+                                    "AlertDefinitionIds": [
+                                        {
+                                            "AlertDefinitionID": "AlertDefinition-dc36105e-a766-4a73-ac9f-8356f9ae9ed7"
+                                        }
+                                    ]
+                                }
+                            }
+                        ],
+                        "id": {
+                            "@ObjectType": "NOTIFICATION_RULE",
+                            "@UUID": "e792d731-e09a-43e8-afbe-dea385681d10"
+                        }
+                    },
+                    {
+                        "Description": "",
+                        "Disabled": false,
                         "Name": "Checks if disks are healthy",
                         "PluginID": {
                             "@pluginName": "",
                             "@pluginType": ""
                         },
                         "PluginNotificationProperty": {
                             "PropertyName": "",
```

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/notifications.py` & `vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/main/notifications.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/send-data-to-vrops.py` & `vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/main/send-data-to-vrops.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/utils/FolderUtility.py` & `vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/main/utils/FolderUtility.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/utils/LogUtility.py` & `vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/main/utils/LogUtility.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/utils/PSUtility.py` & `vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/main/utils/PSUtility.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/utils/SosRest.py` & `vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/main/utils/SosRest.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/vmware_cloud_foundation_health_monitoring.egg-info/PKG-INFO` & `vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/vmware_cloud_foundation_health_monitoring.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmware-cloud-foundation-health-monitoring
-Version: 2.1.1.1001
+Version: 2.1.2.1001
 Summary: Python Module for VMware Cloud Foundation Health Monitoring in VMware Aria Operations
 Home-page: https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
 Author: Broadcom
 Author-email: bhumitra.nagar@broadcom.com, olga.efremov@broadcom.com
 License: BSD-2-Clause
 Project-URL: Issues, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues
 Project-URL: Source, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
```

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/vmware_cloud_foundation_health_monitoring.egg-info/SOURCES.txt` & `vmware_cloud_foundation_health_monitoring-2.1.2.1001/source/vmware_cloud_foundation_health_monitoring.egg-info/SOURCES.txt`

 * *Files identical despite different names*


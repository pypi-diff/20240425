# Comparing `tmp/pyluba-0.0.1.tar.gz` & `tmp/pyluba-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyluba-0.0.1.tar", max compression
+gzip compressed data, was "pyluba-0.0.2.tar", max compression
```

## Comparing `pyluba-0.0.1.tar` & `pyluba-0.0.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0    35149 2024-02-24 00:10:17.430127 pyluba-0.0.1/LICENSE
--rw-r--r--   0        0        0      660 2024-02-24 00:10:17.430127 pyluba-0.0.1/README.md
--rw-r--r--   0        0        0      744 2024-02-24 08:02:07.442793 pyluba-0.0.1/pyluba/__init__.py
--rw-r--r--   0        0        0     1983 2024-03-25 03:39:32.867946 pyluba-0.0.1/pyluba/aliyun/cloud_gateway.py
--rw-r--r--   0        0        0     2233 2024-02-25 00:02:48.028073 pyluba-0.0.1/pyluba/aliyun/cloud_service.py
--rw-r--r--   0        0        0     6460 2024-03-22 21:00:07.350463 pyluba-0.0.1/pyluba/aliyun/test_alicloud_api_gateway.py
--rw-r--r--   0        0        0     6643 2024-02-24 00:10:17.431127 pyluba-0.0.1/pyluba/aliyun/tmp_constant.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.1/pyluba/bluetooth/__init__.py
--rw-r--r--   0        0        0     2918 2024-04-23 05:49:02.984986 pyluba-0.0.1/pyluba/bluetooth/ble.py
--rw-r--r--   0        0        0    33434 2024-04-23 05:07:10.882333 pyluba-0.0.1/pyluba/bluetooth/ble_message.py
--rw-r--r--   0        0        0     1748 2024-02-24 00:10:17.431127 pyluba-0.0.1/pyluba/bluetooth/const.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.1/pyluba/bluetooth/data/__init__.py
--rw-r--r--   0        0        0     4060 2024-04-23 05:35:18.909501 pyluba-0.0.1/pyluba/bluetooth/data/convert.py
--rw-r--r--   0        0        0     1051 2024-02-24 00:10:17.431127 pyluba-0.0.1/pyluba/bluetooth/data/framectrldata.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.1/pyluba/bluetooth/data/model/__init__.py
--rw-r--r--   0        0        0     2009 2024-02-24 00:10:17.431127 pyluba-0.0.1/pyluba/bluetooth/data/notifydata.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.1/pyluba/data/__init__.py
--rw-r--r--   0        0        0      265 2024-02-24 00:10:17.431127 pyluba-0.0.1/pyluba/data/model/__init__.py
--rw-r--r--   0        0        0     1349 2024-04-23 05:07:53.289798 pyluba-0.0.1/pyluba/data/model/excute_boarder_params.py
--rw-r--r--   0        0        0     1075 2024-04-23 05:07:10.891334 pyluba-0.0.1/pyluba/data/model/execute_boarder.py
--rw-r--r--   0        0        0     3271 2024-02-24 00:10:17.431127 pyluba-0.0.1/pyluba/data/model/generate_route_information.py
--rw-r--r--   0        0        0      480 2024-02-24 00:10:17.431127 pyluba-0.0.1/pyluba/data/model/hash_list.py
--rw-r--r--   0        0        0      454 2024-02-24 00:10:17.431127 pyluba-0.0.1/pyluba/data/model/mowing_modes.py
--rw-r--r--   0        0        0     1924 2024-02-24 00:10:17.431127 pyluba-0.0.1/pyluba/data/model/plan.py
--rw-r--r--   0        0        0      986 2024-02-24 00:10:17.431127 pyluba-0.0.1/pyluba/data/model/rapid_state.py
--rw-r--r--   0        0        0     2780 2024-02-24 00:10:17.431127 pyluba-0.0.1/pyluba/data/model/region_data.py
--rw-r--r--   0        0        0        3 2024-02-24 00:10:17.431127 pyluba-0.0.1/pyluba/data/mqtt/__init__.py
--rw-r--r--   0        0        0     1669 2024-02-24 00:10:17.432128 pyluba-0.0.1/pyluba/data/mqtt/event.py
--rw-r--r--   0        0        0     2343 2024-02-24 00:10:17.432128 pyluba-0.0.1/pyluba/data/mqtt/properties.py
--rw-r--r--   0        0        0      924 2024-02-24 00:10:17.432128 pyluba-0.0.1/pyluba/data/mqtt/status.py
--rw-r--r--   0        0        0      122 2024-02-24 00:10:17.432128 pyluba-0.0.1/pyluba/event/__init__.py
--rw-r--r--   0        0        0     1440 2024-02-24 00:10:17.432128 pyluba-0.0.1/pyluba/event/event.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.432128 pyluba-0.0.1/pyluba/http/_init_.py
--rw-r--r--   0        0        0     1832 2024-02-24 11:05:42.835293 pyluba-0.0.1/pyluba/http/http.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.432128 pyluba-0.0.1/pyluba/luba/_init_.py
--rw-r--r--   0        0        0     3279 2024-02-24 00:10:17.432128 pyluba-0.0.1/pyluba/luba/base.py
--rw-r--r--   0        0        0     5392 2024-02-24 08:01:33.605363 pyluba-0.0.1/pyluba/mqtt/mqtt.py
--rw-r--r--   0        0        0       81 2024-02-24 00:10:17.432128 pyluba-0.0.1/pyluba/proto/common.proto
--rw-r--r--   0        0        0     1022 2024-02-24 00:10:17.432128 pyluba-0.0.1/pyluba/proto/common_pb2.py
--rw-r--r--   0        0        0     2699 2024-02-24 00:10:17.432128 pyluba-0.0.1/pyluba/proto/esp_driver.proto
--rw-r--r--   0        0        0     6770 2024-02-24 00:10:17.432128 pyluba-0.0.1/pyluba/proto/esp_driver_pb2.py
--rw-r--r--   0        0        0     1161 2024-02-24 00:10:17.432128 pyluba-0.0.1/pyluba/proto/luba_msg.proto
--rw-r--r--   0        0        0     3365 2024-02-24 00:10:17.432128 pyluba-0.0.1/pyluba/proto/luba_msg_pb2.py
--rw-r--r--   0        0        0      587 2024-02-24 00:10:17.432128 pyluba-0.0.1/pyluba/proto/mctrl_driver.proto
--rw-r--r--   0        0        0     2124 2024-02-24 00:10:17.432128 pyluba-0.0.1/pyluba/proto/mctrl_driver_pb2.py
--rw-r--r--   0        0        0     8806 2024-02-24 00:10:17.432128 pyluba-0.0.1/pyluba/proto/mctrl_nav.proto
--rw-r--r--   0        0        0    18010 2024-02-24 00:10:17.432128 pyluba-0.0.1/pyluba/proto/mctrl_nav_pb2.py
--rw-r--r--   0        0        0     4643 2024-02-24 00:10:17.433127 pyluba-0.0.1/pyluba/proto/mctrl_sys.proto
--rw-r--r--   0        0        0    11241 2024-02-24 00:10:17.433127 pyluba-0.0.1/pyluba/proto/mctrl_sys_pb2.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.433127 pyluba-0.0.1/pyluba/py.typed
--rw-r--r--   0        0        0     2134 2024-02-24 00:10:17.433127 pyluba-0.0.1/pyluba/utility/constant/device_constant.py
--rw-r--r--   0        0        0     1073 2024-02-24 00:10:17.433127 pyluba-0.0.1/pyluba/utility/periodic.py
--rw-r--r--   0        0        0     5097 2024-02-24 00:10:17.433127 pyluba-0.0.1/pyluba/utility/rocker_util.py
--rw-r--r--   0        0        0     1292 2024-04-23 04:59:04.905741 pyluba-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1586 1970-01-01 00:00:00.000000 pyluba-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-24 00:10:17.430127 pyluba-0.0.2/LICENSE
+-rw-r--r--   0        0        0      660 2024-02-24 00:10:17.430127 pyluba-0.0.2/README.md
+-rw-r--r--   0        0        0      744 2024-02-24 08:02:07.442793 pyluba-0.0.2/pyluba/__init__.py
+-rw-r--r--   0        0        0     1983 2024-03-25 03:39:32.867946 pyluba-0.0.2/pyluba/aliyun/cloud_gateway.py
+-rw-r--r--   0        0        0     2233 2024-02-25 00:02:48.028073 pyluba-0.0.2/pyluba/aliyun/cloud_service.py
+-rw-r--r--   0        0        0     6460 2024-03-22 21:00:07.350463 pyluba-0.0.2/pyluba/aliyun/test_alicloud_api_gateway.py
+-rw-r--r--   0        0        0     6643 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/aliyun/tmp_constant.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/bluetooth/__init__.py
+-rw-r--r--   0        0        0     2918 2024-04-23 05:49:02.984986 pyluba-0.0.2/pyluba/bluetooth/ble.py
+-rw-r--r--   0        0        0    34772 2024-04-24 23:43:48.736942 pyluba-0.0.2/pyluba/bluetooth/ble_message.py
+-rw-r--r--   0        0        0     1748 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/bluetooth/const.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/bluetooth/data/__init__.py
+-rw-r--r--   0        0        0     4166 2024-04-24 21:43:54.006537 pyluba-0.0.2/pyluba/bluetooth/data/convert.py
+-rw-r--r--   0        0        0     1051 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/bluetooth/data/framectrldata.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/bluetooth/data/model/__init__.py
+-rw-r--r--   0        0        0     2009 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/bluetooth/data/notifydata.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/data/__init__.py
+-rw-r--r--   0        0        0      265 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/data/model/__init__.py
+-rw-r--r--   0        0        0     1349 2024-04-23 05:07:53.289798 pyluba-0.0.2/pyluba/data/model/excute_boarder_params.py
+-rw-r--r--   0        0        0     1075 2024-04-23 05:07:10.891334 pyluba-0.0.2/pyluba/data/model/execute_boarder.py
+-rw-r--r--   0        0        0     3271 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/data/model/generate_route_information.py
+-rw-r--r--   0        0        0      480 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/data/model/hash_list.py
+-rw-r--r--   0        0        0      454 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/data/model/mowing_modes.py
+-rw-r--r--   0        0        0     1924 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/data/model/plan.py
+-rw-r--r--   0        0        0      986 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/data/model/rapid_state.py
+-rw-r--r--   0        0        0     2780 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/data/model/region_data.py
+-rw-r--r--   0        0        0        3 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/data/mqtt/__init__.py
+-rw-r--r--   0        0        0     1669 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/data/mqtt/event.py
+-rw-r--r--   0        0        0     2343 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/data/mqtt/properties.py
+-rw-r--r--   0        0        0      924 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/data/mqtt/status.py
+-rw-r--r--   0        0        0      122 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/event/__init__.py
+-rw-r--r--   0        0        0     1440 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/event/event.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/http/_init_.py
+-rw-r--r--   0        0        0     1832 2024-02-24 11:05:42.835293 pyluba-0.0.2/pyluba/http/http.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/luba/_init_.py
+-rw-r--r--   0        0        0     3279 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/luba/base.py
+-rw-r--r--   0        0        0     5392 2024-02-24 08:01:33.605363 pyluba-0.0.2/pyluba/mqtt/mqtt.py
+-rw-r--r--   0        0        0       81 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/proto/common.proto
+-rw-r--r--   0        0        0     1022 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/proto/common_pb2.py
+-rw-r--r--   0        0        0     2699 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/proto/esp_driver.proto
+-rw-r--r--   0        0        0     6770 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/proto/esp_driver_pb2.py
+-rw-r--r--   0        0        0     1161 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/proto/luba_msg.proto
+-rw-r--r--   0        0        0     3365 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/proto/luba_msg_pb2.py
+-rw-r--r--   0        0        0      587 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/proto/mctrl_driver.proto
+-rw-r--r--   0        0        0     2124 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/proto/mctrl_driver_pb2.py
+-rw-r--r--   0        0        0     8806 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/proto/mctrl_nav.proto
+-rw-r--r--   0        0        0    18010 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/proto/mctrl_nav_pb2.py
+-rw-r--r--   0        0        0     4643 2024-02-24 00:10:17.433127 pyluba-0.0.2/pyluba/proto/mctrl_sys.proto
+-rw-r--r--   0        0        0    11241 2024-02-24 00:10:17.433127 pyluba-0.0.2/pyluba/proto/mctrl_sys_pb2.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.433127 pyluba-0.0.2/pyluba/py.typed
+-rw-r--r--   0        0        0     2134 2024-02-24 00:10:17.433127 pyluba-0.0.2/pyluba/utility/constant/device_constant.py
+-rw-r--r--   0        0        0     1073 2024-02-24 00:10:17.433127 pyluba-0.0.2/pyluba/utility/periodic.py
+-rw-r--r--   0        0        0     5097 2024-02-24 00:10:17.433127 pyluba-0.0.2/pyluba/utility/rocker_util.py
+-rw-r--r--   0        0        0     1293 2024-04-24 23:46:30.703512 pyluba-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1631 1970-01-01 00:00:00.000000 pyluba-0.0.2/PKG-INFO
```

### Comparing `pyluba-0.0.1/LICENSE` & `pyluba-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/README.md` & `pyluba-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/__init__.py` & `pyluba-0.0.2/pyluba/__init__.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/aliyun/cloud_gateway.py` & `pyluba-0.0.2/pyluba/aliyun/cloud_gateway.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/aliyun/cloud_service.py` & `pyluba-0.0.2/pyluba/aliyun/cloud_service.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/aliyun/test_alicloud_api_gateway.py` & `pyluba-0.0.2/pyluba/aliyun/test_alicloud_api_gateway.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/aliyun/tmp_constant.py` & `pyluba-0.0.2/pyluba/aliyun/tmp_constant.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/bluetooth/ble.py` & `pyluba-0.0.2/pyluba/bluetooth/ble.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/bluetooth/ble_message.py` & `pyluba-0.0.2/pyluba/bluetooth/ble_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-
-
 from asyncio import sleep
 from io import BytesIO
 import itertools
 import json
 import queue
 import sys
 import time
@@ -55,126 +53,144 @@
     mReadSequence = itertools.count()
     mAck = queue.Queue()
     notification = BlufiNotifyData()
 
     def __init__(self, client: BleakClient):
         self.client = client
 
+    async def all_powerful_RW(self, i: int, i2: int, i3: int):
+        mctrl_sys = mctrl_sys_pb2.MctlSys()
 
-    async def getDeviceVersionMain(self):
-        commEsp = esp_driver_pb2.CommEsp()
+        reqIdReq = mctrl_sys_pb2.SysCommCmd()
+        reqIdReq.id = i
+        reqIdReq.context = i2
+        reqIdReq.rw = i3
+        lubaMsg = luba_msg_pb2.LubaMsg()
+        lubaMsg.msgtype = luba_msg_pb2.MSG_CMD_TYPE_EMBED_SYS
+        lubaMsg.sender = luba_msg_pb2.DEV_MOBILEAPP
+        lubaMsg.rcver = luba_msg_pb2.DEV_MAINCTL
+        lubaMsg.msgattr = luba_msg_pb2.MSG_ATTR_REQ
+        lubaMsg.seqs = 1
+        lubaMsg.version = 1
+        lubaMsg.subtype = 1
+        lubaMsg.sys.CopyFrom(mctrl_sys)
+        byte_arr = lubaMsg.SerializeToString()
+        await self.postCustomDataBytes(byte_arr)
+
+    async def get_device_version_main(self):
+        commEsp = esp_driver_pb2.CommEsp(
+            todev_devinfo_req=esp_driver_pb2.DrvDevInfoReq()
+        )
 
-        reqIdReq = commEsp.todev_devinfo_req.req_ids.add()
-        reqIdReq.id = 1
-        reqIdReq.type = 6
         lubaMsg = luba_msg_pb2.LubaMsg()
         lubaMsg.msgtype = luba_msg_pb2.MSG_CMD_TYPE_ESP
         lubaMsg.sender = luba_msg_pb2.DEV_MOBILEAPP
         lubaMsg.rcver = luba_msg_pb2.DEV_COMM_ESP
         lubaMsg.msgattr = luba_msg_pb2.MSG_ATTR_REQ
         lubaMsg.seqs = 1
         lubaMsg.version = 1
         lubaMsg.subtype = 1
         lubaMsg.esp.CopyFrom(commEsp)
         byte_arr = lubaMsg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
-    async def sendTodevBleSync(self):
-        commEsp = esp_driver_pb2.CommEsp()
+    async def send_todev_ble_sync(self, sync_type: int):
+        commEsp = esp_driver_pb2.CommEsp(
+            todev_ble_sync=1
+        )
 
-        commEsp.todev_ble_sync = 1
+        commEsp.todev_ble_sync = sync_type
         lubaMsg = luba_msg_pb2.LubaMsg()
         lubaMsg.msgtype = luba_msg_pb2.MSG_CMD_TYPE_ESP
         lubaMsg.sender = luba_msg_pb2.DEV_MOBILEAPP
         lubaMsg.rcver = luba_msg_pb2.DEV_COMM_ESP
         lubaMsg.seqs = 1
         lubaMsg.version = 1
         lubaMsg.subtype = 1
         lubaMsg.esp.CopyFrom(commEsp)
         byte_arr = lubaMsg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
     async def get_all_boundary_hash_list(self, i: int):
         """.getAllBoundaryHashList(3); 0"""
         luba_msg = luba_msg_pb2.LubaMsg(
-        msgtype = luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_NAV,
-        sender = luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
-        rcver = luba_msg_pb2.MsgDevice.DEV_MAINCTL,
-        msgattr = luba_msg_pb2.MsgAttr.MSG_ATTR_NONE,
-        seqs=1,
-        version=1,
-        subtype=1,
-        nav=mctrl_nav_pb2.MctlNav(
-            todev_gethash=mctrl_nav_pb2.NavGetHashList(
-                pver=1,
-                subCmd=i
+            msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_NAV,
+            sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
+            rcver=luba_msg_pb2.MsgDevice.DEV_MAINCTL,
+            msgattr=luba_msg_pb2.MsgAttr.MSG_ATTR_NONE,
+            seqs=1,
+            version=1,
+            subtype=1,
+            nav=mctrl_nav_pb2.MctlNav(
+                todev_gethash=mctrl_nav_pb2.NavGetHashList(
+                    pver=1,
+                    subCmd=i
                 )
             )
         )
 
         byte_arr = luba_msg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
     async def get_line_info(self, i: int):
         luba_msg = luba_msg_pb2.LubaMsg(
-        msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_NAV,
-        sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
-        rcver=luba_msg_pb2.MsgDevice.DEV_MAINCTL,
-        msgattr=luba_msg_pb2.MsgAttr.MSG_ATTR_REQ,
-        seqs=1,
-        version=1,
-        subtype=1,
-        nav=mctrl_nav_pb2.MctlNav(
-            todev_zigzag_ack=mctrl_nav_pb2.NavUploadZigZagResultAck(
-                pver=1,
-                currentHash=i,
-                subCmd=0
+            msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_NAV,
+            sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
+            rcver=luba_msg_pb2.MsgDevice.DEV_MAINCTL,
+            msgattr=luba_msg_pb2.MsgAttr.MSG_ATTR_REQ,
+            seqs=1,
+            version=1,
+            subtype=1,
+            nav=mctrl_nav_pb2.MctlNav(
+                todev_zigzag_ack=mctrl_nav_pb2.NavUploadZigZagResultAck(
+                    pver=1,
+                    currentHash=i,
+                    subCmd=0
                 )
             ),
         )
         byte_arr = luba_msg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
-
     async def get_hash_response(self, totalFrame: int, currentFrame: int):
         luba_msg = luba_msg_pb2.LubaMsg(
-        msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_NAV,
-        sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
-        rcver=luba_msg_pb2.MsgDevice.DEV_MAINCTL,
-        msgattr=luba_msg_pb2.MsgAttr.MSG_ATTR_REQ,
-        seqs=1,
-        version=1,
-        subtype=1,
-        nav=mctrl_nav_pb2.MctlNav(
-            todev_gethash=mctrl_nav_pb2.NavGetHashList(
-                pver=1,
-                subCmd=2,
-                currentFrame=currentFrame,
-                totalFrame=totalFrame
+            msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_NAV,
+            sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
+            rcver=luba_msg_pb2.MsgDevice.DEV_MAINCTL,
+            msgattr=luba_msg_pb2.MsgAttr.MSG_ATTR_REQ,
+            seqs=1,
+            version=1,
+            subtype=1,
+            nav=mctrl_nav_pb2.MctlNav(
+                todev_gethash=mctrl_nav_pb2.NavGetHashList(
+                    pver=1,
+                    subCmd=2,
+                    currentFrame=currentFrame,
+                    totalFrame=totalFrame
                 )
             )
         )
         byte_arr = luba_msg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
     async def synchronize_hash_data(self, l: int):
         luba_msg = luba_msg_pb2.LubaMsg(
-        msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_NAV,
-        sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
-        rcver=luba_msg_pb2.MsgDevice.DEV_MAINCTL,
-        msgattr=luba_msg_pb2.MsgAttr.MSG_ATTR_REQ,
-        seqs=1,
-        version=1,
-        subtype=1,
-        nav=mctrl_nav_pb2.MctlNav(
-            todev_get_commondata=mctrl_nav_pb2.NavGetCommData(
-                pver=1,
-                action=8,
-                Hash=l,
-                subCmd=1
+            msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_NAV,
+            sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
+            rcver=luba_msg_pb2.MsgDevice.DEV_MAINCTL,
+            msgattr=luba_msg_pb2.MsgAttr.MSG_ATTR_REQ,
+            seqs=1,
+            version=1,
+            subtype=1,
+            nav=mctrl_nav_pb2.MctlNav(
+                todev_get_commondata=mctrl_nav_pb2.NavGetCommData(
+                    pver=1,
+                    action=8,
+                    Hash=l,
+                    subCmd=1
                 )
             )
         )
         byte_arr = luba_msg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
     async def get_task(self):
@@ -183,67 +199,67 @@
 
     async def send_ble_alive(self):
         hash_map = {"ctrl": 1}
         await self.postCustomData(self.get_json_string(bleOrderCmd.bleAlive, hash_map))
 
     async def set_speed(self, speed: float):
         luba_msg = luba_msg_pb2.LubaMsg(
-        msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_EMBED_DRIVER,
-        sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
-        rcver=luba_msg_pb2.MsgDevice.DEV_MAINCTL,
-        msgattr=luba_msg_pb2.MsgAttr.MSG_ATTR_REQ,
-        seqs=1,
-        version=1,
-        subtype=1,
-        driver=mctrl_driver_pb2.MctrlDriver(
-            bidire_speed_read_set=mctrl_driver_pb2.DrvSrSpeed(
-                speed=float(speed),
-                rw=1
+            msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_EMBED_DRIVER,
+            sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
+            rcver=luba_msg_pb2.MsgDevice.DEV_MAINCTL,
+            msgattr=luba_msg_pb2.MsgAttr.MSG_ATTR_REQ,
+            seqs=1,
+            version=1,
+            subtype=1,
+            driver=mctrl_driver_pb2.MctrlDriver(
+                bidire_speed_read_set=mctrl_driver_pb2.DrvSrSpeed(
+                    speed=float(speed),
+                    rw=1
                 )
             )
         )
 
         byte_arr = luba_msg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
     async def start_work_job(self):
         luba_msg = luba_msg_pb2.LubaMsg(
-        msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_NAV,
-        sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
-        rcver=luba_msg_pb2.MsgDevice.DEV_MAINCTL,
-        msgattr=luba_msg_pb2.MsgAttr.MSG_ATTR_REQ,
-        seqs=1,
-        version=1,
-        subtype=1,
-        nav=mctrl_nav_pb2.MctlNav(
-            todev_taskctrl=mctrl_nav_pb2.NavTaskCtrl(
-                type=1,
-                action=1,
-                result=0
+            msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_NAV,
+            sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
+            rcver=luba_msg_pb2.MsgDevice.DEV_MAINCTL,
+            msgattr=luba_msg_pb2.MsgAttr.MSG_ATTR_REQ,
+            seqs=1,
+            version=1,
+            subtype=1,
+            nav=mctrl_nav_pb2.MctlNav(
+                todev_taskctrl=mctrl_nav_pb2.NavTaskCtrl(
+                    type=1,
+                    action=1,
+                    result=0
                 )
             )
         )
 
         byte_arr = luba_msg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
     # (2, 0);
     async def read_plan(self, i: int, i2: int):
         luba_msg = luba_msg_pb2.LubaMsg(
-        msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_NAV,
-        sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
-        rcver=luba_msg_pb2.MsgDevice.DEV_MAINCTL,
-        msgattr=luba_msg_pb2.MsgAttr.MSG_ATTR_REQ,
-        seqs=1,
-        version=1,
-        subtype=1,
-        nav=mctrl_nav_pb2.MctlNav(
-            todev_planjob_set=mctrl_nav_pb2.NavPlanJobSet(
-                subCmd=i,
-                planIndex=i2
+            msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_NAV,
+            sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
+            rcver=luba_msg_pb2.MsgDevice.DEV_MAINCTL,
+            msgattr=luba_msg_pb2.MsgAttr.MSG_ATTR_REQ,
+            seqs=1,
+            version=1,
+            subtype=1,
+            nav=mctrl_nav_pb2.MctlNav(
+                todev_planjob_set=mctrl_nav_pb2.NavPlanJobSet(
+                    subCmd=i,
+                    planIndex=i2
                 )
             )
         )
         byte_arr = luba_msg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
     async def read_plan_unable_time(self, i):
@@ -256,19 +272,17 @@
         luba_msg.rcver = luba_msg_pb2.MsgDevice.DEV_MAINCTL
         luba_msg.msgattr = luba_msg_pb2.MsgAttr.MSG_ATTR_REQ
         luba_msg.seqs = 1
         luba_msg.version = 1
         luba_msg.subtype = 1
         luba_msg.nav.todev_unable_time_set.CopyFrom(build)
 
-
         byte_arr = luba_msg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
-
     async def sendPlan2(self, plan: Plan):
         navPlanJobSet = luba_msg_pb2.NavPlanJobSet()
         navPlanJobSet.pver = plan.pver
         navPlanJobSet.subCmd = plan.subCmd
         navPlanJobSet.area = plan.area
         navPlanJobSet.deviceId = plan.deviceId
         navPlanJobSet.workTime = plan.workTime
@@ -307,36 +321,33 @@
         luba_msg.version = 1
         luba_msg.subtype = 1
         luba_msg.nav.todevPlanjobSet.CopyFrom(navPlanJobSet)
 
         byte_arr = luba_msg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
-
     def get_reserved(self, generate_route_information):
         return bytes([generate_route_information.path_order, generate_route_information.obstacle_laps]).decode('utf-8')
 
-
     async def generate_route_information(self, generate_route_information):
         """how you start a manual job, then call startjob"""
 
         nav_req_cover_path = mctrl_nav_pb2.NavReqCoverPath()
         nav_req_cover_path.pver = 1
         nav_req_cover_path.subCmd = 0
         nav_req_cover_path.zoneHashs.extend(generate_route_information.one_hashs)
         nav_req_cover_path.jobMode = generate_route_information.job_mode  # grid type
-        nav_req_cover_path.edgeMode = generate_route_information.edge_mode # border laps
+        nav_req_cover_path.edgeMode = generate_route_information.edge_mode  # border laps
         nav_req_cover_path.knifeHeight = generate_route_information.knife_height
         nav_req_cover_path.speed = generate_route_information.speed
         nav_req_cover_path.ultraWave = generate_route_information.ultra_wave
         nav_req_cover_path.channelWidth = generate_route_information.channel_width  # mow width
         nav_req_cover_path.channelMode = generate_route_information.channel_mode
         nav_req_cover_path.toward = generate_route_information.toward
-        nav_req_cover_path.reserved = self.get_reserved(generate_route_information)  #grid or border first
-
+        nav_req_cover_path.reserved = self.get_reserved(generate_route_information)  # grid or border first
 
         luba_msg = luba_msg_pb2.LubaMsg()
         luba_msg.msgtype = luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_NAV
         luba_msg.sender = luba_msg_pb2.MsgDevice.DEV_MOBILEAPP
         luba_msg.rcver = luba_msg_pb2.MsgDevice.DEV_MAINCTL
         luba_msg.msgattr = luba_msg_pb2.MsgAttr.MSG_ATTR_REQ
         luba_msg.seqs = 1
@@ -346,16 +357,16 @@
         mctl_nav = mctrl_nav_pb2.MctlNav()
         mctl_nav.bidire_reqconver_path.CopyFrom(nav_req_cover_path)
         luba_msg.nav.CopyFrom(mctl_nav)
 
         byte_arr = luba_msg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
-
-    async def start_work_order(self, job_id, job_ver, rain_tactics, job_mode, knife_height, speed, ultra_wave, channel_width, channel_mode):
+    async def start_work_order(self, job_id, job_ver, rain_tactics, job_mode, knife_height, speed, ultra_wave,
+                               channel_width, channel_mode):
         """Pretty sure this starts a job too but isn't used"""
         luba_msg = luba_msg_pb2.LubaMsg()
         luba_msg.msgtype = luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_NAV
         luba_msg.sender = luba_msg_pb2.MsgDevice.DEV_MOBILEAPP
         luba_msg.rcver = luba_msg_pb2.MsgDevice.DEV_MAINCTL
         luba_msg.msgattr = luba_msg_pb2.MsgAttr.MSG_ATTR_REQ
         luba_msg.seqs = 1
@@ -376,76 +387,73 @@
 
         nav.todev_mow_task.CopyFrom(start_job)
         luba_msg.nav.CopyFrom(nav)
 
         byte_arr = luba_msg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
-
-
     async def breakPointContinue(self):
         luba_msg = luba_msg_pb2.LubaMsg(
-        msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_NAV,
-        sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
-        rcver=luba_msg_pb2.MsgDevice.DEV_MAINCTL,
-        msgattr=luba_msg_pb2.MsgAttr.MSG_ATTR_REQ,
-        seqs=1,
-        version=1,
-        subtype=1,
-        nav=mctrl_nav_pb2.MctlNav(
-            todev_taskctrl=mctrl_nav_pb2.NavTaskCtrl(
-                type=1,
-                action=7,
-                result=0
+            msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_NAV,
+            sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
+            rcver=luba_msg_pb2.MsgDevice.DEV_MAINCTL,
+            msgattr=luba_msg_pb2.MsgAttr.MSG_ATTR_REQ,
+            seqs=1,
+            version=1,
+            subtype=1,
+            nav=mctrl_nav_pb2.MctlNav(
+                todev_taskctrl=mctrl_nav_pb2.NavTaskCtrl(
+                    type=1,
+                    action=7,
+                    result=0
                 )
             )
         )
         byte_arr = luba_msg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
     async def breakPointAnywhereContinue(self, refresh_loading: bool):
         luba_msg = luba_msg_pb2.LubaMsg(
-        msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_NAV,
-        sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
-        rcver=luba_msg_pb2.MsgDevice.DEV_MAINCTL,
-        msgattr=luba_msg_pb2.MsgAttr.MSG_ATTR_REQ,
-        seqs=1,
-        version=1,
-        subtype=1,
-        nav=mctrl_nav_pb2.MctlNav(
-            todev_taskctrl=mctrl_nav_pb2.NavTaskCtrl(
-                type=1,
-                action=9,
-                result=0
+            msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_NAV,
+            sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
+            rcver=luba_msg_pb2.MsgDevice.DEV_MAINCTL,
+            msgattr=luba_msg_pb2.MsgAttr.MSG_ATTR_REQ,
+            seqs=1,
+            version=1,
+            subtype=1,
+            nav=mctrl_nav_pb2.MctlNav(
+                todev_taskctrl=mctrl_nav_pb2.NavTaskCtrl(
+                    type=1,
+                    action=9,
+                    result=0
                 )
             )
         )
         byte_arr = luba_msg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
-
     def clearNotification(self):
         self.notification = None
         self.notification = BlufiNotifyData()
 
-    async def getDeviceInfo(self):
+    async def get_device_info(self):
         await self.postCustomData(self.getJsonString(bleOrderCmd.getDeviceInfo))
 
-    async def sendDeviceInfo(self):
+    async def send_device_info(self):
         """currently not called"""
         luba_msg = luba_msg_pb2.LubaMsg(
-        msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_ESP,
-        sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
-        rcver=luba_msg_pb2.MsgDevice.DEV_COMM_ESP,
-        seqs=1,
-        version=1,
-        subtype=1,
-        esp=esp_driver_pb2.CommEsp(
-            todevBleSync=1,
-            todevDevinfoReq=esp_driver_pb2.DrvDevInfoReq()
+            msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_ESP,
+            sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
+            rcver=luba_msg_pb2.MsgDevice.DEV_COMM_ESP,
+            seqs=1,
+            version=1,
+            subtype=1,
+            esp=esp_driver_pb2.CommEsp(
+                todev_ble_sync=1,
+                todev_devinfo_req=esp_driver_pb2.DrvDevInfoReq()
             )
         )
         byte_arr = luba_msg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
     async def requestDeviceStatus(self):
         request = False
@@ -457,15 +465,14 @@
             # Log.w(TAG, "post requestDeviceStatus interrupted")
             request = False
             print(err)
 
         # if not request:
         #     onStatusResponse(BlufiCallback.CODE_WRITE_DATA_FAILED, null)
 
-
     async def requestDeviceVersion(self):
         request = False
         type = self.getTypeValue(0, 7)
         try:
             request = await self.post(BleMessage.mEncrypted, BleMessage.mChecksum, False, type, None)
             # print(request)
         except Exception as err:
@@ -504,15 +511,14 @@
         lubaMsg.seqs = 1
         lubaMsg.version = 1
         lubaMsg.subtype = 1
         lubaMsg.nav.CopyFrom(mctrlNav)
         bytes = lubaMsg.SerializeToString()
         await self.postCustomDataBytes(bytes)
 
-
     async def setbladeHeight(self, height: int):
         mctrlDriver = mctrl_driver_pb2.MctrlDriver()
         drvKnifeHeight = mctrl_driver_pb2.DrvKnifeHeight()
         drvKnifeHeight.knifeHeight = height
         mctrlDriver.todev_knife_hight_set.CopyFrom(drvKnifeHeight)
 
         lubaMsg = luba_msg_pb2.LubaMsg()
@@ -541,56 +547,49 @@
         lubaMsg.seqs = 1
         lubaMsg.version = 1
         lubaMsg.subtype = 1
         lubaMsg.sys.CopyFrom(mctlsys)
         bytes = lubaMsg.SerializeToString()
         await self.postCustomDataBytes(bytes)
 
-
     async def start_job(self, blade_height):
         """call after calling generate_route_information I think"""
         await self.setbladeHeight(blade_height)
         await self.start_work_job()
 
     async def transformSpeed(self, linear: float, percent: float):
 
         transfrom3 = RockerControlUtil.getInstance().transfrom3(linear, percent)
         if (transfrom3 is not None and len(transfrom3) > 0):
             linearSpeed = transfrom3[0] * 10
-            angularSpeed = (int) (transfrom3[1] * 4.5)
+            angularSpeed = (int)(transfrom3[1] * 4.5)
 
             await self.sendMovement(linearSpeed, angularSpeed)
 
     async def transformBothSpeeds(self, linear: float, angular: float, linearPercent: float, angularPercent: float):
         transfrom3 = RockerControlUtil.getInstance().transfrom3(linear, linearPercent)
         transform4 = RockerControlUtil.getInstance().transfrom3(angular, angularPercent)
 
         if (transfrom3 != None and len(transfrom3) > 0):
             linearSpeed = transfrom3[0] * 10
-            angularSpeed = (int) (transform4[1] * 4.5)
+            angularSpeed = (int)(transform4[1] * 4.5)
             print(linearSpeed, angularSpeed)
             await self.sendMovement(linearSpeed, angularSpeed)
 
-
-
     # asnyc def transfromDoubleRockerSpeed(float f, float f2, boolean z):
     #         transfrom3 = RockerControlUtil.getInstance().transfrom3(f, f2)
     #         if (transfrom3 != null && transfrom3.size() > 0):
     #             if (z):
     #                 this.linearSpeed = transfrom3.get(0).intValue() * 10
     #             else
     #                 this.angularSpeed = (int) (transfrom3.get(1).intValue() * 4.5d)
 
-
     #         if (this.countDownTask == null):
     #             testSendControl()
 
-
-
-
     async def sendMovement(self, linearSpeed: int, angularSpeed: int):
         mctrlDriver = mctrl_driver_pb2.MctrlDriver()
 
         drvMotionCtrl = mctrl_driver_pb2.DrvMotionCtrl()
         drvMotionCtrl.setLinearSpeed = linearSpeed
         drvMotionCtrl.setAngularSpeed = angularSpeed
         mctrlDriver.todev_devmotion_ctrl.CopyFrom(drvMotionCtrl)
@@ -604,21 +603,17 @@
         lubaMsg.version = 1
         lubaMsg.subtype = 1
 
         lubaMsg.driver.CopyFrom(mctrlDriver)
         bytes = lubaMsg.SerializeToString()
         await self.postCustomDataBytes(bytes)
 
-
     async def sendBorderPackage(self, executeBorder: ExecuteBorder):
         await self.postCustomData(serialize(executeBorder))
 
-
-
-
     async def postCustomDataBytes(self, data: bytearray):
         if (data == None):
             return
         type_val = self.getTypeValue(1, 19)
         try:
             suc = await self.post(self.mEncrypted, self.mChecksum, self.mRequireAck, type_val, data)
             # int status = suc ? 0 : BlufiCallback.CODE_WRITE_DATA_FAILED
@@ -637,20 +632,17 @@
             # int status = suc ? 0 : BlufiCallback.CODE_WRITE_DATA_FAILED
             # onPostCustomDataResult(status, data)
             print(suc)
             print(data)
         except Exception as err:
             print(err)
 
-
-
     def getTypeValue(self, type: int, subtype: int):
         return (subtype << 2) | type
 
-
     async def post(self, encrypt: bool, checksum: bool, require_ack: bool, type_of: int, data: bytearray) -> bool:
         if data is None:
             return await self.postNonData(encrypt, checksum, require_ack, type_of)
 
         return await self.postContainsData(encrypt, checksum, require_ack, type_of, data)
 
     async def gattWrite(self, data: bytearray) -> bool:
@@ -658,33 +650,30 @@
 
     async def postNonData(self, encrypt: bool, checksum: bool, require_ack: bool, type_of: int) -> bool:
         sequence = self.generateSendSequence()
         postBytes = self.getPostBytes(type_of, encrypt, checksum, require_ack, False, sequence, None)
         posted = await self.gattWrite(postBytes)
         return posted and (not require_ack or self.receiveAck(sequence))
 
-
-    async def postContainsData(self, encrypt: bool,  checksum: bool,  require_ack: bool,  type_of: int, data: bytearray) -> bool:
+    async def postContainsData(self, encrypt: bool, checksum: bool, require_ack: bool, type_of: int,
+                               data: bytearray) -> bool:
         print("post contains data")
         print(data)
-        chunk_size = 200 # self.client.mtu_size - 3
+        chunk_size = 200  # self.client.mtu_size - 3
 
         chunks = list()
         for i in range(0, len(data), chunk_size):
-            if(i + chunk_size > len(data)):
+            if (i + chunk_size > len(data)):
                 chunks.append(data[i: len(data)])
             else:
-                chunks.append(data[i : i + chunk_size])
-        print("chunks")
-        print(len(chunks))
-        print(chunks)
+                chunks.append(data[i: i + chunk_size])
         for index, chunk in enumerate(chunks):
             print("entered for loop")
             # frag = i < len(data)
-            frag = index != len(chunks)-1
+            frag = index != len(chunks) - 1
             sequence = self.generateSendSequence()
             postBytes = self.getPostBytes(type_of, encrypt, checksum, require_ack, frag, sequence, chunk)
 
             posted = await self.gattWrite(postBytes)
             if (posted != None):
                 return False
 
@@ -693,82 +682,78 @@
                 return not require_ack or self.receiveAck(sequence)
 
             if (require_ack and not self.receiveAck(sequence)):
                 return False
             else:
                 await sleep(0.01)
 
-
-
-
-    def getPostBytes(self, type: int,  encrypt: bool, checksum: bool,  require_ack: bool,  hasFrag: bool, sequence: int, data: bytearray) -> bytearray:
+    def getPostBytes(self, type: int, encrypt: bool, checksum: bool, require_ack: bool, hasFrag: bool, sequence: int,
+                     data: bytearray) -> bytearray:
 
         byteOS = BytesIO()
         dataLength = (0 if data == None else len(data))
         frameCtrl = FrameCtrlData.getFrameCTRLValue(encrypt, checksum, 0, require_ack, hasFrag)
-        byteOS.write(type.to_bytes(1,sys.byteorder))
+        byteOS.write(type.to_bytes(1, sys.byteorder))
         byteOS.write(frameCtrl.to_bytes(1, sys.byteorder))
         byteOS.write(sequence.to_bytes(1, sys.byteorder))
         byteOS.write(dataLength.to_bytes(1, sys.byteorder))
 
         if (data != None):
             byteOS.write(data)
 
-
         print(byteOS.getvalue())
         return byteOS.getvalue()
 
-
     def parseNotification(self, response: bytearray):
         dataOffset = None
         if (response is None):
-            #Log.w(TAG, "parseNotification null data");
+            # Log.w(TAG, "parseNotification null data");
             return -1
 
         # if (this.mPrintDebug):
         #     Log.d(TAG, "parseNotification Notification= " + Arrays.toString(response));
         # }
         if (len(response) >= 4):
-            sequence = int(response[2]) # toInt
+            sequence = int(response[2])  # toInt
             # self.mReadSequence_1.incrementAndGet()
             if (sequence != (next(self.mReadSequence) & 255)):
                 print("parseNotification read sequence wrong")
                 self.mReadSequence = sequence
                 # Log.w(TAG, "parseNotification read sequence wrong")
                 # this is questionable
                 # self.mReadSequence = sequence
                 # self.mReadSequence_2.incrementAndGet()
 
             # LogUtil.m7773e(self.mGatt.getDevice().getName() + "打印丢包率", self.mReadSequence_2 + "/" + self.mReadSequence_1);
-            pkt_type = int(response[0]) # toInt
+            pkt_type = int(response[0])  # toInt
             pkgType = self._getPackageType(pkt_type)
             subType = self._getSubType(pkt_type)
             self.notification.setType(pkt_type)
             self.notification.setPkgType(pkgType)
             self.notification.setSubType(subType)
-            frameCtrl = int(response[1]) # toInt
+            frameCtrl = int(response[1])  # toInt
             print("frame ctrl")
             print(frameCtrl)
             print(response)
             print(f"pktType {pkt_type} pkgType {pkgType} subType {subType}")
             self.notification.setFrameCtrl(frameCtrl)
             frameCtrlData = FrameCtrlData(frameCtrl)
-            dataLen = int(response[3]) # toInt specifies length of data
+            dataLen = int(response[3])  # toInt specifies length of data
             dataBytes = None
 
             try:
 
-                dataBytes = response[4:4+dataLen]
+                dataBytes = response[4: 4 + dataLen]
                 if (frameCtrlData.isEncrypted()):
                     print("is encypted")
                 #     BlufiAES aes = new BlufiAES(self.mAESKey, AES_TRANSFORMATION, generateAESIV(sequence));
                 #     dataBytes = aes.decrypt(dataBytes);
                 # }
                 if (frameCtrlData.isChecksum()):
-                     print("checksum")
+                    print("checksum")
                 #     int respChecksum1 = toInt(response[response.length - 1]);
                 #     int respChecksum2 = toInt(response[response.length - 2]);
                 #     int crc = BlufiCRC.calcCRC(BlufiCRC.calcCRC(0, new byte[]{(byte) sequence, (byte) dataLen}), dataBytes);
                 #     int calcChecksum1 = (crc >> 8) & 255;
                 #     int calcChecksum2 = crc & 255;
                 #     if (respChecksum1 != calcChecksum1 || respChecksum2 != calcChecksum2) {
                 #         Log.w(TAG, "parseNotification: read invalid checksum");
@@ -787,63 +772,63 @@
 
                 self.notification.addData(dataBytes, dataOffset)
                 return 1 if frameCtrlData.hasFrag() else 0
             except Exception as e:
                 print(e)
                 return -100
 
-
         # Log.w(TAG, "parseNotification data length less than 4");
         return -2
 
-
     def parseBlufiNotifyData(self):
         pkgType = self.notification.getPkgType()
         subType = self.notification.getSubType()
         dataBytes = self.notification.getDataArray()
         print("parseBlufi")
         # print(dataBytes)
         # if (self.mUserBlufiCallback is not None):
         #     complete = self.mUserBlufiCallback.onGattNotification(self.mClient, pkgType, subType, dataBytes)
         #     if (complete):
         #         return
 
-
         if (pkgType == 0):
             self._parseCtrlData(subType, dataBytes)
         if (pkgType == 1):
             self._parseDataData(subType, dataBytes)
 
     def _parseCtrlData(self, subType: int, data: bytearray):
         pass
-        #self._parseAck(data)
+        # self._parseAck(data)
 
     def _parseDataData(self, subType: int, data: bytearray):
-    #     if (subType == 0) {
-    #         this.mSecurityCallback.onReceiveDevicePublicKey(data);
-    #         return;
-    #     }
+        #     if (subType == 0) {
+        #         this.mSecurityCallback.onReceiveDevicePublicKey(data);
+        #         return;
+        #     }
+        print(subType)
+        print(bytearray)
         match subType:
-    #         case 15:
-    #             parseWifiState(data);
-    #             return;
-    #         case 16:
-    #             parseVersion(data);
-    #             return;
-    #         case 17:
-    #             parseWifiScanList(data);
-    #             return;
-    #         case 18:
-    #             int errCode = data.length > 0 ? 255 & data[0] : 255;
-    #             onError(errCode);
-    #             return;
+            #         case 15:
+            #             parseWifiState(data);
+            #             return;
+            #         case 16:
+            #             parseVersion(data);
+            #             return;
+            #         case 17:
+            #             parseWifiScanList(data);
+            #             return;
+            #         case 18:
+            #             int errCode = data.length > 0 ? 255 & data[0] : 255;
+            #             onError(errCode);
+            #             return;
             case 19:
-    #             # com/agilexrobotics/utils/EspBleUtil$BlufiCallbackMain.smali
-                parseCustomData(data) #parse to protobuf message
-                #onReceiveCustomData
+                #             # com/agilexrobotics/utils/EspBleUtil$BlufiCallbackMain.smali
+                parseCustomData(data)  # parse to protobuf message
+
+    # onReceiveCustomData
     #             return;
     #         default:
     #             return;
     #     }
     # }
 
     # private void parseCtrlData(int i, byte[] bArr) {
@@ -852,65 +837,53 @@
     #     }
     # }
 
     # private void parseAck(byte[] bArr) {
     #     this.mAck.add(Integer.valueOf(bArr.length > 0 ? bArr[0] & 255 : 256));
     # }
 
-
     def receiveAck(self, expectAck: int) -> bool:
         try:
             ack = next(self.mAck)
             return ack == expectAck
         except Exception as err:
             print(err)
             return False
 
-
     def generateSendSequence(self):
         return next(self.mSendSequence) & 255
 
-
     def getJsonString(self, cmd: int) -> str:
         jSONObject = {}
         try:
             jSONObject["cmd"] = cmd
             jSONObject[tmp_constant.REQUEST_ID] = int(time.time())
             return json.dumps(jSONObject)
         except Exception as err:
 
             return ""
 
-
     def get_json_string(self, cmd: int, hash_map: Dict[str, object]) -> str:
         jSONObject = {}
         try:
             jSONObject["cmd"] = cmd
             jSONObject[tmp_constant.REQUEST_ID] = int(time.time())
             jSONObject2 = {}
             for key, value in hash_map.items():
                 jSONObject2[key] = value
             jSONObject["params"] = jSONObject2
             return json.dumps(jSONObject)
         except Exception as e:
             print(e)
             return ""
 
-
-
     def current_milli_time(self):
         return round(time.time() * 1000)
 
-
     def _getTypeValue(self, type: int, subtype: int):
         return (subtype << 2) | type
 
-
     def _getPackageType(self, typeValue: int):
         return typeValue & 3
 
-
     def _getSubType(self, typeValue: int):
         return (typeValue & 252) >> 2
-
-
-
```

### Comparing `pyluba-0.0.1/pyluba/bluetooth/const.py` & `pyluba-0.0.2/pyluba/bluetooth/const.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/bluetooth/data/convert.py` & `pyluba-0.0.2/pyluba/bluetooth/data/convert.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     # setReceiveDeviceData
     
     
     
     luba_msg = luba_msg_pb2.LubaMsg()
     try:
         luba_msg.ParseFromString(data)
-        # print(luba_msg)
+        print(luba_msg)
         
         # toappGetHashAck = luba_msg.nav.toapp_get_commondata_ack
         # print(toappGetHashAck.Hash)
         
         if(luba_msg.HasField('sys')):
             store_sys_data(luba_msg.sys)
         elif(luba_msg.HasField('esp')):
@@ -60,14 +60,18 @@
         longValue10 = tard_state_data_list[6]
         longValue11 = tard_state_data_list[7]
 
         #device_state_map        
     if sys.HasField("system_rapid_state_tunnel"):
         rapid_state_data_list = sys.system_rapid_state_tunnel.rapid_state_data
         print(rapid_state_data_list)
+
+    if sys.HasField("toapp_batinfo"):
+        battery_info = sys.toapp_batinfo
+        print(battery_info)
         
         
 def store_nav_data(nav):
     if(nav.HasField('toapp_get_commondata_ack')):
         """has data about paths and zones"""   
         toapp_get_commondata_ack = nav.toapp_get_commondata_ack
         region_data = RegionData()
```

### Comparing `pyluba-0.0.1/pyluba/bluetooth/data/framectrldata.py` & `pyluba-0.0.2/pyluba/bluetooth/data/framectrldata.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/bluetooth/data/notifydata.py` & `pyluba-0.0.2/pyluba/bluetooth/data/notifydata.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/data/model/excute_boarder_params.py` & `pyluba-0.0.2/pyluba/data/model/excute_boarder_params.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/data/model/execute_boarder.py` & `pyluba-0.0.2/pyluba/data/model/execute_boarder.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/data/model/generate_route_information.py` & `pyluba-0.0.2/pyluba/data/model/generate_route_information.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/data/model/plan.py` & `pyluba-0.0.2/pyluba/data/model/plan.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/data/model/rapid_state.py` & `pyluba-0.0.2/pyluba/data/model/rapid_state.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/data/model/region_data.py` & `pyluba-0.0.2/pyluba/data/model/region_data.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/data/mqtt/event.py` & `pyluba-0.0.2/pyluba/data/mqtt/event.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/data/mqtt/properties.py` & `pyluba-0.0.2/pyluba/data/mqtt/properties.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/data/mqtt/status.py` & `pyluba-0.0.2/pyluba/data/mqtt/status.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/event/event.py` & `pyluba-0.0.2/pyluba/event/event.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/http/http.py` & `pyluba-0.0.2/pyluba/http/http.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/luba/base.py` & `pyluba-0.0.2/pyluba/luba/base.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/mqtt/mqtt.py` & `pyluba-0.0.2/pyluba/mqtt/mqtt.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/proto/common_pb2.py` & `pyluba-0.0.2/pyluba/proto/common_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/proto/esp_driver.proto` & `pyluba-0.0.2/pyluba/proto/esp_driver.proto`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/proto/esp_driver_pb2.py` & `pyluba-0.0.2/pyluba/proto/esp_driver_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/proto/luba_msg.proto` & `pyluba-0.0.2/pyluba/proto/luba_msg.proto`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/proto/luba_msg_pb2.py` & `pyluba-0.0.2/pyluba/proto/luba_msg_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/proto/mctrl_driver.proto` & `pyluba-0.0.2/pyluba/proto/mctrl_driver.proto`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/proto/mctrl_driver_pb2.py` & `pyluba-0.0.2/pyluba/proto/mctrl_driver_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/proto/mctrl_nav.proto` & `pyluba-0.0.2/pyluba/proto/mctrl_nav.proto`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/proto/mctrl_nav_pb2.py` & `pyluba-0.0.2/pyluba/proto/mctrl_nav_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/proto/mctrl_sys.proto` & `pyluba-0.0.2/pyluba/proto/mctrl_sys.proto`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/proto/mctrl_sys_pb2.py` & `pyluba-0.0.2/pyluba/proto/mctrl_sys_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/utility/constant/device_constant.py` & `pyluba-0.0.2/pyluba/utility/constant/device_constant.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/utility/periodic.py` & `pyluba-0.0.2/pyluba/utility/periodic.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyluba/utility/rocker_util.py` & `pyluba-0.0.2/pyluba/utility/rocker_util.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.1/pyproject.toml` & `pyluba-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name        = "pyluba"
-version     = "0.0.1"
+version     = "0.0.2"
 license     = "GNU-3.0"
 description = ""
 readme      = "README.md"
 authors     = [
     "Michael Arthur <michael@jumblesoft.co.nz>",
     "Jan Dalheimer <jan@dalheimer.de>"
 ]
 packages = [{include = "pyluba"}]
 
 
 [tool.poetry.dependencies]
-python = "~3.11"
+python = ">=3.11"
 bleak = "^0.21.1"
 protobuf = "^4.25.1"
 py-jsonic = "^0.0.2"
 pydantic = "^2.5.3"
 aliyun-python-sdk-iot = "^8.57.0"
 aliyun-iot-linkkit = "^1.2.12"
 aiohttp = "^3.9.1"
```

### Comparing `pyluba-0.0.1/PKG-INFO` & `pyluba-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pyluba
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 License: GNU-3.0
 Author: Michael Arthur
 Author-email: michael@jumblesoft.co.nz
-Requires-Python: >=3.11,<3.12
+Requires-Python: >=3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.1,<4.0.0)
 Requires-Dist: alibabacloud-apigateway-util (>=0.0.2,<0.0.3)
 Requires-Dist: alibabacloud-iot-api-gateway (>=0.0.4,<0.0.5)
 Requires-Dist: alicloud-gateway-iot (>=1.0.0,<2.0.0)
 Requires-Dist: aliyun-iot-linkkit (>=1.2.12,<2.0.0)
 Requires-Dist: aliyun-python-sdk-iot (>=8.57.0,<9.0.0)
 Requires-Dist: bleak (>=0.21.1,<0.22.0)
```


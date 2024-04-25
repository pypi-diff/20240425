# Comparing `tmp/pyrisco-0.6.0.tar.gz` & `tmp/pyrisco-0.7.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrisco-0.6.0.tar", last modified: Sat Mar 23 09:32:29 2024, max compression
+gzip compressed data, was "pyrisco-0.7.0rc0.tar", last modified: Thu Apr 25 15:05:00 2024, max compression
```

## Comparing `pyrisco-0.6.0.tar` & `pyrisco-0.7.0rc0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2024-03-23 09:32:29.701801 pyrisco-0.6.0/
--rw-r--r--   0 onfreund   (501) staff       (20)     1065 2021-08-21 12:09:24.000000 pyrisco-0.6.0/LICENSE
--rw-r--r--   0 onfreund   (501) staff       (20)       25 2021-08-21 12:09:24.000000 pyrisco-0.6.0/MANIFEST.in
--rw-r--r--   0 onfreund   (501) staff       (20)     3030 2024-03-23 09:32:29.701168 pyrisco-0.6.0/PKG-INFO
--rw-r--r--   0 onfreund   (501) staff       (20)     2363 2022-07-23 14:50:37.000000 pyrisco-0.6.0/README.md
-drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2024-03-23 09:32:29.683693 pyrisco-0.6.0/pyrisco/
--rw-r--r--   0 onfreund   (501) staff       (20)      148 2022-07-23 14:51:59.000000 pyrisco-0.6.0/pyrisco/__init__.py
-drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2024-03-23 09:32:29.692037 pyrisco-0.6.0/pyrisco/cloud/
--rw-r--r--   0 onfreund   (501) staff       (20)       36 2022-07-23 14:51:32.000000 pyrisco-0.6.0/pyrisco/cloud/__init__.py
--rw-r--r--   0 onfreund   (501) staff       (20)      687 2022-07-23 08:48:17.000000 pyrisco-0.6.0/pyrisco/cloud/alarm.py
--rw-r--r--   0 onfreund   (501) staff       (20)     1860 2022-07-23 08:48:17.000000 pyrisco-0.6.0/pyrisco/cloud/event.py
--rw-r--r--   0 onfreund   (501) staff       (20)     1532 2022-07-23 08:48:17.000000 pyrisco-0.6.0/pyrisco/cloud/partition.py
--rw-r--r--   0 onfreund   (501) staff       (20)     6109 2022-08-03 19:38:59.000000 pyrisco-0.6.0/pyrisco/cloud/risco_cloud.py
--rw-r--r--   0 onfreund   (501) staff       (20)      790 2022-07-23 08:48:17.000000 pyrisco-0.6.0/pyrisco/cloud/zone.py
--rw-r--r--   0 onfreund   (501) staff       (20)     2891 2024-03-23 09:28:16.000000 pyrisco-0.6.0/pyrisco/common.py
-drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2024-03-23 09:32:29.699376 pyrisco-0.6.0/pyrisco/local/
--rw-r--r--   0 onfreund   (501) staff       (20)       36 2022-07-23 14:52:55.000000 pyrisco-0.6.0/pyrisco/local/__init__.py
--rw-r--r--   0 onfreund   (501) staff       (20)      161 2022-07-23 08:48:17.000000 pyrisco-0.6.0/pyrisco/local/const.py
--rw-r--r--   0 onfreund   (501) staff       (20)     1969 2024-02-14 09:05:38.000000 pyrisco-0.6.0/pyrisco/local/panels.py
--rw-r--r--   0 onfreund   (501) staff       (20)     1849 2022-07-27 14:11:25.000000 pyrisco-0.6.0/pyrisco/local/partition.py
--rw-r--r--   0 onfreund   (501) staff       (20)     5365 2022-09-15 12:11:59.000000 pyrisco-0.6.0/pyrisco/local/risco_crypt.py
--rw-r--r--   0 onfreund   (501) staff       (20)     7272 2024-03-08 07:54:03.000000 pyrisco-0.6.0/pyrisco/local/risco_local.py
--rw-r--r--   0 onfreund   (501) staff       (20)     5176 2024-03-08 07:54:03.000000 pyrisco-0.6.0/pyrisco/local/risco_socket.py
--rw-r--r--   0 onfreund   (501) staff       (20)     1097 2024-03-23 09:28:48.000000 pyrisco-0.6.0/pyrisco/local/system.py
--rw-r--r--   0 onfreund   (501) staff       (20)     1647 2022-11-04 12:33:58.000000 pyrisco-0.6.0/pyrisco/local/zone.py
-drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2024-03-23 09:32:29.700302 pyrisco-0.6.0/pyrisco.egg-info/
--rw-r--r--   0 onfreund   (501) staff       (20)     3030 2024-03-23 09:32:29.000000 pyrisco-0.6.0/pyrisco.egg-info/PKG-INFO
--rw-r--r--   0 onfreund   (501) staff       (20)      614 2024-03-23 09:32:29.000000 pyrisco-0.6.0/pyrisco.egg-info/SOURCES.txt
--rw-r--r--   0 onfreund   (501) staff       (20)        1 2024-03-23 09:32:29.000000 pyrisco-0.6.0/pyrisco.egg-info/dependency_links.txt
--rw-r--r--   0 onfreund   (501) staff       (20)        8 2024-03-23 09:32:29.000000 pyrisco-0.6.0/pyrisco.egg-info/requires.txt
--rw-r--r--   0 onfreund   (501) staff       (20)        8 2024-03-23 09:32:29.000000 pyrisco-0.6.0/pyrisco.egg-info/top_level.txt
--rw-r--r--   0 onfreund   (501) staff       (20)       38 2024-03-23 09:32:29.701904 pyrisco-0.6.0/setup.cfg
--rw-r--r--   0 onfreund   (501) staff       (20)     3379 2024-03-23 09:32:04.000000 pyrisco-0.6.0/setup.py
+drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2024-04-25 15:05:00.613818 pyrisco-0.7.0rc0/
+-rw-r--r--   0 onfreund   (501) staff       (20)     1065 2021-08-21 12:09:24.000000 pyrisco-0.7.0rc0/LICENSE
+-rw-r--r--   0 onfreund   (501) staff       (20)       25 2021-08-21 12:09:24.000000 pyrisco-0.7.0rc0/MANIFEST.in
+-rw-r--r--   0 onfreund   (501) staff       (20)     3033 2024-04-25 15:05:00.612351 pyrisco-0.7.0rc0/PKG-INFO
+-rw-r--r--   0 onfreund   (501) staff       (20)     2363 2022-07-23 14:50:37.000000 pyrisco-0.7.0rc0/README.md
+drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2024-04-25 15:05:00.582764 pyrisco-0.7.0rc0/pyrisco/
+-rw-r--r--   0 onfreund   (501) staff       (20)      148 2022-07-23 14:51:59.000000 pyrisco-0.7.0rc0/pyrisco/__init__.py
+drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2024-04-25 15:05:00.597377 pyrisco-0.7.0rc0/pyrisco/cloud/
+-rw-r--r--   0 onfreund   (501) staff       (20)       36 2022-07-23 14:51:32.000000 pyrisco-0.7.0rc0/pyrisco/cloud/__init__.py
+-rw-r--r--   0 onfreund   (501) staff       (20)      687 2022-07-23 08:48:17.000000 pyrisco-0.7.0rc0/pyrisco/cloud/alarm.py
+-rw-r--r--   0 onfreund   (501) staff       (20)     1860 2022-07-23 08:48:17.000000 pyrisco-0.7.0rc0/pyrisco/cloud/event.py
+-rw-r--r--   0 onfreund   (501) staff       (20)     1532 2022-07-23 08:48:17.000000 pyrisco-0.7.0rc0/pyrisco/cloud/partition.py
+-rw-r--r--   0 onfreund   (501) staff       (20)     6109 2022-08-03 19:38:59.000000 pyrisco-0.7.0rc0/pyrisco/cloud/risco_cloud.py
+-rw-r--r--   0 onfreund   (501) staff       (20)      790 2022-07-23 08:48:17.000000 pyrisco-0.7.0rc0/pyrisco/cloud/zone.py
+-rw-r--r--   0 onfreund   (501) staff       (20)     2891 2024-03-23 09:28:16.000000 pyrisco-0.7.0rc0/pyrisco/common.py
+drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2024-04-25 15:05:00.607351 pyrisco-0.7.0rc0/pyrisco/local/
+-rw-r--r--   0 onfreund   (501) staff       (20)       36 2022-07-23 14:52:55.000000 pyrisco-0.7.0rc0/pyrisco/local/__init__.py
+-rw-r--r--   0 onfreund   (501) staff       (20)      161 2022-07-23 08:48:17.000000 pyrisco-0.7.0rc0/pyrisco/local/const.py
+-rw-r--r--   0 onfreund   (501) staff       (20)     1969 2024-02-14 09:05:38.000000 pyrisco-0.7.0rc0/pyrisco/local/panels.py
+-rw-r--r--   0 onfreund   (501) staff       (20)     1849 2022-07-27 14:11:25.000000 pyrisco-0.7.0rc0/pyrisco/local/partition.py
+-rw-r--r--   0 onfreund   (501) staff       (20)     5365 2022-09-15 12:11:59.000000 pyrisco-0.7.0rc0/pyrisco/local/risco_crypt.py
+-rw-r--r--   0 onfreund   (501) staff       (20)     7352 2024-04-25 15:04:36.000000 pyrisco-0.7.0rc0/pyrisco/local/risco_local.py
+-rw-r--r--   0 onfreund   (501) staff       (20)     5202 2024-04-25 15:04:36.000000 pyrisco-0.7.0rc0/pyrisco/local/risco_socket.py
+-rw-r--r--   0 onfreund   (501) staff       (20)     1097 2024-03-23 09:28:48.000000 pyrisco-0.7.0rc0/pyrisco/local/system.py
+-rw-r--r--   0 onfreund   (501) staff       (20)     1647 2022-11-04 12:33:58.000000 pyrisco-0.7.0rc0/pyrisco/local/zone.py
+drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2024-04-25 15:05:00.609390 pyrisco-0.7.0rc0/pyrisco.egg-info/
+-rw-r--r--   0 onfreund   (501) staff       (20)     3033 2024-04-25 15:05:00.000000 pyrisco-0.7.0rc0/pyrisco.egg-info/PKG-INFO
+-rw-r--r--   0 onfreund   (501) staff       (20)      614 2024-04-25 15:05:00.000000 pyrisco-0.7.0rc0/pyrisco.egg-info/SOURCES.txt
+-rw-r--r--   0 onfreund   (501) staff       (20)        1 2024-04-25 15:05:00.000000 pyrisco-0.7.0rc0/pyrisco.egg-info/dependency_links.txt
+-rw-r--r--   0 onfreund   (501) staff       (20)        8 2024-04-25 15:05:00.000000 pyrisco-0.7.0rc0/pyrisco.egg-info/requires.txt
+-rw-r--r--   0 onfreund   (501) staff       (20)        8 2024-04-25 15:05:00.000000 pyrisco-0.7.0rc0/pyrisco.egg-info/top_level.txt
+-rw-r--r--   0 onfreund   (501) staff       (20)       38 2024-04-25 15:05:00.613990 pyrisco-0.7.0rc0/setup.cfg
+-rw-r--r--   0 onfreund   (501) staff       (20)     3383 2024-04-25 15:03:18.000000 pyrisco-0.7.0rc0/setup.py
```

### Comparing `pyrisco-0.6.0/LICENSE` & `pyrisco-0.7.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.0/PKG-INFO` & `pyrisco-0.7.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrisco
-Version: 0.6.0
+Version: 0.7.0rc0
 Summary: A python library to communicate with Risco Cloud.
 Home-page: https://github.com/OnFreund/PyRisco
 Author: On Freund
 Author-email: onfreund@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pyrisco-0.6.0/README.md` & `pyrisco-0.7.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.0/pyrisco/cloud/alarm.py` & `pyrisco-0.7.0rc0/pyrisco/cloud/alarm.py`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.0/pyrisco/cloud/event.py` & `pyrisco-0.7.0rc0/pyrisco/cloud/event.py`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.0/pyrisco/cloud/partition.py` & `pyrisco-0.7.0rc0/pyrisco/cloud/partition.py`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.0/pyrisco/cloud/risco_cloud.py` & `pyrisco-0.7.0rc0/pyrisco/cloud/risco_cloud.py`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.0/pyrisco/cloud/zone.py` & `pyrisco-0.7.0rc0/pyrisco/cloud/zone.py`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.0/pyrisco/common.py` & `pyrisco-0.7.0rc0/pyrisco/common.py`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.0/pyrisco/local/panels.py` & `pyrisco-0.7.0rc0/pyrisco/local/panels.py`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.0/pyrisco/local/partition.py` & `pyrisco-0.7.0rc0/pyrisco/local/partition.py`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.0/pyrisco/local/risco_crypt.py` & `pyrisco-0.7.0rc0/pyrisco/local/risco_crypt.py`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.0/pyrisco/local/risco_local.py` & `pyrisco-0.7.0rc0/pyrisco/local/risco_local.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,16 +108,16 @@
     handlers.append(handler)
     def _remove():
       handlers.remove(handler)
     return _remove
 
   async def _init_system(self):
     try:
-      label = await self._rs.send_result_command(f'SYSLBL?')
-      status = await self._rs.send_result_command(f'SSTT?')
+      label = await self._rs.send_result_command_limited(f'SYSLBL?')
+      status = await self._rs.send_result_command_limited(f'SSTT?')
     except OperationError:
       return None
     return System(self, label, status)
 
   async def _init_partitions(self):
     return await self._get_objects(1, self._panel_capabilities[MAX_PARTS], self._create_partition)
 
@@ -127,46 +127,46 @@
   async def _get_objects(self, min, max, func):
     ids = range(min, min+max)
     temp = await asyncio.gather(*[func(i) for i in ids])
     return { o.id: o for o in temp if o }
 
   async def _create_partition(self, partition_id):
     try:
-      status = await self._rs.send_result_command(f'PSTT{partition_id}?')
+      status = await self._rs.send_result_command_limited(f'PSTT{partition_id}?')
       if not 'E' in status:
         return None
 
-      label = await self._rs.send_result_command(f'PLBL{partition_id}?')
+      label = await self._rs.send_result_command_limited(f'PLBL{partition_id}?')
     except OperationError:
       return None
     return Partition(self, partition_id, label, status)
 
   async def _create_zone(self, zone_id):
     try:
-      zone_type = int(await self._rs.send_result_command(f'ZTYPE*{zone_id}?'))
+      zone_type = int(await self._rs.send_result_command_limited(f'ZTYPE*{zone_id}?'))
       if zone_type == 0:
         return None
 
       if self._legacy_panel:
         tech = ''
       else:
-        tech = await self._rs.send_result_command(f'ZLNKTYP{zone_id}?')
+        tech = await self._rs.send_result_command_limited(f'ZLNKTYP{zone_id}?')
         if tech.strip() == 'N':
           return None
 
-      status = await self._rs.send_result_command(f'ZSTT*{zone_id}?')
+      status = await self._rs.send_result_command_limited(f'ZSTT*{zone_id}?')
       if status.endswith('N'):
         return None
 
-      label = await self._rs.send_result_command(f'ZLBL*{zone_id}?')
-      partitions = await self._rs.send_result_command(f'ZPART&*{zone_id}?')
+      label = await self._rs.send_result_command_limited(f'ZLBL*{zone_id}?')
+      partitions = await self._rs.send_result_command_limited(f'ZPART&*{zone_id}?')
       if self._legacy_panel:
         groups = '0'
       else:
-        groups = await self._rs.send_result_command(f'ZAREA&*{zone_id}?')
+        groups = await self._rs.send_result_command_limited(f'ZAREA&*{zone_id}?')
 
       return Zone(self, zone_id, status, zone_type, label, partitions, groups, tech)
     except OperationError:
       return None
 
   def _system_status(self, status):
     self._system.update_status(status)
```

### Comparing `pyrisco-0.6.0/pyrisco/local/risco_socket.py` & `pyrisco-0.7.0rc0/pyrisco/local/risco_socket.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,41 +94,45 @@
     command = await self.send_command(command)
     return command == 'ACK'
 
   async def send_result_command(self, command):
     command = await self.send_command(command)
     return command.split("=")[1]
 
-  async def send_command(self, command, force_encryption=False):
+  async def send_result_command_limited(self, command):
     async with self._semaphore:
-      self._increment_cmd_id()
-      cmd_id = self._cmd_id
-      future = asyncio.Future()
-      self._futures[cmd_id-1] = future
-      self._write_command(cmd_id, command, force_encryption)
-      try:
-        return await asyncio.wait_for(future, 1)
-      except asyncio.TimeoutError:
-        raise OperationError(f'Timeout in command: {command}')
+      return await self.send_result_command(command)
+
+  async def send_command(self, command):
+    self._increment_cmd_id()
+    cmd_id = self._cmd_id
+    future = asyncio.Future()
+    self._futures[cmd_id-1] = future
+    self._write_command(cmd_id, command)
+    try:
+      async with asyncio.timeout(1):
+        return await future
+    except asyncio.TimeoutError:
+      raise OperationError(f'Timeout in command: {command}')
 
   async def _handle_incoming(self, cmd_id, command, crc):
     self._write_command(cmd_id, 'ACK')
     if not crc:
       await self._queue.put(OperationError(f'cmd_id: {cmd_id}, Wrong CRC'))
     else:
       await self._queue.put(command)
 
   async def _read_command(self):
     buffer = await self._reader.readuntil(END)
     while buffer.endswith(ESCAPED_END):
       buffer += await self._reader.readuntil(END)
     return self._crypt.decode(buffer)
 
-  def _write_command(self, cmd_id, command, force_encryption=False):
-    buffer = self._crypt.encode(cmd_id, command, force_encryption)
+  def _write_command(self, cmd_id, command):
+    buffer = self._crypt.encode(cmd_id, command)
     self._writer.write(buffer)
 
   async def _close(self):
     if self._keep_alive_task:
       self._keep_alive_task.cancel()
       self._keep_alive_task = None
```

### Comparing `pyrisco-0.6.0/pyrisco/local/system.py` & `pyrisco-0.7.0rc0/pyrisco/local/system.py`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.0/pyrisco/local/zone.py` & `pyrisco-0.7.0rc0/pyrisco/local/zone.py`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.0/pyrisco.egg-info/PKG-INFO` & `pyrisco-0.7.0rc0/pyrisco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrisco
-Version: 0.6.0
+Version: 0.7.0rc0
 Summary: A python library to communicate with Risco Cloud.
 Home-page: https://github.com/OnFreund/PyRisco
 Author: On Freund
 Author-email: onfreund@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pyrisco-0.6.0/pyrisco.egg-info/SOURCES.txt` & `pyrisco-0.7.0rc0/pyrisco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.0/setup.py` & `pyrisco-0.7.0rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'pyrisco'
 DESCRIPTION = 'A python library to communicate with Risco Cloud.'
 URL = 'https://github.com/OnFreund/PyRisco'
 EMAIL = 'onfreund@gmail.com'
 AUTHOR = 'On Freund'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '0.6.0'
+VERSION = '0.7.0-rc0'
 
 REQUIRED = ['aiohttp']
 
 EXTRAS = {}
 
 
 here = os.path.abspath(os.path.dirname(__file__))
```


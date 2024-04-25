# Comparing `tmp/coppeliasim_zmqremoteapi_client-2.0.3.tar.gz` & `tmp/coppeliasim_zmqremoteapi_client-2.0.4.tar.gz`

## Comparing `coppeliasim_zmqremoteapi_client-2.0.3.tar` & `coppeliasim_zmqremoteapi_client-2.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.3/.flake8
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.3/imageStreaming.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.3/opencv.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.3/pController.py
--rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.3/simpleMovement.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.3/simpleTest-nonBlocking.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.3/simpleTest.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.3/synchronousImageTransmission.py
--rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.3/test1.py
--rw-r--r--   0        0        0    13747 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.3/test2.py
--rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.3/src/coppeliasim_zmqremoteapi_client/__init__.py
--rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.3/src/coppeliasim_zmqremoteapi_client/asyncio/__init__.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.3/zmqRemoteApi/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.3/zmqRemoteApi/asyncio/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.3/.gitignore
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.3/LICENSE
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.3/README.md
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.4/.flake8
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.4/imageStreaming.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.4/opencv.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.4/pController.py
+-rw-r--r--   0        0        0     5069 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.4/simpleMovement.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.4/simpleTest-nonBlocking.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.4/simpleTest.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.4/synchronousImageTransmission.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.4/test1.py
+-rw-r--r--   0        0        0    13747 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.4/test2.py
+-rw-r--r--   0        0        0    10626 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.4/src/coppeliasim_zmqremoteapi_client/__init__.py
+-rw-r--r--   0        0        0    10661 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.4/src/coppeliasim_zmqremoteapi_client/asyncio/__init__.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.4/zmqRemoteApi/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.4/zmqRemoteApi/asyncio/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.4/.gitignore
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.4/LICENSE
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.4/README.md
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-2.0.4/PKG-INFO
```

### Comparing `coppeliasim_zmqremoteapi_client-2.0.3/imageStreaming.py` & `coppeliasim_zmqremoteapi_client-2.0.4/imageStreaming.py`

 * *Files identical despite different names*

### Comparing `coppeliasim_zmqremoteapi_client-2.0.3/opencv.py` & `coppeliasim_zmqremoteapi_client-2.0.4/opencv.py`

 * *Files identical despite different names*

### Comparing `coppeliasim_zmqremoteapi_client-2.0.3/pController.py` & `coppeliasim_zmqremoteapi_client-2.0.4/pController.py`

 * *Files identical despite different names*

### Comparing `coppeliasim_zmqremoteapi_client-2.0.3/simpleMovement.py` & `coppeliasim_zmqremoteapi_client-2.0.4/simpleMovement.py`

 * *Files 16% similar despite different names*

```diff
@@ -85,49 +85,48 @@
     maxJerk = [jerk, jerk, jerk, jerk]
     
     initTr = sim.getObjectPose(targetHandle)
 
     for i in range(1):
         goalTr = initTr.copy()
         goalTr[2] = goalTr[2] + 0.2
-        sim.moveToPose(-1, initTr, maxVel, maxAccel, maxJerk, goalTr, poseCallback, {'robotColor': robotColor, 'handle': targetHandle})
+        params = {}
+        params['object'] = targetHandle
+        params['targetPose'] = goalTr
+        params['maxVel'] = maxVel
+        params['maxAccel'] = maxAccel
+        params['maxJerk'] = maxJerk
+        sim.moveToPose(params) # one could also use sim.moveToPose_init, sim.moveToPose_step and sim.moveToPose_cleanup
         
-        startTr = sim.getObjectPose(targetHandle)
         goalTr[2] = goalTr[2] - 0.2
-        sim.moveToPose(-1, startTr, maxVel, maxAccel, maxJerk, goalTr, poseCallback, {'robotColor': robotColor, 'handle': targetHandle})
+        params['targetPose'] = goalTr
+        sim.moveToPose(params)
         
         startTr = sim.getObjectPose(targetHandle)
         goalTr = sim.rotateAroundAxis(goalTr, [1, 0, 0], [startTr[0], startTr[1], startTr[2]], 90 * math.pi / 180)
-        sim.moveToPose(-1, startTr, maxVel, maxAccel, maxJerk, goalTr, poseCallback, {'robotColor': robotColor, 'handle': targetHandle})
+        params['targetPose'] = goalTr
+        sim.moveToPose(params)
 
-        startTr = sim.getObjectPose(targetHandle)
-        sim.moveToPose(-1, startTr, maxVel, maxAccel, maxJerk, initTr, poseCallback, {'robotColor': robotColor, 'handle': targetHandle})
+        params['targetPose'] = initTr
+        sim.moveToPose(params)
     
     sim.setStepping(False)
     
-def poseCallback(tr, vel, accel, data):
-    sim = sims[data['robotColor']]
-    handle = data['handle']
-    sim.setObjectPose(handle, tr)
-
-def confCallback(config, vel, accel, data):
-    sim = sims[data['robotColor']]
-    handles = data['handles']
-    for i in range(len(handles)):
-        if sim.isDynamicallyEnabled(handles[i]):
-            sim.setJointTargetPosition(handles[i], config[i])
-        else:
-            sim.setJointPosition(handles[i], config[i])
-
 def moveToConfig(robotColor, handles, maxVel, maxAccel, maxJerk, targetConf):
     sim = sims[robotColor]
     currentConf = []
     for i in range(len(handles)):
         currentConf.append(sim.getJointPosition(handles[i]))
-    sim.moveToConfig(-1, currentConf, None, None, maxVel, maxAccel, maxJerk, targetConf, None, confCallback, {'robotColor': robotColor, 'handles': handles}, None)
+    params = {}
+    params['joints'] = handles
+    params['targetPos'] = targetConf
+    params['maxVel'] = maxVel
+    params['maxAccel'] = maxAccel
+    params['maxJerk'] = maxJerk
+    sim.moveToConfig(params) # one could also use sim.moveToConfig_init, sim.moveToConfig_step and sim.moveToConfig_cleanup
 
 print('Program started')
 client = RemoteAPIClient()
 sim = client.require('sim')
 
 sim.loadScene(sim.getStringParam(sim.stringparam_scenedefaultdir) + '/messaging/movementViaRemoteApi.ttt')
```

### Comparing `coppeliasim_zmqremoteapi_client-2.0.3/simpleTest-nonBlocking.py` & `coppeliasim_zmqremoteapi_client-2.0.4/simpleTest-nonBlocking.py`

 * *Files identical despite different names*

### Comparing `coppeliasim_zmqremoteapi_client-2.0.3/simpleTest.py` & `coppeliasim_zmqremoteapi_client-2.0.4/simpleTest.py`

 * *Files identical despite different names*

### Comparing `coppeliasim_zmqremoteapi_client-2.0.3/synchronousImageTransmission.py` & `coppeliasim_zmqremoteapi_client-2.0.4/synchronousImageTransmission.py`

 * *Files identical despite different names*

### Comparing `coppeliasim_zmqremoteapi_client-2.0.3/test1.py` & `coppeliasim_zmqremoteapi_client-2.0.4/test1.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,20 @@
 
 client = RemoteAPIClient()
 client.timeout = 5
 
 sim = client.require('sim')
 simIK = client.require('simIK')
 
+a = [1,2,3]
+b = sim.packFloatTable(a)
+c = sim.unpackFloatTable(b)
+print(a)
+print(c)
+
 sim.loadScene('')
 
 simIK.createEnvironment()
 
 a = np.random.uniform(-1, 1, 2)
 a = np.array(a, dtype=np.float32)
 x, y = a
```

### Comparing `coppeliasim_zmqremoteapi_client-2.0.3/test2.py` & `coppeliasim_zmqremoteapi_client-2.0.4/test2.py`

 * *Files identical despite different names*

### Comparing `coppeliasim_zmqremoteapi_client-2.0.3/src/coppeliasim_zmqremoteapi_client/asyncio/__init__.py` & `coppeliasim_zmqremoteapi_client-2.0.4/src/coppeliasim_zmqremoteapi_client/asyncio/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -158,15 +158,15 @@
             
             while isinstance(reply, dict) and 'func' in reply:
                 # We have a callback or a wait/repeat:
                 if reply['func'] == '_*wait*_':
                     func = '_*executed*_'
                     args = []
                     await self._send(socket, {'func': func, 'args': args})
-                else if reply['func'] == '_*repeat*_':
+                elif reply['func'] == '_*repeat*_':
                     await self._send(socket, {'func': func, 'args': args})
                 else:
                     if reply['func'] in self.callbackFuncs:
                         args = self.callbackFuncs[reply['func']](*reply['args'])
                     else:
                         funcToRun = _getFuncIfExists(reply['func'])
                         if funcToRun is not None:  # we cannot raise an error: e.g. a custom UI async callback cannot be assigned to a specific client
@@ -220,14 +220,73 @@
             return wrapper
 
         def custom_getattr(d, func):
             return outer_function(func)
 
         return type('ScriptFunctionWrapper', (object,), {'__getattr__': custom_getattr})()
         
+    def copyTable(self, table):
+        import copy 
+        return copy.deepcopy(table)
+        
+    def _packXTable(self, table, w, start, cnt):
+        import array
+        if cnt == 0:
+            cnt = len(table) - start
+        arr = array.array(w, table[start:(start + cnt)])
+        return arr.tobytes()
+
+    def _unpackXTable(self, data, w, start, cnt, off):
+        import array
+        arr = array.array(w)
+        start *= arr.itemsize
+        start += off
+        if cnt == 0:
+            cnt =  len(data) - start
+        else:
+            cnt *= arr.itemsize
+        arr.frombytes(data[start:(start + cnt)])
+        return list(arr)
+
+    def packUInt8Table(self, table, start=0, cnt=0):
+        return self._packXTable(table, 'B', start, cnt)
+
+    def unpackUInt8Table(self, data, start=0, cnt=0, off=0):
+        return self._unpackXTable(data, 'B', start, cnt, off)
+        
+    def packUInt16Table(self, table, start=0, cnt=0):
+        return self._packXTable(table, 'H', start, cnt)
+        
+    def unpackUInt16Table(self, data, start=0, cnt=0, off=0):
+        return self._unpackXTable(data, 'H', start, cnt, off)
+        
+    def packUInt32Table(self, table, start=0, cnt=0):
+        return self._packXTable(table, 'L', start, cnt)
+        
+    def unpackUInt32Table(self, data, start=0, cnt=0, off=0):
+        return self._unpackXTable(data, 'L', start, cnt, off)
+        
+    def packInt32Table(self, table, start=0, cnt=0):
+        return self._packXTable(table, 'l', start, cnt)
+        
+    def unpackInt32Table(self, data, start=0, cnt=0, off=0):
+        return self._unpackXTable(data, 'l', start, cnt, off)
+        
+    def packFloatTable(self, table, start=0, cnt=0):
+        return self._packXTable(table, 'f', start, cnt)
+        
+    def unpackFloatTable(self, data, start=0, cnt=0, off=0):
+        return self._unpackXTable(data, 'f', start, cnt, off)
+        
+    def packDoubleTable(self, table, start=0, cnt=0):
+        return self._packXTable(table, 'd', start, cnt)
+
+    def unpackDoubleTable(self, data, start=0, cnt=0, off=0):
+        return self._unpackXTable(data, 'd', start, cnt, off)
+        
     async def setStepping(self, enable=True):  # for backw. comp., now via sim.setStepping
         return await self.call('sim.setStepping', [enable])
 
     async def step(self, *, wait=True):  # for backw. comp., now via sim.step
         await self.call('sim.step', [wait])
```

### Comparing `coppeliasim_zmqremoteapi_client-2.0.3/LICENSE` & `coppeliasim_zmqremoteapi_client-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `coppeliasim_zmqremoteapi_client-2.0.3/README.md` & `coppeliasim_zmqremoteapi_client-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `coppeliasim_zmqremoteapi_client-2.0.3/pyproject.toml` & `coppeliasim_zmqremoteapi_client-2.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "coppeliasim_zmqremoteapi_client"
-version = "2.0.3"
+version = "2.0.4"
 authors = [
     { name="Federico Ferri (Coppelia Robotics)", email="federico@coppeliarobotics.com" },
 ]
 description = "Client for the CoppeliaSim's zmqRemoteApi (protocol version 2)"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `coppeliasim_zmqremoteapi_client-2.0.3/PKG-INFO` & `coppeliasim_zmqremoteapi_client-2.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: coppeliasim_zmqremoteapi_client
-Version: 2.0.3
+Version: 2.0.4
 Summary: Client for the CoppeliaSim's zmqRemoteApi (protocol version 2)
 Project-URL: Homepage, https://github.com/CoppeliaRobotics/zmqRemoteApi
 Project-URL: Bug Tracker, https://github.com/CoppeliaRobotics/zmqRemoteApi/issues
 Author-email: "Federico Ferri (Coppelia Robotics)" <federico@coppeliarobotics.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```


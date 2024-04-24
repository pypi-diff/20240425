# Comparing `tmp/nvidia-ml-py-7.346.0.tar.gz` & `tmp/nvidia-ml-py-7.352.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nvidia-ml-py-7.346.0.tar", last modified: Tue Mar 31 18:40:36 2015, max compression
+gzip compressed data, was "dist/nvidia-ml-py-7.352.0.tar", last modified: Tue Oct 13 23:18:46 2015, max compression
```

## Comparing `nvidia-ml-py-7.346.0.tar` & `nvidia-ml-py-7.352.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
-drwxr-xr-x   0 rphull    (1000) rphull    (1000)        0 2015-03-31 18:40:36.000000 nvidia-ml-py-7.346.0/
--rw-r--r--   0 rphull    (1000) rphull    (1000)      785 2015-03-31 18:40:36.000000 nvidia-ml-py-7.346.0/PKG-INFO
--rw-r--r--   0 rphull    (1000) rphull    (1000)     1226 2015-03-31 18:37:54.000000 nvidia-ml-py-7.346.0/setup.py
--r--r--r--   0 rphull    (1000) rphull    (1000)    36980 2015-03-31 18:30:19.000000 nvidia-ml-py-7.346.0/nvidia_smi.py
--r--r--r--   0 rphull    (1000) rphull    (1000)     5492 2015-03-31 18:36:14.000000 nvidia-ml-py-7.346.0/README.txt
--r--r--r--   0 rphull    (1000) rphull    (1000)    55353 2015-03-31 18:30:19.000000 nvidia-ml-py-7.346.0/pynvml.py
+drwxrwxr-x   0 rphull    (1000) rphull    (1000)        0 2015-10-13 23:18:46.000000 nvidia-ml-py-7.352.0/
+-r--r--r--   0 rphull    (1000) rphull    (1000)    37168 2015-10-13 22:19:19.000000 nvidia-ml-py-7.352.0/nvidia_smi.py
+-rw-rw-r--   0 rphull    (1000) rphull    (1000)     1226 2015-10-13 23:16:30.000000 nvidia-ml-py-7.352.0/setup.py
+-r--r--r--   0 rphull    (1000) rphull    (1000)    57174 2015-10-13 22:19:19.000000 nvidia-ml-py-7.352.0/pynvml.py
+-r--r--r--   0 rphull    (1000) rphull    (1000)     5592 2015-10-13 23:15:43.000000 nvidia-ml-py-7.352.0/README.txt
+-rw-rw-r--   0 rphull    (1000) rphull    (1000)      785 2015-10-13 23:18:46.000000 nvidia-ml-py-7.352.0/PKG-INFO
```

### Comparing `nvidia-ml-py-7.346.0/PKG-INFO` & `nvidia-ml-py-7.352.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: nvidia-ml-py
-Version: 7.346.0
+Version: 7.352.0
 Summary: Python Bindings for the NVIDIA Management Library
 Home-page: http://www.nvidia.com/
 Author: NVIDIA Corporation
 Author-email: nvml-bindings@nvidia.com
 License: BSD
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `nvidia-ml-py-7.346.0/setup.py` & `nvidia-ml-py-7.352.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     from distutils.dist import DistributionMetadata
     DistributionMetadata.classifiers = None
     DistributionMetadata.download_url = None
 
 _package_name='nvidia-ml-py'
 
 setup(name=_package_name,
-      version='7.346.0',
+      version='7.352.0',
       description='Python Bindings for the NVIDIA Management Library',
       py_modules=['pynvml', 'nvidia_smi'],
       package_data={_package_name: ['Example.txt']},
       license="BSD",
       url="http://www.nvidia.com/",
       author="NVIDIA Corporation",
       author_email="nvml-bindings@nvidia.com",
```

### Comparing `nvidia-ml-py-7.346.0/nvidia_smi.py` & `nvidia-ml-py-7.352.0/nvidia_smi.py`

 * *Files 1% similar despite different names*

```diff
@@ -828,30 +828,33 @@
                         gpuUtilization = "%d %%" % stats.gpuUtilization
                         memoryUtilization = "%d %%" % stats.memoryUtilization
                         if (stats.maxMemoryUsage == None):
                             maxMemoryUsage = 'N\A'
                         else:
                             maxMemoryUsage = '%d MiB' % (stats.maxMemoryUsage / 1024 / 1024)
                         time = "%d ms" % stats.time
+                        is_running = "%d" % stats.isRunning
                     except NVMLError as err:
                         if (err.value == NVML_ERROR_NOT_FOUND):
                             # probably went away
                             continue
                         err = handleError(err)
                         gpuUtilization = err
                         memoryUtilization = err
                         maxMemoryUsage = err
                         time = err
+                        is_running = err
                     
                     strResult += '    <accounted_process_info>\n'
                     strResult += '      <pid>%d</pid>\n' % pid
                     strResult += '      <gpu_util>' + gpuUtilization + '</gpu_util>\n'
                     strResult += '      <memory_util>' + memoryUtilization + '</memory_util>\n'
                     strResult += '      <max_memory_usage>' + maxMemoryUsage+ '</max_memory_usage>\n'
                     strResult += '      <time>' + time + '</time>\n'
+                    strResult += '      <is_running>' + is_running + '</is_running>\n'
                     strResult += '    </accounted_process_info>\n'
                 
                 strResult += '    </accounted_processes>\n'
             except NVMLError as err:
                 strResult += '    <accounted_processes>' + handleError(err) + '</accounted_processes>\n'
 
             strResult += '  </gpu>\n'
```

### Comparing `nvidia-ml-py-7.346.0/README.txt` & `nvidia-ml-py-7.352.0/README.txt`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 USAGE
 -----
 
     >>> from pynvml import *
     >>> nvmlInit()
     >>> print "Driver Version:", nvmlSystemGetDriverVersion()
-    Driver Version: 346.00
+    Driver Version: 352.00
     >>> deviceCount = nvmlDeviceGetCount()
     >>> for i in range(deviceCount):
     ...     handle = nvmlDeviceGetHandleByIndex(i)
     ...     print "Device", i, ":", nvmlDeviceGetName(handle)
     ... 
     Device 0 : Tesla K40c
     
@@ -127,14 +127,16 @@
 - Fixing nvmlUnitGetDeviceCount bug
 Version 5.319.0
 - Added new functions for NVML 5.319.  See NVML documentation for more information.
 Version 6.340.0
 - Added new functions for NVML 6.340.  See NVML documentation for more information.
 Version 7.346.0
 - Added new functions for NVML 7.346.  See NVML documentation for more information.
+Version 7.352.0
+- Added new functions for NVML 7.352.  See NVML documentation for more information.
 
 COPYRIGHT
 ---------
 Copyright (c) 2011-2015, NVIDIA Corporation.  All rights reserved.
 
 LICENSE
 -------
```

### Comparing `nvidia-ml-py-7.346.0/pynvml.py` & `nvidia-ml-py-7.352.0/pynvml.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,15 @@
 NVML_ERROR_IRQ_ISSUE           = 11
 NVML_ERROR_LIBRARY_NOT_FOUND   = 12
 NVML_ERROR_FUNCTION_NOT_FOUND  = 13
 NVML_ERROR_CORRUPTED_INFOROM   = 14
 NVML_ERROR_GPU_IS_LOST         = 15
 NVML_ERROR_RESET_REQUIRED      = 16
 NVML_ERROR_OPERATING_SYSTEM    = 17
+NVML_ERROR_LIB_RM_VERSION_MISMATCH = 18
 NVML_ERROR_UNKNOWN             = 999
 
 _nvmlFanState_t = c_uint
 NVML_FAN_NORMAL             = 0
 NVML_FAN_FAILED             = 1
 
 _nvmlLedColor_t = c_uint
@@ -198,14 +199,22 @@
 NVML_SAMPLINGTYPE_COUNT = 7
 
 _nvmlPcieUtilCounter_t = c_uint
 NVML_PCIE_UTIL_TX_BYTES = 0
 NVML_PCIE_UTIL_RX_BYTES = 1
 NVML_PCIE_UTIL_COUNT = 2
 
+_nvmlGpuTopologyLevel_t = c_uint
+NVML_TOPOLOGY_INTERNAL = 0
+NVML_TOPOLOGY_SINGLE = 10
+NVML_TOPOLOGY_MULTIPLE = 20
+NVML_TOPOLOGY_HOSTBRIDGE = 30
+NVML_TOPOLOGY_CPU = 40
+NVML_TOPOLOGY_SYSTEM = 50
+
 # C preprocessor defined values
 nvmlFlagDefault             = 0
 nvmlFlagForce               = 1
 
 # buffer size
 NVML_DEVICE_INFOROM_VERSION_BUFFER_SIZE      = 16
 NVML_DEVICE_UUID_BUFFER_SIZE                 = 80
@@ -241,14 +250,16 @@
         NVML_ERROR_TIMEOUT:             "Timeout",
         NVML_ERROR_IRQ_ISSUE:           "Interrupt Request Issue",
         NVML_ERROR_LIBRARY_NOT_FOUND:   "NVML Shared Library Not Found",
         NVML_ERROR_FUNCTION_NOT_FOUND:  "Function Not Found",
         NVML_ERROR_CORRUPTED_INFOROM:   "Corrupted infoROM",
         NVML_ERROR_GPU_IS_LOST:         "GPU is lost",
         NVML_ERROR_RESET_REQUIRED:      "GPU requires restart",
+        NVML_ERROR_OPERATING_SYSTEM:    "The operating system has blocked the request.",
+        NVML_ERROR_LIB_RM_VERSION_MISMATCH: "RM has detected an NVML/RM version mismatch.",
         NVML_ERROR_UNKNOWN:             "Unknown Error",
         }
     def __new__(typ, value):
         '''
         Maps value to a proper subclass of NVMLError.
         See _extractNVMLErrorsAsClasses function for more details
         '''
@@ -583,15 +594,17 @@
 
 class c_nvmlAccountingStats_t(_PrintableStructure):
     _fields_ = [
         ('gpuUtilization', c_uint),
         ('memoryUtilization', c_uint),
         ('maxMemoryUsage', c_ulonglong),
         ('time', c_ulonglong),
-        ('reserved', c_uint * 8)
+        ('startTime', c_ulonglong),
+        ('isRunning', c_uint),
+        ('reserved', c_uint * 5)
     ]
 
 ## C function wrappers ##
 def nvmlInit():
     _LoadNvmlLibrary()
     
     #
@@ -1641,7 +1654,48 @@
     
 def nvmlDeviceGetPcieThroughput(device, counter):
     c_util = c_uint()
     fn = _nvmlGetFunctionPointer("nvmlDeviceGetPcieThroughput")
     ret = fn(device, _nvmlPcieUtilCounter_t(counter), byref(c_util))
     _nvmlCheckReturn(ret)
     return c_util.value
+
+def nvmlSystemGetTopologyGpuSet(cpuNumber):
+    c_count = c_uint(0)
+    fn = _nvmlGetFunctionPointer("nvmlSystemGetTopologyGpuSet")
+
+    # First call will get the size
+    ret = fn(cpuNumber, byref(c_count), None)
+
+    if ret != NVML_SUCCESS:
+        raise NVMLError(ret)
+    print c_count.value
+    # call again with a buffer
+    device_array = c_nvmlDevice_t * c_count.value
+    c_devices = device_array()
+    ret = fn(cpuNumber, byref(c_count), c_devices)
+    _nvmlCheckReturn(ret)
+    return map(None, c_devices[0:c_count.value])
+
+def nvmlDeviceGetTopologyNearestGpus(device, level):
+    c_count = c_uint(0)
+    fn = _nvmlGetFunctionPointer("nvmlDeviceGetTopologyNearestGpus")
+
+    # First call will get the size
+    ret = fn(device, level, byref(c_count), None)
+
+    if ret != NVML_SUCCESS:
+        raise NVMLError(ret)
+
+    # call again with a buffer
+    device_array = c_nvmlDevice_t * c_count.value
+    c_devices = device_array()
+    ret = fn(device, level, byref(c_count), c_devices)
+    _nvmlCheckReturn(ret)
+    return map(None, c_devices[0:c_count.value])
+
+def nvmlDeviceGetTopologyCommonAncestor(device1, device2):
+    c_level = _nvmlGpuTopologyLevel_t()
+    fn = _nvmlGetFunctionPointer("nvmlDeviceGetTopologyCommonAncestor")
+    ret = fn(device1, device2, byref(c_level))
+    _nvmlCheckReturn(ret)
+    return c_level.value
```


# Comparing `tmp/mlscat-0.0.6.tar.gz` & `tmp/mlscat-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlscat-0.0.6.tar", last modified: Wed Apr 17 07:15:35 2024, max compression
+gzip compressed data, was "mlscat-0.0.7.tar", last modified: Thu Apr 25 07:52:53 2024, max compression
```

## Comparing `mlscat-0.0.6.tar` & `mlscat-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 M0nk3y    (1021) M0nk3y    (1021)        0 2024-04-17 07:15:35.942598 mlscat-0.0.6/
--rw-r--r--   0 M0nk3y    (1021) M0nk3y    (1021)      776 2024-04-17 07:15:35.942598 mlscat-0.0.6/PKG-INFO
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      523 2024-04-17 06:13:37.000000 mlscat-0.0.6/README.md
-drwxrwxr-x   0 M0nk3y    (1021) M0nk3y    (1021)        0 2024-04-17 07:15:35.942598 mlscat-0.0.6/mlscat/
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      131 2024-04-17 07:15:25.000000 mlscat-0.0.6/mlscat/__init__.py
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      172 2024-04-17 06:13:37.000000 mlscat-0.0.6/mlscat/api.py
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)     2111 2024-04-17 06:24:18.000000 mlscat-0.0.6/mlscat/attacks.py
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)     1420 2024-04-17 06:13:37.000000 mlscat-0.0.6/mlscat/ranks.py
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)    25641 2024-04-17 07:03:35.000000 mlscat-0.0.6/mlscat/utils.py
-drwxrwxr-x   0 M0nk3y    (1021) M0nk3y    (1021)        0 2024-04-17 07:15:35.942598 mlscat-0.0.6/mlscat.egg-info/
--rw-r--r--   0 M0nk3y    (1021) M0nk3y    (1021)      776 2024-04-17 07:15:35.000000 mlscat-0.0.6/mlscat.egg-info/PKG-INFO
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      250 2024-04-17 07:15:35.000000 mlscat-0.0.6/mlscat.egg-info/SOURCES.txt
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)        1 2024-04-17 07:15:35.000000 mlscat-0.0.6/mlscat.egg-info/dependency_links.txt
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)        6 2024-04-17 07:15:35.000000 mlscat-0.0.6/mlscat.egg-info/requires.txt
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)        7 2024-04-17 07:15:35.000000 mlscat-0.0.6/mlscat.egg-info/top_level.txt
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)       38 2024-04-17 07:15:35.942598 mlscat-0.0.6/setup.cfg
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      590 2024-04-17 07:12:12.000000 mlscat-0.0.6/setup.py
+drwxrwxr-x   0 M0nk3y    (1021) M0nk3y    (1021)        0 2024-04-25 07:52:53.235413 mlscat-0.0.7/
+-rw-r--r--   0 M0nk3y    (1021) M0nk3y    (1021)      776 2024-04-25 07:52:53.235413 mlscat-0.0.7/PKG-INFO
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      523 2024-04-17 06:13:37.000000 mlscat-0.0.7/README.md
+drwxrwxr-x   0 M0nk3y    (1021) M0nk3y    (1021)        0 2024-04-25 07:52:53.235413 mlscat-0.0.7/mlscat/
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      131 2024-04-25 07:52:31.000000 mlscat-0.0.7/mlscat/__init__.py
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      172 2024-04-17 06:13:37.000000 mlscat-0.0.7/mlscat/api.py
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)     2111 2024-04-17 06:24:18.000000 mlscat-0.0.7/mlscat/attacks.py
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)     1441 2024-04-19 02:06:03.000000 mlscat-0.0.7/mlscat/ranks.py
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)     1993 2024-04-25 07:24:37.000000 mlscat-0.0.7/mlscat/security.py
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)    25666 2024-04-19 02:11:10.000000 mlscat-0.0.7/mlscat/utils.py
+drwxrwxr-x   0 M0nk3y    (1021) M0nk3y    (1021)        0 2024-04-25 07:52:53.235413 mlscat-0.0.7/mlscat.egg-info/
+-rw-r--r--   0 M0nk3y    (1021) M0nk3y    (1021)      776 2024-04-25 07:52:53.000000 mlscat-0.0.7/mlscat.egg-info/PKG-INFO
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      269 2024-04-25 07:52:53.000000 mlscat-0.0.7/mlscat.egg-info/SOURCES.txt
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)        1 2024-04-25 07:52:53.000000 mlscat-0.0.7/mlscat.egg-info/dependency_links.txt
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)        6 2024-04-25 07:52:53.000000 mlscat-0.0.7/mlscat.egg-info/requires.txt
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)        7 2024-04-25 07:52:53.000000 mlscat-0.0.7/mlscat.egg-info/top_level.txt
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)       38 2024-04-25 07:52:53.235413 mlscat-0.0.7/setup.cfg
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      590 2024-04-17 12:37:41.000000 mlscat-0.0.7/setup.py
```

### Comparing `mlscat-0.0.6/PKG-INFO` & `mlscat-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlscat
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small cat help you enjoy your side channel attack journal!
 Author: i4mhmh
 Author-email: i4mhmh@outlook.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
```

### Comparing `mlscat-0.0.6/README.md` & `mlscat-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `mlscat-0.0.6/mlscat/attacks.py` & `mlscat-0.0.7/mlscat/attacks.py`

 * *Files identical despite different names*

### Comparing `mlscat-0.0.6/mlscat/ranks.py` & `mlscat-0.0.7/mlscat/ranks.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,22 @@
     return mean rank
 '''
 def rank(predictions, targets, key:int, times:int, num_trace:int, interval:int, verbose=1):
     # 只写这一次 别的方法直接返回报错就行
     assert type(times) == type(num_trace) == type(interval) == type(verbose) == type(key) == int
     
     predictions = np.log(predictions + 1e-40)
-    rank_array = np.zeros(shape=(times, num_trace/interval))
+    rank_array = np.zeros(shape=(times, int(num_trace/interval)))
     for i in range(times):
-        tmp_rank = np.zeros(num_trace/interval)
+        tmp_rank = np.zeros(int(num_trace/interval))
         pred = np.zeros(256)
-        idx = np.random.randint(predictions[0], size=num_trace)
+        idx = np.random.randint(predictions.shape[0], size=num_trace)
         for random_index, trace_index in enumerate(idx):
             for key_value in range(256):
                 # ergodic every keys prob
                 pred[key_value] += predictions[trace_index, targets[trace_index, key_value]]
             
             if random_index % interval == 0:
                 ranked = np.argsort(pred)[::-1]
-                tmp_rank[i/interval] = list(ranked).index(key)
+                tmp_rank[int(i/interval)] = list(ranked).index(key)
         rank_array[i] = tmp_rank
     return np.mean(rank_array, axis=0)
```

### Comparing `mlscat-0.0.6/mlscat/utils.py` & `mlscat-0.0.7/mlscat/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,24 +43,24 @@
 
     ## Parameters
     `data`: ndarray which saved the traces
 
     ## return 
     array which fit cnn inputs
     '''
-    return np.expand_dims(data, 1)
+    return np.expand_dims(data, data.ndim)
 
 def get_targets(plaintexts):
     targets = np.zeros(shape=(plaintexts.shape[0], 256))
     for num, plaintext in enumerate(plaintexts):
         tmp_targets = np.zeros(shape=256)
         for key in range(256):
             tmp_targets[key] = AES_Sbox[key ^ plaintext]
         targets[num] = tmp_targets
-    return targets
+    return targets.astype(np.int64)
 
 
 # Code is ported from https://github.com/fastai/fastai
 class OneCycleLR(Callback):
     def __init__(self,
                  num_samples,
                  batch_size,
```

### Comparing `mlscat-0.0.6/mlscat.egg-info/PKG-INFO` & `mlscat-0.0.7/mlscat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlscat
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small cat help you enjoy your side channel attack journal!
 Author: i4mhmh
 Author-email: i4mhmh@outlook.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
```

### Comparing `mlscat-0.0.6/setup.py` & `mlscat-0.0.7/setup.py`

 * *Files identical despite different names*


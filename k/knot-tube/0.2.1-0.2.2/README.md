# Comparing `tmp/knot_tube-0.2.1.tar.gz` & `tmp/knot_tube-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knot_tube-0.2.1.tar", last modified: Fri Apr 19 13:03:29 2024, max compression
+gzip compressed data, was "knot_tube-0.2.2.tar", last modified: Thu Apr 25 07:04:31 2024, max compression
```

## Comparing `knot_tube-0.2.1.tar` & `knot_tube-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 yongjian  (1002) yongjian  (1002)        0 2024-04-19 13:03:29.928691 knot_tube-0.2.1/
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)      143 2024-04-19 13:03:29.928691 knot_tube-0.2.1/PKG-INFO
-drwxrwxr-x   0 yongjian  (1002) yongjian  (1002)        0 2024-04-19 13:03:29.928691 knot_tube-0.2.1/knot_tube/
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)        0 2023-04-14 13:52:36.000000 knot_tube-0.2.1/knot_tube/__init__.py
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)     7521 2023-09-18 06:57:25.000000 knot_tube-0.2.1/knot_tube/knot.py
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)     1593 2024-01-16 14:30:38.000000 knot_tube-0.2.1/knot_tube/lammps.py
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)        0 2024-01-28 13:31:15.000000 knot_tube-0.2.1/knot_tube/pdb.py
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)     1751 2024-04-16 12:03:58.000000 knot_tube-0.2.1/knot_tube/polymer.py
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)     5809 2024-03-11 05:22:15.000000 knot_tube-0.2.1/knot_tube/xyz.py
-drwxrwxr-x   0 yongjian  (1002) yongjian  (1002)        0 2024-04-19 13:03:29.928691 knot_tube-0.2.1/knot_tube.egg-info/
--rw-r--r--   0 yongjian  (1002) yongjian  (1002)      143 2024-04-19 13:03:29.000000 knot_tube-0.2.1/knot_tube.egg-info/PKG-INFO
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)      287 2024-04-19 13:03:29.000000 knot_tube-0.2.1/knot_tube.egg-info/SOURCES.txt
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)        1 2024-04-19 13:03:29.000000 knot_tube-0.2.1/knot_tube.egg-info/dependency_links.txt
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)       12 2024-04-19 13:03:29.000000 knot_tube-0.2.1/knot_tube.egg-info/requires.txt
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)       10 2024-04-19 13:03:29.000000 knot_tube-0.2.1/knot_tube.egg-info/top_level.txt
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)       38 2024-04-19 13:03:29.928691 knot_tube-0.2.1/setup.cfg
--rw-rw-r--   0 yongjian  (1002) yongjian  (1002)      338 2024-04-19 13:03:26.000000 knot_tube-0.2.1/setup.py
+drwxrwxr-x   0 yongjian  (1002) yongjian  (1002)        0 2024-04-25 07:04:31.370511 knot_tube-0.2.2/
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)      143 2024-04-25 07:04:31.370511 knot_tube-0.2.2/PKG-INFO
+drwxrwxr-x   0 yongjian  (1002) yongjian  (1002)        0 2024-04-25 07:04:31.370511 knot_tube-0.2.2/knot_tube/
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)        0 2023-04-14 13:52:36.000000 knot_tube-0.2.2/knot_tube/__init__.py
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)     7521 2023-09-18 06:57:25.000000 knot_tube-0.2.2/knot_tube/knot.py
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)     1593 2024-01-16 14:30:38.000000 knot_tube-0.2.2/knot_tube/lammps.py
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)        0 2024-01-28 13:31:15.000000 knot_tube-0.2.2/knot_tube/pdb.py
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)     2084 2024-04-19 13:36:39.000000 knot_tube-0.2.2/knot_tube/polymer.py
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)     6734 2024-04-25 07:03:01.000000 knot_tube-0.2.2/knot_tube/xyz.py
+drwxrwxr-x   0 yongjian  (1002) yongjian  (1002)        0 2024-04-25 07:04:31.370511 knot_tube-0.2.2/knot_tube.egg-info/
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)      143 2024-04-25 07:04:31.000000 knot_tube-0.2.2/knot_tube.egg-info/PKG-INFO
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)      287 2024-04-25 07:04:31.000000 knot_tube-0.2.2/knot_tube.egg-info/SOURCES.txt
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)        1 2024-04-25 07:04:31.000000 knot_tube-0.2.2/knot_tube.egg-info/dependency_links.txt
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)       12 2024-04-25 07:04:31.000000 knot_tube-0.2.2/knot_tube.egg-info/requires.txt
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)       10 2024-04-25 07:04:31.000000 knot_tube-0.2.2/knot_tube.egg-info/top_level.txt
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)       38 2024-04-25 07:04:31.370511 knot_tube-0.2.2/setup.cfg
+-rw-rw-r--   0 yongjian  (1002) yongjian  (1002)      338 2024-04-25 07:04:25.000000 knot_tube-0.2.2/setup.py
```

### Comparing `knot_tube-0.2.1/knot_tube/knot.py` & `knot_tube-0.2.2/knot_tube/knot.py`

 * *Files identical despite different names*

### Comparing `knot_tube-0.2.1/knot_tube/lammps.py` & `knot_tube-0.2.2/knot_tube/lammps.py`

 * *Files identical despite different names*

### Comparing `knot_tube-0.2.1/knot_tube/polymer.py` & `knot_tube-0.2.2/knot_tube/polymer.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,8 +31,16 @@
     
     # 计算每个原子到质心的距离的平方
     distances_squared = np.sum(displacement**2, axis=2)
     
     # 计算每帧的回转半径
     gyration_radius = np.sqrt(np.mean(distances_squared, axis=1))
     
-    return gyration_radius
+    return gyration_radius
+
+def end_to_end_distance(trajectory:np.ndarray):
+    """计算轨迹的端到端距离分布,输入应该为N_frames, N_atoms, 3的numpy array."""
+    # 计算每帧的端到端距离
+    end_to_end = trajectory[:,-1] - trajectory[:,0]
+    end_to_end_distance = np.linalg.norm(end_to_end, axis=1)
+    
+    return end_to_end_distance
```

### Comparing `knot_tube-0.2.1/knot_tube/xyz.py` & `knot_tube-0.2.2/knot_tube/xyz.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,14 +60,32 @@
 #         atoms = []
 #         for line in lines:
 #             line = line.split()
 #             atom = [ float(line[1]), float(line[2]), float(line[3])]
 #             atoms.append(atom)
 #     return np.array(atoms)
 
+def save_xyz(file, X:np.ndarray, append = False, intervel =1):
+    """Save trajectory to xyz file. X should be N_frames, N_atoms, 3 numpy array. append = True means append to the file, intervel means the intervel between two frames"""
+    N_frames, N_atoms, _ = X.shape
+    if(append):
+        with open(file, 'a') as f:
+            for i in range(0, N_frames, intervel):
+                f.write(str(N_atoms) + '\n')
+                f.write('frame: {}\n'.format(i))
+                for j in range(N_atoms):
+                    f.write('1\t{:f} {:f} {:f}'.format(X[i,j,0], X[i,j,1], X[i,j,2]) + '\n')
+    else:
+        with open(file, 'w') as f:
+            for i in range(0, N_frames, intervel):
+                f.write(str(N_atoms) + '\n')
+                f.write('frame: {}\n'.format(i))
+                for j in range(N_atoms):
+                    f.write('1\t{:f} {:f} {:f}'.format(X[i,j,0], X[i,j,1], X[i,j,2]) + '\n')
+
 def save_xyz_single(file, X:np.ndarray, title:str, dir=None, append=False):
     # 如果dir不存在则创建
     if dir and not os.path.exists(dir):
         os.makedirs(dir)
     
     if(append):
         with open(dir+'/'+file, 'a') as f:
```


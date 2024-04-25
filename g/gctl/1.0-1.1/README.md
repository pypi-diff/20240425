# Comparing `tmp/gctl-1.0.tar.gz` & `tmp/gctl-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gctl-1.0.tar", last modified: Thu Apr 25 03:19:27 2024, max compression
+gzip compressed data, was "gctl-1.1.tar", last modified: Thu Apr 25 10:24:50 2024, max compression
```

## Comparing `gctl-1.0.tar` & `gctl-1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 han       (1000) han       (1000)        0 2024-04-25 03:19:27.834082 gctl-1.0/
--rw-rw-r--   0 han       (1000) han       (1000)     1060 2024-04-25 02:17:59.000000 gctl-1.0/LICENSE
--rw-r--r--   0 han       (1000) han       (1000)     1254 2024-04-25 03:19:27.834082 gctl-1.0/PKG-INFO
--rw-rw-r--   0 han       (1000) han       (1000)      761 2024-04-25 02:17:59.000000 gctl-1.0/README.md
-drwxrwxr-x   0 han       (1000) han       (1000)        0 2024-04-25 03:19:27.834082 gctl-1.0/gctl/
-drwxrwxr-x   0 han       (1000) han       (1000)        0 2024-04-25 03:19:27.834082 gctl-1.0/gctl/curve/
--rw-rw-r--   0 han       (1000) han       (1000)     9216 2024-04-25 02:25:07.000000 gctl-1.0/gctl/curve/dubins_path.py
--rw-rw-r--   0 han       (1000) han       (1000)    14999 2024-04-25 02:17:59.000000 gctl-1.0/gctl/curve/reeds_shepp.py
--rw-rw-r--   0 han       (1000) han       (1000)     8360 2024-04-25 02:30:55.000000 gctl-1.0/gctl/curve_generator.py
-drwxrwxr-x   0 han       (1000) han       (1000)        0 2024-04-25 03:19:27.834082 gctl-1.0/gctl.egg-info/
--rw-r--r--   0 han       (1000) han       (1000)     1254 2024-04-25 03:19:27.000000 gctl-1.0/gctl.egg-info/PKG-INFO
--rw-rw-r--   0 han       (1000) han       (1000)      247 2024-04-25 03:19:27.000000 gctl-1.0/gctl.egg-info/SOURCES.txt
--rw-rw-r--   0 han       (1000) han       (1000)        1 2024-04-25 03:19:27.000000 gctl-1.0/gctl.egg-info/dependency_links.txt
--rw-rw-r--   0 han       (1000) han       (1000)       23 2024-04-25 03:19:27.000000 gctl-1.0/gctl.egg-info/requires.txt
--rw-rw-r--   0 han       (1000) han       (1000)        5 2024-04-25 03:19:27.000000 gctl-1.0/gctl.egg-info/top_level.txt
--rw-rw-r--   0 han       (1000) han       (1000)      588 2024-04-25 03:12:06.000000 gctl-1.0/pyproject.toml
--rw-rw-r--   0 han       (1000) han       (1000)       38 2024-04-25 03:19:27.834082 gctl-1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-25 10:24:50.079060 gctl-1.1/
+-rw-rw-rw-   0        0        0     1081 2024-04-25 10:08:06.000000 gctl-1.1/LICENSE
+-rw-rw-rw-   0        0        0     1309 2024-04-25 10:24:50.078017 gctl-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      800 2024-04-25 10:08:06.000000 gctl-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 10:24:50.064923 gctl-1.1/gctl/
+-rw-rw-rw-   0        0        0       48 2024-04-25 10:08:06.000000 gctl-1.1/gctl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 10:24:50.077016 gctl-1.1/gctl/curve/
+-rw-rw-rw-   0        0        0     9553 2024-04-25 10:08:06.000000 gctl-1.1/gctl/curve/dubins_path.py
+-rw-rw-rw-   0        0        0    15537 2024-04-25 10:08:06.000000 gctl-1.1/gctl/curve/reeds_shepp.py
+-rw-rw-rw-   0        0        0     8589 2024-04-25 10:08:06.000000 gctl-1.1/gctl/curve_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-25 10:24:50.078017 gctl-1.1/gctl.egg-info/
+-rw-rw-rw-   0        0        0     1309 2024-04-25 10:24:50.000000 gctl-1.1/gctl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2024-04-25 10:24:50.000000 gctl-1.1/gctl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 10:24:50.000000 gctl-1.1/gctl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-04-25 10:24:50.000000 gctl-1.1/gctl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-25 10:24:50.000000 gctl-1.1/gctl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      614 2024-04-25 10:08:06.000000 gctl-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-25 10:24:50.079060 gctl-1.1/setup.cfg
```

### Comparing `gctl-1.0/LICENSE` & `gctl-1.1/LICENSE`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Han
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Han
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `gctl-1.0/PKG-INFO` & `gctl-1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-Metadata-Version: 2.1
-Name: gctl
-Version: 1.0
-Summary: Generate curve tool
-Author-email: Han Ruihua <hanrh@connect.hku.hk>
-Project-URL: Homepage, https://github.com/hanruihua/GenerateCurveTool
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: scipy
-
-# GenerateCurveTool
-
-A tool of generating the common curves from way points for the robot path planning, including dubins path, reeds shepp, etc.
-
-
-Dubins path  |   Reeds Shepp    |
-:-------------------------:|:-------------------------:|
-![](example/gif/dubins.gif)  | ![](example/gif/reeds_shepp.gif) 
-
-## Prerequisite
-
-- Python: >= 3.8
-    - numpy  
-    - matplotlib 
-
-## Installation
-
-```
-git clone https://github.com/hanruihua/GenerateCurveTool  
-cd GenerateCurveTool  
-pip install -e . 
-```
-
-## Usage 
-
-The examples are in [GenerateCurveTool/example/](https://github.com/hanruihua/GenerateCurveTool/tree/main/example)
-
-## Roadmap
-
-- [x] Direct line
-- [x] Dubins path
-- [x] Reeds shepp
-- [ ] bezier 
-
-## Author
-
-Han Ruihua  
-Contact: hanrh@connect.hku.hk
-
+Metadata-Version: 2.1
+Name: gctl
+Version: 1.1
+Summary: Generate curve tool
+Author-email: Han Ruihua <hanrh@connect.hku.hk>
+Project-URL: Homepage, https://github.com/hanruihua/GenerateCurveTool
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scipy
+
+# GenerateCurveTool
+
+A tool of generating the common curves from way points for the robot path planning, including dubins path, reeds shepp, etc.
+
+
+Dubins path  |   Reeds Shepp    |
+:-------------------------:|:-------------------------:|
+![](example/gif/dubins.gif)  | ![](example/gif/reeds_shepp.gif) 
+
+## Prerequisite
+
+- Python: >= 3.8
+    - numpy  
+    - matplotlib 
+
+## Installation
+
+```
+git clone https://github.com/hanruihua/GenerateCurveTool  
+cd GenerateCurveTool  
+pip install -e . 
+```
+
+## Usage 
+
+The examples are in [GenerateCurveTool/example/](https://github.com/hanruihua/GenerateCurveTool/tree/main/example)
+
+## Roadmap
+
+- [x] Direct line
+- [x] Dubins path
+- [x] Reeds shepp
+- [ ] bezier 
+
+## Author
+
+Han Ruihua  
+Contact: hanrh@connect.hku.hk
+
```

### Comparing `gctl-1.0/README.md` & `gctl-1.1/README.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-# GenerateCurveTool
-
-A tool of generating the common curves from way points for the robot path planning, including dubins path, reeds shepp, etc.
-
-
-Dubins path  |   Reeds Shepp    |
-:-------------------------:|:-------------------------:|
-![](example/gif/dubins.gif)  | ![](example/gif/reeds_shepp.gif) 
-
-## Prerequisite
-
-- Python: >= 3.8
-    - numpy  
-    - matplotlib 
-
-## Installation
-
-```
-git clone https://github.com/hanruihua/GenerateCurveTool  
-cd GenerateCurveTool  
-pip install -e . 
-```
-
-## Usage 
-
-The examples are in [GenerateCurveTool/example/](https://github.com/hanruihua/GenerateCurveTool/tree/main/example)
-
-## Roadmap
-
-- [x] Direct line
-- [x] Dubins path
-- [x] Reeds shepp
-- [ ] bezier 
-
-## Author
-
-Han Ruihua  
-Contact: hanrh@connect.hku.hk
-
+# GenerateCurveTool
+
+A tool of generating the common curves from way points for the robot path planning, including dubins path, reeds shepp, etc.
+
+
+Dubins path  |   Reeds Shepp    |
+:-------------------------:|:-------------------------:|
+![](example/gif/dubins.gif)  | ![](example/gif/reeds_shepp.gif) 
+
+## Prerequisite
+
+- Python: >= 3.8
+    - numpy  
+    - matplotlib 
+
+## Installation
+
+```
+git clone https://github.com/hanruihua/GenerateCurveTool  
+cd GenerateCurveTool  
+pip install -e . 
+```
+
+## Usage 
+
+The examples are in [GenerateCurveTool/example/](https://github.com/hanruihua/GenerateCurveTool/tree/main/example)
+
+## Roadmap
+
+- [x] Direct line
+- [x] Dubins path
+- [x] Reeds shepp
+- [ ] bezier 
+
+## Author
+
+Han Ruihua  
+Contact: hanrh@connect.hku.hk
+
```

### Comparing `gctl-1.0/gctl/curve/dubins_path.py` & `gctl-1.1/gctl/curve/dubins_path.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,337 +1,337 @@
-"""
-code author: Han Ruihua
-reference: paper 'Classification of the Dubins set, 2001', github https://github.com/AndrewWalker/Dubins-Curves/blob/master/src/dubins.c
-"""
-
-import numpy as np
-from math import pi, sin, cos, atan2, sqrt, acos, inf
-
-steer_dict = {'L': 1, 'R': -1, 'S': 0 }  # turn left right, straight 
-
-def generate_dubins_path(start=np.zeros((3, 1)), end=np.ones((3, 1)), min_radius=1, step_size=0.1, **kwargs):
-
-    """
-    Arguments:
-        start: the start point of the curve: 3* 1 matrix
-        end: the end point of the curve: 3 * 1 matrix
-        min_radius: The minimum turning radius of the car
-        step_size: the distance between each point
-    """
-    alpha, beta, d = preprocess(start, end, min_radius)
-    admissible_path = [dubins_LSL, dubins_RSR, dubins_RSL, dubins_LSR, dubins_RLR, dubins_LRL] # the candidate curves
-
-    min_length = inf
-        
-    for ap in admissible_path:
-        # find the shortest path
-        t, p, q, mode = ap(alpha, beta, d)
-
-        if t == None:
-            continue
-
-        total_length = abs(t) + abs(p) + abs(q)
-        if total_length < min_length:
-            min_length = total_length
-            sh_t = t
-            sh_p = p
-            sh_q = q
-            sh_mode = mode
-    
-    path_point_list = path_generate(start, sh_t, sh_p, sh_q, sh_mode, min_radius, step_size)  # generate the path points
-
-    return path_point_list
-
-def preprocess(start, end, min_radius):
-    # calculate the relative unit angle and distance
-
-    assert start.shape == (3, 1) and end.shape == (3, 1)
-
-    dis, radian = relative(start, end)
-
-    d = dis / min_radius
-
-    start_theta = start[2, 0]
-    goal_theta = end[2, 0]
-
-    alpha = (start_theta - radian) % (2*pi)
-    beta = (goal_theta - radian) % (2*pi)
-
-    return alpha, beta, d
-
-def path_generate(start, t, p, q, mode, min_radius, step_size):
-    # generate a series points from the (t, p, q) set by the mode
-
-    length = [t, p, q]
-
-    trajectory = [start]
-    init_point = start
-
-    for i in range(3):
-        if length[i] != 0:
-            point_list, end_point = element_sample(length[i], init_point, mode[i], min_radius, step_size)
-            trajectory = trajectory + point_list
-            init_point = end_point
-
-    return trajectory
-
-def element_sample(length, start_point, steer_mode, min_radius, step_size):
-    # generate a series points from the an element
-    
-    # if steer_mode == 'L': steer = 1
-        
-    # elif steer_mode == 'R': steer = -1
-        
-    # if steer_mode == 'S': steer = 0
-
-    steer = steer_dict[steer_mode]
-    real_length = length * min_radius
-
-    # calculate the end point first
-    # end_pose = trans_pose(start_point, real_length, steer, min_radius)
-
-    # generate a series of sample points 
-    cur_length = 0
-    path_list = []
-
-    while cur_length <= real_length - step_size:
-        cur_length = cur_length + step_size
-        next_pose = trans_pose(start_point, cur_length, steer, min_radius)
-        path_list.append(next_pose)
-
-    end_pose = trans_pose(start_point, real_length, steer, min_radius)
-
-    # add the end pose under current transform
-    temp = len(path_list)
-
-    if len(path_list) != 0:
-        if np.linalg.norm(end_pose - path_list[-1]) <= 0.01:
-            path_list[-1] = end_pose
-        else:
-            path_list.append(end_pose)
-    else:
-        path_list.append(end_pose)
-
-    return path_list, end_pose
-        
-def trans_pose(start_pose, length, steer, min_radius):
-    # pose: x, y, theta, 3*1
-    # rotate the start pose with a rot_theta by a center point
-
-    cur_theta = start_pose[2, 0]
-    start_position = start_pose[0:2]
-    rot_theta = steer * length / min_radius
-
-    if rot_theta == 0:
-        trans_matrix = length * np.array([ [cos(cur_theta)], [sin(cur_theta)], [0]])
-        end_pose = start_pose + trans_matrix
-    else:
-        center_theta = cur_theta + steer*pi/2
-        center_position = start_position + min_radius * np.array([ [cos(center_theta)], [sin(center_theta)]])
-
-        rot_matrix = np.array([[cos(rot_theta), -sin(rot_theta)], [sin(rot_theta), cos(rot_theta)]])
-        end_position = center_position + rot_matrix @ (start_position - center_position)
-        end_theta = wraptopi(cur_theta + rot_theta)
-        end_pose = np.vstack((end_position, [end_theta]))
-
-    return end_pose
-
-
-
-# def element_sample(length, start_point, steer_mode, min_radius, step_size):
-#     # generate a series points from the an element
-
-#     cur_x = start_point[0, 0]
-#     cur_y = start_point[1, 0]
-#     cur_theta = start_point[2, 0]
-
-#     path_list = []
-
-#     endpoint = np.zeros((3, 1))
-
-#     if steer_mode == 'L':
-#         steer = 1
-#     elif steer_mode == 'R':
-#         steer = -1
-#     if steer_mode == 'S':
-#         steer = 0
-
-#     curvature = steer * 1/ min_radius
-#     real_length = length * min_radius
-
-#     rot_theta = real_length * curvature
-
-#     # calculate end point
-#     if curvature == 0:
-#         endpoint = trans_point(start_point, cur_theta, real_length)
-#     else:
-#         center_theta = cur_theta + steer*pi/2
-#         center_x = cur_x + cos(center_theta) * min_radius
-#         center_y = cur_y + sin(center_theta) * min_radius
-
-#         center_point = np.array( [ [center_x], [center_y], [center_theta] ])
-
-#         end_cir_theta = cur_theta + rot_theta - steer*pi/2
-#         endpoint = trans_point(center_point, end_cir_theta, min_radius)
-
-#     cur_length = 0
-    
-#     # loop to generate the points
-#     while cur_length <= real_length - step_size:
-        
-#         next_theta = cur_theta + curvature * step_size
-#         cur_length = cur_length + step_size
-
-#         if curvature == 0:
-#             next_x = cur_x + cos(next_theta) * cur_length
-#             next_y = cur_y + sin(next_theta) * cur_length
-#         else:
-#             temp_theta = next_theta - steer*pi/2
-#             next_x = center_x + cos(temp_theta) * min_radius
-#             next_y = center_y + sin(temp_theta) * min_radius
-
-#         next_theta = wraptopi(next_theta)
-
-#         next_point = np.array([[next_x], [next_y], [next_theta]])
-
-#         path_list.append(next_point)
-
-#         cur_theta = next_theta
-
-#     path_list.append(endpoint)
-
-#     return path_list, endpoint
-
-# def trans_point(start_point, theta, length):
-
-#     trans_matrix = np.array([ [ cos(theta) * length ], [ sin(theta) * length ], [ theta ] ])
-#     end_point = start_point + trans_matrix
-#     end_point[2, 0] = wraptopi(end_point[2, 0])
-
-#     return end_point
-
-def dubins_LSL(alpha, beta, d):
-
-    mode = ['L', 'S', 'L']
-
-    temp0 = atan2(cos(beta)- cos(alpha), d+sin(alpha)-sin(beta))
-    t = (-alpha + temp0) % (2*pi)
-
-    temp1 = 2 + d**2 - 2*cos(alpha-beta) + 2 * d * (sin(alpha) - sin(beta))
-
-    if temp1 < 0:
-        return None, None, None, mode
-
-    p = sqrt(temp1)
-
-    q = (beta - temp0) % (2*pi)
-
-    return t, p, q, mode
-
-def dubins_RSR(alpha, beta, d):
-
-    mode = ['R', 'S', 'R']
-
-    temp0 = atan2(cos(alpha)- cos(beta), d-sin(alpha)+sin(beta))
-    t = (alpha - temp0) % (2*pi)
-
-    temp1 = 2 + d**2 - 2*cos(alpha-beta) + 2*d*(sin(beta)-sin(alpha))
-    if temp1 < 0:
-        return None, None, None, mode
-
-    p = sqrt(temp1)
-
-    q = (-beta % (2*pi) + temp0) % (2*pi)
-
-    return t, p, q, mode
-
-def dubins_LSR(alpha, beta, d):
-
-    mode=['L', 'S', 'R']
-
-    temp0 = -2 + d**2 + 2*cos(alpha-beta) + 2*d*(sin(alpha) + sin(beta) )
-    if temp0 < 0:
-        return None, None, None, mode
-
-    p = sqrt(temp0)
-
-    temp1 = atan2( (-cos(alpha)-cos(beta)), (d+sin(alpha)+sin(beta)) )
-    t = (-alpha+temp1 - atan2(-2, p)) % (2*pi)
-
-    q = (-beta % (2*pi)+temp1-atan2(-2, p)) % (2*pi)
-
-    return t, p, q, mode
-    
-def dubins_RSL(alpha, beta, d):
-    
-    mode = ['R', 'S', 'L']
-
-    temp0 = d**2-2+2*cos(alpha-beta)-2*d*(sin(alpha)+sin(beta))
-    if temp0 < 0:
-        return None, None, None, mode
-
-    p = sqrt(temp0)
-
-    temp1 = atan2( (cos(alpha)+cos(beta)), (d-sin(alpha)-sin(beta) ) )
-    t = (alpha - temp1 + atan2(2, p)) % (2*pi)
-
-    q = (beta % (2*pi) - temp1 + atan2(2, p)) % (2*pi)
-
-    return t, p, q, mode
-
-def dubins_RLR(alpha, beta, d):
-
-    mode = ['R', 'L', 'R']
-
-    temp0 = (6-d**2+2*cos(alpha-beta)+2*d*(sin(alpha) - sin(beta))) / 8
-    
-    if abs(temp0) > 1:
-        return None, None, None, mode
-
-    p = acos(temp0)
-    
-    temp1 = atan2( (cos(alpha) - cos(beta)), (d-sin(alpha)+sin(beta)) )
-
-    t = (alpha - temp1 + p/2) % (2*pi)
-
-    q = (alpha - beta - t + p) % (2*pi)
-
-    return t, p, q, mode
-
-# TYPO IN PAPER 
-def dubins_LRL(alpha, beta, d):
-    
-    mode=['L', 'R', 'L']
-
-    temp0 = (6-d**2+2*cos(alpha-beta)+2*d*(sin(beta) - sin(alpha))) / 8 
-    
-    if abs(temp0) > 1:
-        return None, None, None, mode
-
-    p = acos(temp0)
-
-    temp1 = atan2( (cos(beta)) - cos(alpha), (d+sin(alpha)-sin(beta)) )
-    t = (- alpha + temp1 + p/2) % (2*pi)
-
-    q = ( beta % (2*pi) - alpha - t  + p) % (2*pi)
-
-    return t, p, q, mode
-
-
-def relative(state1, state2):
-        
-    diff = state2[0:2] - state1[0:2]
-
-    dis = np.linalg.norm(diff)
-    radian = atan2(diff[1, 0], diff[0, 0])
-    
-    return dis, radian
-
-def wraptopi(rad):
-
-    while rad > pi:
-        rad = rad - 2 * pi
-    
-    while rad < -pi:
-        rad = rad + 2 * pi
-
-    return rad
+"""
+code author: Han Ruihua
+reference: paper 'Classification of the Dubins set, 2001', github https://github.com/AndrewWalker/Dubins-Curves/blob/master/src/dubins.c
+"""
+
+import numpy as np
+from math import pi, sin, cos, atan2, sqrt, acos, inf
+
+steer_dict = {'L': 1, 'R': -1, 'S': 0 }  # turn left right, straight 
+
+def generate_dubins_path(start=np.zeros((3, 1)), end=np.ones((3, 1)), min_radius=1, step_size=0.1, **kwargs):
+
+    """
+    Arguments:
+        start: the start point of the curve: 3* 1 matrix
+        end: the end point of the curve: 3 * 1 matrix
+        min_radius: The minimum turning radius of the car
+        step_size: the distance between each point
+    """
+    alpha, beta, d = preprocess(start, end, min_radius)
+    admissible_path = [dubins_LSL, dubins_RSR, dubins_RSL, dubins_LSR, dubins_RLR, dubins_LRL] # the candidate curves
+
+    min_length = inf
+        
+    for ap in admissible_path:
+        # find the shortest path
+        t, p, q, mode = ap(alpha, beta, d)
+
+        if t == None:
+            continue
+
+        total_length = abs(t) + abs(p) + abs(q)
+        if total_length < min_length:
+            min_length = total_length
+            sh_t = t
+            sh_p = p
+            sh_q = q
+            sh_mode = mode
+    
+    path_point_list = path_generate(start, sh_t, sh_p, sh_q, sh_mode, min_radius, step_size)  # generate the path points
+
+    return path_point_list
+
+def preprocess(start, end, min_radius):
+    # calculate the relative unit angle and distance
+
+    assert start.shape == (3, 1) and end.shape == (3, 1)
+
+    dis, radian = relative(start, end)
+
+    d = dis / min_radius
+
+    start_theta = start[2, 0]
+    goal_theta = end[2, 0]
+
+    alpha = (start_theta - radian) % (2*pi)
+    beta = (goal_theta - radian) % (2*pi)
+
+    return alpha, beta, d
+
+def path_generate(start, t, p, q, mode, min_radius, step_size):
+    # generate a series points from the (t, p, q) set by the mode
+
+    length = [t, p, q]
+
+    trajectory = [start]
+    init_point = start
+
+    for i in range(3):
+        if length[i] != 0:
+            point_list, end_point = element_sample(length[i], init_point, mode[i], min_radius, step_size)
+            trajectory = trajectory + point_list
+            init_point = end_point
+
+    return trajectory
+
+def element_sample(length, start_point, steer_mode, min_radius, step_size):
+    # generate a series points from the an element
+    
+    # if steer_mode == 'L': steer = 1
+        
+    # elif steer_mode == 'R': steer = -1
+        
+    # if steer_mode == 'S': steer = 0
+
+    steer = steer_dict[steer_mode]
+    real_length = length * min_radius
+
+    # calculate the end point first
+    # end_pose = trans_pose(start_point, real_length, steer, min_radius)
+
+    # generate a series of sample points 
+    cur_length = 0
+    path_list = []
+
+    while cur_length <= real_length - step_size:
+        cur_length = cur_length + step_size
+        next_pose = trans_pose(start_point, cur_length, steer, min_radius)
+        path_list.append(next_pose)
+
+    end_pose = trans_pose(start_point, real_length, steer, min_radius)
+
+    # add the end pose under current transform
+    temp = len(path_list)
+
+    if len(path_list) != 0:
+        if np.linalg.norm(end_pose - path_list[-1]) <= 0.01:
+            path_list[-1] = end_pose
+        else:
+            path_list.append(end_pose)
+    else:
+        path_list.append(end_pose)
+
+    return path_list, end_pose
+        
+def trans_pose(start_pose, length, steer, min_radius):
+    # pose: x, y, theta, 3*1
+    # rotate the start pose with a rot_theta by a center point
+
+    cur_theta = start_pose[2, 0]
+    start_position = start_pose[0:2]
+    rot_theta = steer * length / min_radius
+
+    if rot_theta == 0:
+        trans_matrix = length * np.array([ [cos(cur_theta)], [sin(cur_theta)], [0]])
+        end_pose = start_pose + trans_matrix
+    else:
+        center_theta = cur_theta + steer*pi/2
+        center_position = start_position + min_radius * np.array([ [cos(center_theta)], [sin(center_theta)]])
+
+        rot_matrix = np.array([[cos(rot_theta), -sin(rot_theta)], [sin(rot_theta), cos(rot_theta)]])
+        end_position = center_position + rot_matrix @ (start_position - center_position)
+        end_theta = wraptopi(cur_theta + rot_theta)
+        end_pose = np.vstack((end_position, [end_theta]))
+
+    return end_pose
+
+
+
+# def element_sample(length, start_point, steer_mode, min_radius, step_size):
+#     # generate a series points from the an element
+
+#     cur_x = start_point[0, 0]
+#     cur_y = start_point[1, 0]
+#     cur_theta = start_point[2, 0]
+
+#     path_list = []
+
+#     endpoint = np.zeros((3, 1))
+
+#     if steer_mode == 'L':
+#         steer = 1
+#     elif steer_mode == 'R':
+#         steer = -1
+#     if steer_mode == 'S':
+#         steer = 0
+
+#     curvature = steer * 1/ min_radius
+#     real_length = length * min_radius
+
+#     rot_theta = real_length * curvature
+
+#     # calculate end point
+#     if curvature == 0:
+#         endpoint = trans_point(start_point, cur_theta, real_length)
+#     else:
+#         center_theta = cur_theta + steer*pi/2
+#         center_x = cur_x + cos(center_theta) * min_radius
+#         center_y = cur_y + sin(center_theta) * min_radius
+
+#         center_point = np.array( [ [center_x], [center_y], [center_theta] ])
+
+#         end_cir_theta = cur_theta + rot_theta - steer*pi/2
+#         endpoint = trans_point(center_point, end_cir_theta, min_radius)
+
+#     cur_length = 0
+    
+#     # loop to generate the points
+#     while cur_length <= real_length - step_size:
+        
+#         next_theta = cur_theta + curvature * step_size
+#         cur_length = cur_length + step_size
+
+#         if curvature == 0:
+#             next_x = cur_x + cos(next_theta) * cur_length
+#             next_y = cur_y + sin(next_theta) * cur_length
+#         else:
+#             temp_theta = next_theta - steer*pi/2
+#             next_x = center_x + cos(temp_theta) * min_radius
+#             next_y = center_y + sin(temp_theta) * min_radius
+
+#         next_theta = wraptopi(next_theta)
+
+#         next_point = np.array([[next_x], [next_y], [next_theta]])
+
+#         path_list.append(next_point)
+
+#         cur_theta = next_theta
+
+#     path_list.append(endpoint)
+
+#     return path_list, endpoint
+
+# def trans_point(start_point, theta, length):
+
+#     trans_matrix = np.array([ [ cos(theta) * length ], [ sin(theta) * length ], [ theta ] ])
+#     end_point = start_point + trans_matrix
+#     end_point[2, 0] = wraptopi(end_point[2, 0])
+
+#     return end_point
+
+def dubins_LSL(alpha, beta, d):
+
+    mode = ['L', 'S', 'L']
+
+    temp0 = atan2(cos(beta)- cos(alpha), d+sin(alpha)-sin(beta))
+    t = (-alpha + temp0) % (2*pi)
+
+    temp1 = 2 + d**2 - 2*cos(alpha-beta) + 2 * d * (sin(alpha) - sin(beta))
+
+    if temp1 < 0:
+        return None, None, None, mode
+
+    p = sqrt(temp1)
+
+    q = (beta - temp0) % (2*pi)
+
+    return t, p, q, mode
+
+def dubins_RSR(alpha, beta, d):
+
+    mode = ['R', 'S', 'R']
+
+    temp0 = atan2(cos(alpha)- cos(beta), d-sin(alpha)+sin(beta))
+    t = (alpha - temp0) % (2*pi)
+
+    temp1 = 2 + d**2 - 2*cos(alpha-beta) + 2*d*(sin(beta)-sin(alpha))
+    if temp1 < 0:
+        return None, None, None, mode
+
+    p = sqrt(temp1)
+
+    q = (-beta % (2*pi) + temp0) % (2*pi)
+
+    return t, p, q, mode
+
+def dubins_LSR(alpha, beta, d):
+
+    mode=['L', 'S', 'R']
+
+    temp0 = -2 + d**2 + 2*cos(alpha-beta) + 2*d*(sin(alpha) + sin(beta) )
+    if temp0 < 0:
+        return None, None, None, mode
+
+    p = sqrt(temp0)
+
+    temp1 = atan2( (-cos(alpha)-cos(beta)), (d+sin(alpha)+sin(beta)) )
+    t = (-alpha+temp1 - atan2(-2, p)) % (2*pi)
+
+    q = (-beta % (2*pi)+temp1-atan2(-2, p)) % (2*pi)
+
+    return t, p, q, mode
+    
+def dubins_RSL(alpha, beta, d):
+    
+    mode = ['R', 'S', 'L']
+
+    temp0 = d**2-2+2*cos(alpha-beta)-2*d*(sin(alpha)+sin(beta))
+    if temp0 < 0:
+        return None, None, None, mode
+
+    p = sqrt(temp0)
+
+    temp1 = atan2( (cos(alpha)+cos(beta)), (d-sin(alpha)-sin(beta) ) )
+    t = (alpha - temp1 + atan2(2, p)) % (2*pi)
+
+    q = (beta % (2*pi) - temp1 + atan2(2, p)) % (2*pi)
+
+    return t, p, q, mode
+
+def dubins_RLR(alpha, beta, d):
+
+    mode = ['R', 'L', 'R']
+
+    temp0 = (6-d**2+2*cos(alpha-beta)+2*d*(sin(alpha) - sin(beta))) / 8
+    
+    if abs(temp0) > 1:
+        return None, None, None, mode
+
+    p = acos(temp0)
+    
+    temp1 = atan2( (cos(alpha) - cos(beta)), (d-sin(alpha)+sin(beta)) )
+
+    t = (alpha - temp1 + p/2) % (2*pi)
+
+    q = (alpha - beta - t + p) % (2*pi)
+
+    return t, p, q, mode
+
+# TYPO IN PAPER 
+def dubins_LRL(alpha, beta, d):
+    
+    mode=['L', 'R', 'L']
+
+    temp0 = (6-d**2+2*cos(alpha-beta)+2*d*(sin(beta) - sin(alpha))) / 8 
+    
+    if abs(temp0) > 1:
+        return None, None, None, mode
+
+    p = acos(temp0)
+
+    temp1 = atan2( (cos(beta)) - cos(alpha), (d+sin(alpha)-sin(beta)) )
+    t = (- alpha + temp1 + p/2) % (2*pi)
+
+    q = ( beta % (2*pi) - alpha - t  + p) % (2*pi)
+
+    return t, p, q, mode
+
+
+def relative(state1, state2):
+        
+    diff = state2[0:2] - state1[0:2]
+
+    dis = np.linalg.norm(diff)
+    radian = atan2(diff[1, 0], diff[0, 0])
+    
+    return dis, radian
+
+def wraptopi(rad):
+
+    while rad > pi:
+        rad = rad - 2 * pi
+    
+    while rad < -pi:
+        rad = rad + 2 * pi
+
+    return rad
```

### Comparing `gctl-1.0/gctl/curve/reeds_shepp.py` & `gctl-1.1/gctl/curve/reeds_shepp.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,539 +1,539 @@
-"""
-Code Author: Han Ruihua
-Reference: paper 'Optimal paths for a car that goes both forwards and backwards', github: https://github.com/nathanlct/reeds-shepp-curves/tree/master
-
-timeflip: 
-  positive to negative; 
-  LpSpLp --> LnSnLn
-  x, y, phi --> -x, y, -phi  
-
-reflect:
-  left to right; 
-  LpSpLp -- > RpSpRp
-  x, y, phi --> x, -y, -phi 
-
-backward: 
-    reverse the operation
-    LpRnLn --> LnRnLp  
-    x, y, phi --> xcos(phi) + ysin(phi), sin(phi) - ycos(phi), phi 
-"""
-
-import numpy as np
-from collections import namedtuple
-from math import sqrt, atan2, sin, cos, pi, inf, asin, acos
-
-
-element = namedtuple('element','len steer gear') # steer 1,0,-1, gear 1,-1
-
-def generate_reeds_shepp(start=np.zeros((3, 1)), end=np.ones((3, 1)), min_radius=1, step_size=0.1, include_gear=False, **kwargs):
-
-    """
-    Arguments:
-        start: the start point of the curve: 3* 1 matrix
-        end: the end point of the curve: 3 * 1 matrix
-        min_radius: The minimum turning radius of the car
-        step_size: the distance between each point
-    """
-
-    if isinstance(start, tuple):
-        start = np.array([start]).T
-
-    if isinstance(end, tuple):
-        end = np.array([end]).T
-
-    assert start.shape == (3, 1) and end.shape == (3, 1)
-
-    x, y, phi = preprocess(start, end, min_radius)
-
-    path_formula1 = [LpSpLp, LpSpRp, LpRnLp, LpRpLnnRn, LpRnLnRp, LpRnRnLnRp]
-    path_formula2 = [LpRnLn, LpRnSnLn, LpRnSnRn]
-
-    path_list1, List1 = symmetry_curve1(x, y, phi, path_formula1)
-    path_list2, List2 = symmetry_curve2(x, y, phi, path_formula2)
-
-    total_path_list = path_list1 + path_list2
-    total_L_list = List1 + List2
-    
-    L_min = min(total_L_list) 
-    path_min = total_path_list[total_L_list.index(L_min)]
-
-    path_point_list = path_generate(start, path_min, min_radius, step_size, include_gear)
-
-    return path_point_list
-
-
-def preprocess(start, end, min_radius):
-    # preprocess: get coordinates of end in the set of axis where start is (0,0,0) with unit distance
-
-    ro_phi = start[2, 0]
-    ro_matrix = np.array([[cos(ro_phi), sin(ro_phi)], 
-                        [-sin(ro_phi), cos(ro_phi)]])
-
-    diff = end[0:2] - start[0:2]
-    new_pos = ro_matrix @ diff
-
-    new_x = new_pos[0, 0] / min_radius
-    new_y = new_pos[1, 0] / min_radius
-    new_phi = M(end[2, 0] - start[2, 0])
-
-    return new_x, new_y, new_phi
-
-# calculate curves
-def symmetry_curve1(x, y, phi, path_formula1):
-    
-    path_list = []
-    L_list = []
-
-    for timeflip in [False, True]:
-        for reflect in [False, True]:
-            for cal_formula in path_formula1:
-
-                rg_flag = -1 if timeflip else 1
-                rs_flag = -1 if reflect else 1
-                
-                path, L = cal_formula(rg_flag*x, rs_flag*y, rs_flag*rg_flag*phi, timeflip=timeflip, reflect=reflect)
-
-                path_list.append(path.copy())
-                L_list.append(L)
-    
-    return path_list, L_list
-
-def symmetry_curve2(x, y, phi, path_formula2):
-    
-    path_list = []
-    L_list = []
-
-    for timeflip in [False, True]:
-        for reflect in [False, True]:
-            for backward in [False, True]:
-                for cal_formula in path_formula2:
-
-                    rg_flag = -1 if timeflip else 1 
-                    rs_flag = -1 if reflect else 1
-                    sx, sy, sphi = reverse(x,y,phi) if backward else (x,y,phi)
-                    
-                    path, L = cal_formula(rg_flag*sx, rs_flag*sy, rs_flag*rg_flag*sphi, timeflip=timeflip, reflect=reflect, backward=backward)
-
-                    path_list.append(path.copy())
-                    L_list.append(L)
-    
-    return path_list, L_list
-
-def path_generate(start_point, path, min_radius, step_size, include_gear=False):
-
-    if include_gear and start_point.shape[0] == 3:
-        start_point = start_point = np.vstack((start_point, [path[0].gear]))
-
-    path_point_list = [start_point]
-    end_point = None
-
-    if len(path) == 0:
-        print('no path')
-        return path_point_list
-
-    for i in range(len(path)):
-        
-        path_list, end_point = element_sample(path[i], start_point[0:3], min_radius, step_size, include_gear)
-
-        path_point_list = path_point_list + path_list
-        start_point = end_point
-
-    return path_point_list
-
-def element_sample(element, start_point, min_radius, step_size, include_gear=False):
-
-    real_length = element.len * min_radius
-            
-    path_list = []
-    cur_length = 0
-
-    while cur_length <= real_length - step_size:   
-        cur_length = cur_length + step_size
-        next_pose = trans_pose(start_point[0:3], cur_length, element.steer, min_radius, element.gear, include_gear)
-        path_list.append(next_pose)
-    
-    end_pose = trans_pose(start_point[0:3], real_length, element.steer, min_radius, element.gear, include_gear)
-
-    # add end pose
-    if len(path_list) == 0:
-        path_list.append(end_pose)
-    else:
-        if np.linalg.norm(end_pose - path_list[-1]) <= 0.01:
-            path_list[-1] = end_pose
-        else:
-            path_list.append(end_pose)
-
-    return path_list, end_pose
-
-
-def trans_pose(start_pose, length, steer, min_radius, gear, include_gear=False):
-
-    assert start_pose.shape == (3, 1) 
-
-    cur_theta = start_pose[2, 0]
-    start_position = start_pose[0:2]
-    rot_theta = steer * gear * length / min_radius
-    
-    if rot_theta == 0:
-        trans_matrix = gear * length * np.array([ [cos(cur_theta)], [sin(cur_theta)], [0]])
-        end_pose = start_pose + trans_matrix
-
-    else:
-        center_theta = cur_theta + steer*pi/2
-        center_position = start_position + min_radius * np.array([ [cos(center_theta)], [sin(center_theta)]])
-        
-        rot_matrix = np.array([[cos(rot_theta), -sin(rot_theta)], [sin(rot_theta), cos(rot_theta)]])
-        end_position = center_position + rot_matrix @ (start_position - center_position)
-        end_theta = M(cur_theta + rot_theta)
-        end_pose = np.vstack((end_position, [end_theta]))
-
-    if include_gear:
-        end_pose = np.vstack((end_pose, [gear]))
-    
-    return end_pose
-
-
-# def motion_acker_step(start_point, gear, steer, step_size, include_gear=False):
-    
-#     cur_x = start_point[0, 0]
-#     cur_y = start_point[1, 0]
-#     cur_theta = start_point[2, 0]
-
-#     curvature = steer * 1/self.min_r
-    
-#     rot_theta = abs(steer) * step_size * curvature * gear
-#     trans_len = (1 - abs(steer)) * step_size * gear
-
-#     rot_matrix = np.array([[cos(rot_theta), -sin(rot_theta)], [sin(rot_theta), cos(rot_theta)]])
-#     trans_matrix = trans_len * np.array([[cos(cur_theta)], [sin(cur_theta)]]) 
-
-#     center_x = cur_x + cos(cur_theta + steer * pi/2) * self.min_r
-#     center_y = cur_y + sin(cur_theta + steer * pi/2) * self.min_r
-#     center = np.array([[center_x], [center_y]])
-
-#     if include_gear:
-#         new_state = np.zeros((4, 1))
-#         new_state[0:2] = rot_matrix @ (start_point[0:2] - center) + center + trans_matrix
-#         new_state[2, 0] = self.wraptopi(cur_theta + rot_theta)
-#         new_state[3, 0] = gear
-#     else:
-#         new_state = np.zeros((3, 1))
-#         new_state[0:2] = rot_matrix @ (start_point[0:2] - center) + center + trans_matrix
-#         new_state[2, 0] = self.wraptopi(cur_theta + rot_theta)
-    
-#     return new_state
-
-
-# trans to (-pi, pi)
-def M(theta):
-    theta = theta % (2*pi)
-    if theta < - pi: return theta + 2*pi
-    if theta >= pi: return theta - 2*pi
-    return theta
-
-# Polar coordinate  
-def R(x, y):   
-    r = sqrt(x**2 + y**2)
-    theta = atan2(y, x)
-    return r, theta
-
-# for backwards (reverse)
-def reverse(x, y, phi):
-    new_x = x*cos(phi) + y*sin(phi)
-    new_y = x*sin(phi) - y*cos(phi)
-    return new_x, new_y, phi
-
-
-# curve formula
-
-# formula 8.1
-def LpSpLp(x, y, phi, timeflip=False, reflect=False):
-    
-    path = []
-    gear_flag = -1 if timeflip else 1
-    steer_flag = -1 if reflect else 1
-
-    #calculate
-    u, t = R(x - sin(phi), y-1+cos(phi))
-    v = (phi - t) % (2*pi)
-
-    if t<0 or u<0 or v<0:
-        return path, inf
-
-    path.append(element(t, steer_flag, gear_flag)) 
-    path.append(element(u, 0, gear_flag)) 
-    path.append(element(v, steer_flag, gear_flag))
-
-    L = abs(t) + abs(u) + abs(v)
-
-    return path, L
-
-# formula 8.2
-def LpSpRp(x, y, phi, timeflip=False, reflect=False):
-
-    path = []
-    gear_flag = -1 if timeflip else 1
-    steer_flag = -1 if reflect else 1
-
-    u1, t1 = R(x+sin(phi), y-1-cos(phi))
-
-    if u1**2 < 4:
-        L = inf
-    else:
-        u = sqrt(u1**2 - 4)
-
-        T, theta = R(u, 2)
-        t = M(t1+theta)
-        v = M(t-phi)
-        L = abs(t) + abs(u) + abs(v)
-
-        if t<0 or u<0 or v<0:
-            return path, inf
-
-        path.append(element(t, steer_flag*1, gear_flag)) 
-        path.append(element(u, 0, gear_flag)) 
-        path.append(element(v, steer_flag*-1, gear_flag))   
-
-    return path, L
-
-# formula 8.3  typo in paper
-def LpRnLp(x, y, phi, timeflip=False, reflect=False):
-
-    path = []
-    gear_flag = -1 if timeflip else 1
-    steer_flag = -1 if reflect else 1
-
-    xi = x - sin(phi)
-    eta = y - 1 + cos(phi)
-    u1, theta = R(xi, eta)
-
-    # if u1 ** 2 > 4:
-    #     return path, inf
-    if u1 > 4:
-        return path, inf
-    
-    A = acos(u1/4)
-    t = M(theta + pi/2 + A)
-    u = M(pi - 2*A)
-    v = M(phi-t-u)
-    
-    L = abs(t) + abs(u) + abs(v)
-
-    if t<0 or u<0 or v<0:
-        return path, inf
-
-    path.append(element(t, steer_flag*1, gear_flag*1)) 
-    path.append(element(u, steer_flag*-1, gear_flag*-1)) 
-    path.append(element(v, steer_flag*1, gear_flag*1)) 
-
-    return path, L
-
-# formula 8.4, typo in paper, 
-def LpRnLn(x, y, phi, timeflip=False, reflect=False, backward=False):
-
-    path = []
-    gear_flag = -1 if timeflip else 1
-    steer_flag = -1 if reflect else 1
-
-    xi = x - sin(phi)
-    eta = y - 1 + cos(phi)
-    u1, theta = R(xi, eta)
-
-    if u1  > 4:
-        return path, inf
-    
-    A = acos(u1/4)
-    t = M(theta + pi/2 + A)
-    u = M(pi - 2*A)
-    v = M(t+u-phi)
-    
-    if t<0 or u<0 or v<0:
-        return path, inf
-    
-    L = abs(t) + abs(u) + abs(v)
-
-    if backward:
-        path.append(element(v, steer_flag*1, gear_flag*-1))
-        path.append(element(u, steer_flag*-1, gear_flag*-1))
-        path.append(element(t, steer_flag*1, gear_flag*1))
-    else:
-        path.append(element(t, steer_flag*1, gear_flag*1)) 
-        path.append(element(u, steer_flag*-1, gear_flag*-1)) 
-        path.append(element(v, steer_flag*1, gear_flag*-1)) 
-
-    return path, L
-
-# formula 8.7 typo in paper
-def LpRpLnnRn(x, y, phi, timeflip=False, reflect=False):
-
-    path = []
-    gear_flag = -1 if timeflip else 1
-    steer_flag = -1 if reflect else 1
-
-    xi = x + sin(phi)
-    eta = y - 1 - cos(phi)
-    u1, theta = R(xi, eta)
-
-    if u1 > 4:
-        return path, inf 
-    
-    if u1 <= 2:
-        A = acos((u1+2)/4)
-        t = M(theta+pi/2+A)
-        u = M(A)
-        v = M(phi-t+2*u)
-    else:
-        A = acos((u1-2)/4)
-        t = M(theta+pi/2-A)
-        u = M(pi-A)
-        v = M(phi-t+2*u)
-    
-    if t<0 or u<0 or v<0:
-        return path, inf
-
-    L = abs(t) + 2*abs(u) + abs(v)
-
-    path.append(element(t, steer_flag*1, gear_flag*1)) 
-    path.append(element(u, steer_flag*-1, gear_flag*1)) 
-    path.append(element(u, steer_flag*1, gear_flag*-1))
-    path.append(element(v, steer_flag*-1, gear_flag*-1))  
-
-    return path, L
-
-# formula 8.8 
-def LpRnLnRp(x, y, phi, timeflip=False, reflect=False):
-    
-    path = []
-    gear_flag = -1 if timeflip else 1
-    steer_flag = -1 if reflect else 1
-
-    xi = x + sin(phi)
-    eta = y - 1 - cos(phi)
-    u1, theta = R(xi, eta)
-    rho = (20 - u1**2) / 16
-
-    if rho >= 0 and rho <= 1 and u1<=6:
-        u = acos(rho)
-        A = asin(2*sin(u)/u1)
-        t = M(theta+pi/2+A)
-        v = M(t-phi)
-
-        if t<0 or u<0 or v<0:
-            return path, inf
-        
-        L = abs(t) + 2*abs(u) + abs(v)
-
-        path.append(element(t, steer_flag*1, gear_flag*1)) 
-        path.append(element(u, steer_flag*-1, gear_flag*-1)) 
-        path.append(element(u, steer_flag*1, gear_flag*-1))
-        path.append(element(v, steer_flag*-1, gear_flag*1))  
-
-    else:
-        return path, inf
-
-    return path, L
-
-# formula 8.9
-def LpRnSnLn(x, y, phi, timeflip=False, reflect=False, backward=False):
-    
-    path = []
-    gear_flag = -1 if timeflip else 1
-    steer_flag = -1 if reflect else 1
-
-    xi = x - sin(phi)
-    eta = y - 1 + cos(phi)
-    rho, theta = R(xi, eta)
-    
-    if rho < 2:
-        return path, inf
-    
-    u = sqrt(rho**2-4) -2
-    A = atan2(2, u+2)
-    t = M(theta+pi/2+A)
-    v = M(t-phi+pi/2)
-
-    if t<0 or u<0 or v<0:
-        return path, inf
-    
-    L = abs(t) + pi/2 + abs(u) + abs(v)
-
-    if backward:
-        path.append(element(v, steer_flag*1, gear_flag*-1)) 
-        path.append(element(u, steer_flag*0, gear_flag*-1))
-        path.append(element(pi/2, steer_flag*-1, gear_flag*-1)) 
-        path.append(element(t, steer_flag*1, gear_flag*1))               
-    else:
-        path.append(element(t, steer_flag*1, gear_flag*1)) 
-        path.append(element(pi/2, steer_flag*-1, gear_flag*-1)) 
-        path.append(element(u, steer_flag*0, gear_flag*-1))
-        path.append(element(v, steer_flag*1, gear_flag*-1)) 
-
-    return path, L
-
-# formula 8.10
-def LpRnSnRn(x, y, phi, timeflip=False, reflect=False, backward=False):
-
-    path = []
-    gear_flag = -1 if timeflip else 1
-    steer_flag = -1 if reflect else 1
-
-    xi = x + sin(phi)
-    eta = y - 1 - cos(phi)
-    rho, theta = R(xi, eta)
-
-    if rho < 2:
-        return path, inf
-
-    t = M(theta+pi/2)
-    u = rho-2
-    v = M(phi - t -pi/2)
-
-    if t<0 or u<0 or v<0:
-        return path, inf
-
-    L = abs(t) + pi/2 + abs(u) + abs(v)
-    
-    if backward:
-        path.append(element(v, steer_flag*-1, gear_flag*-1))
-        path.append(element(u, steer_flag*0, gear_flag*-1)) 
-        path.append(element(pi/2, steer_flag*-1, gear_flag*-1)) 
-        path.append(element(t, steer_flag*1, gear_flag*1))
-    else:
-        path.append(element(t, steer_flag*1, gear_flag*1)) 
-        path.append(element(pi/2, steer_flag*-1, gear_flag*-1)) 
-        path.append(element(u, steer_flag*0, gear_flag*-1))
-        path.append(element(v, steer_flag*-1, gear_flag*-1))
-
-    return path, L
-
-# formula 8.11 typo in paper
-def LpRnRnLnRp(x, y, phi, timeflip=False, reflect=False):
-
-    path = []
-    gear_flag = -1 if timeflip else 1
-    steer_flag = -1 if reflect else 1
-
-    xi = x + sin(phi)
-    eta = y - 1 - cos(phi)
-    rho, theta = R(xi, eta)
-
-    if rho < 4:
-        return path, inf
-
-    u = sqrt(rho**2 - 4) - 4
-    A = atan2(2, u+4)
-    t = M(theta+pi/2+A)
-    v = M(t-phi)
-
-    if t<0 or u<0 or v<0:
-        return path, inf
-
-    L = abs(t) + pi/2 + abs(u) + pi/2 + abs(v)
-
-    path.append(element(t, steer_flag*1, gear_flag*1)) 
-    path.append(element(pi/2, steer_flag*-1, gear_flag*-1)) 
-    path.append(element(u, steer_flag*0, gear_flag*-1))
-    path.append(element(pi/2, steer_flag*1, gear_flag*-1))
-    path.append(element(v, steer_flag*-1, gear_flag*1))
-
+"""
+Code Author: Han Ruihua
+Reference: paper 'Optimal paths for a car that goes both forwards and backwards', github: https://github.com/nathanlct/reeds-shepp-curves/tree/master
+
+timeflip: 
+  positive to negative; 
+  LpSpLp --> LnSnLn
+  x, y, phi --> -x, y, -phi  
+
+reflect:
+  left to right; 
+  LpSpLp -- > RpSpRp
+  x, y, phi --> x, -y, -phi 
+
+backward: 
+    reverse the operation
+    LpRnLn --> LnRnLp  
+    x, y, phi --> xcos(phi) + ysin(phi), sin(phi) - ycos(phi), phi 
+"""
+
+import numpy as np
+from collections import namedtuple
+from math import sqrt, atan2, sin, cos, pi, inf, asin, acos
+
+
+element = namedtuple('element','len steer gear') # steer 1,0,-1, gear 1,-1
+
+def generate_reeds_shepp(start=np.zeros((3, 1)), end=np.ones((3, 1)), min_radius=1, step_size=0.1, include_gear=False, **kwargs):
+
+    """
+    Arguments:
+        start: the start point of the curve: 3* 1 matrix
+        end: the end point of the curve: 3 * 1 matrix
+        min_radius: The minimum turning radius of the car
+        step_size: the distance between each point
+    """
+
+    if isinstance(start, tuple):
+        start = np.array([start]).T
+
+    if isinstance(end, tuple):
+        end = np.array([end]).T
+
+    assert start.shape == (3, 1) and end.shape == (3, 1)
+
+    x, y, phi = preprocess(start, end, min_radius)
+
+    path_formula1 = [LpSpLp, LpSpRp, LpRnLp, LpRpLnnRn, LpRnLnRp, LpRnRnLnRp]
+    path_formula2 = [LpRnLn, LpRnSnLn, LpRnSnRn]
+
+    path_list1, List1 = symmetry_curve1(x, y, phi, path_formula1)
+    path_list2, List2 = symmetry_curve2(x, y, phi, path_formula2)
+
+    total_path_list = path_list1 + path_list2
+    total_L_list = List1 + List2
+    
+    L_min = min(total_L_list) 
+    path_min = total_path_list[total_L_list.index(L_min)]
+
+    path_point_list = path_generate(start, path_min, min_radius, step_size, include_gear)
+
+    return path_point_list
+
+
+def preprocess(start, end, min_radius):
+    # preprocess: get coordinates of end in the set of axis where start is (0,0,0) with unit distance
+
+    ro_phi = start[2, 0]
+    ro_matrix = np.array([[cos(ro_phi), sin(ro_phi)], 
+                        [-sin(ro_phi), cos(ro_phi)]])
+
+    diff = end[0:2] - start[0:2]
+    new_pos = ro_matrix @ diff
+
+    new_x = new_pos[0, 0] / min_radius
+    new_y = new_pos[1, 0] / min_radius
+    new_phi = M(end[2, 0] - start[2, 0])
+
+    return new_x, new_y, new_phi
+
+# calculate curves
+def symmetry_curve1(x, y, phi, path_formula1):
+    
+    path_list = []
+    L_list = []
+
+    for timeflip in [False, True]:
+        for reflect in [False, True]:
+            for cal_formula in path_formula1:
+
+                rg_flag = -1 if timeflip else 1
+                rs_flag = -1 if reflect else 1
+                
+                path, L = cal_formula(rg_flag*x, rs_flag*y, rs_flag*rg_flag*phi, timeflip=timeflip, reflect=reflect)
+
+                path_list.append(path.copy())
+                L_list.append(L)
+    
+    return path_list, L_list
+
+def symmetry_curve2(x, y, phi, path_formula2):
+    
+    path_list = []
+    L_list = []
+
+    for timeflip in [False, True]:
+        for reflect in [False, True]:
+            for backward in [False, True]:
+                for cal_formula in path_formula2:
+
+                    rg_flag = -1 if timeflip else 1 
+                    rs_flag = -1 if reflect else 1
+                    sx, sy, sphi = reverse(x,y,phi) if backward else (x,y,phi)
+                    
+                    path, L = cal_formula(rg_flag*sx, rs_flag*sy, rs_flag*rg_flag*sphi, timeflip=timeflip, reflect=reflect, backward=backward)
+
+                    path_list.append(path.copy())
+                    L_list.append(L)
+    
+    return path_list, L_list
+
+def path_generate(start_point, path, min_radius, step_size, include_gear=False):
+
+    if include_gear and start_point.shape[0] == 3:
+        start_point = start_point = np.vstack((start_point, [path[0].gear]))
+
+    path_point_list = [start_point]
+    end_point = None
+
+    if len(path) == 0:
+        print('no path')
+        return path_point_list
+
+    for i in range(len(path)):
+        
+        path_list, end_point = element_sample(path[i], start_point[0:3], min_radius, step_size, include_gear)
+
+        path_point_list = path_point_list + path_list
+        start_point = end_point
+
+    return path_point_list
+
+def element_sample(element, start_point, min_radius, step_size, include_gear=False):
+
+    real_length = element.len * min_radius
+            
+    path_list = []
+    cur_length = 0
+
+    while cur_length <= real_length - step_size:   
+        cur_length = cur_length + step_size
+        next_pose = trans_pose(start_point[0:3], cur_length, element.steer, min_radius, element.gear, include_gear)
+        path_list.append(next_pose)
+    
+    end_pose = trans_pose(start_point[0:3], real_length, element.steer, min_radius, element.gear, include_gear)
+
+    # add end pose
+    if len(path_list) == 0:
+        path_list.append(end_pose)
+    else:
+        if np.linalg.norm(end_pose - path_list[-1]) <= 0.01:
+            path_list[-1] = end_pose
+        else:
+            path_list.append(end_pose)
+
+    return path_list, end_pose
+
+
+def trans_pose(start_pose, length, steer, min_radius, gear, include_gear=False):
+
+    assert start_pose.shape == (3, 1) 
+
+    cur_theta = start_pose[2, 0]
+    start_position = start_pose[0:2]
+    rot_theta = steer * gear * length / min_radius
+    
+    if rot_theta == 0:
+        trans_matrix = gear * length * np.array([ [cos(cur_theta)], [sin(cur_theta)], [0]])
+        end_pose = start_pose + trans_matrix
+
+    else:
+        center_theta = cur_theta + steer*pi/2
+        center_position = start_position + min_radius * np.array([ [cos(center_theta)], [sin(center_theta)]])
+        
+        rot_matrix = np.array([[cos(rot_theta), -sin(rot_theta)], [sin(rot_theta), cos(rot_theta)]])
+        end_position = center_position + rot_matrix @ (start_position - center_position)
+        end_theta = M(cur_theta + rot_theta)
+        end_pose = np.vstack((end_position, [end_theta]))
+
+    if include_gear:
+        end_pose = np.vstack((end_pose, [gear]))
+    
+    return end_pose
+
+
+# def motion_acker_step(start_point, gear, steer, step_size, include_gear=False):
+    
+#     cur_x = start_point[0, 0]
+#     cur_y = start_point[1, 0]
+#     cur_theta = start_point[2, 0]
+
+#     curvature = steer * 1/self.min_r
+    
+#     rot_theta = abs(steer) * step_size * curvature * gear
+#     trans_len = (1 - abs(steer)) * step_size * gear
+
+#     rot_matrix = np.array([[cos(rot_theta), -sin(rot_theta)], [sin(rot_theta), cos(rot_theta)]])
+#     trans_matrix = trans_len * np.array([[cos(cur_theta)], [sin(cur_theta)]]) 
+
+#     center_x = cur_x + cos(cur_theta + steer * pi/2) * self.min_r
+#     center_y = cur_y + sin(cur_theta + steer * pi/2) * self.min_r
+#     center = np.array([[center_x], [center_y]])
+
+#     if include_gear:
+#         new_state = np.zeros((4, 1))
+#         new_state[0:2] = rot_matrix @ (start_point[0:2] - center) + center + trans_matrix
+#         new_state[2, 0] = self.wraptopi(cur_theta + rot_theta)
+#         new_state[3, 0] = gear
+#     else:
+#         new_state = np.zeros((3, 1))
+#         new_state[0:2] = rot_matrix @ (start_point[0:2] - center) + center + trans_matrix
+#         new_state[2, 0] = self.wraptopi(cur_theta + rot_theta)
+    
+#     return new_state
+
+
+# trans to (-pi, pi)
+def M(theta):
+    theta = theta % (2*pi)
+    if theta < - pi: return theta + 2*pi
+    if theta >= pi: return theta - 2*pi
+    return theta
+
+# Polar coordinate  
+def R(x, y):   
+    r = sqrt(x**2 + y**2)
+    theta = atan2(y, x)
+    return r, theta
+
+# for backwards (reverse)
+def reverse(x, y, phi):
+    new_x = x*cos(phi) + y*sin(phi)
+    new_y = x*sin(phi) - y*cos(phi)
+    return new_x, new_y, phi
+
+
+# curve formula
+
+# formula 8.1
+def LpSpLp(x, y, phi, timeflip=False, reflect=False):
+    
+    path = []
+    gear_flag = -1 if timeflip else 1
+    steer_flag = -1 if reflect else 1
+
+    #calculate
+    u, t = R(x - sin(phi), y-1+cos(phi))
+    v = (phi - t) % (2*pi)
+
+    if t<0 or u<0 or v<0:
+        return path, inf
+
+    path.append(element(t, steer_flag, gear_flag)) 
+    path.append(element(u, 0, gear_flag)) 
+    path.append(element(v, steer_flag, gear_flag))
+
+    L = abs(t) + abs(u) + abs(v)
+
+    return path, L
+
+# formula 8.2
+def LpSpRp(x, y, phi, timeflip=False, reflect=False):
+
+    path = []
+    gear_flag = -1 if timeflip else 1
+    steer_flag = -1 if reflect else 1
+
+    u1, t1 = R(x+sin(phi), y-1-cos(phi))
+
+    if u1**2 < 4:
+        L = inf
+    else:
+        u = sqrt(u1**2 - 4)
+
+        T, theta = R(u, 2)
+        t = M(t1+theta)
+        v = M(t-phi)
+        L = abs(t) + abs(u) + abs(v)
+
+        if t<0 or u<0 or v<0:
+            return path, inf
+
+        path.append(element(t, steer_flag*1, gear_flag)) 
+        path.append(element(u, 0, gear_flag)) 
+        path.append(element(v, steer_flag*-1, gear_flag))   
+
+    return path, L
+
+# formula 8.3  typo in paper
+def LpRnLp(x, y, phi, timeflip=False, reflect=False):
+
+    path = []
+    gear_flag = -1 if timeflip else 1
+    steer_flag = -1 if reflect else 1
+
+    xi = x - sin(phi)
+    eta = y - 1 + cos(phi)
+    u1, theta = R(xi, eta)
+
+    # if u1 ** 2 > 4:
+    #     return path, inf
+    if u1 > 4:
+        return path, inf
+    
+    A = acos(u1/4)
+    t = M(theta + pi/2 + A)
+    u = M(pi - 2*A)
+    v = M(phi-t-u)
+    
+    L = abs(t) + abs(u) + abs(v)
+
+    if t<0 or u<0 or v<0:
+        return path, inf
+
+    path.append(element(t, steer_flag*1, gear_flag*1)) 
+    path.append(element(u, steer_flag*-1, gear_flag*-1)) 
+    path.append(element(v, steer_flag*1, gear_flag*1)) 
+
+    return path, L
+
+# formula 8.4, typo in paper, 
+def LpRnLn(x, y, phi, timeflip=False, reflect=False, backward=False):
+
+    path = []
+    gear_flag = -1 if timeflip else 1
+    steer_flag = -1 if reflect else 1
+
+    xi = x - sin(phi)
+    eta = y - 1 + cos(phi)
+    u1, theta = R(xi, eta)
+
+    if u1  > 4:
+        return path, inf
+    
+    A = acos(u1/4)
+    t = M(theta + pi/2 + A)
+    u = M(pi - 2*A)
+    v = M(t+u-phi)
+    
+    if t<0 or u<0 or v<0:
+        return path, inf
+    
+    L = abs(t) + abs(u) + abs(v)
+
+    if backward:
+        path.append(element(v, steer_flag*1, gear_flag*-1))
+        path.append(element(u, steer_flag*-1, gear_flag*-1))
+        path.append(element(t, steer_flag*1, gear_flag*1))
+    else:
+        path.append(element(t, steer_flag*1, gear_flag*1)) 
+        path.append(element(u, steer_flag*-1, gear_flag*-1)) 
+        path.append(element(v, steer_flag*1, gear_flag*-1)) 
+
+    return path, L
+
+# formula 8.7 typo in paper
+def LpRpLnnRn(x, y, phi, timeflip=False, reflect=False):
+
+    path = []
+    gear_flag = -1 if timeflip else 1
+    steer_flag = -1 if reflect else 1
+
+    xi = x + sin(phi)
+    eta = y - 1 - cos(phi)
+    u1, theta = R(xi, eta)
+
+    if u1 > 4:
+        return path, inf 
+    
+    if u1 <= 2:
+        A = acos((u1+2)/4)
+        t = M(theta+pi/2+A)
+        u = M(A)
+        v = M(phi-t+2*u)
+    else:
+        A = acos((u1-2)/4)
+        t = M(theta+pi/2-A)
+        u = M(pi-A)
+        v = M(phi-t+2*u)
+    
+    if t<0 or u<0 or v<0:
+        return path, inf
+
+    L = abs(t) + 2*abs(u) + abs(v)
+
+    path.append(element(t, steer_flag*1, gear_flag*1)) 
+    path.append(element(u, steer_flag*-1, gear_flag*1)) 
+    path.append(element(u, steer_flag*1, gear_flag*-1))
+    path.append(element(v, steer_flag*-1, gear_flag*-1))  
+
+    return path, L
+
+# formula 8.8 
+def LpRnLnRp(x, y, phi, timeflip=False, reflect=False):
+    
+    path = []
+    gear_flag = -1 if timeflip else 1
+    steer_flag = -1 if reflect else 1
+
+    xi = x + sin(phi)
+    eta = y - 1 - cos(phi)
+    u1, theta = R(xi, eta)
+    rho = (20 - u1**2) / 16
+
+    if rho >= 0 and rho <= 1 and u1<=6:
+        u = acos(rho)
+        A = asin(2*sin(u)/u1)
+        t = M(theta+pi/2+A)
+        v = M(t-phi)
+
+        if t<0 or u<0 or v<0:
+            return path, inf
+        
+        L = abs(t) + 2*abs(u) + abs(v)
+
+        path.append(element(t, steer_flag*1, gear_flag*1)) 
+        path.append(element(u, steer_flag*-1, gear_flag*-1)) 
+        path.append(element(u, steer_flag*1, gear_flag*-1))
+        path.append(element(v, steer_flag*-1, gear_flag*1))  
+
+    else:
+        return path, inf
+
+    return path, L
+
+# formula 8.9
+def LpRnSnLn(x, y, phi, timeflip=False, reflect=False, backward=False):
+    
+    path = []
+    gear_flag = -1 if timeflip else 1
+    steer_flag = -1 if reflect else 1
+
+    xi = x - sin(phi)
+    eta = y - 1 + cos(phi)
+    rho, theta = R(xi, eta)
+    
+    if rho < 2:
+        return path, inf
+    
+    u = sqrt(rho**2-4) -2
+    A = atan2(2, u+2)
+    t = M(theta+pi/2+A)
+    v = M(t-phi+pi/2)
+
+    if t<0 or u<0 or v<0:
+        return path, inf
+    
+    L = abs(t) + pi/2 + abs(u) + abs(v)
+
+    if backward:
+        path.append(element(v, steer_flag*1, gear_flag*-1)) 
+        path.append(element(u, steer_flag*0, gear_flag*-1))
+        path.append(element(pi/2, steer_flag*-1, gear_flag*-1)) 
+        path.append(element(t, steer_flag*1, gear_flag*1))               
+    else:
+        path.append(element(t, steer_flag*1, gear_flag*1)) 
+        path.append(element(pi/2, steer_flag*-1, gear_flag*-1)) 
+        path.append(element(u, steer_flag*0, gear_flag*-1))
+        path.append(element(v, steer_flag*1, gear_flag*-1)) 
+
+    return path, L
+
+# formula 8.10
+def LpRnSnRn(x, y, phi, timeflip=False, reflect=False, backward=False):
+
+    path = []
+    gear_flag = -1 if timeflip else 1
+    steer_flag = -1 if reflect else 1
+
+    xi = x + sin(phi)
+    eta = y - 1 - cos(phi)
+    rho, theta = R(xi, eta)
+
+    if rho < 2:
+        return path, inf
+
+    t = M(theta+pi/2)
+    u = rho-2
+    v = M(phi - t -pi/2)
+
+    if t<0 or u<0 or v<0:
+        return path, inf
+
+    L = abs(t) + pi/2 + abs(u) + abs(v)
+    
+    if backward:
+        path.append(element(v, steer_flag*-1, gear_flag*-1))
+        path.append(element(u, steer_flag*0, gear_flag*-1)) 
+        path.append(element(pi/2, steer_flag*-1, gear_flag*-1)) 
+        path.append(element(t, steer_flag*1, gear_flag*1))
+    else:
+        path.append(element(t, steer_flag*1, gear_flag*1)) 
+        path.append(element(pi/2, steer_flag*-1, gear_flag*-1)) 
+        path.append(element(u, steer_flag*0, gear_flag*-1))
+        path.append(element(v, steer_flag*-1, gear_flag*-1))
+
+    return path, L
+
+# formula 8.11 typo in paper
+def LpRnRnLnRp(x, y, phi, timeflip=False, reflect=False):
+
+    path = []
+    gear_flag = -1 if timeflip else 1
+    steer_flag = -1 if reflect else 1
+
+    xi = x + sin(phi)
+    eta = y - 1 - cos(phi)
+    rho, theta = R(xi, eta)
+
+    if rho < 4:
+        return path, inf
+
+    u = sqrt(rho**2 - 4) - 4
+    A = atan2(2, u+4)
+    t = M(theta+pi/2+A)
+    v = M(t-phi)
+
+    if t<0 or u<0 or v<0:
+        return path, inf
+
+    L = abs(t) + pi/2 + abs(u) + pi/2 + abs(v)
+
+    path.append(element(t, steer_flag*1, gear_flag*1)) 
+    path.append(element(pi/2, steer_flag*-1, gear_flag*-1)) 
+    path.append(element(u, steer_flag*0, gear_flag*-1))
+    path.append(element(pi/2, steer_flag*1, gear_flag*-1))
+    path.append(element(v, steer_flag*-1, gear_flag*1))
+
     return path, L
```

### Comparing `gctl-1.0/gctl/curve_generator.py` & `gctl-1.1/gctl/curve_generator.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,230 +1,230 @@
-from tkinter import Scale
-import numpy as np
-from gctl.curve.dubins_path import generate_dubins_path
-from gctl.curve.reeds_shepp import generate_reeds_shepp
-import matplotlib.pyplot as plt
-from math import cos, sin, atan2
-
-class curve_generator:
-    def __init__(self, select_mode='default', point_style='pose', x_limit = [0, 10], y_limit=[0, 10]) -> None:
-        """
-        # select_mode: mode of point selection
-            # 'default', use the input point_list
-            # 'mouse', use mouse to select points or vectors
-                -- left click to select points and vectors
-                -- key enter to generate the curve
-        
-        # point_style
-            # position: x,y 2 * 1 matrix
-            # pose: x, y, theta, 3*1 matrix, include orientation
-        """
-        self.select_mode = select_mode
-        self.point_style = point_style
-        
-        self.x_limit = x_limit
-        self.y_limit = y_limit
-
-        if select_mode =='mouse':
-            self.fig, self.ax = plt.subplots()
-            self.ax.set_aspect('equal')
-            self.ax.set_xlim(x_limit)
-            self.ax.set_ylim(y_limit)
-
-        self.cpl = [] # click point list
-
-    def generate_curve(self, curve_style='dubins', way_points=[], step_size = 0.1, min_radius=1, include_gear=False, **kwargs):
-        
-        # way_points: The list of way points
-        # step_size: distance between the sample points
-
-        # min_radius: minimum turning radius for ackermann robot
-        # curve: a list of points
-
-        # curve_style: 
-            # - line: connect the points with line
-            # - reeds: connect the points with reeds shepp path
-            # - dubins: connect the points with dubins path
-        
-        # include_gear: if True, the curve should include the gear flag (-1, 1) and the points should be the 4*1 matrix. Used for reeds shepp
-
-        self.way_points = way_points
-        self.pnum = len(self.way_points)
-
-        if len(way_points) != 0: 
-            self.pdim = self.way_points[0].shape
-        elif self.point_style == 'position':
-            self.pdim = (2, 1)
-        elif self.point_style == 'pose':
-            self.pdim = (3, 1)
-
-        if self.select_mode == 'default':
-
-            if len(way_points) == 0:
-                print('Error: No waypoints !')
-                return None
-
-            curve = self.curve_from_waypoints(curve_style, min_radius, step_size, include_gear, **kwargs)
-
-        elif self.select_mode == 'mouse':
-            # generate reference path by mouse    
-            print('Left-slick to select the way point, Enter to generate the curve')
-
-            def on_press(event):
-                if event.key == 'enter':
-                    
-                    print('press enter, generate curves')
-
-                    if self.point_style == 'position':
-                        self.way_points = self.cpl
-                        self.pnum = len(self.way_points)
-
-                    elif self.point_style == 'pose':
-                        curve = self.curve_from_waypoints(curve_style, min_radius, step_size, include_gear, **kwargs)
-                        self.plot_curve(curve, show_way_points=False)
-                        plt.pause(0.001)
-                
-                if event.key == 'escape':
-                    plt.close()
-
-            self.fig.canvas.mpl_connect('button_press_event', self.onclick)
-            self.fig.canvas.mpl_connect('key_press_event', on_press)
-            plt.show()
-        
-        curve = self.curve_from_waypoints(curve_style, min_radius, step_size, include_gear, **kwargs)
-
-        return curve
-
-    def curve_from_waypoints(self, curve_style, min_radius, step_size, include_gear, **kwargs):
-        
-        curve = [ self.way_points[0] ]
-
-        if curve_style == 'dubins':
-            # generate dubins curve
-            for i in range(self.pnum - 1):
-                start_point = self.way_points[i]
-                end_point = self.way_points[i+1]
-                single_curve = generate_dubins_path(start_point, end_point, min_radius, step_size)
-                curve = curve + single_curve[1:]
-
-        elif curve_style == 'reeds':
-            # generate reeds shepp curve
-            for i in range(self.pnum - 1):
-                start_point = self.way_points[i]
-                end_point = self.way_points[i+1]
-                single_curve = generate_reeds_shepp(start_point, end_point, min_radius, step_size, include_gear, **kwargs)
-                curve = curve + single_curve[1:] 
-
-            if include_gear and self.pdim[0] == 3:
-                curve[0] = np.vstack((curve[0], [curve[1][-1, 0]]))
-
-        elif curve_style == 'line':
-            
-            for i in range(self.pnum - 1):
-                start_point = self.way_points[i]
-                end_point = self.way_points[i+1]
-                single_curve = self.generate_line(start_point, end_point, step_size)
-                curve = curve + single_curve[1:]
-
-        else:
-            print('wrong curve type')
-
-        return curve
-
-    def onclick(self, event):
-        print('%s click: button=%d, x=%d, y=%d, xdata=%f, ydata=%f' %
-            ('double' if event.dblclick else 'single', event.button,
-            event.x, event.y, event.xdata, event.ydata))
-
-        if self.point_style == 'position':
-            self.cpl.append(np.array([ [event.xdata], [event.ydata] ]))
-            self.ax.scatter(event.xdata, event.ydata, c='k')
-            plt.pause(0.001)
-        
-        elif self.point_style == 'pose':
-            self.cpl.append(np.array([ [event.xdata], [event.ydata] ]))
-            
-            if len(self.cpl) == 1:
-                self.ax.scatter(event.xdata, event.ydata, c='k')
-
-            if len(self.cpl) == 2:
-                diff = self.cpl[1] - self.cpl[0]
-                theta = atan2(diff[1, 0], diff[0, 0])
-                
-                self.ax.quiver(self.cpl[0][0, 0], self.cpl[0][1, 0], diff[0, 0], diff[1, 0], color='r', scale=20)
-
-                way_point = np.vstack((self.cpl[0], [theta]))
-                self.way_points.append(way_point)
-                self.pnum = len(self.way_points)
-
-                self.cpl = []
-
-            plt.pause(0.001)
-
-
-    def plot_curve(self, curve, style='-g', show_way_points=True, show_direction=False, **kwargs):
-
-        # self.ax.set_xlim(range_x)
-        # self.ax.set_ylim(range_y)
-
-        if self.select_mode =='default':
-            self.fig, self.ax = plt.subplots()
-            self.ax.set_aspect('equal')
-            self.ax.set_xlim(self.x_limit)
-            self.ax.set_ylim(self.y_limit) 
-
-        path_x_list = [p[0, 0] for p in curve]
-        path_y_list = [p[1, 0] for p in curve]
-
-        self.ax.plot(path_x_list, path_y_list, style, **kwargs)
-
-        if show_way_points:
-
-            px_list = [p[0, 0] for p in self.way_points]
-            py_list = [p[1, 0] for p in self.way_points]
-            
-            if self.pdim[0] > 2:
-                wu_list = [cos(p[2, 0]) for p in self.way_points]
-                wy_list = [sin(p[2, 0]) for p in self.way_points]
-                self.ax.quiver(px_list, py_list, wu_list, wy_list, color='r', scale=20)
-
-            else:
-                self.ax.scatter(px_list, py_list, c='k')
-
-        if show_direction:
-            if self.way_points[0] > 2:
-                u_list = [cos(p[2, 0]) for p in curve]
-                y_list = [sin(p[2, 0]) for p in curve]
-                self.ax.quiver(path_x_list, path_y_list, u_list, y_list, color='k', scale=35, scale_units='height')
-
-            else:
-                print('No direction for 2D way points')
-
-    def generate_line(self, start_point, end_point, step_size):
-
-        single_curve = [start_point]
-        cur_len = 0
-        
-        diff = end_point - start_point
-        length = np.linalg.norm(diff)
-        direction = diff / length
-
-        while cur_len <= length:
-            cur_len += step_size
-            new_point = start_point + cur_len * direction
-            single_curve.append(new_point)
-            
-        single_curve.append(end_point)
-
-        return single_curve
-
-if __name__ == '__main__':
-
-    point_list = []
-
-    cg = curve_generator(select_mode='mouse', )
-    curve = cg.generate_curve('dubins', point_list, 0.1, 2, include_gear=False)
-
-    if curve is not None:
-        cg.plot_curve(curve, show_direction=False)
-
+from tkinter import Scale
+import numpy as np
+from gctl.curve.dubins_path import generate_dubins_path
+from gctl.curve.reeds_shepp import generate_reeds_shepp
+import matplotlib.pyplot as plt
+from math import cos, sin, atan2
+
+class curve_generator:
+    def __init__(self, select_mode='default', point_style='pose', x_limit = [0, 10], y_limit=[0, 10]) -> None:
+        """
+        # select_mode: mode of point selection
+            # 'default', use the input point_list
+            # 'mouse', use mouse to select points or vectors
+                -- left click to select points and vectors
+                -- key enter to generate the curve
+        
+        # point_style
+            # position: x,y 2 * 1 matrix
+            # pose: x, y, theta, 3*1 matrix, include orientation
+        """
+        self.select_mode = select_mode
+        self.point_style = point_style
+        
+        self.x_limit = x_limit
+        self.y_limit = y_limit
+
+        if select_mode =='mouse':
+            self.fig, self.ax = plt.subplots()
+            self.ax.set_aspect('equal')
+            self.ax.set_xlim(x_limit)
+            self.ax.set_ylim(y_limit)
+
+        self.cpl = [] # click point list
+
+    def generate_curve(self, curve_style='dubins', way_points=[], step_size = 0.1, min_radius=1, include_gear=False, **kwargs):
+        
+        # way_points: The list of way points
+        # step_size: distance between the sample points
+
+        # min_radius: minimum turning radius for ackermann robot
+        # curve: a list of points
+
+        # curve_style: 
+            # - line: connect the points with line
+            # - reeds: connect the points with reeds shepp path
+            # - dubins: connect the points with dubins path
+        
+        # include_gear: if True, the curve should include the gear flag (-1, 1) and the points should be the 4*1 matrix. Used for reeds shepp
+
+        self.way_points = way_points
+        self.pnum = len(self.way_points)
+
+        if len(way_points) != 0: 
+            self.pdim = self.way_points[0].shape
+        elif self.point_style == 'position':
+            self.pdim = (2, 1)
+        elif self.point_style == 'pose':
+            self.pdim = (3, 1)
+
+        if self.select_mode == 'default':
+
+            if len(way_points) == 0:
+                print('Error: No waypoints !')
+                return None
+
+            curve = self.curve_from_waypoints(curve_style, min_radius, step_size, include_gear, **kwargs)
+
+        elif self.select_mode == 'mouse':
+            # generate reference path by mouse    
+            print('Left-slick to select the way point, Enter to generate the curve')
+
+            def on_press(event):
+                if event.key == 'enter':
+                    
+                    print('press enter, generate curves')
+
+                    if self.point_style == 'position':
+                        self.way_points = self.cpl
+                        self.pnum = len(self.way_points)
+
+                    elif self.point_style == 'pose':
+                        curve = self.curve_from_waypoints(curve_style, min_radius, step_size, include_gear, **kwargs)
+                        self.plot_curve(curve, show_way_points=False)
+                        plt.pause(0.001)
+                
+                if event.key == 'escape':
+                    plt.close()
+
+            self.fig.canvas.mpl_connect('button_press_event', self.onclick)
+            self.fig.canvas.mpl_connect('key_press_event', on_press)
+            plt.show()
+        
+        curve = self.curve_from_waypoints(curve_style, min_radius, step_size, include_gear, **kwargs)
+
+        return curve
+
+    def curve_from_waypoints(self, curve_style, min_radius, step_size, include_gear, **kwargs):
+        
+        curve = [ self.way_points[0] ]
+
+        if curve_style == 'dubins':
+            # generate dubins curve
+            for i in range(self.pnum - 1):
+                start_point = self.way_points[i]
+                end_point = self.way_points[i+1]
+                single_curve = generate_dubins_path(start_point, end_point, min_radius, step_size)
+                curve = curve + single_curve[1:]
+
+        elif curve_style == 'reeds':
+            # generate reeds shepp curve
+            for i in range(self.pnum - 1):
+                start_point = self.way_points[i]
+                end_point = self.way_points[i+1]
+                single_curve = generate_reeds_shepp(start_point, end_point, min_radius, step_size, include_gear, **kwargs)
+                curve = curve + single_curve[1:] 
+
+            if include_gear and self.pdim[0] == 3:
+                curve[0] = np.vstack((curve[0], [curve[1][-1, 0]]))
+
+        elif curve_style == 'line':
+            
+            for i in range(self.pnum - 1):
+                start_point = self.way_points[i]
+                end_point = self.way_points[i+1]
+                single_curve = self.generate_line(start_point, end_point, step_size)
+                curve = curve + single_curve[1:]
+
+        else:
+            print('wrong curve type')
+
+        return curve
+
+    def onclick(self, event):
+        print('%s click: button=%d, x=%d, y=%d, xdata=%f, ydata=%f' %
+            ('double' if event.dblclick else 'single', event.button,
+            event.x, event.y, event.xdata, event.ydata))
+
+        if self.point_style == 'position':
+            self.cpl.append(np.array([ [event.xdata], [event.ydata] ]))
+            self.ax.scatter(event.xdata, event.ydata, c='k')
+            plt.pause(0.001)
+        
+        elif self.point_style == 'pose':
+            self.cpl.append(np.array([ [event.xdata], [event.ydata] ]))
+            
+            if len(self.cpl) == 1:
+                self.ax.scatter(event.xdata, event.ydata, c='k')
+
+            if len(self.cpl) == 2:
+                diff = self.cpl[1] - self.cpl[0]
+                theta = atan2(diff[1, 0], diff[0, 0])
+                
+                self.ax.quiver(self.cpl[0][0, 0], self.cpl[0][1, 0], diff[0, 0], diff[1, 0], color='r', scale=20)
+
+                way_point = np.vstack((self.cpl[0], [theta]))
+                self.way_points.append(way_point)
+                self.pnum = len(self.way_points)
+
+                self.cpl = []
+
+            plt.pause(0.001)
+
+
+    def plot_curve(self, curve, style='-g', show_way_points=True, show_direction=False, **kwargs):
+
+        # self.ax.set_xlim(range_x)
+        # self.ax.set_ylim(range_y)
+
+        if self.select_mode =='default':
+            self.fig, self.ax = plt.subplots()
+            self.ax.set_aspect('equal')
+            self.ax.set_xlim(self.x_limit)
+            self.ax.set_ylim(self.y_limit) 
+
+        path_x_list = [p[0, 0] for p in curve]
+        path_y_list = [p[1, 0] for p in curve]
+
+        self.ax.plot(path_x_list, path_y_list, style, **kwargs)
+
+        if show_way_points:
+
+            px_list = [p[0, 0] for p in self.way_points]
+            py_list = [p[1, 0] for p in self.way_points]
+            
+            if self.pdim[0] > 2:
+                wu_list = [cos(p[2, 0]) for p in self.way_points]
+                wy_list = [sin(p[2, 0]) for p in self.way_points]
+                self.ax.quiver(px_list, py_list, wu_list, wy_list, color='r', scale=20)
+
+            else:
+                self.ax.scatter(px_list, py_list, c='k')
+
+        if show_direction:
+            if self.way_points[0] > 2:
+                u_list = [cos(p[2, 0]) for p in curve]
+                y_list = [sin(p[2, 0]) for p in curve]
+                self.ax.quiver(path_x_list, path_y_list, u_list, y_list, color='k', scale=35, scale_units='height')
+
+            else:
+                print('No direction for 2D way points')
+
+    def generate_line(self, start_point, end_point, step_size):
+
+        single_curve = [start_point]
+        cur_len = 0
+        
+        diff = end_point - start_point
+        length = np.linalg.norm(diff)
+        direction = diff / length
+
+        while cur_len <= length:
+            cur_len += step_size
+            new_point = start_point + cur_len * direction
+            single_curve.append(new_point)
+            
+        single_curve.append(end_point)
+
+        return single_curve
+
+if __name__ == '__main__':
+
+    point_list = []
+
+    cg = curve_generator(select_mode='mouse', )
+    curve = cg.generate_curve('dubins', point_list, 0.1, 2, include_gear=False)
+
+    if curve is not None:
+        cg.plot_curve(curve, show_direction=False)
+
     plt.show()
```

### Comparing `gctl-1.0/gctl.egg-info/PKG-INFO` & `gctl-1.1/gctl.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-Metadata-Version: 2.1
-Name: gctl
-Version: 1.0
-Summary: Generate curve tool
-Author-email: Han Ruihua <hanrh@connect.hku.hk>
-Project-URL: Homepage, https://github.com/hanruihua/GenerateCurveTool
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: scipy
-
-# GenerateCurveTool
-
-A tool of generating the common curves from way points for the robot path planning, including dubins path, reeds shepp, etc.
-
-
-Dubins path  |   Reeds Shepp    |
-:-------------------------:|:-------------------------:|
-![](example/gif/dubins.gif)  | ![](example/gif/reeds_shepp.gif) 
-
-## Prerequisite
-
-- Python: >= 3.8
-    - numpy  
-    - matplotlib 
-
-## Installation
-
-```
-git clone https://github.com/hanruihua/GenerateCurveTool  
-cd GenerateCurveTool  
-pip install -e . 
-```
-
-## Usage 
-
-The examples are in [GenerateCurveTool/example/](https://github.com/hanruihua/GenerateCurveTool/tree/main/example)
-
-## Roadmap
-
-- [x] Direct line
-- [x] Dubins path
-- [x] Reeds shepp
-- [ ] bezier 
-
-## Author
-
-Han Ruihua  
-Contact: hanrh@connect.hku.hk
-
+Metadata-Version: 2.1
+Name: gctl
+Version: 1.1
+Summary: Generate curve tool
+Author-email: Han Ruihua <hanrh@connect.hku.hk>
+Project-URL: Homepage, https://github.com/hanruihua/GenerateCurveTool
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scipy
+
+# GenerateCurveTool
+
+A tool of generating the common curves from way points for the robot path planning, including dubins path, reeds shepp, etc.
+
+
+Dubins path  |   Reeds Shepp    |
+:-------------------------:|:-------------------------:|
+![](example/gif/dubins.gif)  | ![](example/gif/reeds_shepp.gif) 
+
+## Prerequisite
+
+- Python: >= 3.8
+    - numpy  
+    - matplotlib 
+
+## Installation
+
+```
+git clone https://github.com/hanruihua/GenerateCurveTool  
+cd GenerateCurveTool  
+pip install -e . 
+```
+
+## Usage 
+
+The examples are in [GenerateCurveTool/example/](https://github.com/hanruihua/GenerateCurveTool/tree/main/example)
+
+## Roadmap
+
+- [x] Direct line
+- [x] Dubins path
+- [x] Reeds shepp
+- [ ] bezier 
+
+## Author
+
+Han Ruihua  
+Contact: hanrh@connect.hku.hk
+
```

### Comparing `gctl-1.0/pyproject.toml` & `gctl-1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-
-[project]
-name = "gctl"
-version = "1.0"
-authors = [
-  { name="Han Ruihua", email="hanrh@connect.hku.hk" },
-]
-description = "Generate curve tool"
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-
-dependencies = ['matplotlib',
-                'numpy',
-                'scipy',]
-
-[project.urls]
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+
+[project]
+name = "gctl"
+version = "1.1"
+authors = [
+  { name="Han Ruihua", email="hanrh@connect.hku.hk" },
+]
+description = "Generate curve tool"
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+
+dependencies = ['matplotlib',
+                'numpy',
+                'scipy',]
+
+[project.urls]
 Homepage = "https://github.com/hanruihua/GenerateCurveTool"
```


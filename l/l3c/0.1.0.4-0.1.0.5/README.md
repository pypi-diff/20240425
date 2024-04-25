# Comparing `tmp/l3c-0.1.0.4.tar.gz` & `tmp/l3c-0.1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "l3c-0.1.0.4.tar", last modified: Tue Apr 23 11:01:36 2024, max compression
+gzip compressed data, was "dist/l3c-0.1.0.5.tar", last modified: Thu Apr 25 08:00:52 2024, max compression
```

## Comparing `l3c-0.1.0.4.tar` & `l3c-0.1.0.5.tar`

### file list

```diff
@@ -1,49 +1,48 @@
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-23 11:01:36.618887 l3c-0.1.0.4/
--rw-r--r--   0 wangfan04   (502) staff       (20)    11357 2023-02-23 10:00:57.000000 l3c-0.1.0.4/LICENSE
--rw-r--r--   0 wangfan04   (502) staff       (20)     1015 2024-04-23 11:01:36.618707 l3c-0.1.0.4/PKG-INFO
--rw-r--r--   0 wangfan04   (502) staff       (20)      682 2024-04-23 08:58:47.000000 l3c-0.1.0.4/README.md
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-23 11:01:36.600198 l3c-0.1.0.4/l3c/
--rw-r--r--   0 wangfan04   (502) staff       (20)      762 2023-02-23 10:11:06.000000 l3c-0.1.0.4/l3c/__init__.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-23 11:01:36.604689 l3c-0.1.0.4/l3c/bandits/
--rw-r--r--   0 wangfan04   (502) staff       (20)      838 2023-02-23 10:11:06.000000 l3c-0.1.0.4/l3c/bandits/__init__.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     2717 2023-02-23 10:11:06.000000 l3c-0.1.0.4/l3c/bandits/bandits_env.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     1022 2023-02-23 10:32:50.000000 l3c-0.1.0.4/l3c/bandits/demo_thompson_sampling.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-23 11:01:36.605259 l3c-0.1.0.4/l3c/mazeworld/
--rw-r--r--   0 wangfan04   (502) staff       (20)     1714 2024-02-20 08:03:46.000000 l3c-0.1.0.4/l3c/mazeworld/__init__.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-23 11:01:36.607906 l3c-0.1.0.4/l3c/mazeworld/agents/
--rw-r--r--   0 wangfan04   (502) staff       (20)       45 2024-02-22 03:03:45.000000 l3c-0.1.0.4/l3c/mazeworld/agents/__init__.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     2857 2024-02-22 12:10:38.000000 l3c-0.1.0.4/l3c/mazeworld/agents/agent_base.py
--rw-r--r--   0 wangfan04   (502) staff       (20)    11413 2024-04-16 01:44:52.000000 l3c-0.1.0.4/l3c/mazeworld/agents/smart_slam_agent.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-23 11:01:36.609930 l3c-0.1.0.4/l3c/mazeworld/demo/
--rw-r--r--   0 wangfan04   (502) staff       (20)        0 2024-02-22 12:15:15.000000 l3c-0.1.0.4/l3c/mazeworld/demo/__init__.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     3609 2024-04-15 03:45:14.000000 l3c-0.1.0.4/l3c/mazeworld/demo/agent_play_demo.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     3844 2024-02-26 06:25:37.000000 l3c-0.1.0.4/l3c/mazeworld/demo/dump_maze.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     3366 2024-02-22 14:53:11.000000 l3c-0.1.0.4/l3c/mazeworld/demo/keyboard_play_demo.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-23 11:01:36.614675 l3c-0.1.0.4/l3c/mazeworld/envs/
--rw-r--r--   0 wangfan04   (502) staff       (20)      258 2024-02-04 12:16:02.000000 l3c-0.1.0.4/l3c/mazeworld/envs/__init__.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     3644 2023-02-23 10:11:06.000000 l3c-0.1.0.4/l3c/mazeworld/envs/dynamics.py
--rw-r--r--   0 wangfan04   (502) staff       (20)    14954 2024-04-23 08:19:34.000000 l3c-0.1.0.4/l3c/mazeworld/envs/maze_base.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     6324 2024-04-16 02:20:31.000000 l3c-0.1.0.4/l3c/mazeworld/envs/maze_continuous_3d.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     3345 2024-02-22 06:12:11.000000 l3c-0.1.0.4/l3c/mazeworld/envs/maze_discrete_2d.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     6849 2024-04-16 02:13:20.000000 l3c-0.1.0.4/l3c/mazeworld/envs/maze_discrete_3d.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     7295 2024-04-16 02:07:18.000000 l3c-0.1.0.4/l3c/mazeworld/envs/maze_env.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     9184 2024-02-20 01:19:41.000000 l3c-0.1.0.4/l3c/mazeworld/envs/maze_task.py
--rw-r--r--   0 wangfan04   (502) staff       (20)    12366 2024-04-16 02:19:02.000000 l3c-0.1.0.4/l3c/mazeworld/envs/ray_caster_utils.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-23 11:01:36.616062 l3c-0.1.0.4/l3c/mazeworld/tests/
--rw-r--r--   0 wangfan04   (502) staff       (20)        0 2024-02-22 12:15:23.000000 l3c-0.1.0.4/l3c/mazeworld/tests/__init__.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     2068 2024-02-04 15:06:43.000000 l3c-0.1.0.4/l3c/mazeworld/tests/test.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     2390 2024-02-22 11:56:16.000000 l3c-0.1.0.4/l3c/mazeworld/tests/test_agent.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-23 11:01:36.618074 l3c-0.1.0.4/l3c/metalang/
--rw-r--r--   0 wangfan04   (502) staff       (20)     1112 2024-04-23 10:49:18.000000 l3c-0.1.0.4/l3c/metalang/__init__.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     2666 2024-04-23 10:53:14.000000 l3c-0.1.0.4/l3c/metalang/generator.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     4420 2024-04-23 10:51:20.000000 l3c-0.1.0.4/l3c/metalang/metalangv1.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     5496 2024-04-23 10:52:10.000000 l3c-0.1.0.4/l3c/metalang/metalangv2.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-23 11:01:36.602917 l3c-0.1.0.4/l3c.egg-info/
--rw-r--r--   0 wangfan04   (502) staff       (20)     1015 2024-04-23 11:01:36.000000 l3c-0.1.0.4/l3c.egg-info/PKG-INFO
--rw-r--r--   0 wangfan04   (502) staff       (20)     1082 2024-04-23 11:01:36.000000 l3c-0.1.0.4/l3c.egg-info/SOURCES.txt
--rw-r--r--   0 wangfan04   (502) staff       (20)        1 2024-04-23 11:01:36.000000 l3c-0.1.0.4/l3c.egg-info/dependency_links.txt
--rw-r--r--   0 wangfan04   (502) staff       (20)        1 2023-04-19 12:54:38.000000 l3c-0.1.0.4/l3c.egg-info/not-zip-safe
--rw-r--r--   0 wangfan04   (502) staff       (20)       84 2024-04-23 11:01:36.000000 l3c-0.1.0.4/l3c.egg-info/requires.txt
--rw-r--r--   0 wangfan04   (502) staff       (20)        4 2024-04-23 11:01:36.000000 l3c-0.1.0.4/l3c.egg-info/top_level.txt
--rw-r--r--   0 wangfan04   (502) staff       (20)       38 2024-04-23 11:01:36.618944 l3c-0.1.0.4/setup.cfg
--rwxr-xr-x   0 wangfan04   (502) staff       (20)     1814 2024-04-23 11:01:20.000000 l3c-0.1.0.4/setup.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-25 08:00:52.000000 l3c-0.1.0.5/
+-rw-r--r--   0 wangfan04   (502) staff       (20)     1108 2024-04-25 08:00:52.000000 l3c-0.1.0.5/PKG-INFO
+-rw-r--r--   0 wangfan04   (502) staff       (20)    11357 2023-02-23 10:00:57.000000 l3c-0.1.0.5/LICENSE
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-25 08:00:51.000000 l3c-0.1.0.5/l3c/
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-25 08:00:51.000000 l3c-0.1.0.5/l3c/bandits/
+-rw-r--r--   0 wangfan04   (502) staff       (20)     1022 2023-02-23 10:32:50.000000 l3c-0.1.0.5/l3c/bandits/demo_thompson_sampling.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)      838 2023-02-23 10:11:06.000000 l3c-0.1.0.5/l3c/bandits/__init__.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     2717 2023-02-23 10:11:06.000000 l3c-0.1.0.5/l3c/bandits/bandits_env.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)      762 2023-02-23 10:11:06.000000 l3c-0.1.0.5/l3c/__init__.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-25 08:00:51.000000 l3c-0.1.0.5/l3c/mazeworld/
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-25 08:00:51.000000 l3c-0.1.0.5/l3c/mazeworld/demo/
+-rw-r--r--   0 wangfan04   (502) staff       (20)     3366 2024-02-22 14:53:11.000000 l3c-0.1.0.5/l3c/mazeworld/demo/keyboard_play_demo.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)        0 2024-02-22 12:15:15.000000 l3c-0.1.0.5/l3c/mazeworld/demo/__init__.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     3877 2024-04-25 07:54:35.000000 l3c-0.1.0.5/l3c/mazeworld/demo/agent_play_demo.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-25 08:00:52.000000 l3c-0.1.0.5/l3c/mazeworld/tests/
+-rw-r--r--   0 wangfan04   (502) staff       (20)     2414 2024-04-25 07:55:18.000000 l3c-0.1.0.5/l3c/mazeworld/tests/test_agent.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)        0 2024-02-22 12:15:23.000000 l3c-0.1.0.5/l3c/mazeworld/tests/__init__.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     2068 2024-02-04 15:06:43.000000 l3c-0.1.0.5/l3c/mazeworld/tests/test.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     1714 2024-02-20 08:03:46.000000 l3c-0.1.0.5/l3c/mazeworld/__init__.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-25 08:00:51.000000 l3c-0.1.0.5/l3c/mazeworld/agents/
+-rw-r--r--   0 wangfan04   (502) staff       (20)     3931 2024-04-25 07:54:08.000000 l3c-0.1.0.5/l3c/mazeworld/agents/agent_base.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)       45 2024-02-22 03:03:45.000000 l3c-0.1.0.5/l3c/mazeworld/agents/__init__.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)    11869 2024-04-25 07:30:00.000000 l3c-0.1.0.5/l3c/mazeworld/agents/smart_slam_agent.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-25 08:00:52.000000 l3c-0.1.0.5/l3c/mazeworld/envs/
+-rw-r--r--   0 wangfan04   (502) staff       (20)     7295 2024-04-16 02:07:18.000000 l3c-0.1.0.5/l3c/mazeworld/envs/maze_env.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     3428 2024-04-25 07:44:06.000000 l3c-0.1.0.5/l3c/mazeworld/envs/maze_discrete_2d.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     6781 2024-04-25 06:47:52.000000 l3c-0.1.0.5/l3c/mazeworld/envs/maze_discrete_3d.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)    14954 2024-04-23 08:19:34.000000 l3c-0.1.0.5/l3c/mazeworld/envs/maze_base.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)      258 2024-02-04 12:16:02.000000 l3c-0.1.0.5/l3c/mazeworld/envs/__init__.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     9184 2024-02-20 01:19:41.000000 l3c-0.1.0.5/l3c/mazeworld/envs/maze_task.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     6256 2024-04-25 06:48:19.000000 l3c-0.1.0.5/l3c/mazeworld/envs/maze_continuous_3d.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)    12366 2024-04-16 02:19:02.000000 l3c-0.1.0.5/l3c/mazeworld/envs/ray_caster_utils.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     3644 2023-02-23 10:11:06.000000 l3c-0.1.0.5/l3c/mazeworld/envs/dynamics.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-25 08:00:52.000000 l3c-0.1.0.5/l3c/metalang/
+-rw-r--r--   0 wangfan04   (502) staff       (20)     1112 2024-04-23 10:49:18.000000 l3c-0.1.0.5/l3c/metalang/__init__.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     5496 2024-04-23 10:52:10.000000 l3c-0.1.0.5/l3c/metalang/metalangv2.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     4420 2024-04-23 10:51:20.000000 l3c-0.1.0.5/l3c/metalang/metalangv1.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     2666 2024-04-23 10:53:14.000000 l3c-0.1.0.5/l3c/metalang/generator.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)      682 2024-04-23 08:58:47.000000 l3c-0.1.0.5/README.md
+-rwxr-xr-x   0 wangfan04   (502) staff       (20)     1814 2024-04-25 08:00:49.000000 l3c-0.1.0.5/setup.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-25 08:00:51.000000 l3c-0.1.0.5/l3c.egg-info/
+-rw-r--r--   0 wangfan04   (502) staff       (20)     1108 2024-04-25 08:00:51.000000 l3c-0.1.0.5/l3c.egg-info/PKG-INFO
+-rw-r--r--   0 wangfan04   (502) staff       (20)        1 2023-04-19 12:54:38.000000 l3c-0.1.0.5/l3c.egg-info/not-zip-safe
+-rw-r--r--   0 wangfan04   (502) staff       (20)     1050 2024-04-25 08:00:51.000000 l3c-0.1.0.5/l3c.egg-info/SOURCES.txt
+-rw-r--r--   0 wangfan04   (502) staff       (20)       84 2024-04-25 08:00:51.000000 l3c-0.1.0.5/l3c.egg-info/requires.txt
+-rw-r--r--   0 wangfan04   (502) staff       (20)        4 2024-04-25 08:00:51.000000 l3c-0.1.0.5/l3c.egg-info/top_level.txt
+-rw-r--r--   0 wangfan04   (502) staff       (20)        1 2024-04-25 08:00:51.000000 l3c-0.1.0.5/l3c.egg-info/dependency_links.txt
+-rw-r--r--   0 wangfan04   (502) staff       (20)       38 2024-04-25 08:00:52.000000 l3c-0.1.0.5/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `l3c-0.1.0.4/LICENSE` & `l3c-0.1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.4/PKG-INFO` & `l3c-0.1.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: l3c
-Version: 0.1.0.4
+Version: 0.1.0.5
 Summary: L3C provide abundant environments for Lifelong Learning (L3) in Context.
 Home-page: https://github.com/FutureAGI/L3C
 Author: WorldEditors
 Author-email: 
 License: Apache
+Description: # L3C - Life Long Learning In Context
+        
+        L3C provide abundant environments for Lifelong Learning (L3) in Context, with long-term dependencies on the Contexts for task generalization.
+        
+        In-Context Learning entails a different learning process than that of gradient descent, as it involves feeding data through prompts instead. Our objective is to enhance lifelong learning research by utilizing prompts, which involve agents that learn through interaction in a forward-only manner.
+        
+        # Environments Updating
+        
+        - [MazeWorlds](l3c/mazeworld): 2D/3D maze generators for task generalization
+        
+        - [RPL](l3c/rpl): Randomized Pseudo-Language
+        
+        - [Bandits](l3c/bandits): Bandits task generalization
+        
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# L3C - Life Long Learning In Context
-
-L3C provide abundant environments for Lifelong Learning (L3) in Context, with long-term dependencies on the Contexts for task generalization.
-
-In-Context Learning entails a different learning process than that of gradient descent, as it involves feeding data through prompts instead. Our objective is to enhance lifelong learning research by utilizing prompts, which involve agents that learn through interaction in a forward-only manner.
-
-# Environments Updating
-
-- [MazeWorlds](l3c/mazeworld): 2D/3D maze generators for task generalization
-
-- [RPL](l3c/rpl): Randomized Pseudo-Language
-
-- [Bandits](l3c/bandits): Bandits task generalization
-
-
```

### Comparing `l3c-0.1.0.4/README.md` & `l3c-0.1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.4/l3c/__init__.py` & `l3c-0.1.0.5/l3c/__init__.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.4/l3c/bandits/__init__.py` & `l3c-0.1.0.5/l3c/bandits/__init__.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.4/l3c/bandits/bandits_env.py` & `l3c-0.1.0.5/l3c/bandits/bandits_env.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.4/l3c/bandits/demo_thompson_sampling.py` & `l3c-0.1.0.5/l3c/bandits/demo_thompson_sampling.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.4/l3c/mazeworld/__init__.py` & `l3c-0.1.0.5/l3c/mazeworld/__init__.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.4/l3c/mazeworld/agents/smart_slam_agent.py` & `l3c-0.1.0.5/l3c/mazeworld/agents/smart_slam_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 import pygame
 from .agent_base import AgentBase
 from queue import Queue
 from pygame import font
 from l3c.mazeworld.envs.dynamics import PI
 from l3c.mazeworld.envs.ray_caster_utils import landmarks_color, landmarks_rgb, landmarks_rgb_arr, paint_agent_arrow
 
+def aggregate_unexplorations(mask_info):
+    ret_mask = mask_info.astype(numpy.int32)
+    nx, ny = mask_info.shape
+    for dx,dy in [(1, 1), (1, 0), (0, 1), (1, 2), (2, 1), (2, 2), (0, 2), (2, 0)]:
+        ret_mask[dx:,dy:] = ret_mask[dx:,dy:] + mask_info[:nx-dx, :ny-dy]
+        ret_mask[:nx-dx, :ny-dy] = ret_mask[:nx-dx, :ny-dy] + mask_info[dx:, dy:]
+    return ret_mask * mask_info
+
 class SmartSLAMAgent(AgentBase):
     def render_init(self, view_size=(640, 640)):
         """
         Initialize a God View With Landmarks
         """
         font.init()
         self._font = font.SysFont("Arial", 18)
@@ -236,16 +244,18 @@
                     min_cost = cost_map[n_x, n_y]
                     sel_x = n_x
                     sel_y = n_y
                     path.insert(0, (n_x, n_y))
             cost=cost_map[sel_x, sel_y]
         return path
 
+
     def exploration(self):
-        utility = self._cost_map + 10000 * self._mask_info
+        aggr = aggregate_unexplorations(self._mask_info)
+        utility = self._cost_map + 10000 * self._mask_info - 3 * aggr
         if(numpy.argmin(utility) >= 10000):
             return None 
         target_idx = numpy.unravel_index(numpy.argmin(utility), utility.shape)
         return self.retrieve_path(self._cost_map, target_idx)
 
     def navigate_landmarks_navigate(self, landmarks_id):
         idxes = numpy.argwhere(self._god_info == landmarks_id + 1)
```

### Comparing `l3c-0.1.0.4/l3c/mazeworld/demo/agent_play_demo.py` & `l3c-0.1.0.5/l3c/mazeworld/demo/agent_play_demo.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     parser.add_argument('--wall_height', type=float, default=3.2, help="Only valid in 3D mode")
     parser.add_argument('--cell_size', type=float, default=2.0, help="Only valid in 3D mode")
     parser.add_argument('--step_reward', type=float, default=-0.01, help="Default rewards per-step")
     parser.add_argument('--n_landmarks', type=int, default=5, help="Number of landmarks, valid for both SURVIVAL and NAVIGATION task")
     parser.add_argument('--r_landmarks', type=float, default=0.50, help="Average rewards of the landmarks, only valid in SURVIVAL task")
     parser.add_argument('--cd_landmarks', type=int, default=200, help="Refresh interval of landmarks")
     parser.add_argument('--save_replay', type=str, default=None, help="Save the replay trajectory in file")
+    parser.add_argument('--memory_keep_ratio', type=float, default=1.0, 
+                        help="Keep ratio of memory when the agent switch from short to long term memory. 1.0 means perfect memory, 0.0 means no memory")
     parser.add_argument('--verbose', type=bool, default=False)
 
     args = parser.parse_args()
 
     if(args.maze_type == "Discrete2D"):
         maze_env = gym.make("mazeworld-discrete-2D-v1", enable_render=False, max_steps=args.max_steps, visibility_2D=args.visibility_2D, task_type=args.task_type)
     elif(args.maze_type == "Discrete3D"):
@@ -42,15 +44,15 @@
             step_reward=args.step_reward,
             landmarks_number=args.n_landmarks,
             landmarks_refresh_interval=args.cd_landmarks,
             landmarks_avg_reward=args.r_landmarks,
             verbose=True)
     maze_env.set_task(task)
 
-    agent = SmartSLAMAgent(maze_env=maze_env, render=True)
+    agent = SmartSLAMAgent(maze_env=maze_env, memory_keep_ratio=args.memory_keep_ratio, render=True)
 
     observation = maze_env.reset()
     done=False
     sum_reward = 0
     reward = 0
 
     while not done:
```

### Comparing `l3c-0.1.0.4/l3c/mazeworld/demo/keyboard_play_demo.py` & `l3c-0.1.0.5/l3c/mazeworld/demo/keyboard_play_demo.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.4/l3c/mazeworld/envs/dynamics.py` & `l3c-0.1.0.5/l3c/mazeworld/envs/dynamics.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.4/l3c/mazeworld/envs/maze_base.py` & `l3c-0.1.0.5/l3c/mazeworld/envs/maze_base.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.4/l3c/mazeworld/envs/maze_continuous_3d.py` & `l3c-0.1.0.5/l3c/mazeworld/envs/maze_continuous_3d.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,34 +98,33 @@
         if keys[pygame.K_SPACE]:
             turn_rate = 0.0
             walk_speed = 0.0
         return turn_rate, walk_speed
 
     def update_observation(self):
         if(self.task_type == "SURVIVAL"):
-            self._observation, cell_exposed = maze_view(numpy.array(self._agent_loc, dtype=numpy.float32), self._agent_ori, self._agent_height, 
+            self._observation, self._cell_exposed = maze_view(numpy.array(self._agent_loc, dtype=numpy.float32), self._agent_ori, self._agent_height, 
                     self._cell_walls, self._cell_active_landmarks, self._cell_texts, self._cell_size, MAZE_TASK_MANAGER.grounds,
                     MAZE_TASK_MANAGER.ceil, self._wall_height, 1.0, self.visibility_3D, 0.20, 
                     self.fol_angle, self.resolution_horizon, self.resolution_vertical, landmarks_rgb_arr)
             lifebar_l = self._life / self._max_life * self._lifebar_l
             start_x = int(self._lifebar_start_x)
             start_y = int(self._lifebar_start_y)
             end_x = int(self._lifebar_start_x + lifebar_l)
             end_y = int(self._lifebar_start_y + self._lifebar_w)
             self._observation[start_x:end_x, start_y:end_y, 0] = 255
             self._observation[start_x:end_x, start_y:end_y, 1] = 0
             self._observation[start_x:end_x, start_y:end_y, 2] = 0
         elif(self.task_type == "NAVIGATION"):
-            self._observation, cell_exposed = maze_view(numpy.array(self._agent_loc, dtype=numpy.float32), self._agent_ori, self._agent_height, 
+            self._observation, self._cell_exposed = maze_view(numpy.array(self._agent_loc, dtype=numpy.float32), self._agent_ori, self._agent_height, 
                     self._cell_walls, self._cell_landmarks, self._cell_texts, self._cell_size, MAZE_TASK_MANAGER.grounds,
                     MAZE_TASK_MANAGER.ceil, self._wall_height, 1.0, self.visibility_3D, 0.20, 
                     self.fol_angle, self.resolution_horizon, self.resolution_vertical, landmarks_rgb_arr)
             start_x = int(self._navbar_start_x)
             start_y = int(self._navbar_start_y)
             end_x = int(self._navbar_start_x + self._navbar_l)
             end_y = int(self._navbar_start_y + self._navbar_w)
             self._observation[start_x:end_x, start_y:end_y] = landmarks_rgb[self._command]
         self._obs_surf = pygame.surfarray.make_surface(self._observation)
-        self._cell_exposed = numpy.logical_or(self._cell_exposed, cell_exposed)
 
     def get_observation(self):
         return numpy.copy(self._observation)
```

### Comparing `l3c-0.1.0.4/l3c/mazeworld/envs/maze_discrete_2d.py` & `l3c-0.1.0.5/l3c/mazeworld/envs/maze_discrete_2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,9 +72,10 @@
             # For survival task, the color of the center represents its life value
             f = max(0, int(255 - 128 * self._life))
             self._observation[self.visibility_2D, self.visibility_2D] = numpy.asarray([255, f, f], dtype="int32")
         elif(self.task_type == "NAVIGATION"):
             # For navigation task, the color of the center represents the navigation target
             self._observation[self.visibility_2D, self.visibility_2D] = landmarks_rgb[self._command]
 
+        self._cell_exposed = numpy.zeros_like(self._cell_walls).astype(numpy.bool)
         self._cell_exposed[(self._agent_grid[0] - self.visibility_2D) : (self._agent_grid[0] + self.visibility_2D + 1), \
                 (self._agent_grid[1] - self.visibility_2D) : (self._agent_grid[1] + self.visibility_2D + 1)] = True
```

### Comparing `l3c-0.1.0.4/l3c/mazeworld/envs/maze_discrete_3d.py` & `l3c-0.1.0.5/l3c/mazeworld/envs/maze_discrete_3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,34 +114,33 @@
             return (0, -1)
         if keys[pygame.K_SPACE]:
             return (0, 0)
         return None
 
     def update_observation(self):
         if(self.task_type == "SURVIVAL"):
-            self._observation, cell_exposed = maze_view(numpy.array(self._agent_loc, dtype=numpy.float32), self._agent_ori, self._agent_height, 
+            self._observation, self._cell_exposed = maze_view(numpy.array(self._agent_loc, dtype=numpy.float32), self._agent_ori, self._agent_height, 
                     self._cell_walls, self._cell_active_landmarks, self._cell_texts, self._cell_size, MAZE_TASK_MANAGER.grounds,
                     MAZE_TASK_MANAGER.ceil, self._wall_height, 1.0, self.visibility_3D, 0.20, 
                     self.fol_angle, self.resolution_horizon, self.resolution_vertical, landmarks_rgb_arr)
             lifebar_l = self._life / self._max_life * self._lifebar_l
             start_x = int(self._lifebar_start_x)
             start_y = int(self._lifebar_start_y)
             end_x = int(self._lifebar_start_x + lifebar_l)
             end_y = int(self._lifebar_start_y + self._lifebar_w)
             self._observation[start_x:end_x, start_y:end_y, 0] = 255
             self._observation[start_x:end_x, start_y:end_y, 1] = 0
             self._observation[start_x:end_x, start_y:end_y, 2] = 0
         elif(self.task_type == "NAVIGATION"):
-            self._observation, cell_exposed = maze_view(numpy.array(self._agent_loc, dtype=numpy.float32), self._agent_ori, self._agent_height, 
+            self._observation, self._cell_exposed = maze_view(numpy.array(self._agent_loc, dtype=numpy.float32), self._agent_ori, self._agent_height, 
                     self._cell_walls, self._cell_landmarks, self._cell_texts, self._cell_size, MAZE_TASK_MANAGER.grounds,
                     MAZE_TASK_MANAGER.ceil, self._wall_height, 1.0, self.visibility_3D, 0.20, 
                     self.fol_angle, self.resolution_horizon, self.resolution_vertical, landmarks_rgb_arr)
             start_x = int(self._navbar_start_x)
             start_y = int(self._navbar_start_y)
             end_x = int(self._navbar_start_x + self._navbar_l)
             end_y = int(self._navbar_start_y + self._navbar_w)
             self._observation[start_x:end_x, start_y:end_y] = landmarks_rgb[self._command]
         self._obs_surf = pygame.surfarray.make_surface(self._observation)
-        self._cell_exposed = numpy.logical_or(self._cell_exposed, cell_exposed)
 
     def get_observation(self):
         return numpy.copy(self._observation)
```

### Comparing `l3c-0.1.0.4/l3c/mazeworld/envs/maze_env.py` & `l3c-0.1.0.5/l3c/mazeworld/envs/maze_env.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.4/l3c/mazeworld/envs/maze_task.py` & `l3c-0.1.0.5/l3c/mazeworld/envs/maze_task.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.4/l3c/mazeworld/envs/ray_caster_utils.py` & `l3c-0.1.0.5/l3c/mazeworld/envs/ray_caster_utils.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.4/l3c/mazeworld/tests/test.py` & `l3c-0.1.0.5/l3c/mazeworld/tests/test.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.4/l3c/mazeworld/tests/test_agent.py` & `l3c-0.1.0.5/l3c/mazeworld/tests/test_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             landmarks_number=n_landmarks,
             landmarks_avg_reward=r_landmarks,
             verbose=False)
 
     maze_env.set_task(task)
 
     # Must intialize agent after reset
-    agent = SmartSLAMAgent(maze_env=maze_env, render=False)
+    agent = SmartSLAMAgent(maze_env=maze_env, memory_keep_ratio=0.25, render=False)
 
     done=False
     observation = maze_env.reset()
     sum_reward = 0
     reward = 0
     while not done:
         action = agent.step(observation, reward)
```

### Comparing `l3c-0.1.0.4/l3c/metalang/__init__.py` & `l3c-0.1.0.5/l3c/metalang/__init__.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.4/l3c/metalang/generator.py` & `l3c-0.1.0.5/l3c/metalang/generator.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.4/l3c/metalang/metalangv1.py` & `l3c-0.1.0.5/l3c/metalang/metalangv1.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.4/l3c/metalang/metalangv2.py` & `l3c-0.1.0.5/l3c/metalang/metalangv2.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.4/l3c.egg-info/PKG-INFO` & `l3c-0.1.0.5/l3c.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: l3c
-Version: 0.1.0.4
+Version: 0.1.0.5
 Summary: L3C provide abundant environments for Lifelong Learning (L3) in Context.
 Home-page: https://github.com/FutureAGI/L3C
 Author: WorldEditors
 Author-email: 
 License: Apache
+Description: # L3C - Life Long Learning In Context
+        
+        L3C provide abundant environments for Lifelong Learning (L3) in Context, with long-term dependencies on the Contexts for task generalization.
+        
+        In-Context Learning entails a different learning process than that of gradient descent, as it involves feeding data through prompts instead. Our objective is to enhance lifelong learning research by utilizing prompts, which involve agents that learn through interaction in a forward-only manner.
+        
+        # Environments Updating
+        
+        - [MazeWorlds](l3c/mazeworld): 2D/3D maze generators for task generalization
+        
+        - [RPL](l3c/rpl): Randomized Pseudo-Language
+        
+        - [Bandits](l3c/bandits): Bandits task generalization
+        
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# L3C - Life Long Learning In Context
-
-L3C provide abundant environments for Lifelong Learning (L3) in Context, with long-term dependencies on the Contexts for task generalization.
-
-In-Context Learning entails a different learning process than that of gradient descent, as it involves feeding data through prompts instead. Our objective is to enhance lifelong learning research by utilizing prompts, which involve agents that learn through interaction in a forward-only manner.
-
-# Environments Updating
-
-- [MazeWorlds](l3c/mazeworld): 2D/3D maze generators for task generalization
-
-- [RPL](l3c/rpl): Randomized Pseudo-Language
-
-- [Bandits](l3c/bandits): Bandits task generalization
-
-
```

### Comparing `l3c-0.1.0.4/l3c.egg-info/SOURCES.txt` & `l3c-0.1.0.5/l3c.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 l3c/bandits/demo_thompson_sampling.py
 l3c/mazeworld/__init__.py
 l3c/mazeworld/agents/__init__.py
 l3c/mazeworld/agents/agent_base.py
 l3c/mazeworld/agents/smart_slam_agent.py
 l3c/mazeworld/demo/__init__.py
 l3c/mazeworld/demo/agent_play_demo.py
-l3c/mazeworld/demo/dump_maze.py
 l3c/mazeworld/demo/keyboard_play_demo.py
 l3c/mazeworld/envs/__init__.py
 l3c/mazeworld/envs/dynamics.py
 l3c/mazeworld/envs/maze_base.py
 l3c/mazeworld/envs/maze_continuous_3d.py
 l3c/mazeworld/envs/maze_discrete_2d.py
 l3c/mazeworld/envs/maze_discrete_3d.py
```

### Comparing `l3c-0.1.0.4/setup.py` & `l3c-0.1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
 from setuptools import setup, find_packages
 
-__version__ = '0.1.0.4'
+__version__ = '0.1.0.5'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='l3c',
     version=__version__,
```


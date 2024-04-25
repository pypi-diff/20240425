# Comparing `tmp/dsse-1.0.2.tar.gz` & `tmp/dsse-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsse-1.0.2.tar", last modified: Thu Apr 18 19:39:32 2024, max compression
+gzip compressed data, was "dsse-1.0.3.tar", last modified: Thu Apr 25 20:11:00 2024, max compression
```

## Comparing `dsse-1.0.2.tar` & `dsse-1.0.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:39:32.920237 dsse-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:39:32.916237 dsse-1.0.2/DSSE/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:39:32.920237 dsse-1.0.2/DSSE/environment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/coverage_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:39:32.920237 dsse-1.0.2/DSSE/environment/entities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/entities/drone.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/entities/person.py
--rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/env_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:39:32.920237 dsse-1.0.2/DSSE/environment/imgs/
--rw-r--r--   0 runner    (1001) docker     (127)    14774 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/imgs/drone.png
--rw-r--r--   0 runner    (1001) docker     (127)    13193 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/imgs/person-swimming.png
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/pygame_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:39:32.920237 dsse-1.0.2/DSSE/environment/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/simulation/dynamic_probability.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/simulation/particle_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/environment/simulation/time_step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:39:32.920237 dsse-1.0.2/DSSE/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/tests/drone_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12802 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/tests/test_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/tests/test_env_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 19:39:25.000000 dsse-1.0.2/DSSE/tests/test_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:39:32.920237 dsse-1.0.2/DSSE.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15973 2024-04-18 19:39:32.000000 dsse-1.0.2/DSSE.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-18 19:39:32.000000 dsse-1.0.2/DSSE.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:39:32.000000 dsse-1.0.2/DSSE.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-18 19:39:32.000000 dsse-1.0.2/DSSE.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 19:39:32.000000 dsse-1.0.2/DSSE.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-18 19:39:25.000000 dsse-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 19:39:25.000000 dsse-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15973 2024-04-18 19:39:32.920237 dsse-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15170 2024-04-18 19:39:25.000000 dsse-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:39:32.920237 dsse-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-18 19:39:32.000000 dsse-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:11:00.980493 dsse-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:11:00.972493 dsse-1.0.3/DSSE/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:11:00.976493 dsse-1.0.3/DSSE/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/coverage_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:11:00.976493 dsse-1.0.3/DSSE/environment/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/entities/drone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/entities/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12983 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/env_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:11:00.976493 dsse-1.0.3/DSSE/environment/imgs/
+-rw-r--r--   0 runner    (1001) docker     (127)    14774 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/imgs/drone.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13193 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/imgs/person-swimming.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/pygame_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:11:00.976493 dsse-1.0.3/DSSE/environment/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/simulation/dynamic_probability.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/simulation/particle_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/simulation/time_step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:11:00.976493 dsse-1.0.3/DSSE/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/tests/drone_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12849 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/tests/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/tests/test_env_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/tests/test_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:11:00.976493 dsse-1.0.3/DSSE.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-04-25 20:11:00.000000 dsse-1.0.3/DSSE.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-25 20:11:00.000000 dsse-1.0.3/DSSE.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 20:11:00.000000 dsse-1.0.3/DSSE.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 20:11:00.000000 dsse-1.0.3/DSSE.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 20:11:00.000000 dsse-1.0.3/DSSE.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-25 20:10:46.000000 dsse-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 20:10:46.000000 dsse-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-04-25 20:11:00.980493 dsse-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-25 20:10:46.000000 dsse-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 20:11:00.980493 dsse-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-25 20:11:00.000000 dsse-1.0.3/setup.py
```

### Comparing `dsse-1.0.2/DSSE/environment/coverage_env.py` & `dsse-1.0.3/DSSE/environment/coverage_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 # TODO: Match env_base to conv_env -> If using particle sim, redo __init__ and reset.
 class CoverageDroneSwarmSearch(DroneSwarmSearchBase):
     metadata = {
         "name": "DroneSwarmSearchCPP",
     }
     reward_scheme = Reward(
         default=0,
-        leave_grid=-100,
+        leave_grid=-10,
         exceed_timestep=-100,
-        drones_collision=-100,
+        drones_collision=-10,
         search_cell=10,
         search_and_find=100,
     )
 
     def __init__(
         self,
         grid_size=20,
@@ -128,15 +128,15 @@
             if not self.is_valid_position(new_position):
                 rewards[agent] = self.reward_scheme.leave_grid
                 continue
 
             self.agents_positions[idx] = new_position
             new_x, new_y = new_position
             if new_position in self.not_seen_states:
-                reward_poc = 1 / (self.timestep) * prob_matrix[new_y, new_x] * 1_000
+                reward_poc = (1 / (self.timestep)) * prob_matrix[new_y, new_x] * 1_000
                 rewards[agent] = self.reward_scheme.search_cell + reward_poc
                 self.seen_states.add(new_position)
                 self.not_seen_states.remove(new_position)
                 # Probability of sucess (POS) = POC * POD
                 self.cumm_pos += prob_matrix[new_y, new_x] * self.drone.pod
             else:
                 self.repeated_coverage += 1
```

### Comparing `dsse-1.0.2/DSSE/environment/entities/drone.py` & `dsse-1.0.3/DSSE/environment/entities/drone.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.2/DSSE/environment/entities/person.py` & `dsse-1.0.3/DSSE/environment/entities/person.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.2/DSSE/environment/env.py` & `dsse-1.0.3/DSSE/environment/env.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 
     possible_actions = {action for action in Actions}
     metadata = {
         "name": "DroneSwarmSearchV0",
     }
 
     reward_scheme = Reward(
-        default=1,
-        leave_grid=-100_000,
-        exceed_timestep=-100_000,
-        drones_collision=-100_000,
+        default=0.1,
+        leave_grid=-200,
+        exceed_timestep=-200,
+        drones_collision=-200,
         search_cell=1,
-        search_and_find=100_000,
+        search_and_find=200,
     )
 
     def __init__(
         self,
         grid_size=20,
         render_mode="ansi",
         render_grid=False,
@@ -258,17 +258,15 @@
                     person_found = True
                     for agent in self.agents:
                         terminations[agent] = True
                         truncations[agent] = True
             elif is_searching:
                 prob_matrix = self.probability_matrix.get_matrix()
                 rewards[agent] = (
-                    prob_matrix[drone_y][drone_x] * 10000
-                    if prob_matrix[drone_y][drone_x] * 100 > 1
-                    else -100
+                    prob_matrix[drone_y][drone_x]
                 )
 
             self.rewards_sum[agent] += rewards[agent]
 
         self.timestep += 1
         # Get dummy infos
         infos = {drone: {"Found": person_found} for drone in self.agents}
```

### Comparing `dsse-1.0.2/DSSE/environment/env_base.py` & `dsse-1.0.3/DSSE/environment/env_base.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.2/DSSE/environment/imgs/drone.png` & `dsse-1.0.3/DSSE/environment/imgs/drone.png`

 * *Files identical despite different names*

### Comparing `dsse-1.0.2/DSSE/environment/imgs/person-swimming.png` & `dsse-1.0.3/DSSE/environment/imgs/person-swimming.png`

 * *Files identical despite different names*

### Comparing `dsse-1.0.2/DSSE/environment/pygame_interface.py` & `dsse-1.0.3/DSSE/environment/pygame_interface.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.2/DSSE/environment/simulation/dynamic_probability.py` & `dsse-1.0.3/DSSE/environment/simulation/dynamic_probability.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.2/DSSE/environment/simulation/particle_sim.py` & `dsse-1.0.3/DSSE/environment/simulation/particle_sim.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.2/DSSE/environment/simulation/time_step.py` & `dsse-1.0.3/DSSE/environment/simulation/time_step.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.2/DSSE/tests/drone_policy.py` & `dsse-1.0.3/DSSE/tests/drone_policy.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.2/DSSE/tests/test_env.py` & `dsse-1.0.3/DSSE/tests/test_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         grid_size=grid_size, person_initial_position=person_initial_position
     )
     opt = {"drones_positions": [(0, 0)]}
     _ = env.reset(options=opt)
 
     done = False
     reward_sum = 0
-    while not done and reward_sum >= -500_000:
+    while not done and reward_sum >= env.reward_scheme.leave_grid * (env.timestep_limit - 1):
         actions = {"drone0": Actions.UP.value}
         _, reward, terminations, done, _ = env.step(actions)
         done = any(done.values())
         reward_sum += sum(reward.values())
 
     assert (
         not done
```

### Comparing `dsse-1.0.2/DSSE/tests/test_env_coverage.py` & `dsse-1.0.3/DSSE/tests/test_env_coverage.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         grid_size=grid_size
     )
     opt = {"drones_positions": [(0, 0)]}
     _ = env.reset(options=opt)
 
     done = False
     reward_sum = 0
-    while not done and reward_sum >= -9_000:
+    while not done and reward_sum >=  (env.reward_scheme.leave_grid * (env.timestep_limit-1)) +1:
         actions = {"drone0": Actions.UP.value}
         _, reward, terminations, done, _ = env.step(actions)
         done = any(done.values())
         reward_sum += sum(reward.values())
 
     assert (
         not done
```

### Comparing `dsse-1.0.2/DSSE/tests/test_matrix.py` & `dsse-1.0.3/DSSE/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.2/DSSE.egg-info/SOURCES.txt` & `dsse-1.0.3/DSSE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dsse-1.0.2/LICENSE` & `dsse-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dsse-1.0.2/setup.py` & `dsse-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 
 download_url = (
-    f"https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.0.2.tar.gz"
+    f"https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.0.3.tar.gz"
 )
 setup(
     name="DSSE",
-    version="1.0.2",
+    version="1.0.3",
     author="Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta, Jorás Oliveira, Ricardo Ribeiro Rodrigues, Renato Laffranchi Falcão, Pedro Henrique Britto Aragão Andrade, Fabricio Barth",
     description="An environment to train drones to search and find a shipwrecked person lost in the ocean using reinforcement learning.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pfeinsper/drone-swarm-search",
     license="MIT",
     keywords=["Reinforcement Learning", "AI", "SAR", "Multi Agent"],
```


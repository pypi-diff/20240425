# Comparing `tmp/dune_rivals-0.5.9.tar.gz` & `tmp/dune_rivals-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.5.9.tar", last modified: Sun Apr 21 19:02:30 2024, max compression
+gzip compressed data, was "dune_rivals-0.6.0.tar", last modified: Wed Apr 24 22:21:11 2024, max compression
```

## Comparing `dune_rivals-0.5.9.tar` & `dune_rivals-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 19:02:30.484970 dune_rivals-0.5.9/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 19:02:30.484363 dune_rivals-0.5.9/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.5.9/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-21 19:02:30.483611 dune_rivals-0.5.9/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-21 19:02:30.000000 dune_rivals-0.5.9/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-21 19:02:30.000000 dune_rivals-0.5.9/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-21 19:02:30.000000 dune_rivals-0.5.9/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-21 19:02:30.000000 dune_rivals-0.5.9/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)    31165 2024-04-21 19:02:13.000000 dune_rivals-0.5.9/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-21 19:02:25.000000 dune_rivals-0.5.9/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-21 19:02:30.485070 dune_rivals-0.5.9/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-24 22:21:11.642087 dune_rivals-0.6.0/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-24 22:21:11.641519 dune_rivals-0.6.0/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.6.0/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-24 22:21:11.641094 dune_rivals-0.6.0/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-24 22:21:11.000000 dune_rivals-0.6.0/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-24 22:21:11.000000 dune_rivals-0.6.0/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-24 22:21:11.000000 dune_rivals-0.6.0/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-24 22:21:11.000000 dune_rivals-0.6.0/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    31788 2024-04-24 22:20:28.000000 dune_rivals-0.6.0/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-24 22:20:58.000000 dune_rivals-0.6.0/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-24 22:21:11.642220 dune_rivals-0.6.0/setup.cfg
```

### Comparing `dune_rivals-0.5.9/dune_rivals.py` & `dune_rivals-0.6.0/dune_rivals.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,19 +18,20 @@
 
 class BaseRivalActor:
     """
     DO NOT MODIFY
 
     Base class with common functionality shared across all Fedaykin and Rival Actors.
     """
-    def __init__(self, payload: str):
+    def __init__(self, payload: str, user: str):
         self.payload = payload
+        self.user = user
         self.i = np.random.randint(0, MAP_DIM - 1)
         self.j = np.random.randint(0, MAP_DIM - 1)
-        self.gamestate = ray.get_actor("GameState")
+        self.gamestate = ray.get_actor("GameState", namespace=user)
         self.spice_loc_map = None
         self.spice_file_map = None
         self.order_map = None
         self.name = None
 
     def _set_fields(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict) -> None:
         """
@@ -119,219 +120,219 @@
         time.sleep(total_dist * SLEEP_SECONDS_PER_TRAVEL_COORD)
 
         # update coordinates
         self.i = new_i
         self.j = new_j
 
 
-@ray.remote(num_cpus=0.1, resources={"worker3": 1e-4})
+@ray.remote
 class Noop12(BaseRivalActor):
-    def __init__(self, payload: str):
-        super().__init__(payload)
+    def __init__(self, payload: str, user: str):
+        super().__init__(payload, user)
         self.id = 12
         self.name = "Noop12"
 
     def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
         pass
 
-@ray.remote(num_cpus=0.1, resources={"worker4": 1e-4})
+@ray.remote
 class Noop34(BaseRivalActor):
-    def __init__(self, payload: str):
-        super().__init__(payload)
+    def __init__(self, payload: str, user: str):
+        super().__init__(payload, user)
         self.id = 34
         self.name = "Noop34"
 
     def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
         pass
 
 
 ##############################################################################################
 ################################         Silly Goose          ################################
 ##############################################################################################
 class BaseSillyGoose(BaseRivalActor):
-    def __init__(self, payload: str):
-        super().__init__(payload)
+    def __init__(self, payload: str, user: str):
+        super().__init__(payload, user)
 
     def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
         # set these state variables
         self.spice_loc_map = spice_loc_map
         self.spice_file_map = spice_file_map
         self.order_map = order_map
 
     def get_spice_loc_map(self):
         return self.spice_loc_map
 
 
-@ray.remote(num_cpus=0.8, name="SillyGoose1", resources={"worker3": 1e-4})
+@ray.remote
 class SillyGoose1(BaseSillyGoose):
     """
     SillyGoose1 is the leader. It picks which spice field to target and moves all
     other Geese to that target. Once the necessary Geese arrive, it instructs the
     Geese to destroy spice in the specified order.
     """
-    def __init__(self, payload: str):
-        super().__init__(payload)
+    def __init__(self, payload: str, user: str):
+        super().__init__(payload, user)
         self.id = 1
         self.name = "SillyGoose1"
 
     def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
         # set these state variables
         self.spice_loc_map = spice_loc_map
         self.spice_file_map = spice_file_map
         self.order_map = order_map
 
         # confirm that other actors have set variables
         all_ready = False
         while not all_ready:
             all_ready = True
             for id in [2, 3, 4]:
-                goose = ray.get_actor(f"SillyGoose{id}")
+                goose = ray.get_actor(f"SillyGoose{id}", namespace=self.user)
                 loc_map = ray.get(goose.get_spice_loc_map.remote())
                 all_ready = all_ready and (loc_map is not None)
 
         # get spice locations and iterate over them to destroy spice
         out = np.where(spice_loc_map==1)
         for i, j in zip(out[0], out[1]):
             # move Geese that are needed to location (i,j)
             geese_ids = self.order_map[(i,j)]
             for goose_id in geese_ids:
                 if goose_id != 1:
-                    goose = ray.get_actor(f"SillyGoose{goose_id}")
+                    goose = ray.get_actor(f"SillyGoose{goose_id}", namespace=self.user)
                     goose._ride_sandworm.remote(i, j)
                 else:
                     self._ride_sandworm(i, j)
 
             # destroy spice in synchronous fashion
             for goose_id in geese_ids:
                 if goose_id != 1:
-                    goose = ray.get_actor(f"SillyGoose{goose_id}")
+                    goose = ray.get_actor(f"SillyGoose{goose_id}", namespace=self.user)
                     ray.get(goose._destroy_spice_field.remote())
                 else:
                     self._destroy_spice_field()
 
 
-@ray.remote(num_cpus=0.8, name="SillyGoose2", resources={"worker3": 1e-4})
+@ray.remote
 class SillyGoose2(BaseSillyGoose):
-    def __init__(self, payload: str):
-        super().__init__(payload)
+    def __init__(self, payload: str, user: str):
+        super().__init__(payload, user)
         self.id = 2
         self.name = "SillyGoose2"
 
-@ray.remote(num_cpus=0.8, name="SillyGoose3", resources={"worker4": 1e-4})
+@ray.remote
 class SillyGoose3(BaseSillyGoose):
-    def __init__(self, payload: str):
-        super().__init__(payload)
+    def __init__(self, payload: str, user: str):
+        super().__init__(payload, user)
         self.id = 3
         self.name = "SillyGoose3"
 
-@ray.remote(num_cpus=0.8, name="SillyGoose4", resources={"worker4": 1e-4})
+@ray.remote
 class SillyGoose4(BaseSillyGoose):
-    def __init__(self, payload: str):
-        super().__init__(payload)
+    def __init__(self, payload: str, user: str):
+        super().__init__(payload, user)
         self.id = 4
         self.name = "SillyGoose4"
 
 
 ##############################################################################################
 ###############################         Glossu Rabban          ###############################
 ##############################################################################################
 class BaseGlossuRabban(BaseRivalActor):
-    def __init__(self, payload: str):
-        super().__init__(payload)
+    def __init__(self, payload: str, user: str):
+        super().__init__(payload, user)
 
     def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
         # set these state variables
         self.spice_loc_map = spice_loc_map
         self.spice_file_map = spice_file_map
         self.order_map = order_map
 
     def get_spice_loc_map(self):
         return self.spice_loc_map
 
 
-@ray.remote(num_cpus=0.8, name="GlossuRabban1", resources={"worker3": 1e-4})
+@ray.remote
 class GlossuRabban1(BaseGlossuRabban):
     """
     GlossuRabban1 is the leader. It first filters for the subset of non-S3 spice fields.
     It then picks the closest non-S3 spice field to target and moves all other warriors to that target.
     Once the necessary warriors arrive, it instructs the warriors to destroy spice in the specified order.
     """
-    def __init__(self, payload: str):
-        super().__init__(payload)
+    def __init__(self, payload: str, user: str):
+        super().__init__(payload, user)
         self.id = 1
         self.name = "GlossuRabban1"
 
     def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
         # set these state variables
         self.spice_loc_map = spice_loc_map
         self.spice_file_map = spice_file_map
         self.order_map = order_map
 
         # confirm that other actors have set variables
         all_ready = False
         while not all_ready:
             all_ready = True
             for id in [2, 3, 4]:
-                warrior = ray.get_actor(f"GlossuRabban{id}")
+                warrior = ray.get_actor(f"GlossuRabban{id}", namespace=self.user)
                 loc_map = ray.get(warrior.get_spice_loc_map.remote())
                 all_ready = all_ready and (loc_map is not None)
 
         def destroy_all_spice_of_file_type(file_type):
             # get spice locations and iterate over them to destroy spice
             spice = np.where(spice_file_map==file_type)
             for i, j in zip(spice[0], spice[1]):
                 # move warriors that are needed to location (i,j)
                 warrior_ids = self.order_map[(i,j)]
                 for warrior_id in warrior_ids:
                     if warrior_id != 1:
-                        warrior = ray.get_actor(f"GlossuRabban{warrior_id}")
+                        warrior = ray.get_actor(f"GlossuRabban{warrior_id}", namespace=self.user)
                         warrior._ride_sandworm.remote(i, j)
                     else:
                         self._ride_sandworm(i, j)
 
                 # destroy spice in synchronous fashion
                 for warrior_id in warrior_ids:
                     if warrior_id != 1:
-                        warrior = ray.get_actor(f"GlossuRabban{warrior_id}")
+                        warrior = ray.get_actor(f"GlossuRabban{warrior_id}", namespace=self.user)
                         ray.get(warrior._destroy_spice_field.remote())
                     else:
                         self._destroy_spice_field()
 
         # destroy all object store spice and then all s3 spice
         destroy_all_spice_of_file_type(OBJ_FILE)
         destroy_all_spice_of_file_type(S3_FILE)
 
 
-@ray.remote(num_cpus=0.8, name="GlossuRabban2", resources={"worker3": 1e-4})
+@ray.remote
 class GlossuRabban2(BaseGlossuRabban):
-    def __init__(self, payload: str):
-        super().__init__(payload)
+    def __init__(self, payload: str, user: str):
+        super().__init__(payload, user)
         self.id = 2
         self.name = "GlossuRabban2"
 
-@ray.remote(num_cpus=0.8, name="GlossuRabban3", resources={"worker4": 1e-4})
+@ray.remote
 class GlossuRabban3(BaseGlossuRabban):
-    def __init__(self, payload: str):
-        super().__init__(payload)
+    def __init__(self, payload: str, user: str):
+        super().__init__(payload, user)
         self.id = 3
         self.name = "GlossuRabban3"
 
-@ray.remote(num_cpus=0.8, name="GlossuRabban4", resources={"worker4": 1e-4})
+@ray.remote
 class GlossuRabban4(BaseGlossuRabban):
-    def __init__(self, payload: str):
-        super().__init__(payload)
+    def __init__(self, payload: str, user: str):
+        super().__init__(payload, user)
         self.id = 4
         self.name = "GlossuRabban4"
 
 ##############################################################################################
 ################################         Feyd Rautha          ################################
 ##############################################################################################
 class BaseFeydRautha(BaseRivalActor):
-    def __init__(self, payload: str):
-        super().__init__(payload)
+    def __init__(self, payload: str, user: str):
+        super().__init__(payload, user)
         self.id = None
         self.free = None
         self.num_singletons = {}
 
     def get_spice_loc_map(self):
         return self.spice_loc_map
 
@@ -425,59 +426,59 @@
 
                     if not_free:
                         continue
 
                     # otherwise, move warriors that are needed to location (i,j)
                     for warrior_id in warrior_ids:
                         if warrior_id != self.id:
-                            warrior = ray.get_actor(f"FeydRautha{warrior_id}")
+                            warrior = ray.get_actor(f"FeydRautha{warrior_id}", namespace=self.user)
                             warrior._ride_sandworm.remote(i, j)
                         else:
                             self._ride_sandworm(i, j)
 
                     # destroy spice in asynchronous fashion
                     for warrior_id in warrior_ids:
                         if warrior_id != self.id:
-                            warrior = ray.get_actor(f"FeydRautha{warrior_id}")
+                            warrior = ray.get_actor(f"FeydRautha{warrior_id}", namespace=self.user)
                             warrior.destroy_spice_field_with_retry.remote(leader=self.id)
                         else:
                             self.destroy_spice_field_with_retry(leader=self.id)
 
             # destroy s3 spice
             # get spice locations and iterate over them to destroy spice
             spice = np.where(spice_file_map==S3_FILE)
             for i, j in zip(spice[0], spice[1]):
                 # move warriors that are needed to location (i,j)
                 warrior_ids = self.order_map[(i,j)]
                 for warrior_id in warrior_ids:
                     if warrior_id != self.id:
-                        warrior = ray.get_actor(f"FeydRautha{warrior_id}")
+                        warrior = ray.get_actor(f"FeydRautha{warrior_id}", namespace=self.user)
                         warrior._ride_sandworm.remote(i, j)
                     else:
                         self._ride_sandworm(i, j)
 
                 # destroy spice in synchronous fashion
                 for warrior_id in warrior_ids:
                     if warrior_id != self.id:
-                        warrior = ray.get_actor(f"FeydRautha{warrior_id}")
+                        warrior = ray.get_actor(f"FeydRautha{warrior_id}", namespace=self.user)
                         ray.get(warrior._destroy_spice_field.remote())
                     else:
                         self._destroy_spice_field()
 
 
-@ray.remote(num_cpus=0.8, name="FeydRautha1", resources={"worker3": 1e-4})
+@ray.remote
 class FeydRautha1(BaseFeydRautha):
     """
     FeydRautha computes the distance from each worker to its top-k nearest spice fields
     and coordinates which one(s) to destroy. The (k/2)-kth closest fields are selected to be destroyed,
     and if any actors which are not needed can be used to destroy one of the [k/2, k] fields in parallel
     then that is done as well.
     """
-    def __init__(self, payload: str):
-        super().__init__(payload)
+    def __init__(self, payload: str, user: str):
+        super().__init__(payload, user)
         self.id = 1
         self.name = "FeydRautha1"
         self.k = 10
 
     # def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
     #     # set these state variables
     #     self.spice_loc_map = spice_loc_map
@@ -562,42 +563,42 @@
     #             if warrior_id != 1:
     #                 warrior = ray.get_actor(f"FeydRautha{warrior_id}")
     #                 ray.get(warrior._destroy_spice_field.remote())
     #             else:
     #                 self._destroy_spice_field()
 
 
-@ray.remote(num_cpus=0.8, name="FeydRautha2", resources={"worker3": 1e-4})
+@ray.remote
 class FeydRautha2(BaseFeydRautha):
-    def __init__(self, payload: str):
-        super().__init__(payload)
+    def __init__(self, payload: str, user: str):
+        super().__init__(payload, user)
         self.id = 2
         self.name = "FeydRautha2"
 
-@ray.remote(num_cpus=0.8, name="FeydRautha3", resources={"worker4": 1e-4})
+@ray.remote
 class FeydRautha3(BaseFeydRautha):
-    def __init__(self, payload: str):
-        super().__init__(payload)
+    def __init__(self, payload: str, user: str):
+        super().__init__(payload, user)
         self.id = 3
         self.name = "FeydRautha3"
 
-@ray.remote(num_cpus=0.8, name="FeydRautha4", resources={"worker4": 1e-4})
+@ray.remote
 class FeydRautha4(BaseFeydRautha):
-    def __init__(self, payload: str):
-        super().__init__(payload)
+    def __init__(self, payload: str, user: str):
+        super().__init__(payload, user)
         self.id = 4
         self.name = "FeydRautha4"
 
 
 ##############################################################################################
 ################################          Sardaukar           ################################
 ##############################################################################################
 class BaseSardaukar(BaseRivalActor):
-    def __init__(self, payload: str):
-        super().__init__(payload)
+    def __init__(self, payload: str, user: str):
+        super().__init__(payload, user)
         self.id = None
         self.k = 50
 
     def get_spice_loc_map(self):
         return self.spice_loc_map
 
     def is_free(self):
@@ -648,48 +649,46 @@
                     row_locs = []
                 prev_i = i
 
             return locs
 
         # compute location of spice fields of different num workers
         obj_first_spice = get_warrior_spice_arr(file_type=OBJ_FILE, warrior_idx=0)
-        # obj_second_spice_arr = get_warrior_spice_arr(file_type=OBJ_FILE, warrior_idx=1)
-        # obj_third_spice_arr = get_warrior_spice_arr(file_type=OBJ_FILE, warrior_idx=2)
 
         # destroy all the obj singletons associated with this warrior
         for i, j, next_warrior_ids in obj_first_spice:
             self._ride_sandworm(i, j)
             self._destroy_spice_field()
             if len(next_warrior_ids) > 0:
                 next_warrior_id = next_warrior_ids[0]
                 next_warrior_ids = next_warrior_ids[1:]
                 self.gamestate.send_message.remote(next_warrior_id, self.id, {"loc": [i, j], "next_warrior_ids": next_warrior_ids}, "rival")
 
         # move to center
         self._ride_sandworm(int(MAP_DIM/2), int(MAP_DIM/2))
-
-        all_msgs = []
-        while True:
+        all_msgs, num_iters_no_messages = [], 0
+        while num_iters_no_messages < 2000:
             # fetch messages with fields ready to be destroyed
             for warrior_id in [1, 2, 3, 4]:
                 if warrior_id == self.id:
                     continue
 
                 # fetch messages
                 msgs = ray.get(self.gamestate.get_new_messages.remote(self.id, warrior_id, "rival"))
                 all_msgs.extend(msgs)
 
             # add index to each msg in all_msgs
             all_msgs = [(d, idx) for idx, d in enumerate(all_msgs)]
 
             if len(all_msgs) == 0:
-                print("SLEEPING FOR NEW MESSAGES")
-                print(f"ALL MESSAGES: {all_msgs}")
+                num_iters_no_messages += 1
                 time.sleep(0.001)
                 continue
+            else:
+                num_iters_no_messages = 0
 
             # filter locations for subset with only one warrior left
             elts = list(map(lambda tup: (tup[0]["loc"], tup[0]["next_warrior_ids"], tup[1]), all_msgs))
             elts_ = list(filter(lambda tup: len(tup[1]) == 0, elts))
             if len(elts_) == 0:
                 elts_ = list(filter(lambda tup: len(tup[1]) == 1, elts))
 
@@ -724,34 +723,62 @@
             close_all_msgs_idxs = close_all_msgs_idxs if k > 1 else [close_all_msgs_idxs]
             new_all_msgs = []
             for d, idx in all_msgs:
                 if idx not in close_all_msgs_idxs:
                     new_all_msgs.append(d)
             all_msgs = new_all_msgs
 
-@ray.remote(num_cpus=0.8, name="Sardaukar1", resources={"worker3": 1e-4})
+        # destroy all obj spice fields w/4 workers
+        if self.id == 1:
+            spice = np.where(spice_file_map==OBJ_FILE)
+            for i, j in zip(spice[0], spice[1]):
+                # filter for locations with 4 warriors
+                warrior_ids = self.order_map[(i,j)]
+                if len(warrior_ids) < 4:
+                    continue
+
+                # move warriors that are needed to location (i,j)
+                for warrior_id in warrior_ids:
+                    if warrior_id != self.id:
+                        warrior = ray.get_actor(f"Sardaukar{warrior_id}", namespace=self.user)
+                        warrior._ride_sandworm.remote(i, j)
+                    else:
+                        self._ride_sandworm(i, j)
+
+                # destroy spice in synchronous fashion
+                for warrior_id in warrior_ids:
+                    if warrior_id != self.id:
+                        warrior = ray.get_actor(f"Sardaukar{warrior_id}", namespace=self.user)
+                        ray.get(warrior._destroy_spice_field.remote())
+                    else:
+                        self._destroy_spice_field()
+
+        # print message that you're done
+        print("SLEEPING NOW")
+
+@ray.remote
 class Sardaukar1(BaseSardaukar):
-    def __init__(self, payload: str):
-        super().__init__(payload)
+    def __init__(self, payload: str, user: str):
+        super().__init__(payload, user)
         self.id = 1
         self.name = "Sardaukar1"
 
-@ray.remote(num_cpus=0.8, name="Sardaukar2", resources={"worker3": 1e-4})
+@ray.remote
 class Sardaukar2(BaseSardaukar):
-    def __init__(self, payload: str):
-        super().__init__(payload)
+    def __init__(self, payload: str, user: str):
+        super().__init__(payload, user)
         self.id = 2
         self.name = "Sardaukar2"
 
-@ray.remote(num_cpus=0.8, name="Sardaukar3", resources={"worker4": 1e-4})
+@ray.remote
 class Sardaukar3(BaseSardaukar):
-    def __init__(self, payload: str):
-        super().__init__(payload)
+    def __init__(self, payload: str, user: str):
+        super().__init__(payload, user)
         self.id = 3
         self.name = "Sardaukar3"
 
-@ray.remote(num_cpus=0.8, name="Sardaukar4", resources={"worker4": 1e-4})
+@ray.remote
 class Sardaukar4(BaseSardaukar):
-    def __init__(self, payload: str):
-        super().__init__(payload)
+    def __init__(self, payload: str, user: str):
+        super().__init__(payload, user)
         self.id = 4
         self.name = "Sardaukar4"
```


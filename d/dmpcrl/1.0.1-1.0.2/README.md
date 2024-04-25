# Comparing `tmp/dmpcrl-1.0.1.tar.gz` & `tmp/dmpcrl-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmpcrl-1.0.1.tar", last modified: Thu Jan 18 10:40:38 2024, max compression
+gzip compressed data, was "dmpcrl-1.0.2.tar", last modified: Thu Apr 25 11:40:20 2024, max compression
```

## Comparing `dmpcrl-1.0.1.tar` & `dmpcrl-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-01-18 10:40:38.676000 dmpcrl-1.0.1/
--rw-rw-rw-   0        0        0     1091 2023-08-28 12:20:33.000000 dmpcrl-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      978 2024-01-18 10:40:38.674742 dmpcrl-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1110 2024-01-18 10:39:14.000000 dmpcrl-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-18 10:40:38.676000 dmpcrl-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-18 10:40:38.642073 dmpcrl-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-01-18 10:40:38.657155 dmpcrl-1.0.1/src/dmpcrl/
--rw-rw-rw-   0        0        0        0 2023-09-21 13:25:29.000000 dmpcrl-1.0.1/src/dmpcrl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-18 10:40:38.664909 dmpcrl-1.0.1/src/dmpcrl/agents/
--rw-rw-rw-   0        0        0        0 2023-06-20 13:07:59.000000 dmpcrl-1.0.1/src/dmpcrl/agents/__init__.py
--rw-rw-rw-   0        0        0    16112 2024-01-18 09:16:49.000000 dmpcrl-1.0.1/src/dmpcrl/agents/lstd_ql_coordinator.py
-drwxrwxrwx   0        0        0        0 2024-01-18 10:40:38.667093 dmpcrl-1.0.1/src/dmpcrl/core/
--rw-rw-rw-   0        0        0        0 2023-06-20 14:30:58.000000 dmpcrl-1.0.1/src/dmpcrl/core/__init__.py
--rw-rw-rw-   0        0        0     5854 2024-01-18 09:15:46.000000 dmpcrl-1.0.1/src/dmpcrl/core/admm.py
--rw-rw-rw-   0        0        0     1112 2023-09-05 11:34:31.000000 dmpcrl-1.0.1/src/dmpcrl/core/consensus.py
-drwxrwxrwx   0        0        0        0 2024-01-18 10:40:38.668781 dmpcrl-1.0.1/src/dmpcrl/mpc/
--rw-rw-rw-   0        0        0        0 2023-06-20 13:08:00.000000 dmpcrl-1.0.1/src/dmpcrl/mpc/__init__.py
--rw-rw-rw-   0        0        0     4686 2024-01-18 09:15:46.000000 dmpcrl-1.0.1/src/dmpcrl/mpc/mpc_admm.py
-drwxrwxrwx   0        0        0        0 2024-01-18 10:40:38.670786 dmpcrl-1.0.1/src/dmpcrl/utils/
--rw-rw-rw-   0        0        0        0 2023-09-21 12:27:00.000000 dmpcrl-1.0.1/src/dmpcrl/utils/__init__.py
--rw-rw-rw-   0        0        0     1579 2023-10-17 15:56:37.000000 dmpcrl-1.0.1/src/dmpcrl/utils/discretisation.py
--rw-rw-rw-   0        0        0      947 2024-01-18 09:16:49.000000 dmpcrl-1.0.1/src/dmpcrl/utils/tikz.py
-drwxrwxrwx   0        0        0        0 2024-01-18 10:40:38.673743 dmpcrl-1.0.1/src/dmpcrl.egg-info/
--rw-rw-rw-   0        0        0      978 2024-01-18 10:40:38.000000 dmpcrl-1.0.1/src/dmpcrl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      556 2024-01-18 10:40:38.000000 dmpcrl-1.0.1/src/dmpcrl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-18 10:40:38.000000 dmpcrl-1.0.1/src/dmpcrl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2024-01-18 10:40:38.000000 dmpcrl-1.0.1/src/dmpcrl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-01-18 10:40:38.000000 dmpcrl-1.0.1/src/dmpcrl.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-01-18 10:40:38.673743 dmpcrl-1.0.1/tests/
--rw-rw-rw-   0        0        0      736 2023-09-15 10:16:40.000000 dmpcrl-1.0.1/tests/test_dual_vars.py
--rw-rw-rw-   0        0        0      285 2023-09-21 12:12:44.000000 dmpcrl-1.0.1/tests/test_examples.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:40:20.390821 dmpcrl-1.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-08-28 12:20:33.000000 dmpcrl-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      978 2024-04-25 11:40:20.390821 dmpcrl-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1110 2024-04-25 11:39:54.000000 dmpcrl-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-25 11:40:20.390821 dmpcrl-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-25 11:40:20.371931 dmpcrl-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-25 11:40:20.371931 dmpcrl-1.0.2/src/dmpcrl/
+-rw-rw-rw-   0        0        0        0 2023-09-21 13:25:29.000000 dmpcrl-1.0.2/src/dmpcrl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:40:20.387560 dmpcrl-1.0.2/src/dmpcrl/agents/
+-rw-rw-rw-   0        0        0        0 2023-06-20 13:07:59.000000 dmpcrl-1.0.2/src/dmpcrl/agents/__init__.py
+-rw-rw-rw-   0        0        0    16190 2024-04-04 07:40:53.000000 dmpcrl-1.0.2/src/dmpcrl/agents/lstd_ql_coordinator.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:40:20.390821 dmpcrl-1.0.2/src/dmpcrl/core/
+-rw-rw-rw-   0        0        0        0 2023-06-20 14:30:58.000000 dmpcrl-1.0.2/src/dmpcrl/core/__init__.py
+-rw-rw-rw-   0        0        0     5854 2024-01-18 09:15:46.000000 dmpcrl-1.0.2/src/dmpcrl/core/admm.py
+-rw-rw-rw-   0        0        0     1112 2023-09-05 11:34:31.000000 dmpcrl-1.0.2/src/dmpcrl/core/consensus.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:40:20.390821 dmpcrl-1.0.2/src/dmpcrl/mpc/
+-rw-rw-rw-   0        0        0        0 2023-06-20 13:08:00.000000 dmpcrl-1.0.2/src/dmpcrl/mpc/__init__.py
+-rw-rw-rw-   0        0        0     4699 2024-04-04 07:41:59.000000 dmpcrl-1.0.2/src/dmpcrl/mpc/mpc_admm.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:40:20.390821 dmpcrl-1.0.2/src/dmpcrl/utils/
+-rw-rw-rw-   0        0        0        0 2023-09-21 12:27:00.000000 dmpcrl-1.0.2/src/dmpcrl/utils/__init__.py
+-rw-rw-rw-   0        0        0     1579 2023-10-17 15:56:37.000000 dmpcrl-1.0.2/src/dmpcrl/utils/discretisation.py
+-rw-rw-rw-   0        0        0      947 2024-01-18 09:16:49.000000 dmpcrl-1.0.2/src/dmpcrl/utils/tikz.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:40:20.390821 dmpcrl-1.0.2/src/dmpcrl.egg-info/
+-rw-rw-rw-   0        0        0      978 2024-04-25 11:40:20.000000 dmpcrl-1.0.2/src/dmpcrl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2024-04-25 11:40:20.000000 dmpcrl-1.0.2/src/dmpcrl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 11:40:20.000000 dmpcrl-1.0.2/src/dmpcrl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2024-04-25 11:40:20.000000 dmpcrl-1.0.2/src/dmpcrl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-25 11:40:20.000000 dmpcrl-1.0.2/src/dmpcrl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 11:40:20.390821 dmpcrl-1.0.2/tests/
+-rw-rw-rw-   0        0        0      736 2023-09-15 10:16:40.000000 dmpcrl-1.0.2/tests/test_dual_vars.py
+-rw-rw-rw-   0        0        0      285 2023-09-21 12:12:44.000000 dmpcrl-1.0.2/tests/test_examples.py
```

### Comparing `dmpcrl-1.0.1/LICENSE` & `dmpcrl-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dmpcrl-1.0.1/PKG-INFO` & `dmpcrl-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmpcrl
-Version: 1.0.1
+Version: 1.0.2
 Summary: Distributed Reinforcement Learning with  Distributed Model Predictive Control
 Author-email: Samuel Mallick <sam.mallick.97@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/SamuelMallick/distributed-mpc-reinforcement-learning
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dmpcrl-1.0.1/pyproject.toml` & `dmpcrl-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmpcrl"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Samuel Mallick", email="sam.mallick.97@gmail.com" },
 ]
 description = "Distributed Reinforcement Learning with  Distributed Model Predictive Control"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "MIT" }
```

### Comparing `dmpcrl-1.0.1/src/dmpcrl/agents/lstd_ql_coordinator.py` & `dmpcrl-1.0.2/src/dmpcrl/agents/lstd_ql_coordinator.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,37 +8,38 @@
 from gymnasium import Env
 from mpcrl import LstdQLearningAgent
 from mpcrl.agents.agent import ActType, ObsType, SymType
 from mpcrl.agents.lstd_q_learning import ExpType
 from mpcrl.agents.rl_learning_agent import LrType
 from mpcrl.core.experience import ExperienceReplay
 from mpcrl.core.exploration import ExplorationStrategy, StepWiseExploration
-from mpcrl.core.learning_rate import LearningRate
+# from mpcrl.core.learning_rate import LearningRate
 from mpcrl.core.parameters import LearnableParametersDict
 from mpcrl.core.schedulers import Scheduler
 from mpcrl.core.update import UpdateStrategy
 from mpcrl.wrappers.agents import RecordUpdates
 
 from dmpcrl.core.admm import AdmmCoordinator
 from dmpcrl.core.consensus import ConsensusCoordinator
 from dmpcrl.mpc.mpc_admm import MpcAdmm
 
 
 class LstdQLearningAgentCoordinator(LstdQLearningAgent):
     """Coordinator to handle the communication and learning of a multi-agent q-learning system."""
 
-    admm_iters = 500
+    admm_iters = 50
     consensus_iters = 100
 
     def __init__(
         self,
         mpc_cent: Mpc[SymType],
         update_strategy: Union[int, UpdateStrategy],
         discount_factor: float,
-        learning_rate: Union[LrType, Scheduler[LrType], LearningRate[LrType]],
+        # learning_rate: Union[LrType, Scheduler[LrType], LearningRate[LrType]],    # TODO find out why learning rate cannot import
+        learning_rate,
         learnable_parameters: LearnableParametersDict[SymType],
         n: int,
         mpc_dist_list: list[MpcAdmm],
         learnable_dist_parameters_list: list[LearnableParametersDict[SymType]],
         fixed_dist_parameters_list: list,
         G: list[list[int]],
         Adj: np.ndarray,
```

### Comparing `dmpcrl-1.0.1/src/dmpcrl/core/admm.py` & `dmpcrl-1.0.2/src/dmpcrl/core/admm.py`

 * *Files identical despite different names*

### Comparing `dmpcrl-1.0.1/src/dmpcrl/core/consensus.py` & `dmpcrl-1.0.2/src/dmpcrl/core/consensus.py`

 * *Files identical despite different names*

### Comparing `dmpcrl-1.0.1/src/dmpcrl/mpc/mpc_admm.py` & `dmpcrl-1.0.2/src/dmpcrl/mpc/mpc_admm.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         n_in,
         n_out,
     ) -> None:
         raise RuntimeError(
             "For ADMM based MPC the dynamics must be set manually as constraints due to the coupling."
         )
 
-    def set_local_cost(self, local_cost: cs.SX):
+    def set_local_cost(self, local_cost: cs.SX, rho: float = 0.5):
         """Sets the cost function for the ADMM based MPC. The augmented lagrangian
         terms are augmented to the local cost."""
 
         if not hasattr(self, "x_cat"):
             raise RuntimeError(
                 "You must call augmented_state before setting local cost."
             )
@@ -118,11 +118,11 @@
         self.minimize(
             local_cost
             + sum(
                 (self.y[:, [k]].T @ (self.x_cat[:, [k]] - self.z[:, [k]]))
                 for k in range(self.N + 1)
             )
             + sum(
-                ((self.rho / 2) * cs.norm_2(self.x_cat[:, [k]] - self.z[:, [k]]) ** 2)
+                ((rho / 2) * cs.norm_2(self.x_cat[:, [k]] - self.z[:, [k]]) ** 2)
                 for k in range(self.N + 1)
             )
         )
```

### Comparing `dmpcrl-1.0.1/src/dmpcrl/utils/discretisation.py` & `dmpcrl-1.0.2/src/dmpcrl/utils/discretisation.py`

 * *Files identical despite different names*

### Comparing `dmpcrl-1.0.1/src/dmpcrl/utils/tikz.py` & `dmpcrl-1.0.2/src/dmpcrl/utils/tikz.py`

 * *Files identical despite different names*

### Comparing `dmpcrl-1.0.1/src/dmpcrl.egg-info/PKG-INFO` & `dmpcrl-1.0.2/src/dmpcrl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmpcrl
-Version: 1.0.1
+Version: 1.0.2
 Summary: Distributed Reinforcement Learning with  Distributed Model Predictive Control
 Author-email: Samuel Mallick <sam.mallick.97@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/SamuelMallick/distributed-mpc-reinforcement-learning
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dmpcrl-1.0.1/src/dmpcrl.egg-info/SOURCES.txt` & `dmpcrl-1.0.2/src/dmpcrl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dmpcrl-1.0.1/tests/test_dual_vars.py` & `dmpcrl-1.0.2/tests/test_dual_vars.py`

 * *Files identical despite different names*


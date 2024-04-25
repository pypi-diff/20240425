# Comparing `tmp/dmpcpwa-0.0.1.tar.gz` & `tmp/dmpcpwa-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmpcpwa-0.0.1.tar", last modified: Thu Jan 18 10:25:55 2024, max compression
+gzip compressed data, was "dmpcpwa-0.0.2.tar", last modified: Thu Apr 25 11:44:22 2024, max compression
```

## Comparing `dmpcpwa-0.0.1.tar` & `dmpcpwa-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-01-18 10:25:55.134977 dmpcpwa-0.0.1/
--rw-rw-rw-   0        0        0    35823 2023-09-20 12:29:52.000000 dmpcpwa-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1038 2024-01-18 10:25:55.132255 dmpcpwa-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       23 2023-09-21 12:03:55.000000 dmpcpwa-0.0.1/README.md
--rw-rw-rw-   0        0        0     1127 2024-01-18 10:20:32.000000 dmpcpwa-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-18 10:25:55.134977 dmpcpwa-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-18 10:25:55.100313 dmpcpwa-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-01-18 10:25:55.107319 dmpcpwa-0.0.1/src/dmpcpwa/
--rw-rw-rw-   0        0        0        0 2023-09-21 14:00:09.000000 dmpcpwa-0.0.1/src/dmpcpwa/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-18 10:25:55.121640 dmpcpwa-0.0.1/src/dmpcpwa/agents/
--rw-rw-rw-   0        0        0        0 2023-09-21 12:27:23.000000 dmpcpwa-0.0.1/src/dmpcpwa/agents/__init__.py
--rw-rw-rw-   0        0        0    12865 2024-01-18 09:05:11.000000 dmpcpwa-0.0.1/src/dmpcpwa/agents/g_admm_coordinator.py
--rw-rw-rw-   0        0        0     5587 2024-01-18 10:03:06.000000 dmpcpwa-0.0.1/src/dmpcpwa/agents/mld_agent.py
--rw-rw-rw-   0        0        0     2898 2023-12-15 09:47:34.000000 dmpcpwa-0.0.1/src/dmpcpwa/agents/no_control_agent.py
--rw-rw-rw-   0        0        0     6222 2024-01-15 12:02:35.000000 dmpcpwa-0.0.1/src/dmpcpwa/agents/pwa_agent.py
--rw-rw-rw-   0        0        0     9113 2023-09-21 15:11:09.000000 dmpcpwa-0.0.1/src/dmpcpwa/agents/sqp_admm_coordinator.py
-drwxrwxrwx   0        0        0        0 2024-01-18 10:25:55.125625 dmpcpwa-0.0.1/src/dmpcpwa/mpc/
--rw-rw-rw-   0        0        0        0 2023-09-21 12:27:23.000000 dmpcpwa-0.0.1/src/dmpcpwa/mpc/__init__.py
--rw-rw-rw-   0        0        0    11269 2023-12-15 09:46:21.000000 dmpcpwa-0.0.1/src/dmpcpwa/mpc/mpc_mld.py
--rw-rw-rw-   0        0        0     2608 2023-12-06 10:32:13.000000 dmpcpwa-0.0.1/src/dmpcpwa/mpc/mpc_mld_cent_decup.py
--rw-rw-rw-   0        0        0     3137 2023-12-05 12:38:19.000000 dmpcpwa-0.0.1/src/dmpcpwa/mpc/mpc_switching.py
-drwxrwxrwx   0        0        0        0 2024-01-18 10:25:55.129612 dmpcpwa-0.0.1/src/dmpcpwa/utils/
--rw-rw-rw-   0        0        0        0 2023-09-21 12:27:23.000000 dmpcpwa-0.0.1/src/dmpcpwa/utils/__init__.py
--rw-rw-rw-   0        0        0     2821 2023-09-28 13:28:32.000000 dmpcpwa-0.0.1/src/dmpcpwa/utils/pwa_models.py
--rw-rw-rw-   0        0        0      948 2023-12-05 11:52:38.000000 dmpcpwa-0.0.1/src/dmpcpwa/utils/tikz.py
-drwxrwxrwx   0        0        0        0 2024-01-18 10:25:55.130609 dmpcpwa-0.0.1/src/dmpcpwa.egg-info/
--rw-rw-rw-   0        0        0     1038 2024-01-18 10:25:55.000000 dmpcpwa-0.0.1/src/dmpcpwa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      662 2024-01-18 10:25:55.000000 dmpcpwa-0.0.1/src/dmpcpwa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-18 10:25:55.000000 dmpcpwa-0.0.1/src/dmpcpwa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2024-01-18 10:25:55.000000 dmpcpwa-0.0.1/src/dmpcpwa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-01-18 10:25:55.000000 dmpcpwa-0.0.1/src/dmpcpwa.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 11:44:21.989505 dmpcpwa-0.0.2/
+-rw-rw-rw-   0        0        0    35823 2023-09-20 12:29:52.000000 dmpcpwa-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1038 2024-04-25 11:44:21.989505 dmpcpwa-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       23 2023-09-21 12:03:55.000000 dmpcpwa-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1127 2024-02-08 13:40:09.000000 dmpcpwa-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-25 11:44:22.002816 dmpcpwa-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-25 11:44:21.951713 dmpcpwa-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-25 11:44:21.951713 dmpcpwa-0.0.2/src/dmpcpwa/
+-rw-rw-rw-   0        0        0        0 2023-09-21 14:00:09.000000 dmpcpwa-0.0.2/src/dmpcpwa/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:44:21.972337 dmpcpwa-0.0.2/src/dmpcpwa/agents/
+-rw-rw-rw-   0        0        0        0 2023-09-21 12:27:23.000000 dmpcpwa-0.0.2/src/dmpcpwa/agents/__init__.py
+-rw-rw-rw-   0        0        0    14142 2024-04-24 12:49:24.000000 dmpcpwa-0.0.2/src/dmpcpwa/agents/g_admm_coordinator.py
+-rw-rw-rw-   0        0        0     5724 2024-04-19 08:16:19.000000 dmpcpwa-0.0.2/src/dmpcpwa/agents/mld_agent.py
+-rw-rw-rw-   0        0        0     2842 2024-02-08 13:07:07.000000 dmpcpwa-0.0.2/src/dmpcpwa/agents/no_control_agent.py
+-rw-rw-rw-   0        0        0    10843 2024-04-24 12:43:37.000000 dmpcpwa-0.0.2/src/dmpcpwa/agents/pwa_agent.py
+-rw-rw-rw-   0        0        0     9046 2024-04-25 08:42:43.000000 dmpcpwa-0.0.2/src/dmpcpwa/agents/sqp_admm_coordinator.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:44:21.972337 dmpcpwa-0.0.2/src/dmpcpwa/mpc/
+-rw-rw-rw-   0        0        0        0 2023-09-21 12:27:23.000000 dmpcpwa-0.0.2/src/dmpcpwa/mpc/__init__.py
+-rw-rw-rw-   0        0        0    12057 2024-04-25 09:09:06.000000 dmpcpwa-0.0.2/src/dmpcpwa/mpc/mpc_mld.py
+-rw-rw-rw-   0        0        0     2793 2024-04-25 08:37:30.000000 dmpcpwa-0.0.2/src/dmpcpwa/mpc/mpc_mld_cent_decup.py
+-rw-rw-rw-   0        0        0     3137 2024-02-08 13:19:17.000000 dmpcpwa-0.0.2/src/dmpcpwa/mpc/mpc_switching.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:44:21.972337 dmpcpwa-0.0.2/src/dmpcpwa/utils/
+-rw-rw-rw-   0        0        0        0 2023-09-21 12:27:23.000000 dmpcpwa-0.0.2/src/dmpcpwa/utils/__init__.py
+-rw-rw-rw-   0        0        0     2823 2024-02-14 09:29:37.000000 dmpcpwa-0.0.2/src/dmpcpwa/utils/pwa_models.py
+-rw-rw-rw-   0        0        0      948 2023-12-05 11:52:38.000000 dmpcpwa-0.0.2/src/dmpcpwa/utils/tikz.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:44:21.989505 dmpcpwa-0.0.2/src/dmpcpwa.egg-info/
+-rw-rw-rw-   0        0        0     1038 2024-04-25 11:44:21.000000 dmpcpwa-0.0.2/src/dmpcpwa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      662 2024-04-25 11:44:21.000000 dmpcpwa-0.0.2/src/dmpcpwa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 11:44:21.000000 dmpcpwa-0.0.2/src/dmpcpwa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2024-04-25 11:44:21.000000 dmpcpwa-0.0.2/src/dmpcpwa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-25 11:44:21.000000 dmpcpwa-0.0.2/src/dmpcpwa.egg-info/top_level.txt
```

### Comparing `dmpcpwa-0.0.1/LICENSE` & `dmpcpwa-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dmpcpwa-0.0.1/PKG-INFO` & `dmpcpwa-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmpcpwa
-Version: 0.0.1
+Version: 0.0.2
 Summary: Distributed Model Predictive Control for Piecewise Affine Systems
 Author-email: Samuel Mallick <sam.mallick.97@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/SamuelMallick/distributed-mpc-pwa
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dmpcpwa-0.0.1/pyproject.toml` & `dmpcpwa-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmpcpwa"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Samuel Mallick", email="sam.mallick.97@gmail.com" },
 ]
 description = "Distributed Model Predictive Control for Piecewise Affine Systems"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "MIT" }
```

### Comparing `dmpcpwa-0.0.1/src/dmpcpwa/agents/g_admm_coordinator.py` & `dmpcpwa-0.0.2/src/dmpcpwa/agents/g_admm_coordinator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,105 +1,113 @@
 import logging
-from typing import Any, Literal
+from typing import Any
 
+# from dmpcpwa.utils.tikz import save2tikz
 import casadi as cs
 import matplotlib.pyplot as plt
 import numpy as np
 from dmpcrl.core.admm import AdmmCoordinator
 from dmpcrl.mpc.mpc_admm import MpcAdmm
 from gymnasium import Env
 from mpcrl import Agent
-from mpcrl.agents.agent import ActType, ObsType
 
 from dmpcpwa.agents.pwa_agent import PwaAgent
-
-ADMM_DEBUG_PLOT = False
-DEBUG_PRINT = False
+from dmpcpwa.utils.tikz import save2tikz
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 console_handler = logging.StreamHandler()
 console_handler.setLevel(logging.DEBUG)
 formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 console_handler.setFormatter(formatter)
 logger.addHandler(console_handler)
 
 
 class GAdmmCoordinator(Agent):
     """Coordinates the greedy ADMM algorithm for PWA agents"""
 
-    admm_iters = 50
-    switching_iters = 50
-
     def __init__(
         self,
         local_mpcs: list[MpcAdmm],
         local_fixed_parameters: list[dict],
         systems: list[dict],
         G: list[list[int]],
         Adj: np.ndarray,
         rho: float,
+        debug_plot: bool = False,
+        admm_iters: int = 50,
+        switching_iters: int | float = float("inf"),
         agent_class=PwaAgent,
-        warmstart: Literal["last", "last-successful"] = "last-successful",
-        name: str = None,
     ) -> None:
         """Instantiates the coordinator, creating n PWA agents.
 
         Parameters
         ----------
         local_mpcs: list[MpcAdmm[SymType]]
             List of local MPCs for agents.
         local_fixed_parameters: List[dict]
             List of dictionaries for fixed parameters for agents.
-        systems : dict
+        systems: dict
             PWA model for each agent.
-        G :  List[List[int]]
+        G: List[List[int]]
             Map of local to global vars in ADMM.
         Adj: np.ndarray
-            Adjacency matrix for agent coupling
+            Adjacency matrix for agent coupling.
         rho: float
-            Augmented lagrangian penalty term."""
+            Augmented lagrangian penalty term.
+        debug_plot: bool
+            Flag to activate plotting the switching ADMM convergence for debugging.
+        admm_iters: int
+            Number of iterations for the switching ADMM procedure.
+        switching_iters: int
+            For iterations greater than switching_iters, switching is no longer permitted and the ADMM iterations are standard.
+        agent_class
+            The class to use for local agents."""
 
         # to the super class we pass the first local mpc just to satisfy the constructor
         # we copy it so the parameters don't double up etc.
-        super().__init__(
-            local_mpcs[0].copy(), local_fixed_parameters[0].copy(), warmstart, name
-        )
+        super().__init__(local_mpcs[0].copy(), local_fixed_parameters[0].copy())
+
+        self.admm_iters = admm_iters
+        self.switching_iters = switching_iters
+        self.debug_plot = debug_plot
 
         # construct the agents
         self.n = len(local_mpcs)
-        self.agents: list[PwaAgent] = []
+        self.agents: list[agent_class] = []
         for i in range(self.n):
             self.agents.append(
                 agent_class(local_mpcs[i], local_fixed_parameters[i], systems[i])
             )
 
         # create ADMM coordinator
+        self.G = G
         self.N = local_mpcs[0].horizon
         self.Adj = Adj
         self.nx_l = local_mpcs[0].nx_l
         self.nu_l = local_mpcs[0].nu_l
 
         self.prev_sol = None
         self.prev_traj = None
+        self.prev_sol_time = None
 
         # coordinator of ADMM using 1 iteration as g_admm coordinator checks sequences every ADMM iter
         self.admm_coordinator = AdmmCoordinator(
             self.agents,
             G,
             self.N,
             self.nx_l,
             self.nu_l,
             rho,
             iters=1,
         )
 
     def evaluate(
         self,
-        env: Env[ObsType, ActType],
+        env: Env,
         episodes: int,
         deterministic: bool = True,
         seed: int = None,
         raises: bool = True,
         env_reset_options: dict[str, Any] = None,
     ):
         returns = np.zeros(episodes)
@@ -114,15 +122,20 @@
             truncated, terminated, timestep = False, False, 0
 
             self.on_episode_start(env, episode, state)
             for agent in self.agents:
                 agent.on_episode_start(env, episode, state)
 
             while not (truncated or terminated):
-                action, _, _, _ = self.g_admm_control(state)
+                action, sol_list, infeas_guess_flag, error_flag = self.g_admm_control(
+                    state
+                )
+
+                if infeas_guess_flag or error_flag:
+                    raise RuntimeError("G_admm infeasible or error.")
 
                 state, r, truncated, terminated, _ = env.step(action)
 
                 self.on_env_step(env, episode, timestep)
                 for agent in self.agents:
                     agent.on_env_step(env, episode, timestep)
 
@@ -140,63 +153,65 @@
         self.on_validation_end(env, returns)
         for agent in self.agents:
             agent.on_validation_end(env, returns)
         return returns
 
     def g_admm_control(self, state, warm_start=None):
         """Get the control for the given state. Warm start parameter is an initial guess for control actions."""
-        seqs = [[0] * self.N for i in range(self.n)]  # switching seqs for agents
+        seqs = [[0] * (self.N + 1) for i in range(self.n)]  # switching seqs for agents
 
         xc = [None] * self.n
         x_pred = [None] * self.n
         action_list = None
         sol_list = None
         error_flag = False
+        sol_time = 0.0
 
         # break global state into local pieces
         x = [state[self.nx_l * i : self.nx_l * (i + 1), :] for i in range(self.n)]
 
         if warm_start is None:
             warm_start = [np.zeros((self.nu_l, self.N)) for i in range(self.n)]
 
         infeas_flag = False
         u = warm_start
+
         # generate initial feasible coupling via dynamics rollout
-        try:
-            x_rout = self.dynamics_rollout(x, u)
-        except:
+        x_rout = self.dynamics_rollout(x, u)
+        if x_rout is None:
             logger.debug(f"Rollout of initial control guess {u} was infeasible.")
             infeas_flag = True
 
-        if ADMM_DEBUG_PLOT:  # store control at each iter to plot ADMM convergence
+        if self.debug_plot:  # store control at each iter to plot ADMM convergence
             u_plot_list = [
                 [np.zeros((self.nu_l, self.N)) for k in range(self.admm_iters)]
                 for i in range(self.n)
             ]
             switch_plot_list = [[] for i in range(self.n)]
             z_plot_list = [
-                [np.zeros((self.nx_l, self.N)) for k in range(self.admm_iters)]
+                [np.zeros((self.nx_l, self.N + 1)) for k in range(self.admm_iters)]
                 for i in range(self.n)
             ]
             x_plot_list = [
-                [np.zeros((self.nx_l, self.N)) for k in range(self.admm_iters)]
+                [np.zeros((self.nx_l, self.N + 1)) for k in range(self.admm_iters)]
                 for i in range(self.n)
             ]
-            x_back_plot_list = [
-                [np.zeros((self.nx_l, self.N)) for k in range(self.admm_iters)]
+            x_full_plot_list = [
+                [
+                    np.zeros((self.nx_l * len(self.G[i]), self.N + 1))
+                    for k in range(self.admm_iters)
+                ]
                 for i in range(self.n)
             ]
 
         for iter in range(self.admm_iters):
             if infeas_flag:
                 break
             logger.debug(f"Greedy admm iter {iter}")
-            # generate local sequences and choose one  - CHOICE: this can be done with vars from local output of ADMM
-            # which may not have converged to consensus - therefore adding exploration OR a cooperative
-            # dynamics rollout as before the loop
+            # generate local sequences and choose one
             if iter < self.switching_iters:
                 for i in range(self.n):
                     if iter == 0:  # first iter we must used rolled out state
                         new_seqs = self.agents[i].eval_sequences(
                             x[i],
                             u[i],
                             [x_rout[j] for j in range(self.n) if self.Adj[i, j] == 1],
@@ -214,112 +229,135 @@
                             new_seqs.remove(seqs[i])
                         if len(new_seqs) > 0:
                             logger.debug(
                                 f"Agent {i} switched: {seqs[i]} to {new_seqs[0]}"
                             )
                             seqs[i] = new_seqs[0]  # for now choosing arbritrarily first
 
-                            if ADMM_DEBUG_PLOT:
+                            if self.debug_plot:
                                 switch_plot_list[i].append(iter)
                     # set sequences
                     self.agents[i].set_sequence(seqs[i])
 
             # perform ADMM step
             action_list, sol_list, error_flag = self.admm_coordinator.solve_admm(state)
 
+            if not error_flag and all(
+                ["t_wall_total" in sol_list[i].stats for i in range(self.n)]
+            ):
+                sol_time += max(
+                    [sol_list[i].stats["t_wall_total"] for i in range(self.n)]
+                )
+
             if not error_flag:
-                if ADMM_DEBUG_PLOT:
+                if self.debug_plot:
                     for i in range(self.n):
                         u_plot_list[i][iter] = np.asarray(sol_list[i].vals["u"])
                         z_plot_list[i][iter] = self.admm_coordinator.z[
                             i * self.nx_l : (i + 1) * self.nx_l, :
                         ]
                         x_plot_list[i][iter] = np.asarray(sol_list[i].vals["x"])
-                        if i != self.n - 1:
-                            x_back_plot_list[i][iter] = np.asarray(
-                                sol_list[i].vals["x_c"][-2:, :]
-                            )
+                        x_full_plot_list[i][iter] = np.vstack(
+                            [
+                                np.asarray(sol_list[i].vals["x_c"])[
+                                    : (self.G[i].index(i) * self.nx_l), :
+                                ],
+                                np.asarray(sol_list[i].vals["x"]),
+                                np.asarray(sol_list[i].vals["x_c"])[
+                                    (self.G[i].index(i) * self.nx_l) :, :
+                                ],
+                            ]
+                        )
 
                 # extract the vars across the horizon from the ADMM sol for each agent
                 for i in range(self.n):
                     u[i] = np.asarray(sol_list[i].vals["u"])
                     x_pred[i] = np.asarray(sol_list[i].vals["x"])
                     xc_out = np.asarray(sol_list[i].vals["x_c"])
                     xc_temp = []
                     for j in range(self.agents[i].num_neighbours):
                         xc_temp.append(xc_out[self.nx_l * j : self.nx_l * (j + 1), :])
                     xc[i] = xc_temp
             else:
                 break
 
-        if ADMM_DEBUG_PLOT:
+        if self.debug_plot:
             self.plot_admm_iters(
                 u_plot_list,
                 z_plot_list,
                 x_plot_list,
-                x_back_plot_list,
+                x_full_plot_list,
                 switch_plot_list,
             )
 
-        self.prev_sol = u
-        self.prev_traj = x_pred
-        return cs.DM(action_list), sol_list, error_flag, infeas_flag
+        if not error_flag and not infeas_flag:
+            self.prev_sol = u
+            self.prev_traj = x_pred
+            self.prev_sol_time = sol_time
+
+        return (
+            cs.DM(action_list) if not infeas_flag and not error_flag else warm_start,
+            sol_list,
+            error_flag,
+            infeas_flag,
+        )
 
     def dynamics_rollout(self, x: list[np.ndarray], u: list[np.ndarray]):
-        """For a given state and u, rollout the agents' dynamics step by step."""
-        x_temp = [np.zeros((self.nx_l, self.N)) for i in range(self.n)]
+        """For a given state and u, rollout the agents' dynamics step by step. Return None if the u is infeasible."""
+        x_temp = [np.zeros((self.nx_l, self.N + 1)) for i in range(self.n)]
 
         for i in range(self.n):
             x_temp[i][:, [0]] = x[i]  # add the first known states to the temp
-        for k in range(1, self.N):
+        for k in range(1, self.N + 1):
             for i in range(self.n):
                 xc_temp = []
                 for j in range(self.n):
                     if self.Adj[i, j] == 1:
                         xc_temp.append(x_temp[j][:, [k - 1]])
-                x_temp[i][:, [k]] = self.agents[i].next_state(
+                next_state = self.agents[i].next_state(
                     x_temp[i][:, [k - 1]], u[i][:, [k - 1]], xc_temp
                 )
+                if next_state is None:
+                    return None
+                else:
+                    x_temp[i][:, [k]] = next_state
         return x_temp
 
-    def plot_admm_iters(self, u_list, z_list, x_list, x_back_list, switch_list):
-        t = 1
+    def plot_admm_iters(self, u_list, z_list, x_list, x_full_list, switch_list):
+        plt.rc("text", usetex=True)
+        plt.rc("font", size=14)
+        plt.style.use("bmh")
 
+        t = 0
         _, u_axs = plt.subplots(self.n, 1, constrained_layout=True, sharex=True)
-        _, res_axs = plt.subplots(self.n, 1, constrained_layout=True, sharex=True)
         for i in range(len(u_list)):
             u_axs[i].plot([u_list[i][k][:, t] for k in range(len(u_list[i]))])
             u_axs[i].plot(
-                switch_list[i], [u_list[i][k][0, t] for k in switch_list[i]], "o"
+                switch_list[i],
+                [u_list[i][k][0, t] for k in switch_list[i]],
+                "o",
+                markersize=3,
             )
-            u_axs[i].set_ylabel(f"u {i}")
-            u_axs[i].set_xlabel("admm iter")
-            # self.u_axs[i].set_ylim((-1, 1))
-
-        t = 1
-        _, axs = plt.subplots(1, 1, constrained_layout=True, sharex=True)
-        axs.plot([x_list[2][k][0, t] for k in range(len(u_list[i]))])
-        axs.plot([x_back_list[1][k][0, t] for k in range(len(u_list[i]))])
-        # axs.plot([z_list[2][k][0, t] for k in range(len(u_list[i]))])
-        # for i in range(len(z_list)):
-        #   axs[i].plot([x_list[i][k][1, t] for k in range(len(u_list[i]))])
-        #   if i != 0:
-        #       axs[i].plot(
-        #           [x_back_list[i - 1][k][1, t] for k in range(len(u_list[i]))]
-        #       )
-
-        for i in range(len(z_list)):
-            # res_axs[i].plot(
-            #    [x_list[i][k][1, t] for k in range(len(u_list[i]))]
-            # )
-            res_axs[i].plot(
-                [x_list[i][k][1, t] - z_list[i][k][1, t] for k in range(len(u_list[i]))]
-            )
-            # res_axs[i].plot(
-            #    switch_list[i],
-            #    [x_list[i][k][1, t] - z_list[i][k][1, t] for k in switch_list[i]],
-            #    "o",
-            # )
-            res_axs[i].set_ylabel(f"residual {i}")
-            res_axs[i].set_xlabel("admm iter")
-            # self.res_axs[i].set_ylim((-1, 1))
+            u_axs[i].set_ylabel(f"$u_{i}({t})$")
+        u_axs[i].set_xlabel(r"$\tau$")
+        save2tikz(plt.gcf())
+
+        _, res_axs = plt.subplots(1, 1, constrained_layout=True, sharex=True)
+        res = []
+        for tau in range(len(u_list[i])):
+            res.append(0.0)
+            for i in range(self.n):
+                for j in range(len(self.G[i])):
+                    for k in range(self.N + 1):
+                        res[tau] += np.linalg.norm(
+                            x_full_list[i][tau][
+                                j * self.nx_l : (j + 1) * self.nx_l, [k]
+                            ]
+                            - z_list[self.G[i][j]][tau][:, [k]]
+                        )
+        res_axs.plot(res)
+        res_axs.set_ylabel(f"$r$")
+        res_axs.set_xlabel(r"$\tau$")
+        save2tikz(plt.gcf())
+
+        print(f"Final residaul = {res[-1]}")
         plt.show()
```

### Comparing `dmpcpwa-0.0.1/src/dmpcpwa/agents/mld_agent.py` & `dmpcpwa-0.0.2/src/dmpcpwa/agents/mld_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import numpy as np
 from csnlp.util.io import SupportsDeepcopyAndPickle
 from gymnasium import Env
 from mpcrl import Agent
 from mpcrl.core.callbacks import AgentCallbackMixin
 from mpcrl.core.exploration import ExplorationStrategy, NoExploration
 from mpcrl.util.named import Named
+from mpcrl.core.warmstart import WarmStartStrategy
 
 from dmpcpwa.mpc.mpc_mld import MpcMld
 
 
 class MldAgent(Agent):
     """A pwa agent who uses an mld controller."""
 
@@ -23,15 +24,19 @@
         this agent uses an mpc that does not inheret from the MPC baseclass."""
 
         # this below is just to keep this class compatible with Agent init
         Named.__init__(self, None)
         SupportsDeepcopyAndPickle.__init__(self)
         AgentCallbackMixin.__init__(self)
         self._fixed_pars = None
+
+        # these params are just for compatibility with Agent class
         self._exploration: ExplorationStrategy = NoExploration()
+        self._warmstart = WarmStartStrategy("last")
+
         self._store_last_successful = True
         self._last_action_on_fail = False
         self._last_solution = None
         self._last_action = None
 
         self.mpc = mpc
         self.x_pred = None  # stores most recent predicted state after being solved
@@ -85,15 +90,14 @@
             state, _ = env.reset(seed=current_seed, options=env_reset_options)
             truncated, terminated, timestep = False, False, 0
             self.on_episode_start(env, episode, state)
 
             while not (truncated or terminated):
                 # changed origonal agents evaluate here to use the mld mpc
                 action = self.get_control(state)
-                action = cs.DM(action)
 
                 state, r, truncated, terminated, _ = env.step(action)
                 self.on_env_step(env, episode, timestep)
 
                 returns[episode] += r
                 timestep += 1
                 self.on_timestep_end(env, episode, timestep)
```

### Comparing `dmpcpwa-0.0.1/src/dmpcpwa/agents/no_control_agent.py` & `dmpcpwa-0.0.2/src/dmpcpwa/agents/no_control_agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from typing import Any
 
 import casadi as cs
 import numpy as np
 from gymnasium import Env
 from mpcrl import Agent
-from mpcrl.core.exploration import ExplorationStrategy, NoExploration
 
 
 class NoControlAgent(Agent):
     """An agent who uses zero control input."""
 
-    def __init__(self, nu: int) -> None:
+    def __init__(self, nu: int, mpc) -> None:
         """Initialise the no control agent with control dimension nu."""
-        self._exploration: ExplorationStrategy = NoExploration()  # to keep compatable
         self.nu = nu
 
+        # to keep compatible
+        super().__init__(mpc, {}, "last-succesful", None)
+
     def evaluate(
         self,
         env: Env,
         episodes: int,
         deterministic: bool = True,
         seed: int = None,
         raises: bool = True,
@@ -52,15 +53,15 @@
         self.on_validation_start(env)
         seeds = map(int, np.random.SeedSequence(seed).generate_state(episodes))
 
         for episode, current_seed in zip(range(episodes), seeds):
             self.reset(current_seed)
             state, _ = env.reset(seed=current_seed, options=env_reset_options)
             truncated, terminated, timestep = False, False, 0
-            self.on_episode_start(env, episode)
+            self.on_episode_start(env, episode, state)
 
             while not (truncated or terminated):
                 # changed origonal agents evaluate here not control
                 action = np.zeros((self.nu, 1))
                 action = cs.DM(action)
 
                 state, r, truncated, terminated, _ = env.step(action)
```

### Comparing `dmpcpwa-0.0.1/src/dmpcpwa/agents/sqp_admm_coordinator.py` & `dmpcpwa-0.0.2/src/dmpcpwa/agents/sqp_admm_coordinator.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 import casadi as cs
 import numpy as np
 from dmpcrl.core.admm import AdmmCoordinator
 from dmpcrl.mpc.mpc_admm import MpcAdmm
 from gymnasium import Env
 from mpcrl import Agent
-from mpcrl.agents.agent import ActType, ObsType
 
 from dmpcpwa.agents.pwa_agent import PwaAgent
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 console_handler = logging.StreamHandler()
 console_handler.setLevel(logging.DEBUG)
@@ -83,15 +82,15 @@
             self.nu_l,
             rho,
             iters=self.admm_iters,
         )
 
     def evaluate(
         self,
-        env: Env[ObsType, ActType],
+        env: Env,
         episodes: int,
         deterministic: bool = True,
         seed: int = None,
         raises: bool = True,
         env_reset_options: dict[str, Any] = None,
     ):
         returns = np.zeros(episodes)
```

### Comparing `dmpcpwa-0.0.1/src/dmpcpwa/mpc/mpc_mld.py` & `dmpcpwa-0.0.2/src/dmpcpwa/mpc/mpc_mld.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 console_handler.setFormatter(formatter)
 logger.addHandler(console_handler)
 
 
 class MpcMld:
     """An MPC that converts a PWA mpc problem into a MIP."""
 
-    def __init__(self, system: dict, N: int, verbose=False) -> None:
+    def __init__(self, system: dict, N: int, verbose=False, thread_limit: int | None = None, constrain_first_state: bool = True) -> None:
         """Instantiate the mld based mpc. In the constructor pwa system is converted
         to mld and the associated dynamics and constraints are created, along with states
         and control variables.
 
         Parameters
         ----------
         system: dict
@@ -33,43 +33,46 @@
         m = system["B"][0].shape[1]
 
         # build mld model
 
         mpc_model = gp.Model("mld_mpc")
         mpc_model.setParam("OutputFlag", verbose)
         mpc_model.setParam("Heuristics", 0)
+        # mpc_model.setParam('FeasibilityTol', 1e-3)
+        if thread_limit is not None:
+            mpc_model.params.threads = thread_limit
         # mpc_model.setParam("MIPStart", 1)  # using warm-starting from previous sol
 
         # Uncomment if you need to differentiate between infeasbile and unbounded
-        mpc_model.setParam("DualReductions", 0)
+        # mpc_model.setParam("DualReductions", 0)
 
         x = mpc_model.addMVar(
             (n, N + 1), lb=-float("inf"), ub=float("inf"), name="x"
         )  # state
         u = mpc_model.addMVar(
             (m, N), lb=-float("inf"), ub=float("inf"), name="u"
         )  # control
 
         # create MLD dynamics from PWA
-        self.create_MLD_dynamics_and_constraints(system, mpc_model, x, u, N)
+        self.create_MLD_dynamics_and_constraints(system, mpc_model, x, u, N, constrain_first_state=constrain_first_state)
 
         # IC constraint - gets updated everytime solve_mpc is called
         self.IC = mpc_model.addConstr(x[:, [0]] == np.zeros((n, 1)), name="IC")
 
         # assign parts of model to be used by class later
         self.mpc_model = mpc_model
         self.x = x
         self.u = u
         self.n = n
         self.m = m
         self.N = N
 
         logger.critical("MLD MPC setup complete.")
 
-    def create_MLD_dynamics_and_constraints(self, system, mpc_model, x, u, N):
+    def create_MLD_dynamics_and_constraints(self, system, mpc_model, x, u, N, constrain_first_state: bool = True):
         # extract values from system
         S = system["S"]
         R = system["R"]
         T = system["T"]
         A = system["A"]
         B = system["B"]
         c = system["c"]
@@ -149,15 +152,16 @@
             for i in range(s):
                 # delta[i, k].setAttr('BranchPriority', s*N - s*k - i)
                 # delta[i, k].setAttr('BranchPriority', N-k)
                 pass
 
             # add state and input constraints to model, then binary and auxillary constraint, then dynamics constraints
 
-            mpc_model.addConstr(D @ x[:, [k]] <= E, name="state constraints")
+            if k > 0 or (k == 0 and constrain_first_state):
+                mpc_model.addConstr(D @ x[:, [k]] <= E, name="state constraints")
             mpc_model.addConstr(F @ u[:, [k]] <= G, name=f"control constraints_{k}")
 
             mpc_model.addConstrs(
                 (
                     S[i] @ x[:, [k]] + R[i] @ u[:, [k]] - T[i]
                     <= M_st[i] * (1 - delta[i, [k]])
                     for i in range(s)
@@ -256,34 +260,44 @@
             self.mpc_model.addConstr(x[i, :] <= y[i, :], name="dumb_leq")
             self.mpc_model.addConstr(-x[i, :] <= y[i, :], name="dumb_geq")
         self.mpc_model.addConstr(sum(y[i, :] for i in range(n)) == t, name="dumb_eq")
         return t
 
     def min_2_norm(self, x, Q):
         """return the term x'@Q@x."""
-        # I have to do the tranpose part manually because gurobi does not support
+        # handle the zero matrix case individually as Gurobi is wierd with it
+        if not Q.any(): 
+            return 0
+        
+        # have to do the tranpose part manually because gurobi does not support
         # taking the transpose of an Expr
-        if x.shape[1] > 1:
-            raise RuntimeError("x must be a columb vector.")
         n = x.shape[0]
         M = Q @ x
         return sum(x[i] * M[i] for i in range(n))
 
     def solve_mpc(self, state):
         self.IC.RHS = state
         self.mpc_model.optimize()
         if self.mpc_model.Status == 2:  # check for successful solve
             u = self.u.X
             x = self.x.X
             cost = self.mpc_model.objVal
         else:
-            u = np.zeros((self.m, self.N))
-            x = np.zeros(self.x.shape)
-            cost = float("inf")
-            logger.info("Infeasible")
+            # turn off presolve and try again
+            self.mpc_model.setParam('Presolve', 0)
+            self.mpc_model.reset()
+            self.mpc_model.optimize()  
+            if self.mpc_model.Status == 2:  # check for successful solve
+                u = self.u.X
+                x = self.x.X
+                cost = self.mpc_model.objVal
+                self.mpc_model.setParam('Presolve', 1)
+            else:   
+                logger.info("Infeasible")
+                raise RuntimeError(f'Infeasible problem!')
 
         run_time = self.mpc_model.Runtime
         nodes = self.mpc_model.NodeCount
         try:
             bin_vars = self.mpc_model.presolve().NumBinVars
         except:
             bin_vars = 0
```

### Comparing `dmpcpwa-0.0.1/src/dmpcpwa/mpc/mpc_mld_cent_decup.py` & `dmpcpwa-0.0.2/src/dmpcpwa/mpc/mpc_mld_cent_decup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 logger.addHandler(console_handler)
 
 
 class MpcMldCentDecup(MpcMld):
     """ "An mpc that converts the networked PWA mpc problem to MLD form.
     The PWA systems are assumed decoupled in the dynamics."""
 
-    def __init__(self, systems: list[dict], n: int, N: int, verbose=False) -> None:
+    def __init__(self, systems: list[dict], n: int, N: int, verbose=False, thread_limit: int | None = None, constrain_first_state = True) -> None:
         """Instantiate the mpc.
 
         Parameters
         ----------
         system: List[dict]
             List of dictionary which contain the definitions of the PWA systems {S, R, T, A, B, c, D, E, F, G}.
              When S[i]x+R[x]u <= T[i] -> x+ = A[i]x + B[i]u + c[i].
@@ -36,38 +36,40 @@
         nu_l = systems[0]["B"][0].shape[1]
 
         # build mld model
 
         mpc_model = gp.Model("mld_mpc")
         mpc_model.setParam("OutputFlag", verbose)
         mpc_model.setParam("Heuristics", 0)
-        # mpc_model.setParam("MIPStart", 1)  # using warm-starting from previous sol
+        # mpc_model.setParam("Presolve", 0)
+        # mpc_model.setParam('FeasibilityTol', 1e-3)
+        if thread_limit is not None:
+            mpc_model.params.threads = thread_limit
 
         # Uncomment if you need to differentiate between infeasbile and unbounded
-        mpc_model.setParam("DualReductions", 0)
+        # mpc_model.setParam("DualReductions", 0)
 
         x = mpc_model.addMVar(
             (n * nx_l, N + 1), lb=-float("inf"), ub=float("inf"), name="x"
         )  # state
         u = mpc_model.addMVar(
             (n * nu_l, N), lb=-float("inf"), ub=float("inf"), name="u"
         )  # control
 
         for i in range(n):
             # pull out local parts for agent i
             x_l = x[nx_l * i : nx_l * (i + 1), :]
             u_l = u[nu_l * i : nu_l * (i + 1), :]
 
-            self.create_MLD_dynamics_and_constraints(systems[i], mpc_model, x_l, u_l, N)
+            self.create_MLD_dynamics_and_constraints(systems[i], mpc_model, x_l, u_l, N, constrain_first_state=constrain_first_state)
 
         # IC constraint - gets updated everytime solve_mpc is called
         self.IC = mpc_model.addConstr(x[:, [0]] == np.zeros((n * nx_l, 1)), name="IC")
 
         # assign parts of model to be used by class later
         self.mpc_model = mpc_model
         self.x = x
         self.u = u
-        # self.n = n * nx_l
         self.m = n * nu_l
         self.N = N
 
         logger.critical("MLD MPC setup complete.")
```

### Comparing `dmpcpwa-0.0.1/src/dmpcpwa/mpc/mpc_switching.py` & `dmpcpwa-0.0.2/src/dmpcpwa/mpc/mpc_switching.py`

 * *Files identical despite different names*

### Comparing `dmpcpwa-0.0.1/src/dmpcpwa/utils/pwa_models.py` & `dmpcpwa-0.0.2/src/dmpcpwa/utils/pwa_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,17 +50,17 @@
 
         A_diag = block_diag(*A_tmp)
         # add coupling to A
         for i in range(n):
             coupling_idx = 0  # keep track of which Ac_i_j corresponds to Adj[i, j]
             for j in range(n):
                 if Adj[i, j] == 1:
-                    A_diag[
-                        nx_l * i : nx_l * (i + 1), nx_l * j : nx_l * (j + 1)
-                    ] = d_systems[i]["Ac"][idxs[i]][coupling_idx]
+                    A_diag[nx_l * i : nx_l * (i + 1), nx_l * j : nx_l * (j + 1)] = (
+                        d_systems[i]["Ac"][idxs[i]][coupling_idx]
+                    )
                     coupling_idx += 1
 
         S.append(block_diag(*S_tmp))
         R.append(block_diag(*R_tmp))
         T.append(np.vstack(T_tmp))
         A.append(A_diag)
         B.append(block_diag(*B_tmp))
```

### Comparing `dmpcpwa-0.0.1/src/dmpcpwa/utils/tikz.py` & `dmpcpwa-0.0.2/src/dmpcpwa/utils/tikz.py`

 * *Files identical despite different names*

### Comparing `dmpcpwa-0.0.1/src/dmpcpwa.egg-info/PKG-INFO` & `dmpcpwa-0.0.2/src/dmpcpwa.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmpcpwa
-Version: 0.0.1
+Version: 0.0.2
 Summary: Distributed Model Predictive Control for Piecewise Affine Systems
 Author-email: Samuel Mallick <sam.mallick.97@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/SamuelMallick/distributed-mpc-pwa
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dmpcpwa-0.0.1/src/dmpcpwa.egg-info/SOURCES.txt` & `dmpcpwa-0.0.2/src/dmpcpwa.egg-info/SOURCES.txt`

 * *Files identical despite different names*


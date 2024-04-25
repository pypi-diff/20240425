# Comparing `tmp/chainbench-0.6.7.tar.gz` & `tmp/chainbench-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainbench-0.6.7.tar", max compression
+gzip compressed data, was "chainbench-0.6.8.tar", max compression
```

## Comparing `chainbench-0.6.7.tar` & `chainbench-0.6.8.tar`

### file list

```diff
@@ -1,51 +1,53 @@
--rw-r--r--   0        0        0    11357 2024-04-23 09:37:04.066810 chainbench-0.6.7/LICENSE
--rw-r--r--   0        0        0    12165 2024-04-23 09:37:04.066810 chainbench-0.6.7/README.md
--rw-r--r--   0        0        0        0 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/__init__.py
--rw-r--r--   0        0        0       39 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/__main__.py
--rw-r--r--   0        0        0    15103 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/main.py
--rw-r--r--   0        0        0        0 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/__init__.py
--rw-r--r--   0        0        0     3732 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/avalanche/general.py
--rw-r--r--   0        0        0     2760 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/bsc/general.py
--rw-r--r--   0        0        0     1158 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/ethereum/consensus.py
--rw-r--r--   0        0        0     2776 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/ethereum/general.py
--rw-r--r--   0        0        0      344 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/evm/all.py
--rw-r--r--   0        0        0     1272 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/evm/debug_trace.py
--rw-r--r--   0        0        0      427 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/evm/get_logs.py
--rw-r--r--   0        0        0     4252 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/evm/heavy.py
--rw-r--r--   0        0        0     1655 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/evm/light.py
--rw-r--r--   0        0        0     1931 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/oasis/general.py
--rw-r--r--   0        0        0     2897 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/polygon/general.py
--rw-r--r--   0        0        0     3514 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/solana/general.py
--rw-r--r--   0        0        0     2223 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/profile/starknet/wallet.py
--rw-r--r--   0        0        0      599 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/test_data/__init__.py
--rw-r--r--   0        0        0     6482 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/test_data/blockchain.py
--rw-r--r--   0        0        0     5934 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/test_data/ethereum.py
--rw-r--r--   0        0        0    18785 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/test_data/evm.py
--rw-r--r--   0        0        0     5443 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/test_data/solana.py
--rw-r--r--   0        0        0     2284 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/test_data/starknet.py
--rw-r--r--   0        0        0       24 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/tools/__init__.py
--rw-r--r--   0        0        0       18 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/tools/discovery/__init__.py
--rw-r--r--   0        0        0      977 2024-04-23 09:37:04.066810 chainbench-0.6.7/chainbench/tools/discovery/clients.json
--rw-r--r--   0        0        0    55080 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/tools/discovery/methods.json
--rw-r--r--   0        0        0     5499 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/tools/discovery/rpc.py
--rw-r--r--   0        0        0      416 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/user/__init__.py
--rw-r--r--   0        0        0     2895 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/user/ethereum.py
--rw-r--r--   0        0        0     4622 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/user/evm.py
--rw-r--r--   0        0        0     4672 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/user/http.py
--rw-r--r--   0        0        0      799 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/user/methods/__init__.py
--rw-r--r--   0        0        0      516 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/user/methods/common.py
--rw-r--r--   0        0        0     9082 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/user/methods/ethereum.py
--rw-r--r--   0        0        0    10003 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/user/methods/evm.py
--rw-r--r--   0        0        0     2885 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/user/solana.py
--rw-r--r--   0        0        0     3680 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/user/starknet.py
--rw-r--r--   0        0        0        0 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/util/__init__.py
--rw-r--r--   0        0        0     6218 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/util/cli.py
--rw-r--r--   0        0        0    12953 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/util/event.py
--rw-r--r--   0        0        0     5766 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/util/http.py
--rw-r--r--   0        0        0     2419 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/util/monitor.py
--rw-r--r--   0        0        0     3453 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/util/notify.py
--rw-r--r--   0        0        0      870 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/util/rng.py
--rw-r--r--   0        0        0      337 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/util/rpc.py
--rw-r--r--   0        0        0      455 2024-04-23 09:37:04.070809 chainbench-0.6.7/chainbench/util/timer.py
--rw-r--r--   0        0        0      953 2024-04-23 09:37:04.070809 chainbench-0.6.7/pyproject.toml
--rw-r--r--   0        0        0    12756 1970-01-01 00:00:00.000000 chainbench-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-25 15:53:11.052962 chainbench-0.6.8/LICENSE
+-rw-r--r--   0        0        0    12165 2024-04-25 15:53:11.052962 chainbench-0.6.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-25 15:53:11.052962 chainbench-0.6.8/chainbench/__init__.py
+-rw-r--r--   0        0        0       39 2024-04-25 15:53:11.052962 chainbench-0.6.8/chainbench/__main__.py
+-rw-r--r--   0        0        0    15103 2024-04-25 15:53:11.052962 chainbench-0.6.8/chainbench/main.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:53:11.052962 chainbench-0.6.8/chainbench/profile/__init__.py
+-rw-r--r--   0        0        0     3732 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/avalanche/general.py
+-rw-r--r--   0        0        0     2760 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/bsc/general.py
+-rw-r--r--   0        0        0     1158 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/ethereum/consensus.py
+-rw-r--r--   0        0        0     2776 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/ethereum/general.py
+-rw-r--r--   0        0        0      344 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/evm/all.py
+-rw-r--r--   0        0        0     1272 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/evm/debug_trace.py
+-rw-r--r--   0        0        0      427 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/evm/get_logs.py
+-rw-r--r--   0        0        0     4252 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/evm/heavy.py
+-rw-r--r--   0        0        0     1655 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/evm/light.py
+-rw-r--r--   0        0        0     1931 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/oasis/general.py
+-rw-r--r--   0        0        0     2897 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/polygon/general.py
+-rw-r--r--   0        0        0      366 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/solana/all.py
+-rw-r--r--   0        0        0     1415 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/solana/general.py
+-rw-r--r--   0        0        0     2223 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/starknet/wallet.py
+-rw-r--r--   0        0        0      599 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/test_data/__init__.py
+-rw-r--r--   0        0        0     6482 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/test_data/blockchain.py
+-rw-r--r--   0        0        0     5934 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/test_data/ethereum.py
+-rw-r--r--   0        0        0    18785 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/test_data/evm.py
+-rw-r--r--   0        0        0     6037 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/test_data/solana.py
+-rw-r--r--   0        0        0     2284 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/test_data/starknet.py
+-rw-r--r--   0        0        0       24 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/tools/__init__.py
+-rw-r--r--   0        0        0       18 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/tools/discovery/__init__.py
+-rw-r--r--   0        0        0      977 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/tools/discovery/clients.json
+-rw-r--r--   0        0        0    55080 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/tools/discovery/methods.json
+-rw-r--r--   0        0        0     5499 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/tools/discovery/rpc.py
+-rw-r--r--   0        0        0      416 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/user/__init__.py
+-rw-r--r--   0        0        0     2895 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/user/ethereum.py
+-rw-r--r--   0        0        0     4622 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/user/evm.py
+-rw-r--r--   0        0        0     5252 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/user/http.py
+-rw-r--r--   0        0        0      889 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/user/methods/__init__.py
+-rw-r--r--   0        0        0      516 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/user/methods/common.py
+-rw-r--r--   0        0        0     9082 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/user/methods/ethereum.py
+-rw-r--r--   0        0        0    10003 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/user/methods/evm.py
+-rw-r--r--   0        0        0     9421 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/user/methods/solana.py
+-rw-r--r--   0        0        0     7242 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/user/solana.py
+-rw-r--r--   0        0        0     3680 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/user/starknet.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/util/__init__.py
+-rw-r--r--   0        0        0     6218 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/util/cli.py
+-rw-r--r--   0        0        0    12953 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/util/event.py
+-rw-r--r--   0        0        0     5766 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/util/http.py
+-rw-r--r--   0        0        0     2419 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/util/monitor.py
+-rw-r--r--   0        0        0     3453 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/util/notify.py
+-rw-r--r--   0        0        0      870 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/util/rng.py
+-rw-r--r--   0        0        0      337 2024-04-25 15:53:11.060962 chainbench-0.6.8/chainbench/util/rpc.py
+-rw-r--r--   0        0        0      455 2024-04-25 15:53:11.060962 chainbench-0.6.8/chainbench/util/timer.py
+-rw-r--r--   0        0        0      991 2024-04-25 15:53:11.060962 chainbench-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0    12837 1970-01-01 00:00:00.000000 chainbench-0.6.8/PKG-INFO
```

### Comparing `chainbench-0.6.7/LICENSE` & `chainbench-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/README.md` & `chainbench-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/main.py` & `chainbench-0.6.8/chainbench/main.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/profile/avalanche/general.py` & `chainbench-0.6.8/chainbench/profile/avalanche/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/profile/bsc/general.py` & `chainbench-0.6.8/chainbench/profile/bsc/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/profile/ethereum/consensus.py` & `chainbench-0.6.8/chainbench/profile/ethereum/consensus.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/profile/ethereum/general.py` & `chainbench-0.6.8/chainbench/profile/ethereum/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/profile/evm/debug_trace.py` & `chainbench-0.6.8/chainbench/profile/evm/debug_trace.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/profile/evm/heavy.py` & `chainbench-0.6.8/chainbench/profile/evm/heavy.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/profile/evm/light.py` & `chainbench-0.6.8/chainbench/profile/evm/light.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/profile/oasis/general.py` & `chainbench-0.6.8/chainbench/profile/oasis/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/profile/polygon/general.py` & `chainbench-0.6.8/chainbench/profile/polygon/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/profile/starknet/wallet.py` & `chainbench-0.6.8/chainbench/profile/starknet/wallet.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/test_data/__init__.py` & `chainbench-0.6.8/chainbench/test_data/__init__.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/test_data/blockchain.py` & `chainbench-0.6.8/chainbench/test_data/blockchain.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/test_data/ethereum.py` & `chainbench-0.6.8/chainbench/test_data/ethereum.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/test_data/evm.py` & `chainbench-0.6.8/chainbench/test_data/evm.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/test_data/solana.py` & `chainbench-0.6.8/chainbench/test_data/solana.py`

 * *Files 8% similar despite different names*

```diff
@@ -147,7 +147,20 @@
             start = rng.random.randint(self.start_block_number, self.end_block_number - n)
             return BlockRange(start, start + n)
 
     def get_random_account(self, rng: RNG | None = None) -> Account:
         if rng is None:
             rng = get_rng()
         return self.get_random_block(rng).get_random_account(rng)
+
+    @staticmethod
+    def get_random_token_address(self, rng: RNG | None = None) -> Account:
+        if rng is None:
+            rng = get_rng()
+        token_addresses = [
+            "z3dn17yLaGMKffVogeFHQ9zWVcXgqgf3PQnDsNs2g6M",  # Oxygen Protocol
+            "2cZv8HrgcWSvC6n1uEiS48cEQGb1d3fiowP2rpa4wBL9",  # ACF Game
+            "5fTwKZP2AK39LtFN9Ayppu6hdCVKfMGVm79F2EgHCtsi",  # WHEYO
+            "NeonTjSjsuo3rexg9o6vHuMXw62f9V7zvmu8M8Zut44",  # Neon EVM
+            "8BMzMi2XxZn9afRaMx5Z6fauk9foHXqV5cLTCYWRcVje",  # Staika
+        ]
+        return rng.random.choice(token_addresses)
```

### Comparing `chainbench-0.6.7/chainbench/test_data/starknet.py` & `chainbench-0.6.8/chainbench/test_data/starknet.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/tools/discovery/clients.json` & `chainbench-0.6.8/chainbench/tools/discovery/clients.json`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/tools/discovery/methods.json` & `chainbench-0.6.8/chainbench/tools/discovery/methods.json`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/tools/discovery/rpc.py` & `chainbench-0.6.8/chainbench/tools/discovery/rpc.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/user/ethereum.py` & `chainbench-0.6.8/chainbench/user/ethereum.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/user/evm.py` & `chainbench-0.6.8/chainbench/user/evm.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/user/http.py` & `chainbench-0.6.8/chainbench/user/http.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,37 @@
 import logging
 import typing as t
 
-from locust import FastHttpUser
+from locust import FastHttpUser, TaskSet
 from locust.contrib.fasthttp import ResponseContextManager
 
 from chainbench.test_data import TestData
 from chainbench.util.rng import RNGManager
 from chainbench.util.rpc import generate_request
 
 
+def assign_tasks(
+    tasks: dict[t.Callable | TaskSet, int] | list[t.Callable | TaskSet | tuple[t.Callable | TaskSet, int]]
+) -> list[t.Callable | TaskSet]:
+    new_tasks: list[t.Callable | TaskSet] = []
+    if isinstance(tasks, dict):
+        tasks = list(tasks.items())
+
+    if isinstance(tasks, list):
+        for task in tasks:
+            if isinstance(task, tuple):
+                task, count = task
+                for _ in range(count):
+                    new_tasks.append(task)
+            else:
+                new_tasks.append(task)
+
+    return new_tasks
+
+
 class HttpUser(FastHttpUser):
     """Extension of FastHttpUser for Chainbench."""
 
     abstract = True
     test_data: TestData = TestData()
     logger = logging.getLogger(__name__)
     rng = RNGManager()
```

### Comparing `chainbench-0.6.7/chainbench/user/methods/__init__.py` & `chainbench-0.6.8/chainbench/user/methods/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import os
 import sys
 from typing import Type
 
 from .common import get_subclass_functions
 from .ethereum import EthBeaconMethods
 from .evm import EvmMethods
+from .solana import SolanaMethods
 
 __all__ = [
     "EthBeaconMethods",
     "EvmMethods",
+    "SolanaMethods",
     "get_subclass_functions",
     "all_method_classes",
     "all_methods",
 ]
 
 
-all_method_classes: list[Type[EthBeaconMethods | EvmMethods]] = [
+all_method_classes: list[Type[EthBeaconMethods | EvmMethods | SolanaMethods]] = [
     EthBeaconMethods,
     EvmMethods,
+    SolanaMethods,
 ]
 
 
 def _all_methods() -> dict[str, str]:
     method_list = {}
     for method_class in all_method_classes:
         filepath = sys.modules[method_class.__module__].__file__
```

### Comparing `chainbench-0.6.7/chainbench/user/methods/common.py` & `chainbench-0.6.8/chainbench/user/methods/common.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/user/methods/ethereum.py` & `chainbench-0.6.8/chainbench/user/methods/ethereum.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/user/methods/evm.py` & `chainbench-0.6.8/chainbench/user/methods/evm.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/user/starknet.py` & `chainbench-0.6.8/chainbench/user/starknet.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/util/cli.py` & `chainbench-0.6.8/chainbench/util/cli.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/util/event.py` & `chainbench-0.6.8/chainbench/util/event.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/util/http.py` & `chainbench-0.6.8/chainbench/util/http.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/util/monitor.py` & `chainbench-0.6.8/chainbench/util/monitor.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/util/notify.py` & `chainbench-0.6.8/chainbench/util/notify.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/chainbench/util/rng.py` & `chainbench-0.6.8/chainbench/util/rng.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.7/PKG-INFO` & `chainbench-0.6.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: chainbench
-Version: 0.6.7
+Version: 0.6.8
 Summary: 
 Author: Egor Molodik
 Author-email: egor.molodik@chainstack.com
 Maintainer: Erwin Wee
 Maintainer-email: erwin.wee@chainstack.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: base58 (>=2.1.1,<3.0.0)
 Requires-Dist: click (>=8.1.6,<9.0.0)
 Requires-Dist: locust (>=2.24.1,<3.0.0)
 Requires-Dist: locust-plugins[dashboards] (>=4.4.2,<5.0.0)
+Requires-Dist: solders (>=0.21.0,<0.22.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Description-Content-Type: text/markdown
 
 <img width="1200" alt="Labs" src="https://user-images.githubusercontent.com/99700157/213291931-5a822628-5b8a-4768-980d-65f324985d32.png">
 
 <p>
  <h3 align="center">Chainstack is the leading suite of services connecting developers with Web3 infrastructure</h3>
```


# Comparing `tmp/near-lake-framework-0.0.7.tar.gz` & `tmp/near-lake-framework-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "near-lake-framework-0.0.7.tar", last modified: Wed Sep  7 02:48:38 2022, max compression
+gzip compressed data, was "near-lake-framework-0.0.8.tar", last modified: Thu Apr 25 16:56:08 2024, max compression
```

## Comparing `near-lake-framework-0.0.7.tar` & `near-lake-framework-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 frolik     (501) staff       (20)        0 2022-09-07 02:48:38.538214 near-lake-framework-0.0.7/
--rw-r--r--   0 frolik     (501) staff       (20)     9722 2022-08-18 13:14:08.000000 near-lake-framework-0.0.7/LICENSE-APACHE
--rw-r--r--   0 frolik     (501) staff       (20)     5243 2022-09-07 02:48:38.538294 near-lake-framework-0.0.7/PKG-INFO
--rw-r--r--   0 frolik     (501) staff       (20)     3774 2022-09-06 00:29:34.000000 near-lake-framework-0.0.7/README.md
--rw-r--r--   0 frolik     (501) staff       (20)      110 2022-09-07 02:48:38.538518 near-lake-framework-0.0.7/setup.cfg
--rw-r--r--   0 frolik     (501) staff       (20)     1081 2022-09-07 02:48:33.000000 near-lake-framework-0.0.7/setup.py
-drwxr-xr-x   0 frolik     (501) staff       (20)        0 2022-09-07 02:48:38.536774 near-lake-framework-0.0.7/src/
-drwxr-xr-x   0 frolik     (501) staff       (20)        0 2022-09-07 02:48:38.537575 near-lake-framework-0.0.7/src/near_lake_framework/
--rw-r--r--   0 frolik     (501) staff       (20)     4099 2022-09-06 22:20:23.000000 near-lake-framework-0.0.7/src/near_lake_framework/__init__.py
--rw-r--r--   0 frolik     (501) staff       (20)     4865 2022-09-07 02:45:23.000000 near-lake-framework-0.0.7/src/near_lake_framework/near_primitives.py
--rw-r--r--   0 frolik     (501) staff       (20)     2061 2022-09-06 00:09:28.000000 near-lake-framework-0.0.7/src/near_lake_framework/s3_fetchers.py
-drwxr-xr-x   0 frolik     (501) staff       (20)        0 2022-09-07 02:48:38.538121 near-lake-framework-0.0.7/src/near_lake_framework.egg-info/
--rw-r--r--   0 frolik     (501) staff       (20)     5243 2022-09-07 02:48:38.000000 near-lake-framework-0.0.7/src/near_lake_framework.egg-info/PKG-INFO
--rw-r--r--   0 frolik     (501) staff       (20)      395 2022-09-07 02:48:38.000000 near-lake-framework-0.0.7/src/near_lake_framework.egg-info/SOURCES.txt
--rw-r--r--   0 frolik     (501) staff       (20)        1 2022-09-07 02:48:38.000000 near-lake-framework-0.0.7/src/near_lake_framework.egg-info/dependency_links.txt
--rw-r--r--   0 frolik     (501) staff       (20)       75 2022-09-07 02:48:38.000000 near-lake-framework-0.0.7/src/near_lake_framework.egg-info/requires.txt
--rw-r--r--   0 frolik     (501) staff       (20)       20 2022-09-07 02:48:38.000000 near-lake-framework-0.0.7/src/near_lake_framework.egg-info/top_level.txt
+drwxr-xr-x   0 frolik     (501) staff       (20)        0 2024-04-25 16:56:08.446586 near-lake-framework-0.0.8/
+-rw-r--r--   0 frolik     (501) staff       (20)     9722 2023-10-15 22:01:13.000000 near-lake-framework-0.0.8/LICENSE-APACHE
+-rw-r--r--   0 frolik     (501) staff       (20)     4617 2024-04-25 16:56:08.446505 near-lake-framework-0.0.8/PKG-INFO
+-rw-r--r--   0 frolik     (501) staff       (20)     3840 2024-04-25 16:42:44.000000 near-lake-framework-0.0.8/README.md
+-rw-r--r--   0 frolik     (501) staff       (20)      110 2024-04-25 16:56:08.446958 near-lake-framework-0.0.8/setup.cfg
+-rw-r--r--   0 frolik     (501) staff       (20)     1139 2024-04-25 16:39:59.000000 near-lake-framework-0.0.8/setup.py
+drwxr-xr-x   0 frolik     (501) staff       (20)        0 2024-04-25 16:56:08.442794 near-lake-framework-0.0.8/src/
+drwxr-xr-x   0 frolik     (501) staff       (20)        0 2024-04-25 16:56:08.444902 near-lake-framework-0.0.8/src/near_lake_framework/
+-rw-r--r--   0 frolik     (501) staff       (20)     4884 2024-04-25 16:39:35.000000 near-lake-framework-0.0.8/src/near_lake_framework/__init__.py
+-rw-r--r--   0 frolik     (501) staff       (20)     4879 2023-10-15 22:01:13.000000 near-lake-framework-0.0.8/src/near_lake_framework/near_primitives.py
+-rw-r--r--   0 frolik     (501) staff       (20)        0 2024-04-25 16:39:35.000000 near-lake-framework-0.0.8/src/near_lake_framework/py.typed
+-rw-r--r--   0 frolik     (501) staff       (20)     2431 2024-04-25 16:53:20.000000 near-lake-framework-0.0.8/src/near_lake_framework/s3_fetchers.py
+drwxr-xr-x   0 frolik     (501) staff       (20)        0 2024-04-25 16:56:08.446211 near-lake-framework-0.0.8/src/near_lake_framework.egg-info/
+-rw-r--r--   0 frolik     (501) staff       (20)     4617 2024-04-25 16:56:08.000000 near-lake-framework-0.0.8/src/near_lake_framework.egg-info/PKG-INFO
+-rw-r--r--   0 frolik     (501) staff       (20)      428 2024-04-25 16:56:08.000000 near-lake-framework-0.0.8/src/near_lake_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 frolik     (501) staff       (20)        1 2024-04-25 16:56:08.000000 near-lake-framework-0.0.8/src/near_lake_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 frolik     (501) staff       (20)       75 2024-04-25 16:56:08.000000 near-lake-framework-0.0.8/src/near_lake_framework.egg-info/requires.txt
+-rw-r--r--   0 frolik     (501) staff       (20)       20 2024-04-25 16:56:08.000000 near-lake-framework-0.0.8/src/near_lake_framework.egg-info/top_level.txt
```

### Comparing `near-lake-framework-0.0.7/LICENSE-APACHE` & `near-lake-framework-0.0.8/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `near-lake-framework-0.0.7/PKG-INFO` & `near-lake-framework-0.0.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,118 +1,124 @@
 Metadata-Version: 2.1
 Name: near-lake-framework
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python Library to connect to the NEAR Lake S3 and stream the data
 Home-page: https://github.com/frolvanya/near-lake-framework-py
 Author: Ivan Frolov
 Author-email: frolvanya@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/frolvanya/near-lake-framework-py/issues
-Description: # NEAR Lake Framework for Python
-        
-        Available in programming languages: [Rust](https://github.com/near/near-lake-framework-rs) | [Javascript](https://github.com/near/near-lake-framework-js) | **Python3**
-        
-        NEAR Lake Framework is a small library companion to [NEAR Lake](https://github.com/near/near-lake). It allows you to build
-        your own indexer that subscribes to the stream of blocks from the NEAR Lake data source and create your own logic to process
-        the NEAR Protocol data.
-        
-        [![PyPI version](https://badge.fury.io/py/near-lake-framework.svg)](https://badge.fury.io/py/near-lake-framework)
-        ![MIT or Apache 2.0 licensed](https://img.shields.io/crates/l/near-lake-framework.svg)
-        
-        ---
-        
-        [Official NEAR Lake Framework launch announcement](https://gov.near.org/t/announcement-near-lake-framework-brand-new-word-in-indexer-building-approach/17668) has been published on the NEAR Gov Forum
-        Greetings from the Data Platform Team! We are happy and proud to announce an MVP release of a brand new word in indexer building approach - NEAR Lake Framework.
-        
-        ---
-        
-        ## Example
-        
-        ```python3
-        import asyncio
-        import os
-        
-        from near_lake_framework import LakeConfig, streamer
-        
-        
-        async def main():
-            config = LakeConfig.mainnet()
-            config.start_block_height = 69130938
-            config.aws_access_key_id = os.getenv("AWS_ACCESS_KEY_ID")
-            config.aws_secret_key = os.getenv("AWS_SECRET_ACCESS_KEY")
-        
-            stream_handle, streamer_messages_queue = streamer(config)
-            while True:
-                streamer_message = await streamer_messages_queue.get()
-                print(
-                    f"Received Block #{streamer_message.block.header.height} from Lake Framework"
-                )
-        
-        
-        loop = asyncio.get_event_loop()
-        loop.run_until_complete(main())
-        ```
-        
-        ## How to use
-        
-        ### Dependencies
-        
-        Install `near-lake-framework`
-        
-        ```bash
-        $ pip3 install near-lake-framework
-        ```
-        
-        ### Credentials
-        
-        To be able to access the data from NEAR Lake you need to provide credentials. Please, see the [Credentials article](https://near-indexers.io/tutorials/lake/credentials)
-        
-        ## Configuration
-        
-        Everything should be configured before the start of your indexer application via `LakeConfig` struct.
-        
-        Available parameters:
-        
-        - `s3_bucket_name: str` - provide the AWS S3 bucket name (`near-lake-testnet`, `near-lake-mainnet` or yours if you run your own NEAR Lake)
-        - `s3_region_name: str` - provide the region for AWS S3 bucket
-        - `start_block_height: BlockHeight` - block height to start the stream from
-        - `blocks_preload_pool_size: int` - provide the number of blocks to preload (default: 200)
-        
-        ## Cost estimates
-        
-        **TL;DR** approximately $18.15 per month (for AWS S3 access, paid directly to AWS) for the reading of fresh blocks
-        
-        Explanation:
-        
-        Assuming NEAR Protocol produces accurately 1 block per second (which is really not, the average block production time is 1.3s). A full day consists of 86400 seconds, that's the max number of blocks that can be produced.
-        
-        According the [Amazon S3 prices](https://aws.amazon.com/s3/pricing/?nc1=h_ls) `list` requests are charged for $0.005 per 1000 requests and `get` is charged for $0.0004 per 1000 requests.
-        
-        Calculations (assuming we are following the tip of the network all the time):
-        
-        ```
-        86400 blocks per day * 5 requests for each block / 1000 requests * $0.0004 per 1k requests = $0.173 * 30 days = $5.19
-        ```
-        **Note:** 5 requests for each block means we have 4 shards (1 file for common block data and 4 separate files for each shard)
-        
-        And a number of `list` requests we need to perform for 30 days:
-        
-        ```
-        86400 blocks per day / 1000 requests * $0.005 per 1k list requests = $0.432 * 30 days = $12.96
-        
-        $5.19 + $12.96 = $18.15
-        ```
-        
-        The price depends on the number of shards
-        
-        
-        ### Publishing to PyPi
-        
-        [Follow this guide to safely publish PyPi package](https://widdowquinn.github.io/coding/update-pypi-package/)
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE-APACHE
+Requires-Dist: asyncio>=3.4.3
+Requires-Dist: dataclasses>=0.6
+Requires-Dist: dataclasses-json>=0.5.7
+Requires-Dist: aiobotocore>=2.3.0
+
+# NEAR Lake Framework for Python
+
+Available in programming languages: [Rust](https://github.com/near/near-lake-framework-rs) | [Javascript](https://github.com/near/near-lake-framework-js) | **Python3**
+
+NEAR Lake Framework is a small library companion to [NEAR Lake](https://github.com/near/near-lake). It allows you to build
+your own indexer that subscribes to the stream of blocks from the NEAR Lake data source and create your own logic to process
+the NEAR Protocol data.
+
+[![PyPI version](https://badge.fury.io/py/near-lake-framework.svg)](https://badge.fury.io/py/near-lake-framework)
+![MIT or Apache 2.0 licensed](https://img.shields.io/crates/l/near-lake-framework.svg)
+
+---
+
+[Official NEAR Lake Framework launch announcement](https://gov.near.org/t/announcement-near-lake-framework-brand-new-word-in-indexer-building-approach/17668) has been published on the NEAR Gov Forum
+Greetings from the Data Platform Team! We are happy and proud to announce an MVP release of a brand new word in indexer building approach - NEAR Lake Framework.
+
+---
+
+## Example
+
+```python3
+import asyncio
+import os
+
+from near_lake_framework import LakeConfig, streamer, Network
+
+
+async def main():
+    config = LakeConfig(
+        network=Network.MAINNET,
+        aws_access_key_id=os.getenv("AWS_ACCESS_KEY_ID"),
+        aws_secret_key=os.getenv("AWS_SECRET_ACCESS_KEY"),
+        start_block_height=69130938,
+    )
+
+    stream_handle, streamer_messages_queue = streamer(config)
+    while True:
+        streamer_message = await streamer_messages_queue.get()
+        print(
+            f"Received Block #{streamer_message.block.header.height} from Lake Framework"
+        )
+
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(main())
+```
+
+## How to use
+
+### Dependencies
+
+Install `near-lake-framework`
+
+```bash
+$ pip3 install near-lake-framework
+```
+
+### Credentials
+
+To be able to access the data from NEAR Lake you need to provide credentials. Please, see the [Credentials article](https://near-indexers.io/tutorials/lake/credentials)
+
+## Configuration
+
+Everything should be configured before the start of your indexer application via `LakeConfig` struct.
+
+Available parameters:
+
+- `network: Network` - provide network
+- `s3_bucket_name: str` - provide the AWS S3 bucket name (`near-lake-testnet`, `near-lake-mainnet` or yours if you run your own NEAR Lake)
+- `s3_region_name: str` - provide the region for AWS S3 bucket
+- `start_block_height: BlockHeight` - block height to start the stream from
+- `blocks_preload_pool_size: int` - provide the number of blocks to preload (default: 200)
+
+## Cost estimates
+
+**TL;DR** approximately $18.15 per month (for AWS S3 access, paid directly to AWS) for the reading of fresh blocks
+
+Explanation:
+
+Assuming NEAR Protocol produces accurately 1 block per second (which is really not, the average block production time is 1.3s). A full day consists of 86400 seconds, that's the max number of blocks that can be produced.
+
+According the [Amazon S3 prices](https://aws.amazon.com/s3/pricing/?nc1=h_ls) `list` requests are charged for $0.005 per 1000 requests and `get` is charged for $0.0004 per 1000 requests.
+
+Calculations (assuming we are following the tip of the network all the time):
+
+```
+86400 blocks per day * 5 requests for each block / 1000 requests * $0.0004 per 1k requests = $0.173 * 30 days = $5.19
+```
+**Note:** 5 requests for each block means we have 4 shards (1 file for common block data and 4 separate files for each shard)
+
+And a number of `list` requests we need to perform for 30 days:
+
+```
+86400 blocks per day / 1000 requests * $0.005 per 1k list requests = $0.432 * 30 days = $12.96
+
+$5.19 + $12.96 = $18.15
+```
+
+The price depends on the number of shards
+
+
+### Publishing to PyPi
+
+[Follow this guide to safely publish PyPi package](https://widdowquinn.github.io/coding/update-pypi-package/)
```

### Comparing `near-lake-framework-0.0.7/README.md` & `near-lake-framework-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,22 +18,24 @@
 
 ## Example
 
 ```python3
 import asyncio
 import os
 
-from near_lake_framework import LakeConfig, streamer
+from near_lake_framework import LakeConfig, streamer, Network
 
 
 async def main():
-    config = LakeConfig.mainnet()
-    config.start_block_height = 69130938
-    config.aws_access_key_id = os.getenv("AWS_ACCESS_KEY_ID")
-    config.aws_secret_key = os.getenv("AWS_SECRET_ACCESS_KEY")
+    config = LakeConfig(
+        network=Network.MAINNET,
+        aws_access_key_id=os.getenv("AWS_ACCESS_KEY_ID"),
+        aws_secret_key=os.getenv("AWS_SECRET_ACCESS_KEY"),
+        start_block_height=69130938,
+    )
 
     stream_handle, streamer_messages_queue = streamer(config)
     while True:
         streamer_message = await streamer_messages_queue.get()
         print(
             f"Received Block #{streamer_message.block.header.height} from Lake Framework"
         )
@@ -59,14 +61,15 @@
 
 ## Configuration
 
 Everything should be configured before the start of your indexer application via `LakeConfig` struct.
 
 Available parameters:
 
+- `network: Network` - provide network
 - `s3_bucket_name: str` - provide the AWS S3 bucket name (`near-lake-testnet`, `near-lake-mainnet` or yours if you run your own NEAR Lake)
 - `s3_region_name: str` - provide the region for AWS S3 bucket
 - `start_block_height: BlockHeight` - block height to start the stream from
 - `blocks_preload_pool_size: int` - provide the number of blocks to preload (default: 200)
 
 ## Cost estimates
```

### Comparing `near-lake-framework-0.0.7/setup.py` & `near-lake-framework-0.0.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="near-lake-framework",
-    version="0.0.7",
+    version="0.0.8",
     author="Ivan Frolov",
     author_email="frolvanya@gmail.com",
     description="Python Library to connect to the NEAR Lake S3 and stream the data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/frolvanya/near-lake-framework-py",
     project_urls={
@@ -19,15 +19,16 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.6",
+    python_requires=">=3.9",
     install_requires=[
         "asyncio>=3.4.3",
         "dataclasses>=0.6",
         "dataclasses-json>=0.5.7",
-        "aiobotocore>=2.3.0"
-    ]
+        "aiobotocore>=2.3.0",
+    ],
+    package_data={"near_lake_framework": ["py.typed"]},
 )
```

### Comparing `near-lake-framework-0.0.7/src/near_lake_framework/__init__.py` & `near-lake-framework-0.0.8/src/near_lake_framework/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,68 @@
+from __future__ import annotations
 import asyncio
 import itertools
-from typing import Optional, Type
+from enum import Enum
+from typing import Optional
 
 from aiobotocore.session import get_session  # type: ignore
 
 from near_lake_framework import near_primitives
 from near_lake_framework import s3_fetchers
 
 
 from dataclasses import dataclass
 
 
+class Network(Enum):
+    MAINNET = "mainnet"
+    TESTNET = "testnet"
+
+    @staticmethod
+    def from_string(value: str):
+        try:
+            return Network(value.lower())
+        except ValueError as err:
+            valid_values = [v.value for v in Network]
+            raise ValueError(
+                f"Unknown network: {value}. Valid values are: {valid_values}"
+            ) from err
+
+    def __str__(self) -> str:
+        return self.value
+
+    def __repr__(self) -> str:
+        return self.value
+
+
 @dataclass
 class LakeConfig:
     s3_bucket_name: str
     s3_region_name: str
     aws_access_key_id: str
     aws_secret_key: str
     start_block_height: near_primitives.BlockHeight
     blocks_preload_pool_size: int = 200
 
-    @classmethod
-    def mainnet(cls) -> Type["LakeConfig"]:
-        cls.s3_bucket_name = "near-lake-data-mainnet"
-        cls.s3_region_name = "eu-central-1"
-
-        return cls
-
-    @classmethod
-    def testnet(cls) -> Type["LakeConfig"]:
-        cls.s3_bucket_name = "near-lake-data-testnet"
-        cls.s3_region_name = "eu-central-1"
-
-        return cls
+    def __init__(
+        self,
+        network: Network,
+        aws_access_key_id: str,
+        aws_secret_key: str,
+        start_block_height: near_primitives.BlockHeight,
+        preload_pool_size: int = 200,
+    ):
+        # These are entirely determined by Network.
+        self.s3_bucket_name = f"near-lake-data-{network.value}"
+        self.s3_region_name = "eu-central-1"
+
+        self.aws_access_key_id = aws_access_key_id
+        self.aws_secret_key = aws_secret_key
+        self.start_block_height = start_block_height
+        self.preload_pool_size = preload_pool_size
 
 
 async def start(config: LakeConfig, streamer_messages_queue: asyncio.Queue):
     session = get_session()
     async with session.create_client(
         "s3",
         region_name=config.s3_region_name,
@@ -114,8 +140,8 @@
 
 
 def streamer(config: LakeConfig):
     streamer_messages_queue: asyncio.Queue = asyncio.Queue(
         maxsize=config.blocks_preload_pool_size
     )
     stream_handle = asyncio.create_task(start(config, streamer_messages_queue))
-    return (stream_handle, streamer_messages_queue)
+    return stream_handle, streamer_messages_queue
```

### Comparing `near-lake-framework-0.0.7/src/near_lake_framework/near_primitives.py` & `near-lake-framework-0.0.8/src/near_lake_framework/near_primitives.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,17 @@
     next_bp_hash: CryptoHash
     block_merkle_root: CryptoHash
     epoch_sync_data_hash: Optional[CryptoHash]
     approvals: List[Optional[str]]
     signature: str
     latest_protocol_version: int
     height: BlockHeight = field(metadata=config(mm_field=BlockHeightField()))
-    prev_height: Optional[BlockHeight] = field(default=None, metadata=config(mm_field=BlockHeightField()))
+    prev_height: Optional[BlockHeight] = field(
+        default=None, metadata=config(mm_field=BlockHeightField())
+    )
 
 
 @dataclass
 class ChunkHeader(DataClassJsonMixin):
     chunk_hash: CryptoHash
     prev_block_hash: CryptoHash
     outcome_root: CryptoHash
```

### Comparing `near-lake-framework-0.0.7/src/near_lake_framework.egg-info/PKG-INFO` & `near-lake-framework-0.0.8/src/near_lake_framework.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,118 +1,124 @@
 Metadata-Version: 2.1
 Name: near-lake-framework
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python Library to connect to the NEAR Lake S3 and stream the data
 Home-page: https://github.com/frolvanya/near-lake-framework-py
 Author: Ivan Frolov
 Author-email: frolvanya@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/frolvanya/near-lake-framework-py/issues
-Description: # NEAR Lake Framework for Python
-        
-        Available in programming languages: [Rust](https://github.com/near/near-lake-framework-rs) | [Javascript](https://github.com/near/near-lake-framework-js) | **Python3**
-        
-        NEAR Lake Framework is a small library companion to [NEAR Lake](https://github.com/near/near-lake). It allows you to build
-        your own indexer that subscribes to the stream of blocks from the NEAR Lake data source and create your own logic to process
-        the NEAR Protocol data.
-        
-        [![PyPI version](https://badge.fury.io/py/near-lake-framework.svg)](https://badge.fury.io/py/near-lake-framework)
-        ![MIT or Apache 2.0 licensed](https://img.shields.io/crates/l/near-lake-framework.svg)
-        
-        ---
-        
-        [Official NEAR Lake Framework launch announcement](https://gov.near.org/t/announcement-near-lake-framework-brand-new-word-in-indexer-building-approach/17668) has been published on the NEAR Gov Forum
-        Greetings from the Data Platform Team! We are happy and proud to announce an MVP release of a brand new word in indexer building approach - NEAR Lake Framework.
-        
-        ---
-        
-        ## Example
-        
-        ```python3
-        import asyncio
-        import os
-        
-        from near_lake_framework import LakeConfig, streamer
-        
-        
-        async def main():
-            config = LakeConfig.mainnet()
-            config.start_block_height = 69130938
-            config.aws_access_key_id = os.getenv("AWS_ACCESS_KEY_ID")
-            config.aws_secret_key = os.getenv("AWS_SECRET_ACCESS_KEY")
-        
-            stream_handle, streamer_messages_queue = streamer(config)
-            while True:
-                streamer_message = await streamer_messages_queue.get()
-                print(
-                    f"Received Block #{streamer_message.block.header.height} from Lake Framework"
-                )
-        
-        
-        loop = asyncio.get_event_loop()
-        loop.run_until_complete(main())
-        ```
-        
-        ## How to use
-        
-        ### Dependencies
-        
-        Install `near-lake-framework`
-        
-        ```bash
-        $ pip3 install near-lake-framework
-        ```
-        
-        ### Credentials
-        
-        To be able to access the data from NEAR Lake you need to provide credentials. Please, see the [Credentials article](https://near-indexers.io/tutorials/lake/credentials)
-        
-        ## Configuration
-        
-        Everything should be configured before the start of your indexer application via `LakeConfig` struct.
-        
-        Available parameters:
-        
-        - `s3_bucket_name: str` - provide the AWS S3 bucket name (`near-lake-testnet`, `near-lake-mainnet` or yours if you run your own NEAR Lake)
-        - `s3_region_name: str` - provide the region for AWS S3 bucket
-        - `start_block_height: BlockHeight` - block height to start the stream from
-        - `blocks_preload_pool_size: int` - provide the number of blocks to preload (default: 200)
-        
-        ## Cost estimates
-        
-        **TL;DR** approximately $18.15 per month (for AWS S3 access, paid directly to AWS) for the reading of fresh blocks
-        
-        Explanation:
-        
-        Assuming NEAR Protocol produces accurately 1 block per second (which is really not, the average block production time is 1.3s). A full day consists of 86400 seconds, that's the max number of blocks that can be produced.
-        
-        According the [Amazon S3 prices](https://aws.amazon.com/s3/pricing/?nc1=h_ls) `list` requests are charged for $0.005 per 1000 requests and `get` is charged for $0.0004 per 1000 requests.
-        
-        Calculations (assuming we are following the tip of the network all the time):
-        
-        ```
-        86400 blocks per day * 5 requests for each block / 1000 requests * $0.0004 per 1k requests = $0.173 * 30 days = $5.19
-        ```
-        **Note:** 5 requests for each block means we have 4 shards (1 file for common block data and 4 separate files for each shard)
-        
-        And a number of `list` requests we need to perform for 30 days:
-        
-        ```
-        86400 blocks per day / 1000 requests * $0.005 per 1k list requests = $0.432 * 30 days = $12.96
-        
-        $5.19 + $12.96 = $18.15
-        ```
-        
-        The price depends on the number of shards
-        
-        
-        ### Publishing to PyPi
-        
-        [Follow this guide to safely publish PyPi package](https://widdowquinn.github.io/coding/update-pypi-package/)
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE-APACHE
+Requires-Dist: asyncio>=3.4.3
+Requires-Dist: dataclasses>=0.6
+Requires-Dist: dataclasses-json>=0.5.7
+Requires-Dist: aiobotocore>=2.3.0
+
+# NEAR Lake Framework for Python
+
+Available in programming languages: [Rust](https://github.com/near/near-lake-framework-rs) | [Javascript](https://github.com/near/near-lake-framework-js) | **Python3**
+
+NEAR Lake Framework is a small library companion to [NEAR Lake](https://github.com/near/near-lake). It allows you to build
+your own indexer that subscribes to the stream of blocks from the NEAR Lake data source and create your own logic to process
+the NEAR Protocol data.
+
+[![PyPI version](https://badge.fury.io/py/near-lake-framework.svg)](https://badge.fury.io/py/near-lake-framework)
+![MIT or Apache 2.0 licensed](https://img.shields.io/crates/l/near-lake-framework.svg)
+
+---
+
+[Official NEAR Lake Framework launch announcement](https://gov.near.org/t/announcement-near-lake-framework-brand-new-word-in-indexer-building-approach/17668) has been published on the NEAR Gov Forum
+Greetings from the Data Platform Team! We are happy and proud to announce an MVP release of a brand new word in indexer building approach - NEAR Lake Framework.
+
+---
+
+## Example
+
+```python3
+import asyncio
+import os
+
+from near_lake_framework import LakeConfig, streamer, Network
+
+
+async def main():
+    config = LakeConfig(
+        network=Network.MAINNET,
+        aws_access_key_id=os.getenv("AWS_ACCESS_KEY_ID"),
+        aws_secret_key=os.getenv("AWS_SECRET_ACCESS_KEY"),
+        start_block_height=69130938,
+    )
+
+    stream_handle, streamer_messages_queue = streamer(config)
+    while True:
+        streamer_message = await streamer_messages_queue.get()
+        print(
+            f"Received Block #{streamer_message.block.header.height} from Lake Framework"
+        )
+
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(main())
+```
+
+## How to use
+
+### Dependencies
+
+Install `near-lake-framework`
+
+```bash
+$ pip3 install near-lake-framework
+```
+
+### Credentials
+
+To be able to access the data from NEAR Lake you need to provide credentials. Please, see the [Credentials article](https://near-indexers.io/tutorials/lake/credentials)
+
+## Configuration
+
+Everything should be configured before the start of your indexer application via `LakeConfig` struct.
+
+Available parameters:
+
+- `network: Network` - provide network
+- `s3_bucket_name: str` - provide the AWS S3 bucket name (`near-lake-testnet`, `near-lake-mainnet` or yours if you run your own NEAR Lake)
+- `s3_region_name: str` - provide the region for AWS S3 bucket
+- `start_block_height: BlockHeight` - block height to start the stream from
+- `blocks_preload_pool_size: int` - provide the number of blocks to preload (default: 200)
+
+## Cost estimates
+
+**TL;DR** approximately $18.15 per month (for AWS S3 access, paid directly to AWS) for the reading of fresh blocks
+
+Explanation:
+
+Assuming NEAR Protocol produces accurately 1 block per second (which is really not, the average block production time is 1.3s). A full day consists of 86400 seconds, that's the max number of blocks that can be produced.
+
+According the [Amazon S3 prices](https://aws.amazon.com/s3/pricing/?nc1=h_ls) `list` requests are charged for $0.005 per 1000 requests and `get` is charged for $0.0004 per 1000 requests.
+
+Calculations (assuming we are following the tip of the network all the time):
+
+```
+86400 blocks per day * 5 requests for each block / 1000 requests * $0.0004 per 1k requests = $0.173 * 30 days = $5.19
+```
+**Note:** 5 requests for each block means we have 4 shards (1 file for common block data and 4 separate files for each shard)
+
+And a number of `list` requests we need to perform for 30 days:
+
+```
+86400 blocks per day / 1000 requests * $0.005 per 1k list requests = $0.432 * 30 days = $12.96
+
+$5.19 + $12.96 = $18.15
+```
+
+The price depends on the number of shards
+
+
+### Publishing to PyPi
+
+[Follow this guide to safely publish PyPi package](https://widdowquinn.github.io/coding/update-pypi-package/)
```


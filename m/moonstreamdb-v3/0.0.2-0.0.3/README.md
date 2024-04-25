# Comparing `tmp/moonstreamdb-v3-0.0.2.tar.gz` & `tmp/moonstreamdb-v3-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonstreamdb-v3-0.0.2.tar", last modified: Thu Apr 11 12:27:41 2024, max compression
+gzip compressed data, was "moonstreamdb-v3-0.0.3.tar", last modified: Thu Apr 25 09:42:18 2024, max compression
```

## Comparing `moonstreamdb-v3-0.0.2.tar` & `moonstreamdb-v3-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:27:41.601107 moonstreamdb-v3-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-11 12:27:41.601107 moonstreamdb-v3-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 12:27:27.000000 moonstreamdb-v3-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:27:41.601107 moonstreamdb-v3-0.0.2/moonstreamdb_v3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-11 12:27:41.000000 moonstreamdb-v3-0.0.2/moonstreamdb_v3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-11 12:27:41.000000 moonstreamdb-v3-0.0.2/moonstreamdb_v3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:27:41.000000 moonstreamdb-v3-0.0.2/moonstreamdb_v3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:27:32.000000 moonstreamdb-v3-0.0.2/moonstreamdb_v3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-11 12:27:41.000000 moonstreamdb-v3-0.0.2/moonstreamdb_v3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 12:27:41.000000 moonstreamdb-v3-0.0.2/moonstreamdb_v3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:27:41.601107 moonstreamdb-v3-0.0.2/moonstreamdbv3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:27:27.000000 moonstreamdb-v3-0.0.2/moonstreamdbv3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:27:41.601107 moonstreamdb-v3-0.0.2/moonstreamdbv3/alembic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:27:27.000000 moonstreamdb-v3-0.0.2/moonstreamdbv3/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-11 12:27:27.000000 moonstreamdb-v3-0.0.2/moonstreamdbv3/alembic/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:27:41.601107 moonstreamdb-v3-0.0.2/moonstreamdbv3/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (127)    49749 2024-04-11 12:27:27.000000 moonstreamdb-v3-0.0.2/moonstreamdbv3/alembic/versions/994e614b5500_tables_initial_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:27:27.000000 moonstreamdb-v3-0.0.2/moonstreamdbv3/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-11 12:27:27.000000 moonstreamdb-v3-0.0.2/moonstreamdbv3/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-04-11 12:27:27.000000 moonstreamdb-v3-0.0.2/moonstreamdbv3/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-11 12:27:27.000000 moonstreamdb-v3-0.0.2/moonstreamdbv3/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 12:27:41.601107 moonstreamdb-v3-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-11 12:27:27.000000 moonstreamdb-v3-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:42:18.399941 moonstreamdb-v3-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-25 09:42:18.399941 moonstreamdb-v3-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 09:42:04.000000 moonstreamdb-v3-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:42:18.399941 moonstreamdb-v3-0.0.3/moonstreamdb_v3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-25 09:42:18.000000 moonstreamdb-v3-0.0.3/moonstreamdb_v3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-25 09:42:18.000000 moonstreamdb-v3-0.0.3/moonstreamdb_v3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:42:18.000000 moonstreamdb-v3-0.0.3/moonstreamdb_v3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:42:08.000000 moonstreamdb-v3-0.0.3/moonstreamdb_v3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-25 09:42:18.000000 moonstreamdb-v3-0.0.3/moonstreamdb_v3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 09:42:18.000000 moonstreamdb-v3-0.0.3/moonstreamdb_v3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:42:18.399941 moonstreamdb-v3-0.0.3/moonstreamdbv3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:42:04.000000 moonstreamdb-v3-0.0.3/moonstreamdbv3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:42:18.399941 moonstreamdb-v3-0.0.3/moonstreamdbv3/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:42:04.000000 moonstreamdb-v3-0.0.3/moonstreamdbv3/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-25 09:42:04.000000 moonstreamdb-v3-0.0.3/moonstreamdbv3/alembic/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:42:18.399941 moonstreamdb-v3-0.0.3/moonstreamdbv3/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)    49749 2024-04-25 09:42:04.000000 moonstreamdb-v3-0.0.3/moonstreamdbv3/alembic/versions/994e614b5500_tables_initial_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:42:04.000000 moonstreamdb-v3-0.0.3/moonstreamdbv3/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13956 2024-04-25 09:42:04.000000 moonstreamdb-v3-0.0.3/moonstreamdbv3/alembic/versions/e9e1b43f49e1_amoy_blast_and_apex_blockchains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-04-25 09:42:04.000000 moonstreamdb-v3-0.0.3/moonstreamdbv3/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-04-25 09:42:04.000000 moonstreamdb-v3-0.0.3/moonstreamdbv3/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-25 09:42:04.000000 moonstreamdb-v3-0.0.3/moonstreamdbv3/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 09:42:18.399941 moonstreamdb-v3-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-25 09:42:04.000000 moonstreamdb-v3-0.0.3/setup.py
```

### Comparing `moonstreamdb-v3-0.0.2/PKG-INFO` & `moonstreamdb-v3-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonstreamdb-v3
-Version: 0.0.2
+Version: 0.0.3
 Summary: Moonstream V3 database
 Home-page: https://github.com/bugout-dev/moonstream
 Author: Bugout.dev
 Author-email: engineers@bugout.dev
 License: Apache License 2.0
 Description: # moonstreamdb-v3
```

### Comparing `moonstreamdb-v3-0.0.2/moonstreamdb_v3.egg-info/PKG-INFO` & `moonstreamdb-v3-0.0.3/moonstreamdb_v3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonstreamdb-v3
-Version: 0.0.2
+Version: 0.0.3
 Summary: Moonstream V3 database
 Home-page: https://github.com/bugout-dev/moonstream
 Author: Bugout.dev
 Author-email: engineers@bugout.dev
 License: Apache License 2.0
 Description: # moonstreamdb-v3
```

### Comparing `moonstreamdb-v3-0.0.2/moonstreamdb_v3.egg-info/SOURCES.txt` & `moonstreamdb-v3-0.0.3/moonstreamdb_v3.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -9,8 +9,9 @@
 moonstreamdbv3/__init__.py
 moonstreamdbv3/db.py
 moonstreamdbv3/models.py
 moonstreamdbv3/version.py
 moonstreamdbv3/alembic/__init__.py
 moonstreamdbv3/alembic/env.py
 moonstreamdbv3/alembic/versions/994e614b5500_tables_initial_generation.py
-moonstreamdbv3/alembic/versions/__init__.py
+moonstreamdbv3/alembic/versions/__init__.py
+moonstreamdbv3/alembic/versions/e9e1b43f49e1_amoy_blast_and_apex_blockchains.py
```

### Comparing `moonstreamdb-v3-0.0.2/moonstreamdbv3/alembic/env.py` & `moonstreamdb-v3-0.0.3/moonstreamdbv3/alembic/env.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,45 +27,53 @@
 # my_important_option = config.get_main_option("my_important_option")
 # ... etc.
 from moonstreamdbv3.models import (
     EthereumLabel,
     SepoliaLabel,
     PolygonLabel,
     MumbaiLabel,
+    AmoyLabel,
     XDaiLabel,
     ZkSyncEraLabel,
     ZkSyncEraSepoliaLabel,
     BaseLabel,
     ArbitrumNovaLabel,
     ArbitrumSepoliaLabel,
     XaiLabel,
     XaiSepoliaLabel,
     AvalancheLabel,
     AvalancheFujiLabel,
+    BlastLabel,
+    BlastSepoliaLabel,
+    ProofOfPlayApexLabel,
     StarknetLabel,
     StarknetSepoliaLabel,
 )
 
 
 def include_symbol(tablename, schema):
     return tablename in {
         EthereumLabel.__tablename__,
         SepoliaLabel.__tablename__,
         PolygonLabel.__tablename__,
         MumbaiLabel.__tablename__,
+        AmoyLabel.__tablename__,
         XDaiLabel.__tablename__,
         ZkSyncEraLabel.__tablename__,
         ZkSyncEraSepoliaLabel.__tablename__,
         BaseLabel.__tablename__,
         ArbitrumNovaLabel.__tablename__,
         ArbitrumSepoliaLabel.__tablename__,
         XaiLabel.__tablename__,
         XaiSepoliaLabel.__tablename__,
         AvalancheLabel.__tablename__,
         AvalancheFujiLabel.__tablename__,
+        BlastLabel.__tablename__,
+        BlastSepoliaLabel.__tablename__,
+        ProofOfPlayApexLabel.__tablename__,
         StarknetLabel.__tablename__,
         StarknetSepoliaLabel.__tablename__,
     }
 
 
 def run_migrations_offline() -> None:
     """Run migrations in 'offline' mode.
```

### Comparing `moonstreamdb-v3-0.0.2/moonstreamdbv3/alembic/versions/994e614b5500_tables_initial_generation.py` & `moonstreamdb-v3-0.0.3/moonstreamdbv3/alembic/versions/994e614b5500_tables_initial_generation.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-v3-0.0.2/moonstreamdbv3/db.py` & `moonstreamdb-v3-0.0.3/moonstreamdbv3/db.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,94 +3,100 @@
 """
 
 import logging
 import os
 from contextlib import contextmanager
 from typing import Generator, Optional
 
-from sqlalchemy import create_engine
+from sqlalchemy import create_engine, Engine
 from sqlalchemy.orm import Session, sessionmaker
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 try:
     MOONSTREAM_DB_URI = os.environ.get("MOONSTREAM_DB_URI")
     if MOONSTREAM_DB_URI is None:
         raise Warning("MOONSTREAM_DB_URI environment variable must be set")
 
     MOONSTREAM_DB_URI_READ_ONLY = os.environ.get("MOONSTREAM_DB_URI_READ_ONLY")
     if MOONSTREAM_DB_URI_READ_ONLY is None:
         raise Warning("MOONSTREAM_DB_URI_READ_ONLY environment variable must be set")
-
-    MOONSTREAM_POOL_SIZE_RAW = os.environ.get("MOONSTREAM_POOL_SIZE")
-    MOONSTREAM_POOL_SIZE = 1
-    try:
-        if MOONSTREAM_POOL_SIZE_RAW is not None:
-            MOONSTREAM_POOL_SIZE = int(MOONSTREAM_POOL_SIZE_RAW)
-    except:
-        raise ValueError(
-            f"Could not parse MOONSTREAM_POOL_SIZE as int: {MOONSTREAM_POOL_SIZE_RAW}"
-        )
-
-    MOONSTREAM_DB_STATEMENT_TIMEOUT_MILLIS_RAW = os.environ.get(
-        "MOONSTREAM_DB_STATEMENT_TIMEOUT_MILLIS"
-    )
-    MOONSTREAM_DB_STATEMENT_TIMEOUT_MILLIS = 30000
-    try:
-        if MOONSTREAM_DB_STATEMENT_TIMEOUT_MILLIS_RAW is not None:
-            MOONSTREAM_DB_STATEMENT_TIMEOUT_MILLIS = int(
-                MOONSTREAM_DB_STATEMENT_TIMEOUT_MILLIS_RAW
-            )
-    except:
-        raise ValueError(
-            f"MOONSTREAM_DB_STATEMENT_TIMEOUT_MILLIS must be an integer: {MOONSTREAM_DB_STATEMENT_TIMEOUT_MILLIS_RAW}"
-        )
 except ValueError as e:
     raise ValueError(e)
 except Warning:
     logger.warning("Database variables not set")
 
+MOONSTREAM_POOL_SIZE_RAW = os.environ.get("MOONSTREAM_POOL_SIZE")
+MOONSTREAM_POOL_SIZE = 1
+try:
+    if MOONSTREAM_POOL_SIZE_RAW is not None:
+        MOONSTREAM_POOL_SIZE = int(MOONSTREAM_POOL_SIZE_RAW)
+except:
+    raise ValueError(
+        f"Could not parse MOONSTREAM_POOL_SIZE as int: {MOONSTREAM_POOL_SIZE_RAW}"
+    )
+
+MOONSTREAM_DB_STATEMENT_TIMEOUT_MILLIS_RAW = os.environ.get(
+    "MOONSTREAM_DB_STATEMENT_TIMEOUT_MILLIS"
+)
+MOONSTREAM_DB_STATEMENT_TIMEOUT_MILLIS = 30000
+try:
+    if MOONSTREAM_DB_STATEMENT_TIMEOUT_MILLIS_RAW is not None:
+        MOONSTREAM_DB_STATEMENT_TIMEOUT_MILLIS = int(
+            MOONSTREAM_DB_STATEMENT_TIMEOUT_MILLIS_RAW
+        )
+except:
+    raise ValueError(
+        f"MOONSTREAM_DB_STATEMENT_TIMEOUT_MILLIS must be an integer: {MOONSTREAM_DB_STATEMENT_TIMEOUT_MILLIS_RAW}"
+    )
+
 
 def create_moonstream_engine(
     url: str,
     pool_size: int,
     statement_timeout: int,
     pool_pre_ping: bool = False,
     schema: Optional[str] = None,
-):
+) -> Engine:
     # Pooling: https://docs.sqlalchemy.org/en/14/core/pooling.html#sqlalchemy.pool.QueuePool
     # Statement timeout: https://stackoverflow.com/a/44936982
     options = f"-c statement_timeout={statement_timeout}"
     if schema is not None:
         options += f" -c search_path={schema}"
     return create_engine(
         url=url,
         pool_pre_ping=pool_pre_ping,
         pool_size=pool_size,
         connect_args={"options": options},
     )
 
 
-class MoonstreamDBEngine:
-    def __init__(self, schema: Optional[str] = None) -> None:
+class DBEngine:
+    def __init__(self, url: str, schema: Optional[str] = None) -> None:
         self._engine = create_moonstream_engine(
-            url=MOONSTREAM_DB_URI,  # type: ignore
+            url=url,  # type: ignore
             pool_size=MOONSTREAM_POOL_SIZE,
             statement_timeout=MOONSTREAM_DB_STATEMENT_TIMEOUT_MILLIS,
             schema=schema,
         )
-        self._session_local = sessionmaker(bind=self.engine)
-
-        self._yield_db_session_ctx = contextmanager(self.yield_db_session)
 
     @property
-    def engine(self):
+    def engine(self) -> Engine:
         return self._engine
 
+
+class MoonstreamDBEngine(DBEngine):
+    def __init__(self, schema: Optional[str] = None) -> None:
+        super().__init__(url=MOONSTREAM_DB_URI, schema=schema)
+
+        self._session_local = sessionmaker(bind=self.engine)
+
+        self._yield_db_session_ctx = contextmanager(self.yield_db_session)
+
     @property
     def session_local(self):
         return self._session_local
 
     @property
     def yield_db_session_ctx(self):
         return self._yield_db_session_ctx
@@ -106,42 +112,40 @@
         session = self._session_local()
         try:
             yield session
         finally:
             session.close()
 
 
-class MoonstreamDBEngineRO:
+class MoonstreamDBEngineRO(DBEngine):
     def __init__(self, schema: Optional[str] = None) -> None:
-        self._RO_engine = create_moonstream_engine(
-            url=MOONSTREAM_DB_URI_READ_ONLY,  # type: ignore
-            pool_size=MOONSTREAM_POOL_SIZE,
-            statement_timeout=MOONSTREAM_DB_STATEMENT_TIMEOUT_MILLIS,
-            schema=schema,
-        )
-        self._RO_session_local = sessionmaker(bind=self.RO_engine)
+        super().__init__(url=MOONSTREAM_DB_URI_READ_ONLY, schema=schema)
 
-        self._RO_yield_db_session_ctx = contextmanager(self.yield_db_read_only_session)
+    @property
+    def engine(self):
+        raise AttributeError(
+            "RO_engine should be used instead of engine for read-only access."
+        )
 
     @property
-    def RO_engine(self):
-        return self._RO_engine
+    def RO_engine(self) -> Engine:
+        return self._engine
 
     @property
     def RO_session_local(self):
-        return self._RO_session_local
+        return self._session_local
 
     @property
     def RO_yield_db_session_ctx(self):
-        return self._RO_yield_db_session_ctx
+        return self._yield_db_session_ctx
 
     def yield_db_read_only_session(self) -> Generator[Session, None, None]:
         """
         Yields read-only database connection (created using environment variables).
         As per FastAPI docs:
         https://fastapi.tiangolo.com/tutorial/sql-databases/#create-a-dependency
         """
-        session = self._RO_session_local()
+        session = self._session_local()
         try:
             yield session
         finally:
             session.close()
```

### Comparing `moonstreamdb-v3-0.0.2/moonstreamdbv3/models.py` & `moonstreamdb-v3-0.0.3/moonstreamdbv3/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -189,14 +189,33 @@
             "address",
             "block_timestamp",
             unique=False,
         ),
     )
 
 
+class AmoyLabel(EvmBasedLabel):  # type: ignore
+    __tablename__ = "amoy_labels"
+
+    __table_args__ = (
+        Index(
+            "ix_amoy_labels_addr_block_num",
+            "address",
+            "block_number",
+            unique=False,
+        ),
+        Index(
+            "ix_amoy_labels_addr_block_ts",
+            "address",
+            "block_timestamp",
+            unique=False,
+        ),
+    )
+
+
 class XDaiLabel(EvmBasedLabel):  # type: ignore
     __tablename__ = "xdai_labels"
 
     __table_args__ = (
         Index(
             "ix_xdai_labels_addr_block_num",
             "address",
@@ -379,14 +398,71 @@
             "address",
             "block_timestamp",
             unique=False,
         ),
     )
 
 
+class BlastLabel(EvmBasedLabel):  # type: ignore
+    __tablename__ = "blast_labels"
+
+    __table_args__ = (
+        Index(
+            "ix_blast_labels_addr_block_num",
+            "address",
+            "block_number",
+            unique=False,
+        ),
+        Index(
+            "ix_blast_labels_addr_block_ts",
+            "address",
+            "block_timestamp",
+            unique=False,
+        ),
+    )
+
+
+class BlastSepoliaLabel(EvmBasedLabel):  # type: ignore
+    __tablename__ = "blast_sepolia_labels"
+
+    __table_args__ = (
+        Index(
+            "ix_blast_sepolia_labels_addr_block_num",
+            "address",
+            "block_number",
+            unique=False,
+        ),
+        Index(
+            "ix_blast_sepolia_labels_addr_block_ts",
+            "address",
+            "block_timestamp",
+            unique=False,
+        ),
+    )
+
+
+class ProofOfPlayApexLabel(EvmBasedLabel):  # type: ignore
+    __tablename__ = "proofofplay_apex_labels"
+
+    __table_args__ = (
+        Index(
+            "ix_proofofplay_apex_labels_addr_block_num",
+            "address",
+            "block_number",
+            unique=False,
+        ),
+        Index(
+            "ix_proofofplay_apex_labels_addr_block_ts",
+            "address",
+            "block_timestamp",
+            unique=False,
+        ),
+    )
+
+
 class StarknetLabel(EvmBasedLabel):  # type: ignore
     __tablename__ = "starknet_labels"
 
     __table_args__ = (
         Index(
             "ix_starknet_labels_addr_block_num",
             "address",
```

### Comparing `moonstreamdb-v3-0.0.2/setup.py` & `moonstreamdb-v3-0.0.3/setup.py`

 * *Files identical despite different names*


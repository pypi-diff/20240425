# Comparing `tmp/asqlorm-0.5.2.tar.gz` & `tmp/asqlorm-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asqlorm-0.5.2.tar", max compression
+gzip compressed data, was "asqlorm-0.6.1.tar", max compression
```

## Comparing `asqlorm-0.5.2.tar` & `asqlorm-0.6.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        7 2024-02-20 21:09:44.192439 asqlorm-0.5.2/README.md
--rw-r--r--   0        0        0        0 2024-02-06 21:46:57.101551 asqlorm-0.5.2/asqlorm/__init__.py
--rw-r--r--   0        0        0    30571 2024-02-24 23:55:25.233638 asqlorm-0.5.2/asqlorm/generator/main.py
--rw-r--r--   0        0        0    44452 2024-02-29 20:35:58.956976 asqlorm-0.5.2/asqlorm/models.py
--rw-r--r--   0        0        0     8621 2024-02-25 00:04:13.192024 asqlorm-0.5.2/asqlorm/sql/sql_alchemy.py
--rw-r--r--   0        0        0     1753 2024-02-24 00:45:59.861298 asqlorm-0.5.2/asqlorm/utils.py
--rw-r--r--   0        0        0      659 2024-02-29 20:35:55.997813 asqlorm-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 asqlorm-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0        7 2024-02-20 21:09:44.192439 asqlorm-0.6.1/README.md
+-rw-r--r--   0        0        0        0 2024-02-06 21:46:57.101551 asqlorm-0.6.1/asqlorm/__init__.py
+-rw-r--r--   0        0        0    30571 2024-02-24 23:55:25.233638 asqlorm-0.6.1/asqlorm/generator/main.py
+-rw-r--r--   0        0        0    44452 2024-02-29 20:35:58.956976 asqlorm-0.6.1/asqlorm/models.py
+-rw-r--r--   0        0        0     8402 2024-04-24 23:09:35.099688 asqlorm-0.6.1/asqlorm/sql/sql_alchemy.py
+-rw-r--r--   0        0        0     1753 2024-02-24 00:45:59.861298 asqlorm-0.6.1/asqlorm/utils.py
+-rw-r--r--   0        0        0      659 2024-04-24 23:07:40.288367 asqlorm-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 asqlorm-0.6.1/PKG-INFO
```

### Comparing `asqlorm-0.5.2/asqlorm/generator/main.py` & `asqlorm-0.6.1/asqlorm/generator/main.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.5.2/asqlorm/models.py` & `asqlorm-0.6.1/asqlorm/models.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.5.2/asqlorm/sql/sql_alchemy.py` & `asqlorm-0.6.1/asqlorm/sql/sql_alchemy.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,28 +28,22 @@
 
 
 class TooManyRowsReturnedError(SQLError):
     pass
 
 
 def build_engine(echo: bool) -> AsyncEngine:
-    pg_to_use = os.environ["POSTGRES_DSN_TO_USE"]
-    dsn = os.environ[pg_to_use]
-    if pg_to_use.lower().startswith("edgedb"):
-        dsn = dsn.replace("sql://", "sql+psycopg://")
-    else:
-        dsn = dsn.replace("sql://", "sql+asyncpg://")
+    dsn = os.environ["POSTGRES_DSN"].replace("sql://", "sql+asyncpg://")
     return create_async_engine(
         dsn, echo=echo, echo_pool=echo, pool_size=50, future=True, pool_recycle=300
     )
 
 
 def build_sync_engine(echo: bool) -> Engine:
-    pg_to_use = os.environ["POSTGRES_DSN_TO_USE"]
-    dsn = os.environ[pg_to_use].replace("sql://", "sql+psycopg://")
+    dsn = os.environ["POSTGRES_DSN"].replace("sql://", "sql+psycopg://")
     return create_engine(
         dsn, echo=echo, echo_pool=echo, pool_size=50, future=True, pool_recycle=300
     )
 
 
 SHOULD_ECHO: bool = True
```

### Comparing `asqlorm-0.5.2/asqlorm/utils.py` & `asqlorm-0.6.1/asqlorm/utils.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.5.2/pyproject.toml` & `asqlorm-0.6.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "asqlorm"
-version = "0.5.2"
+version = "0.6.1"
 description = ""
 authors = ["Jeremy Berman <jerber@sas.upenn.edu>"]
 readme = "README.md"
 packages = [{ include = 'asqlorm' }]
 exclude = ["tests/**/*"]
 
 
 [tool.poetry.dependencies]
 python = "^3.12"
-pydantic = "^2.6"
+pydantic = "^2.7"
 fastgql = "^0.20"
 devtools = "*"
 sqlparse = "*"
 black = "*"
 psycopg = {extras = ["binary"], version = "*"}
-sqlalchemy = "^2.0.25"
-sentry-sdk = {extras = ["sqlalchemy"], version = "^1.40.2"}
+sqlalchemy = "^2.0.29"
+sentry-sdk = {extras = ["sqlalchemy"], version = "^1.45.0"}
 greenlet = "^3.0.3"
 asyncpg = "^0.29.0"
 
 [tool.poetry.dev-dependencies]
 mypy = '^1.8'
 ruff = '*'
 doppler-env = '^0.3.1'
```

### Comparing `asqlorm-0.5.2/PKG-INFO` & `asqlorm-0.6.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: asqlorm
-Version: 0.5.2
+Version: 0.6.1
 Summary: 
 Author: Jeremy Berman
 Author-email: jerber@sas.upenn.edu
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asyncpg (>=0.29.0,<0.30.0)
 Requires-Dist: black
 Requires-Dist: devtools
 Requires-Dist: fastgql (>=0.20,<0.21)
 Requires-Dist: greenlet (>=3.0.3,<4.0.0)
 Requires-Dist: psycopg[binary]
-Requires-Dist: pydantic (>=2.6,<3.0)
-Requires-Dist: sentry-sdk[sqlalchemy] (>=1.40.2,<2.0.0)
-Requires-Dist: sqlalchemy (>=2.0.25,<3.0.0)
+Requires-Dist: pydantic (>=2.7,<3.0)
+Requires-Dist: sentry-sdk[sqlalchemy] (>=1.45.0,<2.0.0)
+Requires-Dist: sqlalchemy (>=2.0.29,<3.0.0)
 Requires-Dist: sqlparse
 Description-Content-Type: text/markdown
 
 sqlorm!
```


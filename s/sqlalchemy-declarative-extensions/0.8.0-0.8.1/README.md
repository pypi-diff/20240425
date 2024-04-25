# Comparing `tmp/sqlalchemy-declarative-extensions-0.8.0.tar.gz` & `tmp/sqlalchemy-declarative-extensions-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-declarative-extensions-0.8.0.tar", max compression
+gzip compressed data, was "sqlalchemy-declarative-extensions-0.8.1.tar", max compression
```

## Comparing `sqlalchemy-declarative-extensions-0.8.0.tar` & `sqlalchemy-declarative-extensions-0.8.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0      191 2024-03-20 11:30:49.598443 sqlalchemy-declarative-extensions-0.8.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2024-03-20 11:30:49.598443 sqlalchemy-declarative-extensions-0.8.0/LICENSE
--rw-r--r--   0        0        0    11624 2024-03-20 11:30:49.598443 sqlalchemy-declarative-extensions-0.8.0/README.md
--rw-r--r--   0        0        0     3348 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1350 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/__init__.py
--rw-r--r--   0        0        0      129 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/alembic/__init__.py
--rw-r--r--   0        0        0     1054 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/alembic/base.py
--rw-r--r--   0        0        0     1338 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/alembic/function.py
--rw-r--r--   0        0        0     1916 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/alembic/grant.py
--rw-r--r--   0        0        0     1894 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/alembic/role.py
--rw-r--r--   0        0        0     2102 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/alembic/row.py
--rw-r--r--   0        0        0     1551 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/alembic/schema.py
--rw-r--r--   0        0        0     1480 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/alembic/trigger.py
--rw-r--r--   0        0        0     1510 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/alembic/view.py
--rw-r--r--   0        0        0     8347 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/api.py
--rw-r--r--   0        0        0     8191 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/audit.py
--rw-r--r--   0        0        0      770 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/__init__.py
--rw-r--r--   0        0        0      775 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/from_string.py
--rw-r--r--   0        0        0        0 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/mysql/__init__.py
--rw-r--r--   0        0        0      716 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/mysql/query.py
--rw-r--r--   0        0        0      853 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/mysql/schema.py
--rw-r--r--   0        0        0     1104 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/postgresql/__init__.py
--rw-r--r--   0        0        0     4503 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/postgresql/acl.py
--rw-r--r--   0        0        0     1403 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/postgresql/function.py
--rw-r--r--   0        0        0    11857 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/postgresql/grant.py
--rw-r--r--   0        0        0     5557 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/postgresql/grant_type.py
--rw-r--r--   0        0        0     5944 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/postgresql/query.py
--rw-r--r--   0        0        0     8148 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/postgresql/role.py
--rw-r--r--   0        0        0     7384 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/postgresql/schema.py
--rw-r--r--   0        0        0     4941 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/postgresql/trigger.py
--rw-r--r--   0        0        0     2801 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/query.py
--rw-r--r--   0        0        0        0 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/snowflake/__init__.py
--rw-r--r--   0        0        0      868 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/snowflake/query.py
--rw-r--r--   0        0        0        0 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/sqlite/__init__.py
--rw-r--r--   0        0        0     1215 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/sqlite/query.py
--rw-r--r--   0        0        0      677 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/sqlite/schema.py
--rw-r--r--   0        0        0      189 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/function/__init__.py
--rw-r--r--   0        0        0     3079 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/function/base.py
--rw-r--r--   0        0        0     3071 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/function/compare.py
--rw-r--r--   0        0        0      529 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/function/ddl.py
--rw-r--r--   0        0        0       93 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/grant/__init__.py
--rw-r--r--   0        0        0     2308 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/grant/base.py
--rw-r--r--   0        0        0     4488 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/grant/compare.py
--rw-r--r--   0        0        0      643 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/grant/ddl.py
--rw-r--r--   0        0        0        0 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/py.typed
--rw-r--r--   0        0        0       91 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/role/__init__.py
--rw-r--r--   0        0        0     1092 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/role/base.py
--rw-r--r--   0        0        0     3861 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/role/compare.py
--rw-r--r--   0        0        0      707 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/role/ddl.py
--rw-r--r--   0        0        0     1088 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/role/generic.py
--rw-r--r--   0        0        0     2615 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/role/topological_sort.py
--rw-r--r--   0        0        0      196 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/row/__init__.py
--rw-r--r--   0        0        0     2973 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/row/base.py
--rw-r--r--   0        0        0    10743 2024-03-20 11:30:49.602443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/row/compare.py
--rw-r--r--   0        0        0      471 2024-03-20 11:30:49.606443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/row/query.py
--rw-r--r--   0        0        0      194 2024-03-20 11:30:49.606443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/schema/__init__.py
--rw-r--r--   0        0        0     1691 2024-03-20 11:30:49.606443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/schema/base.py
--rw-r--r--   0        0        0     1649 2024-03-20 11:30:49.606443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/schema/compare.py
--rw-r--r--   0        0        0      568 2024-03-20 11:30:49.606443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/schema/ddl.py
--rw-r--r--   0        0        0      528 2024-03-20 11:30:49.606443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/sql.py
--rw-r--r--   0        0        0     2712 2024-03-20 11:30:49.606443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/sqlalchemy.py
--rw-r--r--   0        0        0      182 2024-03-20 11:30:49.606443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/trigger/__init__.py
--rw-r--r--   0        0        0     2176 2024-03-20 11:30:49.606443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/trigger/base.py
--rw-r--r--   0        0        0     2334 2024-03-20 11:30:49.606443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/trigger/compare.py
--rw-r--r--   0        0        0      541 2024-03-20 11:30:49.606443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/trigger/ddl.py
--rw-r--r--   0        0        0      103 2024-03-20 11:30:49.606443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/typing.py
--rw-r--r--   0        0        0      215 2024-03-20 11:30:49.606443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/view/__init__.py
--rw-r--r--   0        0        0    16955 2024-03-20 11:30:49.606443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/view/base.py
--rw-r--r--   0        0        0     3378 2024-03-20 11:30:49.606443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/view/compare.py
--rw-r--r--   0        0        0      580 2024-03-20 11:30:49.606443 sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/view/ddl.py
--rw-r--r--   0        0        0    13506 1970-01-01 00:00:00.000000 sqlalchemy-declarative-extensions-0.8.0/setup.py
--rw-r--r--   0        0        0    12693 1970-01-01 00:00:00.000000 sqlalchemy-declarative-extensions-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      191 2024-04-25 20:10:59.872990 sqlalchemy-declarative-extensions-0.8.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2024-04-25 20:10:59.872990 sqlalchemy-declarative-extensions-0.8.1/LICENSE
+-rw-r--r--   0        0        0    11624 2024-04-25 20:10:59.872990 sqlalchemy-declarative-extensions-0.8.1/README.md
+-rw-r--r--   0        0        0     3348 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1350 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/__init__.py
+-rw-r--r--   0        0        0      129 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/alembic/__init__.py
+-rw-r--r--   0        0        0     1054 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/alembic/base.py
+-rw-r--r--   0        0        0     1338 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/alembic/function.py
+-rw-r--r--   0        0        0     1916 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/alembic/grant.py
+-rw-r--r--   0        0        0     1894 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/alembic/role.py
+-rw-r--r--   0        0        0     2102 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/alembic/row.py
+-rw-r--r--   0        0        0     1551 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/alembic/schema.py
+-rw-r--r--   0        0        0     1480 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/alembic/trigger.py
+-rw-r--r--   0        0        0     1510 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/alembic/view.py
+-rw-r--r--   0        0        0     8347 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/api.py
+-rw-r--r--   0        0        0     8191 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/audit.py
+-rw-r--r--   0        0        0      770 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/__init__.py
+-rw-r--r--   0        0        0      775 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/from_string.py
+-rw-r--r--   0        0        0        0 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/mysql/__init__.py
+-rw-r--r--   0        0        0      716 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/mysql/query.py
+-rw-r--r--   0        0        0      853 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/mysql/schema.py
+-rw-r--r--   0        0        0     1104 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/__init__.py
+-rw-r--r--   0        0        0     4503 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/acl.py
+-rw-r--r--   0        0        0     1403 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/function.py
+-rw-r--r--   0        0        0    11857 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/grant.py
+-rw-r--r--   0        0        0     5557 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/grant_type.py
+-rw-r--r--   0        0        0     5944 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/query.py
+-rw-r--r--   0        0        0     8148 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/role.py
+-rw-r--r--   0        0        0     7384 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/schema.py
+-rw-r--r--   0        0        0     4941 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/trigger.py
+-rw-r--r--   0        0        0     2801 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/query.py
+-rw-r--r--   0        0        0        0 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/snowflake/__init__.py
+-rw-r--r--   0        0        0      868 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/snowflake/query.py
+-rw-r--r--   0        0        0        0 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/sqlite/__init__.py
+-rw-r--r--   0        0        0     1215 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/sqlite/query.py
+-rw-r--r--   0        0        0      677 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/sqlite/schema.py
+-rw-r--r--   0        0        0      189 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/function/__init__.py
+-rw-r--r--   0        0        0     3079 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/function/base.py
+-rw-r--r--   0        0        0     3071 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/function/compare.py
+-rw-r--r--   0        0        0      529 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/function/ddl.py
+-rw-r--r--   0        0        0       93 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/grant/__init__.py
+-rw-r--r--   0        0        0     2308 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/grant/base.py
+-rw-r--r--   0        0        0     4488 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/grant/compare.py
+-rw-r--r--   0        0        0      643 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/grant/ddl.py
+-rw-r--r--   0        0        0        0 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/py.typed
+-rw-r--r--   0        0        0       91 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/role/__init__.py
+-rw-r--r--   0        0        0     1092 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/role/base.py
+-rw-r--r--   0        0        0     3861 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/role/compare.py
+-rw-r--r--   0        0        0      707 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/role/ddl.py
+-rw-r--r--   0        0        0     1088 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/role/generic.py
+-rw-r--r--   0        0        0     2615 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/role/topological_sort.py
+-rw-r--r--   0        0        0      196 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/row/__init__.py
+-rw-r--r--   0        0        0     2973 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/row/base.py
+-rw-r--r--   0        0        0    10831 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/row/compare.py
+-rw-r--r--   0        0        0      471 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/row/query.py
+-rw-r--r--   0        0        0      194 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/schema/__init__.py
+-rw-r--r--   0        0        0     1691 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/schema/base.py
+-rw-r--r--   0        0        0     1649 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/schema/compare.py
+-rw-r--r--   0        0        0      568 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/schema/ddl.py
+-rw-r--r--   0        0        0      528 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/sql.py
+-rw-r--r--   0        0        0     2712 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/sqlalchemy.py
+-rw-r--r--   0        0        0      182 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/trigger/__init__.py
+-rw-r--r--   0        0        0     2176 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/trigger/base.py
+-rw-r--r--   0        0        0     2334 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/trigger/compare.py
+-rw-r--r--   0        0        0      541 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/trigger/ddl.py
+-rw-r--r--   0        0        0      103 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/typing.py
+-rw-r--r--   0        0        0      215 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/view/__init__.py
+-rw-r--r--   0        0        0    16955 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/view/base.py
+-rw-r--r--   0        0        0     3378 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/view/compare.py
+-rw-r--r--   0        0        0      580 2024-04-25 20:10:59.876990 sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/view/ddl.py
+-rw-r--r--   0        0        0    13506 1970-01-01 00:00:00.000000 sqlalchemy-declarative-extensions-0.8.1/setup.py
+-rw-r--r--   0        0        0    12693 1970-01-01 00:00:00.000000 sqlalchemy-declarative-extensions-0.8.1/PKG-INFO
```

### Comparing `sqlalchemy-declarative-extensions-0.8.0/LICENSE` & `sqlalchemy-declarative-extensions-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/README.md` & `sqlalchemy-declarative-extensions-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/pyproject.toml` & `sqlalchemy-declarative-extensions-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlalchemy-declarative-extensions"
-version = "0.8.0"
+version = "0.8.1"
 authors = ["Dan Cardin <ddcardin@gmail.com>"]
 
 description = "Library to declare additional kinds of objects not natively supported by SQLAlchemy/Alembic."
 license = "Apache-2.0"
 repository = "https://github.com/dancardin/sqlalchemy-declarative-extensions"
 readme = 'README.md'
```

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/__init__.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/alembic/base.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/alembic/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/alembic/function.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/alembic/function.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/alembic/grant.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/alembic/grant.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/alembic/role.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/alembic/role.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/alembic/row.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/alembic/row.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/alembic/schema.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/alembic/schema.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/alembic/trigger.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/alembic/trigger.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/alembic/view.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/alembic/view.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/api.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/api.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/audit.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/audit.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/__init__.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/from_string.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/from_string.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/mysql/query.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/mysql/query.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/mysql/schema.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/mysql/schema.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/postgresql/__init__.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/postgresql/acl.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/acl.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/postgresql/function.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/function.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/postgresql/grant.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/grant.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/postgresql/grant_type.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/grant_type.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/postgresql/query.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/query.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/postgresql/role.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/role.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/postgresql/schema.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/schema.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/postgresql/trigger.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/postgresql/trigger.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/query.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/query.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/snowflake/query.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/snowflake/query.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/sqlite/query.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/sqlite/query.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/dialects/sqlite/schema.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/dialects/sqlite/schema.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/function/base.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/function/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/function/compare.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/function/compare.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/function/ddl.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/function/ddl.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/grant/base.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/grant/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/grant/compare.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/grant/compare.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/grant/ddl.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/grant/ddl.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/role/base.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/role/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/role/compare.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/role/compare.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/role/ddl.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/role/ddl.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/role/generic.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/role/generic.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/role/topological_sort.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/role/topological_sort.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/row/base.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/row/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/row/compare.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/row/compare.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,17 +310,21 @@
         table_exists = existing_tables[table.fullname]
         if not table_exists:
             result[table.fullname] = {}
             continue
 
         primary_key_columns = [c.name for c in table.primary_key.columns]
 
-        filter_str = or_(*filters).compile(
-            dialect=connection.dialect, compile_kwargs={"literal_binds": True}
+        filter_str = str(
+            or_(*filters).compile(
+                dialect=connection.dialect, compile_kwargs={"literal_binds": True}
+            )
         )
+        filter_str = filter_str.replace(":", r"\:")
+
         records = connection.execute(
             text(f"SELECT * FROM {table.fullname} WHERE {filter_str}")  # noqa: S608
         )
         assert records
 
         existing_rows = result.setdefault(table.fullname, {})
         for record in records.fetchall():
```

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/schema/base.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/schema/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/schema/compare.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/schema/compare.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/schema/ddl.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/schema/ddl.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/sql.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/sql.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/sqlalchemy.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/trigger/base.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/trigger/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/trigger/compare.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/trigger/compare.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/trigger/ddl.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/trigger/ddl.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/view/base.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/view/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/view/compare.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/view/compare.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/src/sqlalchemy_declarative_extensions/view/ddl.py` & `sqlalchemy-declarative-extensions-0.8.1/src/sqlalchemy_declarative_extensions/view/ddl.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-declarative-extensions-0.8.0/setup.py` & `sqlalchemy-declarative-extensions-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 ['sqlalchemy>=1.3']
 
 extras_require = \
 {'alembic': ['alembic>=1.0'], 'parse': ['sqlglot']}
 
 setup_kwargs = {
     'name': 'sqlalchemy-declarative-extensions',
-    'version': '0.8.0',
+    'version': '0.8.1',
     'description': 'Library to declare additional kinds of objects not natively supported by SQLAlchemy/Alembic.',
     'long_description': '# SQLAlchemy Declarative Extensions\n\n[![Actions Status](https://github.com/dancardin/sqlalchemy-declarative-extensions/workflows/test/badge.svg)](https://github.com/dancardin/sqlalchemy-declarative-extensions/actions)\n[![Coverage Status](https://coveralls.io/repos/github/DanCardin/sqlalchemy-declarative-extensions/badge.svg?branch=main)](https://coveralls.io/github/DanCardin/sqlalchemy-declarative-extensions?branch=main)\n[![Documentation Status](https://readthedocs.org/projects/sqlalchemy-declarative-extensions/badge/?version=latest)](https://sqlalchemy-declarative-extensions.readthedocs.io/en/latest/?badge=latest)\n\nSee the full documentation\n[here](https://sqlalchemy-declarative-extensions.readthedocs.io/en/latest/).\n\nAdds extensions to SQLAlchemy (and/or Alembic) which allows declaratively\nstating the existence of additional kinds of objects about your database not\nnatively supported by SQLAlchemy/Alembic.\n\nThis includes:\n\n- Schemas\n- Views\n- Roles\n- Privileges (Grants/Default Grants)\n- Functions\n- Triggers\n- Rows (i.e. data)\n- "audit tables" (i.e. triggers which record data changes to some source table)\n\nThe primary function(s) of this library include:\n\n- Registering onto the SQLAlchemy event system such that `metadata.create_all`\n  creates these objects.\n- (Optionally) Registers into Alembic such that\n  `alembic revision --autogenerate` automatically creates/updates/deletes\n  declared objects.\n\n## Kitchen Sink Example (using all available features)\n\n```python\nfrom sqlalchemy import Column, types, select\nfrom sqlalchemy.orm import as_declarative\nfrom sqlalchemy_declarative_extensions import (\n    declarative_database, Schemas, Roles, Row, View, view,\n)\nfrom sqlalchemy_declarative_extensions.dialects.postgresql import (\n    DefaultGrant, Function, Trigger, Role\n)\nfrom sqlalchemy_declarative_extensions.audit import audit\n\n\n@declarative_database\n@as_declarative\nclass Base:\n    # Note: each object type also has a plural version (i.e. Schemas/Roles/etc) where you can specify\n    # collection-level options like `ignore_unspecified`).\n    #\n    # If you dont set any collection-level options, you can instead use raw list/iterable as the collection.\n    schemas = Schemas().are("example")\n    roles = Roles(ignore_unspecified=True).are(\n        Role("read", login=False),\n        Role(\n            "app",\n            in_roles=[\'read\']\n        ),\n    )\n    grants = [\n        DefaultGrant.on_tables_in_schema("public", \'example\').grant("select", to="read"),\n        DefaultGrant.on_sequences_in_schema("public").grant("usage", to="read"),\n        Grant.new("usage", to="read").on_schemas("example")\n    ]\n    rows = [\n        Row(\'foo\', id=1),\n    ]\n    views = [\n        View("low_foo", "select * from foo where i < 10"),\n    ]\n    functions = [\n        Function(\n            "fancy_function",\n            """\n            BEGIN\n            INSERT INTO foo (id) select NEW.id + 1;\n            RETURN NULL;\n            END\n            """,\n            language="plpgsql",\n            returns="trigger",\n        ),\n    ]\n    triggers = [\n        Trigger.after("insert", on="foo", execute="fancy_function")\n        .named("on_insert_foo")\n        .when("pg_trigger_depth() < 1")\n        .for_each_row(),\n    ]\n\n\n@audit()\nclass Foo(Base):\n    __tablename__ = \'foo\'\n\n    id = Column(types.Integer(), primary_key=True)\n\n\naudit_table = Foo.__audit_table__\n\n\n@view(Base)\nclass HighFoo:\n    __tablename__ = "high_foo"\n    __view__ = select(Foo.__table__).where(Foo.__table__.c.id >= 10)\n```\n\nNote, there is also support for declaring objects directly through the\n`MetaData` for users not using sqlalchemy\'s declarative API.\n\n## Event Registration\n\nBy default, the above example does not automatically do anything. Depending on\nthe context, you can use one of two registration hooks:\n`register_sqlalchemy_events` or `register_alembic_events`.\n\n### `register_sqlalchemy_events`\n\nThis registers events in SQLAlchemy\'s event system such that a\n`metadata.create_all(...)` call will create the declared database objects.\n\n```python\nfrom sqlalchemy_declarative_extensions import register_sqlalchemy_events\n\nmetadata = Base.metadata  # Given the example above.\nregister_sqlalchemy_events(metadata)\n# Which is equivalent to...\nregister_sqlalchemy_events(metadata, schemas=False, roles=False, grants=False, rows=False)\n```\n\nAll object types are opt in, and should be explicitly included in order to get\nregistered.\n\nPractically, this is to avoid issues with testing. In **most** cases the\n`metadata.create_all` call will be run in tests, a context where it\'s more\nlikely that you dont **need** grants or grants, and where parallel test\nexecution could lead to issues with role or schema creation, depending on your\nsetup.\n\n### `register_alembic_events`\n\nThis registers comparators in Alembic\'s registration system such that an\n`alembic revision --autogenerate` command will diff the existing database state\nagainst the declared database objects, and issue statements to\ncreate/update/delete objects in order to match the declared state.\n\n```python\n# alembic\'s `env.py`\nfrom sqlalchemy_declarative_extensions import register_alembic_events\n\nregister_alembic_events()\n# Which is equivalent to...\nregister_sqlalchemy_events(schemas=True, roles=True, grants=True, rows=True)\n```\n\nAll object types are opt out but can be excluded.\n\nIn contrast to `register_sqlalchemy_events`, it\'s much more likely that you\'re\ndeclaring most of these object types in order to have alembic track them\n\n## Database support\n\nIn principle, this library **can** absolutely support any database supported by\nSQLAlchemy, and capable of being introspected enough to support detection of\ndifferent kinds of objects.\n\nAs you can see below, in reality the existence of implementations are going to\nbe purely driven by actual usage. The current maintainer(s) primarily use\nPostgreSQL and as such individual features for other databases will either\nsuffer or lack implementation.\n\n|               | Postgres | MySQL | SQLite | Snowflake |\n| ------------- | -------- | ----- | ------ | --------- |\n| Schema        | ✓        | N/A   | ✓      | ✓         |\n| View          | ✓        | ✓     | ✓      |           |\n| Role          | ✓        |       | N/A    |           |\n| Grant         | ✓        |       | N/A    |           |\n| Default Grant | ✓        |       | N/A    |           |\n| Function      | ✓        | *     |        |           |\n| Trigger       | ✓        | *     |        |           |\n| Row (data)    | ✓        | ✓     | ✓      | ✓         |\n| "Audit Table" | ✓        |       |        |           |\n\n**note** "Row" is implemented with pure SQLAlchemy concepts, so should work for\nany dialect that you can use SQLAlchemy to connect to.\n\nThe astrisks above note pending or provisional support through basic test cases.\nThe level of expertise in each dialects\' particular behaviors is not uniform,\nand deciding on the correct behavior for those dialects will require users to\nsubmit issues/fixes!\n\nSupporting a new dialect **can** be as simple as providing the\ndialect-dispatched implementations for detecting existing objects of the given\ntype. Very much the intent is that once a given object type is supported at all,\nthe comparison infrastructure for that type should make it straightforward to\nsupport other dialects. At the end of the day, this library is primarily\nproducing SQL statements, so in theory any dialect supporting a given object\ntype should be able to be supported.\n\nIn such cases (like Grants/Roles) that different dialects support wildly\ndifferent options/syntax, there are also patterns for defining dialect-specific\nobjects, to mediate any additional differences.\n\n## Alembic-utils\n\n[Alembic Utils](https://github.com/olirice/alembic_utils) is the primary library\nagainst which this library can be compared. At time of writing, **most** (but\nnot all) object types supported by alembic-utils are supported by this library.\nOne might begin to question when to use which library.\n\nBelow is a list of points on which the two libraries diverge. But note that you\n**can** certainly use both in tandem! It doesn\'t need to be one or the other,\nand certainly for any object types which do not overlap, you might **need** to\nuse both.\n\n- Database Support\n\n  - Alembic Utils seems to explicitly only support PostgreSQL.\n\n  - This library is designed to support any dialect (in theory). Certainly\n    PostgreSQL is **best** supported, but there does exist support for specific\n    kinds of objects to varying levels of support for SQLite and MySQL, so far.\n\n- Architecture\n\n  - Alembic Utils is directly tied to Alembic and does not support SQLAlchemy\'s\n    `MetaData.create_all`. It\'s also the responsibility of the user to\n    discover/register objects in alembic.\n\n  - This library **depends** only on SQLAlchemy, although it also supports\n    alembic. Support for `MetaData.create_all` can be important for creating all\n    object types in tests. It also is designed such that objects are registered\n    on the `MetaData` itself, so there is no need for any specific discovery\n    phase.\n\n- Scope\n\n  - Alembic Utils declares specific, individual objects. I.e. you instantiate\n    one specific `PGGrantTable` or `PGView` instance and Alembic know knows you\n    want that object to be created. It cannot drop objects it is not already\n    aware of.\n\n  - This library declares ths objects the system as a whole expects to exist.\n    Similar to Alembic\'s behavior on tables, it will (by default) detect any\n    **undeclared** objects that should not exist and drop them. That means, you\n    can rely on this object to ensure the state of your migrations matches the\n    state of your database exactly.\n\n- Migration history\n\n  - Alembic Utils imports and references its own objects in your migrations\n    history. This can be unfortunate, in that it deeply ties your migrations\n    history to alembic-utils.\n\n    (In fact, this can be a sticking point, trying to convert **away** from\n    `alembic_utils`, because it will attempt to drop all the (e.g `PGView`)\n    instances previously created when we replaced it with this library.)\n\n  - This library, by contrast, prefers to emit the raw SQL of the operation into\n    your migration. That means you know the exact commands that will execute in\n    your migration, which can be helpful in debugging failure. It also means, if\n    at any point you decide to stop use of the library (or pause a given type of\n    object, due to a bug), you can! This library\'s behaviors are primarily very\n    much `--autogenerate`-time only.\n\n- Abstraction Level\n\n  - Alembic Utils appears to define a very "literal" interface (for example,\n    `PGView` accepts the whole view definition as a raw literal string).\n\n  - This library tries to, as much as possible, provide a more abstracted\n    interface that enables more compatibility with SQLAlchemy (For example\n    `View` accepts SQLAlchemy objects which can be coerced into a `SELECT`). It\n    also tends towards "builder" interfaces which progressively produce a object\n    (Take a look at the `DefaultGrant` above, for an example of where that\'s\n    helpful).\n\nA separate note on conversion/compatibility. Where possible, this library tries\nto support alembic-utils native objects as stand-ins for the objects defined in\nthis library. For example, `alembic_utils.pg_view.PGView` can be declared\ninstead of a `sqlalchemy_declarative_extensions.View`, and we will internally\ncoerce it into the appropriate type. Hopefully this eases any transitional\ncosts, or issues using one or the other library.\n',
     'author': 'Dan Cardin',
     'author_email': 'ddcardin@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/dancardin/sqlalchemy-declarative-extensions',
```

### Comparing `sqlalchemy-declarative-extensions-0.8.0/PKG-INFO` & `sqlalchemy-declarative-extensions-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-declarative-extensions
-Version: 0.8.0
+Version: 0.8.1
 Summary: Library to declare additional kinds of objects not natively supported by SQLAlchemy/Alembic.
 Home-page: https://github.com/dancardin/sqlalchemy-declarative-extensions
 License: Apache-2.0
 Keywords: alembic,declarative,grant,mysql,postgresql,role,schema,sqlalchemy,view
 Author: Dan Cardin
 Author-email: ddcardin@gmail.com
 Requires-Python: >=3.8,<4
```


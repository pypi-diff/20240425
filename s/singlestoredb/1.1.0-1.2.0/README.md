# Comparing `tmp/singlestoredb-1.1.0.tar.gz` & `tmp/singlestoredb-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singlestoredb-1.1.0.tar", last modified: Thu Apr 18 15:00:25 2024, max compression
+gzip compressed data, was "singlestoredb-1.2.0.tar", last modified: Thu Apr 25 18:57:34 2024, max compression
```

## Comparing `singlestoredb-1.1.0.tar` & `singlestoredb-1.2.0.tar`

### file list

```diff
@@ -1,138 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.941615 singlestoredb-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-18 15:00:25.941615 singlestoredb-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   154182 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/accel.c
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-18 15:00:25.941615 singlestoredb-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.929615 singlestoredb-1.1.0/singlestoredb/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.929615 singlestoredb-1.1.0/singlestoredb/alchemy/
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/alchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    11625 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    44227 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.929615 singlestoredb-1.1.0/singlestoredb/functions/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/functions/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    31408 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/functions/dtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.933615 singlestoredb-1.1.0/singlestoredb/functions/ext/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/functions/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/functions/ext/arrow.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    39861 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/functions/ext/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/functions/ext/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/functions/ext/mmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    22306 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/functions/ext/rowdat_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/functions/ext/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18866 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/functions/signature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.933615 singlestoredb-1.1.0/singlestoredb/fusion/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/fusion/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)    21337 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/fusion/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.933615 singlestoredb-1.1.0/singlestoredb/fusion/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/fusion/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/fusion/handlers/stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/fusion/handlers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19643 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/fusion/handlers/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/fusion/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/fusion/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.933615 singlestoredb-1.1.0/singlestoredb/http/
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38818 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/http/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.933615 singlestoredb-1.1.0/singlestoredb/management/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/management/billing_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/management/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     8810 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/management/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/management/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/management/region.py
--rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/management/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    59380 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/management/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.933615 singlestoredb-1.1.0/singlestoredb/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/charset.py
--rw-r--r--   0 runner    (1001) docker     (127)    67380 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.937615 singlestoredb-1.1.0/singlestoredb/mysql/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/constants/CLIENT.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/constants/COMMAND.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/constants/CR.py
--rw-r--r--   0 runner    (1001) docker     (127)    12296 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/constants/ER.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/constants/FIELD_TYPE.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/constants/FLAG.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/constants/SERVER_STATUS.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)    26481 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/cursors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/err.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/optionfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.937615 singlestoredb-1.1.0/singlestoredb/mysql/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/test_DictCursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/test_SSCursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15465 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    32297 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/test_cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/test_err.py
--rw-r--r--   0 runner    (1001) docker     (127)    18965 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/test_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/test_load_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/test_nextset.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/test_optionfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.937615 singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.937615 singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    31414 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/mysql/times.py
--rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/pytest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.941615 singlestoredb-1.1.0/singlestoredb/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/empty.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.941615 singlestoredb-1.1.0/singlestoredb/tests/ext_funcs/
--rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/ext_funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/local_infile.csv
--rw-r--r--   0 runner    (1001) docker     (127)    16196 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test.sql
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test2.sql
--rwxr-xr-x   0 runner    (1001) docker     (127)    44180 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_basics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11184 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   111071 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_dbapi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1131 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    37357 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_ext_func.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    47695 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_ext_func_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15100 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_fusion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8580 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_http.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28223 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_plugin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6582 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_results.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4500 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_types.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28075 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_udf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10408 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/test_xdict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.941615 singlestoredb-1.1.0/singlestoredb/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24503 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/utils/convert_rows.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/utils/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/utils/mogrify.py
--rw-r--r--   0 runner    (1001) docker     (127)    15153 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/utils/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    12896 2024-04-18 15:00:04.000000 singlestoredb-1.1.0/singlestoredb/utils/xdict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:00:25.929615 singlestoredb-1.1.0/singlestoredb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-18 15:00:25.000000 singlestoredb-1.1.0/singlestoredb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-04-18 15:00:25.000000 singlestoredb-1.1.0/singlestoredb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:00:25.000000 singlestoredb-1.1.0/singlestoredb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 15:00:25.000000 singlestoredb-1.1.0/singlestoredb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-18 15:00:25.000000 singlestoredb-1.1.0/singlestoredb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-18 15:00:25.000000 singlestoredb-1.1.0/singlestoredb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.074437 singlestoredb-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-25 18:57:34.074437 singlestoredb-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   161827 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/accel.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-25 18:57:34.078437 singlestoredb-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.062437 singlestoredb-1.2.0/singlestoredb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.062437 singlestoredb-1.2.0/singlestoredb/alchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/alchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44392 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20681 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.066437 singlestoredb-1.2.0/singlestoredb/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/functions/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31408 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/functions/dtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.066437 singlestoredb-1.2.0/singlestoredb/functions/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/functions/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/functions/ext/arrow.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    40088 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/functions/ext/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/functions/ext/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/functions/ext/mmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22306 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/functions/ext/rowdat_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/functions/ext/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18866 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/functions/signature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.066437 singlestoredb-1.2.0/singlestoredb/fusion/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/fusion/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21581 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/fusion/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.066437 singlestoredb-1.2.0/singlestoredb/fusion/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/fusion/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13643 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/fusion/handlers/stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/fusion/handlers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25000 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/fusion/handlers/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/fusion/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/fusion/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.066437 singlestoredb-1.2.0/singlestoredb/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38818 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/http/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.066437 singlestoredb-1.2.0/singlestoredb/management/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/management/billing_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/management/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8810 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/management/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/management/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/management/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/management/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61632 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/management/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.070437 singlestoredb-1.2.0/singlestoredb/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/charset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67884 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.070437 singlestoredb-1.2.0/singlestoredb/mysql/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/constants/CLIENT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/constants/COMMAND.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/constants/CR.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12296 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/constants/ER.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/constants/EXTENDED_TYPE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/constants/FIELD_TYPE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/constants/FLAG.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/constants/SERVER_STATUS.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/constants/VECTOR_TYPE.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26527 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/cursors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/err.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/optionfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14451 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.070437 singlestoredb-1.2.0/singlestoredb/mysql/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/test_DictCursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/test_SSCursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15465 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32297 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/test_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/test_err.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18965 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/test_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/test_load_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/test_nextset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/test_optionfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.070437 singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.070437 singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31414 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/times.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.074437 singlestoredb-1.2.0/singlestoredb/notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/notebook/_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/pytest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.074437 singlestoredb-1.2.0/singlestoredb/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/empty.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.074437 singlestoredb-1.2.0/singlestoredb/tests/ext_funcs/
+-rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/ext_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/local_infile.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    17679 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test2.sql
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44180 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_basics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11184 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   117405 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_dbapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1131 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37357 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_ext_func.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    47695 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_ext_func_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15100 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_fusion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8580 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_http.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28223 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_plugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6582 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_results.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4500 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_types.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28075 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_udf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10408 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_xdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.074437 singlestoredb-1.2.0/singlestoredb/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24503 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/utils/convert_rows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/utils/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/utils/mogrify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15153 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/utils/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12896 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/utils/xdict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.062437 singlestoredb-1.2.0/singlestoredb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-25 18:57:34.000000 singlestoredb-1.2.0/singlestoredb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-25 18:57:34.000000 singlestoredb-1.2.0/singlestoredb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:57:34.000000 singlestoredb-1.2.0/singlestoredb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 18:57:34.000000 singlestoredb-1.2.0/singlestoredb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-25 18:57:34.000000 singlestoredb-1.2.0/singlestoredb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-25 18:57:34.000000 singlestoredb-1.2.0/singlestoredb.egg-info/top_level.txt
```

### Comparing `singlestoredb-1.1.0/LICENSE` & `singlestoredb-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/PKG-INFO` & `singlestoredb-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singlestoredb
-Version: 1.1.0
+Version: 1.2.0
 Summary: Interface to the SingleStoreDB database and workspace management APIs
 Home-page: https://github.com/singlestore-labs/singlestoredb-python
 Author: SingleStore
 Author-email: support@singlestore.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `singlestoredb-1.1.0/README.md` & `singlestoredb-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/accel.c` & `singlestoredb-1.2.0/accel.c`

 * *Files 3% similar despite different names*

```diff
@@ -77,14 +77,29 @@
 #define MYSQL_TYPE_MEDIUM_BLOB 250
 #define MYSQL_TYPE_LONG_BLOB 251
 #define MYSQL_TYPE_BLOB 252
 #define MYSQL_TYPE_VAR_STRING 253
 #define MYSQL_TYPE_STRING 254
 #define MYSQL_TYPE_GEOMETRY 255
 
+// SingleStoreDB extended types
+#define MYSQL_TYPE_BSON 1001
+#define MYSQL_TYPE_FLOAT32_VECTOR_JSON 2001
+#define MYSQL_TYPE_FLOAT64_VECTOR_JSON 2002
+#define MYSQL_TYPE_INT8_VECTOR_JSON 2003
+#define MYSQL_TYPE_INT16_VECTOR_JSON 2004
+#define MYSQL_TYPE_INT32_VECTOR_JSON 2005
+#define MYSQL_TYPE_INT64_VECTOR_JSON 2006
+#define MYSQL_TYPE_FLOAT32_VECTOR 3001
+#define MYSQL_TYPE_FLOAT64_VECTOR 3002
+#define MYSQL_TYPE_INT8_VECTOR 3003
+#define MYSQL_TYPE_INT16_VECTOR 3004
+#define MYSQL_TYPE_INT32_VECTOR 3005
+#define MYSQL_TYPE_INT64_VECTOR 3006
+
 #define MYSQL_TYPE_CHAR MYSQL_TYPE_TINY
 #define MYSQL_TYPE_INTERVAL MYSQL_TYPE_ENUM
 
 #define MYSQL_COLUMN_NULL 251
 #define MYSQL_COLUMN_UNSIGNED_CHAR 251
 #define MYSQL_COLUMN_UNSIGNED_SHORT 252
 #define MYSQL_COLUMN_UNSIGNED_INT24 253
@@ -329,14 +344,16 @@
     int parse_json;
     PyObject *invalid_values;
 } MySQLAccelOptions;
 
 inline int IMAX(int a, int b) { return((a) > (b) ? a : b); }
 inline int IMIN(int a, int b) { return((a) < (b) ? a : b); }
 
+static PyObject *create_numpy_array(PyObject *py_memview, char *data_format, int data_type, PyObject *py_objs);
+
 char *_PyUnicode_AsUTF8(PyObject *unicode) {
     PyObject *bytes = PyUnicode_AsEncodedString(unicode, "utf-8", "strict");
     if (!bytes) return NULL;
 
     char *str = NULL;
     Py_ssize_t str_l = 0;
     if (PyBytes_AsStringAndSize(bytes, &str, &str_l) < 0) {
@@ -392,14 +409,22 @@
     PyObject *Row;
     PyObject *Series;
     PyObject *array;
     PyObject *vectorize;
     PyObject *DataFrame;
     PyObject *Table;
     PyObject *from_pylist;
+    PyObject *int8;
+    PyObject *int16;
+    PyObject *int32;
+    PyObject *int64;
+    PyObject *float32;
+    PyObject *float64;
+    PyObject *unpack;
+    PyObject *decode;
 } PyStrings;
 
 static PyStrings PyStr = {0};
 
 //
 // Cached Python functions
 //
@@ -413,25 +438,30 @@
     PyObject *collections_namedtuple;
     PyObject *numpy_array;
     PyObject *numpy_vectorize;
     PyObject *pandas_DataFrame;
     PyObject *polars_DataFrame;
     PyObject *pyarrow_Table;
     PyObject *pyarrow_Table_from_pylist;
+    PyObject *struct_unpack;
+    PyObject *bson_decode;
 } PyFunctions;
 
 static PyFunctions PyFunc = {0};
 
 //
 // Cached Python objects
 //
 typedef struct {
     PyObject *namedtuple_kwargs;
     PyObject *create_numpy_array_args;
     PyObject *create_numpy_array_kwargs;
+    PyObject *create_numpy_array_kwargs_vector[7];
+    PyObject *struct_unpack_args;
+    PyObject *bson_decode_args;
 } PyObjects;
 
 static PyObjects PyObj = {0};
 
 //
 // State
 //
@@ -494,14 +524,15 @@
     PyFunc.numpy_vectorize = PyObject_GetAttr(numpy_mod, PyStr.vectorize);
     if (!PyFunc.numpy_vectorize) goto error;
 
 exit:
     return 0;
 
 error:
+    PyErr_Clear();
     return -1;
 }
 
 
 int ensure_pandas() {
     if (PyFunc.pandas_DataFrame) goto exit;
 
@@ -512,14 +543,15 @@
     PyFunc.pandas_DataFrame = PyObject_GetAttr(pandas_mod, PyStr.DataFrame);
     if (!PyFunc.pandas_DataFrame) goto error;
 
 exit:
     return 0;
 
 error:
+    PyErr_Clear();
     return -1;
 }
 
 
 int ensure_polars() {
     if (PyFunc.polars_DataFrame) goto exit;
 
@@ -530,14 +562,15 @@
     PyFunc.polars_DataFrame = PyObject_GetAttr(polars_mod, PyStr.DataFrame);
     if (!PyFunc.polars_DataFrame) goto error;
 
 exit:
     return 0;
 
 error:
+    PyErr_Clear();
     return -1;
 }
 
 
 int ensure_pyarrow() {
     if (PyFunc.pyarrow_Table_from_pylist) goto exit;
 
@@ -551,14 +584,34 @@
     PyFunc.pyarrow_Table_from_pylist = PyObject_GetAttr(PyFunc.pyarrow_Table, PyStr.from_pylist);
     if (!PyFunc.pyarrow_Table_from_pylist) goto error;
 
 exit:
     return 0;
 
 error:
+    PyErr_Clear();
+    return -1;
+}
+
+
+int ensure_bson() {
+    if (PyFunc.bson_decode) goto exit;
+
+    // Import bson if it exists
+    PyObject *bson_mod = PyImport_ImportModule("bson");
+    if (!bson_mod) goto error;
+
+    PyFunc.bson_decode = PyObject_GetAttr(bson_mod, PyStr.decode);
+    if (!PyFunc.bson_decode) goto error;
+
+exit:
+    return 0;
+
+error:
+    PyErr_Clear();
     return -1;
 }
 
 
 static void State_clear_fields(StateObject *self) {
     if (!self) return;
     DESTROY(self->offsets);
@@ -764,17 +817,18 @@
         self->encodings[i] = (!py_encoding || py_encoding == Py_None) ?
                               NULL : _PyUnicode_AsUTF8(py_encoding);
 
         self->py_invalid_values[i] = (!py_invalid_value || py_invalid_value == Py_None) ?
                                       NULL : py_converter;
         Py_XINCREF(self->py_invalid_values[i]);
 
-        self->py_converters[i] = (!py_converter
-                                  // || py_converter == Py_None
-                                  || py_converter == py_default_converter) ?
+        self->py_converters[i] = ((!py_converter || py_converter == py_default_converter)
+                                   // TODO: Need C accelerated converters for extended types
+                                   // && self->type_codes[i] < 256
+                                   ) ?
                                  NULL : py_converter;
         Py_XINCREF(self->py_converters[i]);
     }
 
     // Loop over all data packets.
     self->py_conn = PyObject_GetAttr(py_res, PyStr.connection);
     if (!self->py_conn) goto error;
@@ -1416,15 +1470,18 @@
     char *orig_out = NULL;
     unsigned long long out_l = 0;
     unsigned long long orig_out_l = 0;
     int is_null = 0;
     PyObject *py_result = NULL;
     PyObject *py_item = NULL;
     PyObject *py_str = NULL;
+    PyObject *py_memview = NULL;
     char end = '\0';
+    char *cast_type_codes[] = {"", "f", "d", "b", "h", "l", "q"};
+    int item_type_lengths[] = {0, 4, 8, 1, 2, 4, 8};
 
     int sign = 1;
     int year = 0;
     int month = 0;
     int day = 0;
     int hour = 0;
     int minute = 0;
@@ -1432,15 +1489,15 @@
     int microsecond = 0;
 
     switch (py_state->options.results_type) {
     case ACCEL_OUT_DICTS:
     case ACCEL_OUT_ARROW:
         py_result = PyDict_New();
         break;
-   case ACCEL_OUT_STRUCTSEQUENCES: {
+    case ACCEL_OUT_STRUCTSEQUENCES: {
         if (!py_state->structsequence) goto error;
         py_result = PyStructSequence_New(py_state->structsequence);
         break;
         }
     case ACCEL_OUT_NAMEDTUPLES:
         if (!py_state->py_namedtuple) goto error;
         if (!py_state->py_namedtuple_args) goto error;
@@ -1661,31 +1718,110 @@
                 case MYSQL_TYPE_BLOB:
                 case MYSQL_TYPE_GEOMETRY:
                 case MYSQL_TYPE_ENUM:
                 case MYSQL_TYPE_SET:
                 case MYSQL_TYPE_VARCHAR:
                 case MYSQL_TYPE_VAR_STRING:
                 case MYSQL_TYPE_STRING:
+                case MYSQL_TYPE_FLOAT32_VECTOR_JSON:
+                case MYSQL_TYPE_FLOAT64_VECTOR_JSON:
+                case MYSQL_TYPE_INT8_VECTOR_JSON:
+                case MYSQL_TYPE_INT16_VECTOR_JSON:
+                case MYSQL_TYPE_INT32_VECTOR_JSON:
+                case MYSQL_TYPE_INT64_VECTOR_JSON:
                     if (!py_state->encodings[i]) {
                         py_item = PyBytes_FromStringAndSize(out, out_l);
                         if (!py_item) goto error;
                         break;
                     }
 
                     py_item = PyUnicode_Decode(out, out_l, py_state->encodings[i], py_state->encoding_errors);
                     if (!py_item) goto error;
 
                     // Parse JSON string.
-                    if (py_state->type_codes[i] == MYSQL_TYPE_JSON && py_state->options.parse_json) {
+                    if ((py_state->type_codes[i] == MYSQL_TYPE_JSON && py_state->options.parse_json)
+                        || (py_state->type_codes[i] >= MYSQL_TYPE_FLOAT32_VECTOR_JSON
+                            && py_state->type_codes[i] <= MYSQL_TYPE_INT64_VECTOR_JSON)) {
                         py_str = py_item;
                         py_item = PyObject_CallFunctionObjArgs(PyFunc.json_loads, py_str, NULL);
                         Py_CLEAR(py_str);
                         if (!py_item) goto error;
                     }
 
+                    if (ensure_numpy() == 0) {
+                        switch (py_state->type_codes[i]) {
+                        case MYSQL_TYPE_FLOAT32_VECTOR_JSON:
+                        case MYSQL_TYPE_FLOAT64_VECTOR_JSON:
+                        case MYSQL_TYPE_INT8_VECTOR_JSON:
+                        case MYSQL_TYPE_INT16_VECTOR_JSON:
+                        case MYSQL_TYPE_INT32_VECTOR_JSON:
+                        case MYSQL_TYPE_INT64_VECTOR_JSON:
+                            CHECKRC(PyTuple_SetItem(PyObj.create_numpy_array_args, 0, py_item));
+                            py_item = PyObject_Call(
+                                PyFunc.numpy_array,
+                                PyObj.create_numpy_array_args,
+                                PyObj.create_numpy_array_kwargs_vector[py_state->type_codes[i] % 1000]
+                            );
+                            if (!py_item) goto error;
+                        }
+                    }
+
+                    break;
+
+                case MYSQL_TYPE_FLOAT32_VECTOR:
+                case MYSQL_TYPE_FLOAT64_VECTOR:
+                case MYSQL_TYPE_INT8_VECTOR:
+                case MYSQL_TYPE_INT16_VECTOR:
+                case MYSQL_TYPE_INT32_VECTOR:
+                case MYSQL_TYPE_INT64_VECTOR:
+                    if (ensure_numpy() == 0) {
+                        py_memview = PyMemoryView_FromMemory(out, out_l, PyBUF_WRITE);
+                        if (!py_memview) goto error;
+
+                        py_item = create_numpy_array(
+                            py_memview,
+                            cast_type_codes[py_state->type_codes[i] % 1000],
+                            py_state->type_codes[i],
+                            NULL
+                        );
+                        Py_CLEAR(py_memview);
+                        if (!py_item) goto error;
+
+                    } else {
+                        py_memview = PyBytes_FromStringAndSize(out, out_l);
+                        if (!py_memview) goto error;
+
+                        CHECKRC(PyTuple_SetItem(PyObj.struct_unpack_args, 0,
+                                                PyUnicode_FromFormat("<%l%s", out_l / item_type_lengths[i], cast_type_codes[i])));
+                        CHECKRC(PyTuple_SetItem(PyObj.struct_unpack_args, 1, py_memview));
+
+                        py_item = PyObject_Call(
+                            PyFunc.struct_unpack,
+                            PyObj.struct_unpack_args,
+                            NULL
+                        );
+                        if (!py_item) goto error;
+                    }
+
+                    break;
+
+                case MYSQL_TYPE_BSON:
+                    py_item = PyBytes_FromStringAndSize(out, out_l);
+                    if (!py_item) goto error;
+
+                    if (ensure_bson() == 0) {
+                        CHECKRC(PyTuple_SetItem(PyObj.bson_decode_args, 0, py_item));
+                        py_item = PyObject_Call(
+                            PyFunc.bson_decode,
+                            PyObj.bson_decode_args,
+                            NULL
+                        );
+                        if (!py_item) goto error;
+                    }
+
                     break;
 
                 default:
                     PyErr_Format(PyExc_TypeError, "unknown type code: %ld",
                                  py_state->type_codes[i], NULL);
                     goto error;
                 }
@@ -4466,23 +4602,33 @@
     PyStr.Row = PyUnicode_FromString("Row");
     PyStr.Series = PyUnicode_FromString("Series");
     PyStr.array = PyUnicode_FromString("array");
     PyStr.vectorize = PyUnicode_FromString("vectorize");
     PyStr.DataFrame = PyUnicode_FromString("DataFrame");
     PyStr.Table = PyUnicode_FromString("Table");
     PyStr.from_pylist = PyUnicode_FromString("from_pylist");
+    PyStr.int8 = PyUnicode_FromString("int8");
+    PyStr.int16 = PyUnicode_FromString("int16");
+    PyStr.int32 = PyUnicode_FromString("int32");
+    PyStr.int64 = PyUnicode_FromString("int64");
+    PyStr.float32 = PyUnicode_FromString("float32");
+    PyStr.float64 = PyUnicode_FromString("float64");
+    PyStr.unpack = PyUnicode_FromString("unpack");
+    PyStr.decode = PyUnicode_FromString("decode");
 
     PyObject *decimal_mod = PyImport_ImportModule("decimal");
     if (!decimal_mod) goto error;
     PyObject *datetime_mod = PyImport_ImportModule("datetime");
     if (!datetime_mod) goto error;
     PyObject *json_mod = PyImport_ImportModule("json");
     if (!json_mod) goto error;
     PyObject *collections_mod = PyImport_ImportModule("collections");
     if (!collections_mod) goto error;
+    PyObject *struct_mod = PyImport_ImportModule("struct");
+    if (!struct_mod) goto error;
 
     PyFunc.decimal_Decimal = PyObject_GetAttr(decimal_mod, PyStr.Decimal);
     if (!PyFunc.decimal_Decimal) goto error;
     PyFunc.datetime_date = PyObject_GetAttr(datetime_mod, PyStr.date);
     if (!PyFunc.datetime_date) goto error;
     PyFunc.datetime_timedelta = PyObject_GetAttr(datetime_mod, PyStr.timedelta);
     if (!PyFunc.datetime_timedelta) goto error;
@@ -4490,14 +4636,16 @@
     if (!PyFunc.datetime_time) goto error;
     PyFunc.datetime_datetime = PyObject_GetAttr(datetime_mod, PyStr.datetime);
     if (!PyFunc.datetime_datetime) goto error;
     PyFunc.json_loads = PyObject_GetAttr(json_mod, PyStr.loads);
     if (!PyFunc.json_loads) goto error;
     PyFunc.collections_namedtuple = PyObject_GetAttr(collections_mod, PyStr.namedtuple);
     if (!PyFunc.collections_namedtuple) goto error;
+    PyFunc.struct_unpack = PyObject_GetAttr(struct_mod, PyStr.unpack);
+    if (!PyFunc.struct_unpack) goto error;
 
     PyObj.namedtuple_kwargs = PyDict_New();
     if (!PyObj.namedtuple_kwargs) goto error;
     if (PyDict_SetItemString(PyObj.namedtuple_kwargs, "rename", Py_True)) {
         goto error;
     }
 
@@ -4506,12 +4654,49 @@
 
     PyObj.create_numpy_array_kwargs = PyDict_New();
     if (!PyObj.create_numpy_array_kwargs) goto error;
     if (PyDict_SetItemString(PyObj.create_numpy_array_kwargs, "copy", Py_False)) {
         goto error;
     }
 
+    PyObj.create_numpy_array_kwargs_vector[1] = PyDict_New();
+    if (!PyObj.create_numpy_array_kwargs_vector[1]) goto error;
+    if (PyDict_SetItemString(PyObj.create_numpy_array_kwargs_vector[1], "dtype", PyStr.float32)) {
+        goto error;
+    }
+    PyObj.create_numpy_array_kwargs_vector[2] = PyDict_New();
+    if (!PyObj.create_numpy_array_kwargs_vector[2]) goto error;
+    if (PyDict_SetItemString(PyObj.create_numpy_array_kwargs_vector[2], "dtype", PyStr.float64)) {
+        goto error;
+    }
+    PyObj.create_numpy_array_kwargs_vector[3] = PyDict_New();
+    if (!PyObj.create_numpy_array_kwargs_vector[3]) goto error;
+    if (PyDict_SetItemString(PyObj.create_numpy_array_kwargs_vector[3], "dtype", PyStr.int8)) {
+        goto error;
+    }
+    PyObj.create_numpy_array_kwargs_vector[4] = PyDict_New();
+    if (!PyObj.create_numpy_array_kwargs_vector[4]) goto error;
+    if (PyDict_SetItemString(PyObj.create_numpy_array_kwargs_vector[4], "dtype", PyStr.int16)) {
+        goto error;
+    }
+    PyObj.create_numpy_array_kwargs_vector[5] = PyDict_New();
+    if (!PyObj.create_numpy_array_kwargs_vector[5]) goto error;
+    if (PyDict_SetItemString(PyObj.create_numpy_array_kwargs_vector[5], "dtype", PyStr.int32)) {
+        goto error;
+    }
+    PyObj.create_numpy_array_kwargs_vector[6] = PyDict_New();
+    if (!PyObj.create_numpy_array_kwargs_vector[6]) goto error;
+    if (PyDict_SetItemString(PyObj.create_numpy_array_kwargs_vector[6], "dtype", PyStr.int64)) {
+        goto error;
+    }
+
+    PyObj.struct_unpack_args = PyTuple_New(2);
+    if (!PyObj.struct_unpack_args) goto error;
+
+    PyObj.bson_decode_args = PyTuple_New(1);
+    if (!PyObj.bson_decode_args) goto error;
+
     return PyModule_Create(&_singlestoredb_accelmodule);
 
 error:
     return NULL;
 }
```

### Comparing `singlestoredb-1.1.0/setup.cfg` & `singlestoredb-1.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = singlestoredb
-version = 1.1.0
+version = 1.2.0
 description = Interface to the SingleStoreDB database and workspace management APIs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/singlestore-labs/singlestoredb-python
 author = SingleStore
 author_email = support@singlestore.com
 license = Apache-2.0
```

### Comparing `singlestoredb-1.1.0/setup.py` & `singlestoredb-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/__init__.py` & `singlestoredb-1.2.0/singlestoredb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 >>> cur = conn.cursor()
 >>> cur.execute('select * from customers')
 >>> for row in cur:
 ...     print(row)
 
 """
 
-__version__ = '1.1.0'
+__version__ = '1.2.0'
 
 from typing import Any
 
 from .config import options, get_option, set_option, describe_option
 from .connection import connect, apilevel, threadsafety, paramstyle
 from .exceptions import (
     Warning, Error, InterfaceError, DatabaseError, OperationalError,
```

### Comparing `singlestoredb-1.1.0/singlestoredb/alchemy/__init__.py` & `singlestoredb-1.2.0/singlestoredb/alchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/auth.py` & `singlestoredb-1.2.0/singlestoredb/auth.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/config.py` & `singlestoredb-1.2.0/singlestoredb/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,14 +212,20 @@
 register_option(
     'track_env', 'bool', check_bool, False,
     'Should connections track the SINGLESTOREDB_URL environment variable?',
     environ='SINGLESTOREDB_TRACK_ENV',
 )
 
 register_option(
+    'enable_extended_data_types', 'bool', check_bool, True,
+    'Should extended data types (BSON, vector) be enabled?',
+    environ='SINGLESTOREDB_ENABLE_EXTENDED_DATA_TYPES',
+)
+
+register_option(
     'fusion.enabled', 'bool', check_bool, False,
     'Should Fusion SQL queries be enabled?',
     environ='SINGLESTOREDB_FUSION_ENABLED',
 )
 
 #
 # Query results options
```

### Comparing `singlestoredb-1.1.0/singlestoredb/connection.py` & `singlestoredb-1.2.0/singlestoredb/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1281,14 +1281,15 @@
     conn_attrs: Optional[Dict[str, str]] = None,
     multi_statements: Optional[bool] = None,
     connect_timeout: Optional[int] = None,
     nan_as_null: Optional[bool] = None,
     inf_as_null: Optional[bool] = None,
     encoding_errors: Optional[str] = None,
     track_env: Optional[bool] = None,
+    enable_extended_data_types: Optional[bool] = None,
 ) -> Connection:
     """
     Return a SingleStoreDB connection.
 
     Parameters
     ----------
     host : str, optional
@@ -1357,14 +1358,16 @@
     inf_as_null : bool, optional
         Should Inf values be treated as NULLs when used in parameter
         substitutions including uploaded data?
     encoding_errors : str, optional
         The error handler name for value decoding errors
     track_env : bool, optional
         Should the connection track the SINGLESTOREDB_URL environment variable?
+    enable_extended_data_types : bool, optional
+        Should extended data types (BSON, vector) be enabled?
 
     Examples
     --------
     Standard database connection
 
     >>> conn = s2.connect('me:p455w0rd@s2-host.com/my_db')
```

### Comparing `singlestoredb-1.1.0/singlestoredb/exceptions.py` & `singlestoredb-1.2.0/singlestoredb/exceptions.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/functions/decorator.py` & `singlestoredb-1.2.0/singlestoredb/functions/decorator.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/functions/dtypes.py` & `singlestoredb-1.2.0/singlestoredb/functions/dtypes.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/functions/ext/arrow.py` & `singlestoredb-1.2.0/singlestoredb/functions/ext/arrow.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/functions/ext/asgi.py` & `singlestoredb-1.2.0/singlestoredb/functions/ext/asgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -451,25 +451,31 @@
                             continue
                         name = x._singlestoredb_attrs.get('name', x.__name__)
                         external_functions[x.__name__] = x
                         func, info = make_func(name, x)
                         endpoints[name.encode('utf-8')] = func, info
 
                 # Fully qualified function name
-                else:
+                elif '.' in funcs:
                     pkg_path, func_names = funcs.rsplit('.', 1)
                     pkg = importlib.import_module(pkg_path)
 
+                    if pkg is None:
+                        raise RuntimeError(f'Could not locate module: {pkg}')
+
                     # Add endpoint for each exported function
                     for name, alias in get_func_names(func_names):
                         item = getattr(pkg, name)
                         external_functions[name] = item
                         func, info = make_func(alias, item)
                         endpoints[alias.encode('utf-8')] = func, info
 
+                else:
+                    raise RuntimeError(f'Could not locate module: {funcs}')
+
             elif isinstance(funcs, ModuleType):
                 for x in vars(funcs).values():
                     if not hasattr(x, '_singlestoredb_attrs'):
                         continue
                     name = x._singlestoredb_attrs.get('name', x.__name__)
                     external_functions[x.__name__] = x
                     func, info = make_func(name, x)
```

### Comparing `singlestoredb-1.1.0/singlestoredb/functions/ext/json.py` & `singlestoredb-1.2.0/singlestoredb/functions/ext/json.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/functions/ext/mmap.py` & `singlestoredb-1.2.0/singlestoredb/functions/ext/mmap.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/functions/ext/rowdat_1.py` & `singlestoredb-1.2.0/singlestoredb/functions/ext/rowdat_1.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/functions/ext/utils.py` & `singlestoredb-1.2.0/singlestoredb/functions/ext/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/functions/signature.py` & `singlestoredb-1.2.0/singlestoredb/functions/signature.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/fusion/graphql.py` & `singlestoredb-1.2.0/singlestoredb/fusion/graphql.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/fusion/handler.py` & `singlestoredb-1.2.0/singlestoredb/fusion/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,38 +216,38 @@
         else:
             out.append(line.strip())
     return '\n'.join(out)
 
 
 def _to_markdown(txt: str) -> str:
     """Convert formatting to markdown."""
+    txt = re.sub(r'`([^`]+)\s+\<([^\>]+)>`_', r'[\1](\2)', txt)
     txt = txt.replace('``', '`')
 
     # Format code blocks
     lines = re.split(r'\n', txt)
     out = []
     while lines:
         line = lines.pop(0)
         if line.endswith('::'):
-            out.append(line[:-2])
+            out.append(line[:-2] + '.')
             code = []
             while lines and (not lines[0].strip() or lines[0].startswith(' ')):
                 code.append(lines.pop(0).rstrip())
-            out.extend(['```sql', '\n'.join(code).rstrip(), '```\n'])
+            code_str = re.sub(r'^\s*\n', r'', '\n'.join(code).rstrip())
+            out.extend([f'```sql\n{code_str}\n```\n'])
         else:
             out.append(line)
 
     return '\n'.join(out)
 
 
 def build_help(syntax: str, grammar: str) -> str:
     """Build full help text."""
-    syntax = re.sub(r'\s*\n+\s*', r' ', syntax.strip())
-
-    cmd = re.match(r'([A-Z0-9_ ]+)', syntax)
+    cmd = re.match(r'([A-Z0-9_ ]+)', syntax.strip())
     if not cmd:
         raise ValueError(f'no command found: {syntax}')
 
     out = [f'# {cmd.group(1)}\n\n']
 
     sections: Dict[str, str] = {}
     grammar = textwrap.dedent(grammar.rstrip())
@@ -260,33 +260,39 @@
             key = txt.pop(0)
             value = txt.pop(0)
             sections[key.lower()] = _to_markdown(value).strip()
 
     if 'description' in sections:
         out.extend([sections['description'], '\n\n'])
 
-    out.extend(['## Syntax\n```sql\n', syntax, '\n```\n\n'])
+    out.append(f'## Syntax\n\n```sql{syntax}\n```\n\n')
 
     if 'arguments' in sections:
         out.extend([
             '## Arguments\n\n',
             _format_arguments(sections['arguments']),
             '\n\n',
         ])
+    if 'argument' in sections:
+        out.extend([
+            '## Argument\n\n',
+            _format_arguments(sections['argument']),
+            '\n\n',
+        ])
 
     if 'remarks' in sections:
-        out.extend(['## Remarks\n', sections['remarks'], '\n\n'])
+        out.extend(['## Remarks\n\n', sections['remarks'], '\n\n'])
 
     if 'examples' in sections:
         out.extend(['## Examples\n\n', _format_examples(sections['examples']), '\n\n'])
     elif 'example' in sections:
         out.extend(['## Example\n\n', _format_examples(sections['example']), '\n\n'])
 
     if 'see also' in sections:
-        out.extend(['## See Also\n', sections['see also'], '\n\n'])
+        out.extend(['## See Also\n\n', sections['see also'], '\n\n'])
 
     return ''.join(out).rstrip() + '\n'
 
 
 def strip_comments(grammar: str) -> str:
     """Strip comments from grammar."""
     desc_re = re.compile(r'(^\s*Description\s*^\s*-----------\s*$)', flags=re.M)
```

### Comparing `singlestoredb-1.1.0/singlestoredb/fusion/handlers/utils.py` & `singlestoredb-1.2.0/singlestoredb/fusion/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/fusion/registry.py` & `singlestoredb-1.2.0/singlestoredb/fusion/registry.py`

 * *Files 5% similar despite different names*

```diff
@@ -119,25 +119,36 @@
     SHOW FUSION COMMANDS [ like ];
 
     # LIKE pattern
     like = LIKE '<pattern>'
 
     Description
     -----------
-    Display all Fusion SQL commands.
+    Displays a list of all the Fusion commands.
+
+    Arguments
+    ---------
+    * `<pattern>``: A pattern similar to SQL LIKE clause. Uses ``%`` as
+      the wildcard character.
 
     Remarks
     -------
-    * ``LIKE`` indicates a pattern of commands to display. ``%`` is a wildcard.
+    * Use the ``LIKE`` clause to specify a pattern and return only the
+      commands that match the specified pattern.
 
     Example
     -------
-    Display all commands starting with 'SHOW'::
+    The following command returns all the Fusion commands that start
+    with 'SHOW'::
+
+        SHOW FUSION COMMANDS LIKE 'SHOW%'
 
-        SHOW FUSION COMMANDS LIKE 'SHOW%';
+    See Also
+    --------
+    * ``SHOW FUSION HELP``
 
     """
 
     def run(self, params: Dict[str, Any]) -> Optional[result.FusionSQLResult]:
         res = result.FusionSQLResult()
         res.add_field('Command', result.STRING)
 
@@ -163,21 +174,22 @@
     # Query to show grammar for
     for_query = FOR '<query>'
 
     Description
     -----------
     Show the full grammar of a Fusion SQL command for a given query.
 
-    Remarks
-    -------
-    * ``<query>`` is a string containing a Fusion SQL command.
+    Arguments
+    ---------
+    * ``<command>``: A Fusion command.
 
     Example
     -------
-    Display the full grammar of the ``CREATE WORKSPACE`` command::
+    The following command displays the grammar for the
+    ``CREATE WORKSPACE`` Fusion command::
 
         SHOW FUSION GRAMMAR FOR 'CREATE WORKSPACE';
 
     """
 
     def run(self, params: Dict[str, Any]) -> Optional[result.FusionSQLResult]:
         res = result.FusionSQLResult()
@@ -198,19 +210,24 @@
     SHOW FUSION HELP for_command;
 
     # Command to show help for
     for_command = FOR '<command>'
 
     Description
     -----------
-    Show the documentation for a Fusion SQL command.
+    Displays the documentation for a Fusion command.
+
+    Arguments
+    ---------
+    * ``<command>``: A Fusion command.
 
     Example
     -------
-    Display the help for the ``CREATE WORKSPACE`` command::
+    The following command displays the documentation for
+    the ``CREATE WORKSPACE`` Fusion command.
 
         SHOW FUSION HELP FOR 'CREATE WORKSPACE';
 
     """
 
     def run(self, params: Dict[str, Any]) -> Optional[result.FusionSQLResult]:
         handler = get_handler(params['for_command'])
```

### Comparing `singlestoredb-1.1.0/singlestoredb/fusion/result.py` & `singlestoredb-1.2.0/singlestoredb/fusion/result.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/http/__init__.py` & `singlestoredb-1.2.0/singlestoredb/http/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/http/connection.py` & `singlestoredb-1.2.0/singlestoredb/http/connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/management/billing_usage.py` & `singlestoredb-1.2.0/singlestoredb/management/billing_usage.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/management/cluster.py` & `singlestoredb-1.2.0/singlestoredb/management/cluster.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/management/manager.py` & `singlestoredb-1.2.0/singlestoredb/management/manager.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/management/organization.py` & `singlestoredb-1.2.0/singlestoredb/management/organization.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,14 +117,18 @@
 
     See Also
     --------
     :attr:`WorkspaceManager.organization`
 
     """
 
+    id: str
+    name: str
+    firewall_ranges: List[str]
+
     def __init__(self, id: str, name: str, firewall_ranges: List[str]):
         """Use :attr:`WorkspaceManager.organization` instead."""
         #: Unique ID of the organization
         self.id = id
 
         #: Name of the organization
         self.name = name
```

### Comparing `singlestoredb-1.1.0/singlestoredb/management/region.py` & `singlestoredb-1.2.0/singlestoredb/management/region.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/management/utils.py` & `singlestoredb-1.2.0/singlestoredb/management/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,25 +290,25 @@
     cap_first: bool = False,
 ) -> Optional[Dict[str, Any]]:
     """Convert snake-case keys to camel-case keys."""
     if s is None:
         return None
     out = {}
     for k, v in s.items():
-        if isinstance(s, Mapping):
+        if isinstance(v, Mapping):
             out[str(snake_to_camel(k))] = snake_to_camel_dict(v, cap_first=cap_first)
         else:
             out[str(snake_to_camel(k))] = v
     return out
 
 
 def camel_to_snake_dict(s: Optional[Mapping[str, Any]]) -> Optional[Dict[str, Any]]:
     """Convert camel-case keys to snake-case keys."""
     if s is None:
         return None
     out = {}
     for k, v in s.items():
-        if isinstance(s, Mapping):
+        if isinstance(v, Mapping):
             out[str(camel_to_snake(k))] = camel_to_snake_dict(v)
         else:
             out[str(camel_to_snake(k))] = v
     return out
```

### Comparing `singlestoredb-1.1.0/singlestoredb/management/workspace.py` & `singlestoredb-1.2.0/singlestoredb/management/workspace.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,17 +30,61 @@
 from .utils import snake_to_camel
 from .utils import snake_to_camel_dict
 from .utils import to_datetime
 from .utils import ttl_property
 from .utils import vars_to_str
 
 
+def get_organization() -> Organization:
+    """Get the organization."""
+    return manage_workspaces().organization
+
+
 def get_secret(name: str) -> str:
     """Get a secret from the organization."""
-    return manage_workspaces().organization.get_secret(name).value
+    return get_organization().get_secret(name).value
+
+
+def get_workspace_group(
+    workspace_group: Optional[Union[WorkspaceGroup, str]] = None,
+) -> WorkspaceGroup:
+    """Get the stage for the workspace group."""
+    if isinstance(workspace_group, WorkspaceGroup):
+        return workspace_group
+    elif workspace_group:
+        return manage_workspaces().workspace_groups[workspace_group]
+    elif 'SINGLESTOREDB_WORKSPACE_GROUP' in os.environ:
+        return manage_workspaces().workspace_groups[
+            os.environ['SINGLESTOREDB_WORKSPACE_GROUP']
+        ]
+    raise RuntimeError('no workspace group specified')
+
+
+def get_stage(
+    workspace_group: Optional[Union[WorkspaceGroup, str]] = None,
+) -> Stage:
+    """Get the stage for the workspace group."""
+    return get_workspace_group(workspace_group).stage
+
+
+def get_workspace(
+    workspace_group: Optional[Union[WorkspaceGroup, str]] = None,
+    workspace: Optional[Union[Workspace, str]] = None,
+) -> Workspace:
+    """Get the workspaces for a workspace_group."""
+    if isinstance(workspace, Workspace):
+        return workspace
+    wg = get_workspace_group(workspace_group)
+    if workspace:
+        return wg.workspaces[workspace]
+    elif 'SINGLESTOREDB_WORKSPACE' in os.environ:
+        return wg.workspaces[
+            os.environ['SINGLESTOREDB_WORKSPACE']
+        ]
+    raise RuntimeError('no workspace group specified')
 
 
 class StageObject(object):
     """
     Stage file / folder object.
 
     This object is not instantiated directly. It is used in the results
@@ -922,30 +966,45 @@
     --------
     :meth:`WorkspaceManager.create_workspace`
     :meth:`WorkspaceManager.get_workspace`
     :attr:`WorkspaceManager.workspaces`
 
     """
 
+    name: str
+    id: str
+    group_id: str
+    size: str
+    state: str
+    created_at: Optional[datetime.datetime]
+    terminated_at: Optional[datetime.datetime]
+    endpoint: Optional[str]
+    auto_suspend: Optional[Dict[str, Any]]
+    cache_config: Optional[int]
+    deployment_type: Optional[str]
+    resume_attachments: Optional[List[Dict[str, Any]]]
+    scaling_progress: Optional[int]
+    last_resumed_at: Optional[datetime.datetime]
+
     def __init__(
         self,
         name: str,
         workspace_id: str,
         workspace_group: Union[str, 'WorkspaceGroup'],
         size: str,
         state: str,
         created_at: Union[str, datetime.datetime],
         terminated_at: Optional[Union[str, datetime.datetime]] = None,
         endpoint: Optional[str] = None,
         auto_suspend: Optional[Dict[str, Any]] = None,
         cache_config: Optional[int] = None,
         deployment_type: Optional[str] = None,
-        resume_attachments: Optional[Dict[str, Any]] = None,
+        resume_attachments: Optional[List[Dict[str, Any]]] = None,
         scaling_progress: Optional[int] = None,
-        last_resumed_at: Optional[str] = None,
+        last_resumed_at: Optional[Union[str, datetime.datetime]] = None,
     ):
         #: Name of the workspace
         self.name = name
 
         #: Unique ID of the workspace
         self.id = workspace_id
 
@@ -977,15 +1036,19 @@
         #: Multiplier for the persistent cache
         self.cache_config = cache_config
 
         #: Deployment type of the workspace
         self.deployment_type = deployment_type
 
         #: Database attachments
-        self.resume_attachments = camel_to_snake_dict(resume_attachments)
+        self.resume_attachments = [
+            camel_to_snake_dict(x)  # type: ignore
+            for x in resume_attachments or []
+            if x is not None
+        ]
 
         #: Current progress percentage for scaling the workspace
         self.scaling_progress = scaling_progress
 
         #: Timestamp when workspace was last resumed
         self.last_resumed_at = to_datetime(last_resumed_at)
 
@@ -1244,16 +1307,26 @@
     --------
     :meth:`WorkspaceManager.create_workspace_group`
     :meth:`WorkspaceManager.get_workspace_group`
     :attr:`WorkspaceManager.workspace_groups`
 
     """
 
+    name: str
+    id: str
+    created_at: Optional[datetime.datetime]
+    region: Optional[Region]
+    firewall_ranges: List[str]
+    terminated_at: Optional[datetime.datetime]
+    allow_all_traffic: bool
+
     def __init__(
-        self, name: str, id: str,
+        self,
+        name: str,
+        id: str,
         created_at: Union[str, datetime.datetime],
         region: Optional[Region],
         firewall_ranges: List[str],
         terminated_at: Optional[Union[str, datetime.datetime]],
         allow_all_traffic: Optional[bool],
     ):
         #: Name of the workspace group
@@ -1271,15 +1344,15 @@
         #: List of allowed incoming IP addresses / ranges
         self.firewall_ranges = firewall_ranges
 
         #: Timestamp of when the workspace group was terminated
         self.terminated_at = to_datetime(terminated_at)
 
         #: Should all traffic be allowed?
-        self.allow_all_traffic = allow_all_traffic
+        self.allow_all_traffic = allow_all_traffic or False
 
         self._manager: Optional[WorkspaceManager] = None
 
     def __str__(self) -> str:
         """Return string representation."""
         return vars_to_str(self)
```

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/__init__.py` & `singlestoredb-1.2.0/singlestoredb/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/_auth.py` & `singlestoredb-1.2.0/singlestoredb/mysql/_auth.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/charset.py` & `singlestoredb-1.2.0/singlestoredb/mysql/charset.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/connection.py` & `singlestoredb-1.2.0/singlestoredb/mysql/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,14 +255,16 @@
         Should NaN values be treated as NULLs in parameter substitution including
         uploading data?
     inf_as_null : bool, optional
         Should Inf values be treated as NULLs in parameter substitution including
         uploading data?
     track_env : bool, optional
         Should the connection track the SINGLESTOREDB_URL environment variable?
+    enable_extended_data_types : bool, optional
+        Should extended data types (BSON, vector) be enabled?
 
     See `Connection <https://www.python.org/dev/peps/pep-0249/#connection-objects>`_
     in the specification.
 
     """
 
     driver = 'mysql'
@@ -324,14 +326,15 @@
         driver=None,  # internal use
         conn_attrs=None,
         multi_statements=None,
         nan_as_null=None,
         inf_as_null=None,
         encoding_errors='strict',
         track_env=False,
+        enable_extended_data_types=True,
     ):
         BaseConnection.__init__(**dict(locals()))
 
         if db is not None and database is None:
             # We will raise warning in 2022 or later.
             # See https://github.com/PyMySQL/PyMySQL/issues/939
             # warnings.warn("'db' is deprecated, use 'database'", DeprecationWarning, 3)
@@ -605,14 +608,15 @@
             # do not overwrite the attributes that we set ourselves
             for k, v in conn_attrs.items():
                 if k not in self._connect_attrs:
                     self._connect_attrs[k] = v
 
         self._in_sync = False
         self._track_env = bool(track_env) or self.host == 'singlestore.com'
+        self._enable_extended_data_types = enable_extended_data_types
 
         if defer_connect or self._track_env:
             self._sock = None
         else:
             self.connect()
 
     @property
@@ -1066,14 +1070,22 @@
             self.set_character_set(self.charset, self.collation)
 
             if self.sql_mode is not None:
                 c = self.cursor()
                 c.execute('SET sql_mode=%s', (self.sql_mode,))
                 c.close()
 
+            if self._enable_extended_data_types:
+                c = self.cursor()
+                try:
+                    c.execute('SET @@SESSION.enable_extended_types_metadata=on')
+                except self.OperationalError:
+                    pass
+                c.close()
+
             if self.init_command is not None:
                 c = self.cursor()
                 c.execute(self.init_command)
                 c.close()
 
             if self.autocommit_mode is not None:
                 self.autocommit(self.autocommit_mode)
```

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/constants/CLIENT.py` & `singlestoredb-1.2.0/singlestoredb/mysql/constants/CLIENT.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/constants/COMMAND.py` & `singlestoredb-1.2.0/singlestoredb/mysql/constants/COMMAND.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/constants/CR.py` & `singlestoredb-1.2.0/singlestoredb/mysql/constants/CR.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/constants/ER.py` & `singlestoredb-1.2.0/singlestoredb/mysql/constants/ER.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/converters.py` & `singlestoredb-1.2.0/singlestoredb/mysql/converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/cursors.py` & `singlestoredb-1.2.0/singlestoredb/mysql/cursors.py`

 * *Files 1% similar despite different names*

```diff
@@ -413,18 +413,19 @@
         self.rowcount = result.affected_rows
         self.warning_count = result.warning_count
         # Affected rows is set to max int64 for compatibility with MySQLdb, but
         # the DB-API requires this value to be -1. This happens in unbuffered mode.
         if self.rowcount == 18446744073709551615:
             self.rowcount = -1
         self._description = result.description
-        self._format_schema = get_schema(
-            self.connection._results_type,
-            result.description,
-        )
+        if self._description:
+            self._format_schema = get_schema(
+                self.connection._results_type,
+                result.description,
+            )
         self.lastrowid = result.insert_id
         self._rows = result.rows
 
     def __iter__(self):
         self._check_executed()
 
         def fetchall_unbuffered_gen(_unchecked_fetchone=self._unchecked_fetchone):
```

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/err.py` & `singlestoredb-1.2.0/singlestoredb/mysql/err.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/optionfile.py` & `singlestoredb-1.2.0/singlestoredb/mysql/optionfile.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/protocol.py` & `singlestoredb-1.2.0/singlestoredb/mysql/protocol.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 import struct
 import sys
 
 from . import err
 from ..config import get_option
 from ..utils.results import Description
 from .charset import MBLENGTH
+from .constants import EXTENDED_TYPE
 from .constants import FIELD_TYPE
 from .constants import SERVER_STATUS
+from .constants import VECTOR_TYPE
 
 
 DEBUG = get_option('debug.connection')
 
 NULL_COLUMN = 251
 UNSIGNED_CHAR_COLUMN = 251
 UNSIGNED_SHORT_COLUMN = 252
@@ -260,24 +262,71 @@
         """
         self.catalog = self.read_length_coded_string()
         self.db = self.read_length_coded_string()
         self.table_name = self.read_length_coded_string().decode(encoding)
         self.org_table = self.read_length_coded_string().decode(encoding)
         self.name = self.read_length_coded_string().decode(encoding)
         self.org_name = self.read_length_coded_string().decode(encoding)
+        n_bytes = 0
         (
+            n_bytes,
             self.charsetnr,
             self.length,
             self.type_code,
             self.flags,
             self.scale,
-        ) = self.read_struct('<xHIBHBxx')
+        ) = self.read_struct('<BHIBHBxx')
+
         # 'default' is a length coded binary and is still in the buffer?
         # not used for normal result sets...
 
+        # Extended types
+        if n_bytes > 12:
+            ext_type_code = self.read_uint8()
+            if ext_type_code == EXTENDED_TYPE.NONE:
+                pass
+            elif ext_type_code == EXTENDED_TYPE.BSON:
+                self.type_code = FIELD_TYPE.BSON
+            elif ext_type_code == EXTENDED_TYPE.VECTOR:
+                (self.length, vec_type) = self.read_struct('<IB')
+                if vec_type == VECTOR_TYPE.FLOAT32:
+                    if self.charsetnr == 63:
+                        self.type_code = FIELD_TYPE.FLOAT32_VECTOR
+                    else:
+                        self.type_code = FIELD_TYPE.FLOAT32_VECTOR_JSON
+                elif vec_type == VECTOR_TYPE.FLOAT64:
+                    if self.charsetnr == 63:
+                        self.type_code = FIELD_TYPE.FLOAT64_VECTOR
+                    else:
+                        self.type_code = FIELD_TYPE.FLOAT64_VECTOR_JSON
+                elif vec_type == VECTOR_TYPE.INT8:
+                    if self.charsetnr == 63:
+                        self.type_code = FIELD_TYPE.INT8_VECTOR
+                    else:
+                        self.type_code = FIELD_TYPE.INT8_VECTOR_JSON
+                elif vec_type == VECTOR_TYPE.INT16:
+                    if self.charsetnr == 63:
+                        self.type_code = FIELD_TYPE.INT16_VECTOR
+                    else:
+                        self.type_code = FIELD_TYPE.INT16_VECTOR_JSON
+                elif vec_type == VECTOR_TYPE.INT32:
+                    if self.charsetnr == 63:
+                        self.type_code = FIELD_TYPE.INT32_VECTOR
+                    else:
+                        self.type_code = FIELD_TYPE.INT32_VECTOR_JSON
+                elif vec_type == VECTOR_TYPE.INT64:
+                    if self.charsetnr == 63:
+                        self.type_code = FIELD_TYPE.INT64_VECTOR
+                    else:
+                        self.type_code = FIELD_TYPE.INT64_VECTOR_JSON
+                else:
+                    raise TypeError(f'unrecognized vector data type: {vec_type}')
+            else:
+                raise TypeError(f'unrecognized extended data type: {ext_type_code}')
+
     def description(self):
         """Provides a 7-item tuple compatible with the Python PEP249 DB Spec."""
         return Description(
             self.name,
             self.type_code,
             None,  # TODO: display_length; should this be self.length?
             self.get_column_length(),  # 'internal_size'
```

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/tests/__init__.py` & `singlestoredb-1.2.0/singlestoredb/mysql/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/tests/base.py` & `singlestoredb-1.2.0/singlestoredb/mysql/tests/base.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/tests/conftest.py` & `singlestoredb-1.2.0/singlestoredb/mysql/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/tests/test_DictCursor.py` & `singlestoredb-1.2.0/singlestoredb/mysql/tests/test_DictCursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/tests/test_SSCursor.py` & `singlestoredb-1.2.0/singlestoredb/mysql/tests/test_SSCursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/tests/test_basic.py` & `singlestoredb-1.2.0/singlestoredb/mysql/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/tests/test_connection.py` & `singlestoredb-1.2.0/singlestoredb/mysql/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/tests/test_converters.py` & `singlestoredb-1.2.0/singlestoredb/mysql/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/tests/test_cursor.py` & `singlestoredb-1.2.0/singlestoredb/mysql/tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/tests/test_issues.py` & `singlestoredb-1.2.0/singlestoredb/mysql/tests/test_issues.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/tests/test_load_local.py` & `singlestoredb-1.2.0/singlestoredb/mysql/tests/test_load_local.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/tests/test_nextset.py` & `singlestoredb-1.2.0/singlestoredb/mysql/tests/test_nextset.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/tests/test_optionfile.py` & `singlestoredb-1.2.0/singlestoredb/mysql/tests/test_optionfile.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py` & `singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py` & `singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py` & `singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py` & `singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py` & `singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/pytest.py` & `singlestoredb-1.2.0/singlestoredb/pytest.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/tests/ext_funcs/__init__.py` & `singlestoredb-1.2.0/singlestoredb/tests/ext_funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/tests/test.sql` & `singlestoredb-1.2.0/singlestoredb/tests/test.sql`

 * *Files 18% similar despite different names*

```diff
@@ -602,8 +602,57 @@
 COLLATE='utf8_unicode_ci';
 
 
 INSERT INTO `badutf8` VALUES ('🥷🧙👻.eth');
 INSERT INTO `badutf8` VALUES ('🥒rick.eth');
 
 
+CREATE TABLE IF NOT EXISTS `f32_vectors` (
+    id INT(11),
+    a VECTOR(3)
+);
+INSERT INTO f32_vectors VALUES(1, '[0.267261237,0.534522474,0.801783681]');
+INSERT INTO f32_vectors VALUES(2, '[0.371390671,0.557085991,0.742781341]');
+INSERT INTO f32_vectors VALUES(3, '[-0.424264073,-0.565685451,0.707106829]');
+
+CREATE TABLE IF NOT EXISTS `f64_vectors` (
+    id INT(11),
+    a VECTOR(3, F64)
+);
+INSERT INTO f64_vectors VALUES(1, '[0.267261237,0.534522474,0.801783681]');
+INSERT INTO f64_vectors VALUES(2, '[0.371390671,0.557085991,0.742781341]');
+INSERT INTO f64_vectors VALUES(3, '[-0.424264073,-0.565685451,0.707106829]');
+
+CREATE TABLE `i8_vectors` (
+    id INT(11),
+    a VECTOR(3, I8)
+);
+INSERT INTO i8_vectors VALUES(1, '[1, 2, 3]');
+INSERT INTO i8_vectors VALUES(2, '[4, 5, 6]');
+INSERT INTO i8_vectors VALUES(3, '[-1, -4, 8]');
+
+CREATE TABLE `i16_vectors` (
+    id INT(11),
+    a VECTOR(3, I16)
+);
+INSERT INTO i16_vectors VALUES(1, '[1, 2, 3]');
+INSERT INTO i16_vectors VALUES(2, '[4, 5, 6]');
+INSERT INTO i16_vectors VALUES(3, '[-1, -4, 8]');
+
+CREATE TABLE `i32_vectors` (
+    id INT(11),
+    a VECTOR(3, I32)
+);
+INSERT INTO i32_vectors VALUES(1, '[1, 2, 3]');
+INSERT INTO i32_vectors VALUES(2, '[4, 5, 6]');
+INSERT INTO i32_vectors VALUES(3, '[-1, -4, 8]');
+
+CREATE TABLE `i64_vectors` (
+    id INT(11),
+    a VECTOR(3, I64)
+);
+INSERT INTO i64_vectors VALUES(1, '[1, 2, 3]');
+INSERT INTO i64_vectors VALUES(2, '[4, 5, 6]');
+INSERT INTO i64_vectors VALUES(3, '[-1, -4, 8]');
+
+
 COMMIT;
```

### Comparing `singlestoredb-1.1.0/singlestoredb/tests/test_basics.py` & `singlestoredb-1.2.0/singlestoredb/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/tests/test_config.py` & `singlestoredb-1.2.0/singlestoredb/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/tests/test_connection.py` & `singlestoredb-1.2.0/singlestoredb/tests/test_connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -2872,11 +2872,185 @@
         assert 'CreateTable' in out.columns, out.columns
         assert '`id` varchar(255)' in out.CreateTable[0], out.CreateTable[0]
         assert '`name` varchar(255)' in out.CreateTable[0], out.CreateTable[0]
         assert '`value` bigint(20)' in out.CreateTable[0], out.CreateTable[0]
 
         # out = self.conn.show.create_view('vname')
 
+    def test_f32_vectors(self):
+        if self.conn.driver in ['http', 'https']:
+            self.skipTest('Data API does not surface vector information')
+
+        self.cur.execute('show variables like "enable_extended_types_metadata"')
+        out = list(self.cur)
+        if not out or out[0][1].lower() == 'off':
+            self.skipTest('Database engine does not support extended types metadata')
+
+        self.cur.execute('select a from f32_vectors order by id')
+        out = list(self.cur)
+
+        assert out[0][0].dtype is np.dtype('float32')
+        assert out[1][0].dtype is np.dtype('float32')
+        assert out[2][0].dtype is np.dtype('float32')
+
+        np.testing.assert_array_equal(
+            out[0][0],
+            np.array([0.267261237, 0.534522474, 0.801783681], dtype=np.float32),
+        )
+        np.testing.assert_array_equal(
+            out[1][0],
+            np.array([0.371390671, 0.557085991, 0.742781341], dtype=np.float32),
+        )
+        np.testing.assert_array_equal(
+            out[2][0],
+            np.array([-0.424264073, -0.565685451, 0.707106829], dtype=np.float32),
+        )
+
+    def test_f64_vectors(self):
+        if self.conn.driver in ['http', 'https']:
+            self.skipTest('Data API does not surface vector information')
+
+        self.cur.execute('show variables like "enable_extended_types_metadata"')
+        out = list(self.cur)
+        if not out or out[0][1].lower() == 'off':
+            self.skipTest('Database engine does not support extended types metadata')
+
+        self.cur.execute('select a from f64_vectors order by id')
+        out = list(self.cur)
+
+        assert out[0][0].dtype is np.dtype('float64')
+        assert out[1][0].dtype is np.dtype('float64')
+        assert out[2][0].dtype is np.dtype('float64')
+
+        np.testing.assert_array_equal(
+            out[0][0],
+            np.array([0.267261237, 0.534522474, 0.801783681], dtype=np.float64),
+        )
+        np.testing.assert_array_equal(
+            out[1][0],
+            np.array([0.371390671, 0.557085991, 0.742781341], dtype=np.float64),
+        )
+        np.testing.assert_array_equal(
+            out[2][0],
+            np.array([-0.424264073, -0.565685451, 0.707106829], dtype=np.float64),
+        )
+
+    def test_i8_vectors(self):
+        if self.conn.driver in ['http', 'https']:
+            self.skipTest('Data API does not surface vector information')
+
+        self.cur.execute('show variables like "enable_extended_types_metadata"')
+        out = list(self.cur)
+        if not out or out[0][1].lower() == 'off':
+            self.skipTest('Database engine does not support extended types metadata')
+
+        self.cur.execute('select a from i8_vectors order by id')
+        out = list(self.cur)
+
+        assert out[0][0].dtype is np.dtype('int8')
+        assert out[1][0].dtype is np.dtype('int8')
+        assert out[2][0].dtype is np.dtype('int8')
+
+        np.testing.assert_array_equal(
+            out[0][0],
+            np.array([1, 2, 3], dtype=np.int8),
+        )
+        np.testing.assert_array_equal(
+            out[1][0],
+            np.array([4, 5, 6], dtype=np.int8),
+        )
+        np.testing.assert_array_equal(
+            out[2][0],
+            np.array([-1, -4, 8], dtype=np.int8),
+        )
+
+    def test_i16_vectors(self):
+        if self.conn.driver in ['http', 'https']:
+            self.skipTest('Data API does not surface vector information')
+
+        self.cur.execute('show variables like "enable_extended_types_metadata"')
+        out = list(self.cur)
+        if not out or out[0][1].lower() == 'off':
+            self.skipTest('Database engine does not support extended types metadata')
+
+        self.cur.execute('select a from i16_vectors order by id')
+        out = list(self.cur)
+
+        assert out[0][0].dtype is np.dtype('int16')
+        assert out[1][0].dtype is np.dtype('int16')
+        assert out[2][0].dtype is np.dtype('int16')
+
+        np.testing.assert_array_equal(
+            out[0][0],
+            np.array([1, 2, 3], dtype=np.int16),
+        )
+        np.testing.assert_array_equal(
+            out[1][0],
+            np.array([4, 5, 6], dtype=np.int16),
+        )
+        np.testing.assert_array_equal(
+            out[2][0],
+            np.array([-1, -4, 8], dtype=np.int16),
+        )
+
+    def test_i32_vectors(self):
+        if self.conn.driver in ['http', 'https']:
+            self.skipTest('Data API does not surface vector information')
+
+        self.cur.execute('show variables like "enable_extended_types_metadata"')
+        out = list(self.cur)
+        if not out or out[0][1].lower() == 'off':
+            self.skipTest('Database engine does not support extended types metadata')
+
+        self.cur.execute('select a from i32_vectors order by id')
+        out = list(self.cur)
+
+        assert out[0][0].dtype is np.dtype('int32')
+        assert out[1][0].dtype is np.dtype('int32')
+        assert out[2][0].dtype is np.dtype('int32')
+
+        np.testing.assert_array_equal(
+            out[0][0],
+            np.array([1, 2, 3], dtype=np.int32),
+        )
+        np.testing.assert_array_equal(
+            out[1][0],
+            np.array([4, 5, 6], dtype=np.int32),
+        )
+        np.testing.assert_array_equal(
+            out[2][0],
+            np.array([-1, -4, 8], dtype=np.int32),
+        )
+
+    def test_i64_vectors(self):
+        if self.conn.driver in ['http', 'https']:
+            self.skipTest('Data API does not surface vector information')
+
+        self.cur.execute('show variables like "enable_extended_types_metadata"')
+        out = list(self.cur)
+        if not out or out[0][1].lower() == 'off':
+            self.skipTest('Database engine does not support extended types metadata')
+
+        self.cur.execute('select a from i64_vectors order by id')
+        out = list(self.cur)
+
+        assert out[0][0].dtype is np.dtype('int64')
+        assert out[1][0].dtype is np.dtype('int64')
+        assert out[2][0].dtype is np.dtype('int64')
+
+        np.testing.assert_array_equal(
+            out[0][0],
+            np.array([1, 2, 3], dtype=np.int64),
+        )
+        np.testing.assert_array_equal(
+            out[1][0],
+            np.array([4, 5, 6], dtype=np.int64),
+        )
+        np.testing.assert_array_equal(
+            out[2][0],
+            np.array([-1, -4, 8], dtype=np.int64),
+        )
+
 
 if __name__ == '__main__':
     import nose2
     nose2.main()
```

### Comparing `singlestoredb-1.1.0/singlestoredb/tests/test_dbapi.py` & `singlestoredb-1.2.0/singlestoredb/tests/test_dbapi.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/tests/test_exceptions.py` & `singlestoredb-1.2.0/singlestoredb/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/tests/test_ext_func.py` & `singlestoredb-1.2.0/singlestoredb/tests/test_ext_func.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/tests/test_ext_func_data.py` & `singlestoredb-1.2.0/singlestoredb/tests/test_ext_func_data.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/tests/test_fusion.py` & `singlestoredb-1.2.0/singlestoredb/tests/test_fusion.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/tests/test_http.py` & `singlestoredb-1.2.0/singlestoredb/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/tests/test_management.py` & `singlestoredb-1.2.0/singlestoredb/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/tests/test_plugin.py` & `singlestoredb-1.2.0/singlestoredb/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/tests/test_results.py` & `singlestoredb-1.2.0/singlestoredb/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/tests/test_types.py` & `singlestoredb-1.2.0/singlestoredb/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/tests/test_udf.py` & `singlestoredb-1.2.0/singlestoredb/tests/test_udf.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/tests/test_xdict.py` & `singlestoredb-1.2.0/singlestoredb/tests/test_xdict.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/tests/utils.py` & `singlestoredb-1.2.0/singlestoredb/tests/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/types.py` & `singlestoredb-1.2.0/singlestoredb/types.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/utils/config.py` & `singlestoredb-1.2.0/singlestoredb/utils/config.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/utils/convert_rows.py` & `singlestoredb-1.2.0/singlestoredb/utils/convert_rows.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/utils/dtypes.py` & `singlestoredb-1.2.0/singlestoredb/utils/dtypes.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/utils/mogrify.py` & `singlestoredb-1.2.0/singlestoredb/utils/mogrify.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/utils/results.py` & `singlestoredb-1.2.0/singlestoredb/utils/results.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb/utils/xdict.py` & `singlestoredb-1.2.0/singlestoredb/utils/xdict.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.1.0/singlestoredb.egg-info/PKG-INFO` & `singlestoredb-1.2.0/singlestoredb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singlestoredb
-Version: 1.1.0
+Version: 1.2.0
 Summary: Interface to the SingleStoreDB database and workspace management APIs
 Home-page: https://github.com/singlestore-labs/singlestoredb-python
 Author: SingleStore
 Author-email: support@singlestore.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `singlestoredb-1.1.0/singlestoredb.egg-info/SOURCES.txt` & `singlestoredb-1.2.0/singlestoredb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -58,17 +58,19 @@
 singlestoredb/mysql/optionfile.py
 singlestoredb/mysql/protocol.py
 singlestoredb/mysql/times.py
 singlestoredb/mysql/constants/CLIENT.py
 singlestoredb/mysql/constants/COMMAND.py
 singlestoredb/mysql/constants/CR.py
 singlestoredb/mysql/constants/ER.py
+singlestoredb/mysql/constants/EXTENDED_TYPE.py
 singlestoredb/mysql/constants/FIELD_TYPE.py
 singlestoredb/mysql/constants/FLAG.py
 singlestoredb/mysql/constants/SERVER_STATUS.py
+singlestoredb/mysql/constants/VECTOR_TYPE.py
 singlestoredb/mysql/constants/__init__.py
 singlestoredb/mysql/tests/__init__.py
 singlestoredb/mysql/tests/base.py
 singlestoredb/mysql/tests/conftest.py
 singlestoredb/mysql/tests/test_DictCursor.py
 singlestoredb/mysql/tests/test_SSCursor.py
 singlestoredb/mysql/tests/test_basic.py
@@ -83,14 +85,16 @@
 singlestoredb/mysql/tests/thirdparty/__init__.py
 singlestoredb/mysql/tests/thirdparty/test_MySQLdb/__init__.py
 singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py
 singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py
 singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py
 singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py
 singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py
+singlestoredb/notebook/__init__.py
+singlestoredb/notebook/_objects.py
 singlestoredb/tests/__init__.py
 singlestoredb/tests/empty.sql
 singlestoredb/tests/local_infile.csv
 singlestoredb/tests/test.sql
 singlestoredb/tests/test2.sql
 singlestoredb/tests/test_basics.py
 singlestoredb/tests/test_config.py
```


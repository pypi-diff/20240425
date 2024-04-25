# Comparing `tmp/everysk_beta-1.3.656.tar.gz` & `tmp/everysk_beta-1.4.815.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "everysk_beta-1.3.656.tar", last modified: Thu Apr 25 17:05:36 2024, max compression
+gzip compressed data, was "everysk_beta-1.4.815.tar", last modified: Thu Apr 25 19:05:53 2024, max compression
```

## Comparing `everysk_beta-1.3.656.tar` & `everysk_beta-1.4.815.tar`

### file list

```diff
@@ -1,133 +1,187 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.595170 everysk_beta-1.3.656/
--rw-rw-r--   0 root         (0) root         (0)      312 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     7819 2024-04-25 17:05:36.595170 everysk_beta-1.3.656/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3431 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/README.md
--rw-r--r--   0 root         (0) root         (0)     2648 2024-04-25 17:05:32.000000 everysk_beta-1.3.656/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 17:05:36.595170 everysk_beta-1.3.656/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.583170 everysk_beta-1.3.656/src/
--rw-rw-r--   0 root         (0) root         (0)      653 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/src/__builtins__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.587170 everysk_beta-1.3.656/src/everysk/
--rw-rw-r--   0 root         (0) root         (0)      927 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6698 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/config.py
--rw-r--r--   0 root         (0) root         (0)     3105 2024-04-09 17:26:44.000000 everysk_beta-1.3.656/src/everysk/config.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.587170 everysk_beta-1.3.656/src/everysk/core/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.587170 everysk_beta-1.3.656/src/everysk/core/_tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/src/everysk/core/_tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2463 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/src/everysk/core/_tests/compress.py
--rw-r--r--   0 root         (0) root         (0)     8743 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/_tests/config.py
--rw-rw-r--   0 root         (0) root         (0)     3251 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/src/everysk/core/_tests/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    17440 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/_tests/fields.py
--rw-r--r--   0 root         (0) root         (0)    26824 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/_tests/firestore.py
--rw-r--r--   0 root         (0) root         (0)     8136 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/_tests/http.py
--rw-r--r--   0 root         (0) root         (0)    13085 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/_tests/log.py
--rw-rw-r--   0 root         (0) root         (0)      795 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/src/everysk/core/_tests/number.py
--rw-r--r--   0 root         (0) root         (0)    41630 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/_tests/object.py
--rw-r--r--   0 root         (0) root         (0)    13699 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/_tests/redis.py
--rw-rw-r--   0 root         (0) root         (0)     3631 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/src/everysk/core/_tests/slack.py
--rw-rw-r--   0 root         (0) root         (0)     3415 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/src/everysk/core/_tests/string.py
--rw-rw-r--   0 root         (0) root         (0)     5158 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/core/_tests/threads.py
--rw-r--r--   0 root         (0) root         (0)     2432 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/_tests/undefined.py
--rw-rw-r--   0 root         (0) root         (0)     1800 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/src/everysk/core/_tests/utils.py
--rw-rw-r--   0 root         (0) root         (0)    12441 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/src/everysk/core/_tests/workers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.587170 everysk_beta-1.3.656/src/everysk/core/cloud_function/
--rw-rw-r--   0 root         (0) root         (0)     2571 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/src/everysk/core/cloud_function/main.py
--rw-rw-r--   0 root         (0) root         (0)     3731 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/src/everysk/core/cloud_function/tests.py
--rw-r--r--   0 root         (0) root         (0)     2819 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/compress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.587170 everysk_beta-1.3.656/src/everysk/core/datetime/
--rw-rw-r--   0 root         (0) root         (0)      584 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/src/everysk/core/datetime/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1622 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/datetime/calendar.py
--rw-r--r--   0 root         (0) root         (0)    18083 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/datetime/date.py
--rw-r--r--   0 root         (0) root         (0)    67775 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/datetime/date_mixin.py
--rw-rw-r--   0 root         (0) root         (0)      897 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/src/everysk/core/datetime/date_settings.py
--rw-rw-r--   0 root         (0) root         (0)    32198 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/core/datetime/datetime.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.587170 everysk_beta-1.3.656/src/everysk/core/datetime/tests/
--rw-r--r--   0 root         (0) root         (0)     6194 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/datetime/tests/calendar.py
--rw-r--r--   0 root         (0) root         (0)    37520 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/datetime/tests/date.py
--rw-rw-r--   0 root         (0) root         (0)     1278 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/src/everysk/core/datetime/tests/date_mixin.py
--rw-r--r--   0 root         (0) root         (0)    45622 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/datetime/tests/datetime.py
--rw-r--r--   0 root         (0) root         (0)     2123 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    15920 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/fields.py
--rw-r--r--   0 root         (0) root         (0)    14211 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/firestore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.587170 everysk_beta-1.3.656/src/everysk/core/fixtures/
--rw-r--r--   0 root         (0) root         (0)      979 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/fixtures/_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.587170 everysk_beta-1.3.656/src/everysk/core/fixtures/other/
--rw-rw-r--   0 root         (0) root         (0)      822 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/core/fixtures/other/_settings.py
--rw-r--r--   0 root         (0) root         (0)     8606 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/http.py
--rw-r--r--   0 root         (0) root         (0)    11092 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/log.py
--rw-rw-r--   0 root         (0) root         (0)     1067 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/core/number.py
--rw-r--r--   0 root         (0) root         (0)    29002 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/object.py
--rw-r--r--   0 root         (0) root         (0)    12468 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/redis.py
--rw-rw-r--   0 root         (0) root         (0)     2200 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/core/slack.py
--rw-rw-r--   0 root         (0) root         (0)     3590 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/core/string.py
--rw-r--r--   0 root         (0) root         (0)     7393 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/tests.py
--rw-rw-r--   0 root         (0) root         (0)     7948 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/src/everysk/core/threads.py
--rw-r--r--   0 root         (0) root         (0)     2476 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/core/undefined.py
--rw-rw-r--   0 root         (0) root         (0)     8440 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/core/workers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.587170 everysk_beta-1.3.656/src/everysk/sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.587170 everysk_beta-1.3.656/src/everysk/sdk/_tests/
--rw-r--r--   0 root         (0) root         (0)     5811 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/sdk/_tests/base.py
--rw-r--r--   0 root         (0) root         (0)     4965 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/sdk/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.587170 everysk_beta-1.3.656/src/everysk/sdk/engines/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.587170 everysk_beta-1.3.656/src/everysk/sdk/engines/_tests/
--rw-rw-r--   0 root         (0) root         (0)     1839 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/src/everysk/sdk/engines/_tests/cryptography.py
--rw-rw-r--   0 root         (0) root         (0)     2134 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/src/everysk/sdk/engines/cryptography.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.587170 everysk_beta-1.3.656/src/everysk/sdk/entities/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.587170 everysk_beta-1.3.656/src/everysk/sdk/entities/_tests/
--rw-r--r--   0 root         (0) root         (0)    24085 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/_tests/base.py
--rw-rw-r--   0 root         (0) root         (0)     3443 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/_tests/base_list.py
--rw-rw-r--   0 root         (0) root         (0)    10853 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/_tests/fields.py
--rw-r--r--   0 root         (0) root         (0)    14073 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/_tests/query.py
--rw-r--r--   0 root         (0) root         (0)     2565 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/_tests/script.py
--rw-rw-r--   0 root         (0) root         (0)     8512 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/_tests/tags.py
--rw-rw-r--   0 root         (0) root         (0)    19813 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/base.py
--rw-rw-r--   0 root         (0) root         (0)     3693 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/base_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.587170 everysk_beta-1.3.656/src/everysk/sdk/entities/custom_index/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.591170 everysk_beta-1.3.656/src/everysk/sdk/entities/custom_index/_tests/
--rw-r--r--   0 root         (0) root         (0)     5529 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/custom_index/_tests/base.py
--rw-rw-r--   0 root         (0) root         (0)     6939 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/custom_index/base.py
--rw-rw-r--   0 root         (0) root         (0)     2015 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/custom_index/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.591170 everysk_beta-1.3.656/src/everysk/sdk/entities/datastore/
--rw-rw-r--   0 root         (0) root         (0)     6182 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/datastore/base.py
--rw-rw-r--   0 root         (0) root         (0)     1105 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/datastore/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.591170 everysk_beta-1.3.656/src/everysk/sdk/entities/datastore/tests/
--rw-r--r--   0 root         (0) root         (0)     6140 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/datastore/tests/base.py
--rw-rw-r--   0 root         (0) root         (0)    11318 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.591170 everysk_beta-1.3.656/src/everysk/sdk/entities/file/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.591170 everysk_beta-1.3.656/src/everysk/sdk/entities/file/_tests/
--rw-r--r--   0 root         (0) root         (0)     6263 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/file/_tests/base.py
--rw-rw-r--   0 root         (0) root         (0)     6940 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/file/base.py
--rw-rw-r--   0 root         (0) root         (0)     2101 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/file/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.591170 everysk_beta-1.3.656/src/everysk/sdk/entities/portfolio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.591170 everysk_beta-1.3.656/src/everysk/sdk/entities/portfolio/_tests/
--rw-r--r--   0 root         (0) root         (0)    12396 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/portfolio/_tests/base.py
--rw-rw-r--   0 root         (0) root         (0)     5459 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/portfolio/_tests/securities.py
--rw-rw-r--   0 root         (0) root         (0)     9393 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/portfolio/_tests/security.py
--rw-rw-r--   0 root         (0) root         (0)     8423 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/portfolio/base.py
--rw-rw-r--   0 root         (0) root         (0)    10366 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/portfolio/securities.py
--rw-rw-r--   0 root         (0) root         (0)    21835 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/portfolio/security.py
--rw-rw-r--   0 root         (0) root         (0)     3377 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/portfolio/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.591170 everysk_beta-1.3.656/src/everysk/sdk/entities/private_security/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.591170 everysk_beta-1.3.656/src/everysk/sdk/entities/private_security/_tests/
--rw-r--r--   0 root         (0) root         (0)     6811 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/private_security/_tests/base.py
--rw-rw-r--   0 root         (0) root         (0)     7353 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/private_security/base.py
--rw-rw-r--   0 root         (0) root         (0)     1421 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/private_security/settings.py
--rw-r--r--   0 root         (0) root         (0)    20288 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.591170 everysk_beta-1.3.656/src/everysk/sdk/entities/report/
--rw-rw-r--   0 root         (0) root         (0)     7421 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/report/base.py
--rw-rw-r--   0 root         (0) root         (0)     1383 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/report/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.591170 everysk_beta-1.3.656/src/everysk/sdk/entities/report/tests/
--rw-r--r--   0 root         (0) root         (0)     5998 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/report/tests/base.py
--rw-r--r--   0 root         (0) root         (0)     4194 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/script.py
--rw-rw-r--   0 root         (0) root         (0)     2070 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/settings.py
--rw-rw-r--   0 root         (0) root         (0)     6312 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/src/everysk/sdk/entities/tags.py
--rw-r--r--   0 root         (0) root         (0)      957 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/sdk/settings.py
--rw-rw-r--   0 root         (0) root         (0)     2843 2024-03-28 14:19:49.000000 everysk_beta-1.3.656/src/everysk/sdk/tests.py
--rw-r--r--   0 root         (0) root         (0)     1022 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/settings.py
--rw-r--r--   0 root         (0) root         (0)      478 2024-04-08 13:02:58.000000 everysk_beta-1.3.656/src/everysk/tests.py
--rw-rw-r--   0 root         (0) root         (0)     1839 2024-02-15 17:58:48.000000 everysk_beta-1.3.656/src/everysk/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:05:36.591170 everysk_beta-1.3.656/src/everysk_beta.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7819 2024-04-25 17:05:36.000000 everysk_beta-1.3.656/src/everysk_beta.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3697 2024-04-25 17:05:36.000000 everysk_beta-1.3.656/src/everysk_beta.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 17:05:36.000000 everysk_beta-1.3.656/src/everysk_beta.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1404 2024-04-25 17:05:36.000000 everysk_beta-1.3.656/src/everysk_beta.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-25 17:05:36.000000 everysk_beta-1.3.656/src/everysk_beta.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.952679 everysk_beta-1.4.815/
+-rw-rw-r--   0 root         (0) root         (0)      312 2024-02-15 17:58:48.000000 everysk_beta-1.4.815/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     7819 2024-04-25 19:05:53.952679 everysk_beta-1.4.815/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3431 2024-02-15 17:58:48.000000 everysk_beta-1.4.815/README.md
+-rw-r--r--   0 root         (0) root         (0)     2648 2024-04-25 19:05:50.000000 everysk_beta-1.4.815/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 19:05:53.952679 everysk_beta-1.4.815/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.940679 everysk_beta-1.4.815/src/
+-rw-rw-r--   0 root         (0) root         (0)      653 2024-02-15 17:58:48.000000 everysk_beta-1.4.815/src/__builtins__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.940679 everysk_beta-1.4.815/src/everysk/
+-rw-rw-r--   0 root         (0) root         (0)      927 2024-03-28 14:19:49.000000 everysk_beta-1.4.815/src/everysk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.940679 everysk_beta-1.4.815/src/everysk/api/
+-rw-r--r--   0 root         (0) root         (0)     2240 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.944679 everysk_beta-1.4.815/src/everysk/api/_tests/
+-rw-r--r--   0 root         (0) root         (0)     6260 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/_tests/api_requestor.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/_tests/http_client.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/_tests/init.py
+-rw-r--r--   0 root         (0) root         (0)     9160 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/_tests/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6071 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_requestor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.944679 everysk_beta-1.4.815/src/everysk/api/api_resources/
+-rw-r--r--   0 root         (0) root         (0)     1267 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.944679 everysk_beta-1.4.815/src/everysk/api/api_resources/_tests/
+-rw-r--r--   0 root         (0) root         (0)    13161 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/_tests/api_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7530 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/_tests/calculation.py
+-rw-r--r--   0 root         (0) root         (0)     1007 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/_tests/custom_index.py
+-rw-r--r--   0 root         (0) root         (0)     1927 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/_tests/datastore.py
+-rw-r--r--   0 root         (0) root         (0)      976 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/_tests/file.py
+-rw-r--r--   0 root         (0) root         (0)     4114 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/_tests/market_data.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/_tests/parser.py
+-rw-r--r--   0 root         (0) root         (0)      996 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/_tests/portfolio.py
+-rw-r--r--   0 root         (0) root         (0)     1045 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/_tests/private_security.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/_tests/report.py
+-rw-r--r--   0 root         (0) root         (0)     1055 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/_tests/report_template.py
+-rw-r--r--   0 root         (0) root         (0)     1746 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/_tests/worker_execution.py
+-rw-r--r--   0 root         (0) root         (0)     1776 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/_tests/workflow.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/_tests/workflow_execution.py
+-rw-r--r--   0 root         (0) root         (0)     1006 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/_tests/workspace.py
+-rw-r--r--   0 root         (0) root         (0)    14326 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/api_resource.py
+-rw-r--r--   0 root         (0) root         (0)    33844 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/calculation.py
+-rw-r--r--   0 root         (0) root         (0)     1382 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/custom_index.py
+-rw-r--r--   0 root         (0) root         (0)     3248 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/datastore.py
+-rw-r--r--   0 root         (0) root         (0)     1386 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/file.py
+-rw-r--r--   0 root         (0) root         (0)     9324 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/market_data.py
+-rw-r--r--   0 root         (0) root         (0)     2749 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1501 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/portfolio.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/private_security.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/report.py
+-rw-r--r--   0 root         (0) root         (0)     1307 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/report_template.py
+-rw-r--r--   0 root         (0) root         (0)     5749 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/tests.py
+-rw-r--r--   0 root         (0) root         (0)     2790 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/worker_execution.py
+-rw-r--r--   0 root         (0) root         (0)     2378 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/workflow.py
+-rw-r--r--   0 root         (0) root         (0)     4257 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/workflow_execution.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/api_resources/workspace.py
+-rw-r--r--   0 root         (0) root         (0)     2156 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/http_client.py
+-rw-r--r--   0 root         (0) root         (0)     1248 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/tests.py
+-rw-r--r--   0 root         (0) root         (0)     8431 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/api/utils.py
+-rw-r--r--   0 root         (0) root         (0)    14406 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/config.py
+-rw-r--r--   0 root         (0) root         (0)     3105 2024-04-25 17:25:07.000000 everysk_beta-1.4.815/src/everysk/config.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.944679 everysk_beta-1.4.815/src/everysk/core/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.944679 everysk_beta-1.4.815/src/everysk/core/_tests/
+-rw-r--r--   0 root         (0) root         (0)     2962 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/_tests/compress.py
+-rw-r--r--   0 root         (0) root         (0)    13215 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/_tests/config.py
+-rw-r--r--   0 root         (0) root         (0)     4273 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/_tests/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    23565 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/_tests/fields.py
+-rw-r--r--   0 root         (0) root         (0)    26984 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/_tests/firestore.py
+-rw-r--r--   0 root         (0) root         (0)    12904 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/_tests/http.py
+-rw-r--r--   0 root         (0) root         (0)    13110 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/_tests/log.py
+-rw-rw-r--   0 root         (0) root         (0)      795 2024-02-15 17:58:48.000000 everysk_beta-1.4.815/src/everysk/core/_tests/number.py
+-rw-r--r--   0 root         (0) root         (0)    47464 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/_tests/object.py
+-rw-r--r--   0 root         (0) root         (0)    13765 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/_tests/redis.py
+-rw-r--r--   0 root         (0) root         (0)     5662 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/_tests/serialize.py
+-rw-rw-r--   0 root         (0) root         (0)     3631 2024-02-15 17:58:48.000000 everysk_beta-1.4.815/src/everysk/core/_tests/slack.py
+-rw-rw-r--   0 root         (0) root         (0)     3415 2024-02-15 17:58:48.000000 everysk_beta-1.4.815/src/everysk/core/_tests/string.py
+-rw-r--r--   0 root         (0) root         (0)     5285 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/_tests/threads.py
+-rw-r--r--   0 root         (0) root         (0)     2432 2024-04-08 13:02:58.000000 everysk_beta-1.4.815/src/everysk/core/_tests/undefined.py
+-rw-rw-r--   0 root         (0) root         (0)     1800 2024-02-15 17:58:48.000000 everysk_beta-1.4.815/src/everysk/core/_tests/utils.py
+-rw-rw-r--   0 root         (0) root         (0)    12441 2024-02-15 17:58:48.000000 everysk_beta-1.4.815/src/everysk/core/_tests/workers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.944679 everysk_beta-1.4.815/src/everysk/core/cloud_function/
+-rw-rw-r--   0 root         (0) root         (0)     2571 2024-02-15 17:58:48.000000 everysk_beta-1.4.815/src/everysk/core/cloud_function/main.py
+-rw-rw-r--   0 root         (0) root         (0)     3731 2024-02-15 17:58:48.000000 everysk_beta-1.4.815/src/everysk/core/cloud_function/tests.py
+-rw-r--r--   0 root         (0) root         (0)     3667 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/compress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.944679 everysk_beta-1.4.815/src/everysk/core/datetime/
+-rw-rw-r--   0 root         (0) root         (0)      584 2024-02-15 17:58:48.000000 everysk_beta-1.4.815/src/everysk/core/datetime/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3465 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/datetime/calendar.py
+-rw-r--r--   0 root         (0) root         (0)    18083 2024-04-08 13:02:58.000000 everysk_beta-1.4.815/src/everysk/core/datetime/date.py
+-rw-r--r--   0 root         (0) root         (0)    68313 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/datetime/date_mixin.py
+-rw-rw-r--   0 root         (0) root         (0)      897 2024-02-15 17:58:48.000000 everysk_beta-1.4.815/src/everysk/core/datetime/date_settings.py
+-rw-r--r--   0 root         (0) root         (0)    32446 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/datetime/datetime.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.944679 everysk_beta-1.4.815/src/everysk/core/datetime/tests/
+-rw-r--r--   0 root         (0) root         (0)     6194 2024-04-08 13:02:58.000000 everysk_beta-1.4.815/src/everysk/core/datetime/tests/calendar.py
+-rw-r--r--   0 root         (0) root         (0)    37520 2024-04-08 13:02:58.000000 everysk_beta-1.4.815/src/everysk/core/datetime/tests/date.py
+-rw-rw-r--   0 root         (0) root         (0)     1278 2024-02-15 17:58:48.000000 everysk_beta-1.4.815/src/everysk/core/datetime/tests/date_mixin.py
+-rw-r--r--   0 root         (0) root         (0)    45622 2024-04-08 13:02:58.000000 everysk_beta-1.4.815/src/everysk/core/datetime/tests/datetime.py
+-rw-r--r--   0 root         (0) root         (0)     3641 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    36597 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/fields.py
+-rw-r--r--   0 root         (0) root         (0)    19553 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/firestore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.944679 everysk_beta-1.4.815/src/everysk/core/fixtures/
+-rw-r--r--   0 root         (0) root         (0)     1204 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/fixtures/_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.944679 everysk_beta-1.4.815/src/everysk/core/fixtures/other/
+-rw-rw-r--   0 root         (0) root         (0)      822 2024-03-28 14:19:49.000000 everysk_beta-1.4.815/src/everysk/core/fixtures/other/_settings.py
+-rw-r--r--   0 root         (0) root         (0)    10149 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/http.py
+-rw-r--r--   0 root         (0) root         (0)    11998 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/log.py
+-rw-rw-r--   0 root         (0) root         (0)     1067 2024-03-28 14:19:49.000000 everysk_beta-1.4.815/src/everysk/core/number.py
+-rw-r--r--   0 root         (0) root         (0)    32797 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/object.py
+-rw-r--r--   0 root         (0) root         (0)    12963 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/redis.py
+-rw-r--r--   0 root         (0) root         (0)     6575 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     1035 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/settings.py
+-rw-r--r--   0 root         (0) root         (0)     2199 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/slack.py
+-rw-r--r--   0 root         (0) root         (0)     5432 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/string.py
+-rw-r--r--   0 root         (0) root         (0)     7965 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/tests.py
+-rw-r--r--   0 root         (0) root         (0)     6749 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/threads.py
+-rw-r--r--   0 root         (0) root         (0)     2476 2024-04-08 13:02:58.000000 everysk_beta-1.4.815/src/everysk/core/undefined.py
+-rw-r--r--   0 root         (0) root         (0)     8414 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/core/workers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.948679 everysk_beta-1.4.815/src/everysk/sdk/
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.948679 everysk_beta-1.4.815/src/everysk/sdk/_tests/
+-rw-r--r--   0 root         (0) root         (0)     9755 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/_tests/base.py
+-rw-r--r--   0 root         (0) root         (0)     3490 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/_tests/init.py
+-rw-r--r--   0 root         (0) root         (0)     6322 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.948679 everysk_beta-1.4.815/src/everysk/sdk/engines/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.948679 everysk_beta-1.4.815/src/everysk/sdk/engines/_tests/
+-rw-rw-r--   0 root         (0) root         (0)     1839 2024-02-15 17:58:48.000000 everysk_beta-1.4.815/src/everysk/sdk/engines/_tests/cryptography.py
+-rw-r--r--   0 root         (0) root         (0)     2775 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/engines/cryptography.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.948679 everysk_beta-1.4.815/src/everysk/sdk/entities/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.948679 everysk_beta-1.4.815/src/everysk/sdk/entities/_tests/
+-rw-r--r--   0 root         (0) root         (0)    24306 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/_tests/base.py
+-rw-rw-r--   0 root         (0) root         (0)     3443 2024-02-15 17:58:48.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/_tests/base_list.py
+-rw-rw-r--   0 root         (0) root         (0)    10853 2024-03-28 14:19:49.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/_tests/fields.py
+-rw-r--r--   0 root         (0) root         (0)    17108 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/_tests/query.py
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/_tests/script.py
+-rw-rw-r--   0 root         (0) root         (0)     8512 2024-02-15 17:58:48.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/_tests/tags.py
+-rw-r--r--   0 root         (0) root         (0)    19910 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/base.py
+-rw-rw-r--   0 root         (0) root         (0)     3693 2024-02-15 17:58:48.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/base_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.948679 everysk_beta-1.4.815/src/everysk/sdk/entities/custom_index/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.948679 everysk_beta-1.4.815/src/everysk/sdk/entities/custom_index/_tests/
+-rw-r--r--   0 root         (0) root         (0)     5584 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/custom_index/_tests/base.py
+-rw-r--r--   0 root         (0) root         (0)     7001 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/custom_index/base.py
+-rw-rw-r--   0 root         (0) root         (0)     2015 2024-03-28 14:19:49.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/custom_index/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.948679 everysk_beta-1.4.815/src/everysk/sdk/entities/datastore/
+-rw-r--r--   0 root         (0) root         (0)     6284 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/datastore/base.py
+-rw-rw-r--   0 root         (0) root         (0)     1105 2024-03-28 14:19:49.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/datastore/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.948679 everysk_beta-1.4.815/src/everysk/sdk/entities/datastore/tests/
+-rw-r--r--   0 root         (0) root         (0)     6295 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/datastore/tests/base.py
+-rw-r--r--   0 root         (0) root         (0)    12719 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.948679 everysk_beta-1.4.815/src/everysk/sdk/entities/file/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.948679 everysk_beta-1.4.815/src/everysk/sdk/entities/file/_tests/
+-rw-r--r--   0 root         (0) root         (0)     6326 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/file/_tests/base.py
+-rw-r--r--   0 root         (0) root         (0)     6945 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/file/base.py
+-rw-r--r--   0 root         (0) root         (0)     2246 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/file/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.948679 everysk_beta-1.4.815/src/everysk/sdk/entities/portfolio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.948679 everysk_beta-1.4.815/src/everysk/sdk/entities/portfolio/_tests/
+-rw-r--r--   0 root         (0) root         (0)    12574 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/portfolio/_tests/base.py
+-rw-rw-r--   0 root         (0) root         (0)     5459 2024-02-15 17:58:48.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/portfolio/_tests/securities.py
+-rw-rw-r--   0 root         (0) root         (0)     9393 2024-02-15 17:58:48.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/portfolio/_tests/security.py
+-rw-r--r--   0 root         (0) root         (0)     9335 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/portfolio/base.py
+-rw-rw-r--   0 root         (0) root         (0)    10366 2024-03-28 14:19:49.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/portfolio/securities.py
+-rw-r--r--   0 root         (0) root         (0)    21834 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/portfolio/security.py
+-rw-r--r--   0 root         (0) root         (0)     3622 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/portfolio/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.948679 everysk_beta-1.4.815/src/everysk/sdk/entities/private_security/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.948679 everysk_beta-1.4.815/src/everysk/sdk/entities/private_security/_tests/
+-rw-r--r--   0 root         (0) root         (0)     6874 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/private_security/_tests/base.py
+-rw-rw-r--   0 root         (0) root         (0)     7353 2024-03-28 14:19:49.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/private_security/base.py
+-rw-rw-r--   0 root         (0) root         (0)     1421 2024-03-28 14:19:49.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/private_security/settings.py
+-rw-r--r--   0 root         (0) root         (0)    22855 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.948679 everysk_beta-1.4.815/src/everysk/sdk/entities/report/
+-rw-r--r--   0 root         (0) root         (0)     7600 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/report/base.py
+-rw-rw-r--   0 root         (0) root         (0)     1383 2024-03-28 14:19:49.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/report/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.948679 everysk_beta-1.4.815/src/everysk/sdk/entities/report/tests/
+-rw-r--r--   0 root         (0) root         (0)     6150 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/report/tests/base.py
+-rw-r--r--   0 root         (0) root         (0)     4168 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/script.py
+-rw-rw-r--   0 root         (0) root         (0)     2070 2024-03-28 14:19:49.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/settings.py
+-rw-rw-r--   0 root         (0) root         (0)     6312 2024-02-15 17:58:48.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.948679 everysk_beta-1.4.815/src/everysk/sdk/entities/worker_template/
+-rw-r--r--   0 root         (0) root         (0)     3344 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/worker_template/base.py
+-rw-r--r--   0 root         (0) root         (0)     3447 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/worker_template/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.948679 everysk_beta-1.4.815/src/everysk/sdk/entities/worker_template/tests/
+-rw-r--r--   0 root         (0) root         (0)     3028 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/entities/worker_template/tests/base.py
+-rw-r--r--   0 root         (0) root         (0)     2496 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/settings.py
+-rw-r--r--   0 root         (0) root         (0)     3047 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/sdk/tests.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/settings.py
+-rw-r--r--   0 root         (0) root         (0)      614 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/tests.py
+-rw-r--r--   0 root         (0) root         (0)     2382 2024-04-25 19:04:03.000000 everysk_beta-1.4.815/src/everysk/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:05:53.948679 everysk_beta-1.4.815/src/everysk_beta.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7819 2024-04-25 19:05:53.000000 everysk_beta-1.4.815/src/everysk_beta.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5786 2024-04-25 19:05:53.000000 everysk_beta-1.4.815/src/everysk_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 19:05:53.000000 everysk_beta-1.4.815/src/everysk_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1404 2024-04-25 19:05:53.000000 everysk_beta-1.4.815/src/everysk_beta.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-25 19:05:53.000000 everysk_beta-1.4.815/src/everysk_beta.egg-info/top_level.txt
```

### Comparing `everysk_beta-1.3.656/PKG-INFO` & `everysk_beta-1.4.815/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: everysk-beta
-Version: 1.3.656
+Version: 1.4.815
 Summary: Generic lib to share python code on Everysk.
 License: (C) Copyright 2023 EVERYSK TECHNOLOGIES
         
         This is an unpublished work containing confidential and proprietary
         information of EVERYSK TECHNOLOGIES. Disclosure, use, or reproduction
         without authorization of EVERYSK TECHNOLOGIES is prohibited.
```

### Comparing `everysk_beta-1.3.656/README.md` & `everysk_beta-1.4.815/README.md`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/pyproject.toml` & `everysk_beta-1.4.815/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 name = "everysk-beta"
 description = "Generic lib to share python code on Everysk."
 requires-python = ">=3.11"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 # Do not remove/change version here, change on run.sh build section
-version = "1.3.656"
+version = "1.4.815"
 
 keywords = [
     "python",
     "setuptools",
     "development",
     "lib"
 ]
```

### Comparing `everysk_beta-1.3.656/src/__builtins__.py` & `everysk_beta-1.4.815/src/__builtins__.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/__init__.py` & `everysk_beta-1.4.815/src/everysk/__init__.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/config.pyi` & `everysk_beta-1.4.815/src/everysk/config.pyi`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/core/_tests/compress.py` & `everysk_beta-1.4.815/src/everysk/core/_tests/compress.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,26 +22,39 @@
         string = b'x\x9cSJLT\xc0\x86\x94\x00]\xbd\x075'
         self.assertEqual(decompress_json(string), 'aa aa aa aa aa aa aa aa')
 
     def test_undefined(self):
         obj_compressed = compress_json(Undefined)
         self.assertEqual(decompress_json(obj_compressed), Undefined)
 
-    def test_complex_obj(self):
+    def test_complex_obj_with_convert_true(self):
         obj = [
             {'datetime': DateTime.now()},
             {'a': 1, 'b': True},
             'Test',
             1.1,
             ['1', '2', '3', Date.today()],
             Undefined,
             {'undefined': Undefined}
         ]
         obj_compressed = compress_json(obj)
-        self.assertListEqual(decompress_json(obj_compressed), obj)
+        self.assertListEqual(decompress_json(obj_compressed, convert_str_to_date=True), obj)
+
+    def test_complex_obj_with_convert_false(self):
+        obj = [
+            {'datetime': DateTime.now().isoformat()},
+            {'a': 1, 'b': True},
+            'Test',
+            1.1,
+            ['1', '2', '3', Date.today().isoformat()],
+            Undefined,
+            {'undefined': Undefined}
+        ]
+        obj_compressed = compress_json(obj)
+        self.assertListEqual(decompress_json(obj_compressed, convert_str_to_date=False), obj)
 
 
 class CompressPickleTestCase(TestCase):
 
     def setUp(self) -> None:
         self.str_repr = b'x\x9ck`\x99*\xcd\x00\x01=\xe2\x89\x89\n\xd8\xd0\x14=\x00\x9f\xef\t\x8a'
```

### Comparing `everysk_beta-1.3.656/src/everysk/core/_tests/fields.py` & `everysk_beta-1.4.815/src/everysk/core/_tests/fields.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # This is an unpublished work containing confidential and proprietary
 # information of EVERYSK TECHNOLOGIES. Disclosure, use, or reproduction
 # without authorization of EVERYSK TECHNOLOGIES is prohibited.
 #
 ###############################################################################
 import re
 from collections.abc import Iterator
+from sys import maxsize as max_int
 from unittest import TestCase
 from zoneinfo import ZoneInfo
 
 from everysk.core import fields
 from everysk.core.datetime.date import date, Date
 from everysk.core.datetime.datetime import datetime, DateTime
 from everysk.core.exceptions import ReadonlyError, RequiredError, FieldValueError
@@ -21,14 +22,18 @@
 
 class FieldTestCase(TestCase):
 
     def test_attr_type(self):
         field = fields.Field()
         self.assertIsNone(field.attr_type)
 
+    def test_vscode_autocomplete(self):
+        for cls in fields.Field.__subclasses__():
+            self.assertEqual(cls.__new__.__annotations__['return'], cls.attr_type)
+
 
 class BoolFieldTestCase(TestCase):
 
     def test_attr_type(self):
         field = fields.BoolField()
         self.assertEqual(field.attr_type, bool)
 
@@ -99,15 +104,15 @@
             field.clean_value('20220912'),
             Date(year=2022, month=9, day=12)
         )
 
     def test_validate(self):
         field = fields.DateField()
         field.validate(attr_name='test', value=Date.fromisoformat('2023-01-01'))
-        field.validate(attr_name='test', value=date.fromisoformat('2023-01-01'))
+        field.validate(attr_name='test', value=date.fromisoformat('2023-01-01'))# pylint: disable=no-member
 
 
 class DateTimeFieldTestCase(TestCase):
 
     def test_attr_type(self):
         field = fields.DateTimeField()
         self.assertEqual(field.attr_type, DateTime)
@@ -148,23 +153,73 @@
             field.clean_value(Date(2022, 9, 12)),
             DateTime(year=2022, month=9, day=12, tzinfo=ZoneInfo('UTC'))
         )
 
     def test_validate(self):
         field = fields.DateTimeField()
         field.validate(attr_name='test', value=DateTime.fromisoformat('2022-09-12T13:00:00+00:00'))
-        field.validate(attr_name='test', value=datetime.fromisoformat('2022-09-12T13:00:00+00:00'))
+        field.validate(attr_name='test', value=datetime.fromisoformat('2022-09-12T13:00:00+00:00')) # pylint: disable=no-member
 
 
 class DictFieldTestCase(TestCase):
 
     def test_attr_type(self):
         field = fields.DictField()
         self.assertEqual(field.attr_type, dict)
 
+    def test_readonly(self):
+        field = fields.DictField(default={'a': 1}, readonly=True)
+        self.assertRaises(ReadonlyError, field.default.__setitem__, 'a', 2)
+        self.assertRaises(ReadonlyError, field.default.__delitem__, 'a')
+        self.assertRaises(ReadonlyError, field.default.pop)
+        self.assertRaises(ReadonlyError, field.default.popitem, 'a')
+        self.assertRaises(ReadonlyError, field.default.clear)
+        self.assertRaises(ReadonlyError, field.default.update, {'a': 2})
+        self.assertRaises(ReadonlyError, field.default.setdefault, 'b', 2)
+        self.assertDictEqual(field.default, {'a': 1})
+
+    def test_int_keys(self):
+        class DictObjectIntKey(BaseObject):
+            field = fields.DictField(default={1: 0})
+
+        obj = DictObjectIntKey()
+        self.assertEqual(obj.field[1], 0)
+        obj.field = {1: 1}
+        self.assertEqual(obj.field[1], 1)
+        obj.field[1] = 2
+        self.assertEqual(obj.field[1], 2)
+
+    def test_int_keys_readonly(self):
+        class DictObjectIntKey(BaseObject):
+            field = fields.DictField(default={1: 0}, readonly=True)
+
+        obj = DictObjectIntKey()
+        self.assertEqual(obj.field[1], 0)
+
+
+class EmailFieldTestCase(TestCase):
+
+    def test_attr_type(self):
+        field = fields.EmailField()
+        self.assertEqual(field.attr_type, str)
+
+    def test_valid_email(self):
+        field = fields.EmailField()
+        field.validate(attr_name='test', value='fscariott@everysk.com', attr_type=field.attr_type)
+
+    def test_invalid_email(self):
+        field = fields.EmailField()
+        with self.assertRaisesRegex(FieldValueError, 'Key test must be an e-mail.'):
+            field.validate(attr_name='test', value='fscariott.everysk.com', attr_type=field.attr_type)
+
+    def test_invalid_email_with_more_at(self):
+        field = fields.EmailField()
+        with self.assertRaisesRegex(FieldValueError, 'Key test must be an e-mail.'):
+            field.validate(attr_name='test', value='fscariott@everysk@com', attr_type=field.attr_type)
+
 
 class FloatFieldTestCase(TestCase):
 
     def test_attr_type(self):
         field = fields.FloatField()
         self.assertEqual(field.attr_type, float)
 
@@ -257,14 +312,19 @@
     def test_clean_value(self):
         field = fields.ListField()
         self.assertEqual(field.clean_value('aaa'), ['aaa'])
         self.assertEqual(field.clean_value([0, 1]), [0, 1])
         self.assertEqual(field.clean_value(1), 1)
         self.assertEqual(field.clean_value({'a': 1}), {'a': 1})
 
+    def test_max_size_default(self):
+        # https://stackoverflow.com/questions/855191/how-big-can-a-python-list-get#comment112727918_15739630
+        field = fields.ListField()
+        self.assertEqual(field.max_size, max_int / 8)
+
     def test_max_size(self):
         field = fields.ListField(min_size=1, max_size=2)
         self.assertRaisesRegex(
             FieldValueError,
             "The attribute 'banana' is not within the specified list range. min_size: 1 max_size: 2",
             field.validate,
             attr_name='banana',
@@ -296,14 +356,97 @@
             FieldValueError,
             "The 'banana' value must be a list.",
             field.validate,
             attr_name='banana',
             value=1234
         )
 
+    def test_readonly(self):
+        field = fields.ListField(default=[9, 1, 2, 3], readonly=True)
+        self.assertRaises(ReadonlyError, field.default.__setitem__, 0, 1)
+        self.assertRaises(ReadonlyError, field.default.__delitem__, 0)
+        self.assertRaises(ReadonlyError, field.default.append, 4)
+        self.assertRaises(ReadonlyError, field.default.clear)
+        self.assertRaises(ReadonlyError, field.default.extend, [5, 6])
+        self.assertRaises(ReadonlyError, field.default.insert, 0, 7)
+        self.assertRaises(ReadonlyError, field.default.pop)
+        self.assertRaises(ReadonlyError, field.default.remove, 0)
+        self.assertRaises(ReadonlyError, field.default.reverse)
+        self.assertRaises(ReadonlyError, field.default.sort)
+        self.assertListEqual(field.default, [9, 1, 2, 3])
+
+
+class SetFieldTestCase(TestCase):
+
+    def test_attr_type(self):
+        field = fields.SetField()
+        self.assertEqual(field.attr_type, set)
+
+    def test_clean_value(self):
+        field = fields.SetField()
+        self.assertEqual(field.clean_value({0, 1}), {0, 1})
+        self.assertEqual(field.clean_value(1), 1)
+        self.assertEqual(field.clean_value({'a': 1}), {'a': 1})
+
+    def test_max_size_default(self):
+        # https://stackoverflow.com/questions/855191/how-big-can-a-python-list-get#comment112727918_15739630
+        field = fields.SetField()
+        self.assertEqual(field.max_size, max_int / 8)
+
+    def test_max_size(self):
+        field = fields.SetField(min_size=1, max_size=2)
+        self.assertRaisesRegex(
+            FieldValueError,
+            "The attribute 'banana' is not within the specified set range. min_size: 1 max_size: 2",
+            field.validate,
+            attr_name='banana',
+            value={1, 2, 3}
+        )
+
+    def test_min_size(self):
+        field = fields.SetField(min_size=2, max_size=3)
+        self.assertRaisesRegex(
+            FieldValueError,
+            "The attribute 'banana' is not within the specified set range. min_size: 2 max_size: 3",
+            field.validate,
+            attr_name='banana',
+            value={1}
+        )
+
+    def test_min_size_negative(self):
+        self.assertRaisesRegex(
+            FieldValueError,
+            'Set min_size cloud not be a negative number.',
+            fields.SetField,
+            min_size=-1,
+            max_size=3
+        )
+
+    def test_validate(self):
+        field = fields.SetField()
+        self.assertRaisesRegex(
+            FieldValueError,
+            "Key banana must be <class 'set'>.",
+            field.validate,
+            attr_name='banana',
+            value=1234
+        )
+
+    def test_readonly(self):
+        field = fields.SetField(default={9, 1, 2, 3}, readonly=True)
+        self.assertRaises(ReadonlyError, field.default.__setitem__, 0, 1)
+        self.assertRaises(ReadonlyError, field.default.__delitem__, 0)
+        self.assertRaises(ReadonlyError, field.default.add, 4)
+        self.assertRaises(ReadonlyError, field.default.clear)
+        self.assertRaises(ReadonlyError, field.default.discard, 1)
+        self.assertRaises(ReadonlyError, field.default.pop)
+        self.assertRaises(ReadonlyError, field.default.remove, 1)
+        self.assertRaises(ReadonlyError, field.default.update, {1, 4})
+        self.assertSetEqual(field.default, {9, 1, 2, 3})
+
 
 class StrFieldTestCase(TestCase):
 
     def test_attr_type(self):
         field = fields.StrField()
         self.assertEqual(field.attr_type, str)
 
@@ -355,53 +498,14 @@
 class TupleFieldTestCase(TestCase):
 
     def test_attr_type(self):
         field = fields.TupleField()
         self.assertEqual(field.attr_type, tuple)
 
 
-class ReadonlyDictFieldTestCase(TestCase):
-
-    def test_attr_type(self):
-        field = fields.ReadonlyDictField({'a': 1})
-        self.assertEqual(field.attr_type, dict)
-
-    def test_readonly(self):
-        field = fields.ReadonlyDictField({'a': 1})
-        self.assertRaises(ReadonlyError, field.default.__setitem__, 'a', 2)
-        self.assertRaises(ReadonlyError, field.default.__delitem__, 'a')
-        self.assertRaises(ReadonlyError, field.default.pop)
-        self.assertRaises(ReadonlyError, field.default.popitem, 'a')
-        self.assertRaises(ReadonlyError, field.default.clear)
-        self.assertRaises(ReadonlyError, field.default.update, {'a': 2})
-        self.assertRaises(ReadonlyError, field.default.setdefault, 'b', 2)
-        self.assertDictEqual(field.default, {'a': 1})
-
-
-class ReadonlyListFieldTestCase(TestCase):
-
-    def test_attr_type(self):
-        field = fields.ReadonlyListField({'a': 1})
-        self.assertEqual(field.attr_type, list)
-
-    def test_readonly(self):
-        field = fields.ReadonlyListField([9, 1, 2, 3])
-        self.assertRaises(ReadonlyError, field.default.__setitem__, 0, 1)
-        self.assertRaises(ReadonlyError, field.default.__delitem__, 0)
-        self.assertRaises(ReadonlyError, field.default.append, 4)
-        self.assertRaises(ReadonlyError, field.default.clear)
-        self.assertRaises(ReadonlyError, field.default.extend, [5, 6])
-        self.assertRaises(ReadonlyError, field.default.insert, 0, 7)
-        self.assertRaises(ReadonlyError, field.default.pop)
-        self.assertRaises(ReadonlyError, field.default.remove, 0)
-        self.assertRaises(ReadonlyError, field.default.reverse)
-        self.assertRaises(ReadonlyError, field.default.sort)
-        self.assertListEqual(field.default, [9, 1, 2, 3])
-
-
 class FieldUndefinedClass(BaseObject):
     f01 = fields.BoolField(default=Undefined)
     f02 = fields.ChoiceField(default=Undefined, choices=[Undefined, None])
     f03 = fields.DateField(default=Undefined)
     f04 = fields.DateTimeField(default=Undefined)
     f05 = fields.FloatField(default=Undefined)
     f06 = fields.IntField(default=Undefined)
@@ -530,7 +634,67 @@
         obj = COD3770()
         self.assertEqual(obj.var, self.date)
 
     def test_instance_var_attribution(self):
         obj = COD3770()
         obj.var = '2024-01-02'
         self.assertEqual(obj.var, Date(2024, 1, 2))
+
+
+class URLFieldTestCase(TestCase):
+
+    class ObjectClass(BaseObject):
+        url = fields.URLField()
+
+    class DictClass(BaseDict):
+        url = fields.URLField()
+
+    def test_http_url(self):
+        url = 'http://exampe.com/path?var=1&var=2'
+        obj = self.ObjectClass()
+        dct = self.DictClass()
+        obj.url = url
+        dct['url'] = url
+        self.assertEqual(obj.url, dct['url'])
+
+    def test_https_url(self):
+        url = 'https://exampe.com/path?var=1&var=2'
+        obj = self.ObjectClass()
+        dct = self.DictClass()
+        obj.url = url
+        dct['url'] = url
+        self.assertEqual(obj.url, dct['url'])
+
+    def test_localhost_url(self):
+        url = 'http://localhost:8080/path?var=1&var=2'
+        obj = self.ObjectClass()
+        dct = self.DictClass()
+        obj.url = url
+        dct['url'] = url
+        self.assertEqual(obj.url, dct['url'])
+
+    def test_not_valid_scheme(self):
+        url = 'ttp://localhost:8080/path?var=1&var=2'
+        obj = self.ObjectClass()
+        dct = self.DictClass()
+        with self.assertRaisesRegex(FieldValueError, 'Key url must be an URL.'):
+            obj.url = url
+        with self.assertRaisesRegex(FieldValueError, 'Key url must be an URL.'):
+            dct['url'] = url
+
+    def test_not_valid_domain(self):
+        url = 'http://localhost.host:/path?var=1&var=2'
+        obj = self.ObjectClass()
+        dct = self.DictClass()
+        with self.assertRaisesRegex(FieldValueError, 'Key url must be an URL.'):
+            obj.url = url
+        with self.assertRaisesRegex(FieldValueError, 'Key url must be an URL.'):
+            dct['url'] = url
+
+    def test_not_valid_query(self):
+        url = 'http://localhost:8080/path?var=1 var=2'
+        obj = self.ObjectClass()
+        dct = self.DictClass()
+        with self.assertRaisesRegex(FieldValueError, 'Key url must be an URL.'):
+            obj.url = url
+        with self.assertRaisesRegex(FieldValueError, 'Key url must be an URL.'):
+            dct['url'] = url
```

### Comparing `everysk_beta-1.3.656/src/everysk/core/_tests/firestore.py` & `everysk_beta-1.4.815/src/everysk/core/_tests/firestore.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,22 +5,21 @@
 # This is an unpublished work containing confidential and proprietary
 # information of EVERYSK TECHNOLOGIES. Disclosure, use, or reproduction
 # without authorization of EVERYSK TECHNOLOGIES is prohibited.
 #
 ###############################################################################
 # pylint: disable=invalid-name, protected-access
 from os import environ
-from threading import Thread
 from unittest import TestCase, mock
 from everysk.core import firestore
 from everysk.core.compress import compress_pickle
 from everysk.config import settings
 from everysk.core.datetime import Date, DateTime
 from everysk.core.exceptions import FieldValueError
-from everysk.core.redis import Redis
+from everysk.core import redis as redis_module
 from everysk.core.threads import ThreadPool
 
 
 def _test_connection(Client: mock.MagicMock):
     doc = firestore.FirestoreClient(project_name='P01', database_name='D01')
     assert doc.connection == Client.return_value
 
@@ -274,15 +273,17 @@
     @mock.patch.object(firestore.DateTime, 'now', return_value='2023-10-11T00:00:00+00:00')
     def test_save(self, now: mock.MagicMock, Client: mock.MagicMock):
         firestore.Document.config.collection_name = 'my-collection'
         doc = firestore.Document(firestore_id='my-id', var='1', created_at='2023-04-03T00:00:00+00:00')
         doc.save()
         Client.return_value.collection.return_value.document.assert_called_once_with('my-id')
         Client.return_value.collection.return_value.document.return_value.set.assert_called_once_with(
-            {'created_at': '2023-04-03T00:00:00+00:00', 'firestore_id': 'my-id', 'updated_at': '2023-10-11T00:00:00+00:00', 'var': '1'}, True
+            document_data={'created_at': '2023-04-03T00:00:00+00:00', 'firestore_id': 'my-id', 'updated_at': '2023-10-11T00:00:00+00:00', 'var': '1'},
+            merge=True,
+            timeout=60.0
         )
         now.assert_called_once_with()
         firestore.Document.config.collection_name = None
 
     def test_to_dict(self, Client: mock.MagicMock):
         obj = FakeObject()
         doc = firestore.Document(
@@ -416,14 +417,15 @@
         Client.return_value.collection.assert_called_once_with('my-collection')
         Client.return_value.collection.return_value.select.assert_called_once_with(field_paths=['created_at', 'firestore_id', 'mic', 'updated_at'])
         Client.return_value.collection.return_value.select.return_value.order_by.assert_called_once_with('mic')
         Client.return_value.collection.return_value.select.return_value.order_by.return_value.limit.assert_called_once_with(100)
         Client.return_value.collection.return_value.select.return_value.order_by.return_value.limit.return_value.get.assert_called_once_with()
 
 
+@mock.patch.object(redis_module.log, 'debug', mock.MagicMock)
 class BaseDocumentCachedConfigTestCase(TestCase):
 
     def test_readonly_attributes(self):
         msg = "The field 'key_prefix' value cannot be changed."
         self.assertRaisesRegex(FieldValueError, msg, firestore.BaseDocumentCachedConfig, key_prefix='BANANA')
         with self.assertRaisesRegex(FieldValueError, msg):
             firestore.BaseDocumentCachedConfig(key_prefix='BANANA')
@@ -444,15 +446,15 @@
 @mock.patch.object(firestore.firestore, 'Client')
 class DocumentCachedTestCase(TestCase):
     # pylint: disable=invalid-name
 
     @classmethod
     def setUpClass(cls) -> None:
         firestore.DocumentCached.config.collection_name = 'my-collection'
-        cls.redis = Redis(host=settings.REDIS_HOST, port=settings.REDIS_PORT)
+        cls.redis = redis_module.Redis(host=settings.REDIS_HOST, port=settings.REDIS_PORT)
         cls.key = '86085ac4d100a96d4e1739e87857bd4e266f6a2e4ad62b7ac5bee2aa62f88d2e'
 
     @classmethod
     def tearDownClass(cls) -> None:
         firestore.DocumentCached.config.collection_name = None
 
     def setUp(self) -> None:
@@ -512,16 +514,17 @@
     @mock.patch.object(firestore.DateTime, 'now', return_value='2023-11-11T00:00:00+00:00')
     def test_save(self, now: mock.MagicMock, Client: mock.MagicMock):
         doc = firestore.DocumentCached(firestore_id='my-id', created_at='2023-04-03T00:00:00+00:00')
         self.assertIsNotNone(doc.config.cache.get(doc.get_cache_key()))
         doc.save()
         self.assertIsNone(doc.config.cache.get(doc.get_cache_key()))
         Client.return_value.collection.return_value.document.return_value.set.assert_called_once_with(
-            {
+            document_data={
                 'created_at': '2023-04-03T00:00:00+00:00',
                 'firestore_id': 'my-id',
                 'redis_key': '86085ac4d100a96d4e1739e87857bd4e266f6a2e4ad62b7ac5bee2aa62f88d2e',
                 'updated_at': '2023-11-11T00:00:00+00:00',
             },
-            True
+            merge=True,
+            timeout=60.0
         )
         now.assert_called_once_with()
```

### Comparing `everysk_beta-1.3.656/src/everysk/core/_tests/log.py` & `everysk_beta-1.4.815/src/everysk/core/_tests/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 ###############################################################################
 # pylint: disable=protected-access
 import sys
 from logging import Logger as PythonLogger, DEBUG, INFO, StreamHandler
 from unittest import TestCase, mock
 from everysk.config import settings
-from everysk.core import log as log_module
+from everysk.core import log as log_module, slack as slack_module
 from everysk.core.log import Logger, LoggerManager
 
 
 class LoggerManagerTestCase(TestCase):
 
     def test_context_manager(self):
         with LoggerManager(labels={'key': 'out'}):
@@ -188,15 +188,15 @@
         log.deprecated('Teste 2', show_once=False)
         getLogger.return_value.warning.assert_has_calls([
             mock.call('DeprecationWarning: Teste 2', extra={'labels': {}}, stacklevel=2),
             mock.call('DeprecationWarning: Teste 2', extra={'labels': {}}, stacklevel=2),
         ])
 
 
-@mock.patch.object(log_module, 'Slack')
+@mock.patch.object(slack_module, 'Slack')
 class LoggerSlackTestCase(TestCase):
 
     @classmethod
     def setUpClass(cls) -> None:
         cls.log = Logger(name='everysk-lib-test-slack-message')
 
     def setUp(self) -> None:
```

### Comparing `everysk_beta-1.3.656/src/everysk/core/_tests/number.py` & `everysk_beta-1.4.815/src/everysk/core/_tests/number.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/core/_tests/object.py` & `everysk_beta-1.4.815/src/everysk/core/_tests/object.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,23 @@
         _validate(attr_name='test', value=None, attr_type=DateTime)
         _validate(attr_name='test', value=None, attr_type=dict)
         _validate(attr_name='test', value=None, attr_type=float)
         _validate(attr_name='test', value=None, attr_type=int)
         _validate(attr_name='test', value=None, attr_type=list)
         _validate(attr_name='test', value=None, attr_type=str)
 
+    def test_undefined(self):
+        _validate(attr_name='test', value=Undefined, attr_type=Date)
+        _validate(attr_name='test', value=Undefined, attr_type=DateTime)
+        _validate(attr_name='test', value=Undefined, attr_type=dict)
+        _validate(attr_name='test', value=Undefined, attr_type=float)
+        _validate(attr_name='test', value=Undefined, attr_type=int)
+        _validate(attr_name='test', value=Undefined, attr_type=list)
+        _validate(attr_name='test', value=Undefined, attr_type=str)
+
     def test_date(self):
         _validate(attr_name='test', value=Date.today(), attr_type=Date)
         self.assertRaises(FieldValueError, _validate, attr_name='test', value=DateTime.now(), attr_type=Date)
         self.assertRaises(FieldValueError, _validate, attr_name='test', value='1', attr_type=Date)
         self.assertRaises(FieldValueError, _validate, attr_name='test', value=1, attr_type=Date)
         self.assertRaises(FieldValueError, _validate, attr_name='test', value=1.0, attr_type=Date)
         self.assertRaises(FieldValueError, _validate, attr_name='test', value=[], attr_type=Date)
@@ -104,19 +113,26 @@
     def test_any(self):
         _validate(attr_name='test', value=None, attr_type=Any)
         _validate(attr_name='test', value={}, attr_type=Any)
         _validate(attr_name='test', value=[], attr_type=Any)
         _validate(attr_name='test', value=123, attr_type=Any)
         _validate(attr_name='test', value='123', attr_type=Any)
         _validate(attr_name='test', value=callable, attr_type=Any)
+        _validate(attr_name='test', value=Undefined, attr_type=Any)
+        _validate(attr_name='test', value=Undefined.default_parse_string, attr_type=Any)
 
     def test_callable(self):
         _validate(attr_name='test', value=lambda x: x, attr_type=callable)
         with self.assertRaisesRegex(FieldValueError, 'Key test must be <built-in function callable>.'):
-            _validate(attr_name='test', value=None, attr_type=callable)
+            _validate(attr_name='test', value='func', attr_type=callable)
+
+    def test_annotation_string(self):
+        _validate(attr_name='test', value=object(), attr_type='object')
+        with self.assertRaisesRegex(FieldValueError, 'Key test must be object.'):
+            _validate(attr_name='test', value=str(), attr_type='object')
 
 
 class BaseFieldTestCase(TestCase):
 
     def test_init(self):
         field = BaseField(attr_type=str, default='default', required=True, readonly=True, other='Test')
         self.assertEqual(field.attr_type, str)
@@ -154,18 +170,24 @@
     def test_validate_readonly(self):
         field = BaseField(attr_type=str, readonly=True, default='Teste')
         self.assertRaises(FieldValueError, field.validate, attr_name='test', value='new')
 
     def test_validate_required(self):
         field = BaseField(attr_type=str, required=True)
         self.assertRaises(RequiredError, field.validate, attr_name='test', value=None)
+        field = BaseField(default=Undefined, attr_type=int, required=True)
+        self.assertRaises(RequiredError, field.validate, attr_name='test', value=None)
+        field = BaseField(default=Undefined.default_parse_string, attr_type=int, required=True)
+        self.assertRaises(RequiredError, field.validate, attr_name='test', value=None)
 
     def test_validate_required_lazy(self):
         field = BaseField(attr_type=str, required=False, required_lazy=True)
         field.validate(attr_name='test', value=None)
+        field = BaseField(attr_type=int, required=False, required_lazy=True)
+        field.validate(attr_name='test', value=Undefined)
 
     def test_repr(self):
         field = BaseField(attr_type=str)
         self.assertEqual(repr(field), 'BaseField')
 
     def test_get_value(self):
         def func():
@@ -314,15 +336,15 @@
 
     def test_get_attribute_inheritance_class(self):
         self.assertEqual(BaseObjectAttributeInheritanceTestClass.local_attr, 'Local Field')
         self.assertEqual(BaseObjectAttributeInheritanceTestClass.field_readonly, 'default_value')
 
     def test_get_attribute_class_error(self):
         with self.assertRaisesRegex(AttributeError, "type object 'BaseObjectFieldsTestClass' has no attribute 'field_default_erro'"):
-            BaseObjectFieldsTestClass.field_default_erro # pylint: disable=pointless-statement
+            BaseObjectFieldsTestClass.field_default_erro # pylint: disable=pointless-statement, no-member
 
     def test_get_clean_value(self):
         obj = BaseObjectFieldsTestClass()
         self.assertIsNone(obj.field1)
         obj.field1 = 21
         self.assertEqual(obj.field1, 21)
 
@@ -407,14 +429,43 @@
 class BaseDictRequiredLazyTestClass(BaseDict):
     normal: bool = True
     required = BaseField(attr_type=int, required_lazy=True)
 
 class BaseDictBoolTestClass(BaseDict):
     attr = BoolField()
 
+class BaseDictUndefinedTestClass(BaseDict):
+    attr = BaseField(default=Undefined, attr_type=str)
+
+class FakeNPArray:
+    def __eq__(self, obj: Any) -> bool:
+        raise ValueError('The truth value of an array with more than one element is ambiguous. Use a.any() or a.all()')
+
+class BaseDictNpArrayTestCase(BaseDict):
+    attr: FakeNPArray = None
+
+class NpArrayTestCase(TestCase):
+
+    def test_equal_raise(self):
+        obj = FakeNPArray()
+        with self.assertRaisesRegex(ValueError, r'The truth value of an array with more than one element is ambiguous. Use a.any\(\) or a.all\(\)'):
+            assert obj == ''
+
+    def test_set_value(self):
+        fake_np_array = FakeNPArray()
+
+        obj = BaseDictNpArrayTestCase()
+        obj.attr = fake_np_array
+        self.assertIsNotNone(obj.attr)
+        self.assertIsNotNone(obj['attr'])
+
+        obj = BaseDictNpArrayTestCase(attr=fake_np_array)
+        self.assertIsNotNone(obj.attr)
+        self.assertIsNotNone(obj['attr'])
+
 class BaseDictTestCase(TestCase):
 
     def test_init(self):
         obj = BaseDictTestClass()
         self.assertIsNone(obj.attr)
         self.assertIsNone(obj['field'])
 
@@ -610,14 +661,38 @@
     def test_replace_config(self):
         obj1 = BaseDict()
         obj1.config = 1
         obj2 = obj1.replace(public=4)
         with self.assertRaisesRegex(AttributeError, "'BaseDict' object has no attribute 'config'"):
             obj2.config # pylint: disable=pointless-statement
 
+    def test_init_with_undefined(self):
+        obj = BaseDictUndefinedTestClass(attr='foo')
+        self.assertEqual(obj.attr, 'foo')
+        self.assertEqual(obj['attr'], 'foo')
+        obj = BaseDictUndefinedTestClass(attr=Undefined.default_parse_string)
+        self.assertEqual(obj.attr, Undefined)
+        self.assertEqual(obj['attr'], Undefined)
+        obj = BaseDictUndefinedTestClass(attr=Undefined)
+        self.assertEqual(obj.attr, Undefined)
+        self.assertEqual(obj['attr'], Undefined)
+        obj = BaseDictUndefinedTestClass(attr=None)
+        self.assertEqual(obj.attr, None)
+        self.assertEqual(obj['attr'], None)
+
+    def test_set_undefined(self):
+        obj = BaseDictUndefinedTestClass()
+        obj.attr = Undefined.default_parse_string
+        self.assertEqual(obj.attr, Undefined)
+        self.assertEqual(obj['attr'], Undefined)
+
+        obj.attr = Undefined
+        self.assertEqual(obj.attr, Undefined)
+        self.assertEqual(obj['attr'], Undefined)
+
 
 class BaseDictProperty(BaseDict):
     _to_date = BaseField(attr_type=str)
 
     @property
     def to_date(self):
         return self._to_date
@@ -663,23 +738,26 @@
 
     config: Config
 
 
 class MetaClassConfigTestCase(TestCase):
 
     def setUp(self) -> None:
+        # pylint: disable=no-member
         BaseObjectConfig.config.value = 1
         BaseDictConfig.config.value = 1
 
     def test_object_config_attribute(self):
+        # pylint: disable=no-member
         self.assertEqual(BaseObjectConfig.config.value, 1)
         obj = BaseObjectConfig()
         self.assertEqual(obj.config.value, BaseObjectConfig.config.value)
 
     def test_object_config_singleton(self):
+        # pylint: disable=no-member
         obj = BaseObjectConfig()
         obj.config.value = 3
         self.assertEqual(BaseObjectConfig.config.value, 3)
         self.assertEqual(obj.config.value, BaseObjectConfig.config.value)
 
     def test_object_config_delete(self):
         obj = BaseObjectConfig()
@@ -898,14 +976,15 @@
     class Config:
         pass
 
 class ConfigHashTestCase(TestCase):
     # https://everysk.atlassian.net/browse/COD-2746
 
     def test_different_values(self):
+        # pylint: disable=no-member
         self.assertEqual(FakeBaseObject.config.f1, 'FakeBaseObject')
         self.assertEqual(FakeBaseObject.config.f2, 'FakeBaseObject')
         self.assertEqual(FakeBaseDict.config.f1, 'FakeBaseDict')
         self.assertEqual(FakeBaseDict.config.f2, 'FakeBaseDict')
 
     def test_python_qualname(self):
         self.assertEqual(Fake01PythonClass.Config.__name__, 'Config')
@@ -1088,7 +1167,85 @@
         obj = MetaClassParent(p01='01')
         self.assertEqual(obj.p01, '01')
         self.assertEqual(obj.prop, '01')
 
         obj = MetaClassParent(prop='02')
         self.assertEqual(obj.p01, '02')
         self.assertEqual(obj.prop, '02')
+
+
+class BeforeInitTestCase(TestCase):
+
+    class BeforeInitBaseObject(BaseObject):
+        key: str = None
+
+        @classmethod
+        def __before_init__(cls, **kwargs: dict) -> dict:
+            return {'key': 'before'}
+
+    class BeforeInitBaseDict(BaseDict):
+        key: str = None
+
+        @classmethod
+        def __before_init__(cls, **kwargs: dict) -> dict:
+            return {'key': 'before'}
+
+    class BeforeInitBaseObjectNone(BaseObject):
+        key: str = None
+
+        @classmethod
+        def __before_init__(cls, **kwargs: dict) -> dict:
+            return None
+
+    class BeforeInitBaseDictNone(BaseDict):
+        key: str = None
+
+        @classmethod
+        def __before_init__(cls, **kwargs: dict) -> dict:
+            return None
+
+    def test_base_object(self):
+        obj = BeforeInitTestCase.BeforeInitBaseObject(key='test')
+        self.assertEqual(obj.key, 'before')
+
+    def test_base_object_none(self):
+        obj = BeforeInitTestCase.BeforeInitBaseObjectNone(key='test')
+        self.assertEqual(obj.key, 'test')
+
+    def test_base_dict(self):
+        obj = BeforeInitTestCase.BeforeInitBaseDict(key='test')
+        self.assertEqual(obj.key, 'before')
+        self.assertEqual(obj['key'], 'before')
+
+    def test_base_dict_none(self):
+        obj = BeforeInitTestCase.BeforeInitBaseDictNone(key='test')
+        self.assertEqual(obj.key, 'test')
+        self.assertEqual(obj['key'], 'test')
+
+
+class AfterInitTestCase(TestCase):
+
+    class AfterInitBaseObject(BaseObject):
+        key: str = None
+        def __after_init__(self) -> None:
+            self.key = 'after'
+
+    class AfterInitBaseDict(BaseDict):
+        key: str = None
+        def __after_init__(self) -> None:
+            self.key = 'after'
+
+    def test_after_base_object(self):
+        obj = BaseObject(key='test')
+        self.assertEqual(obj.key, 'test')
+
+        obj = AfterInitTestCase.AfterInitBaseObject(key='test')
+        self.assertEqual(obj.key, 'after')
+
+    def test_after_base_dict(self):
+        obj = BaseDict(key='test')
+        self.assertEqual(obj.key, 'test')
+        self.assertEqual(obj['key'], 'test')
+
+        obj = AfterInitTestCase.AfterInitBaseDict(key='test')
+        self.assertEqual(obj.key, 'after')
+        self.assertEqual(obj['key'], 'after')
```

### Comparing `everysk_beta-1.3.656/src/everysk/core/_tests/redis.py` & `everysk_beta-1.4.815/src/everysk/core/_tests/redis.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     def test_connection_error_connection(self, _connect: mock.MagicMock):
         with mock.patch.object(RedisClient, '_connection', spec=redis_module.Redis) as _connection:
             _connection.ping.side_effect = exceptions.ConnectionError
             connection = RedisClient().connection # pylint: disable=unused-variable
             _connection.ping.assert_called_once_with()
         _connect.assert_called_once_with()
 
+    @mock.patch.object(redis_module.log, 'debug', mock.MagicMock)
     def test_flush_all(self):
         cli = RedisClient()
         # Generate a random key to test
         key = uuid4().hex
         cli.connection.set(key, 'Flush-test')
         cli.flush_all()
         self.assertIsNone(cli.connection.get(key))
```

### Comparing `everysk_beta-1.3.656/src/everysk/core/_tests/slack.py` & `everysk_beta-1.4.815/src/everysk/core/_tests/slack.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/core/_tests/string.py` & `everysk_beta-1.4.815/src/everysk/core/_tests/string.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/core/_tests/threads.py` & `everysk_beta-1.4.815/src/everysk/core/_tests/threads.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,78 +3,73 @@
 # (C) Copyright 2023 EVERYSK TECHNOLOGIES
 #
 # This is an unpublished work containing confidential and proprietary
 # information of EVERYSK TECHNOLOGIES. Disclosure, use, or reproduction
 # without authorization of EVERYSK TECHNOLOGIES is prohibited.
 #
 ###############################################################################
+# pylint: disable=protected-access
 from concurrent import futures
 from contextvars import ContextVar
 from time import sleep
-from threading import Semaphore
 from unittest import TestCase, mock
 from everysk.core import threads
 from everysk.core.datetime import DateTime
 
 
+user = ContextVar('username', default='default_user')
+def fake_func_context_var():
+    return user.get()
+
 def div(v1: int, v2: int) -> int:
     sleep(0.1)
     return v1 / v2
 
 
 class ThreadTestCase(TestCase):
 
     def test_results(self):
         results = []
-        t1 = threads.Thread(target=div, args=(1, 2), results=results)
-        t2 = threads.Thread(target=div, args=(1, 4), results=results)
+        t1 = threads.Thread(target=div, args=(1, 2))
+        t2 = threads.Thread(target=div, args=(1, 4))
         t1.start()
         t2.start()
-        t1.join()
-        t2.join()
+        results = [t1.join(), t2.join()]
         self.assertEqual(len(results), 2)
         self.assertIn(0.25, results)
         self.assertIn(0.5, results)
 
-    def test_semaphore(self):
-        semaphore = mock.MagicMock(spec=Semaphore)
-        t1 = threads.Thread(target=div, args=(1, 2), semaphore=semaphore)
-        t1.start()
-        t1.join()
-        semaphore.assert_has_calls([
-            mock.call.acquire(blocking=True),
-            mock.call.acquire().__bool__(), # pylint: disable=unnecessary-dunder-call
-            mock.call.release()
-        ])
-
     @mock.patch.object(threads, 'log')
     def test_error(self, log: mock.MagicMock):
         t1 = threads.Thread(target=div, args=(1, 0))
         t1.start()
         t1.join()
         log.error.assert_called_once_with(
-            'Thread execution error. target: %s, args: %s, kwargs: %s, traceback: %s',
+            'Thread execution error -> target: %s, args: %s, kwargs: %s, traceback: %s',
             div,
             (1, 0),
             {},
-            f'Traceback (most recent call last):\n  File "{threads.__file__}", line 74, in run\n    result = self._target(*self._args, **self._kwargs)\n             ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n  File "{__file__}", line 21, in div\n    return v1 / v2\n           ~~~^~~~\nZeroDivisionError: division by zero\n'
+            f'Traceback (most recent call last):\n  File "{threads.__file__}", line 177, in wait\n    self.results.append(future.result())\n                        ^^^^^^^^^^^^^^^\n  File "{futures._base.__file__}", line 449, in result\n    return self.__get_result()\n           ^^^^^^^^^^^^^^^^^^^\n  File "{futures._base.__file__}", line 401, in __get_result\n    raise self._exception\n  File "{futures.thread.__file__}", line 58, in run\n    result = self.fn(*self.args, **self.kwargs)\n             ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n  File "{__file__}", line 25, in div\n    return v1 / v2\n           ~~~^~~~\nZeroDivisionError: division by zero\n'
         )
 
+    def test_context_var(self):
+        user.set('new_user')
+        thread = threads.Thread(target=fake_func_context_var)
+        thread.start()
+        result = thread.join()
+        self.assertEqual(result, 'new_user')
+
 
 def fake_func():
     sleep(1)
     return DateTime.now()
 
 def fake_func_error():
     raise KeyError('MyKey')
 
-user = ContextVar('username', default='default_user')
-def fake_func_context_var():
-    return user.get()
-
 
 class ThreadPoolTestCase(TestCase):
 
     def test_results(self):
         pool = threads.ThreadPool()
         pool.add(target=div, args=(1, 2))
         pool.add(target=div, args=(1, 4))
@@ -108,15 +103,15 @@
         pool.add(target=fake_func_error)
         pool.wait()
         error.assert_called_once_with(
             'Thread execution error -> target: %s, args: %s, kwargs: %s, traceback: %s',
             fake_func_error,
             (),
             {},
-            f'Traceback (most recent call last):\n  File "{threads.__file__}", line 191, in wait\n    self.results.append(future.result())\n                        ^^^^^^^^^^^^^^^\n  File "{futures._base.__file__}", line 449, in result\n    return self.__get_result()\n           ^^^^^^^^^^^^^^^^^^^\n  File "{futures._base.__file__}", line 401, in __get_result\n    raise self._exception\n  File "{futures.thread.__file__}", line 58, in run\n    result = self.fn(*self.args, **self.kwargs)\n             ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n  File "{__file__}", line 68, in fake_func_error\n    raise KeyError(\'MyKey\')\nKeyError: \'MyKey\'\n'
+            f'Traceback (most recent call last):\n  File "{threads.__file__}", line 177, in wait\n    self.results.append(future.result())\n                        ^^^^^^^^^^^^^^^\n  File "{futures._base.__file__}", line 449, in result\n    return self.__get_result()\n           ^^^^^^^^^^^^^^^^^^^\n  File "{futures._base.__file__}", line 401, in __get_result\n    raise self._exception\n  File "{futures.thread.__file__}", line 58, in run\n    result = self.fn(*self.args, **self.kwargs)\n             ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n  File "{__file__}", line 67, in fake_func_error\n    raise KeyError(\'MyKey\')\nKeyError: \'MyKey\'\n'
         )
 
     @mock.patch.object(threads.log, 'error')
     def test_raise_thread(self, error: mock.MagicMock):
         pool = threads.ThreadPool(concurrency=1, silent=False)
         pool.add(target=fake_func_error)
         with self.assertRaisesRegex(KeyError, 'MyKey'):
```

### Comparing `everysk_beta-1.3.656/src/everysk/core/_tests/undefined.py` & `everysk_beta-1.4.815/src/everysk/core/_tests/undefined.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/core/_tests/utils.py` & `everysk_beta-1.4.815/src/everysk/core/_tests/utils.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/core/_tests/workers.py` & `everysk_beta-1.4.815/src/everysk/core/_tests/workers.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/core/cloud_function/main.py` & `everysk_beta-1.4.815/src/everysk/core/cloud_function/main.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/core/cloud_function/tests.py` & `everysk_beta-1.4.815/src/everysk/core/cloud_function/tests.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/core/datetime/__init__.py` & `everysk_beta-1.4.815/src/everysk/core/datetime/__init__.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/core/datetime/calendar.py` & `everysk_beta-1.4.815/src/everysk/core/datetime/calendar.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,41 +9,96 @@
 ###############################################################################
 
 import holidays
 from holidays.countries import BR
 from everysk.core.datetime import Date
 
 class BRHolidays(BR):
+    """
+    Subclass of BR representing holidays specific to Brazil and also provides further functionality
+    """
 
     def _populate(self, year):
+        """
+        Populate holidays specific to Brazil for the given year
+
+        Args:
+            year (int): The year for which holidays are to be populated
+
+        Usage:
+            >>> from everysk.core.datetime.calendar import BRHolidays
+            >>> br_holidays = BRHolidays()
+            >>> br_holidays._populate(2022)
+            >>> print(br_holidays)
+            {
+                datetime.date(2022, 1, 1): 'Confraternização Universal',
+                datetime.date(2022, 4, 15): 'Sexta-feira Santa',
+                ...
+            }
+        """
         super()._populate(year)
 
         self.pop_named('Início da Quaresma')
         self.pop_named('Dia do Servidor Público')
         self.pop_named('Véspera de Natal')
         self.pop_named('Véspera de Ano-Novo')
 
 class ANBIMA(BRHolidays):
     pass
 
 class BVMF(BRHolidays):
+    """
+    Subclass of BRHolidays representing holidays specific to the BVMF calendar.
+    """
     def _populate(self, year):
+        """
+        _summary_
+
+        Args:
+            year (int): The year for the holidays to be populated
+
+        Usage:
+            Display the holidays for the year of 2022
+
+            >>> from everysk.core.datetime.calendar import BVMF
+            >>> bvmf_holidays = BVMF()
+            >>> bvmf_holidays._populate(2022)
+            >>> print(bvmf_holidays)
+            {
+                datetime.date(2022, 1, 1): 'Confraternização Universal',
+                datetime.date(2022, 4, 15): 'Sexta-feira Santa',
+                ...
+            }
+        """
         super()._populate(year)
 
         if year < 2022:
             self[Date(year, 1, 25)] = 'Aniversário de São Paulo'
             self[Date(year, 11, 20)] = 'Dia da Consciência Negra'
 
 def get_holidays(calendar: str, years: list = range(2000, 2100)) -> dict:
     """
-    Uses https://pypi.org/project/holidays/ to make a list of dates.
-    Pass a list of years if you need a more specific list.
+    Uses the holidays library (https://pypi.org/project/holidays/) to retrieve a list of holidays for a specific country
+
+    It also uses a range of years, if more specification needed
 
     Args:
         calendar (str): Two digit country symbol.
         years (list, optional): List of int years. Ex: [2021, 2022]. Defaults to [2000, ..., 2099].
+
+    Usage:
+        Getting holidays for Brazil (BVMF calendar) for the years 2021 and 2022
+
+        >>> from everysk.core.datetime.calendar import get_holidays
+        >>> brazil_holidays = get_holidays('BR', years=[2021, 2022])
+        >>> print(brazil_holidays)
+        {
+            datetime.date(2021, 1, 1) : 'Confraternização Universal',
+            datetime.date(2021, 4, 2) : 'Sexta-feira Santa',
+            ...
+        }
     """
 
     holidays.BVMF = BVMF
     holidays.ANBIMA = ANBIMA
 
     return {Date(dt.year, dt.month, dt.day): name for dt, name in holidays.country_holidays(calendar, years=years).items()}
```

### Comparing `everysk_beta-1.3.656/src/everysk/core/datetime/date.py` & `everysk_beta-1.4.815/src/everysk/core/datetime/date.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/core/datetime/date_mixin.py` & `everysk_beta-1.4.815/src/everysk/core/datetime/date_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,28 +6,43 @@
 # This is an unpublished work containing confidential and proprietary
 # information of EVERYSK TECHNOLOGIES. Disclosure, use, or reproduction
 # without authorization of EVERYSK TECHNOLOGIES is prohibited.
 #
 ###############################################################################
 from calendar import monthrange, SATURDAY, SUNDAY
 from datetime import datetime, date, timedelta
-
-from typing import List, Union, Self
+from typing import List, Union, Self, TYPE_CHECKING
 
 from everysk.core.datetime import date_settings
 
+if TYPE_CHECKING:
+    from everysk.core.datetime import Date, DateTime
+
 
 def get_holidays(calendar: str, years: list = Undefined) -> dict:
     """
     Uses https://pypi.org/project/holidays/ to make a list of dates.
     Pass a list of years if you need a more specific list.
 
     Args:
         calendar (str): Two digit country symbol. Defaults to None.
         years (list, optional): List of int years. Ex: [2021, 2022].
+
+    Returns:
+        dict: A dictionary containing holiday dates as keys and holiday names as values.
+
+    Usage:
+        >>> from everysk.core.datetime.date_mixin import get_holidays
+        >>> br_holidays = get_holidays('BR', years=[2021, 2022])
+        >>> print(brazil_holidays)
+        {
+            datetime.date(2021, 1, 1): 'Confraternização Universal',
+            datetime.date(2023, 4, 2): 'Sexta-feira Santa',
+            ...
+        }
     """
     if calendar:
         kwargs = {'calendar': calendar}
 
         if years is not Undefined:
             kwargs['years'] = years
```

### Comparing `everysk_beta-1.3.656/src/everysk/core/datetime/date_settings.py` & `everysk_beta-1.4.815/src/everysk/core/datetime/date_settings.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/core/datetime/datetime.py` & `everysk_beta-1.4.815/src/everysk/core/datetime/datetime.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         Example of exception message:
             'ValueError: Invalid timestamp value.'
         """
         if tz is None:
             tz = ZoneInfo('UTC')
         return super().fromtimestamp(timestamp, tz)
 
-    # OLD date_time_ajust_time_zone
+    # OLD date_time_adjust_time_zone
     def adjust_time_zone(self, time_zone: str = date_settings.DEFAULT_TIME_ZONE) -> Self:
         """
         Adjust the time zone of a DateTime object by replacing its timezone information.
 
         Args:
             time_zone (str, optional): The time zone string to set for the date and time object.
                 Should be a valid time zone string recognized by `zoneinfo.ZoneInfo`.
@@ -362,21 +362,19 @@
         elif force_time == 'FIRST_MINUTE':
             hour, minute, second = 0, 0, 0
         elif force_time == 'LAST_MINUTE':
             hour, minute, second = 23, 59, 59
         else:
             raise ValueError("Invalid force_time. Please choose one of the following: NOW, MIDDAY, FIRST_MINUTE, LAST_MINUTE.")
 
-        self = self.replace(hour=hour, minute=minute, second=second)
-
-        return self
+        return self.replace(hour=hour, minute=minute, second=second)
 
     # OLD string_to_date_time
     @classmethod
-    def strptime(cls, date_string: str, format: str = date_settings.DEFAULT_DATE_TIME_FORMAT) -> Self:
+    def strptime(cls, date_string: str, format: str = date_settings.DEFAULT_DATE_TIME_FORMAT) -> Self: # pylint: disable=redefined-builtin
         """
         Parse a string representing a date and time into a DateTime object.
 
         This class method parses a string `date_string` representing a date and time according to the provided
         format string `format` and returns a DateTime object.
 
         Args:
@@ -403,15 +401,15 @@
 
         Example of exception message:
             'ValueError: time data '2023-09-15 12:00:00' does not match format '%Y-%m-%d %H:%M:%S''
         """
         return super().strptime(date_string, format)
 
     @classmethod
-    def strptime_or_null(cls, date_string: str, format: str = date_settings.DEFAULT_DATE_TIME_FORMAT) -> Union[Self, None]:
+    def strptime_or_null(cls, date_string: str, format: str = date_settings.DEFAULT_DATE_TIME_FORMAT) -> Union[Self, None]: # pylint: disable=redefined-builtin
         """
         Parse a string representing a date and time into a DateTime object, or return None if parsing fails.
 
         This class method attempts to parse a string `date_string` representing a date and time according to
         the provided format string `format` and returns a DateTime object. If parsing fails, it returns None.
 
         Args:
@@ -436,15 +434,15 @@
             >>> DateTime.strptime_or_null(invalid_date_string)
             None
         """
         date_time = None
 
         try:
             date_time = cls.strptime(date_string, format=format)
-        except Exception:
+        except Exception: # pylint: disable=broad-exception-caught
             pass
 
         return date_time
 
     # OLD string_date_to_date_time
     @classmethod
     def string_date_to_date_time(cls, date_string: str, force_time: str = date_settings.DEFAULT_FORCE_TIME) -> Self:
@@ -495,15 +493,15 @@
             force_time = super().utcnow().strftime('%H:%M:%S')
         elif force_time == 'FIRST_MINUTE':
             force_time = '00:00:00'
         elif force_time == 'LAST_MINUTE':
             force_time = '23:59:59'
         return super().strptime(f'{date_string} {force_time}', date_settings.DEFAULT_DATE_TIME_FORMAT)
 
-    def strftime(self, format: str = date_settings.DEFAULT_DATE_TIME_FORMAT) -> str:
+    def strftime(self, format: str = date_settings.DEFAULT_DATE_TIME_FORMAT) -> str: # pylint: disable=redefined-builtin, useless-parent-delegation
         """
         Convert a DateTime object to a date string.
 
         This method takes a DateTime object and converts it to a date string using the specified date format.
         If no format is provided, the method will use the default date format specified in `date_settings.DEFAULT_DATE_TIME_FORMAT`.
 
         Args:
@@ -533,15 +531,15 @@
 
         Example of exception message:
             'ValueError: Invalid format string. Please provide a valid date format string.'
         """
         return super().strftime(format)
 
     @classmethod
-    def strftime_or_null(cls, datetime_: Any, format: str = date_settings.DEFAULT_DATE_TIME_FORMAT) -> Union[str, None]:
+    def strftime_or_null(cls, datetime_: Any, format: str = date_settings.DEFAULT_DATE_TIME_FORMAT) -> Union[str, None]: # pylint: disable=redefined-builtin
         """
         Convert a `DateTime` object to a string representation or return None if the input is not a Date.
 
         This class method takes a `DateTime` object and converts it to a string representation
         using the specified date format. If the input date is None, the method returns None.
 
         Args:
@@ -572,15 +570,15 @@
 
         Example of exception message:
             'ValueError: Invalid format string. Please provide a valid date format string.'
         """
         if datetime_ is not None:
             try:
                 datetime_ = datetime_.strftime(format=format)
-            except Exception:
+            except Exception: # pylint: disable=broad-exception-caught
                 datetime_ = None
 
         return datetime_
 
     # OLD date_time_to_pretty
     def strftime_pretty(self, just_date: bool = False, just_time: bool = False) -> str:
         """
@@ -636,15 +634,15 @@
         else:
             out = self.strftime('%b. %d, %Y, %I:%M:%S %p')
         out = out.replace('PM', 'p.m.')
         out = out.replace('AM', 'a.m.')
         return out
 
     @classmethod
-    def date_to_date_time(cls, date_: 'Date', frc_time: str = date_settings.DEFAULT_FORCE_TIME) -> Self:
+    def date_to_date_time(cls, date_: 'Date', frc_time: str = date_settings.DEFAULT_FORCE_TIME) -> Self: # type: ignore
         """
         Convert a Date object to a DateTime object.
 
         This class method takes a Date object and converts it to a DateTime
         object by combining the specified `date` with the provided `frc_time`, creating a combined
         date and time representation.
```

### Comparing `everysk_beta-1.3.656/src/everysk/core/datetime/tests/calendar.py` & `everysk_beta-1.4.815/src/everysk/core/datetime/tests/calendar.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/core/datetime/tests/date.py` & `everysk_beta-1.4.815/src/everysk/core/datetime/tests/date.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/core/datetime/tests/date_mixin.py` & `everysk_beta-1.4.815/src/everysk/core/datetime/tests/date_mixin.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/core/datetime/tests/datetime.py` & `everysk_beta-1.4.815/src/everysk/core/datetime/tests/datetime.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/core/firestore.py` & `everysk_beta-1.4.815/src/everysk/core/firestore.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from everysk.core.redis import RedisCacheCompressed, RedisLock
 from everysk.core.object import BaseDict, BaseObject
 
 
 class FirestoreClient(BaseObject):
     """
     Client that creates a connection with the Firestore database.
+
     If the project name and the database name are not passed as params we use
     the ones that are on the settings module.
 
     Example:
 
         >>> from everysk.core.firestore import FirestoreClient
         >>> FirestoreClient(project_name='teste', database_name='default')
@@ -37,14 +38,21 @@
     _connections: dict = {}
 
     ## Public attributes
     database_name = StrField()
     project_name = StrField()
 
     def __init__(self, **kwargs) -> None:
+        """
+        Initializes a FirestoreClient instance with the specified project name and database name
+
+        Args:
+            ** kwargs: Additional keyword arguments.
+        """
+
         super().__init__(**kwargs)
         if self.database_name is None:
             self.database_name = _DEFAULT_DATABASE
 
         if self.project_name is None:
             self.project_name = settings.EVERYSK_GOOGLE_CLOUD_PROJECT
 
@@ -81,14 +89,17 @@
 
     def get_collection(self, collection_name: str) -> CollectionReference:
         """
         Returns the CollectionReference object that refers to the collection_name inside Firestore.
 
         Args:
             collection_name (str): The name of the collection.
+
+        Returns:
+            CollectionReference: TheCollectionReference object representing the specified collection
         """
         return self.connection.collection(collection_name)
 
 
 class BaseDocumentConfig(BaseObject):
     """
     Base class that has all config values used inside the Document class.
@@ -102,22 +113,38 @@
     excluded_keys = ListField()
     project_name = StrField()
 
     @property
     def client(self) -> FirestoreClient:
         """
         We use this property to create the connection if it does not exists.
+
+        If the client instance does not exist, it will be created using the project_name and the database_name attributes.
+
+        Returns:
+            FirestoreClient: The Firestore client instance.
         """
         if self._client is None:
             self._client = FirestoreClient(project_name=self.project_name, database_name=self.database_name)
         return self._client
 
     @property
     def collection(self) -> CollectionReference:
-        """ Alias to the CollectionReference on Firestore"""
+        """
+        Alias to the CollectionReference on Firestore
+
+        This property retrieves the CollectionReference associated with the specified
+        collection name from the Firestore client.
+
+        Raises:
+            AttributeError: If the collection_name attribute is empty
+
+        Returns:
+            CollectionReference: The CollectionReference object representing the specified collection
+        """
         if not self.collection_name:
             raise AttributeError('The collection_name is empty.')
 
         return self.client.get_collection(self.collection_name)
 
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
@@ -126,19 +153,31 @@
         if self.excluded_keys is None:
             self.excluded_keys = []
 
 
 class Document(BaseDict):
     """
     Class that represents a Document in Firestore database.
+
     All documents that use this class will have these fields:
 
     - created_at: A DateTime field that is filled when we create the object.
     - firestore_id: A string field that has the Document ID from Firestore.
     - updated_at: A DateTime field that is filled when we save the object.
+
+    Usage:
+        >>> from everysk.core.firestore import Document
+        >>> doc = Document(firestore_id='example_id', created_at='2024-03-18T12:00:00', updated_at='2024-03-18T12:30:00')
+        >>> print(doc)
+        {
+            'firestore_id': 'example_id',
+            'created_at': DateTime(2024, 3, 18, 12, 0, tzinfo=zoneinfo.ZoneInfo(key='UTC')),
+            'updated_at': DateTime(2024, 3, 18, 12, 30, tzinfo=zoneinfo.ZoneInfo(key='UTC'))
+        }
+
     """
     # This need to be configured on child classes
     class Config(BaseDocumentConfig):
         pass
 
     ## Public attributes
     config: BaseDocumentConfig = None # We put this here to use the Autocomplete correctly
@@ -152,15 +191,29 @@
             kwargs[key] = self._parser_in(value)
 
         super().__init__(**kwargs)
         if self.created_at is None:
             self.created_at = DateTime.now()
 
     def _parser_in(self, obj: Any) -> Any:
-        """ Parse all data to convert in python format to be used on the instance. """
+        """
+        Parse all data to convert in python format to be used on the instance.
+
+        Args:
+            obj (Any): The input data to be parsed
+
+        Notes:
+            - If the input is a dictionary, it recursively parses each key-value pair.
+            - If the input is a list, it recursively parses each item.
+            - If the input is a string, it attempts to parse as a date or a datetime obj
+            - If the input is bytes, it attempts to decompress it using pickle
+
+        Returns:
+            Any: The parsed data in Python format.
+        """
         ret = obj
         if isinstance(obj, dict):
             ret = {}
             for key, value in obj.items():
                 ret[key] = self._parser_in(value)
 
         elif isinstance(obj, list):
@@ -182,15 +235,29 @@
                 ret = decompress_pickle(obj)
             except Exception: # pylint: disable=broad-except
                 pass
 
         return ret
 
     def _parser_out(self, obj: Any) -> Any:
-        """ Parse all data to convert in Firestore format to be used on the save to Firestore. """
+        """
+        Parse all data to convert in Firestore format to be used on the save to Firestore.
+
+        Args:
+            obj (Any): The data to be parsed.
+
+        Notes:
+            - If the input is a dictionary, it recursively parses each key-value pair.
+            - If the input is a list, it recursively parses each item.
+            - If the input has an 'isoformat' method (e.g., datetime objects), it converts it to ISO format.
+            - All other non-primitive types are serialized using pickle and compressed before saving to Firestore.
+
+        Returns:
+            Any: The parsed data in Firestore-compatible format.
+        """
         ret = obj
         if obj is not None:
             if isinstance(obj, dict):
                 ret = {}
                 for key, value in obj.items():
                     ret[key] = self._parser_out(value)
 
@@ -264,38 +331,86 @@
             doc_aux = [cls(**doc.to_dict()) for doc in query.start_after(last).get()]
             docs.extend(doc_aux)
 
         return docs
 
     # Instance methods
     def get_firestore_id(self) -> str:
-        """ Uses the property firestore_id or generate one from UUID4. """
+        """
+        Uses the property firestore_id or generate one from UUID4.
+        If the document already has a 'firestore_id' attribute set it simply returns the value.
+        Otherwise, it generates a new ID using UUID4.
+
+        Usage:
+            >>> from everysk.core.firestore import Document
+            >>> doc = Document()
+            >>> firestore_id = doc.get_firestore_id()
+            >>> print(firestore_id)
+            >>> fb440ff261da42b48ff2332952bf240e
+
+        Returns:
+            str: The Firestore ID
+        """
         firestore_id = getattr(self, 'firestore_id', None)
         if not firestore_id:
             firestore_id = uuid4().hex
 
         return firestore_id
 
     def load(self) -> None:
-        """ Load all data from Firestore for self.firestore_id. """
+        """
+        Load all data from Firestore for self.firestore_id.
+        This method retrieves data from Firestore for the Firestore ID associated with the document.
+
+        Usage:
+            >>> from everysk.core.firestore import Document
+            >>> doc = Document(firestore_id='example_id')
+            >>> doc.load()
+        """
         doc = self.config.collection.document(self.get_firestore_id()).get()
         if doc.exists:
             # https://everysk.atlassian.net/browse/COD-1818
             # To convert all fields to the correct format we need to pass to _parser_in
             result = self._parser_in(doc.to_dict())
             self.update(result)
 
-    def save(self, merge: bool = True) -> dict:
-        """ Save/Update Firestore document, auto update 'updated_at' attribute before save. """
+    def save(self, merge: bool = True, timeout: float = 60.0) -> dict:
+        """
+        Save or Update Firestore document, auto update 'updated_at' attribute before save.
+
+        Args:
+            merge (bool, optional):
+                Determines the behavior of the save operation. If True, the method updates the
+                existing document, merging the new data with any existing data. If False, the method
+                replaces the existing document entirely with the new data.
+
+        Usage:
+            >>> doc = FirestoreDocument(...)
+            >>> doc.save(merge=True)  # Updates the document, preserving unspecified fields
+            >>> doc.save(merge=False) # Completely replaces the document with new data
+
+        Returns:
+            dict: A dictionary containing information about the save operation
+        """
         self.firestore_id = self.get_firestore_id()
         self.updated_at = DateTime.now()
-        return self.config.collection.document(self.firestore_id).set(self.to_dict(), merge)
+        return self.config.collection.document(self.firestore_id).set(
+            document_data=self.to_dict(),
+            merge=merge,
+            timeout=timeout
+        )
 
     def to_dict(self) -> dict:
-        """ Transform 'self' into a dict using _parse_out method to change some data. """
+        """
+        Transform 'self' into a dict using _parse_out method to change some data.
+        This method utilizes the `_parse_out` method to transform the data before converting it into a dictionary
+
+        Returns:
+            dict: A dictionary representation of the Document object
+        """
         ret = BaseDict()
         for key, value in self.items():
             # Discard some keys if needed
             if key not in self.config.excluded_keys:
                 ret[key] = self._parser_out(value)
 
         return ret
@@ -309,15 +424,22 @@
     _cache: RedisCacheCompressed = None
 
     ## Public attributes
     key_prefix = StrField(default='firestore-document-redis-cached', readonly=True)
 
     @property
     def cache(self) -> RedisCacheCompressed:
-        """ Used to access the cache instance, if we don't have a connection we create one. """
+        """
+        Used to access the cache instance
+
+        If we don't have a connection we create one.
+
+        Returns:
+            RedisCacheCompressed: The Redis cache instance.
+        """
         if self._cache is None:
             self._cache = RedisCacheCompressed()
         return self._cache
 
 
 class DocumentCached(Document):
     """
@@ -336,35 +458,63 @@
     firestore_id = StrField(required=True)
 
     # This key will be used to store the Firestore result in Redis and we need to store it
     # along with the document so that the trigger that syncs Firestore and Redis can use it.
     redis_key = StrField()
 
     def __init__(self, **kwargs) -> None:
+        """
+        Initializes a DocumentCached instance.
+
+        Args:
+            **kwargs: Additional keyword arguments
+        """
         super().__init__(**kwargs)
         self.load()
         # This keeps the redis_key hash always updated
         self.redis_key = self.config.cache.get_hash_key(self.get_cache_key())
 
     def clear_cache_key(self) -> None:
-        """ Delete the content from cache. """
+        """
+        Delete the content from cache.
+        This method removes the cached content from the Redis cache using the cache key generated by the `get_cache_key` method
+        """
         self.config.cache.delete(self.get_cache_key())
 
     def get_cache_key(self) -> str:
-        """ Returns the key that will be used to get/set the cache """
+        """
+        Returns the key that will be used to get/set the cache
+
+        Returns:
+            str: The cache key constructed using the document's collection name and Firestore ID.
+        """
         return f'{self.config.key_prefix}-{self.config.collection_name}-{self.get_firestore_id()}'
 
     ## Override methods to work with cache
     def load(self) -> None:
-        """ Load all data from Redis or Firestore """
+        """
+        Load all data from Redis or Firestore
+
+        This method attempts to retrieve the document data from the Redis cache using
+        the cache key generated by the `get_cache_key` method. If the data is found in
+        the cache, it updates the document with the cached data. Otherwise, it loads
+        the data from Firestore and stores it in the cache.
+        """
         key = self.get_cache_key()
         result = self.config.cache.get(key)
         if result is not None:
             self.update(result)
         else:
             super().load()
             self.config.cache.set(key, self.to_dict())
 
-    def save(self, merge: bool = True):
-        """ Removes the key from Redis and update the data on Firestore """
+    def save(self, merge: bool = True, timeout: float = 60) -> dict:
+        """
+        Save/Update Firestore document, auto update 'updated_at' attribute before save.
+        We clear the cache to be able to set the new value.
+
+        Args:
+            merge (bool, optional): If True, apply merging instead of overwriting the state of the document. Defaults to True
+            timeout (int, optional): The timeout for this request. Defaults to 60.0
+        """
         self.clear_cache_key()
-        return super().save(merge)
+        return super().save(merge, timeout)
```

### Comparing `everysk_beta-1.3.656/src/everysk/core/fixtures/_settings.py` & `everysk_beta-1.4.815/src/everysk/core/fixtures/_settings.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,21 +3,27 @@
 # (C) Copyright 2023 EVERYSK TECHNOLOGIES
 #
 # This is an unpublished work containing confidential and proprietary
 # information of EVERYSK TECHNOLOGIES. Disclosure, use, or reproduction
 # without authorization of EVERYSK TECHNOLOGIES is prohibited.
 #
 ###############################################################################
+import re
 from everysk.core.fields import BoolField, StrField
 
 
 _EVERYSK_PRIVATE = StrField(default='private-attribute')
 EVERYSK_TEST_NAME = StrField(default='test-case', readonly=True)
 EVERYSK_TEST_FAKE = True
 EVERYSK_TEST_INT: int = 1
 EVERYSK_TEST_FIELD_INHERIT = StrField(default='{EVERYSK_TEST_NAME} as {EVERYSK_TEST_FAKE}')
 EVERYSK_TEST_VAR_INHERIT = '{EVERYSK_TEST_FAKE} as {EVERYSK_TEST_NAME}'
 EVERYSK_TEST_BOOL_VAR = BoolField(default=False)
 
 # Settings with default values
 EVERYSK_TEST_STR_DEFAULT_NONE: str = None
 EVERYSK_TEST_STR_DEFAULT_UNDEFINED: str = Undefined
+
+# https://everysk.atlassian.net/browse/COD-4197
+EVERYSK_TEST_RE_PATTERN: re.Pattern = re.compile(r'[azAZ]')
+EVERYSK_TEST_RE_PATTERN_NONE: re.Pattern = None
+EVERYSK_TEST_RE_PATTERN_UNDEFINED: re.Pattern = Undefined
```

### Comparing `everysk_beta-1.3.656/src/everysk/core/fixtures/other/_settings.py` & `everysk_beta-1.4.815/src/everysk/core/fixtures/other/_settings.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/core/http.py` & `everysk_beta-1.4.815/src/everysk/core/http.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,79 +3,88 @@
 # (C) Copyright 2023 EVERYSK TECHNOLOGIES
 #
 # This is an unpublished work containing confidential and proprietary
 # information of EVERYSK TECHNOLOGIES. Disclosure, use, or reproduction
 # without authorization of EVERYSK TECHNOLOGIES is prohibited.
 #
 ###############################################################################
-#
+# pylint: disable=unused-import
 # Classes that handle HTTP Connections.
 
 # Url: https://requests.readthedocs.io/en/latest/
 #      https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers
 #      https://developer.mozilla.org/en-US/docs/Glossary/Quality_values
 #
 import random
 import time
 from os import getenv
 
 import requests
-from everysk.core.exceptions import HttpError
-from everysk.core.fields import BoolField, DictField, IntField, ReadonlyListField, StrField
+from everysk.core.exceptions import HttpError, InvalidArgumentError
 from everysk.core.object import BaseObject
-from everysk.core.compress import compress_json, decompress_json
+from everysk.core.serialize import dumps, loads
+from everysk.core.fields import BoolField, DictField, IntField, ListField, StrField
+from everysk.core.log import Logger
+from everysk.config import settings
+
+log = Logger(name='everysk-lib-core-http-log')
+
+class HttpConnectionConfig(BaseObject):
+    # Limit for retries
+    retry_limit = IntField(default=5)
+
+    # Times that randrange will use to do the next retry
+    retry_end_seconds = IntField(default=30)
+    retry_start_seconds = IntField(default=5)
+
+    # 200 - Default for success
+    # 202 - Default for success, but response is being processed.
+    success_status_codes = ListField(default=[200, 202], readonly=True)
 
 
 class HttpConnection(BaseObject):
     """
     Base class to use for HTTP connections, has two attributes:
         - timeout: It's in and represent seconds, defaults to 30.
         - url: It's string and will be the destination.
     """
-    ## Private attributes
-    _count = 1
+    class Config(HttpConnectionConfig):
+        pass
 
-    # 200 - Default for success
-    # 202 - Default for success, but response is being processed.
-    _success_status_codes = ReadonlyListField(default=[200, 202])
+    ## Private attributes
+    _retry_count = IntField(default=1) # Used to control how many times this connection was retry
 
     ## Public attributes
+    config: Config # To autocomplete correctly
     headers = DictField(default=None)
     timeout = IntField(default=30)
     url = StrField(default=None)
 
     def _clean_response(self, response: requests.models.Response) -> requests.models.Response:
         """
         Checks status_code for response, if status_code is different than 200 throws an exception.
 
         Args:
             response (requests.models.Response): Http response from server.
 
         Raises:
             HttpError: If something goes wrong raise exception with status_code and content.
         """
-        if getattr(response, 'status_code', self._success_status_codes[0]) not in self._success_status_codes:
+        if getattr(response, 'status_code', self.config.success_status_codes[0]) not in self.config.success_status_codes:
             raise HttpError(status_code=response.status_code, msg=response.content)
 
         return response
 
     def get_headers(self) -> dict:
         """
         Headers needed to send HTTP methods.
         Below are the most common Headers used by browsers,
         we use them to look less like a Bot and more like a valid access.
         """
-        headers = {
-            'Accept-Encoding': 'gzip, deflate;q=0.9',
-            'Accept-Language': 'en-US, en;q=0.9, pt-BR;q=0.8, pt;q=0.7',
-            'Cache-control': 'no-cache',
-            'Connection': 'close', # Remove on HTTP/2 requests
-            'Content-Type': 'text/html; charset=UTF-8',
-            'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/106.0.0.0 Safari/537.36'
-        }
+        headers = settings.HTTP_DEFAULT_HEADERS.copy()
         if self.headers is not None:
             headers.update(self.headers)
 
         return headers
 
     def get_url(self) -> str:
         """
@@ -97,25 +106,27 @@
         This will be implemented on child classes to really do the connection.
         """
         return None
 
     def get_response(self) -> requests.models.Response:
         """
         Try to fetch data from self.get_url and calling self._get_response_from_url for the complete response.
-        On HttpError, if self.message_error_check is True we will try connect again more 5 times.
+        On HttpError, if self.message_error_check is True we will try connect again for a few more times.
         """
         try:
             response = self._clean_response(self._get_response_from_url())
+            # After a success we set the value to 1 again
+            self._retry_count = 1
         except Exception as error: # pylint: disable=broad-exception-caught
             # Sometimes it can happen that the server is busy, if this happen the error message must be tested
             # and must return true to enable recursion and we will try again the connection.
-            if self.message_error_check(str(error).lower()) and self._count < 5:
-                self._count += 1
+            if self.message_error_check(str(error).lower()) and self._retry_count < self.config.retry_limit:
+                self._retry_count += 1
                 # As we have several processes, we use a random number to avoid collision between them.
-                time.sleep(random.randint(10, 120))
+                time.sleep(random.randint(self.config.retry_start_seconds, self.config.retry_end_seconds))
                 response = self.get_response()
             else:
                 raise error
 
         return response
 
 
@@ -142,15 +153,34 @@
             'headers': self.get_headers(),
             'params': self.get_params(),
             'timeout': self.timeout
         }
         if self.user:
             params['auth'] = (self.user, self.password)
 
-        return requests.get(**params)
+        if settings.HTTP_LOG_RESPONSE:
+            dct = params.copy()
+            # To remove the password in the logs
+            if 'auth' in params:
+                dct['auth'] = (params['auth'][0], '***********')
+
+            log.debug('HTTP GET request: %s', dct)
+
+        response = requests.get(**params)
+
+        if settings.HTTP_LOG_RESPONSE:
+            dct = {
+                'status_code': response.status_code,
+                'time': response.elapsed.total_seconds(),
+                'headers': response.headers,
+                'content': response.content
+            }
+            log.debug('HTTP GET response: %s', dct)
+
+        return response
 
 
 class HttpPOSTConnection(HttpConnection):
     """
     Class that implements a interface for HTTP POST connections.
     If self.is_json is True the POST method will be a JSON POST,
     otherwise will be a Form POST Data.
@@ -180,58 +210,76 @@
             'timeout': self.timeout
         }
         if self.is_json:
             params['json'] = self.get_payload()
         else:
             params['data'] = self.get_payload()
 
+        if settings.HTTP_LOG_RESPONSE:
+            log.debug('HTTP POST request: %s', params)
+
         response = requests.post(**params)
+
+        if settings.HTTP_LOG_RESPONSE:
+            dct = {
+                'status_code': response.status_code,
+                'time': response.elapsed.total_seconds(),
+                'headers': response.headers,
+                'content': response.content
+            }
+            log.debug('HTTP POST response: %s', dct)
+
         return response
 
+
 class HttpPOSTCompressedConnection(HttpPOSTConnection):
 
     def get_payload(self) -> dict:
         """ Make the correct payload body to pass on POST request. """
-        return compress_json(self.payload)
+        return dumps(self.payload)
 
     def get_response(self) -> dict:
         """
         Try to fetch data from self.get_url and calling self._get_response_from_url for the complete response.
         On HttpError, if self.message_error_check is True we will try connect again more 5 times.
         Decompress the response.content
         """
         response = super().get_response()
-        return decompress_json(response.content)
+        return loads(response.content)
+
 
 class HttpSDKPOSTConnection(HttpPOSTCompressedConnection):
 
     is_json = BoolField(default=False, readonly=True)
 
     class_name = StrField()
     method_name = StrField()
     self_obj = DictField()
     params = DictField()
 
-    def __init__(self, **kwargs) -> None:
-        if 'url' not in kwargs or kwargs['url'] is None:
-            kwargs['url'] = getenv('EVERYSK_API_URL', None)
-        super().__init__(**kwargs)
+    def get_url(self) -> str:
+        return f'{settings.EVERYSK_API_URL}/{settings.EVERYSK_SDK_VERSION}/{settings.EVERYSK_SDK_ROUTE}'
 
     def get_payload(self) -> dict:
         """ Make the correct payload body to pass on POST request. """
         self.payload = {
             'class_name': self.class_name,
             'method_name': self.method_name,
             'self_obj': self.self_obj,
             'params': self.params
         }
         return super().get_payload()
 
     def get_headers(self) -> dict:
         """ Headers needed to send HTTP Post methods. """
         headers = super().get_headers()
-        everysk_api_sid = getenv('EVERYSK_API_SID', None)
-        everysk_api_token = getenv('EVERYSK_API_TOKEN', None)
+        everysk_api_sid = settings.EVERYSK_API_SID
+        everysk_api_token = settings.EVERYSK_API_TOKEN
+
+        if not everysk_api_sid:
+            raise InvalidArgumentError('Invalid API SID')
+        if not everysk_api_token:
+            raise InvalidArgumentError('Invalid API TOKEN')
 
         headers['Authorization'] = f'Bearer {everysk_api_sid}:{everysk_api_token}'
 
         return headers
```

### Comparing `everysk_beta-1.3.656/src/everysk/core/log.py` & `everysk_beta-1.4.815/src/everysk/core/log.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import sys
 from contextlib import AbstractContextManager
 from contextvars import ContextVar
 from types import TracebackType
 from threading import Thread
 from typing import Any
 from everysk.config import settings
-from everysk.core.slack import Slack
 
 
 # This only makes sense in Production
 try:
     # Imports the Cloud Logging client library
     from google.cloud.logging.handlers import StructuredLogHandler # type: ignore
 except ImportError:
@@ -116,29 +115,50 @@
             name (str): Attribute name.
             value (Any): Value that should be validated.
             default (Any): Default value if "value" is Undefined.
             klass (type): Class used to check if the "value" is an instance.
 
         Raises:
             ValueError: If the value is not of the klass type.
+
+        Returns:
+            None
+
+        Usage:
+            >>> from everysk.core.log import Logger
+            >>> obj = Logger()
+            >>> obj._set_value(name='example_attribute', value=42, default=0, klass=int)
+            >>> print(obj.example_attribute)
+            >>> 42
+
         """
         if value is Undefined:
             value = default
         elif not isinstance(value, klass):
             raise ValueError(f'The "{name}" attribute must be a {klass}.')
 
         setattr(self, name, value)
 
     ## Methods
     def get_python_logger(self) -> logging.Logger:
         """
         Method that creates/get the Python Logger object and attach the correct handler.
         If you need to deactivate the Google Logging Handler, set the settings.EVERYSK_GOOGLE_CLOUD_LOGGING_INTEGRATION
-        to False or does not install the Handler pip package.
+        to False or do not install the Handler pip package.
         The default handler will be the stdout.
+
+        Returns:
+            logging.Logger: The Python Logger object.
+
+        Usage:
+            >>> logger = Logger(name='example_log')
+            >>> python_logger = logger.get_python_logger()
+            >>> print(python_logger)
+            <Logger example_log (DEBUG)>
+
         """
         # Create the log
         log = logging.getLogger(self.name)
         log.setLevel(self.level)
         log.propagate = False # Don't pass message to others loggers
 
         # We should only have one handler per log name
@@ -158,16 +178,25 @@
         log.handler.setLevel(self.level)
 
         return log
 
     def get_labels(self) -> dict:
         """
         The labels are extra information that the Google Logging uses to create filters.
+
         Normally we set one at every request to be able to filter all logs from one request.
         If they are not set an empty dict will be the default value.
+
+        Returns:
+            dict: The labels dictionary
+
+        Usage:
+            >>> from everysk.core.log import Logger
+            >>> logger = Logger()
+            >>> labels = logger.get_labels()
         """
         labels = self.labels.copy()
         context_labels = LoggerManager.labels.get()
         if context_labels:
             labels.update(context_labels)
 
         return labels
@@ -256,14 +285,16 @@
             if self.slack_url is None:
                 url = settings.SLACK_URL
             else:
                 url = self.slack_url
 
         # We send the message only if url is set and we are in PROD
         if url and settings.PROFILE == 'PROD' and 'unittest' not in sys.modules:
+            # The import must be here to avoid circular import inside http module
+            from everysk.core.slack import Slack # pylint: disable=import-outside-toplevel
             client = Slack(title=title, message=message, color=color, url=url)
             # This will send the message to Slack without block the request
             Thread(target=client.send).start()
 
         log_message = f'Slack message: {title} -> {message}'
         if color == 'danger':
             self.error(log_message)
```

### Comparing `everysk_beta-1.3.656/src/everysk/core/number.py` & `everysk_beta-1.4.815/src/everysk/core/number.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/core/object.py` & `everysk_beta-1.4.815/src/everysk/core/object.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,17 @@
         obj (Any): A class or a instance of BaseObject.
         attr (str): The attribute name.
         value (Any): The value that is assigned to this attribute.
 
     Raises:
         FieldValueError: If we find validation errors.
     """
+    # Transforms the given value to Undefined if it matches the default_parse_string.
+    value = _transform_to_undefined(value)
+
     # Get all attributes that the object has
     attributes = getattr(obj, MetaClass._attr_name) # pylint: disable=protected-access
     try:
         field = attributes[attr]
     except KeyError:
         return value
 
@@ -46,41 +49,100 @@
         field.validate(attr, value)
     else:
         _validate(attr, value, field)
 
     return value
 
 
+def _transform_to_undefined(value: Any) -> Any:
+    """
+    Transforms the given value to Undefined if it matches the default parse string.
+
+    Args:
+        value (Any): The value to transform.
+
+    Returns:
+        Any: The transformed value.
+    """
+    if isinstance(value, str) and value == Undefined.default_parse_string:
+        value = Undefined
+
+    return value
+
+
 def _required(attr_name: str, value: Any) -> None:
     """
     Checks if value is required, required values can't be: None, '', [], {}.
 
     Raises:
         RequiredError: When value is required and match with False conditions.
     """
     if value in (Undefined, None, '', (), [], {}):
         raise RequiredError(f'The {attr_name} attribute is required.')
 
 
-def _validate(attr_name: str, value: Any, attr_type: type) -> None:
+def _validate(attr_name: str, value: Any, attr_type: type) -> None: # pylint: disable=too-many-branches, too-many-return-statements
     """
-    Checks if value is of value_type.
+    Validates that the given value is of the expected attribute type. The function supports special type checks for
+    Date and DateTime types and handles general type validation for other types. It allows the value to pass through
+    if it matches the expected type, is None, or is an instance of Undefined. The function uses custom checks for Date
+    and DateTime to accommodate their unique validation requirements.
+
+    Args:
+        attr_name (str):
+            The name of the attribute being validated. This is used for generating error messages.
+
+        value (Any):
+            The value to be validated against the expected type.
+
+        attr_type (type):
+            The expected type of the value. This can be a standard Python type, a custom type, or
+            specific types like Date and DateTime which have dedicated validation logic.
 
     Raises:
         FieldValueError: When value is not of value_type.
     """
+    # We always accept these 2 values
+    if value is None or value is Undefined:
+        return None
+
+    if attr_type == Date:
+        # If we are expecting a Date we don't need to check other things
+        if Date.is_date(value):
+            return None
+
+    if attr_type == DateTime:
+        # If we are expecting a DateTime we don't need to check other things
+        if DateTime.is_datetime(value):
+            return None
+
+    # TypeError: typing.Any cannot be used with isinstance()
     if attr_type is Any:
         return None
-    elif attr_type is callable:
-        check = callable(value)
-    else:
-        check = value is None or value is Undefined or (attr_type == Date and Date.is_date(value)) or (attr_type == DateTime and DateTime.is_datetime(value)) or isinstance(value, attr_type)
 
-    if check is False:
-        raise FieldValueError(f'Key {attr_name} must be {attr_type}.')
+    # https://everysk.atlassian.net/browse/COD-4286
+    # If we use 'class'/callable as a annotation, the isinstance will fail
+    # because attr_type will be a string/function so we need to discard it first
+    if attr_type is callable:
+        if callable(value):
+            return None
+
+    if isinstance(attr_type, str):
+        if type(value).__name__ == attr_type:
+            return None
+
+    try:
+        # When the second attribute is not a type or a tuple of types
+        # the isinstance will fail with TypeError
+        if isinstance(value, attr_type):
+            return None
+    except TypeError:
+        pass
+
+    raise FieldValueError(f'Key {attr_name} must be {attr_type}.')
 
 
 class BaseField:
     """ Base class of all fields that will guarantee their type. """
     ## Public attributes
     attr_type: type = None
     default: Any = None
@@ -218,14 +280,41 @@
         return getattr(self.attr_type, name)
 
 
 class MetaClass(type):
     _attr_name: str = '__attributes__'
     _anno_name: str = '__annotations__'
 
+    def __call__(cls, *args: tuple, **kwargs: dict) -> Any:
+        """
+        Method that creates a sequence of method calls like:
+            before_init
+            init
+            after_init
+        If the BaseObject class implement one of these methods they will be executed.
+        https://discuss.python.org/t/add-a-post-method-equivalent-to-the-new-method-but-called-after-init/5449/11
+        """
+        ## If the before init method is implemented we run it
+        before_init: callable = getattr(cls, '__before_init__', None)
+        if before_init:
+            # If the method returns a dict we update kwargs
+            dct = before_init(**kwargs) # pylint: disable=not-callable
+            if dct and isinstance(dct, dict):
+                kwargs.update(dct)
+
+        ## Here we create the object
+        obj = super().__call__(*args, **kwargs)
+
+        ## If the after init method is implemented we run it
+        after_init: callable = getattr(obj, '__after_init__', None)
+        if after_init:
+            after_init() # pylint: disable=not-callable
+
+        return obj
+
     def __new__(mcs, name: str, bases: tuple, attrs: dict) -> type:
         """
         This method is executed every time a BaseObject Class is created in the Python runtime.
         We changed this method to create the config and attributes properties and update the annotations.
 
         Example:
 
@@ -351,15 +440,24 @@
             _validate(attr, value, annotations[attr])
         File "/var/app/utils/object.py", line 56, in _validate
             raise DataTypeError(f'Key {attr_name} must be {attr_type}.')
         utils.exceptions.DataTypeError: Key var_int must be <class 'int'>.
     """
     _is_frozen: bool = False # This will control if we can update data on this class
 
-    def __init__(self, **kwargs) -> None:
+    @classmethod
+    def __before_init__(cls, **kwargs: dict) -> dict:
+        """
+        Method that runs before the __init__ method.
+        If needed we must return the kwargs that will be passed to the init
+        otherwise return None to not change the current behavior.
+        """
+        return kwargs
+
+    def __init__(self, **kwargs: dict) -> None:
         # Validate all required fields
         attributes = self.__get_attributes__()
         for attr_name, field in attributes.items():
             if getattr(field, 'required', False):
                 _required(attr_name=attr_name, value=kwargs.get(attr_name))
 
         # Set all kwargs on the object
@@ -368,14 +466,21 @@
 
         # Set the instance to be Frozen
         try:
             self._is_frozen = self.config.frozen
         except AttributeError:
             pass
 
+    def __after_init__(self) -> None:
+        """
+        Method that runs after the __init__ method.
+        This method must return None.
+        """
+        pass
+
     def __check_frozen__(self) -> None:
         """
         Method that checks if this class is a Frozen object and raises attribute error.
         """
         if self._is_frozen:
             raise AttributeError(f'Class {self.get_full_doted_class_path()} is frozen and cannot be modified.')
```

### Comparing `everysk_beta-1.3.656/src/everysk/core/redis.py` & `everysk_beta-1.4.815/src/everysk/core/redis.py`

 * *Files 5% similar despite different names*

```diff
@@ -179,21 +179,36 @@
 class RedisCacheCompressed(RedisCache):
     """
     Store data on Redis server using pickle and zlib
     Use this if you need to store objects ons Redis.
     """
 
     def get(self, key: bytes) -> Any:
+        """
+        Retrieve the value associated with the given key from the Redis cache
+
+        Args:
+            key (bytes): The key to retrieve the value for
+
+        """
         value = super().get(key)
         if value is not None:
             value = decompress_pickle(value)
 
         return value
 
     def set(self, key: bytes, value: Any, timeout: int = None) -> None:
+        """
+        Store the provided value in the Redis cache associated with the given key
+
+        Args:
+            key (bytes): The key to associate with the value
+            value (Any): The value to store in the Redis cache
+            timeout (int, optional): Expiration time for the cached item
+        """
         value = compress_pickle(value)
         super().set(key, value, timeout)
 
 
 class RedisList(RedisClient):
     """
     First in, first out Redis list implementation.
```

### Comparing `everysk_beta-1.3.656/src/everysk/core/slack.py` & `everysk_beta-1.4.815/src/everysk/core/slack.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 #
 # This is an unpublished work containing confidential and proprietary
 # information of EVERYSK TECHNOLOGIES. Disclosure, use, or reproduction
 # without authorization of EVERYSK TECHNOLOGIES is prohibited.
 #
 ###############################################################################
 from requests import Response
-from everysk.core.fields import BoolField, ChoiceField, ReadonlyDictField, StrField
+from everysk.core.fields import BoolField, ChoiceField, DictField, StrField
 from everysk.core.http import HttpPOSTConnection
 
 
 class Slack(HttpPOSTConnection):
     ## Private attributes
-    _color_map = ReadonlyDictField(default={
+    _color_map = DictField(default={
         'danger': '#a90a05',
         'success': '#138138',
         'warning': '#e9932d'
-    })
+    }, readonly=True)
     is_json = BoolField(default=True, readonly=True)
 
     ## Public attributes
     color = ChoiceField(default=None, choices=(None, 'danger', 'success', 'warning'))
     message = StrField(default=None, required=True)
     title = StrField(default=None, required=True)
```

### Comparing `everysk_beta-1.3.656/src/everysk/core/tests.py` & `everysk_beta-1.4.815/src/everysk/core/tests.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,37 +22,42 @@
 ## Compress Test Cases
 from everysk.core._tests.compress import (
     CompressJsonTestCase as EveryskLibCompressJsonTestCase,
     CompressPickleTestCase as EveryskLibCompressPickleTestCase
 )
 
 ## Config Test Cases
-from everysk.core._tests.config import SettingsModulesTestCase as EveryskLibSettingsModulesTestCase, SettingsTestCase as EveryskLibSettingsTestCase
+from everysk.core._tests.config import (
+    SettingsModulesTestCase as EveryskLibSettingsModulesTestCase,
+    SettingsTestCase as EveryskLibSettingsTestCase,
+    SettingsManagerTestCase as EveryskLibSettingsManagerTestCase
+)
 
 ## Date, DateTime Test Cases
 from everysk.core.datetime.tests.date import DateTestCase as EveryskLibDateTestCase
 from everysk.core.datetime.tests.datetime import DateTimeTestCase as EveryskLibDateTimeTestCase
 from everysk.core.datetime.tests.date_mixin import GetHolidaysTestCase as EveryskLibDateMixinGetHolidaysTestCase
 from everysk.core.datetime.tests.calendar import CalendarTestCase as EveryskLibCalendarTestCase
 
 ## Exceptions Test Cases
 from everysk.core._tests.exceptions import (
     BaseExceptionTestCase as EveryskLibBaseExceptionTestCase, DefaultErrorTestCase as EveryskLibDefaultErrorTestCase,
     HttpErrorTestCase as EveryskLibHttpErrorTestCase, FieldValueErrorTestCase as EveryskLibFieldValueErrorTestCase,
-    ReadonlyErrorTestCase as EveryskLibReadonlyErrorTestCase, RequiredErrorTestCase as EveryskLibRequiredErrorTestCase
+    ReadonlyErrorTestCase as EveryskLibReadonlyErrorTestCase, RequiredErrorTestCase as EveryskLibRequiredErrorTestCase,
+    TestAPIError as EveryskLibTestAPIError
 )
 
 ## Fields Test Cases
 from everysk.core._tests.fields import (
     BoolFieldTestCase as EveryskLibBoolFieldTestCase, ChoiceFieldTestCase as EveryskLibChoiceFieldTestCase, DateFieldTestCase as EveryskLibDateFieldTestCase,
     DateTimeFieldTestCase as EveryskLibDateTimeFieldTestCase, DictFieldTestCase as EveryskLibDictFieldTestCase, FieldTestCase as EveryskLibFieldTestCase,
     FieldUndefinedTestCase as EveryskLibFieldUndefinedTestCase, FloatFieldTestCase as EveryskLibFloatFieldTestCase, IntFieldTestCase as EveryskLibIntFieldTestCase,
-    IteratorFieldTestCase as EveryskLibIteratorFieldTestCase, ListFieldTestCase as EveryskLibListFieldTestCase, ReadonlyDictFieldTestCase as EveryskLibReadonlyDictFieldTestCase,
-    ReadonlyListFieldTestCase as EveryskLibReadonlyListFieldTestCase, StrFieldTestCase as EveryskLibStrFieldTestCase, TupleFieldTestCase as EveryskLibTupleFieldTestCase,
-    ObjectInitPropertyTestCase as EveryskLibObjectInitPropertyTestCase, COD3770TestCase as EveryskLibCOD3770TestCase
+    IteratorFieldTestCase as EveryskLibIteratorFieldTestCase, ListFieldTestCase as EveryskLibListFieldTestCase, StrFieldTestCase as EveryskLibStrFieldTestCase,
+    TupleFieldTestCase as EveryskLibTupleFieldTestCase, ObjectInitPropertyTestCase as EveryskLibObjectInitPropertyTestCase, COD3770TestCase as EveryskLibCOD3770TestCase,
+    URLFieldTestCase as EveryskLibURLFieldTestCase, SetFieldTestCase as EveryskLibSetFieldTestCase, EmailFieldTestCase as EveryskLibEmailFieldTestCase
 )
 
 ## Firestore Test Cases
 try:
     from everysk.core._tests.firestore import (
         BaseDocumentCachedConfigTestCase as EveryskLibBaseDocumentCachedConfigTestCase,
         BaseDocumentConfigTestCase as EveryskLibBaseDocumentConfigTestCase,
@@ -66,16 +71,18 @@
     if not error.args[0].startswith("No module named 'google'"):
         raise error
 
 ## Http Test Cases
 try:
     from everysk.core._tests.http import (
         HttpConnectionTestCase as EveryskLibHttpConnectionTestCase,
+        HttpConnectionConfigTestCase as EveryskLibHttpConnectionConfigTestCase,
         HttpGETConnectionTestCase as EveryskLibHttpGETConnectionTestCase,
-        HttpPOSTConnectionTestCase as EveryskLibHttpPOSTConnectionTestCase
+        HttpPOSTConnectionTestCase as EveryskLibHttpPOSTConnectionTestCase,
+        HttpSDKPOSTConnectionTestCase as EveryskLibHttpSDKPOSTConnectionTestCase
     )
 except ModuleNotFoundError as error:
     # This will prevent running these tests if requests is not installed
     if not error.args[0].startswith("No module named 'requests'"):
         raise error
 
 ## Log Test Cases
@@ -90,15 +97,17 @@
 ## Object Test Cases
 from everysk.core._tests.object import (
     BaseDictPropertyTestCase as EveryskLibBaseDictPropertyTestCase, BaseDictTestCase as EveryskLibBaseDictTestCase,
     BaseFieldTestCase as EveryskLibBaseFieldTestCase, BaseObjectTestCase as EveryskLibBaseObjectTestCase,
     ConfigHashTestCase as EveryskLibConfigHashTestCase, FrozenDictTestCase as EveryskLibFrozenDictTestCase,
     FrozenObjectTestCase as EveryskLibFrozenObjectTestCase, MetaClassConfigTestCase as EveryskLibMetaClassConfigTestCase,
     RequiredTestCase as EveryskLibRequiredTestCase, ValidateTestCase as EveryskLibValidateTestCase,
-    MetaClassAttributesTestCase as EveryskLibMetaClassAttributesTestCase
+    MetaClassAttributesTestCase as EveryskLibMetaClassAttributesTestCase,
+    NpArrayTestCase as EveryskLibNpArrayTestCase, AfterInitTestCase as EveryskLibAfterInitTestCase,
+    BeforeInitTestCase as EveryskLibBeforeInitTestCase
 )
 
 ## Number Test Cases
 from everysk.core._tests.number import NumberTestCase as EveryskLibNumberTestCase
 
 ## String Test Cases
 from everysk.core._tests.string import StringTestCase as EveryskLibStringTestCase
@@ -120,14 +129,17 @@
 try:
     from everysk.core._tests.slack import SlackTestCase as EveryskLibSlackTestCase
 except ModuleNotFoundError as error:
     # This will prevent running these tests if requests is not installed
     if not error.args[0].startswith("No module named 'requests'"):
         raise error
 
+## Serialize Test Cases
+from everysk.core._tests.serialize import SerializeTestCase as EveryskLibSerializeTestCase
+
 ## Thread Test Cases
 from everysk.core._tests.threads import ThreadPoolTestCase as EveryskLibThreadPoolTestCase, ThreadTestCase as EveryskLibThreadTestCase
 
 ## Undefined Test Cases
 from everysk.core._tests.undefined import UndefinedTestCase as EveryskLibUndefinedTestCase
 
 ## Utils Test Cases
```

### Comparing `everysk_beta-1.3.656/src/everysk/core/threads.py` & `everysk_beta-1.4.815/src/everysk/core/threads.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,97 +6,83 @@
 # information of EVERYSK TECHNOLOGIES. Disclosure, use, or reproduction
 # without authorization of EVERYSK TECHNOLOGIES is prohibited.
 #
 ###############################################################################
 import traceback
 from concurrent.futures import ThreadPoolExecutor, Future, wait
 from contextvars import Context, copy_context
-from threading import Thread as _Thread, Semaphore
 from typing import Any
 from everysk.core.log import Logger
+from everysk.core.object import BaseObject
 
 
 # Create a Thread log to print all errors
 log = Logger(name='everysk-thread-error-log')
 
 
-class Thread(_Thread):
-    results: list = None
-    semaphore: Semaphore = None
-
-    def __init__(self, target: callable, args: tuple = (), kwargs: dict = None, results: list = None, semaphore: Semaphore = None):
-        """
-        Base class to implement Threads, the main difference for a normal Thread is the use
-        of semaphores and store the results of every call.
-        We need to pass the function that will be executed in the Thread.
-        Semaphore needs to be created before to works.
+class Thread(BaseObject):
+    ## Private attributes
+    _pool: 'ThreadPool' = None
+
+    ## Public attributes
+    args: tuple = None
+    kwargs: dict = None
+    target: callable = None
+
+    def __init__(self, target: callable, args: tuple = (), kwargs: dict = None):
+        """
+        Use to execute the target inside a Thread and do parallel process.
+        This differs from the Python Threads for the capacity to use contextVars
+        and return the result.
+        AnOther ability
 
         Args:
-            target (callable): The function that will be executed in the Thread.
-            args (tuple, optional): The arguments that are needed to this function. Defaults to ().
-            kwargs (dict, optional): The keyword arguments that are needed to this function. Defaults to None.
-            results (list, optional): A list to store the result from the target. Defaults to None.
-            semaphore (Semaphore, optional): The semaphore to control the rate execution. Defaults to None.
+            target (callable): The function that will be executed.
+            args (tuple, optional): The args attributes to be sent to the function. Defaults to ().
+            kwargs (dict, optional): The args attributes to be sent to the function. Defaults to None.
 
-        Example:
+        Usage:
 
             >>> from everysk.core.threads import Thread
-            >>> def sum(a: int, b: int) -> int:
+            >>> def sum(a, b):
             ...     return a + b
-
-            >>> results = []
-            >>> Thread(target=sum, args=(1, 1), results=results).start()
-            >>> Thread(target=sum, args=(2, 2), results=results).start()
-            >>> results
-            [2, 4]
-
+            ...
+            >>> thread = Thread(target=sum, args=(1, 2))
+            >>> thread.start()
+            >>> thread.join()
+            3
+            >>> thread = Thread(target=sum, kwargs={'a': 1, 'b': 2})
+            >>> thread.start()
+            >>> thread.join()
+            3
         """
-        self.results = results
-        self.semaphore = semaphore
         super().__init__(target=target, args=args, kwargs=kwargs)
+        if self.kwargs is None:
+            self.kwargs = {}
 
-    def start(self) -> None:
+        self._pool = ThreadPool(concurrency=1, silent=True)
+
+    def join(self) -> Any | None:
         """
-        Send the execution of the "target" inside a Thread, if semaphore exists this
-        function will be blocked until we have a free slot.
+        Wait for the Thread to finish and returns the result.
         """
-        if self.semaphore is None or self.semaphore.acquire(blocking=True):
-            super().start()
+        self._pool.wait()
+        return self._pool.results[0]
 
-    def run(self) -> None:
+    def run(self) -> Any:
+        """
+        The method used to run the target inside the Thread.
         """
-        Method that really execute the "target".
-        After it finish it's execution we release the semaphore if needed.
-        """
-        try:
-            if self._target is not None:
-                try:
-                    # To avoid infinite running Threads we capture the exception and log it.
-                    result = self._target(*self._args, **self._kwargs)
-
-                    # Then we store the result
-                    if self.results is not None:
-                        self.results.append(result)
-
-                except Exception: # pylint: disable=broad-exception-caught
-                    log.error(
-                        'Thread execution error. target: %s, args: %s, kwargs: %s, traceback: %s',
-                        self._target,
-                        self._args,
-                        self._kwargs,
-                        traceback.format_exc()
-                    )
-
-        finally:
-            # Avoid a refcycle if the thread is running a function with
-            # an argument that has a member that points to the thread.
-            del self._target, self._args, self._kwargs
+        self._pool.add(target=self.target, args=self.args, kwargs=self.kwargs)
 
-        if self.semaphore is not None:
-            self.semaphore.release()
+    def start(self) -> None:
+        """
+        The method used to start the Thread.
+        """
+        self.run()
 
 
 class ThreadPool(ThreadPoolExecutor):
     context: Context = None
     default_error_value: Any = Undefined
     futures: list[Future] = None
     results: list = None
```

### Comparing `everysk_beta-1.3.656/src/everysk/core/undefined.py` & `everysk_beta-1.4.815/src/everysk/core/undefined.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/core/workers.py` & `everysk_beta-1.4.815/src/everysk/core/workers.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # (C) Copyright 2023 EVERYSK TECHNOLOGIES
 #
 # This is an unpublished work containing confidential and proprietary
 # information of EVERYSK TECHNOLOGIES. Disclosure, use, or reproduction
 # without authorization of EVERYSK TECHNOLOGIES is prohibited.
 #
 ###############################################################################
-__all__ = ['TaskGoogle', 'WorkerGoogle']
 import traceback
 from typing import Any
 from uuid import uuid4
 from google.api_core.exceptions import AlreadyExists, DeadlineExceeded, ServiceUnavailable, TooManyRequests
 from google.cloud.tasks_v2 import (
     CloudTasksClient, CreateTaskRequest, HttpMethod, PauseQueueRequest, ResumeQueueRequest, Task, Queue
 )
@@ -97,14 +96,15 @@
     ## Public methods
     def get_headers(self) -> dict:
         """
         Return the headers that must be used to receive the task.
         Remember that body must be always a byte object, then on child
         classes do like de example bellow.
 
+        Usage:
             >>> def get_headers(self) -> dict:
             ...     headers = super().get_headers()
             ...     headers['new_header'] = 'bla bla'
             ...     return headers
         """
         return {'Content-type': 'application/octet-stream'}
```

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/base.py` & `everysk_beta-1.4.815/src/everysk/sdk/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 ###############################################################################
 #   Imports
 ###############################################################################
 from typing import Any
 import inspect
 import requests
 
+from everysk.core.string import import_from_string
 from everysk.core.object import BaseDict
 from everysk.core.exceptions import HttpError, SDKError
 from everysk.core.http import HttpSDKPOSTConnection
 
 ###############################################################################
 #   Base Entity Implementation
 ###############################################################################
@@ -60,19 +61,52 @@
         ret = type(obj)(ret)
 
     elif isinstance(obj, set):
         ret = []
         for item in obj:
             ret.append(_parser_out(item, with_internals))
 
+    elif obj == Undefined:
+        ret = Undefined.default_parse_string
+
     elif hasattr(obj, 'strftime_or_null'):
         ret = obj.__class__.strftime_or_null(obj)
 
     return ret
 
+def _mount_self_obj(self_obj: Any) -> dict | None:
+    """
+    This function mounts the self_obj with there private attributes and
+    returns the dictionary.
+
+    Args:
+        self_obj (Any): The object to be mounted.
+
+    Returns:
+        dict: The parsed object. If the object is not serializable, returns None.
+    """
+    if self_obj is None:
+        return None
+
+    ret = dict(self_obj)
+
+    if hasattr(self_obj, '__dict__'):
+        for key, value in self_obj.__dict__.items():
+            if key.startswith('_') and not inspect.ismethod(value):
+                if inspect.isclass(value):
+                    ret[key] = value.__name__
+                elif isinstance(value, BaseDict):
+                    ret[key] = _mount_self_obj(value)
+                elif isinstance(value, (tuple, set)):
+                    ret[key] = list(value)
+                else:
+                    ret[key] = value
+
+    return ret
+
 class BaseSDK(BaseDict):
     """
     A base class for SDK classes.
 
     This class provides a base implementation for SDK classes.
     """
     # This is a blacklist to not create keys
@@ -109,19 +143,25 @@
 
         # Set default values for keyword arguments if not provided
         kwargs.setdefault('class_name', cls.__name__)
         kwargs.setdefault('method_name', inspect.stack()[1].function)
         kwargs.setdefault('self_obj', None)
         kwargs.setdefault('params', {})
 
+        kwargs['self_obj'] = _mount_self_obj(kwargs['self_obj'])
+
         try:
             response: requests.models.Response = HttpSDKPOSTConnection(**kwargs).get_response()
         except HttpError as error:
             raise SDKError(error.msg) from error
 
+        if response and isinstance(response, dict) and 'error_message' in response and 'error_module' in response:
+            error_module = import_from_string(response['error_module'])
+            raise error_module(response['error_message'])
+
         return response
 
     def to_dict(self, with_internals: bool = True) -> dict: # pylint: disable=unused-argument
         """
         Convert the object to a dictionary.
 
         This method converts the object to a dictionary by recursively parsing its attributes.
```

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/engines/_tests/cryptography.py` & `everysk_beta-1.4.815/src/everysk/sdk/engines/_tests/cryptography.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/_tests/base.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/_tests/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,21 @@
 #   Imports
 ###############################################################################
 from unittest import TestCase, mock
 
 from everysk.core.exceptions import RequiredError
 from everysk.core.datetime.datetime import DateTime, timezone, ZoneInfo
 
+from everysk.sdk.entities.query import Query
 from everysk.sdk.entities.base import BaseEntity
 from everysk.sdk.entities.portfolio.base import Portfolio
 from everysk.sdk.entities.portfolio.securities import Securities
 
+from everysk.sdk.base import _mount_self_obj
+
 ###############################################################################
 #   Base Entity TestCase Implementation
 ###############################################################################
 class TestBaseEntity(TestCase):
 
     def setUp(self):
         self.expected_response = {
@@ -174,67 +177,68 @@
         expected_response = self.expected_response.copy()
         expected_response['page_token'] = 'my_test_page'
         result = Portfolio.query.set_page_token('my_test_page')
         self.assertDictEqual(result, expected_response)
 
     def test_load(self):
         """ Test find method """
-        expected_response = self.expected_response.copy()
+        expected_response = Query(Portfolio)
+        expected_response.update(self.expected_response)
         expected_response['filters'] = [('workspace', '=', 'my_workspace')]
 
         with mock.patch('everysk.sdk.base.HttpSDKPOSTConnection') as mock_http_connection:
             result = Portfolio.query.where('workspace', 'my_workspace').load(offset=5)
 
-        mock_http_connection.assert_any_call(class_name='Query', params={'offset': 5}, method_name='load', self_obj=expected_response)
+        mock_http_connection.assert_any_call(class_name='Query', params={'offset': 5}, method_name='load', self_obj=_mount_self_obj(expected_response))
         mock_http_connection.return_value.get_response.assert_called_once_with()
         self.assertIsInstance(result, Portfolio)
 
     def test_list(self):
         """ Test list method """
-        expected_response = self.expected_response.copy()
+        expected_response = Query(Portfolio)
+        expected_response.update(self.expected_response)
         expected_response['filters'] = [('workspace', '=', 'my_workspace')]
 
         with mock.patch('everysk.sdk.base.HttpSDKPOSTConnection') as mock_http_connection:
             Portfolio.query.where('workspace', 'my_workspace').loads(limit=10, offset=5)
 
-        mock_http_connection.assert_any_call(class_name='Query', params={'limit': 10, 'offset': 5}, method_name='loads', self_obj=expected_response)
+        mock_http_connection.assert_any_call(class_name='Query', params={'limit': 10, 'offset': 5}, method_name='loads', self_obj=_mount_self_obj(expected_response))
         mock_http_connection.return_value.get_response.assert_called_once_with()
 
     def test_page(self):
         """ Test page method """
-        expected_response = self.expected_response.copy()
+        expected_response = Query(Portfolio)
+        expected_response.update(self.expected_response)
         expected_response['filters'] = [('workspace', '=', 'my_workspace')]
 
         with mock.patch('everysk.sdk.base.HttpSDKPOSTConnection') as mock_http_connection:
             Portfolio.query.where('workspace', 'my_workspace').page(page_size=10, page_token='page_token')
 
-        mock_http_connection.assert_any_call(class_name='Query', params={'page_size': 10, 'page_token': 'page_token'}, method_name='page', self_obj=expected_response)
+        mock_http_connection.assert_any_call(class_name='Query', params={'page_size': 10, 'page_token': 'page_token'}, method_name='page', self_obj=_mount_self_obj(expected_response))
         mock_http_connection.return_value.get_response.assert_called_once_with()
 
     def test_pages(self):
         """ Test pages method """
-        expected_response = self.expected_response.copy()
+        expected_response = Query(Portfolio)
+        expected_response.update(self.expected_response)
         expected_response['filters'] = [('workspace', '=', 'my_workspace')]
 
         with mock.patch('everysk.sdk.base.HttpSDKPOSTConnection') as mock_http_connection:
             result = Portfolio.query.where('workspace', 'my_workspace').pages(page_size=10)
             next(result)
 
-        mock_http_connection.assert_any_call(class_name='Query', params={'page_size': 10, 'page_token': Undefined}, method_name='page', self_obj=expected_response)
+        mock_http_connection.assert_any_call(class_name='Query', params={'page_size': 10, 'page_token': Undefined}, method_name='page', self_obj=_mount_self_obj(expected_response))
         mock_http_connection.return_value.get_response.assert_called_once_with()
 
     def test_script_query(self):
         """ Test script_query method """
-        expected_response = self.expected_response.copy()
-        expected_response['filters'] = [('workspace', '=', 'my_workspace')]
-
         with mock.patch('everysk.sdk.base.HttpSDKPOSTConnection') as mock_http_connection:
             Portfolio.script.fetch(user_input='port_12456', variant='select', workspace=None)
 
-        mock_http_connection.assert_any_call(self_obj={}, params={'user_input': 'port_12456', 'variant': 'select', 'workspace': None}, class_name='Script', method_name='fetch')
+        mock_http_connection.assert_any_call(self_obj={'_klass': 'Portfolio'}, params={'user_input': 'port_12456', 'variant': 'select', 'workspace': None}, class_name='Script', method_name='fetch')
         mock_http_connection.return_value.get_response.assert_called_once_with()
 
     def test_retrieve(self):
         with mock.patch('everysk.sdk.base.HttpSDKPOSTConnection') as mock_http_connection:
             mock_http_connection.return_value.get_response.return_value = self.sample_portfolio_data
             result = Portfolio.retrieve(entity_id=self.sample_portfolio_data['id'])
 
@@ -417,32 +421,32 @@
 
     def test_save(self):
         portfolio = Portfolio(**self.sample_portfolio_data)
         with mock.patch('everysk.sdk.base.HttpSDKPOSTConnection') as mock_http_connection:
             mock_http_connection.return_value.get_response.return_value = self.sample_portfolio_data
             result = portfolio.save()
 
-        mock_http_connection.assert_any_call(class_name='Portfolio', params={}, method_name='save', self_obj=self.sample_portfolio_data)
+        mock_http_connection.assert_any_call(class_name='Portfolio', params={}, method_name='save', self_obj=_mount_self_obj(portfolio))
         mock_http_connection.return_value.get_response.assert_called_once_with()
         self.assertEqual(result, self.portfolio)
         self.assertIsInstance(result, Portfolio)
 
     def test_delete(self):
         portfolio = Portfolio(**self.sample_portfolio_data)
         with mock.patch('everysk.sdk.base.HttpSDKPOSTConnection') as mock_http_connection:
             mock_http_connection.return_value.get_response.return_value = self.sample_portfolio_data
             result = portfolio.delete()
 
-        mock_http_connection.assert_any_call(class_name='Portfolio', params={}, method_name='delete', self_obj=self.sample_portfolio_data)
+        mock_http_connection.assert_any_call(class_name='Portfolio', params={}, method_name='delete', self_obj=_mount_self_obj(portfolio))
         mock_http_connection.return_value.get_response.assert_called_once_with()
         self.assertEqual(result, self.portfolio)
         self.assertIsInstance(result, Portfolio)
 
     def test_delete_return_none(self):
         portfolio = Portfolio(**self.sample_portfolio_data)
         with mock.patch('everysk.sdk.base.HttpSDKPOSTConnection') as mock_http_connection:
             mock_http_connection.return_value.get_response.return_value = None
             result = portfolio.delete()
 
-        mock_http_connection.assert_any_call(class_name='Portfolio', params={}, method_name='delete', self_obj=self.sample_portfolio_data)
+        mock_http_connection.assert_any_call(class_name='Portfolio', params={}, method_name='delete', self_obj=_mount_self_obj(portfolio))
         mock_http_connection.return_value.get_response.assert_called_once_with()
         self.assertIsNone(result)
```

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/_tests/base_list.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/_tests/base_list.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/_tests/fields.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/_tests/fields.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/_tests/query.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/_tests/query.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 ###############################################################################
 #   Imports
 ###############################################################################
 from unittest import TestCase, mock
 from unittest.mock import MagicMock
 
 from everysk.core.datetime import DateTime, ZoneInfo
+from everysk.core.exceptions import SDKValueError
 
 from everysk.sdk.entities.query import Query
 from everysk.sdk.entities.portfolio.base import Portfolio
 
 ###############################################################################
 #   Query TestCase Implementation
 ###############################################################################
@@ -96,14 +97,23 @@
         self.assertListEqual(query.filters, [('date', '=', DateTime(2023, 8, 10, 12, tzinfo=ZoneInfo('UTC')))])
 
     def test_where_tags_property(self):
         query = Query(self.mock_klass)
         query.where('tags', ['tag1', 'tag2'])
         self.assertListEqual(query.filters, [('tags', '=', 'tag1'), ('tags', '=', 'tag2')])
 
+        query = Query(self.mock_klass)
+        query.where('tags', 'tag')
+        self.assertListEqual(query.filters, [('tags', '=', 'tag')])
+
+    def test_where_tags_invalid(self):
+        with self.assertRaisesRegex(SDKValueError, 'The tags value must be a string or a list of strings'):
+            query = Query(self.mock_klass)
+            query.where('tags', {'tag1': 'tag2'})
+
     def test_where_name_property(self):
         query = Query(self.mock_klass)
         query.where('name', 'value')
         expected_filters = [('name', '<', 'valuf'), ('name', '>=', 'value')]
         self.assertListEqual(query.filters, expected_filters)
 
     def test_where_name_property_special_case(self):
@@ -187,28 +197,69 @@
     def test_set_limit(self):
         limit_value = 10
         result = self.query.set_limit(limit_value)
 
         self.assertEqual(self.query.limit, limit_value)
         self.assertIs(result, self.query)
 
+        self.assertRaisesRegexp(
+            SDKValueError,
+            'The limit value must be greater than or equal to 0.',
+            self.query.set_limit,
+            -1
+        )
+        self.assertRaisesRegexp(
+            SDKValueError,
+            'The limit value must be an integer.',
+            self.query.set_limit,
+            [1]
+        )
+
     def test_set_offset(self):
         offset_value = 5
         result = self.query.set_offset(offset_value)
 
         self.assertEqual(self.query.offset, offset_value)
         self.assertIs(result, self.query)
 
+        self.assertRaisesRegexp(
+            SDKValueError,
+            'The offset value must be greater than or equal to 0.',
+            self.query.set_offset,
+            -1
+        )
+
+        self.assertRaisesRegexp(
+            SDKValueError,
+            'The offset value must be an integer.',
+            self.query.set_offset,
+            [1]
+        )
+
     def test_set_page_size(self):
         page_size_value = 20
         result = self.query.set_page_size(page_size_value)
 
         self.assertEqual(self.query.page_size, page_size_value)
         self.assertIs(result, self.query)
 
+        self.assertRaisesRegexp(
+            SDKValueError,
+            'The page_size value must be greater than or equal to 0.',
+            self.query.set_page_size,
+            -1
+        )
+
+        self.assertRaisesRegexp(
+            SDKValueError,
+            'The page_size value must be an integer.',
+            self.query.set_page_size,
+            [1]
+        )
+
     def test_set_page_token(self):
         token = 'sample_token'
         result = self.query.set_page_token(token)
 
         self.assertEqual(self.query.page_token, token)
         self.assertIs(result, self.query)
 
@@ -320,7 +371,37 @@
 
             # Assert the generator has exhausted
             with self.assertRaises(StopIteration):
                 next(pages_generator)
 
             # Ensure the mock was called twice
             self.assertEqual(mock_page.call_count, 2)
+
+    def test_fetch_ids(self):
+        with mock.patch('everysk.sdk.base.BaseSDK.get_response') as mock_get_response:
+            mock_get_response.return_value = ['port_druyZmYpHsXbgTbC8IMmS4B2Q']
+            result = self.query.fetch_ids(limit=1, offset=2)
+
+        self.assertListEqual(result, ['port_druyZmYpHsXbgTbC8IMmS4B2Q'])
+        mock_get_response.assert_called_once_with(self_obj=self.query, params={'limit': 1, 'offset': 2})
+
+        with mock.patch('everysk.sdk.base.BaseSDK.get_response') as mock_get_response:
+            mock_get_response.return_value = []
+            result = self.query.fetch_ids()
+
+        self.assertListEqual(result, [])
+        mock_get_response.assert_called_once_with(self_obj=self.query, params={'limit': Undefined, 'offset': Undefined})
+
+    def test_fetch_id(self):
+        with mock.patch('everysk.sdk.base.BaseSDK.get_response') as mock_get_response:
+            mock_get_response.return_value = 'port_druyZmYpHsXbgTbC8IMmS4B2Q'
+            result = self.query.fetch_id(offset=2)
+
+        self.assertEqual(result, 'port_druyZmYpHsXbgTbC8IMmS4B2Q')
+        mock_get_response.assert_called_once_with(self_obj=self.query, params={'offset': 2})
+
+        with mock.patch('everysk.sdk.base.BaseSDK.get_response') as mock_get_response:
+            mock_get_response.return_value = None
+            result = self.query.fetch_id()
+
+        self.assertIsNone(result)
+        mock_get_response.assert_called_once_with(self_obj=self.query, params={'offset': Undefined})
```

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/_tests/script.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/_tests/script.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 ###############################################################################
 from unittest import TestCase, mock
 from unittest.mock import MagicMock
 
 from everysk.sdk.entities.query import Query
 from everysk.sdk.entities.portfolio.base import Portfolio
 
+from everysk.sdk.base import _mount_self_obj
+
 ###############################################################################
 #   Script TestCase Implementation
 ###############################################################################
 class ScriptTestCase(TestCase):
     def setUp(self):
         self.mock_klass = MagicMock()
         self.query = Query(Portfolio)
```

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/_tests/tags.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/_tests/tags.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/base.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,17 @@
     Metaclass for the Script class that allows for the script attribute to be accessed
     directly from the entity class.
 
     Example usage:
         To access the script attribute from the entity class:
         >>> MyClass.script
         Script()
+
+    Notes:
+        This metaclass overrides the __getatrribute__ method to enable direct access
     """
     def __getattribute__(cls, __name: str) -> Any:
         """
         Get the script attribute from the entity class.
         """
         if __name == 'script':
             return Script(cls)
```

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/base_list.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/base_list.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/custom_index/_tests/base.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/custom_index/_tests/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from unittest import TestCase, mock
 
 from everysk.config import settings
 from everysk.core.exceptions import FieldValueError
 from everysk.core.datetime import DateTime
 
 from everysk.sdk.entities.custom_index.base import CustomIndex
+from everysk.sdk.base import _mount_self_obj
 
 ###############################################################################
 #   Custom Index TestCase Implementation
 ###############################################################################
 class CustomIndexTestCase(TestCase):
 
     def setUp(self):
@@ -76,20 +77,20 @@
             self.custom_index.symbol = 'Potato'
         self.assertEqual("The value 'Potato' for field 'symbol' must match with this regex: ^CUSTOM:[A-Z0-9_]*$.", e.exception.msg)
 
     def test_get_id_prefix(self):
         self.assertEqual(CustomIndex.get_id_prefix(), settings.CUSTOM_INDEX_SYMBOL_PREFIX)
 
     def test_validate(self):
-        custom_index: CustomIndex = self.custom_index.copy()
+        custom_index: CustomIndex = self.custom_index
         with mock.patch('everysk.sdk.base.HttpSDKPOSTConnection') as mock_http_connection:
             mock_http_connection.return_value.get_response.return_value = True
             result = custom_index.validate()
 
-        mock_http_connection.assert_called_once_with(class_name='CustomIndex', params={}, method_name='validate', self_obj=custom_index)
+        mock_http_connection.assert_called_once_with(class_name='CustomIndex', params={}, method_name='validate', self_obj=_mount_self_obj(custom_index))
         mock_http_connection.return_value.get_response.assert_called_once_with()
         self.assertTrue(result)
 
     def test_entity_to_query(self):
         custom_index: CustomIndex = self.custom_index.copy()
         query = custom_index._entity_to_query() #pylint: disable=protected-access
         self.assertListEqual(query.filters, [
```

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/custom_index/base.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/custom_index/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,16 @@
     def get_id_prefix() -> str:
         """
         Returns the prefix of the custom index id field value.
 
         Returns:
             str: The prefix of the custom index id field value.
 
-        Example usage:
+        Usage:
+            >>> from everysk.sdk.custom_index.base import CustomIndex
             >>> CustomIndex.get_id_prefix()
             'CUSTOM:'
         """
         return settings.CUSTOM_INDEX_SYMBOL_PREFIX
 
     @classmethod
     def modify_many(cls, entity_id_list: list[str], overwrites: dict | list[dict]) -> list:
```

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/custom_index/settings.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/custom_index/settings.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/datastore/base.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/datastore/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,17 +98,20 @@
     def get_id_prefix() -> str:
         """
         Returns the prefix of the datastore id field value.
 
         Returns:
             str: The prefix of the datastore id field value.
 
-        Example usage:
+        Usage:
             >>> Datastore.get_id_prefix()
             'dats_'
+
+        Notes:
+            The prefix is typically used to distinguish datastore IDs from other types of IDs
         """
         return settings.DATASTORE_ID_PREFIX
 
     def validate_type_data(self) -> bool:
         """
         Validates the 'data' attribute of the Datastore entity to ensure it is not None and contains valid JSON data.
```

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/datastore/settings.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/datastore/settings.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/datastore/tests/base.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/datastore/tests/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 from everysk.core.datetime import DateTime, Date
 
 from everysk.core.exceptions import RequiredError, FieldValueError
 
 from everysk.sdk.entities.datastore.base import Datastore
 
+from everysk.sdk.base import _mount_self_obj
+
 ###############################################################################
 #   Datastore TestCase Implementation
 ###############################################################################
 class DatastoreTestCase(unittest.TestCase):
 
     def setUp(self):
         self.sample_data = {
@@ -47,15 +49,15 @@
 
     def test_validate(self):
         datastore: Datastore = self.datastore.copy()
         with unittest.mock.patch('everysk.sdk.base.HttpSDKPOSTConnection') as mock_http_connection:
             mock_http_connection.return_value.get_response.return_value = True
             result = datastore.validate()
 
-        mock_http_connection.assert_called_once_with(class_name='Datastore', params={}, method_name='validate', self_obj=datastore)
+        mock_http_connection.assert_called_once_with(class_name='Datastore', params={}, method_name='validate', self_obj=_mount_self_obj(datastore))
         mock_http_connection.return_value.get_response.assert_called_once_with()
         self.assertTrue(result)
 
     def test_validate_error(self):
         datastore: Datastore = self.datastore.copy()
         datastore.data = DateTime.now()
         with self.assertRaisesRegex(FieldValueError, "Datastore data is not a valid json"):
@@ -126,24 +128,26 @@
 
     def test_query_load(self):
         with unittest.mock.patch('everysk.sdk.base.HttpSDKPOSTConnection') as mock_http_connection:
             mock_http_connection.return_value.get_response.return_value = self.sample_data
             result = Datastore(link_uid='SampleLinkUID', workspace='SampleWorkspace').load()
 
         mock_http_connection.assert_called_once_with(
-            self_obj={
+            self_obj=_mount_self_obj({
                 'filters': [('workspace', '=', 'SampleWorkspace'), ('link_uid', '=', 'SampleLinkUID')],
                 'order': [],
                 'projection': None,
                 'limit': None,
                 'offset': None,
                 'page_size': None,
                 'page_token': None,
-                'distinct_on': []
-            },
+                'distinct_on': [],
+                '_klass': 'Datastore',
+                '_clean_order': []
+            }),
             params={'offset': None},
             class_name='Query',
             method_name='load'
         )
         mock_http_connection.return_value.get_response.assert_called_once_with()
 
         self.assertEqual(result, self.datastore)
```

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/fields.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/fields.py`

 * *Files 7% similar despite different names*

```diff
@@ -211,14 +211,33 @@
         **kwargs
     ) -> None:
         super().__init__(default, min_date=min_date, max_date=max_date, force_time=force_time, required=required, readonly=readonly, required_lazy=required_lazy, empty_is_none=empty_is_none, **kwargs)
 
     def validate(self, attr_name: str, value: Any, attr_type: type = None) -> None:
         """
         Checks if value is greater than min and lower than max including both values.
+
+        Args:
+            attr_name (str): The name of the attribute being validated.
+            value (Any): The value to validate.
+            attr_type (type): The type of the attribute being validated.
+
+        Raises:
+            FieldValueError: If the value is not within the specified range.
+
+        Usage:
+            >>> from everysk.sdk.entities.fields import EntityDateTimeField
+            >>> from everysk.core.datetime.datetime import DateTime
+            >>> field = EntityDateTimeField(min_date=DateTime(2023-01-01), max_date=DateTime(2023-12-31))
+            >>> try:
+            >>> ... field.validate("test_field", DateTime(2023, 6, 15))
+            >>> ... print("Valid Date")
+            >>> except Exception as e:
+            >>> ... print(f"Validation error: {e}")
+            >>> Valid Date
         """
         min_date = self.min_date if self.min_date is not None else DateTime.market_start()
         max_date = self.max_date if self.max_date is not None else DateTime.now().delta(1, 'D').force_time('LAST_MINUTE')
         _min_max_validate(min_date, max_date, value, attr_name)
         return super().validate(attr_name, value, attr_type)
 
 ###############################################################################
@@ -251,14 +270,30 @@
         super().__init__(default=default, min_size=min_size, max_size=max_size, readonly=readonly, required=required, required_lazy=required_lazy, empty_is_none=empty_is_none, **kwargs)
 
     def clean_value(self, value: Any) -> Any:
         """
         This method ensures that the provided value is in the expected format before assigning it to an attribute.
         If the value is None, it is replaced with an empty TagsList. If it is not already a TagsList instance,
         it is converted into one.
+
+        Args:
+            value (Any): The value to clean, None, A TagsList instance, or any other value.
+
+        Usage:
+            >>> from everysk.sdk.entities.tags import Tags
+            >>> from everysk.sdk.entities.fields import EntityTagsField
+            >>> field = EntityTagsField()
+
+            >>> cleaned_value_none = field.clean_value(None)
+            >>> print(cleaned_value_none)
+            >>> []
+
+            >>> cleaned_non_empty_tags = field.clean_value(Tags(['tag1', 'tag2']))
+            >>> print(cleaned_non_empty_tags)
+            >>> ['tag1', 'tag2']
         """
         value = super().clean_value(value)
         if value is None:
             value = Tags()
         elif not isinstance(value, Tags):
             value = Tags(value)
         return value
```

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/file/_tests/base.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/file/_tests/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
 from everysk.config import settings
 from everysk.core.datetime import DateTime
 from everysk.core.exceptions import RequiredError
 
 from everysk.sdk.entities.file.base import File
 
+from everysk.sdk.base import _mount_self_obj
+
 ###############################################################################
 #   File TestCase Implementation
 ###############################################################################
 class FileTestCase(TestCase):
 
     def setUp(self):
         self.sample_data = {
@@ -48,15 +50,15 @@
 
     def test_validate(self):
         file: File = self.file.copy()
         with mock.patch('everysk.sdk.base.HttpSDKPOSTConnection') as mock_http_connection:
             mock_http_connection.return_value.get_response.return_value = True
             result = file.validate()
 
-        mock_http_connection.assert_called_once_with(class_name='File', params={}, method_name='validate', self_obj=file)
+        mock_http_connection.assert_called_once_with(class_name='File', params={}, method_name='validate', self_obj=_mount_self_obj(file))
         mock_http_connection.return_value.get_response.assert_called_once_with()
         self.assertTrue(result)
 
     def test_entity_to_query(self):
         file: File = self.file.copy()
         query = file._entity_to_query() #pylint: disable=protected-access
         self.assertListEqual(query.filters, [
```

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/file/base.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/file/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         serialized to JSON.
 
         Args:
             self (Self): The entity instance to convert.
             with_internals (bool, optional): Whether to include internal parameters. Defaults to True.
 
         Returns:
-            dict: A dictionary representation of the entity.
+            dict: A dictionary representation of the File entity.
 
         Raises:
             NotImplementedError: This method should be implemented in subclasses.
         """
         dct: dict = super().to_dict(with_internals=with_internals)
         dct['url'] = f"{settings.FILE_URL_PATH}{dct['url']}" if dct['url'] else None
         return dct
```

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/file/settings.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/file/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # without authorization of EVERYSK TECHNOLOGIES is prohibited.
 #
 ###############################################################################
 
 ###############################################################################
 #   Imports
 ###############################################################################
-from everysk.core.fields import StrField, IntField, RegexField
+from everysk.core.fields import StrField, IntField, RegexField, ListField
 
 ###############################################################################
 #   Settings Implementation
 ###############################################################################
 
 FILE_URL_PATH = StrField(default='/file', readonly=True)
 FILE_URL_LENGTH = IntField(default=32, readonly=True)
@@ -24,32 +24,35 @@
 FILE_ID_REGEX = RegexField(default=r'^file_[a-zA-Z0-9]', readonly=True)
 FILE_ID_MAX_SIZE = IntField(default=30, readonly=True)
 FILE_ID_PREFIX = StrField(default='file_', readonly=True)
 
 FILE_DATA_MAX_SIZE_IN_RAW = IntField(default=int(50 * 1024 * 1024), readonly=True)
 FILE_DATA_MAX_SIZE_IN_BASE64 = IntField(default=69905066, readonly=True) # int(FILE_DATA_MAX_SIZE_IN_RAW / 3 * 4) # 13.33MB in BASE64 ~= 10MB in RAW
 
-FILE_CONTENT_TYPES: list = [
-    None,
-    'text/x-comma-separated-values',
-    'image/jpeg',
-    'application/zip',
-    'application/vnd.ms-excel',
-    'image/svg+xml',
-    'application/javascript',
-    'application/msword',
-    'application/vnd.openxmlformats-officedocument.wordprocessingml.document',
-    'image/bmp',
-    'application/octet-stream',
-    'text/xml',
-    'application/x-zip-compressed',
-    'application/pdf',
-    'text/csv',
-    'application/csv',
-    'image/gif',
-    'application/xml',
-    'text/comma-separated-values',
-    'application/json',
-    'image/png',
-    'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet',
-    'text/plain'
-]
+FILE_CONTENT_TYPES = ListField(
+    default=[
+        None,
+        'application/csv',
+        'application/javascript',
+        'application/json',
+        'application/msword',
+        'application/octet-stream',
+        'application/pdf',
+        'application/vnd.ms-excel',
+        'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet',
+        'application/vnd.openxmlformats-officedocument.wordprocessingml.document',
+        'application/x-zip-compressed',
+        'application/xml',
+        'application/zip',
+        'image/bmp',
+        'image/gif',
+        'image/jpeg',
+        'image/png',
+        'image/svg+xml',
+        'text/comma-separated-values',
+        'text/csv',
+        'text/plain',
+        'text/x-comma-separated-values',
+        'text/xml'
+    ],
+    readonly=True
+)
```

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/portfolio/_tests/base.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/portfolio/_tests/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 from everysk.core.datetime import DateTime, Date
 
 from everysk.sdk.entities.portfolio.base import SecuritiesField, Portfolio
 from everysk.sdk.entities.portfolio.securities import Securities
 from everysk.sdk.entities.portfolio.security import Security
 
+from everysk.sdk.base import _mount_self_obj
+
 ###############################################################################
 #   Securities Field TestCase Implementation
 ###############################################################################
 class TestSecuritiesField(TestCase):
 
     def setUp(self):
         self.securities_field = SecuritiesField()
@@ -78,33 +80,33 @@
     def test_validate(self):
         portfolio: Portfolio = self.portfolio.copy()
         portfolio.check_securities = True
         with mock.patch('everysk.sdk.base.HttpSDKPOSTConnection') as mock_http_connection:
             mock_http_connection.return_value.get_response.return_value = True
             result = portfolio.validate()
 
-        mock_http_connection.assert_called_once_with(class_name='Portfolio', params={}, method_name='validate', self_obj=portfolio)
+        mock_http_connection.assert_called_once_with(class_name='Portfolio', params={}, method_name='validate', self_obj=_mount_self_obj(portfolio))
         mock_http_connection.return_value.get_response.assert_called_once_with()
         self.assertTrue(result)
 
     def test_to_dict(self):
         dict_output = self.portfolio.to_dict()
         self.assertIsInstance(dict_output, dict)
         self.assertEqual(dict_output['name'], self.sample_data['name'])
         self.assertEqual(dict_output['date'], Date.strftime_or_null(self.sample_data['date']))
         self.assertEqual(dict_output['created'], self.sample_data['created_on'].timestamp())
 
     def test_check(self):
-        entity_dict = self.sample_data.copy()
+        entity_dict = self.sample_data
         entity_dict['check_securities'] = True
         with mock.patch('everysk.sdk.base.HttpSDKPOSTConnection') as mock_http_connection:
             mock_http_connection.return_value.get_response.return_value = self.sample_data
             result = Portfolio.check(entity_dict=entity_dict)
 
-        mock_http_connection.assert_any_call(class_name='Portfolio', params={}, method_name='validate', self_obj=entity_dict)
+        mock_http_connection.assert_any_call(class_name='Portfolio', params={}, method_name='validate', self_obj=_mount_self_obj(Portfolio(**entity_dict)))
         mock_http_connection.return_value.get_response.assert_called_once_with()
 
         check_port = self.portfolio.copy()
         check_port.check_securities = True
         self.assertEqual(result, check_port)
         self.assertIsInstance(result, Portfolio)
 
@@ -262,24 +264,26 @@
 
     def test_query_load(self):
         with mock.patch('everysk.sdk.base.HttpSDKPOSTConnection') as mock_http_connection:
             mock_http_connection.return_value.get_response.return_value = self.sample_data
             result = Portfolio(link_uid='SampleLinkUID', workspace='SampleWorkspace').load()
 
         mock_http_connection.assert_called_once_with(
-            self_obj={
+            self_obj=_mount_self_obj({
                 'filters': [('workspace', '=', 'SampleWorkspace'), ('link_uid', '=', 'SampleLinkUID')],
                 'order': [],
                 'projection': None,
                 'limit': None,
                 'offset': None,
                 'page_size': None,
                 'page_token': None,
-                'distinct_on': []
-            },
+                'distinct_on': [],
+                '_klass': 'Portfolio',
+                '_clean_order': []
+            }),
             params={'offset': None},
             class_name='Query',
             method_name='load'
         )
         mock_http_connection.return_value.get_response.assert_called_once_with()
 
         self.assertEqual(result, self.portfolio)
```

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/portfolio/_tests/securities.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/portfolio/_tests/securities.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/portfolio/_tests/security.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/portfolio/_tests/security.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/portfolio/base.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/portfolio/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,17 +142,20 @@
     def get_id_prefix() -> str:
         """
         Returns the prefix of the portfolio id field value.
 
         Returns:
             str: The prefix of the portfolio id field value.
 
-        Example usage:
+        Usage:
             >>> Portfolio.get_id_prefix()
             'port_'
+
+        Notes:
+            The prefix is typically used to distinguish portfolio IDs from other types of IDs.
         """
         return settings.PORTFOLIO_ID_PREFIX
 
     def validate(self) -> bool:
         """
         This method validates the entity object and raises an exception if it is not
         valid. The validation is performed by calling the `validate` method of each field
@@ -186,14 +189,36 @@
         Example usage:
             >>> entity = Entity()
             >>> entity.to_csv()
             "name,date,base_currency,nlv,description,tags,securities
             My Portfolio,2021-01-01,USD,1000.0,My Portfolio Description,tag1 tag2,sec1,sec2,sec3"
         """
         def write_row(csv_writer_: Any, line: list[str], length: int) -> None:
+            """
+            Write a row to a CSV file
+
+            Args:
+                csv_writer_ (Any): CSV writer object to use for writing the row
+                line (list[str]): The list of values to write as a row
+                length (int): The desired length of the row
+
+            Returns:
+                None
+
+            Usage:
+                >>> from everysk.sdk.entities.portfolio.base import Portfolio
+                >>> import csv
+                >>> csv_file = open('output'.csv', 'w', newline='')
+                >>> write = csv.writer(csv_file)
+                >>> Portfolio.write_row(writer, ['value1', 'value2'], 5)
+                >>> csv_file.close()
+
+            Notes:
+                This function pads the row with empty strings to ensure the fixed length.
+            """
             out: list[str] = line + ([''] * (length - len(line)))
             out = [to_string(s) if s is not None else None for s in out]
             csv_writer_.writerow(out)
             return None
 
         csv_file: StringIO = six.StringIO()
         csv_writer: Any = csv.writer(csv_file)
```

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/portfolio/securities.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/portfolio/securities.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/portfolio/security.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/portfolio/security.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 ###############################################################################
 #   Imports
 ###############################################################################
 from typing import Callable, Any, Self
 from everysk.config import settings
 
-from everysk.core.fields import StrField, DictField, FloatField, DateField, ReadonlyListField
+from everysk.core.fields import StrField, DictField, FloatField, DateField, ListField
 from everysk.core.object import BaseDict, BaseObject
 
 from everysk.sdk.engines import cryptography
 from everysk.sdk.base import BaseSDK, _parser_out
 
 ###############################################################################
 #   Security Implementation
@@ -147,15 +147,15 @@
             'comparable': None,
             'previous_quantity': None
         }
     """
 
     class Config(BaseObject):
         default_status = StrField(default=settings.SECURITY_STATUS_OK, readonly=True)
-        valid_status = ReadonlyListField(default=[settings.SECURITY_STATUS_OK, settings.SECURITY_STATUS_DELISTED])
+        valid_status = ListField(default=[settings.SECURITY_STATUS_OK, settings.SECURITY_STATUS_DELISTED], readonly=True)
 
     config: Config
     status = StrField()
     id = StrField(required_lazy=True, min_size=1, max_size=settings.SYMBOL_ID_MAX_LEN)
 
     symbol = StrField(required_lazy=True, max_size=settings.SYMBOL_MAX_LENGTH)
     quantity = FloatField(required_lazy=True, min_size=settings.QUANTITY_MIN_VALUE, max_size=settings.QUANTITY_MAX_VALUE)
```

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/portfolio/settings.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/portfolio/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # without authorization of EVERYSK TECHNOLOGIES is prohibited.
 #
 ###############################################################################
 
 ###############################################################################
 #   Imports
 ###############################################################################
-from everysk.core.fields import StrField, IntField, FloatField, RegexField
+from everysk.core.fields import StrField, IntField, FloatField, RegexField, ListField
 
 ###############################################################################
 #   Settings Implementation
 ###############################################################################
 PORTFOLIO_ID_REGEX = RegexField(default=r'^port_[a-zA-Z0-9]', readonly=True)
 PORTFOLIO_ID_PREFIX = StrField(default='port_', readonly=True)
 PORTFOLIO_ID_MAX_SIZE = IntField(default=30, readonly=True) # len(PORTFOLIO_ID_PREFIX) + ENTITY_ID_LENGTH
@@ -45,57 +45,60 @@
 SYMBOL_MAX_LENGTH = IntField(default=100, readonly=True)
 LABEL_MAX_LENGTH = IntField(default=100, readonly=True)
 
 PORTFOLIO_SECURITY_ERROR_TYPE_MAX_LEN = IntField(default=100, readonly=True)
 PORTFOLIO_SECURITY_ERROR_MESSAGE_MAX_LEN = IntField(default=500, readonly=True)
 PORTFOLIO_SECURITY_TYPE_MAX_LEN = IntField(default=100, readonly=True)
 
-PORTFOLIO_PROPERTIES_ORDER: list = [
-    'status',
-    'id',
-    'symbol',
-    'quantity',
-    'instrument_class',
-    'ticker',
-    'label',
-    'name',
-    'isin',
-    'exchange',
-    'currency',
-    'fx_rate',
-    'market_price',
-    'market_value',
-    'instrument_type',
-    'instrument_subtype',
-    'asset_class',
-    'asset_subclass',
-    'error_type',
-    'error_message',
-    'maturity_date',
-    'indexer',
-    'percent_index',
-    'rate',
-    'coupon',
-    'multiplier',
-    'underlying',
-    'series',
-    'option_type',
-    'strike',
-    'issue_price',
-    'issue_date',
-    'issuer',
-    'issuer_type',
-    'cost_price',
-    'unrealized_pl',
-    'unrealized_pl_in_base',
-    'book',
-    'trader',
-    'trade_id',
-    'operation',
-    'accounting',
-    'warranty',
-    'return_date',
-    'settlement',
-    'look_through_reference',
-    'extra_data',
-    'hash'
-]
+PORTFOLIO_PROPERTIES_ORDER = ListField(
+    default=[
+        'status',
+        'id',
+        'symbol',
+        'quantity',
+        'instrument_class',
+        'ticker',
+        'label',
+        'name',
+        'isin',
+        'exchange',
+        'currency',
+        'fx_rate',
+        'market_price',
+        'market_value',
+        'instrument_type',
+        'instrument_subtype',
+        'asset_class',
+        'asset_subclass',
+        'error_type',
+        'error_message',
+        'maturity_date',
+        'indexer',
+        'percent_index',
+        'rate',
+        'coupon',
+        'multiplier',
+        'underlying',
+        'series',
+        'option_type',
+        'strike',
+        'issue_price',
+        'issue_date',
+        'issuer',
+        'issuer_type',
+        'cost_price',
+        'unrealized_pl',
+        'unrealized_pl_in_base',
+        'book',
+        'trader',
+        'trade_id',
+        'operation',
+        'accounting',
+        'warranty',
+        'return_date',
+        'settlement',
+        'look_through_reference',
+        'extra_data',
+        'hash'
+    ],
+    readonly=True
+)
```

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/private_security/_tests/base.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/private_security/_tests/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
 from everysk.config import settings
 from everysk.core.exceptions import FieldValueError
 from everysk.core.datetime import DateTime
 
 from everysk.sdk.entities.private_security.base import PrivateSecurity
 
+from everysk.sdk.base import _mount_self_obj
+
 ###############################################################################
 #   Private Security TestCase Implementation
 ###############################################################################
 class PrivateSecurityTestCase(TestCase):
 
     def setUp(self):
         self.sample_data = {
@@ -115,15 +117,15 @@
 
     def test_validate(self):
         private_security: PrivateSecurity = self.private_security.copy()
         with mock.patch('everysk.sdk.base.HttpSDKPOSTConnection') as mock_http_connection:
             mock_http_connection.return_value.get_response.return_value = True
             result = private_security.validate()
 
-        mock_http_connection.assert_called_once_with(class_name='PrivateSecurity', params={}, method_name='validate', self_obj=private_security)
+        mock_http_connection.assert_called_once_with(class_name='PrivateSecurity', params={}, method_name='validate', self_obj=_mount_self_obj(private_security))
         mock_http_connection.return_value.get_response.assert_called_once_with()
         self.assertTrue(result)
 
     def test_entity_to_query(self):
         private_security: PrivateSecurity = self.private_security.copy()
         query = private_security._entity_to_query() #pylint: disable=protected-access
         self.assertListEqual(query.filters, [
```

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/private_security/base.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/private_security/base.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/private_security/settings.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/private_security/settings.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/query.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #   Imports
 ###############################################################################
 from typing import Any, Self, Generator, TypedDict, Callable
 
 from everysk.core.fields import StrField, IntField, ListField, BoolField
 from everysk.core.datetime import DateTime
 from everysk.core.string import is_string_object, normalize_string_to_search
+from everysk.core.exceptions import SDKValueError
 
 from everysk.sdk.base import BaseSDK
 
 ###############################################################################
 #   Query Page Implementation
 ###############################################################################
 class QueryPage(TypedDict):
@@ -81,18 +82,20 @@
     offset = IntField()
 
     # PAGE / PAGES PARAMETERS
     page_size = IntField()
     page_token = StrField()
 
     def __init__(self, _klass: Callable, filters: list | None = None, order: list | None = None, projection: list | None = None, distinct_on: list | None = None,
-                 limit: int | None = None, offset: int | None = None, page_size: int | None = None, page_token: str | None = None):
+                 limit: int | None = None, offset: int | None = None, page_size: int | None = None, page_token: str | None = None, **kwargs):
 
-        super().__init__(_klass=_klass, _clean_order=None, filters=None, order=None, projection=None, distinct_on=None, limit=None,
-                         offset=None, page_size=None, page_token=None)
+        # Initialize the query with the provided parameters, setting each parameter to None. Each parameter is
+        # associated with a respective function that will assign its value and perform validation.
+        super().__init__(_klass=_klass, filters=None, order=None, projection=None, distinct_on=None, limit=None,
+                         offset=None, page_size=None, page_token=None, **kwargs)
 
         self._klass = _klass
         self._clean_order = set()
 
         order = [] if order is None else order
         self.order = []
         for property_name in order:
@@ -159,15 +162,20 @@
 
         # Validate the operator for certain properties
         if operator != '=' and property_name not in ('date', 'created_on', 'updated_on'):
             raise ValueError(f'Filter by {property_name} operator must be \'=\'')
 
         # Handle special case for 'tags' property
         if property_name == 'tags':
-            self.filters.extend([('tags', '=', tag.lower().strip()) for tag in value])
+            if isinstance(value, list):
+                self.filters.extend([('tags', '=', tag.lower().strip()) for tag in value])
+            elif isinstance(value, str):
+                self.filters.append(('tags', '=', value.lower().strip()))
+            else:
+                raise SDKValueError('The tags value must be a string or a list of strings')
 
             return self
 
         # Handle special case for 'date' property
         if property_name == 'date':
             if is_string_object(value):
                 value = DateTime.fromisoformat(value).replace(hour=12)
@@ -316,14 +324,19 @@
         Returns:
             - Query: The instance of the current object, allowing for method chaining.
 
         Example usage:
             To create a query with a limit condition:
             >>> query = Query(MyEntity).set_limit(10)
         """
+        if not isinstance(limit, int):
+            raise SDKValueError('The limit value must be an integer.')
+        if isinstance(limit, int) and limit < 0:
+            raise SDKValueError('The limit value must be greater than or equal to 0.')
+
         self.limit = limit
         return self
 
     def set_offset(self, offset: int) -> Self:
         """
         Set the starting point from which to retrieve the results in the query.
 
@@ -336,14 +349,19 @@
         Returns:
             - Query: The instance of the current object, allowing for method chaining.
 
         Example usage:
             To create a query with an offset condition:
             >>> query = Query(MyEntity).set_offset(10)
         """
+        if not isinstance(offset, int):
+            raise SDKValueError('The offset value must be an integer.')
+        if isinstance(offset, int) and  offset < 0:
+            raise SDKValueError('The offset value must be greater than or equal to 0.')
+
         self.offset = offset
         return self
 
     def set_page_size(self, page_size: int) -> Self:
         """
         Set the number of results to be returned per page for the query.
 
@@ -356,14 +374,19 @@
         Returns:
             - Query: The instance of the current object, allowing for method chaining.
 
         Example usage:
             To create a query with a page size condition:
             >>> query = Query(MyEntity).set_page_size(10)
         """
+        if not isinstance(page_size, int):
+            raise SDKValueError('The page_size value must be an integer.')
+        if isinstance(page_size, int) and page_size < 0:
+            raise SDKValueError('The page_size value must be greater than or equal to 0.')
+
         self.page_size = page_size
         return self
 
     def set_page_token(self, page_token: str) -> Self:
         """
         Set the token representing a specific page of results in the query.
 
@@ -501,17 +524,49 @@
         This generator function will continue to fetch and yield pages until no more pages are available.
 
         Example usage:
         To create a query with a pages condition:
             >>> for entities in Query(MyEntity).where('property_name', 'value').pages():
             ...     print(entities)
         """
-        next_page_token: Undefined | str = Undefined
+        next_page_token: str = Undefined
 
         while True:
             result: QueryPage = self.page(page_size=page_size, page_token=next_page_token)
             yield result['entities']
 
             if not result['next_page_token']:
                 break
 
             next_page_token = result['next_page_token']
+
+    def fetch_ids(self, limit: int = Undefined, offset: int = Undefined) -> list[str]:
+        """
+        Fetch a list of entity IDs based on the query.
+
+        This method retrieves a list of entity IDs from the data source based on the conditions
+        specified in the query.
+
+        Returns:
+            - List[str]: A list of entity IDs. Returns an empty list if no entities match the query.
+
+        Example usage:
+            To create a query with a fetch_ids condition:
+            >>> entity_ids = Query(MyEntity).where('property_name', 'value').fetch_ids()
+        """
+        return self.get_response(self_obj=self, params={'limit': limit, 'offset': offset})
+
+    def fetch_id(self, offset: int = Undefined) -> str | None:
+        """
+        Load a single entity matching the query and return its id.
+
+        Args:
+            offset (int, optional): The offset of the entity to load. Defaults to DEFAULT_QUERY_OFFSET.
+
+        Returns:
+            str: The id of the entity, or None if no entity is found.
+
+        Example usage:
+            To create a query with a fetch_id condition:
+            >>> entity_id = Query(MyEntity).where('property_name', 'value').fetch_id()
+        """
+        return self.get_response(self_obj=self, params={'offset': offset})
```

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/report/base.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/report/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,17 +124,21 @@
     def get_id_prefix() -> str:
         """
         Returns the prefix of the report id field value.
 
         Returns:
             str: The prefix of the report id field value.
 
-        Example usage:
+        Usage:
+            >>> from everysk.sdk.entities.report.base import Report
             >>> Report.get_id_prefix()
             'repo_'
+
+        Notes:
+            The prefix is typically used to distinguish report IDs from the other types of IDs
         """
         return settings.REPORT_ID_PREFIX
 
     def to_dict(self, with_internals: bool = True) -> dict:
         """
         Convert the entity to a JSON-serializable dictionary.
 
@@ -153,15 +157,15 @@
         """
         dct: dict = super().to_dict(with_internals)
 
         relative_url = None
         absolute_url = None
         if self.url is not None:
             relative_url: str = f'{settings.REPORT_URL_PATH}{self.url}'
-            absolute_url: str = f'{settings.APP_URL}{relative_url}'
+            absolute_url: str = f'{settings.EVERYSK_APP_URL}{relative_url}'
 
         dct['url'] = absolute_url
         dct['absolute_url'] = absolute_url
         dct['relative_url'] = relative_url
 
         dct['authorization'] = dct['authorization'].upper() if dct['authorization'] else None
```

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/report/settings.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/report/settings.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/report/tests/base.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/report/tests/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 import unittest
 from everysk.config import settings
 
 from everysk.core.datetime import DateTime, ZoneInfo
 
 from everysk.sdk.entities.report.base import Report
 
+from everysk.sdk.base import _mount_self_obj
+
 ###############################################################################
 #   Report TestCase Implementation
 ###############################################################################
 class ReportTestCase(unittest.TestCase):
 
     def setUp(self):
         self.sample_data = {
@@ -50,15 +52,15 @@
 
     def test_validate(self):
         report: Report = self.report.copy()
         with unittest.mock.patch('everysk.sdk.base.HttpSDKPOSTConnection') as mock_http_connection:
             mock_http_connection.return_value.get_response.return_value = True
             result = report.validate()
 
-        mock_http_connection.assert_called_once_with(class_name='Report', params={}, method_name='validate', self_obj=report)
+        mock_http_connection.assert_called_once_with(class_name='Report', params={}, method_name='validate', self_obj=_mount_self_obj(report))
         mock_http_connection.return_value.get_response.assert_called_once_with()
         self.assertTrue(result)
 
     def test_to_dict(self):
         dict_output = self.report.to_dict()
         self.assertDictEqual(dict_output, {
             'version': 'v1',
@@ -114,24 +116,26 @@
 
     def test_query_load(self):
         with unittest.mock.patch('everysk.sdk.base.HttpSDKPOSTConnection') as mock_http_connection:
             mock_http_connection.return_value.get_response.return_value = self.sample_data
             result = Report(link_uid='SampleLinkUID', workspace='SampleWorkspace').load()
 
         mock_http_connection.assert_called_once_with(
-            self_obj={
+            self_obj=_mount_self_obj({
                 'filters': [('workspace', '=', 'SampleWorkspace'), ('link_uid', '=', 'SampleLinkUID')],
                 'order': [],
                 'projection': None,
                 'limit': None,
                 'offset': None,
                 'page_size': None,
                 'page_token': None,
-                'distinct_on': []
-            },
+                'distinct_on': [],
+                '_klass': 'Report',
+                '_clean_order': []
+            }),
             params={'offset': None},
             class_name='Query',
             method_name='load'
         )
         mock_http_connection.return_value.get_response.assert_called_once_with()
 
         self.assertEqual(result, self.report)
```

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/script.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/script.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,16 @@
     Example usage:
         To fetch an entity:
         >>> script = Script(klass=MyEntity)
         >>> entity = script.fetch(user_input, variant, workspace)
     """
     _klass: Callable = None
 
-    def __init__(self, klass: Callable) -> None:
-        super().__init__(_klass=klass)
-        self._klass = klass
+    def __init__(self, _klass: Callable) -> None:
+        super().__init__(_klass=_klass)
 
     def fetch(self, user_input: Any, variant: str, workspace: str) -> Any:
         """
         Process a scripted query based on user input, variant, and workspace.
 
         This method provides a way to construct and execute different types of queries
         based on the specified variant. It's designed to handle a variety of scenarios
```

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/settings.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/settings.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/entities/tags.py` & `everysk_beta-1.4.815/src/everysk/sdk/entities/tags.py`

 * *Files identical despite different names*

### Comparing `everysk_beta-1.3.656/src/everysk/sdk/tests.py` & `everysk_beta-1.4.815/src/everysk/sdk/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 ###############################################################################
 # pylint: disable=unused-import
 
 ## Remember to prefix all import with EveryskLib to avoid clash with other tests
 try:
     from everysk.sdk._tests.base import TestBaseSDK as EveryskLibTestBaseSDK
 
+    from everysk.sdk._tests.init import InitTestCase as EveryskLibInitTestCase
+
+
     from everysk.sdk.engines._tests.cryptography import TestCryptography as EveryskLibTestCryptography
 
     from everysk.sdk.entities._tests.base_list import TestEntityList as EveryskLibTestEntityList
 
     from everysk.sdk.entities._tests.script import ScriptTestCase as EveryskLibScriptTestCase
     from everysk.sdk.entities._tests.base import TestBaseEntity as EveryskLibTestBaseEntity
     from everysk.sdk.entities._tests.tags import TagsTestCase as EveryskLibTestTagsList
@@ -40,11 +43,12 @@
     )
 
     from everysk.sdk.entities.custom_index._tests.base import CustomIndexTestCase as EveryskLibCustomIndexTestCase
     from everysk.sdk.entities.datastore.tests.base import DatastoreTestCase as EveryskLibDatastoreTestCase
     from everysk.sdk.entities.private_security._tests.base import PrivateSecurityTestCase as EveryskLibPrivateSecurityTestCase
     from everysk.sdk.entities.file._tests.base import FileTestCase as EveryskLibFileTestCase
     from everysk.sdk.entities.report.tests.base import ReportTestCase as EveryskLibReportTestCase
+    from everysk.sdk.entities.worker_template.tests.base import WorkerTemplateTestCase as EveryskLibWorkerTemplateTestCase
 except ModuleNotFoundError as error:
     # This will prevent running these tests if requests is not installed
     if not error.args[0].startswith("No module named 'requests'"):
         raise error
```

### Comparing `everysk_beta-1.3.656/src/everysk/settings.py` & `everysk_beta-1.4.815/src/everysk/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,12 +18,16 @@
 ## Redis
 REDIS_HOST = StrField(default='0.0.0.0')
 REDIS_PORT = IntField(default=6379)
 
 ## Google Cloud
 EVERYSK_GOOGLE_CLOUD_LOCATION = StrField(default='us-central1')
 EVERYSK_GOOGLE_CLOUD_PROJECT = StrField()
+
 # This enables/disables the Google Cloud Logging Handler
 EVERYSK_GOOGLE_CLOUD_LOGGING_INTEGRATION = BoolField(default=True)
 
 ## Slack URL to send messages
 SLACK_URL = StrField()
+
+## Activate/deactivate HTTP Log for every request/response
+HTTP_LOG_RESPONSE = BoolField(default=False)
```

### Comparing `everysk_beta-1.3.656/src/everysk/utils.py` & `everysk_beta-1.4.815/src/everysk/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,16 +10,30 @@
 from typing import Any, Generator
 
 def bool_convert(value: Any) -> bool:
     """
     Convert any of these to True: 'y', 'yes', 'true', 'on', '1'
     Convert any of these to Fale: 'n', 'no', 'false', 'off', '0'
 
+    Returns:
+        Boolean: indicating if the value is either True or False
+
     Raises:
-        ValueError: Raises if value is none off these presented upper.
+        ValueError: if value is none of these presented above.
+
+    Usage:
+        >>> from everysk.utils import bool_convert
+        >>> bool_convert('y')
+        >>> True
+
+        >>> bool_convert('n')
+        >>> False
+
+        >>> bool_convert('a')
+        >>> ValueError: Invalid truth value 'a'
     """
     value = str(value).lower()
     if value in ('y', 'yes', 'true', 'on', '1'):
         value = True
     elif value in ('n', 'no', 'false', 'off', '0'):
         value = False
     else:
@@ -34,14 +48,23 @@
 
     Args:
         search_key (str): The key that must be found.
         value (Any): The item where the key must be found.
 
     Yields:
         Generator: The generator with all corresponding values found by the key.
+
+    Usage:
+        >>> from everysk.utils import search_key_on_dict
+        >>> data = {
+        >>> ... "name" : "John Doe",
+        >>> ... "age" : 32
+        >>> }
+        >>> search_key_on_dict("name", data)
+        >>> John Doe
     """
     if hasattr(value, 'items'):
         for key, val in value.items():
             if key == search_key:
                 yield val
             if isinstance(val, dict):
                 for result in search_key_on_dict(search_key, val):
```

### Comparing `everysk_beta-1.3.656/src/everysk_beta.egg-info/PKG-INFO` & `everysk_beta-1.4.815/src/everysk_beta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: everysk-beta
-Version: 1.3.656
+Version: 1.4.815
 Summary: Generic lib to share python code on Everysk.
 License: (C) Copyright 2023 EVERYSK TECHNOLOGIES
         
         This is an unpublished work containing confidential and proprietary
         information of EVERYSK TECHNOLOGIES. Disclosure, use, or reproduction
         without authorization of EVERYSK TECHNOLOGIES is prohibited.
```

### Comparing `everysk_beta-1.3.656/src/everysk_beta.egg-info/requires.txt` & `everysk_beta-1.4.815/src/everysk_beta.egg-info/requires.txt`

 * *Files identical despite different names*


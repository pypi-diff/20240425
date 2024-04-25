# Comparing `tmp/flamingo-1.8.tar.gz` & `tmp/flamingo-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flamingo-1.8.tar", last modified: Thu May 12 17:07:16 2022, max compression
+gzip compressed data, was "flamingo-1.9.tar", last modified: Tue Nov 22 09:50:22 2022, max compression
```

## Comparing `flamingo-1.8.tar` & `flamingo-1.9.tar`

### file list

```diff
@@ -1,675 +1,675 @@
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.354283 flamingo-1.8/
--rw-r--r--   0 chris     (1000) chris     (1000)    10759 2019-04-20 10:57:54.000000 flamingo-1.8/LICENCE
--rw-rw-r--   0 chris     (1000) chris     (1000)      109 2019-12-16 13:56:30.000000 flamingo-1.8/MANIFEST.in
--rw-r--r--   0 chris     (1000) chris     (1000)     3353 2022-05-12 17:07:16.354283 flamingo-1.8/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     1437 2020-03-21 08:11:37.000000 flamingo-1.8/README.rst
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.302283 flamingo-1.8/bin/
--rwxrwxr-x   0 chris     (1000) chris     (1000)      513 2019-12-16 13:56:30.000000 flamingo-1.8/bin/_flamingo-args
--rwxrwxr-x   0 chris     (1000) chris     (1000)      336 2019-12-16 13:56:30.000000 flamingo-1.8/bin/_flamingo-build
--rwxrwxr-x   0 chris     (1000) chris     (1000)     3584 2019-12-16 13:56:30.000000 flamingo-1.8/bin/_flamingo-init
--rwxrwxr-x   0 chris     (1000) chris     (1000)     4063 2021-12-06 19:14:04.000000 flamingo-1.8/bin/_flamingo-server
--rwxrwxr-x   0 chris     (1000) chris     (1000)      362 2021-12-06 19:14:04.000000 flamingo-1.8/bin/_flamingo-shell
--rwxrwxr-x   0 chris     (1000) chris     (1000)      643 2020-03-21 08:11:37.000000 flamingo-1.8/bin/flamingo
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.302283 flamingo-1.8/flamingo/
--rw-r--r--   0 chris     (1000) chris     (1000)      490 2022-05-12 17:06:13.000000 flamingo-1.8/flamingo/__init__.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.302283 flamingo-1.8/flamingo/__pycache__/
--rw-r--r--   0 chris     (1000) chris     (1000)      730 2022-04-06 13:30:00.000000 flamingo-1.8/flamingo/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      782 2020-08-14 13:05:39.000000 flamingo-1.8/flamingo/__pycache__/__init__.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      718 2020-03-18 10:00:13.000000 flamingo-1.8/flamingo/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      721 2022-05-12 17:06:35.000000 flamingo-1.8/flamingo/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      826 2019-04-20 10:57:54.000000 flamingo-1.8/flamingo/__pycache__/default_settings.cpython-35.pyc
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.302283 flamingo-1.8/flamingo/core/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2019-04-20 10:57:54.000000 flamingo-1.8/flamingo/core/__init__.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.302283 flamingo-1.8/flamingo/core/__pycache__/
--rw-r--r--   0 chris     (1000) chris     (1000)      160 2022-04-06 13:30:00.000000 flamingo-1.8/flamingo/core/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      150 2020-03-21 08:12:41.000000 flamingo-1.8/flamingo/core/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      154 2020-03-18 10:00:13.000000 flamingo-1.8/flamingo/core/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      158 2022-05-09 07:40:40.000000 flamingo-1.8/flamingo/core/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     8439 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/core/__pycache__/context.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     6876 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/core/__pycache__/context.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     6239 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/core/__pycache__/context.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     8366 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/core/__pycache__/context.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)    12137 2022-04-06 13:30:00.000000 flamingo-1.8/flamingo/core/__pycache__/data_model.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)    13164 2020-08-14 13:05:39.000000 flamingo-1.8/flamingo/core/__pycache__/data_model.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)    11462 2020-03-18 10:00:13.000000 flamingo-1.8/flamingo/core/__pycache__/data_model.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)    12244 2022-05-09 07:40:40.000000 flamingo-1.8/flamingo/core/__pycache__/data_model.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1362 2022-04-06 13:30:00.000000 flamingo-1.8/flamingo/core/__pycache__/errors.cpython-310.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1541 2020-03-21 08:12:41.000000 flamingo-1.8/flamingo/core/__pycache__/errors.cpython-35.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1489 2020-03-18 10:00:13.000000 flamingo-1.8/flamingo/core/__pycache__/errors.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1452 2022-05-09 07:40:40.000000 flamingo-1.8/flamingo/core/__pycache__/errors.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     3953 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/core/__pycache__/parser.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     4156 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/core/__pycache__/parser.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     3865 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/core/__pycache__/parser.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     3935 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/core/__pycache__/parser.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1685 2019-04-20 10:57:54.000000 flamingo-1.8/flamingo/core/__pycache__/settings.cpython-35.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     2808 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/core/__pycache__/types.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     3253 2020-08-14 13:06:01.000000 flamingo-1.8/flamingo/core/__pycache__/types.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     2967 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/core/__pycache__/types.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     2950 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/core/__pycache__/types.cpython-39.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)    10716 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/core/context.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    11258 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/core/data_model.py
--rw-r--r--   0 chris     (1000) chris     (1000)      623 2019-04-20 10:57:54.000000 flamingo-1.8/flamingo/core/errors.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3678 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/core/parser.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.302283 flamingo-1.8/flamingo/core/plugins/
--rw-rw-r--   0 chris     (1000) chris     (1000)      116 2020-03-21 08:11:37.000000 flamingo-1.8/flamingo/core/plugins/__init__.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.306283 flamingo-1.8/flamingo/core/plugins/__pycache__/
--rw-r--r--   0 chris     (1000) chris     (1000)      290 2022-04-06 13:30:00.000000 flamingo-1.8/flamingo/core/plugins/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      292 2020-03-21 08:12:41.000000 flamingo-1.8/flamingo/core/plugins/__pycache__/__init__.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      284 2020-03-18 10:00:13.000000 flamingo-1.8/flamingo/core/plugins/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      288 2022-05-09 07:40:40.000000 flamingo-1.8/flamingo/core/plugins/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1369 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/core/plugins/__pycache__/layers.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1591 2020-03-21 12:25:42.000000 flamingo-1.8/flamingo/core/plugins/__pycache__/layers.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1210 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/core/plugins/__pycache__/layers.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1457 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/core/plugins/__pycache__/layers.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1552 2022-04-06 13:30:00.000000 flamingo-1.8/flamingo/core/plugins/__pycache__/media.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1675 2020-03-21 08:12:41.000000 flamingo-1.8/flamingo/core/plugins/__pycache__/media.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1517 2020-03-18 10:00:13.000000 flamingo-1.8/flamingo/core/plugins/__pycache__/media.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1539 2022-05-09 07:40:40.000000 flamingo-1.8/flamingo/core/plugins/__pycache__/media.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      848 2022-04-06 13:30:00.000000 flamingo-1.8/flamingo/core/plugins/__pycache__/meta_data.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      885 2020-08-14 13:05:39.000000 flamingo-1.8/flamingo/core/plugins/__pycache__/meta_data.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      797 2020-03-18 10:00:13.000000 flamingo-1.8/flamingo/core/plugins/__pycache__/meta_data.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      840 2022-05-09 07:40:40.000000 flamingo-1.8/flamingo/core/plugins/__pycache__/meta_data.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     6861 2022-04-06 13:30:00.000000 flamingo-1.8/flamingo/core/plugins/__pycache__/plugin_manager.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     5244 2020-08-14 13:05:39.000000 flamingo-1.8/flamingo/core/plugins/__pycache__/plugin_manager.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     4106 2020-03-18 10:00:13.000000 flamingo-1.8/flamingo/core/plugins/__pycache__/plugin_manager.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     6853 2022-05-09 07:40:40.000000 flamingo-1.8/flamingo/core/plugins/__pycache__/plugin_manager.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      785 2022-04-06 13:30:00.000000 flamingo-1.8/flamingo/core/plugins/__pycache__/static.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      836 2020-08-14 13:05:39.000000 flamingo-1.8/flamingo/core/plugins/__pycache__/static.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      773 2020-03-18 10:00:13.000000 flamingo-1.8/flamingo/core/plugins/__pycache__/static.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      775 2022-05-09 07:40:40.000000 flamingo-1.8/flamingo/core/plugins/__pycache__/static.cpython-39.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1074 2020-03-27 21:00:49.000000 flamingo-1.8/flamingo/core/plugins/layers.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1891 2020-03-21 08:11:37.000000 flamingo-1.8/flamingo/core/plugins/media.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      932 2020-08-14 13:04:36.000000 flamingo-1.8/flamingo/core/plugins/meta_data.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    10172 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/core/plugins/plugin_manager.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      620 2020-03-22 21:24:47.000000 flamingo-1.8/flamingo/core/plugins/static.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.306283 flamingo-1.8/flamingo/core/settings/
--rw-rw-r--   0 chris     (1000) chris     (1000)       39 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/core/settings/__init__.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.306283 flamingo-1.8/flamingo/core/settings/__pycache__/
--rw-r--r--   0 chris     (1000) chris     (1000)      210 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/core/settings/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      204 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/core/settings/__pycache__/__init__.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      204 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/core/settings/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      208 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/core/settings/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1642 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/core/settings/__pycache__/defaults.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1708 2020-08-14 13:06:01.000000 flamingo-1.8/flamingo/core/settings/__pycache__/defaults.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1600 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/core/settings/__pycache__/defaults.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1640 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/core/settings/__pycache__/defaults.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1691 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/core/settings/__pycache__/settings.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1782 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/core/settings/__pycache__/settings.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1657 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/core/settings/__pycache__/settings.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1675 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/core/settings/__pycache__/settings.cpython-39.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1566 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/core/settings/defaults.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1178 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/core/settings/settings.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.306283 flamingo-1.8/flamingo/core/templating/
--rw-r--r--   0 chris     (1000) chris     (1000)       78 2019-04-20 10:57:54.000000 flamingo-1.8/flamingo/core/templating/__init__.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.306283 flamingo-1.8/flamingo/core/templating/__pycache__/
--rw-r--r--   0 chris     (1000) chris     (1000)      253 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/core/templating/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      251 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/core/templating/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      247 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/core/templating/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      251 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/core/templating/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1202 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/core/templating/__pycache__/base.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1244 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/core/templating/__pycache__/base.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1180 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/core/templating/__pycache__/base.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1210 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/core/templating/__pycache__/base.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     9025 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/core/templating/__pycache__/jinja2.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     8152 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/core/templating/__pycache__/jinja2.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     7413 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/core/templating/__pycache__/jinja2.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     8996 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/core/templating/__pycache__/jinja2.cpython-39.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      781 2020-08-14 13:04:36.000000 flamingo-1.8/flamingo/core/templating/base.py
--rw-r--r--   0 chris     (1000) chris     (1000)    12416 2022-05-12 17:06:13.000000 flamingo-1.8/flamingo/core/templating/jinja2.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2636 2020-08-14 13:04:36.000000 flamingo-1.8/flamingo/core/types.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.306283 flamingo-1.8/flamingo/core/utils/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2019-04-20 10:57:54.000000 flamingo-1.8/flamingo/core/utils/__init__.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.310283 flamingo-1.8/flamingo/core/utils/__pycache__/
--rw-r--r--   0 chris     (1000) chris     (1000)      166 2022-04-06 13:30:00.000000 flamingo-1.8/flamingo/core/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      156 2020-03-21 08:12:41.000000 flamingo-1.8/flamingo/core/utils/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      160 2020-03-18 10:00:13.000000 flamingo-1.8/flamingo/core/utils/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      164 2022-05-09 07:40:40.000000 flamingo-1.8/flamingo/core/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      696 2022-05-09 07:44:34.000000 flamingo-1.8/flamingo/core/utils/__pycache__/aiohttp.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      700 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/core/utils/__pycache__/aiohttp.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      676 2020-03-18 10:14:46.000000 flamingo-1.8/flamingo/core/utils/__pycache__/aiohttp.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      690 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/core/utils/__pycache__/aiohttp.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     2477 2019-04-20 10:57:54.000000 flamingo-1.8/flamingo/core/utils/__pycache__/aionotify.cpython-35.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     4339 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/core/utils/__pycache__/cli.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     4703 2020-03-21 08:12:57.000000 flamingo-1.8/flamingo/core/utils/__pycache__/cli.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     4323 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/core/utils/__pycache__/cli.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     4349 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/core/utils/__pycache__/cli.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1240 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/core/utils/__pycache__/html.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1263 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/core/utils/__pycache__/html.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1181 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/core/utils/__pycache__/html.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1234 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/core/utils/__pycache__/html.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1291 2022-04-06 13:30:00.000000 flamingo-1.8/flamingo/core/utils/__pycache__/imports.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1439 2020-03-21 08:12:41.000000 flamingo-1.8/flamingo/core/utils/__pycache__/imports.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1277 2020-03-18 10:00:13.000000 flamingo-1.8/flamingo/core/utils/__pycache__/imports.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1289 2022-05-09 07:40:40.000000 flamingo-1.8/flamingo/core/utils/__pycache__/imports.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      585 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/core/utils/__pycache__/pagination.cpython-310.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      582 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/core/utils/__pycache__/pagination.cpython-35.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      550 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/core/utils/__pycache__/pagination.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      577 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/core/utils/__pycache__/pagination.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     4129 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/core/utils/__pycache__/pprint.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     4565 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/core/utils/__pycache__/pprint.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     4094 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/core/utils/__pycache__/pprint.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     4149 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/core/utils/__pycache__/pprint.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      930 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/core/utils/__pycache__/string.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1049 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/core/utils/__pycache__/string.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      928 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/core/utils/__pycache__/string.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      926 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/core/utils/__pycache__/string.cpython-39.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      347 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/core/utils/aiohttp.py
--rw-r--r--   0 chris     (1000) chris     (1000)      389 2019-04-20 10:57:54.000000 flamingo-1.8/flamingo/core/utils/chardet.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4878 2020-03-21 08:11:37.000000 flamingo-1.8/flamingo/core/utils/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      883 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/core/utils/html.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1580 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/core/utils/imports.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      660 2020-08-14 13:04:36.000000 flamingo-1.8/flamingo/core/utils/pagination.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5505 2020-03-21 08:11:37.000000 flamingo-1.8/flamingo/core/utils/pprint.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      624 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/core/utils/string.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.310283 flamingo-1.8/flamingo/plugins/
--rw-r--r--   0 chris     (1000) chris     (1000)     1304 2022-05-12 16:46:39.000000 flamingo-1.8/flamingo/plugins/__init__.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.314283 flamingo-1.8/flamingo/plugins/__pycache__/
--rw-r--r--   0 chris     (1000) chris     (1000)     1411 2022-05-12 16:49:28.000000 flamingo-1.8/flamingo/plugins/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1358 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/__pycache__/__init__.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1280 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1409 2022-05-12 16:47:31.000000 flamingo-1.8/flamingo/plugins/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1050 2019-04-20 10:57:54.000000 flamingo-1.8/flamingo/plugins/__pycache__/authors.cpython-35.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1910 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/__pycache__/feeds.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1985 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/__pycache__/feeds.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1837 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/__pycache__/feeds.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1919 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/__pycache__/feeds.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1269 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/__pycache__/git.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1335 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/__pycache__/git.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1234 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/__pycache__/git.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1253 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/__pycache__/git.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1275 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/__pycache__/html.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1333 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/__pycache__/html.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1245 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/__pycache__/html.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1267 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/__pycache__/html.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1701 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/__pycache__/i18n.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1790 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/__pycache__/i18n.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1643 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/__pycache__/i18n.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1686 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/__pycache__/i18n.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1769 2019-04-20 10:57:54.000000 flamingo-1.8/flamingo/plugins/__pycache__/layers.cpython-35.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1418 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/__pycache__/md.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1509 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/__pycache__/md.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1390 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/__pycache__/md.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1412 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/__pycache__/md.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1846 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/__pycache__/redirects.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1937 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/__pycache__/redirects.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1807 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/__pycache__/redirects.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1831 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/__pycache__/redirects.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1731 2019-04-20 10:57:54.000000 flamingo-1.8/flamingo/plugins/__pycache__/tags.cpython-35.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     5820 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/__pycache__/thumbnails.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     6125 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/__pycache__/thumbnails.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     5568 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/__pycache__/thumbnails.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     5806 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/__pycache__/thumbnails.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     3742 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/__pycache__/time.cpython-310.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     3898 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/__pycache__/time.cpython-35.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     3637 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/__pycache__/time.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     3806 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/__pycache__/time.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      891 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/__pycache__/yaml.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      903 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/__pycache__/yaml.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      861 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/__pycache__/yaml.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      881 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/__pycache__/yaml.cpython-39.pyc
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.314283 flamingo-1.8/flamingo/plugins/authors/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/authors/__init__.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.314283 flamingo-1.8/flamingo/plugins/authors/__pycache__/
--rw-r--r--   0 chris     (1000) chris     (1000)      171 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/authors/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      161 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/authors/__pycache__/__init__.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      165 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/authors/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      169 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/authors/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1085 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/authors/__pycache__/authors.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1157 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/authors/__pycache__/authors.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1062 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/authors/__pycache__/authors.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1074 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/authors/__pycache__/authors.cpython-39.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      955 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/authors/authors.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/authors/theme/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.314283 flamingo-1.8/flamingo/plugins/authors/theme/templates/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/authors/theme/templates/author.html
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/authors/theme/templates/authors.html
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.314283 flamingo-1.8/flamingo/plugins/bootstrap/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/__init__.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.314283 flamingo-1.8/flamingo/plugins/bootstrap/__pycache__/
--rw-r--r--   0 chris     (1000) chris     (1000)      173 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/bootstrap/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      163 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/bootstrap/__pycache__/__init__.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      167 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/bootstrap/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      171 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/bootstrap/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      568 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/bootstrap/__pycache__/plugins.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      672 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/bootstrap/__pycache__/plugins.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      630 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/bootstrap/__pycache__/plugins.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      604 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/bootstrap/__pycache__/plugins.cpython-39.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      242 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/plugins.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/bootstrap/theme/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.314283 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/
--rw-rw-r--   0 chris     (1000) chris     (1000)    25682 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap-theme.css
--rw-rw-r--   0 chris     (1000) chris     (1000)    48005 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap-theme.css.map
--rw-rw-r--   0 chris     (1000) chris     (1000)    23411 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap-theme.min.css
--rw-rw-r--   0 chris     (1000) chris     (1000)    75600 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap-theme.min.css.map
--rw-rw-r--   0 chris     (1000) chris     (1000)   145933 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap.css
--rw-rw-r--   0 chris     (1000) chris     (1000)   390887 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap.css.map
--rw-rw-r--   0 chris     (1000) chris     (1000)   121457 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap.min.css
--rw-rw-r--   0 chris     (1000) chris     (1000)   540434 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap.min.css.map
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.314283 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/fonts/
--rw-rw-r--   0 chris     (1000) chris     (1000)    20127 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/fonts/glyphicons-halflings-regular.eot
--rw-rw-r--   0 chris     (1000) chris     (1000)   108738 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/fonts/glyphicons-halflings-regular.svg
--rw-rw-r--   0 chris     (1000) chris     (1000)    45404 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/fonts/glyphicons-halflings-regular.ttf
--rw-rw-r--   0 chris     (1000) chris     (1000)    23424 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/fonts/glyphicons-halflings-regular.woff
--rw-rw-r--   0 chris     (1000) chris     (1000)    18028 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.318283 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/js/
--rw-rw-r--   0 chris     (1000) chris     (1000)    75484 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/js/bootstrap.js
--rw-rw-r--   0 chris     (1000) chris     (1000)    39680 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/js/bootstrap.min.js
--rw-rw-r--   0 chris     (1000) chris     (1000)      484 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/js/npm.js
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.318283 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/
--rw-rw-r--   0 chris     (1000) chris     (1000)    64548 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-grid.css
--rw-rw-r--   0 chris     (1000) chris     (1000)   151749 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-grid.css.map
--rw-rw-r--   0 chris     (1000) chris     (1000)    48488 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-grid.min.css
--rw-rw-r--   0 chris     (1000) chris     (1000)   108539 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-grid.min.css.map
--rw-rw-r--   0 chris     (1000) chris     (1000)     4897 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-reboot.css
--rw-rw-r--   0 chris     (1000) chris     (1000)    76483 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-reboot.css.map
--rw-rw-r--   0 chris     (1000) chris     (1000)     4021 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-reboot.min.css
--rw-rw-r--   0 chris     (1000) chris     (1000)    32461 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-reboot.min.css.map
--rw-rw-r--   0 chris     (1000) chris     (1000)   192348 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap.css
--rw-rw-r--   0 chris     (1000) chris     (1000)   492048 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap.css.map
--rw-rw-r--   0 chris     (1000) chris     (1000)   155758 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap.min.css
--rw-rw-r--   0 chris     (1000) chris     (1000)   625953 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap.min.css.map
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.322283 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/
--rw-rw-r--   0 chris     (1000) chris     (1000)   222911 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.bundle.js
--rw-rw-r--   0 chris     (1000) chris     (1000)   402249 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.bundle.js.map
--rw-rw-r--   0 chris     (1000) chris     (1000)    78635 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.bundle.min.js
--rw-rw-r--   0 chris     (1000) chris     (1000)   311949 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.bundle.min.js.map
--rw-rw-r--   0 chris     (1000) chris     (1000)   131637 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.js
--rw-rw-r--   0 chris     (1000) chris     (1000)   250568 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.js.map
--rw-rw-r--   0 chris     (1000) chris     (1000)    58072 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.min.js
--rw-rw-r--   0 chris     (1000) chris     (1000)   190253 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.min.js.map
--rw-rw-r--   0 chris     (1000) chris     (1000)     3352 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/feeds.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1189 2020-08-14 13:04:36.000000 flamingo-1.8/flamingo/plugins/git.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      948 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/html.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2720 2020-08-14 13:04:36.000000 flamingo-1.8/flamingo/plugins/i18n.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.322283 flamingo-1.8/flamingo/plugins/jquery/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/jquery/__init__.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.322283 flamingo-1.8/flamingo/plugins/jquery/__pycache__/
--rw-r--r--   0 chris     (1000) chris     (1000)      170 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/jquery/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      160 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/jquery/__pycache__/__init__.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      164 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/jquery/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      168 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/jquery/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      676 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/jquery/__pycache__/plugins.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      877 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/jquery/__pycache__/plugins.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      814 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/jquery/__pycache__/plugins.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      752 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/jquery/__pycache__/plugins.cpython-39.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      340 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/jquery/plugins.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/jquery/theme/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/jquery/theme/jquery-1/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/jquery/theme/jquery-1/static/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.322283 flamingo-1.8/flamingo/plugins/jquery/theme/jquery-1/static/jquery/
--rw-rw-r--   0 chris     (1000) chris     (1000)   293430 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/jquery/theme/jquery-1/static/jquery/jquery-1.12.4.js
--rw-rw-r--   0 chris     (1000) chris     (1000)    97163 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/jquery/theme/jquery-1/static/jquery/jquery-1.12.4.min.js
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/jquery/theme/jquery-2/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/jquery/theme/jquery-2/static/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.322283 flamingo-1.8/flamingo/plugins/jquery/theme/jquery-2/static/jquery/
--rw-rw-r--   0 chris     (1000) chris     (1000)   257551 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/jquery/theme/jquery-2/static/jquery/jquery-2.2.4.js
--rw-rw-r--   0 chris     (1000) chris     (1000)    85578 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/jquery/theme/jquery-2/static/jquery/jquery-2.2.4.min.js
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/jquery/theme/jquery-3/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/jquery/theme/jquery-3/static/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.322283 flamingo-1.8/flamingo/plugins/jquery/theme/jquery-3/static/jquery/
--rw-rw-r--   0 chris     (1000) chris     (1000)   280364 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/jquery/theme/jquery-3/static/jquery/jquery-3.4.1.js
--rw-rw-r--   0 chris     (1000) chris     (1000)    88145 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/jquery/theme/jquery-3/static/jquery/jquery-3.4.1.min.js
--rw-rw-r--   0 chris     (1000) chris     (1000)   227022 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/jquery/theme/jquery-3/static/jquery/jquery-3.4.1.slim.js
--rw-rw-r--   0 chris     (1000) chris     (1000)    71037 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/jquery/theme/jquery-3/static/jquery/jquery-3.4.1.slim.min.js
--rw-rw-r--   0 chris     (1000) chris     (1000)     1225 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/md.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.322283 flamingo-1.8/flamingo/plugins/menu/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2020-03-21 08:11:37.000000 flamingo-1.8/flamingo/plugins/menu/__init__.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.322283 flamingo-1.8/flamingo/plugins/menu/__pycache__/
--rw-r--r--   0 chris     (1000) chris     (1000)      168 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/menu/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      158 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/menu/__pycache__/__init__.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      162 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/menu/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      166 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/menu/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     4550 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/menu/__pycache__/menu.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     2646 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/menu/__pycache__/menu.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     2435 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/menu/__pycache__/menu.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     4554 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/menu/__pycache__/menu.cpython-39.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     5587 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/menu/menu.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/menu/theme/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/menu/theme/templates/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.322283 flamingo-1.8/flamingo/plugins/menu/theme/templates/menu/
--rw-rw-r--   0 chris     (1000) chris     (1000)      669 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/menu/theme/templates/menu/bootstrap3.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      875 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/menu/theme/templates/menu/bootstrap4.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      290 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/menu/theme/templates/menu/index.html
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.322283 flamingo-1.8/flamingo/plugins/photoswipe/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/photoswipe/__init__.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.326283 flamingo-1.8/flamingo/plugins/photoswipe/__pycache__/
--rw-r--r--   0 chris     (1000) chris     (1000)      174 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/photoswipe/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      164 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/photoswipe/__pycache__/__init__.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      168 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/photoswipe/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      172 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/photoswipe/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      427 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/photoswipe/__pycache__/plugin.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      434 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/photoswipe/__pycache__/plugin.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      413 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/photoswipe/__pycache__/plugin.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      423 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/photoswipe/__pycache__/plugin.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1334 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/photoswipe/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1328 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/photoswipe/__pycache__/utils.cpython-39.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      114 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/photoswipe/plugin.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/photoswipe/theme/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/photoswipe/theme/static/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.326283 flamingo-1.8/flamingo/plugins/photoswipe/theme/static/photoswipe/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.326283 flamingo-1.8/flamingo/plugins/photoswipe/theme/static/photoswipe/default-skin/
--rw-rw-r--   0 chris     (1000) chris     (1000)    11607 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/photoswipe/theme/static/photoswipe/default-skin/default-skin.css
--rw-rw-r--   0 chris     (1000) chris     (1000)      547 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/photoswipe/theme/static/photoswipe/default-skin/default-skin.png
--rw-rw-r--   0 chris     (1000) chris     (1000)     1554 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/photoswipe/theme/static/photoswipe/default-skin/default-skin.svg
--rw-rw-r--   0 chris     (1000) chris     (1000)      866 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/photoswipe/theme/static/photoswipe/default-skin/preloader.gif
--rw-rw-r--   0 chris     (1000) chris     (1000)     6308 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/photoswipe/theme/static/photoswipe/photoswipe-init.js
--rw-rw-r--   0 chris     (1000) chris     (1000)    21504 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/photoswipe/theme/static/photoswipe/photoswipe-ui-default.js
--rw-rw-r--   0 chris     (1000) chris     (1000)     9878 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/photoswipe/theme/static/photoswipe/photoswipe-ui-default.min.js
--rw-rw-r--   0 chris     (1000) chris     (1000)     4137 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/photoswipe/theme/static/photoswipe/photoswipe.css
--rw-rw-r--   0 chris     (1000) chris     (1000)    94045 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/photoswipe/theme/static/photoswipe/photoswipe.js
--rw-rw-r--   0 chris     (1000) chris     (1000)    31904 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/photoswipe/theme/static/photoswipe/photoswipe.min.js
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/photoswipe/theme/templates/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.326283 flamingo-1.8/flamingo/plugins/photoswipe/theme/templates/photoswipe/
--rw-rw-r--   0 chris     (1000) chris     (1000)     2405 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/photoswipe/theme/templates/photoswipe/gallery.html
--rw-rw-r--   0 chris     (1000) chris     (1000)       69 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/photoswipe/theme/templates/photoswipe/image.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      181 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/photoswipe/theme/templates/photoswipe/photoswipe.css.html
--rw-rw-r--   0 chris     (1000) chris     (1000)     2502 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/photoswipe/theme/templates/photoswipe/photoswipe.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      195 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/photoswipe/theme/templates/photoswipe/photoswipe.js.html
--rw-rw-r--   0 chris     (1000) chris     (1000)     1184 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/photoswipe/utils.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1568 2020-08-14 13:04:36.000000 flamingo-1.8/flamingo/plugins/redirects.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.326283 flamingo-1.8/flamingo/plugins/rst/
--rw-rw-r--   0 chris     (1000) chris     (1000)      208 2020-08-14 13:04:36.000000 flamingo-1.8/flamingo/plugins/rst/__init__.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.326283 flamingo-1.8/flamingo/plugins/rst/__pycache__/
--rw-r--r--   0 chris     (1000) chris     (1000)      417 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      157 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      161 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      415 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     8089 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/base.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     7449 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/base.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     4538 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/bootstrap3.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     5002 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/bootstrap3.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     4642 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/bootstrap3.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     4612 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/bootstrap3.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1465 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/directives.cpython-310.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1465 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/directives.cpython-39.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1327 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/file.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1250 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/file.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     3897 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/image.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     4083 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/image.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     3681 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/image.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     3884 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/image.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     3399 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/include.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     2292 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/include.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     2139 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/include.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     3392 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/include.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     2846 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/link.cpython-310.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     2844 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/link.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     5532 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/parser.cpython-310.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     5514 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/parser.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     3129 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/plugin.cpython-310.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     3111 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/plugin.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     4688 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/pygments.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     2203 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/pygments.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     2022 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/pygments.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     4668 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/pygments.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     3995 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/table.cpython-310.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     3977 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/table.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1683 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1739 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/rst/__pycache__/utils.cpython-39.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     4314 2020-08-14 13:04:36.000000 flamingo-1.8/flamingo/plugins/rst/bootstrap3.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1036 2020-08-14 13:04:36.000000 flamingo-1.8/flamingo/plugins/rst/directives.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5926 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/rst/image.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4629 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/rst/include.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3360 2020-08-14 13:04:36.000000 flamingo-1.8/flamingo/plugins/rst/link.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6380 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/rst/parser.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2577 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/rst/plugin.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4878 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/rst/pygments.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5889 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/rst/table.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1939 2020-08-14 13:04:36.000000 flamingo-1.8/flamingo/plugins/rst/utils.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.326283 flamingo-1.8/flamingo/plugins/rtd/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/__init__.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.330283 flamingo-1.8/flamingo/plugins/rtd/__pycache__/
--rw-r--r--   0 chris     (1000) chris     (1000)      167 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/rtd/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      157 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/rtd/__pycache__/__init__.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      161 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/rtd/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      165 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/rtd/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      887 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/rtd/__pycache__/plugin.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      907 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/rtd/__pycache__/plugin.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      863 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/rtd/__pycache__/plugin.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      883 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/rtd/__pycache__/plugin.cpython-39.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      404 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/plugin.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/rtd/theme/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.330283 flamingo-1.8/flamingo/plugins/rtd/theme/static/
--rw-rw-r--   0 chris     (1000) chris     (1000)    68650 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/elasticlunr.js
--rw-rw-r--   0 chris     (1000) chris     (1000)    18051 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/elasticlunr.min.js
--rw-rw-r--   0 chris     (1000) chris     (1000)      261 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/helper.js
--rw-rw-r--   0 chris     (1000) chris     (1000)    33665 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/mark.js
--rw-rw-r--   0 chris     (1000) chris     (1000)    16917 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/mark.min.js
--rw-rw-r--   0 chris     (1000) chris     (1000)   510145 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/ractive.js
--rw-rw-r--   0 chris     (1000) chris     (1000)  1106790 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/ractive.js.map
--rw-rw-r--   0 chris     (1000) chris     (1000)   226170 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/ractive.min.js
--rw-rw-r--   0 chris     (1000) chris     (1000)   863802 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/ractive.min.js.map
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.334283 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.334283 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/css/
--rw-rw-r--   0 chris     (1000) chris     (1000)   118340 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/css/theme.css
--rw-rw-r--   0 chris     (1000) chris     (1000)     9313 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/doctools.js
--rw-rw-r--   0 chris     (1000) chris     (1000)      307 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/documentation_options.js
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.334283 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.342283 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/
--rw-rw-r--   0 chris     (1000) chris     (1000)   256056 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bold.eot
--rw-rw-r--   0 chris     (1000) chris     (1000)   256056 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bold.eot?
--rw-rw-r--   0 chris     (1000) chris     (1000)   600856 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bold.ttf
--rw-rw-r--   0 chris     (1000) chris     (1000)   309728 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bold.woff
--rw-rw-r--   0 chris     (1000) chris     (1000)   184912 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bold.woff2
--rw-rw-r--   0 chris     (1000) chris     (1000)   266158 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bolditalic.eot
--rw-rw-r--   0 chris     (1000) chris     (1000)   266158 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bolditalic.eot?
--rw-rw-r--   0 chris     (1000) chris     (1000)   622572 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bolditalic.ttf
--rw-rw-r--   0 chris     (1000) chris     (1000)   323344 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bolditalic.woff
--rw-rw-r--   0 chris     (1000) chris     (1000)   193308 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bolditalic.woff2
--rw-rw-r--   0 chris     (1000) chris     (1000)   268604 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-italic.eot
--rw-rw-r--   0 chris     (1000) chris     (1000)   268604 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-italic.eot?
--rw-rw-r--   0 chris     (1000) chris     (1000)   639388 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-italic.ttf
--rw-rw-r--   0 chris     (1000) chris     (1000)   328412 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-italic.woff
--rw-rw-r--   0 chris     (1000) chris     (1000)   195704 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-italic.woff2
--rw-rw-r--   0 chris     (1000) chris     (1000)   253461 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-regular.eot
--rw-rw-r--   0 chris     (1000) chris     (1000)   253461 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-regular.eot?
--rw-rw-r--   0 chris     (1000) chris     (1000)   607720 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-regular.ttf
--rw-rw-r--   0 chris     (1000) chris     (1000)   309192 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-regular.woff
--rw-rw-r--   0 chris     (1000) chris     (1000)   182708 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-regular.woff2
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.342283 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/
--rw-rw-r--   0 chris     (1000) chris     (1000)    79520 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-bold.eot
--rw-rw-r--   0 chris     (1000) chris     (1000)    79520 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-bold.eot?
--rw-rw-r--   0 chris     (1000) chris     (1000)   170616 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-bold.ttf
--rw-rw-r--   0 chris     (1000) chris     (1000)    87624 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-bold.woff
--rw-rw-r--   0 chris     (1000) chris     (1000)    67312 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-bold.woff2
--rw-rw-r--   0 chris     (1000) chris     (1000)    78331 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-regular.eot?
--rw-rw-r--   0 chris     (1000) chris     (1000)   169064 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-regular.ttf
--rw-rw-r--   0 chris     (1000) chris     (1000)    86288 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-regular.woff
--rw-rw-r--   0 chris     (1000) chris     (1000)    66444 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-regular.woff2
--rw-rw-r--   0 chris     (1000) chris     (1000)   165742 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/fontawesome-webfont.eot
--rw-rw-r--   0 chris     (1000) chris     (1000)   444379 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/fontawesome-webfont.svg
--rw-rw-r--   0 chris     (1000) chris     (1000)   165548 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/fontawesome-webfont.ttf
--rw-rw-r--   0 chris     (1000) chris     (1000)    98024 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/fontawesome-webfont.woff
--rw-rw-r--   0 chris     (1000) chris     (1000)    77160 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/fontawesome-webfont.woff2
--rw-rw-r--   0 chris     (1000) chris     (1000)    86659 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/jquery.js
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.342283 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/js/
--rw-rw-r--   0 chris     (1000) chris     (1000)    15414 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/js/modernizr.min.js
--rw-rw-r--   0 chris     (1000) chris     (1000)     4414 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/js/theme.js
--rw-rw-r--   0 chris     (1000) chris     (1000)    10847 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/language_data.js
--rw-rw-r--   0 chris     (1000) chris     (1000)       90 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/minus.png
--rw-rw-r--   0 chris     (1000) chris     (1000)     4395 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/pygments.css
--rw-rw-r--   0 chris     (1000) chris     (1000)      480 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/readthedocs-data.js
--rw-rw-r--   0 chris     (1000) chris     (1000)    15060 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/searchtools.js
--rw-rw-r--   0 chris     (1000) chris     (1000)    12140 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/underscore.js
--rw-rw-r--   0 chris     (1000) chris     (1000)      275 2020-03-21 08:11:37.000000 flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd.css
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/rtd/theme/templates/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.342283 flamingo-1.8/flamingo/plugins/rtd/theme/templates/rtd/
--rw-rw-r--   0 chris     (1000) chris     (1000)      382 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/templates/rtd/mark.html
--rw-rw-r--   0 chris     (1000) chris     (1000)     4955 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/rtd/theme/templates/rtd/page.html
--rw-rw-r--   0 chris     (1000) chris     (1000)     1319 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/rtd/theme/templates/rtd/search.html
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.342283 flamingo-1.8/flamingo/plugins/sphinx_themes/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/__init__.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.342283 flamingo-1.8/flamingo/plugins/sphinx_themes/__pycache__/
--rw-r--r--   0 chris     (1000) chris     (1000)      177 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      175 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1093 2022-05-12 16:49:29.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/__pycache__/defaults.cpython-310.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1091 2022-05-12 16:47:31.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/__pycache__/defaults.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     9780 2022-05-12 16:49:29.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/__pycache__/plugin.cpython-310.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     9667 2022-05-12 17:02:53.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/__pycache__/plugin.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     7296 2022-05-12 16:49:29.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/__pycache__/sphinx_theme.cpython-310.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     7296 2022-05-12 16:47:31.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/__pycache__/sphinx_theme.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      805 2022-05-12 17:06:13.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/defaults.py
--rw-r--r--   0 chris     (1000) chris     (1000)    13861 2022-05-12 17:06:13.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/plugin.py
--rw-r--r--   0 chris     (1000) chris     (1000)     8762 2022-05-12 17:06:13.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/sphinx_theme.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/sphinx_themes/theme/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/sphinx_themes/theme/static/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.346283 flamingo-1.8/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/
--rw-rw-r--   0 chris     (1000) chris     (1000)    68650 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/elasticlunr.js
--rw-rw-r--   0 chris     (1000) chris     (1000)    18051 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/elasticlunr.min.js
--rw-rw-r--   0 chris     (1000) chris     (1000)      261 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/helper.js
--rw-rw-r--   0 chris     (1000) chris     (1000)    89476 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/jquery.js
--rw-rw-r--   0 chris     (1000) chris     (1000)      298 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/main.js
--rw-rw-r--   0 chris     (1000) chris     (1000)    33665 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/mark.js
--rw-rw-r--   0 chris     (1000) chris     (1000)    16917 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/mark.min.js
--rw-rw-r--   0 chris     (1000) chris     (1000)   510145 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/ractive.js
--rw-rw-r--   0 chris     (1000) chris     (1000)  1106790 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/ractive.js.map
--rw-rw-r--   0 chris     (1000) chris     (1000)   226170 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/ractive.min.js
--rw-rw-r--   0 chris     (1000) chris     (1000)   863802 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/ractive.min.js.map
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/sphinx_themes/theme/templates/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.346283 flamingo-1.8/flamingo/plugins/sphinx_themes/theme/templates/sphinx_themes/
--rw-rw-r--   0 chris     (1000) chris     (1000)       64 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/theme/templates/sphinx_themes/body.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      901 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/theme/templates/sphinx_themes/search.js
--rw-rw-r--   0 chris     (1000) chris     (1000)      415 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/theme/templates/sphinx_themes/search_variables.js
--rw-rw-r--   0 chris     (1000) chris     (1000)     2043 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/sphinx_themes/theme/templates/sphinx_themes/toctree.html
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.346283 flamingo-1.8/flamingo/plugins/tags/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/tags/__init__.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.346283 flamingo-1.8/flamingo/plugins/tags/__pycache__/
--rw-r--r--   0 chris     (1000) chris     (1000)      168 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/tags/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      158 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/tags/__pycache__/__init__.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      162 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/tags/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      166 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/tags/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1712 2022-04-06 13:30:15.000000 flamingo-1.8/flamingo/plugins/tags/__pycache__/tags.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1835 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/plugins/tags/__pycache__/tags.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1648 2020-03-18 10:08:20.000000 flamingo-1.8/flamingo/plugins/tags/__pycache__/tags.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1697 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/plugins/tags/__pycache__/tags.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     2318 2022-04-06 13:20:24.000000 flamingo-1.8/flamingo/plugins/tags/tags.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/plugins/tags/theme/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.346283 flamingo-1.8/flamingo/plugins/tags/theme/templates/
--rw-rw-r--   0 chris     (1000) chris     (1000)       93 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/tags/theme/templates/tag.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      310 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/tags/theme/templates/tags.html
--rw-rw-r--   0 chris     (1000) chris     (1000)     9260 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/thumbnails.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3534 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/plugins/time.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      951 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/plugins/yaml.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.346283 flamingo-1.8/flamingo/project_templates/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.350283 flamingo-1.8/flamingo/project_templates/bootstrap4/
--rw-rw-r--   0 chris     (1000) chris     (1000)      659 2020-03-21 08:11:37.000000 flamingo-1.8/flamingo/project_templates/bootstrap4/Makefile.template
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/project_templates/bootstrap4/README.rst
--rw-rw-r--   0 chris     (1000) chris     (1000)      173 2020-03-21 08:11:37.000000 flamingo-1.8/flamingo/project_templates/bootstrap4/REQUIREMENTS.txt.template
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.350283 flamingo-1.8/flamingo/project_templates/bootstrap4/content/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.350283 flamingo-1.8/flamingo/project_templates/bootstrap4/content/category-1/
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/project_templates/bootstrap4/content/category-1/page-1.rst
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/project_templates/bootstrap4/content/category-1/page-2.rst
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.350283 flamingo-1.8/flamingo/project_templates/bootstrap4/content/category-2/
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/project_templates/bootstrap4/content/category-2/page-3.rst
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/project_templates/bootstrap4/content/category-2/page-4.rst
--rw-rw-r--   0 chris     (1000) chris     (1000)       54 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/project_templates/bootstrap4/content/home.rst
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.350283 flamingo-1.8/flamingo/project_templates/bootstrap4/overlay/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1150 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/project_templates/bootstrap4/overlay/favicon.ico
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.350283 flamingo-1.8/flamingo/project_templates/bootstrap4/plugins/
--rw-rw-r--   0 chris     (1000) chris     (1000)      423 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/project_templates/bootstrap4/plugins/example.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      586 2020-03-21 08:11:37.000000 flamingo-1.8/flamingo/project_templates/bootstrap4/settings.py.template
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/project_templates/bootstrap4/theme/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.350283 flamingo-1.8/flamingo/project_templates/bootstrap4/theme/static/
--rw-rw-r--   0 chris     (1000) chris     (1000)      320 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/project_templates/bootstrap4/theme/static/custom.css
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.350283 flamingo-1.8/flamingo/project_templates/bootstrap4/theme/templates/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1476 2020-03-21 08:11:37.000000 flamingo-1.8/flamingo/project_templates/bootstrap4/theme/templates/base.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      290 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/project_templates/bootstrap4/theme/templates/page.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      684 2020-03-21 08:11:37.000000 flamingo-1.8/flamingo/project_templates/data.ini
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.350283 flamingo-1.8/flamingo/project_templates/readthedocs/
--rw-rw-r--   0 chris     (1000) chris     (1000)      659 2020-03-21 08:11:37.000000 flamingo-1.8/flamingo/project_templates/readthedocs/Makefile.template
--rw-rw-r--   0 chris     (1000) chris     (1000)      191 2020-03-21 08:11:37.000000 flamingo-1.8/flamingo/project_templates/readthedocs/REQUIREMENTS.txt.template
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.350283 flamingo-1.8/flamingo/project_templates/readthedocs/content/
--rw-rw-r--   0 chris     (1000) chris     (1000)       14 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/project_templates/readthedocs/content/index.rst
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.350283 flamingo-1.8/flamingo/project_templates/readthedocs/overlay/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1150 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/project_templates/readthedocs/overlay/favicon.ico
--rw-rw-r--   0 chris     (1000) chris     (1000)      376 2020-03-21 08:11:37.000000 flamingo-1.8/flamingo/project_templates/readthedocs/settings.py.template
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/project_templates/readthedocs/theme/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.350283 flamingo-1.8/flamingo/project_templates/readthedocs/theme/static/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/project_templates/readthedocs/theme/static/custom.css
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.350283 flamingo-1.8/flamingo/project_templates/readthedocs/theme/templates/
--rw-rw-r--   0 chris     (1000) chris     (1000)      138 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/project_templates/readthedocs/theme/templates/page.html
--rw-r--r--   0 chris     (1000) chris     (1000)     5564 2022-05-12 17:06:13.000000 flamingo-1.8/flamingo/pytest.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.350283 flamingo-1.8/flamingo/server/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2020-03-21 08:11:37.000000 flamingo-1.8/flamingo/server/__init__.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.350283 flamingo-1.8/flamingo/server/__pycache__/
--rw-r--r--   0 chris     (1000) chris     (1000)      162 2022-05-09 07:44:34.000000 flamingo-1.8/flamingo/server/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      152 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/server/__pycache__/__init__.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)      156 2020-03-18 10:14:46.000000 flamingo-1.8/flamingo/server/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)      160 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/server/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     3687 2022-05-09 07:44:34.000000 flamingo-1.8/flamingo/server/__pycache__/build_environment.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     3285 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/server/__pycache__/build_environment.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     2950 2020-03-18 10:14:46.000000 flamingo-1.8/flamingo/server/__pycache__/build_environment.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     3663 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/server/__pycache__/build_environment.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     8510 2022-05-09 07:44:34.000000 flamingo-1.8/flamingo/server/__pycache__/exporter.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     5321 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/server/__pycache__/exporter.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     4877 2020-03-18 10:14:46.000000 flamingo-1.8/flamingo/server/__pycache__/exporter.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     8502 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/server/__pycache__/exporter.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1777 2022-05-09 07:44:34.000000 flamingo-1.8/flamingo/server/__pycache__/frontend_controller.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1981 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/server/__pycache__/frontend_controller.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     1869 2020-03-18 10:14:46.000000 flamingo-1.8/flamingo/server/__pycache__/frontend_controller.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     1821 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/server/__pycache__/frontend_controller.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     3824 2022-05-09 07:44:34.000000 flamingo-1.8/flamingo/server/__pycache__/logging.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     3903 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/server/__pycache__/logging.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     3574 2020-03-18 10:14:46.000000 flamingo-1.8/flamingo/server/__pycache__/logging.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     3826 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/server/__pycache__/logging.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     5251 2022-05-09 07:44:34.000000 flamingo-1.8/flamingo/server/__pycache__/rpc.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     2850 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/server/__pycache__/rpc.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     2657 2020-03-18 10:14:46.000000 flamingo-1.8/flamingo/server/__pycache__/rpc.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     5229 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/server/__pycache__/rpc.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)    12294 2022-05-09 07:44:34.000000 flamingo-1.8/flamingo/server/__pycache__/server.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)    11314 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/server/__pycache__/server.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)    10187 2020-03-18 10:14:46.000000 flamingo-1.8/flamingo/server/__pycache__/server.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)    12262 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/server/__pycache__/server.cpython-39.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     4472 2022-05-09 07:44:34.000000 flamingo-1.8/flamingo/server/__pycache__/watcher.cpython-310.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     4925 2020-03-21 08:12:58.000000 flamingo-1.8/flamingo/server/__pycache__/watcher.cpython-35.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     4429 2020-03-18 10:14:46.000000 flamingo-1.8/flamingo/server/__pycache__/watcher.cpython-37.pyc
--rw-r--r--   0 chris     (1000) chris     (1000)     4454 2022-05-09 07:40:47.000000 flamingo-1.8/flamingo/server/__pycache__/watcher.cpython-39.pyc
--rw-rw-r--   0 chris     (1000) chris     (1000)     5079 2020-08-14 13:04:36.000000 flamingo-1.8/flamingo/server/build_environment.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    10160 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/server/exporter.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1222 2020-03-21 08:11:37.000000 flamingo-1.8/flamingo/server/frontend_controller.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5600 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/server/logging.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6730 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/server/rpc.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    17399 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/server/server.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.350283 flamingo-1.8/flamingo/server/static/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.354283 flamingo-1.8/flamingo/server/static/lib/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1642 2020-03-21 08:11:37.000000 flamingo-1.8/flamingo/server/static/lib/js.cookie-2.2.1.min.js
--rw-rw-r--   0 chris     (1000) chris     (1000)   508398 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/server/static/lib/ractive.js
--rw-rw-r--   0 chris     (1000) chris     (1000)  1101495 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/server/static/lib/ractive.js.map
--rw-rw-r--   0 chris     (1000) chris     (1000)   225749 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/server/static/lib/ractive.min.js
--rw-rw-r--   0 chris     (1000) chris     (1000)   859629 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/server/static/lib/ractive.min.js.map
--rw-rw-r--   0 chris     (1000) chris     (1000)     4296 2020-03-21 08:11:37.000000 flamingo-1.8/flamingo/server/static/lib/rpc.js
--rw-rw-r--   0 chris     (1000) chris     (1000)      375 2020-03-21 08:11:37.000000 flamingo-1.8/flamingo/server/static/loading.svg
--rw-rw-r--   0 chris     (1000) chris     (1000)    13557 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/server/static/main.js
--rw-rw-r--   0 chris     (1000) chris     (1000)     7808 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/server/static/style.css
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.354283 flamingo-1.8/flamingo/server/templates/
--rw-rw-r--   0 chris     (1000) chris     (1000)      271 2020-08-14 13:04:36.000000 flamingo-1.8/flamingo/server/templates/404.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      277 2020-08-14 13:04:36.000000 flamingo-1.8/flamingo/server/templates/500.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      992 2020-08-14 13:04:36.000000 flamingo-1.8/flamingo/server/templates/directory_list.html
--rw-rw-r--   0 chris     (1000) chris     (1000)     8995 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/server/templates/index.html
--rw-rw-r--   0 chris     (1000) chris     (1000)     2107 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/server/templates/plugin_options.html
--rw-rw-r--   0 chris     (1000) chris     (1000)     6201 2020-03-21 08:11:37.000000 flamingo-1.8/flamingo/server/watcher.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.298283 flamingo-1.8/flamingo/theme/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.354283 flamingo-1.8/flamingo/theme/templates/
--rw-rw-r--   0 chris     (1000) chris     (1000)      273 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/theme/templates/base.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      350 2020-03-21 08:11:37.000000 flamingo-1.8/flamingo/theme/templates/code-block.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      119 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/theme/templates/gallery.html
--rw-rw-r--   0 chris     (1000) chris     (1000)     1736 2020-03-21 08:11:37.000000 flamingo-1.8/flamingo/theme/templates/image.html
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.354283 flamingo-1.8/flamingo/theme/templates/jinja2/
--rw-rw-r--   0 chris     (1000) chris     (1000)     6278 2020-08-14 13:04:36.000000 flamingo-1.8/flamingo/theme/templates/jinja2/error.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      130 2019-12-16 13:56:30.000000 flamingo-1.8/flamingo/theme/templates/page.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      401 2021-12-06 19:14:04.000000 flamingo-1.8/flamingo/theme/templates/table.html
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-05-12 17:07:16.302283 flamingo-1.8/flamingo.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)     3353 2022-05-12 17:07:16.000000 flamingo-1.8/flamingo.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)    31107 2022-05-12 17:07:16.000000 flamingo-1.8/flamingo.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        1 2022-05-12 17:07:16.000000 flamingo-1.8/flamingo.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       39 2022-05-12 17:07:16.000000 flamingo-1.8/flamingo.egg-info/entry_points.txt
--rw-r--r--   0 chris     (1000) chris     (1000)      437 2022-05-12 17:07:16.000000 flamingo-1.8/flamingo.egg-info/requires.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        9 2022-05-12 17:07:16.000000 flamingo-1.8/flamingo.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)     1006 2022-05-12 17:07:16.354283 flamingo-1.8/setup.cfg
--rwxr-xr-x   0 chris     (1000) chris     (1000)     1571 2022-05-12 17:06:13.000000 flamingo-1.8/setup.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.541410 flamingo-1.9/
+-rw-r--r--   0 chris     (1000) chris     (1000)    10759 2019-04-20 10:57:54.000000 flamingo-1.9/LICENCE
+-rw-rw-r--   0 chris     (1000) chris     (1000)      109 2019-12-16 13:56:30.000000 flamingo-1.9/MANIFEST.in
+-rw-r--r--   0 chris     (1000) chris     (1000)     3353 2022-11-22 09:50:22.541410 flamingo-1.9/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1437 2020-03-21 08:11:37.000000 flamingo-1.9/README.rst
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/bin/
+-rwxrwxr-x   0 chris     (1000) chris     (1000)      513 2019-12-16 13:56:30.000000 flamingo-1.9/bin/_flamingo-args
+-rwxrwxr-x   0 chris     (1000) chris     (1000)      336 2019-12-16 13:56:30.000000 flamingo-1.9/bin/_flamingo-build
+-rwxrwxr-x   0 chris     (1000) chris     (1000)     3584 2019-12-16 13:56:30.000000 flamingo-1.9/bin/_flamingo-init
+-rwxrwxr-x   0 chris     (1000) chris     (1000)     4063 2021-12-06 19:14:04.000000 flamingo-1.9/bin/_flamingo-server
+-rwxrwxr-x   0 chris     (1000) chris     (1000)      362 2021-12-06 19:14:04.000000 flamingo-1.9/bin/_flamingo-shell
+-rwxrwxr-x   0 chris     (1000) chris     (1000)      643 2020-03-21 08:11:37.000000 flamingo-1.9/bin/flamingo
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.493409 flamingo-1.9/flamingo/
+-rw-r--r--   0 chris     (1000) chris     (1000)      490 2022-11-22 09:47:37.000000 flamingo-1.9/flamingo/__init__.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.493409 flamingo-1.9/flamingo/__pycache__/
+-rw-r--r--   0 chris     (1000) chris     (1000)      725 2022-11-06 21:06:23.000000 flamingo-1.9/flamingo/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      782 2020-08-14 13:05:39.000000 flamingo-1.9/flamingo/__pycache__/__init__.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      718 2020-03-18 10:00:13.000000 flamingo-1.9/flamingo/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      721 2022-11-22 09:49:46.000000 flamingo-1.9/flamingo/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      826 2019-04-20 10:57:54.000000 flamingo-1.9/flamingo/__pycache__/default_settings.cpython-35.pyc
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.493409 flamingo-1.9/flamingo/core/
+-rw-r--r--   0 chris     (1000) chris     (1000)        0 2019-04-20 10:57:54.000000 flamingo-1.9/flamingo/core/__init__.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.493409 flamingo-1.9/flamingo/core/__pycache__/
+-rw-r--r--   0 chris     (1000) chris     (1000)      160 2022-04-06 13:30:00.000000 flamingo-1.9/flamingo/core/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      150 2020-03-21 08:12:41.000000 flamingo-1.9/flamingo/core/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      154 2020-03-18 10:00:13.000000 flamingo-1.9/flamingo/core/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      158 2022-05-09 07:40:40.000000 flamingo-1.9/flamingo/core/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     8439 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/core/__pycache__/context.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6876 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/core/__pycache__/context.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6239 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/core/__pycache__/context.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     8366 2022-11-22 09:49:46.000000 flamingo-1.9/flamingo/core/__pycache__/context.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)    12137 2022-04-06 13:30:00.000000 flamingo-1.9/flamingo/core/__pycache__/data_model.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)    13164 2020-08-14 13:05:39.000000 flamingo-1.9/flamingo/core/__pycache__/data_model.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)    11462 2020-03-18 10:00:13.000000 flamingo-1.9/flamingo/core/__pycache__/data_model.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)    12244 2022-05-09 07:40:40.000000 flamingo-1.9/flamingo/core/__pycache__/data_model.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1362 2022-04-06 13:30:00.000000 flamingo-1.9/flamingo/core/__pycache__/errors.cpython-310.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1541 2020-03-21 08:12:41.000000 flamingo-1.9/flamingo/core/__pycache__/errors.cpython-35.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1489 2020-03-18 10:00:13.000000 flamingo-1.9/flamingo/core/__pycache__/errors.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1452 2022-05-09 07:40:40.000000 flamingo-1.9/flamingo/core/__pycache__/errors.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     3953 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/core/__pycache__/parser.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4156 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/core/__pycache__/parser.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3865 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/core/__pycache__/parser.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     3935 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/core/__pycache__/parser.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1685 2019-04-20 10:57:54.000000 flamingo-1.9/flamingo/core/__pycache__/settings.cpython-35.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     2808 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/core/__pycache__/types.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3253 2020-08-14 13:06:01.000000 flamingo-1.9/flamingo/core/__pycache__/types.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2967 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/core/__pycache__/types.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     2950 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/core/__pycache__/types.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)    10718 2022-11-22 09:41:39.000000 flamingo-1.9/flamingo/core/context.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    11258 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/core/data_model.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      623 2019-04-20 10:57:54.000000 flamingo-1.9/flamingo/core/errors.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3678 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/core/parser.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.493409 flamingo-1.9/flamingo/core/plugins/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      116 2020-03-21 08:11:37.000000 flamingo-1.9/flamingo/core/plugins/__init__.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.497409 flamingo-1.9/flamingo/core/plugins/__pycache__/
+-rw-r--r--   0 chris     (1000) chris     (1000)      290 2022-04-06 13:30:00.000000 flamingo-1.9/flamingo/core/plugins/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      292 2020-03-21 08:12:41.000000 flamingo-1.9/flamingo/core/plugins/__pycache__/__init__.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      284 2020-03-18 10:00:13.000000 flamingo-1.9/flamingo/core/plugins/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      288 2022-05-09 07:40:40.000000 flamingo-1.9/flamingo/core/plugins/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1369 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/core/plugins/__pycache__/layers.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1591 2020-03-21 12:25:42.000000 flamingo-1.9/flamingo/core/plugins/__pycache__/layers.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1210 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/core/plugins/__pycache__/layers.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1457 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/core/plugins/__pycache__/layers.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1552 2022-04-06 13:30:00.000000 flamingo-1.9/flamingo/core/plugins/__pycache__/media.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1675 2020-03-21 08:12:41.000000 flamingo-1.9/flamingo/core/plugins/__pycache__/media.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1517 2020-03-18 10:00:13.000000 flamingo-1.9/flamingo/core/plugins/__pycache__/media.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1539 2022-05-09 07:40:40.000000 flamingo-1.9/flamingo/core/plugins/__pycache__/media.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      848 2022-04-06 13:30:00.000000 flamingo-1.9/flamingo/core/plugins/__pycache__/meta_data.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      885 2020-08-14 13:05:39.000000 flamingo-1.9/flamingo/core/plugins/__pycache__/meta_data.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      797 2020-03-18 10:00:13.000000 flamingo-1.9/flamingo/core/plugins/__pycache__/meta_data.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      840 2022-05-09 07:40:40.000000 flamingo-1.9/flamingo/core/plugins/__pycache__/meta_data.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     6861 2022-04-06 13:30:00.000000 flamingo-1.9/flamingo/core/plugins/__pycache__/plugin_manager.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5244 2020-08-14 13:05:39.000000 flamingo-1.9/flamingo/core/plugins/__pycache__/plugin_manager.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4106 2020-03-18 10:00:13.000000 flamingo-1.9/flamingo/core/plugins/__pycache__/plugin_manager.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     6853 2022-11-22 09:49:46.000000 flamingo-1.9/flamingo/core/plugins/__pycache__/plugin_manager.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      785 2022-04-06 13:30:00.000000 flamingo-1.9/flamingo/core/plugins/__pycache__/static.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      836 2020-08-14 13:05:39.000000 flamingo-1.9/flamingo/core/plugins/__pycache__/static.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      773 2020-03-18 10:00:13.000000 flamingo-1.9/flamingo/core/plugins/__pycache__/static.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      775 2022-05-09 07:40:40.000000 flamingo-1.9/flamingo/core/plugins/__pycache__/static.cpython-39.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1074 2020-03-27 21:00:49.000000 flamingo-1.9/flamingo/core/plugins/layers.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1891 2020-03-21 08:11:37.000000 flamingo-1.9/flamingo/core/plugins/media.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      932 2020-08-14 13:04:36.000000 flamingo-1.9/flamingo/core/plugins/meta_data.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    10185 2022-11-22 09:41:39.000000 flamingo-1.9/flamingo/core/plugins/plugin_manager.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      620 2020-03-22 21:24:47.000000 flamingo-1.9/flamingo/core/plugins/static.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.497409 flamingo-1.9/flamingo/core/settings/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       39 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/core/settings/__init__.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.497409 flamingo-1.9/flamingo/core/settings/__pycache__/
+-rw-r--r--   0 chris     (1000) chris     (1000)      210 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/core/settings/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      204 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/core/settings/__pycache__/__init__.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      204 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/core/settings/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      208 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/core/settings/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1642 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/core/settings/__pycache__/defaults.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1708 2020-08-14 13:06:01.000000 flamingo-1.9/flamingo/core/settings/__pycache__/defaults.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1600 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/core/settings/__pycache__/defaults.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1640 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/core/settings/__pycache__/defaults.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1691 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/core/settings/__pycache__/settings.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1782 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/core/settings/__pycache__/settings.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1657 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/core/settings/__pycache__/settings.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1675 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/core/settings/__pycache__/settings.cpython-39.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1566 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/core/settings/defaults.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1178 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/core/settings/settings.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.497409 flamingo-1.9/flamingo/core/templating/
+-rw-r--r--   0 chris     (1000) chris     (1000)       78 2019-04-20 10:57:54.000000 flamingo-1.9/flamingo/core/templating/__init__.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.497409 flamingo-1.9/flamingo/core/templating/__pycache__/
+-rw-r--r--   0 chris     (1000) chris     (1000)      253 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/core/templating/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      251 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/core/templating/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      247 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/core/templating/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      251 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/core/templating/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1202 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/core/templating/__pycache__/base.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1244 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/core/templating/__pycache__/base.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1180 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/core/templating/__pycache__/base.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1210 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/core/templating/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     9025 2022-11-06 21:06:38.000000 flamingo-1.9/flamingo/core/templating/__pycache__/jinja2.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8152 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/core/templating/__pycache__/jinja2.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7413 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/core/templating/__pycache__/jinja2.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     8996 2022-11-22 09:49:46.000000 flamingo-1.9/flamingo/core/templating/__pycache__/jinja2.cpython-39.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      781 2020-08-14 13:04:36.000000 flamingo-1.9/flamingo/core/templating/base.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    12421 2022-11-22 09:41:39.000000 flamingo-1.9/flamingo/core/templating/jinja2.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2636 2020-08-14 13:04:36.000000 flamingo-1.9/flamingo/core/types.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.497409 flamingo-1.9/flamingo/core/utils/
+-rw-r--r--   0 chris     (1000) chris     (1000)        0 2019-04-20 10:57:54.000000 flamingo-1.9/flamingo/core/utils/__init__.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.501409 flamingo-1.9/flamingo/core/utils/__pycache__/
+-rw-r--r--   0 chris     (1000) chris     (1000)      166 2022-04-06 13:30:00.000000 flamingo-1.9/flamingo/core/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      156 2020-03-21 08:12:41.000000 flamingo-1.9/flamingo/core/utils/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      160 2020-03-18 10:00:13.000000 flamingo-1.9/flamingo/core/utils/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      164 2022-05-09 07:40:40.000000 flamingo-1.9/flamingo/core/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      696 2022-05-09 07:44:34.000000 flamingo-1.9/flamingo/core/utils/__pycache__/aiohttp.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      700 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/core/utils/__pycache__/aiohttp.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      676 2020-03-18 10:14:46.000000 flamingo-1.9/flamingo/core/utils/__pycache__/aiohttp.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      690 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/core/utils/__pycache__/aiohttp.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     2477 2019-04-20 10:57:54.000000 flamingo-1.9/flamingo/core/utils/__pycache__/aionotify.cpython-35.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     4339 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/core/utils/__pycache__/cli.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4703 2020-03-21 08:12:57.000000 flamingo-1.9/flamingo/core/utils/__pycache__/cli.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4323 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/core/utils/__pycache__/cli.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     4349 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/core/utils/__pycache__/cli.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1240 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/core/utils/__pycache__/html.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1263 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/core/utils/__pycache__/html.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1181 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/core/utils/__pycache__/html.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1234 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/core/utils/__pycache__/html.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1291 2022-04-06 13:30:00.000000 flamingo-1.9/flamingo/core/utils/__pycache__/imports.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1439 2020-03-21 08:12:41.000000 flamingo-1.9/flamingo/core/utils/__pycache__/imports.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1277 2020-03-18 10:00:13.000000 flamingo-1.9/flamingo/core/utils/__pycache__/imports.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1289 2022-05-09 07:40:40.000000 flamingo-1.9/flamingo/core/utils/__pycache__/imports.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      585 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/core/utils/__pycache__/pagination.cpython-310.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      582 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/core/utils/__pycache__/pagination.cpython-35.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      550 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/core/utils/__pycache__/pagination.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      577 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/core/utils/__pycache__/pagination.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     4129 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/core/utils/__pycache__/pprint.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4565 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/core/utils/__pycache__/pprint.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4094 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/core/utils/__pycache__/pprint.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     4149 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/core/utils/__pycache__/pprint.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      930 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/core/utils/__pycache__/string.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1049 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/core/utils/__pycache__/string.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      928 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/core/utils/__pycache__/string.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      926 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/core/utils/__pycache__/string.cpython-39.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      347 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/core/utils/aiohttp.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      389 2019-04-20 10:57:54.000000 flamingo-1.9/flamingo/core/utils/chardet.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4878 2020-03-21 08:11:37.000000 flamingo-1.9/flamingo/core/utils/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      883 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/core/utils/html.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1580 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/core/utils/imports.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      660 2020-08-14 13:04:36.000000 flamingo-1.9/flamingo/core/utils/pagination.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5505 2020-03-21 08:11:37.000000 flamingo-1.9/flamingo/core/utils/pprint.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      624 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/core/utils/string.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.501409 flamingo-1.9/flamingo/plugins/
+-rw-r--r--   0 chris     (1000) chris     (1000)     1304 2022-11-06 20:41:58.000000 flamingo-1.9/flamingo/plugins/__init__.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.501409 flamingo-1.9/flamingo/plugins/__pycache__/
+-rw-r--r--   0 chris     (1000) chris     (1000)     1411 2022-11-06 21:06:38.000000 flamingo-1.9/flamingo/plugins/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1358 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/__pycache__/__init__.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1280 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1409 2022-11-06 20:48:25.000000 flamingo-1.9/flamingo/plugins/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1050 2019-04-20 10:57:54.000000 flamingo-1.9/flamingo/plugins/__pycache__/authors.cpython-35.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1910 2022-11-06 21:06:38.000000 flamingo-1.9/flamingo/plugins/__pycache__/feeds.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1985 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/__pycache__/feeds.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1837 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/__pycache__/feeds.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     2795 2022-11-22 09:49:46.000000 flamingo-1.9/flamingo/plugins/__pycache__/feeds.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1269 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/__pycache__/git.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1335 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/__pycache__/git.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1234 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/__pycache__/git.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1253 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/__pycache__/git.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1275 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/__pycache__/html.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1333 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/__pycache__/html.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1245 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/__pycache__/html.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1267 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/__pycache__/html.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1701 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/__pycache__/i18n.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1790 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/__pycache__/i18n.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1643 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/__pycache__/i18n.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1686 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/__pycache__/i18n.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1769 2019-04-20 10:57:54.000000 flamingo-1.9/flamingo/plugins/__pycache__/layers.cpython-35.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1418 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/__pycache__/md.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1509 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/__pycache__/md.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1390 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/__pycache__/md.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1412 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/__pycache__/md.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1846 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/__pycache__/redirects.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1937 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/__pycache__/redirects.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1807 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/__pycache__/redirects.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1831 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/__pycache__/redirects.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1731 2019-04-20 10:57:54.000000 flamingo-1.9/flamingo/plugins/__pycache__/tags.cpython-35.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     5820 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/__pycache__/thumbnails.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6125 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/__pycache__/thumbnails.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5568 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/__pycache__/thumbnails.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     5806 2022-11-22 09:49:46.000000 flamingo-1.9/flamingo/plugins/__pycache__/thumbnails.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     3742 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/__pycache__/time.cpython-310.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     3898 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/__pycache__/time.cpython-35.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     3637 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/__pycache__/time.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     3806 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/__pycache__/time.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      891 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/__pycache__/yaml.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      903 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/__pycache__/yaml.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      861 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/__pycache__/yaml.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      881 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/__pycache__/yaml.cpython-39.pyc
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.501409 flamingo-1.9/flamingo/plugins/authors/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/authors/__init__.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.505409 flamingo-1.9/flamingo/plugins/authors/__pycache__/
+-rw-r--r--   0 chris     (1000) chris     (1000)      171 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/authors/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      161 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/authors/__pycache__/__init__.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      165 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/authors/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      169 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/authors/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1085 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/authors/__pycache__/authors.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1157 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/authors/__pycache__/authors.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1062 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/authors/__pycache__/authors.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1074 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/authors/__pycache__/authors.cpython-39.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      955 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/authors/authors.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/authors/theme/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.505409 flamingo-1.9/flamingo/plugins/authors/theme/templates/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/authors/theme/templates/author.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/authors/theme/templates/authors.html
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.505409 flamingo-1.9/flamingo/plugins/bootstrap/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/__init__.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.505409 flamingo-1.9/flamingo/plugins/bootstrap/__pycache__/
+-rw-r--r--   0 chris     (1000) chris     (1000)      173 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/bootstrap/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      163 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/bootstrap/__pycache__/__init__.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      167 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/bootstrap/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      171 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/bootstrap/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      568 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/bootstrap/__pycache__/plugins.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      672 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/bootstrap/__pycache__/plugins.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      630 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/bootstrap/__pycache__/plugins.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      604 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/bootstrap/__pycache__/plugins.cpython-39.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      242 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/plugins.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/bootstrap/theme/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.505409 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/
+-rw-rw-r--   0 chris     (1000) chris     (1000)    25682 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap-theme.css
+-rw-rw-r--   0 chris     (1000) chris     (1000)    48005 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap-theme.css.map
+-rw-rw-r--   0 chris     (1000) chris     (1000)    23411 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap-theme.min.css
+-rw-rw-r--   0 chris     (1000) chris     (1000)    75600 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap-theme.min.css.map
+-rw-rw-r--   0 chris     (1000) chris     (1000)   145933 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap.css
+-rw-rw-r--   0 chris     (1000) chris     (1000)   390887 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap.css.map
+-rw-rw-r--   0 chris     (1000) chris     (1000)   121457 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap.min.css
+-rw-rw-r--   0 chris     (1000) chris     (1000)   540434 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap.min.css.map
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.505409 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/fonts/
+-rw-rw-r--   0 chris     (1000) chris     (1000)    20127 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/fonts/glyphicons-halflings-regular.eot
+-rw-rw-r--   0 chris     (1000) chris     (1000)   108738 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/fonts/glyphicons-halflings-regular.svg
+-rw-rw-r--   0 chris     (1000) chris     (1000)    45404 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-r--   0 chris     (1000) chris     (1000)    23424 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/fonts/glyphicons-halflings-regular.woff
+-rw-rw-r--   0 chris     (1000) chris     (1000)    18028 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.505409 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/js/
+-rw-rw-r--   0 chris     (1000) chris     (1000)    75484 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/js/bootstrap.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)    39680 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/js/bootstrap.min.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)      484 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/js/npm.js
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.509409 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/
+-rw-rw-r--   0 chris     (1000) chris     (1000)    64548 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-grid.css
+-rw-rw-r--   0 chris     (1000) chris     (1000)   151749 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-grid.css.map
+-rw-rw-r--   0 chris     (1000) chris     (1000)    48488 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-grid.min.css
+-rw-rw-r--   0 chris     (1000) chris     (1000)   108539 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-grid.min.css.map
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4897 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-reboot.css
+-rw-rw-r--   0 chris     (1000) chris     (1000)    76483 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-reboot.css.map
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4021 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-reboot.min.css
+-rw-rw-r--   0 chris     (1000) chris     (1000)    32461 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-reboot.min.css.map
+-rw-rw-r--   0 chris     (1000) chris     (1000)   192348 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap.css
+-rw-rw-r--   0 chris     (1000) chris     (1000)   492048 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap.css.map
+-rw-rw-r--   0 chris     (1000) chris     (1000)   155758 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap.min.css
+-rw-rw-r--   0 chris     (1000) chris     (1000)   625953 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap.min.css.map
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.509409 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/
+-rw-rw-r--   0 chris     (1000) chris     (1000)   222911 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.bundle.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)   402249 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.bundle.js.map
+-rw-rw-r--   0 chris     (1000) chris     (1000)    78635 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.bundle.min.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)   311949 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.bundle.min.js.map
+-rw-rw-r--   0 chris     (1000) chris     (1000)   131637 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)   250568 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.js.map
+-rw-rw-r--   0 chris     (1000) chris     (1000)    58072 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.min.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)   190253 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.min.js.map
+-rw-r--r--   0 chris     (1000) chris     (1000)     5788 2022-11-22 09:41:39.000000 flamingo-1.9/flamingo/plugins/feeds.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1189 2020-08-14 13:04:36.000000 flamingo-1.9/flamingo/plugins/git.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      948 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/html.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2720 2020-08-14 13:04:36.000000 flamingo-1.9/flamingo/plugins/i18n.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.513409 flamingo-1.9/flamingo/plugins/jquery/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/jquery/__init__.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.513409 flamingo-1.9/flamingo/plugins/jquery/__pycache__/
+-rw-r--r--   0 chris     (1000) chris     (1000)      170 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/jquery/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      160 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/jquery/__pycache__/__init__.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      164 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/jquery/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      168 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/jquery/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      676 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/jquery/__pycache__/plugins.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      877 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/jquery/__pycache__/plugins.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      814 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/jquery/__pycache__/plugins.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      752 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/jquery/__pycache__/plugins.cpython-39.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      340 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/jquery/plugins.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/jquery/theme/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/jquery/theme/jquery-1/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/jquery/theme/jquery-1/static/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.513409 flamingo-1.9/flamingo/plugins/jquery/theme/jquery-1/static/jquery/
+-rw-rw-r--   0 chris     (1000) chris     (1000)   293430 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/jquery/theme/jquery-1/static/jquery/jquery-1.12.4.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)    97163 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/jquery/theme/jquery-1/static/jquery/jquery-1.12.4.min.js
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/jquery/theme/jquery-2/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/jquery/theme/jquery-2/static/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.513409 flamingo-1.9/flamingo/plugins/jquery/theme/jquery-2/static/jquery/
+-rw-rw-r--   0 chris     (1000) chris     (1000)   257551 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/jquery/theme/jquery-2/static/jquery/jquery-2.2.4.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)    85578 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/jquery/theme/jquery-2/static/jquery/jquery-2.2.4.min.js
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/jquery/theme/jquery-3/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/jquery/theme/jquery-3/static/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.513409 flamingo-1.9/flamingo/plugins/jquery/theme/jquery-3/static/jquery/
+-rw-rw-r--   0 chris     (1000) chris     (1000)   280364 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/jquery/theme/jquery-3/static/jquery/jquery-3.4.1.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)    88145 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/jquery/theme/jquery-3/static/jquery/jquery-3.4.1.min.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)   227022 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/jquery/theme/jquery-3/static/jquery/jquery-3.4.1.slim.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)    71037 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/jquery/theme/jquery-3/static/jquery/jquery-3.4.1.slim.min.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1225 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/md.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.513409 flamingo-1.9/flamingo/plugins/menu/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2020-03-21 08:11:37.000000 flamingo-1.9/flamingo/plugins/menu/__init__.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.513409 flamingo-1.9/flamingo/plugins/menu/__pycache__/
+-rw-r--r--   0 chris     (1000) chris     (1000)      168 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/menu/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      158 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/menu/__pycache__/__init__.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      162 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/menu/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      166 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/menu/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     4550 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/menu/__pycache__/menu.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2646 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/menu/__pycache__/menu.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2435 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/menu/__pycache__/menu.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     4554 2022-11-22 09:49:46.000000 flamingo-1.9/flamingo/plugins/menu/__pycache__/menu.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     5588 2022-11-22 09:41:39.000000 flamingo-1.9/flamingo/plugins/menu/menu.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/menu/theme/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/menu/theme/templates/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.513409 flamingo-1.9/flamingo/plugins/menu/theme/templates/menu/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      669 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/menu/theme/templates/menu/bootstrap3.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)      875 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/menu/theme/templates/menu/bootstrap4.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)      290 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/menu/theme/templates/menu/index.html
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.513409 flamingo-1.9/flamingo/plugins/photoswipe/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/photoswipe/__init__.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.513409 flamingo-1.9/flamingo/plugins/photoswipe/__pycache__/
+-rw-r--r--   0 chris     (1000) chris     (1000)      174 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/photoswipe/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      164 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/photoswipe/__pycache__/__init__.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      168 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/photoswipe/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      172 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/photoswipe/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      427 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/photoswipe/__pycache__/plugin.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      434 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/photoswipe/__pycache__/plugin.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      413 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/photoswipe/__pycache__/plugin.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      423 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/photoswipe/__pycache__/plugin.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1334 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/photoswipe/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1328 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/photoswipe/__pycache__/utils.cpython-39.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      114 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/photoswipe/plugin.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/photoswipe/theme/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/photoswipe/theme/static/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.517409 flamingo-1.9/flamingo/plugins/photoswipe/theme/static/photoswipe/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.517409 flamingo-1.9/flamingo/plugins/photoswipe/theme/static/photoswipe/default-skin/
+-rw-rw-r--   0 chris     (1000) chris     (1000)    11607 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/photoswipe/theme/static/photoswipe/default-skin/default-skin.css
+-rw-rw-r--   0 chris     (1000) chris     (1000)      547 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/photoswipe/theme/static/photoswipe/default-skin/default-skin.png
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1554 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/photoswipe/theme/static/photoswipe/default-skin/default-skin.svg
+-rw-rw-r--   0 chris     (1000) chris     (1000)      866 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/photoswipe/theme/static/photoswipe/default-skin/preloader.gif
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6308 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/photoswipe/theme/static/photoswipe/photoswipe-init.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)    21504 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/photoswipe/theme/static/photoswipe/photoswipe-ui-default.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9878 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/photoswipe/theme/static/photoswipe/photoswipe-ui-default.min.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4137 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/photoswipe/theme/static/photoswipe/photoswipe.css
+-rw-rw-r--   0 chris     (1000) chris     (1000)    94045 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/photoswipe/theme/static/photoswipe/photoswipe.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)    31904 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/photoswipe/theme/static/photoswipe/photoswipe.min.js
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/photoswipe/theme/templates/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.517409 flamingo-1.9/flamingo/plugins/photoswipe/theme/templates/photoswipe/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2405 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/photoswipe/theme/templates/photoswipe/gallery.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)       69 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/photoswipe/theme/templates/photoswipe/image.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)      181 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/photoswipe/theme/templates/photoswipe/photoswipe.css.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2502 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/photoswipe/theme/templates/photoswipe/photoswipe.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)      195 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/photoswipe/theme/templates/photoswipe/photoswipe.js.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1184 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/photoswipe/utils.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1568 2020-08-14 13:04:36.000000 flamingo-1.9/flamingo/plugins/redirects.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.517409 flamingo-1.9/flamingo/plugins/rst/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      208 2020-08-14 13:04:36.000000 flamingo-1.9/flamingo/plugins/rst/__init__.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.517409 flamingo-1.9/flamingo/plugins/rst/__pycache__/
+-rw-r--r--   0 chris     (1000) chris     (1000)      417 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      157 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      161 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      415 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8089 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/base.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7449 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/base.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     4538 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/bootstrap3.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5002 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/bootstrap3.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4642 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/bootstrap3.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     4612 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/bootstrap3.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1465 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/directives.cpython-310.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1465 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/directives.cpython-39.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1327 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/file.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1250 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/file.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     3897 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/image.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4083 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/image.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3681 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/image.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     3884 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/image.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     3399 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/include.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2292 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/include.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2139 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/include.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     3392 2022-11-22 09:49:46.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/include.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     2846 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/link.cpython-310.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     2844 2022-11-22 09:49:46.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/link.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     5532 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/parser.cpython-310.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     5514 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/parser.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     3129 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/plugin.cpython-310.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     3111 2022-11-22 09:49:46.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/plugin.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     4688 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/pygments.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2203 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/pygments.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2022 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/pygments.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     4668 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/pygments.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     3995 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/table.cpython-310.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     3977 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/table.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1683 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1739 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/rst/__pycache__/utils.cpython-39.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4314 2020-08-14 13:04:36.000000 flamingo-1.9/flamingo/plugins/rst/bootstrap3.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1036 2020-08-14 13:04:36.000000 flamingo-1.9/flamingo/plugins/rst/directives.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5926 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/rst/image.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4630 2022-11-22 09:41:39.000000 flamingo-1.9/flamingo/plugins/rst/include.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3361 2022-11-22 09:41:39.000000 flamingo-1.9/flamingo/plugins/rst/link.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6380 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/rst/parser.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2581 2022-11-22 09:41:39.000000 flamingo-1.9/flamingo/plugins/rst/plugin.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4878 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/rst/pygments.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5889 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/rst/table.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1939 2020-08-14 13:04:36.000000 flamingo-1.9/flamingo/plugins/rst/utils.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.517409 flamingo-1.9/flamingo/plugins/rtd/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/__init__.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.521410 flamingo-1.9/flamingo/plugins/rtd/__pycache__/
+-rw-r--r--   0 chris     (1000) chris     (1000)      167 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/rtd/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      157 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/rtd/__pycache__/__init__.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      161 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/rtd/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      165 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/rtd/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      887 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/rtd/__pycache__/plugin.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      907 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/rtd/__pycache__/plugin.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      863 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/rtd/__pycache__/plugin.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      883 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/rtd/__pycache__/plugin.cpython-39.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      404 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/plugin.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/rtd/theme/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.521410 flamingo-1.9/flamingo/plugins/rtd/theme/static/
+-rw-rw-r--   0 chris     (1000) chris     (1000)    68650 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/elasticlunr.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)    18051 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/elasticlunr.min.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)      261 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/helper.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)    33665 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/mark.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)    16917 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/mark.min.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)   510145 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/ractive.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)  1106790 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/ractive.js.map
+-rw-rw-r--   0 chris     (1000) chris     (1000)   226170 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/ractive.min.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)   863802 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/ractive.min.js.map
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.521410 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.521410 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/css/
+-rw-rw-r--   0 chris     (1000) chris     (1000)   118340 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/css/theme.css
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9313 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/doctools.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)      307 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/documentation_options.js
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.525410 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.529410 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/
+-rw-rw-r--   0 chris     (1000) chris     (1000)   256056 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bold.eot
+-rw-rw-r--   0 chris     (1000) chris     (1000)   256056 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bold.eot?
+-rw-rw-r--   0 chris     (1000) chris     (1000)   600856 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bold.ttf
+-rw-rw-r--   0 chris     (1000) chris     (1000)   309728 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bold.woff
+-rw-rw-r--   0 chris     (1000) chris     (1000)   184912 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bold.woff2
+-rw-rw-r--   0 chris     (1000) chris     (1000)   266158 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bolditalic.eot
+-rw-rw-r--   0 chris     (1000) chris     (1000)   266158 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bolditalic.eot?
+-rw-rw-r--   0 chris     (1000) chris     (1000)   622572 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bolditalic.ttf
+-rw-rw-r--   0 chris     (1000) chris     (1000)   323344 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bolditalic.woff
+-rw-rw-r--   0 chris     (1000) chris     (1000)   193308 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bolditalic.woff2
+-rw-rw-r--   0 chris     (1000) chris     (1000)   268604 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-italic.eot
+-rw-rw-r--   0 chris     (1000) chris     (1000)   268604 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-italic.eot?
+-rw-rw-r--   0 chris     (1000) chris     (1000)   639388 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-italic.ttf
+-rw-rw-r--   0 chris     (1000) chris     (1000)   328412 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-italic.woff
+-rw-rw-r--   0 chris     (1000) chris     (1000)   195704 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-italic.woff2
+-rw-rw-r--   0 chris     (1000) chris     (1000)   253461 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-regular.eot
+-rw-rw-r--   0 chris     (1000) chris     (1000)   253461 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-regular.eot?
+-rw-rw-r--   0 chris     (1000) chris     (1000)   607720 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-regular.ttf
+-rw-rw-r--   0 chris     (1000) chris     (1000)   309192 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-regular.woff
+-rw-rw-r--   0 chris     (1000) chris     (1000)   182708 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-regular.woff2
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.529410 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/
+-rw-rw-r--   0 chris     (1000) chris     (1000)    79520 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-bold.eot
+-rw-rw-r--   0 chris     (1000) chris     (1000)    79520 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-bold.eot?
+-rw-rw-r--   0 chris     (1000) chris     (1000)   170616 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-bold.ttf
+-rw-rw-r--   0 chris     (1000) chris     (1000)    87624 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-bold.woff
+-rw-rw-r--   0 chris     (1000) chris     (1000)    67312 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-bold.woff2
+-rw-rw-r--   0 chris     (1000) chris     (1000)    78331 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-regular.eot?
+-rw-rw-r--   0 chris     (1000) chris     (1000)   169064 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-regular.ttf
+-rw-rw-r--   0 chris     (1000) chris     (1000)    86288 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-regular.woff
+-rw-rw-r--   0 chris     (1000) chris     (1000)    66444 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-regular.woff2
+-rw-rw-r--   0 chris     (1000) chris     (1000)   165742 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/fontawesome-webfont.eot
+-rw-rw-r--   0 chris     (1000) chris     (1000)   444379 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/fontawesome-webfont.svg
+-rw-rw-r--   0 chris     (1000) chris     (1000)   165548 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/fontawesome-webfont.ttf
+-rw-rw-r--   0 chris     (1000) chris     (1000)    98024 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/fontawesome-webfont.woff
+-rw-rw-r--   0 chris     (1000) chris     (1000)    77160 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/fontawesome-webfont.woff2
+-rw-rw-r--   0 chris     (1000) chris     (1000)    86659 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/jquery.js
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.529410 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/js/
+-rw-rw-r--   0 chris     (1000) chris     (1000)    15414 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/js/modernizr.min.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4414 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/js/theme.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10847 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/language_data.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)       90 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/minus.png
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4395 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/pygments.css
+-rw-rw-r--   0 chris     (1000) chris     (1000)      480 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/readthedocs-data.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)    15060 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/searchtools.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)    12140 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/underscore.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)      275 2020-03-21 08:11:37.000000 flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd.css
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/rtd/theme/templates/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.529410 flamingo-1.9/flamingo/plugins/rtd/theme/templates/rtd/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      382 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/templates/rtd/mark.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4955 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/rtd/theme/templates/rtd/page.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1319 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/rtd/theme/templates/rtd/search.html
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.529410 flamingo-1.9/flamingo/plugins/sphinx_themes/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/__init__.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.533410 flamingo-1.9/flamingo/plugins/sphinx_themes/__pycache__/
+-rw-r--r--   0 chris     (1000) chris     (1000)      177 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      175 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1093 2022-11-06 21:06:38.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/__pycache__/defaults.cpython-310.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1091 2022-11-04 15:49:13.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/__pycache__/defaults.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     9780 2022-11-06 21:06:38.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/__pycache__/plugin.cpython-310.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     9667 2022-11-13 11:21:24.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/__pycache__/plugin.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     7387 2022-11-06 21:06:38.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/__pycache__/sphinx_theme.cpython-310.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     7387 2022-11-22 09:49:46.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/__pycache__/sphinx_theme.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      805 2022-05-12 17:06:13.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/defaults.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    13861 2022-11-07 17:12:27.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/plugin.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     8888 2022-11-22 09:41:39.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/sphinx_theme.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/sphinx_themes/theme/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/sphinx_themes/theme/static/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.533410 flamingo-1.9/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/
+-rw-rw-r--   0 chris     (1000) chris     (1000)    68650 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/elasticlunr.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)    18051 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/elasticlunr.min.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)      261 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/helper.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)    89476 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/jquery.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)      298 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/main.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)    33665 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/mark.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)    16917 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/mark.min.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)   510145 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/ractive.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)  1106790 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/ractive.js.map
+-rw-rw-r--   0 chris     (1000) chris     (1000)   226170 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/ractive.min.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)   863802 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/ractive.min.js.map
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/sphinx_themes/theme/templates/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.533410 flamingo-1.9/flamingo/plugins/sphinx_themes/theme/templates/sphinx_themes/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       64 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/theme/templates/sphinx_themes/body.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)      901 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/theme/templates/sphinx_themes/search.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)      415 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/theme/templates/sphinx_themes/search_variables.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2043 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/sphinx_themes/theme/templates/sphinx_themes/toctree.html
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.533410 flamingo-1.9/flamingo/plugins/tags/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/tags/__init__.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.533410 flamingo-1.9/flamingo/plugins/tags/__pycache__/
+-rw-r--r--   0 chris     (1000) chris     (1000)      168 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/tags/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      158 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/tags/__pycache__/__init__.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      162 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/tags/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      166 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/tags/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1712 2022-04-06 13:30:15.000000 flamingo-1.9/flamingo/plugins/tags/__pycache__/tags.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1835 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/plugins/tags/__pycache__/tags.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1648 2020-03-18 10:08:20.000000 flamingo-1.9/flamingo/plugins/tags/__pycache__/tags.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1697 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/plugins/tags/__pycache__/tags.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     2318 2022-04-06 13:20:24.000000 flamingo-1.9/flamingo/plugins/tags/tags.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/plugins/tags/theme/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.533410 flamingo-1.9/flamingo/plugins/tags/theme/templates/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       93 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/tags/theme/templates/tag.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)      310 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/tags/theme/templates/tags.html
+-rw-r--r--   0 chris     (1000) chris     (1000)     9261 2022-11-22 09:41:39.000000 flamingo-1.9/flamingo/plugins/thumbnails.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3534 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/plugins/time.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      951 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/plugins/yaml.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.533410 flamingo-1.9/flamingo/project_templates/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.537410 flamingo-1.9/flamingo/project_templates/bootstrap4/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      659 2020-03-21 08:11:37.000000 flamingo-1.9/flamingo/project_templates/bootstrap4/Makefile.template
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/project_templates/bootstrap4/README.rst
+-rw-rw-r--   0 chris     (1000) chris     (1000)      173 2020-03-21 08:11:37.000000 flamingo-1.9/flamingo/project_templates/bootstrap4/REQUIREMENTS.txt.template
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.537410 flamingo-1.9/flamingo/project_templates/bootstrap4/content/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.537410 flamingo-1.9/flamingo/project_templates/bootstrap4/content/category-1/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/project_templates/bootstrap4/content/category-1/page-1.rst
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/project_templates/bootstrap4/content/category-1/page-2.rst
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.537410 flamingo-1.9/flamingo/project_templates/bootstrap4/content/category-2/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/project_templates/bootstrap4/content/category-2/page-3.rst
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/project_templates/bootstrap4/content/category-2/page-4.rst
+-rw-rw-r--   0 chris     (1000) chris     (1000)       54 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/project_templates/bootstrap4/content/home.rst
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.537410 flamingo-1.9/flamingo/project_templates/bootstrap4/overlay/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1150 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/project_templates/bootstrap4/overlay/favicon.ico
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.537410 flamingo-1.9/flamingo/project_templates/bootstrap4/plugins/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      423 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/project_templates/bootstrap4/plugins/example.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      586 2020-03-21 08:11:37.000000 flamingo-1.9/flamingo/project_templates/bootstrap4/settings.py.template
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/project_templates/bootstrap4/theme/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.537410 flamingo-1.9/flamingo/project_templates/bootstrap4/theme/static/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      320 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/project_templates/bootstrap4/theme/static/custom.css
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.537410 flamingo-1.9/flamingo/project_templates/bootstrap4/theme/templates/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1476 2020-03-21 08:11:37.000000 flamingo-1.9/flamingo/project_templates/bootstrap4/theme/templates/base.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)      290 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/project_templates/bootstrap4/theme/templates/page.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)      684 2020-03-21 08:11:37.000000 flamingo-1.9/flamingo/project_templates/data.ini
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.537410 flamingo-1.9/flamingo/project_templates/readthedocs/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      659 2020-03-21 08:11:37.000000 flamingo-1.9/flamingo/project_templates/readthedocs/Makefile.template
+-rw-rw-r--   0 chris     (1000) chris     (1000)      191 2020-03-21 08:11:37.000000 flamingo-1.9/flamingo/project_templates/readthedocs/REQUIREMENTS.txt.template
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.537410 flamingo-1.9/flamingo/project_templates/readthedocs/content/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       14 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/project_templates/readthedocs/content/index.rst
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.537410 flamingo-1.9/flamingo/project_templates/readthedocs/overlay/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1150 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/project_templates/readthedocs/overlay/favicon.ico
+-rw-rw-r--   0 chris     (1000) chris     (1000)      376 2020-03-21 08:11:37.000000 flamingo-1.9/flamingo/project_templates/readthedocs/settings.py.template
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/project_templates/readthedocs/theme/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.537410 flamingo-1.9/flamingo/project_templates/readthedocs/theme/static/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/project_templates/readthedocs/theme/static/custom.css
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.537410 flamingo-1.9/flamingo/project_templates/readthedocs/theme/templates/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      138 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/project_templates/readthedocs/theme/templates/page.html
+-rw-r--r--   0 chris     (1000) chris     (1000)     5564 2022-05-12 17:06:13.000000 flamingo-1.9/flamingo/pytest.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.537410 flamingo-1.9/flamingo/server/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2020-03-21 08:11:37.000000 flamingo-1.9/flamingo/server/__init__.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.537410 flamingo-1.9/flamingo/server/__pycache__/
+-rw-r--r--   0 chris     (1000) chris     (1000)      162 2022-05-09 07:44:34.000000 flamingo-1.9/flamingo/server/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      152 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/server/__pycache__/__init__.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)      156 2020-03-18 10:14:46.000000 flamingo-1.9/flamingo/server/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)      160 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/server/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     3687 2022-05-09 07:44:34.000000 flamingo-1.9/flamingo/server/__pycache__/build_environment.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3285 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/server/__pycache__/build_environment.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2950 2020-03-18 10:14:46.000000 flamingo-1.9/flamingo/server/__pycache__/build_environment.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     3663 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/server/__pycache__/build_environment.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     8510 2022-05-09 07:44:34.000000 flamingo-1.9/flamingo/server/__pycache__/exporter.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5321 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/server/__pycache__/exporter.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4877 2020-03-18 10:14:46.000000 flamingo-1.9/flamingo/server/__pycache__/exporter.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     8502 2022-11-13 14:30:22.000000 flamingo-1.9/flamingo/server/__pycache__/exporter.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1777 2022-05-09 07:44:34.000000 flamingo-1.9/flamingo/server/__pycache__/frontend_controller.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1981 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/server/__pycache__/frontend_controller.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1869 2020-03-18 10:14:46.000000 flamingo-1.9/flamingo/server/__pycache__/frontend_controller.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     1821 2022-05-09 07:40:47.000000 flamingo-1.9/flamingo/server/__pycache__/frontend_controller.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     3824 2022-05-09 07:44:34.000000 flamingo-1.9/flamingo/server/__pycache__/logging.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3903 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/server/__pycache__/logging.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3574 2020-03-18 10:14:46.000000 flamingo-1.9/flamingo/server/__pycache__/logging.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     3826 2022-11-13 14:30:22.000000 flamingo-1.9/flamingo/server/__pycache__/logging.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     5251 2022-05-09 07:44:34.000000 flamingo-1.9/flamingo/server/__pycache__/rpc.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2850 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/server/__pycache__/rpc.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2657 2020-03-18 10:14:46.000000 flamingo-1.9/flamingo/server/__pycache__/rpc.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     5229 2022-11-13 14:30:22.000000 flamingo-1.9/flamingo/server/__pycache__/rpc.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)    12294 2022-05-09 07:44:34.000000 flamingo-1.9/flamingo/server/__pycache__/server.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)    11314 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/server/__pycache__/server.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10187 2020-03-18 10:14:46.000000 flamingo-1.9/flamingo/server/__pycache__/server.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)    12262 2022-11-13 14:30:22.000000 flamingo-1.9/flamingo/server/__pycache__/server.cpython-39.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     4472 2022-05-09 07:44:34.000000 flamingo-1.9/flamingo/server/__pycache__/watcher.cpython-310.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4925 2020-03-21 08:12:58.000000 flamingo-1.9/flamingo/server/__pycache__/watcher.cpython-35.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4429 2020-03-18 10:14:46.000000 flamingo-1.9/flamingo/server/__pycache__/watcher.cpython-37.pyc
+-rw-r--r--   0 chris     (1000) chris     (1000)     4454 2022-11-13 14:30:22.000000 flamingo-1.9/flamingo/server/__pycache__/watcher.cpython-39.pyc
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5079 2020-08-14 13:04:36.000000 flamingo-1.9/flamingo/server/build_environment.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    10161 2022-11-22 09:41:39.000000 flamingo-1.9/flamingo/server/exporter.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1222 2020-03-21 08:11:37.000000 flamingo-1.9/flamingo/server/frontend_controller.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     5605 2022-11-22 09:41:39.000000 flamingo-1.9/flamingo/server/logging.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6731 2022-11-22 09:41:39.000000 flamingo-1.9/flamingo/server/rpc.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    17401 2022-11-22 09:41:39.000000 flamingo-1.9/flamingo/server/server.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.537410 flamingo-1.9/flamingo/server/static/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.541410 flamingo-1.9/flamingo/server/static/lib/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1642 2020-03-21 08:11:37.000000 flamingo-1.9/flamingo/server/static/lib/js.cookie-2.2.1.min.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)   508398 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/server/static/lib/ractive.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)  1101495 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/server/static/lib/ractive.js.map
+-rw-rw-r--   0 chris     (1000) chris     (1000)   225749 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/server/static/lib/ractive.min.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)   859629 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/server/static/lib/ractive.min.js.map
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4296 2020-03-21 08:11:37.000000 flamingo-1.9/flamingo/server/static/lib/rpc.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)      375 2020-03-21 08:11:37.000000 flamingo-1.9/flamingo/server/static/loading.svg
+-rw-rw-r--   0 chris     (1000) chris     (1000)    13557 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/server/static/main.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7808 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/server/static/style.css
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.541410 flamingo-1.9/flamingo/server/templates/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      271 2020-08-14 13:04:36.000000 flamingo-1.9/flamingo/server/templates/404.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)      277 2020-08-14 13:04:36.000000 flamingo-1.9/flamingo/server/templates/500.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)      992 2020-08-14 13:04:36.000000 flamingo-1.9/flamingo/server/templates/directory_list.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8995 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/server/templates/index.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2107 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/server/templates/plugin_options.html
+-rw-r--r--   0 chris     (1000) chris     (1000)     6202 2022-11-22 09:41:39.000000 flamingo-1.9/flamingo/server/watcher.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.489409 flamingo-1.9/flamingo/theme/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.541410 flamingo-1.9/flamingo/theme/templates/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      273 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/theme/templates/base.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)      350 2020-03-21 08:11:37.000000 flamingo-1.9/flamingo/theme/templates/code-block.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)      119 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/theme/templates/gallery.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1736 2020-03-21 08:11:37.000000 flamingo-1.9/flamingo/theme/templates/image.html
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.541410 flamingo-1.9/flamingo/theme/templates/jinja2/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6278 2020-08-14 13:04:36.000000 flamingo-1.9/flamingo/theme/templates/jinja2/error.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)      130 2019-12-16 13:56:30.000000 flamingo-1.9/flamingo/theme/templates/page.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)      401 2021-12-06 19:14:04.000000 flamingo-1.9/flamingo/theme/templates/table.html
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-11-22 09:50:22.493409 flamingo-1.9/flamingo.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     3353 2022-11-22 09:50:22.000000 flamingo-1.9/flamingo.egg-info/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)    31107 2022-11-22 09:50:22.000000 flamingo-1.9/flamingo.egg-info/SOURCES.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2022-11-22 09:50:22.000000 flamingo-1.9/flamingo.egg-info/dependency_links.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       39 2022-11-22 09:50:22.000000 flamingo-1.9/flamingo.egg-info/entry_points.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)      437 2022-11-22 09:50:22.000000 flamingo-1.9/flamingo.egg-info/requires.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        9 2022-11-22 09:50:22.000000 flamingo-1.9/flamingo.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1006 2022-11-22 09:50:22.541410 flamingo-1.9/setup.cfg
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     1571 2022-05-12 17:06:13.000000 flamingo-1.9/setup.py
```

### Comparing `flamingo-1.8/LICENCE` & `flamingo-1.9/LICENCE`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/PKG-INFO` & `flamingo-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamingo
-Version: 1.8
+Version: 1.9
 Summary: Flamingo is a python3-based, pelican-inspired static site generator
 Home-page: https://github.com/pengutronix/flamingo
 Author: Florian Scherf
 Author-email: python@pengutronix.de
 License: Apache License 2.0
 Description: flamingo
         ========
```

### Comparing `flamingo-1.8/README.rst` & `flamingo-1.9/README.rst`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/bin/_flamingo-args` & `flamingo-1.9/bin/_flamingo-args`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/bin/_flamingo-init` & `flamingo-1.9/bin/_flamingo-init`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/bin/_flamingo-server` & `flamingo-1.9/bin/_flamingo-server`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/bin/flamingo` & `flamingo-1.9/bin/flamingo`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/__pycache__/__init__.cpython-310.pyc` & `flamingo-1.9/flamingo/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Apr  6 13:20:24 2022 UTC, .py size: 493 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-00000000: 6f0d 0d0a 0000 0000 9893 4d62 ed01 0000  o.........Mb....
+00000000: 6f0d 0d0a 0000 0000 853e 7d62 ea01 0000  o........>}b....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6500 6a08 a009  d.l.m.Z...e.j...
 00000060: 650a a101 5a0b 6404 5a0c 6405 a00d 6406  e...Z.d.Z.d...d.
 00000070: 6407 8400 650c 4400 8301 a101 5a0e 6500  d...e.D.....Z.e.
 00000080: 6a08 a00d 650b 6408 a102 5a0f 6500 6a08  j...e.d...Z.e.j.
 00000090: a00d 650b 6409 a102 5a10 6500 6a08 a00d  ..e.d...Z.e.j...
 000000a0: 6510 640a a102 5a11 6401 5300 290b e900  e.d...Z.d.S.)...
 000000b0: 0000 004e 2904 da07 436f 6e74 656e 74da  ...N)...Content.
 000000c0: 0a43 6f6e 7465 6e74 5365 74da 0146 da01  .ContentSet..F..
-000000d0: 5129 01da 0468 6f6f 6b29 03e9 0100 0000  Q)...hook)......
-000000e0: e907 0000 0072 0700 0000 da01 2e63 0100  .....r.......c..
-000000f0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00000100: 0000 4300 0000 7314 0000 0067 007c 005d  ..C...s....g.|.]
-00000110: 067d 0174 007c 0183 0191 0271 0253 00a9  .}.t.|.....q.S..
-00000120: 0029 01da 0373 7472 2902 da02 2e30 da01  .)...str)....0..
-00000130: 6972 0a00 0000 720a 0000 00fa 3e2f 686f  ir....r.....>/ho
-00000140: 6d65 2f63 6872 6973 2f77 6f72 6b2f 5072  me/chris/work/Pr
-00000150: 6f6a 6563 7473 2f67 6974 6875 622f 666c  ojects/github/fl
-00000160: 616d 696e 676f 2f66 6c61 6d69 6e67 6f2f  amingo/flamingo/
-00000170: 5f5f 696e 6974 5f5f 2e70 79da 0a3c 6c69  __init__.py..<li
-00000180: 7374 636f 6d70 3e09 0000 0073 0200 0000  stcomp>....s....
-00000190: 1400 720f 0000 005a 0574 6865 6d65 5a11  ..r....Z.themeZ.
-000001a0: 7072 6f6a 6563 745f 7465 6d70 6c61 7465  project_template
-000001b0: 737a 0864 6174 612e 696e 6929 12da 026f  sz.data.ini)...o
-000001c0: 735a 1866 6c61 6d69 6e67 6f2e 636f 7265  sZ.flamingo.core
-000001d0: 2e64 6174 615f 6d6f 6465 6c72 0200 0000  .data_modelr....
-000001e0: 7203 0000 0072 0400 0000 7205 0000 005a  r....r....r....Z
-000001f0: 2466 6c61 6d69 6e67 6f2e 636f 7265 2e70  $flamingo.core.p
-00000200: 6c75 6769 6e73 2e70 6c75 6769 6e5f 6d61  lugins.plugin_ma
-00000210: 6e61 6765 7272 0600 0000 da04 7061 7468  nagerr......path
-00000220: da07 6469 726e 616d 65da 085f 5f66 696c  ..dirname..__fil
-00000230: 655f 5f5a 085f 6469 726e 616d 65da 0756  e__Z._dirname..V
-00000240: 4552 5349 4f4e da04 6a6f 696e da0e 5645  ERSION..join..VE
-00000250: 5253 494f 4e5f 5354 5249 4e47 5a0a 5448  RSION_STRINGZ.TH
-00000260: 454d 455f 524f 4f54 5a16 5052 4f4a 4543  EME_ROOTZ.PROJEC
-00000270: 545f 5445 4d50 4c41 5445 535f 524f 4f54  T_TEMPLATES_ROOT
-00000280: 5a1b 5052 4f4a 4543 545f 5445 4d50 4c41  Z.PROJECT_TEMPLA
-00000290: 5445 535f 4441 5441 5f50 4154 4872 0a00  TES_DATA_PATHr..
-000002a0: 0000 720a 0000 0072 0a00 0000 720e 0000  ..r....r....r...
-000002b0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-000002c0: 1600 0000 0800 1802 0c01 0c02 0402 1401  ................
-000002d0: 0e01 0e01 0802 0201 08ff                 ..........
+000000d0: 5129 01da 0468 6f6f 6b29 02e9 0100 0000  Q)...hook)......
+000000e0: e908 0000 00da 012e 6301 0000 0000 0000  ........c.......
+000000f0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+00000100: 0073 1400 0000 6700 7c00 5d06 7d01 7400  .s....g.|.].}.t.
+00000110: 7c01 8301 9102 7102 5300 a900 2901 da03  |.....q.S...)...
+00000120: 7374 7229 02da 022e 30da 0169 720a 0000  str)....0..ir...
+00000130: 0072 0a00 0000 fa3e 2f68 6f6d 652f 6368  .r.....>/home/ch
+00000140: 7269 732f 776f 726b 2f50 726f 6a65 6374  ris/work/Project
+00000150: 732f 6769 7468 7562 2f66 6c61 6d69 6e67  s/github/flaming
+00000160: 6f2f 666c 616d 696e 676f 2f5f 5f69 6e69  o/flamingo/__ini
+00000170: 745f 5f2e 7079 da0a 3c6c 6973 7463 6f6d  t__.py..<listcom
+00000180: 703e 0900 0000 7302 0000 0014 0072 0f00  p>....s......r..
+00000190: 0000 5a05 7468 656d 655a 1170 726f 6a65  ..Z.themeZ.proje
+000001a0: 6374 5f74 656d 706c 6174 6573 7a08 6461  ct_templatesz.da
+000001b0: 7461 2e69 6e69 2912 da02 6f73 5a18 666c  ta.ini)...osZ.fl
+000001c0: 616d 696e 676f 2e63 6f72 652e 6461 7461  amingo.core.data
+000001d0: 5f6d 6f64 656c 7202 0000 0072 0300 0000  _modelr....r....
+000001e0: 7204 0000 0072 0500 0000 5a24 666c 616d  r....r....Z$flam
+000001f0: 696e 676f 2e63 6f72 652e 706c 7567 696e  ingo.core.plugin
+00000200: 732e 706c 7567 696e 5f6d 616e 6167 6572  s.plugin_manager
+00000210: 7206 0000 00da 0470 6174 68da 0764 6972  r......path..dir
+00000220: 6e61 6d65 da08 5f5f 6669 6c65 5f5f 5a08  name..__file__Z.
+00000230: 5f64 6972 6e61 6d65 da07 5645 5253 494f  _dirname..VERSIO
+00000240: 4eda 046a 6f69 6eda 0e56 4552 5349 4f4e  N..join..VERSION
+00000250: 5f53 5452 494e 475a 0a54 4845 4d45 5f52  _STRINGZ.THEME_R
+00000260: 4f4f 545a 1650 524f 4a45 4354 5f54 454d  OOTZ.PROJECT_TEM
+00000270: 504c 4154 4553 5f52 4f4f 545a 1b50 524f  PLATES_ROOTZ.PRO
+00000280: 4a45 4354 5f54 454d 504c 4154 4553 5f44  JECT_TEMPLATES_D
+00000290: 4154 415f 5041 5448 720a 0000 0072 0a00  ATA_PATHr....r..
+000002a0: 0000 720a 0000 0072 0e00 0000 da08 3c6d  ..r....r......<m
+000002b0: 6f64 756c 653e 0100 0000 7316 0000 0008  odule>....s.....
+000002c0: 0018 020c 010c 0204 0214 010e 010e 0108  ................
+000002d0: 0202 0108 ff                             .....
```

### Comparing `flamingo-1.8/flamingo/__pycache__/__init__.cpython-35.pyc` & `flamingo-1.9/flamingo/__pycache__/__init__.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/__pycache__/__init__.cpython-37.pyc` & `flamingo-1.9/flamingo/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/__pycache__/__init__.cpython-39.pyc` & `flamingo-1.9/flamingo/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May 12 17:06:13 2022 UTC, .py size: 490 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-00000000: 610d 0d0a 0000 0000 853e 7d62 ea01 0000  a........>}b....
+00000000: 610d 0d0a 0000 0000 b99a 7c63 ea01 0000  a.........|c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6500 6a08 a009  d.l.m.Z...e.j...
 00000060: 650a a101 5a0b 6404 5a0c 6405 a00d 6406  e...Z.d.Z.d...d.
 00000070: 6407 8400 650c 4400 8301 a101 5a0e 6500  d...e.D.....Z.e.
 00000080: 6a08 a00d 650b 6408 a102 5a0f 6500 6a08  j...e.d...Z.e.j.
 00000090: a00d 650b 6409 a102 5a10 6500 6a08 a00d  ..e.d...Z.e.j...
 000000a0: 6510 640a a102 5a11 6401 5300 290b e900  e.d...Z.d.S.)...
 000000b0: 0000 004e 2904 da07 436f 6e74 656e 74da  ...N)...Content.
 000000c0: 0a43 6f6e 7465 6e74 5365 74da 0146 da01  .ContentSet..F..
 000000d0: 5129 01da 0468 6f6f 6b29 02e9 0100 0000  Q)...hook)......
-000000e0: e908 0000 00da 012e 6301 0000 0000 0000  ........c.......
+000000e0: e909 0000 00da 012e 6301 0000 0000 0000  ........c.......
 000000f0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
 00000100: 0073 1400 0000 6700 7c00 5d0c 7d01 7400  .s....g.|.].}.t.
 00000110: 7c01 8301 9102 7104 5300 a900 2901 da03  |.....q.S...)...
 00000120: 7374 7229 02da 022e 30da 0169 720a 0000  str)....0..ir...
 00000130: 0072 0a00 0000 fa3e 2f68 6f6d 652f 6368  .r.....>/home/ch
 00000140: 7269 732f 776f 726b 2f50 726f 6a65 6374  ris/work/Project
 00000150: 732f 6769 7468 7562 2f66 6c61 6d69 6e67  s/github/flaming
@@ -30,15 +30,15 @@
 000001d0: 6f64 656c 7202 0000 0072 0300 0000 7204  odelr....r....r.
 000001e0: 0000 0072 0500 0000 5a24 666c 616d 696e  ...r....Z$flamin
 000001f0: 676f 2e63 6f72 652e 706c 7567 696e 732e  go.core.plugins.
 00000200: 706c 7567 696e 5f6d 616e 6167 6572 7206  plugin_managerr.
 00000210: 0000 00da 0470 6174 68da 0764 6972 6e61  .....path..dirna
 00000220: 6d65 da08 5f5f 6669 6c65 5f5f 5a08 5f64  me..__file__Z._d
 00000230: 6972 6e61 6d65 da07 5645 5253 494f 4eda  irname..VERSION.
-00000240: 046a 6f69 6eda 0e56 4552 5349 4f4e 5f53  .join..VERSION_S
+00000240: 046a 6f69 6e5a 0e56 4552 5349 4f4e 5f53  .joinZ.VERSION_S
 00000250: 5452 494e 475a 0a54 4845 4d45 5f52 4f4f  TRINGZ.THEME_ROO
 00000260: 545a 1650 524f 4a45 4354 5f54 454d 504c  TZ.PROJECT_TEMPL
 00000270: 4154 4553 5f52 4f4f 545a 1b50 524f 4a45  ATES_ROOTZ.PROJE
 00000280: 4354 5f54 454d 504c 4154 4553 5f44 4154  CT_TEMPLATES_DAT
 00000290: 415f 5041 5448 720a 0000 0072 0a00 0000  A_PATHr....r....
 000002a0: 720a 0000 0072 0e00 0000 da08 3c6d 6f64  r....r......<mod
 000002b0: 756c 653e 0100 0000 7314 0000 0008 0218  ule>....s.......
```

### Comparing `flamingo-1.8/flamingo/__pycache__/default_settings.cpython-35.pyc` & `flamingo-1.9/flamingo/__pycache__/default_settings.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/__pycache__/context.cpython-310.pyc` & `flamingo-1.9/flamingo/core/__pycache__/context.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/__pycache__/context.cpython-35.pyc` & `flamingo-1.9/flamingo/core/__pycache__/context.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/__pycache__/context.cpython-37.pyc` & `flamingo-1.9/flamingo/core/__pycache__/context.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/__pycache__/context.cpython-39.pyc` & `flamingo-1.9/flamingo/core/__pycache__/context.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Dec  6 19:14:04 2021 UTC, .py size: 10716 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 fc60 ae61 dc29 0000  a........`.a.)..
+00000000: 610d 0d0a 0000 0000 5399 7c63 de29 0000  a.......S.|c.)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 6d08 5a08  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d09 5a09 0100 6400 6403 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6404 6c0c 6d0d 5a0d 6d0e 5a0e  ..d.d.l.m.Z.m.Z.
@@ -367,15 +367,15 @@
 000016e0: 6720 2573 722b 0000 0072 5e00 0000 724b  g %sr+...r^...rK
 000016f0: 0000 0072 5f00 0000 725c 0000 0072 5d00  ...r_...r\...r].
 00001700: 0000 5472 5b00 0000 5a16 7465 6d70 6c61  ..Tr[...Z.templa
 00001710: 7465 5f63 6f6e 7465 7874 5f73 6574 7570  te_context_setup
 00001720: 2908 7224 0000 0072 2500 0000 725a 0000  ).r$...r%...rZ..
 00001730: 0072 6100 0000 7214 0000 00da 0872 756e  .ra...r......run
 00001740: 5f68 6f6f 6b72 2900 0000 da06 7265 6e64  _hookr).....rend
-00001750: 6572 2906 7216 0000 0072 0f00 0000 da0d  er).r....r......
+00001750: 6572 2906 7216 0000 0072 0f00 0000 5a0d  er).r....r....Z.
 00001760: 7465 6d70 6c61 7465 5f6e 616d 6572 5e00  template_namer^.
 00001770: 0000 da08 6578 6974 636f 6465 da06 6f75  ....exitcode..ou
 00001780: 7470 7574 7219 0000 0072 1900 0000 721a  tputr....r....r.
 00001790: 0000 0072 6400 0000 0301 0000 732c 0000  ...rd.......s,..
 000017a0: 0000 010c 0212 0102 ff04 0304 0108 020c  ................
 000017b0: 020c 0204 0102 0102 fe0a 0504 0108 010a  ................
 000017c0: 0304 0208 0106 ff04 030e 0108 027a 0e43  .............z.C
@@ -400,50 +400,50 @@
 000018f0: 0000 0000 0000 0000 0400 0000 0400 0000  ................
 00001900: 4300 0000 7344 0000 007c 006a 006a 0172  C...sD...|.j.j.r
 00001910: 107c 0273 1064 0053 0074 026a 03a0 047c  .|.s.d.S.t.j...|
 00001920: 01a1 017d 0374 026a 03a0 057c 03a1 0173  ...}.t.j...|...s
 00001930: 407c 006a 06a0 0764 017c 03a1 0201 0074  @|.j...d.|.....t
 00001940: 02a0 087c 03a1 0101 0064 0053 0029 024e  ...|.....d.S.).N
 00001950: 7a0b 6d6b 6469 7220 2d70 2025 7329 0972  z.mkdir -p %s).r
-00001960: 1300 0000 7268 0000 0072 2d00 0000 722b  ....rh...r-...r+
+00001960: 1300 0000 7267 0000 0072 2d00 0000 722b  ....rg...r-...r+
 00001970: 0000 0072 2f00 0000 7231 0000 0072 2400  ...r/...r1...r$.
 00001980: 0000 7225 0000 00da 086d 616b 6564 6972  ..r%.....makedir
-00001990: 7329 0472 1600 0000 722b 0000 0072 6d00  s).r....r+...rm.
+00001990: 7329 0472 1600 0000 722b 0000 0072 6c00  s).r....r+...rl.
 000019a0: 0000 722f 0000 0072 1900 0000 7219 0000  ..r/...r....r...
 000019b0: 0072 1a00 0000 da07 6d6b 6469 725f 7030  .r......mkdir_p0
 000019c0: 0100 0073 0c00 0000 0001 0c01 0402 0c02  ...s............
 000019d0: 0c01 0e01 7a0f 436f 6e74 6578 742e 6d6b  ....z.Context.mk
 000019e0: 6469 725f 7063 0400 0000 0000 0000 0000  dir_pc..........
 000019f0: 0000 0400 0000 0500 0000 4300 0000 733a  ..........C...s:
 00001a00: 0000 007c 006a 006a 0172 107c 0373 1064  ...|.j.j.r.|.s.d
 00001a10: 0053 007c 00a0 027c 02a1 0101 007c 006a  .S.|...|.....|.j
 00001a20: 03a0 0464 017c 017c 02a1 0301 0074 05a0  ...d.|.|.....t..
 00001a30: 067c 017c 02a1 0201 0064 0053 0029 024e  .|.|.....d.S.).N
 00001a40: 7a08 6370 2025 7320 2573 2907 7213 0000  z.cp %s %s).r...
-00001a50: 0072 6800 0000 7270 0000 0072 2400 0000  .rh...rp...r$...
-00001a60: 7225 0000 0072 6a00 0000 da04 636f 7079  r%...rj.....copy
+00001a50: 0072 6700 0000 726f 0000 0072 2400 0000  .rg...ro...r$...
+00001a60: 7225 0000 0072 6900 0000 da04 636f 7079  r%...ri.....copy
 00001a70: 2904 7216 0000 00da 0673 6f75 7263 65da  ).r......source.
-00001a80: 0b64 6573 7469 6e61 7469 6f6e 726d 0000  .destinationrm..
+00001a80: 0b64 6573 7469 6e61 7469 6f6e 726c 0000  .destinationrl..
 00001a90: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
 00001aa0: da02 6370 3a01 0000 730a 0000 0000 010c  ..cp:...s.......
 00001ab0: 0104 020a 0110 017a 0a43 6f6e 7465 7874  .......z.Context
 00001ac0: 2e63 70fa 0277 2b63 0500 0000 0000 0000  .cp..w+c........
 00001ad0: 0000 0000 0600 0000 0800 0000 4300 0000  ............C...
 00001ae0: 7356 0000 007c 006a 006a 0172 107c 0473  sV...|.j.j.r.|.s
 00001af0: 1064 0053 007c 006a 02a0 0364 017c 01a1  .d.S.|.j...d.|..
 00001b00: 0201 0074 047c 017c 0383 028f 1a7d 057c  ...t.|.|.....}.|
 00001b10: 05a0 057c 02a1 0101 0057 0064 0004 0004  ...|.....W.d....
 00001b20: 0083 0301 006e 1031 0073 4830 0001 0001  .....n.1.sH0....
 00001b30: 0001 0059 0001 0064 0053 0029 024e 7a0b  ...Y...d.S.).Nz.
 00001b40: 7772 6974 696e 6720 2725 7329 0672 1300  writing '%s).r..
-00001b50: 0000 7268 0000 0072 2400 0000 7225 0000  ..rh...r$...r%..
+00001b50: 0000 7267 0000 0072 2400 0000 7225 0000  ..rg...r$...r%..
 00001b60: 00da 046f 7065 6eda 0577 7269 7465 2906  ...open..write).
 00001b70: 7216 0000 0072 2b00 0000 da04 7465 7874  r....r+.....text
-00001b80: da04 6d6f 6465 726d 0000 00da 0166 7219  ..moderm.....fr.
-00001b90: 0000 0072 1900 0000 721a 0000 0072 7700  ...r....r....rw.
+00001b80: da04 6d6f 6465 726c 0000 00da 0166 7219  ..moderl.....fr.
+00001b90: 0000 0072 1900 0000 721a 0000 0072 7600  ...r....r....rv.
 00001ba0: 0000 4201 0000 730a 0000 0000 010c 0104  ..B...s.........
 00001bb0: 020e 020c 017a 0d43 6f6e 7465 7874 2e77  .....z.Context.w
 00001bc0: 7269 7465 6303 0000 0000 0000 0000 0000  ritec...........
 00001bd0: 0004 0000 0006 0000 004b 0000 0073 2000  .........K...s .
 00001be0: 0000 7c02 7008 7c00 6a00 7d02 7401 6600  ..|.p.|.j.}.t.f.
 00001bf0: 7c01 7c00 7c02 6401 9c03 7c03 a401 8e01  |.|.|.d...|.....
 00001c00: 5300 2902 4e29 0372 5800 0000 721d 0000  S.).N).rX...r...
@@ -463,50 +463,50 @@
 00001ce0: 8d01 740b 7c00 6a03 6a08 6403 8d01 4200  ..t.|.j.j.d...B.
 00001cf0: a101 7d02 6e06 7c00 6a09 7d02 7c02 4400  ..}.n.|.j.}.|.D.
 00001d00: 5d36 7d03 7400 6a01 a00c 7c00 6a03 6a04  ]6}.t.j...|.j.j.
 00001d10: 7c03 6404 1900 a102 7d04 7c00 a00d 7c04  |.d.....}.|...|.
 00001d20: a101 0100 7c00 a00e 7c04 7c00 a00f 7c03  ....|...|.|...|.
 00001d30: a101 a102 0100 7166 7c00 6a06 a007 6405  ......qf|.j...d.
 00001d40: a101 0100 6400 5300 2906 4eda 0970 7265  ....d.S.).N..pre
-00001d50: 5f62 7569 6c64 2901 da08 7061 7468 5f5f  _build)...path__
-00001d60: 696e 2901 da0d 6931 386e 5f70 6174 685f  in)...i18n_path_
-00001d70: 5f69 6e72 6700 0000 da0a 706f 7374 5f62  _inrg.....post_b
+00001d50: 5f62 7569 6c64 2901 5a08 7061 7468 5f5f  _build).Z.path__
+00001d60: 696e 2901 5a0d 6931 386e 5f70 6174 685f  in).Z.i18n_path_
+00001d70: 5f69 6e72 6600 0000 da0a 706f 7374 5f62  _inrf.....post_b
 00001d80: 7569 6c64 2910 722d 0000 0072 2b00 0000  uild).r-...r+...
 00001d90: 7231 0000 0072 1300 0000 da0b 4f55 5450  r1...r......OUTP
-00001da0: 5554 5f52 4f4f 5472 6e00 0000 7214 0000  UT_ROOTrn...r...
+00001da0: 5554 5f52 4f4f 5472 6d00 0000 7214 0000  UT_ROOTrm...r...
 00001db0: 0072 2600 0000 724f 0000 0072 1000 0000  .r&...rO...r....
 00001dc0: 7230 0000 0072 0600 0000 722e 0000 0072  r0...r....r....r
-00001dd0: 7000 0000 7277 0000 0072 6400 0000 2905  p...rw...rd...).
+00001dd0: 6f00 0000 7276 0000 0072 6400 0000 2905  o...rv...rd...).
 00001de0: 7216 0000 00da 0563 6c65 616e 7210 0000  r......cleanr...
 00001df0: 0072 0f00 0000 5a0b 6f75 7470 7574 5f70  .r....Z.output_p
 00001e00: 6174 6872 1900 0000 7219 0000 0072 1a00  athr....r....r..
 00001e10: 0000 da05 6275 696c 6451 0100 0073 2200  ....buildQ...s".
 00001e20: 0000 0002 1401 0e03 0c03 0801 0601 0c01  ................
 00001e30: 0cff 02ff 0606 0602 0801 0c01 06ff 0403  ................
 00001e40: 0a01 1402 7a0d 436f 6e74 6578 742e 6275  ....z.Context.bu
 00001e50: 696c 6429 024e 5429 014e 2901 4e29 0172  ild).NT).N).N).r
 00001e60: 5f00 0000 2901 4629 0146 2901 4629 0272  _...).F).F).F).r
-00001e70: 7500 0000 4629 014e 2901 5429 16da 085f  u...F).N).T)..._
+00001e70: 7400 0000 4629 014e 2901 5429 16da 085f  t...F).N).T)..._
 00001e80: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
 00001e90: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
 00001ea0: 5f5a 235f 436f 6e74 6578 745f 5f6f 7665  _Z#_Context__ove
 00001eb0: 726c 6179 5f69 676e 6f72 655f 6174 7472  rlay_ignore_attr
 00001ec0: 6962 7574 6573 7212 0000 0072 1500 0000  ibutesr....r....
 00001ed0: 723d 0000 00da 0870 726f 7065 7274 7972  r=.....propertyr
 00001ee0: 4000 0000 7245 0000 0072 2a00 0000 724d  @...rE...r*...rM
 00001ef0: 0000 0072 5a00 0000 7261 0000 0072 6400  ...rZ...ra...rd.
-00001f00: 0000 726e 0000 0072 7000 0000 7274 0000  ..rn...rp...rt..
-00001f10: 0072 7700 0000 720b 0000 0072 8200 0000  .rw...r....r....
+00001f00: 0000 726d 0000 0072 6f00 0000 7273 0000  ..rm...ro...rs..
+00001f10: 0072 7600 0000 720b 0000 0072 7f00 0000  .rv...r....r....
 00001f20: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
 00001f30: 1900 0000 7219 0000 0072 1700 0000 721a  ....r....r....r.
 00001f40: 0000 0072 0e00 0000 0d00 0000 7328 0000  ...r........s(..
 00001f50: 0008 0202 0102 fe04 050e 0b08 200a 2e02  ............ ...
 00001f60: 010a 0c08 2508 1108 2b08 0c0a 1d0a 210a  ....%...+.....!.
 00001f70: 0c0a 0a0a 080a 090a 0672 0e00 0000 2916  .........r....).
-00001f80: 7222 0000 0072 6a00 0000 722d 0000 00da  r"...rj...r-....
+00001f80: 7222 0000 0072 6900 0000 722d 0000 00da  r"...ri...r-....
 00001f90: 1866 6c61 6d69 6e67 6f2e 636f 7265 2e64  .flamingo.core.d
 00001fa0: 6174 615f 6d6f 6465 6c72 0200 0000 7203  ata_modelr....r.
 00001fb0: 0000 0072 0400 0000 7205 0000 0072 0600  ...r....r....r..
 00001fc0: 0000 7207 0000 00da 2466 6c61 6d69 6e67  ..r.....$flaming
 00001fd0: 6f2e 636f 7265 2e70 6c75 6769 6e73 2e70  o.core.plugins.p
 00001fe0: 6c75 6769 6e5f 6d61 6e61 6765 7272 0800  lugin_managerr..
 00001ff0: 0000 5a14 666c 616d 696e 676f 2e63 6f72  ..Z.flamingo.cor
```

### Comparing `flamingo-1.8/flamingo/core/__pycache__/data_model.cpython-310.pyc` & `flamingo-1.9/flamingo/core/__pycache__/data_model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/__pycache__/data_model.cpython-35.pyc` & `flamingo-1.9/flamingo/core/__pycache__/data_model.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/__pycache__/data_model.cpython-37.pyc` & `flamingo-1.9/flamingo/core/__pycache__/data_model.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/__pycache__/data_model.cpython-39.pyc` & `flamingo-1.9/flamingo/core/__pycache__/data_model.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/__pycache__/errors.cpython-310.pyc` & `flamingo-1.9/flamingo/core/__pycache__/errors.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/__pycache__/errors.cpython-35.pyc` & `flamingo-1.9/flamingo/core/__pycache__/errors.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/__pycache__/errors.cpython-37.pyc` & `flamingo-1.9/flamingo/core/__pycache__/errors.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/__pycache__/errors.cpython-39.pyc` & `flamingo-1.9/flamingo/core/__pycache__/errors.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/__pycache__/parser.cpython-310.pyc` & `flamingo-1.9/flamingo/core/__pycache__/parser.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/__pycache__/parser.cpython-35.pyc` & `flamingo-1.9/flamingo/core/__pycache__/parser.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/__pycache__/parser.cpython-37.pyc` & `flamingo-1.9/flamingo/core/__pycache__/parser.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/__pycache__/parser.cpython-39.pyc` & `flamingo-1.9/flamingo/core/__pycache__/parser.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/__pycache__/settings.cpython-35.pyc` & `flamingo-1.9/flamingo/core/__pycache__/settings.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/__pycache__/types.cpython-310.pyc` & `flamingo-1.9/flamingo/core/__pycache__/types.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/__pycache__/types.cpython-35.pyc` & `flamingo-1.9/flamingo/core/__pycache__/types.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/__pycache__/types.cpython-37.pyc` & `flamingo-1.9/flamingo/core/__pycache__/types.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/__pycache__/types.cpython-39.pyc` & `flamingo-1.9/flamingo/core/__pycache__/types.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/context.py` & `flamingo-1.9/flamingo/core/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,16 +224,16 @@
             'Q': Q,
             'F': F,
             **self.settings.EXTRA_CONTEXT,
             **extra_context,
         }
 
     def pre_render(self, content, template_context=None):
-        if(not self.settings.PRE_RENDER_CONTENT or
-           not content.get('is_template', True) or
+        if (not self.settings.PRE_RENDER_CONTENT or
+            not content.get('is_template', True) or
            content['_content_body_rendered']):
 
             return True, content['content_body']
 
         self.logger.debug('pre rendering %s', content['path'] or content)
 
         if template_context is None:
```

### Comparing `flamingo-1.8/flamingo/core/data_model.py` & `flamingo-1.9/flamingo/core/data_model.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/errors.py` & `flamingo-1.9/flamingo/core/errors.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/parser.py` & `flamingo-1.9/flamingo/core/parser.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/plugins/__pycache__/layers.cpython-310.pyc` & `flamingo-1.9/flamingo/core/plugins/__pycache__/layers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/plugins/__pycache__/layers.cpython-35.pyc` & `flamingo-1.9/flamingo/core/plugins/__pycache__/layers.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/plugins/__pycache__/layers.cpython-37.pyc` & `flamingo-1.9/flamingo/core/plugins/__pycache__/layers.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/plugins/__pycache__/layers.cpython-39.pyc` & `flamingo-1.9/flamingo/core/plugins/__pycache__/layers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/plugins/__pycache__/media.cpython-310.pyc` & `flamingo-1.9/flamingo/core/plugins/__pycache__/media.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/plugins/__pycache__/media.cpython-35.pyc` & `flamingo-1.9/flamingo/core/plugins/__pycache__/media.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/plugins/__pycache__/media.cpython-37.pyc` & `flamingo-1.9/flamingo/core/plugins/__pycache__/media.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/plugins/__pycache__/media.cpython-39.pyc` & `flamingo-1.9/flamingo/core/plugins/__pycache__/media.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/plugins/__pycache__/meta_data.cpython-310.pyc` & `flamingo-1.9/flamingo/core/plugins/__pycache__/meta_data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/plugins/__pycache__/meta_data.cpython-35.pyc` & `flamingo-1.9/flamingo/core/plugins/__pycache__/meta_data.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/plugins/__pycache__/meta_data.cpython-37.pyc` & `flamingo-1.9/flamingo/core/plugins/__pycache__/meta_data.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/plugins/__pycache__/meta_data.cpython-39.pyc` & `flamingo-1.9/flamingo/core/plugins/__pycache__/meta_data.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/plugins/__pycache__/plugin_manager.cpython-310.pyc` & `flamingo-1.9/flamingo/core/plugins/__pycache__/plugin_manager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/plugins/__pycache__/plugin_manager.cpython-35.pyc` & `flamingo-1.9/flamingo/core/plugins/__pycache__/plugin_manager.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/plugins/__pycache__/plugin_manager.cpython-37.pyc` & `flamingo-1.9/flamingo/core/plugins/__pycache__/plugin_manager.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/plugins/__pycache__/plugin_manager.cpython-39.pyc` & `flamingo-1.9/flamingo/core/plugins/__pycache__/plugin_manager.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Dec  6 19:14:04 2021 UTC, .py size: 10172 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-00000000: 610d 0d0a 0000 0000 fc60 ae61 bc27 0000  a........`.a.'..
+00000000: 610d 0d0a 0000 0000 5399 7c63 c927 0000  a.......S.|c.'..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6500 a003 6403 a101 5a04 6700 6404  ..e...d...Z.g.d.
 00000050: a201 5a05 6405 6406 8400 5a06 4700 6407  ..Z.d.d...Z.G.d.
 00000060: 6408 8400 6408 8302 5a07 4700 6409 640a  d...d...Z.G.d.d.
 00000070: 8400 640a 8302 5a08 6401 5300 290b e900  ..d...Z.d.S.)...
 00000080: 0000 004e 2901 da07 6163 7175 6972 657a  ...N)...acquirez
 00000090: 1b66 6c61 6d69 6e67 6f2e 636f 7265 2e50  .flamingo.core.P
-000000a0: 6c75 6769 6e4d 616e 6167 6572 290c da05  luginManager)...
+000000a0: 6c75 6769 6e4d 616e 6167 6572 290c 5a05  luginManager).Z.
 000000b0: 7365 7475 705a 0e73 6574 7469 6e67 735f  setupZ.settings_
 000000c0: 7365 7475 705a 0c70 6172 7365 725f 7365  setupZ.parser_se
 000000d0: 7475 705a 1774 656d 706c 6174 696e 675f  tupZ.templating_
 000000e0: 656e 6769 6e65 5f73 6574 7570 5a0e 636f  engine_setupZ.co
 000000f0: 6e74 656e 745f 7061 7273 6564 da0f 636f  ntent_parsed..co
 00000100: 6e74 656e 7473 5f70 6172 7365 645a 0d63  ntents_parsedZ.c
 00000110: 6f6e 7465 7874 5f73 6574 7570 5a09 7072  ontext_setupZ.pr
@@ -33,27 +33,27 @@
 00000200: 2f50 726f 6a65 6374 732f 6769 7468 7562  /Projects/github
 00000210: 2f66 6c61 6d69 6e67 6f2f 666c 616d 696e  /flamingo/flamin
 00000220: 676f 2f63 6f72 652f 706c 7567 696e 732f  go/core/plugins/
 00000230: 706c 7567 696e 5f6d 616e 6167 6572 2e70  plugin_manager.p
 00000240: 79da 0964 6563 6f72 6174 6f72 1c00 0000  y..decorator....
 00000250: 7304 0000 0000 0106 027a 1768 6f6f 6b2e  s........z.hook.
 00000260: 3c6c 6f63 616c 733e 2e64 6563 6f72 6174  <locals>.decorat
-00000270: 6f72 720c 0000 0029 0272 0b00 0000 720e  orr....).r....r.
-00000280: 0000 0072 0c00 0000 720a 0000 0072 0d00  ...r....r....r..
+00000270: 6f72 720b 0000 0029 0272 0a00 0000 720d  orr....).r....r.
+00000280: 0000 0072 0b00 0000 7209 0000 0072 0c00  ...r....r....r..
 00000290: 0000 da04 686f 6f6b 1b00 0000 7304 0000  ....hook....s...
-000002a0: 0000 010c 0572 0f00 0000 6300 0000 0000  .....r....c.....
+000002a0: 0000 010c 0572 0e00 0000 6300 0000 0000  .....r....c.....
 000002b0: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
 000002c0: 0000 0073 0c00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
 000002d0: 6401 5300 2902 da0c 5365 7474 696e 6773  d.S.)...Settings
 000002e0: 486f 6f6b 4e29 03da 085f 5f6e 616d 655f  HookN)...__name_
 000002f0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000300: 5f71 7561 6c6e 616d 655f 5f72 0c00 0000  _qualname__r....
-00000310: 720c 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
-00000320: 1000 0000 2400 0000 7302 0000 0008 0172  ....$...s......r
-00000330: 1000 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000300: 5f71 7561 6c6e 616d 655f 5f72 0b00 0000  _qualname__r....
+00000310: 720b 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
+00000320: 0f00 0000 2400 0000 7302 0000 0008 0172  ....$...s......r
+00000330: 0f00 0000 6300 0000 0000 0000 0000 0000  ....c...........
 00000340: 0000 0000 0003 0000 0000 0000 0073 8000  .............s..
 00000350: 0000 6500 5a01 6400 5a02 6401 6402 8400  ..e.Z.d.Z.d.d...
 00000360: 5a03 8700 6601 6403 6404 8408 5a04 8700  Z...f.d.d...Z...
 00000370: 6601 6405 6406 8408 5a05 6407 6408 8400  f.d.d...Z.d.d...
 00000380: 5a06 6507 6409 640a 8400 8301 5a08 6507  Z.e.d.d.....Z.e.
 00000390: 640b 640c 8400 8301 5a09 640d 640e 8400  d.d.....Z.d.d...
 000003a0: 5a0a 640f 6410 8400 5a0b 6411 6412 8400  Z.d.d...Z.d.d...
@@ -88,15 +88,15 @@
 00000570: 0059 0071 5630 0071 567c 00a0 1b74 1ca1  .Y.qV0.qV|...t..
 00000580: 0101 0064 0053 0029 0c4e da00 7a17 7365  ...d.S.).N..z.se
 00000590: 7474 696e 6720 7570 2070 6c75 6769 6e20  tting up plugin 
 000005a0: 2725 7327 20da 012e 7a22 2725 7327 2067  '%s' ...z"'%s' g
 000005b0: 6574 7320 6861 6e64 6c65 6420 6173 2073  ets handled as s
 000005c0: 6574 7469 6e67 7320 686f 6f6b e901 0000  ettings hook....
 000005d0: 007a 1a73 6574 7469 6e67 732e 2573 2064  .z.settings.%s d
-000005e0: 6f65 7320 6e6f 7420 6578 6973 7472 0800  oes not existr..
+000005e0: 6f65 7320 6e6f 7420 6578 6973 7472 0700  oes not existr..
 000005f0: 0000 7a1f 7365 7474 696e 6773 2e25 7320  ..z.settings.%s 
 00000600: 6973 206e 6f20 666c 616d 696e 676f 2068  is no flamingo h
 00000610: 6f6f 6b7a 1473 6574 7570 206f 6620 2725  ookz.setup of '%
 00000620: 7327 2066 6169 6c65 6454 a901 da08 6578  s' failedT....ex
 00000630: 635f 696e 666f 291d da08 5f63 6f6e 7465  c_info)..._conte
 00000640: 7874 da08 5f70 6c75 6769 6e73 5a0d 5f70  xt.._pluginsZ._p
 00000650: 6c75 6769 6e5f 7061 7468 73da 065f 686f  lugin_paths.._ho
@@ -107,27 +107,27 @@
 000006a0: 535f 5052 455a 0f44 4546 4155 4c54 5f50  S_PREZ.DEFAULT_P
 000006b0: 4c55 4749 4e53 5a07 504c 5547 494e 535a  LUGINSZ.PLUGINSZ
 000006c0: 1143 4f52 455f 504c 5547 494e 535f 504f  .CORE_PLUGINS_PO
 000006d0: 5354 da06 6c6f 6767 6572 da05 6465 6275  ST..logger..debu
 000006e0: 67da 0a69 7369 6e73 7461 6e63 65da 0373  g..isinstance..s
 000006f0: 7472 da0a 7374 6172 7473 7769 7468 da07  tr..startswith..
 00000700: 6861 7361 7474 72da 0565 7272 6f72 da07  hasattr..error..
-00000710: 6765 7461 7474 7272 1000 0000 da07 7365  getattrr......se
-00000720: 7461 7474 72da 0661 7070 656e 6472 1100  tattr..appendr..
+00000710: 6765 7461 7474 7272 0f00 0000 da07 7365  getattrr......se
+00000720: 7461 7474 72da 0661 7070 656e 6472 1000  tattr..appendr..
 00000730: 0000 7202 0000 00da 095f 5f63 6c61 7373  ..r......__class
 00000740: 5f5f da09 4578 6365 7074 696f 6eda 095f  __..Exception.._
 00000750: 6469 7363 6f76 6572 da0a 484f 4f4b 5f4e  discover..HOOK_N
 00000760: 414d 4553 290a da04 7365 6c66 da07 636f  AMES)...self..co
 00000770: 6e74 6578 74da 0770 6c75 6769 6e73 5a06  ntext..pluginsZ.
-00000780: 706c 7567 696e 720f 0000 005a 0d73 6574  pluginr....Z.set
+00000780: 706c 7567 696e 720e 0000 005a 0d73 6574  pluginr....Z.set
 00000790: 7469 6e67 735f 686f 6f6b da09 686f 6f6b  tings_hook..hook
 000007a0: 5f6e 616d 655a 0c70 6c75 6769 6e5f 636c  _nameZ.plugin_cl
 000007b0: 6173 73da 0b70 6c75 6769 6e5f 7061 7468  ass..plugin_path
 000007c0: da0d 706c 7567 696e 5f6f 626a 6563 7472  ..plugin_objectr
-000007d0: 0c00 0000 720c 0000 0072 0d00 0000 da08  ....r....r......
+000007d0: 0b00 0000 720b 0000 0072 0c00 0000 da08  ....r....r......
 000007e0: 5f5f 696e 6974 5f5f 2900 0000 7356 0000  __init__)...sV..
 000007f0: 0000 0106 0106 0106 0106 0106 0206 0206  ................
 00000800: 0308 0108 ff02 0208 fe02 0308 fd04 050a  ................
 00000810: 010c 0202 0218 010c 020c 020e 010c 0204  ................
 00000820: 020e 020a 010c 0204 0206 020a 010c 0206  ................
 00000830: 0108 ff06 060c 0106 020c 0206 010a ff04  ................
 00000840: 0410 020e 0118 027a 1650 6c75 6769 6e4d  .......z.PluginM
@@ -135,36 +135,36 @@
 00000860: 0100 0000 0000 0000 0000 0000 0100 0000  ................
 00000870: 0300 0000 0300 0000 731e 0000 0067 0074  ........s....g.t
 00000880: 0083 00a0 01a1 00a2 0164 0164 0284 007c  .........d.d...|
 00000890: 006a 0244 0083 01a2 0153 0029 034e 6301  .j.D.....S.).Nc.
 000008a0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
 000008b0: 0000 0053 0000 0073 1400 0000 6700 7c00  ...S...s....g.|.
 000008c0: 5d0c 7d01 7c01 6400 1900 9102 7104 5300  ].}.|.d.....q.S.
-000008d0: 2901 7201 0000 0072 0c00 0000 2902 da02  ).r....r....)...
-000008e0: 2e30 da01 6972 0c00 0000 720c 0000 0072  .0..ir....r....r
-000008f0: 0d00 0000 da0a 3c6c 6973 7463 6f6d 703e  ......<listcomp>
+000008d0: 2901 7201 0000 0072 0b00 0000 2902 da02  ).r....r....)...
+000008e0: 2e30 da01 6972 0b00 0000 720b 0000 0072  .0..ir....r....r
+000008f0: 0c00 0000 da0a 3c6c 6973 7463 6f6d 703e  ......<listcomp>
 00000900: 6e00 0000 f300 0000 007a 2950 6c75 6769  n........z)Plugi
 00000910: 6e4d 616e 6167 6572 2e5f 5f64 6972 5f5f  nManager.__dir__
 00000920: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
 00000930: 6f6d 703e 2903 da05 7375 7065 72da 075f  omp>)...super.._
-00000940: 5f64 6972 5f5f 721b 0000 00a9 0172 2e00  _dir__r......r..
-00000950: 0000 a901 722a 0000 0072 0c00 0000 720d  ....r*...r....r.
-00000960: 0000 0072 3a00 0000 6b00 0000 730a 0000  ...r:...k...s...
+00000940: 5f64 6972 5f5f 721a 0000 00a9 0172 2d00  _dir__r......r-.
+00000950: 0000 a901 7229 0000 0072 0b00 0000 720c  ....r)...r....r.
+00000960: 0000 0072 3900 0000 6b00 0000 730a 0000  ...r9...k...s...
 00000970: 0000 0102 0108 ff02 020e fe7a 1550 6c75  ...........z.Plu
 00000980: 6769 6e4d 616e 6167 6572 2e5f 5f64 6972  ginManager.__dir
 00000990: 5f5f 6302 0000 0000 0000 0000 0000 0004  __c.............
 000009a0: 0000 0003 0000 0003 0000 0073 2c00 0000  ...........s,...
 000009b0: 7c00 6a00 4400 5d18 5c02 7d02 7d03 7c01  |.j.D.].\.}.}.|.
 000009c0: 7c02 6b02 7206 7c03 0200 0100 5300 7106  |.k.r.|.....S.q.
-000009d0: 7401 8300 a002 7c01 a101 5300 7207 0000  t.....|...S.r...
-000009e0: 0029 0372 1b00 0000 7239 0000 00da 0b5f  .).r....r9....._
-000009f0: 5f67 6574 6174 7472 5f5f a904 722e 0000  _getattr__..r...
-00000a00: 0072 0b00 0000 da0b 706c 7567 696e 5f6e  .r......plugin_n
-00000a10: 616d 6572 3300 0000 723c 0000 0072 0c00  amer3...r<...r..
-00000a20: 0000 720d 0000 0072 3d00 0000 7100 0000  ..r....r=...q...
+000009d0: 7401 8300 a002 7c01 a101 5300 7206 0000  t.....|...S.r...
+000009e0: 0029 0372 1a00 0000 7238 0000 00da 0b5f  .).r....r8....._
+000009f0: 5f67 6574 6174 7472 5f5f a904 722d 0000  _getattr__..r-..
+00000a00: 0072 0a00 0000 da0b 706c 7567 696e 5f6e  .r......plugin_n
+00000a10: 616d 6572 3200 0000 723b 0000 0072 0b00  amer2...r;...r..
+00000a20: 0000 720c 0000 0072 3c00 0000 7100 0000  ..r....r<...q...
 00000a30: 7308 0000 0000 010e 0108 010a 027a 1950  s............z.P
 00000a40: 6c75 6769 6e4d 616e 6167 6572 2e5f 5f67  luginManager.__g
 00000a50: 6574 6174 7472 5f5f 6302 0000 0000 0000  etattr__c.......
 00000a60: 0000 0000 0008 0000 0008 0000 0043 0000  .............C..
 00000a70: 0073 0001 0000 6700 7d02 7c01 4400 5d22  .s....g.}.|.D.]"
 00000a80: 7d03 7c03 7c00 6a00 7601 7208 7c02 a001  }.|.|.j.v.r.|...
 00000a90: 7c03 a101 0100 6700 7c00 6a00 7c03 3c00  |.....g.|.j.|.<.
@@ -182,50 +182,50 @@
 00000b50: 6405 7c07 6a0c a102 0100 7c00 6a00 7c07  d.|.j.....|.j.|.
 00000b60: 6a0c 1900 a001 6406 7c07 6602 a101 0100  j.....d.|.f.....
 00000b70: 719e 6400 5300 2907 4e7a 1873 6561 7263  q.d.S.).Nz.searc
 00000b80: 6869 6e67 2066 6f72 2027 2573 2720 686f  hing for '%s' ho
 00000b90: 6f6b 737a 0f25 732e 2573 2064 6973 636f  oksz.%s.%s disco
 00000ba0: 7665 7264 7a1c 7365 6172 6368 696e 6720  verdz.searching 
 00000bb0: 666f 7220 7365 7474 696e 6773 2068 6f6f  for settings hoo
-00000bc0: 6b73 7208 0000 007a 1873 6574 7469 6e67  ksr....z.setting
+00000bc0: 6b73 7207 0000 007a 1873 6574 7469 6e67  ksr....z.setting
 00000bd0: 732e 2573 2064 6973 636f 7665 7264 2061  s.%s discoverd a
-00000be0: 7372 1f00 0000 290d 721c 0000 0072 2900  sr....).r....r).
-00000bf0: 0000 7220 0000 0072 2100 0000 721b 0000  ..r ...r!...r...
-00000c00: 0072 2500 0000 722a 0000 0072 1100 0000  .r%...r*...r....
-00000c10: 7227 0000 00da 0364 6972 721a 0000 0072  r'.....dirr....r
-00000c20: 1f00 0000 7208 0000 0029 0872 2e00 0000  ....r....).r....
+00000be0: 7372 1e00 0000 290d 721b 0000 0072 2800  sr....).r....r(.
+00000bf0: 0000 721f 0000 0072 2000 0000 721a 0000  ..r....r ...r...
+00000c00: 0072 2400 0000 7229 0000 0072 1000 0000  .r$...r)...r....
+00000c10: 7226 0000 00da 0364 6972 7219 0000 0072  r&.....dirr....r
+00000c20: 1e00 0000 7207 0000 0029 0872 2d00 0000  ....r....).r-...
 00000c30: da05 6e61 6d65 735a 1668 6f6f 6b5f 6e61  ..namesZ.hook_na
 00000c40: 6d65 735f 746f 5f64 6973 636f 7665 7272  mes_to_discoverr
-00000c50: 3100 0000 7232 0000 0072 3300 0000 da09  1...r2...r3.....
+00000c50: 3000 0000 7231 0000 0072 3200 0000 da09  0...r1...r2.....
 00000c60: 6174 7472 5f6e 616d 65da 0461 7474 7272  attr_name..attrr
-00000c70: 0c00 0000 720c 0000 0072 0d00 0000 722c  ....r....r....r,
+00000c70: 0b00 0000 720b 0000 0072 0c00 0000 722b  ....r....r....r+
 00000c80: 0000 0078 0000 0073 3800 0000 0001 0402  ...x...s8.......
 00000c90: 0801 0a01 0a01 0c02 0801 0c02 0e01 0a01  ................
 00000ca0: 0e02 0a01 0601 08ff 02ff 0806 0a02 1001  ................
 00000cb0: 0e02 0a01 08ff 0202 0efe 0204 0202 0e02  ................
 00000cc0: 0c01 06ff 7a17 506c 7567 696e 4d61 6e61  ....z.PluginMana
 00000cd0: 6765 722e 5f64 6973 636f 7665 7263 0100  ger._discoverc..
 00000ce0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
 00000cf0: 0000 4300 0000 7306 0000 007c 006a 0053  ..C...s....|.j.S
-00000d00: 0072 0700 0000 2901 721d 0000 0072 3b00  .r....).r....r;.
-00000d10: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+00000d00: 0072 0600 0000 2901 721c 0000 0072 3a00  .r....).r....r:.
+00000d10: 0000 720b 0000 0072 0b00 0000 720c 0000  ..r....r....r...
 00000d20: 00da 0c72 756e 6e69 6e67 5f68 6f6f 6b9e  ...running_hook.
 00000d30: 0000 0073 0200 0000 0002 7a1a 506c 7567  ...s......z.Plug
 00000d40: 696e 4d61 6e61 6765 722e 7275 6e6e 696e  inManager.runnin
 00000d50: 675f 686f 6f6b 6301 0000 0000 0000 0000  g_hookc.........
 00000d60: 0000 0004 0000 0004 0000 0043 0000 0073  ...........C...s
 00000d70: 2e00 0000 6700 7d01 7c00 6a00 4400 5d1e  ....g.}.|.j.D.].
 00000d80: 5c02 7d02 7d03 7401 7c03 6401 8302 720a  \.}.}.t.|.d...r.
 00000d90: 7c01 a002 7c03 6a03 a101 0100 710a 7c01  |...|.j.....q.|.
 00000da0: 5300 2902 4eda 0b54 4845 4d45 5f50 4154  S.).N..THEME_PAT
-00000db0: 4853 2904 721b 0000 0072 2500 0000 da06  HS).r....r%.....
-00000dc0: 6578 7465 6e64 7245 0000 0029 0472 2e00  extendrE...).r..
-00000dd0: 0000 da05 7061 7468 7372 3200 0000 7233  ....pathsr2...r3
-00000de0: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
-00000df0: 0000 7245 0000 00a2 0000 0073 0a00 0000  ..rE.......s....
+00000db0: 4853 2904 721a 0000 0072 2400 0000 da06  HS).r....r$.....
+00000dc0: 6578 7465 6e64 7244 0000 0029 0472 2d00  extendrD...).r-.
+00000dd0: 0000 da05 7061 7468 7372 3100 0000 7232  ....pathsr1...r2
+00000de0: 0000 0072 0b00 0000 720b 0000 0072 0c00  ...r....r....r..
+00000df0: 0000 7244 0000 00a2 0000 0073 0a00 0000  ..rD.......s....
 00000e00: 0002 0402 0e01 0a01 0e02 7a19 506c 7567  ..........z.Plug
 00000e10: 696e 4d61 6e61 6765 722e 5448 454d 455f  inManager.THEME_
 00000e20: 5041 5448 5363 0200 0000 0000 0000 0000  PATHSc..........
 00000e30: 0000 0600 0000 0a00 0000 4f00 0000 73f2  ..........O...s.
 00000e40: 0000 007c 017c 006a 006a 016a 0276 0072  ...|.|.j.j.j.v.r
 00000e50: 1e74 03a0 0464 017c 01a1 0201 0064 0053  .t...d.|.....d.S
 00000e60: 007c 017c 006a 0576 0172 347c 00a0 067c  .|.|.j.v.r4|...|
@@ -242,50 +242,50 @@
 00000f10: 0071 8057 0064 097c 005f 0764 007c 005f  .q.W.d.|._.d.|._
 00000f20: 086e 0e64 097c 005f 0764 007c 005f 0830  .n.d.|._.d.|._.0
 00000f30: 0064 0053 0029 0a4e 7a2b 2725 7327 2073  .d.S.).Nz+'%s' s
 00000f40: 6b69 7070 6564 2062 6563 6175 7365 206f  kipped because o
 00000f50: 6620 7365 7474 696e 6773 2e53 4b49 505f  f settings.SKIP_
 00000f60: 484f 4f4b 537a 1872 756e 6e69 6e67 2070  HOOKSz.running p
 00000f70: 6c75 6769 6e20 686f 6f6b 2027 2573 2772  lugin hook '%s'r
-00000f80: 0600 0000 7201 0000 007a 0d72 756e 6e69  ....r....z.runni
+00000f80: 0500 0000 7201 0000 007a 0d72 756e 6e69  ....r....z.runni
 00000f90: 6e67 2025 732e 2573 7a0c 2573 2e25 7320  ng %s.%sz.%s.%s 
-00000fa0: 6661 696c 6564 5472 1800 0000 7215 0000  failedTr....r...
-00000fb0: 0029 0b72 1a00 0000 721f 0000 005a 0a53  .).r....r....Z.S
-00000fc0: 4b49 505f 484f 4f4b 5372 2000 0000 7221  KIP_HOOKSr ...r!
-00000fd0: 0000 0072 1c00 0000 722c 0000 0072 1d00  ...r....r,...r..
-00000fe0: 0000 721e 0000 0072 2b00 0000 7226 0000  ..r....r+...r&..
-00000ff0: 0029 0672 2e00 0000 720b 0000 00da 0461  .).r....r......a
-00001000: 7267 73da 066b 7761 7267 7372 3f00 0000  rgs..kwargsr?...
-00001010: 720f 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
-00001020: 0d00 0000 da0f 7275 6e5f 706c 7567 696e  ......run_plugin
+00000fa0: 6661 696c 6564 5472 1700 0000 7214 0000  failedTr....r...
+00000fb0: 0029 0b72 1900 0000 721e 0000 005a 0a53  .).r....r....Z.S
+00000fc0: 4b49 505f 484f 4f4b 5372 1f00 0000 7220  KIP_HOOKSr....r 
+00000fd0: 0000 0072 1b00 0000 722b 0000 0072 1c00  ...r....r+...r..
+00000fe0: 0000 721d 0000 0072 2a00 0000 7225 0000  ..r....r*...r%..
+00000ff0: 0029 0672 2d00 0000 720a 0000 00da 0461  .).r-...r......a
+00001000: 7267 73da 066b 7761 7267 7372 3e00 0000  rgs..kwargsr>...
+00001010: 720e 0000 0072 0b00 0000 720b 0000 0072  r....r....r....r
+00001020: 0c00 0000 da0f 7275 6e5f 706c 7567 696e  ......run_plugin
 00001030: 5f68 6f6f 6bac 0000 0073 3200 0000 0001  _hook....s2.....
 00001040: 0e01 0c02 0402 0a01 0c02 0a01 0402 0201  ................
 00001050: 0c01 0603 0801 0a02 0e02 1201 0e02 0201  ................
 00001060: 1202 0c01 0a01 02ff 1004 0601 08ff 0601  ................
 00001070: 7a1d 506c 7567 696e 4d61 6e61 6765 722e  z.PluginManager.
 00001080: 7275 6e5f 706c 7567 696e 5f68 6f6f 6b63  run_plugin_hookc
 00001090: 0200 0000 0000 0000 0000 0000 0400 0000  ................
 000010a0: 0400 0000 4300 0000 7332 0000 007c 006a  ....C...s2...|.j
 000010b0: 0044 005d 185c 027d 027d 037c 027c 016b  .D.].\.}.}.|.|.k
 000010c0: 0272 067c 0302 0001 0053 0071 0674 0164  .r.|.....S.q.t.d
 000010d0: 01a0 027c 01a1 0183 0182 0164 0053 0029  ...|.......d.S.)
 000010e0: 024e 7a13 756e 6b6e 6f77 6e20 706c 7567  .Nz.unknown plug
-000010f0: 696e 2027 7b7d 2729 0372 1b00 0000 da0a  in '{}').r......
+000010f0: 696e 2027 7b7d 2729 0372 1a00 0000 da0a  in '{}').r......
 00001100: 5661 6c75 6545 7272 6f72 da06 666f 726d  ValueError..form
-00001110: 6174 723e 0000 0072 0c00 0000 720c 0000  atr>...r....r...
-00001120: 0072 0d00 0000 da0a 6765 745f 706c 7567  .r......get_plug
+00001110: 6174 723d 0000 0072 0b00 0000 720b 0000  atr=...r....r...
+00001120: 0072 0c00 0000 da0a 6765 745f 706c 7567  .r......get_plug
 00001130: 696e d000 0000 7308 0000 0000 010e 0108  in....s.........
 00001140: 010a 027a 1850 6c75 6769 6e4d 616e 6167  ...z.PluginManag
 00001150: 6572 2e67 6574 5f70 6c75 6769 6e63 0100  er.get_pluginc..
 00001160: 0000 0000 0000 0000 0000 0300 0000 0400  ................
 00001170: 0000 4f00 0000 7310 0000 007c 006a 007c  ..O...s....|.j.|
-00001180: 0169 007c 02a4 018e 0153 0072 0700 0000  .i.|.....S.r....
-00001190: 2901 724a 0000 0029 0372 2e00 0000 7248  ).rJ...).r....rH
-000011a0: 0000 0072 4900 0000 720c 0000 0072 0c00  ...rI...r....r..
-000011b0: 0000 720d 0000 00da 0872 756e 5f68 6f6f  ..r......run_hoo
+00001180: 0169 007c 02a4 018e 0153 0072 0600 0000  .i.|.....S.r....
+00001190: 2901 7249 0000 0029 0372 2d00 0000 7247  ).rI...).r-...rG
+000011a0: 0000 0072 4800 0000 720b 0000 0072 0b00  ...rH...r....r..
+000011b0: 0000 720c 0000 00da 0872 756e 5f68 6f6f  ..r......run_hoo
 000011c0: 6bd7 0000 0073 0200 0000 0001 7a16 506c  k....s......z.Pl
 000011d0: 7567 696e 4d61 6e61 6765 722e 7275 6e5f  uginManager.run_
 000011e0: 686f 6f6b 6301 0000 0000 0000 0000 0000  hookc...........
 000011f0: 000b 0000 0009 0000 0043 0000 0073 8801  .........C...s..
 00001200: 0000 7400 7c00 6401 8302 739c 6700 7c00  ..t.|.d...s.g.|.
 00001210: 5f01 7c00 6a02 4400 5d70 5c02 7d01 7d02  _.|.j.D.]p\.}.}.
 00001220: 7400 7c02 6402 8302 7216 7403 7c02 6a04  t.|.d...r.t.|.j.
@@ -329,42 +329,42 @@
 00001480: 5d0a 2020 2020 2020 2020 da08 5f6f 7074  ].        .._opt
 00001490: 696f 6e73 da0b 6765 745f 6f70 7469 6f6e  ions..get_option
 000014a0: 73da 0a73 6574 5f6f 7074 696f 6eda 0d72  s..set_option..r
 000014b0: 6573 6574 5f6f 7074 696f 6e73 da10 6765  eset_options..ge
 000014c0: 745f 6f70 7469 6f6e 735f 6865 6c70 6301  t_options_helpc.
 000014d0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
 000014e0: 0000 0053 0000 0073 0800 0000 7c00 6401  ...S...s....|.d.
-000014f0: 1900 5300 2902 4e72 0100 0000 720c 0000  ..S.).Nr....r...
-00001500: 0029 01da 0176 720c 0000 0072 0c00 0000  .)...vr....r....
-00001510: 720d 0000 00da 083c 6c61 6d62 6461 3e09  r......<lambda>.
-00001520: 0100 0072 3800 0000 7a2b 506c 7567 696e  ...r8...z+Plugin
+000014f0: 1900 5300 2902 4e72 0100 0000 720b 0000  ..S.).Nr....r...
+00001500: 0029 01da 0176 720b 0000 0072 0b00 0000  .)...vr....r....
+00001510: 720c 0000 00da 083c 6c61 6d62 6461 3e09  r......<lambda>.
+00001520: 0100 0072 3700 0000 7a2b 506c 7567 696e  ...r7...z+Plugin
 00001530: 4d61 6e61 6765 722e 6765 745f 6f70 7469  Manager.get_opti
 00001540: 6f6e 732e 3c6c 6f63 616c 733e 2e3c 6c61  ons.<locals>.<la
 00001550: 6d62 6461 3e29 01da 036b 6579 544e 4672  mbda>)...keyTNFr
-00001560: 0100 0000 7217 0000 007a 3345 7863 6570  ....r....z3Excep
+00001560: 0100 0000 7216 0000 007a 3345 7863 6570  ....r....z3Excep
 00001570: 7469 6f6e 206f 6363 7572 7265 6420 7768  tion occurred wh
 00001580: 696c 6520 7275 6e6e 696e 6720 2725 732e  ile running '%s.
-00001590: 6765 745f 6f70 7469 6f6e 7328 2927 7218  get_options()'r.
+00001590: 6765 745f 6f70 7469 6f6e 7328 2927 7217  get_options()'r.
 000015a0: 0000 007a 3845 7863 6570 7469 6f6e 206f  ...z8Exception o
 000015b0: 6363 7572 7265 6420 7768 696c 6520 7275  ccurred while ru
 000015c0: 6e6e 696e 6720 2725 732e 6765 745f 6f70  nning '%s.get_op
-000015d0: 7469 6f6e 735f 6865 6c70 2829 2772 1500  tions_help()'r..
-000015e0: 0000 290e 7225 0000 0072 4f00 0000 721b  ..).r%...rO...r.
-000015f0: 0000 00da 0863 616c 6c61 626c 6572 5000  .....callablerP.
-00001600: 0000 7252 0000 0072 5300 0000 7229 0000  ..rR...rS...r)..
-00001610: 00da 0673 6f72 7465 6472 2200 0000 7223  ...sortedr"...r#
-00001620: 0000 0072 2b00 0000 7220 0000 0072 2600  ...r+...r ...r&.
-00001630: 0000 290b 722e 0000 0072 3f00 0000 7233  ..).r....r?...r3
+000015d0: 7469 6f6e 735f 6865 6c70 2829 2772 1400  tions_help()'r..
+000015e0: 0000 290e 7224 0000 0072 4e00 0000 721a  ..).r$...rN...r.
+000015f0: 0000 00da 0863 616c 6c61 626c 6572 4f00  .....callablerO.
+00001600: 0000 7251 0000 0072 5200 0000 7228 0000  ..rQ...rR...r(..
+00001610: 00da 0673 6f72 7465 6472 2100 0000 7222  ...sortedr!...r"
+00001620: 0000 0072 2a00 0000 721f 0000 0072 2500  ...r*...r....r%.
+00001630: 0000 290b 722d 0000 0072 3e00 0000 7232  ..).r-...r>...r2
 00001640: 0000 005a 0865 6469 7461 626c 655a 0972  ...Z.editableZ.r
 00001650: 6573 6574 6162 6c65 5a0d 6861 735f 6865  esetableZ.has_he
 00001660: 6c70 5f74 6578 74da 076f 7074 696f 6e73  lp_text..options
-00001670: 7236 0000 005a 0e70 6c75 6769 6e5f 6f70  r6...Z.plugin_op
-00001680: 7469 6f6e 73da 066f 7074 696f 6e5a 0968  tions..optionZ.h
-00001690: 656c 705f 7465 7874 720c 0000 0072 0c00  elp_textr....r..
-000016a0: 0000 720d 0000 0072 5000 0000 db00 0000  ..r....rP.......
+00001670: 7235 0000 005a 0e70 6c75 6769 6e5f 6f70  r5...Z.plugin_op
+00001680: 7469 6f6e 735a 066f 7074 696f 6e5a 0968  tionsZ.optionZ.h
+00001690: 656c 705f 7465 7874 720b 0000 0072 0b00  elp_textr....r..
+000016a0: 0000 720c 0000 0072 4f00 0000 db00 0000  ..r....rO.......
 000016b0: 738c 0000 0000 0f0a 0106 020e 040a 0108  s...............
 000016c0: ff02 0302 020a 0108 ff02 030a 0108 ff02  ................
 000016d0: 030a 0108 ff02 0306 0202 0102 0102 0102  ................
 000016e0: 0102 fb02 ff06 0a14 0304 020a 0502 fc04  ................
 000016f0: 0102 0102 0102 0102 0302 0104 020c 010a  ................
 00001700: 0104 0108 ff06 0504 0110 ff0a 040e 0104  ................
 00001710: 0102 0102 0102 fd06 060a 0306 0102 010c  ................
@@ -377,53 +377,53 @@
 00001780: 7c01 a101 a001 7c02 7c03 a102 0100 5700  |.....|.|.....W.
 00001790: 6401 5300 0400 7402 7940 0100 0100 0100  d.S...t.y@......
 000017a0: 7403 6a04 6402 7c01 7c02 7c03 6401 6403  t.j.d.|.|.|.d.d.
 000017b0: 8d05 0100 5900 6404 5300 3000 6400 5300  ....Y.d.S.0.d.S.
 000017c0: 2905 4e54 7a38 4578 6365 7074 696f 6e20  ).NTz8Exception 
 000017d0: 6f63 6375 7272 6564 2077 6869 6c65 2072  occurred while r
 000017e0: 756e 6e69 6e67 2027 2573 2e73 6574 5f6f  unning '%s.set_o
-000017f0: 7074 696f 6e28 2573 2c20 2573 2927 7218  ption(%s, %s)'r.
-00001800: 0000 0046 2905 724d 0000 0072 5100 0000  ...F).rM...rQ...
-00001810: 722b 0000 0072 2000 0000 7226 0000 0029  r+...r ...r&...)
-00001820: 0472 2e00 0000 723f 0000 0072 0b00 0000  .r....r?...r....
-00001830: da05 7661 6c75 6572 0c00 0000 720c 0000  ..valuer....r...
-00001840: 0072 0d00 0000 7251 0000 004a 0100 0073  .r....rQ...J...s
+000017f0: 7074 696f 6e28 2573 2c20 2573 2927 7217  ption(%s, %s)'r.
+00001800: 0000 0046 2905 724c 0000 0072 5000 0000  ...F).rL...rP...
+00001810: 722a 0000 0072 1f00 0000 7225 0000 0029  r*...r....r%...)
+00001820: 0472 2d00 0000 723e 0000 0072 0a00 0000  .r-...r>...r....
+00001830: da05 7661 6c75 6572 0b00 0000 720b 0000  ..valuer....r...
+00001840: 0072 0c00 0000 7250 0000 004a 0100 0073  .r....rP...J...s
 00001850: 1800 0000 0001 0201 1202 0602 0c01 0401  ................
 00001860: 0201 0201 0201 0201 02fb 0608 7a18 506c  ............z.Pl
 00001870: 7567 696e 4d61 6e61 6765 722e 7365 745f  uginManager.set_
 00001880: 6f70 7469 6f6e 6302 0000 0000 0000 0000  optionc.........
 00001890: 0000 0002 0000 0008 0000 0043 0000 0073  ...........C...s
 000018a0: 3e00 0000 7a14 7c00 a000 7c01 a101 a001  >...z.|...|.....
 000018b0: a100 0100 5700 6401 5300 0400 7402 7938  ....W.d.S...t.y8
 000018c0: 0100 0100 0100 7403 6a04 6402 7c01 6401  ......t.j.d.|.d.
 000018d0: 6403 8d03 0100 5900 6404 5300 3000 6400  d.....Y.d.S.0.d.
 000018e0: 5300 2905 4e54 7a35 4578 6365 7074 696f  S.).NTz5Exceptio
 000018f0: 6e20 6f63 6375 7272 6564 2077 6869 6c65  n occurred while
 00001900: 2072 756e 6e69 6e67 2027 2573 2e72 6573   running '%s.res
-00001910: 6574 5f6f 7074 696f 6e73 2829 2772 1800  et_options()'r..
-00001920: 0000 4629 0572 4d00 0000 7252 0000 0072  ..F).rM...rR...r
-00001930: 2b00 0000 7220 0000 0072 2600 0000 2902  +...r ...r&...).
-00001940: 722e 0000 0072 3f00 0000 720c 0000 0072  r....r?...r....r
-00001950: 0c00 0000 720d 0000 0072 5200 0000 5b01  ....r....rR...[.
+00001910: 6574 5f6f 7074 696f 6e73 2829 2772 1700  et_options()'r..
+00001920: 0000 4629 0572 4c00 0000 7251 0000 0072  ..F).rL...rQ...r
+00001930: 2a00 0000 721f 0000 0072 2500 0000 2902  *...r....r%...).
+00001940: 722d 0000 0072 3e00 0000 720b 0000 0072  r-...r>...r....r
+00001950: 0b00 0000 720c 0000 0072 5100 0000 5b01  ....r....rQ...[.
 00001960: 0000 7314 0000 0000 0102 010e 0206 020c  ..s.............
 00001970: 0104 0102 0102 0102 fd06 067a 1b50 6c75  ...........z.Plu
 00001980: 6769 6e4d 616e 6167 6572 2e72 6573 6574  ginManager.reset
-00001990: 5f6f 7074 696f 6e73 2911 7211 0000 0072  _options).r....r
-000019a0: 1200 0000 7213 0000 0072 3400 0000 723a  ....r....r4...r:
-000019b0: 0000 0072 3d00 0000 722c 0000 00da 0870  ...r=...r,.....p
-000019c0: 726f 7065 7274 7972 4400 0000 7245 0000  ropertyrD...rE..
-000019d0: 0072 4a00 0000 724d 0000 0072 4e00 0000  .rJ...rM...rN...
-000019e0: 7250 0000 0072 5100 0000 7252 0000 00da  rP...rQ...rR....
-000019f0: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 720c  .__classcell__r.
-00001a00: 0000 0072 0c00 0000 723c 0000 0072 0d00  ...r....r<...r..
-00001a10: 0000 7214 0000 0028 0000 0073 1c00 0000  ..r....(...s....
+00001990: 5f6f 7074 696f 6e73 2911 7210 0000 0072  _options).r....r
+000019a0: 1100 0000 7212 0000 0072 3300 0000 7239  ....r....r3...r9
+000019b0: 0000 0072 3c00 0000 722b 0000 00da 0870  ...r<...r+.....p
+000019c0: 726f 7065 7274 7972 4300 0000 7244 0000  ropertyrC...rD..
+000019d0: 0072 4900 0000 724c 0000 0072 4d00 0000  .rI...rL...rM...
+000019e0: 724f 0000 0072 5000 0000 7251 0000 00da  rO...rP...rQ....
+000019f0: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 720b  .__classcell__r.
+00001a00: 0000 0072 0b00 0000 723b 0000 0072 0c00  ...r....r;...r..
+00001a10: 0000 7213 0000 0028 0000 0073 1c00 0000  ..r....(...s....
 00001a20: 0801 0842 0c06 0c07 0826 0201 0a03 0201  ...B.....&......
-00001a30: 0a09 0824 0807 0804 086f 0811 7214 0000  ...$.....o..r...
+00001a30: 0a09 0824 0807 0804 086f 0811 7213 0000  ...$.....o..r...
 00001a40: 0029 09da 076c 6f67 6769 6e67 5a1b 666c  .)...loggingZ.fl
 00001a50: 616d 696e 676f 2e63 6f72 652e 7574 696c  amingo.core.util
 00001a60: 732e 696d 706f 7274 7372 0200 0000 da09  s.importsr......
-00001a70: 6765 744c 6f67 6765 7272 2000 0000 722d  getLoggerr ...r-
-00001a80: 0000 0072 0f00 0000 7210 0000 0072 1400  ...r....r....r..
-00001a90: 0000 720c 0000 0072 0c00 0000 720c 0000  ..r....r....r...
-00001aa0: 0072 0d00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00001a70: 6765 744c 6f67 6765 7272 1f00 0000 722c  getLoggerr....r,
+00001a80: 0000 0072 0e00 0000 720f 0000 0072 1300  ...r....r....r..
+00001a90: 0000 720b 0000 0072 0b00 0000 720b 0000  ..r....r....r...
+00001aa0: 0072 0c00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
 00001ab0: 0100 0000 730c 0000 0008 020c 020a 0208  ....s...........
 00001ac0: 1408 090e 04                             .....
```

### Comparing `flamingo-1.8/flamingo/core/plugins/__pycache__/static.cpython-310.pyc` & `flamingo-1.9/flamingo/core/plugins/__pycache__/static.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/plugins/__pycache__/static.cpython-35.pyc` & `flamingo-1.9/flamingo/core/plugins/__pycache__/static.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/plugins/__pycache__/static.cpython-37.pyc` & `flamingo-1.9/flamingo/core/plugins/__pycache__/static.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/plugins/__pycache__/static.cpython-39.pyc` & `flamingo-1.9/flamingo/core/plugins/__pycache__/static.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/plugins/layers.py` & `flamingo-1.9/flamingo/core/plugins/layers.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/plugins/media.py` & `flamingo-1.9/flamingo/core/plugins/media.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/plugins/meta_data.py` & `flamingo-1.9/flamingo/core/plugins/meta_data.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/plugins/plugin_manager.py` & `flamingo-1.9/flamingo/core/plugins/plugin_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,17 +139,17 @@
 
         # settings hooks
         logger.debug('searching for settings hooks')
 
         for attr_name in dir(self._context.settings):
             attr = getattr(self._context.settings, attr_name)
 
-            if(not hasattr(attr, 'flamingo_hook_name') or
-               attr.flamingo_hook_name not in hook_names_to_discover or
-               attr in self._hooks[attr.flamingo_hook_name]):
+            if (not hasattr(attr, 'flamingo_hook_name') or
+                attr.flamingo_hook_name not in hook_names_to_discover or
+                    attr in self._hooks[attr.flamingo_hook_name]):
 
                 continue
 
             logger.debug("settings.%s discoverd as", attr.flamingo_hook_name)
 
             self._hooks[attr.flamingo_hook_name].append(
                 ('settings', attr, ),
@@ -234,16 +234,16 @@
         if not hasattr(self, '_options'):
             self._options = []
 
             for plugin_name, plugin_object in self._plugins:
 
                 # a plugin needs to implement at least 'get_options()'
                 # to get listed
-                if(not hasattr(plugin_object, 'get_options') or
-                   not callable(plugin_object.get_options)):
+                if (not hasattr(plugin_object, 'get_options') or
+                        not callable(plugin_object.get_options)):
 
                     continue
 
                 editable = (hasattr(plugin_object, 'set_option') and
                             callable(plugin_object.get_options))
 
                 resetable = (hasattr(plugin_object, 'reset_options') and
```

### Comparing `flamingo-1.8/flamingo/core/plugins/static.py` & `flamingo-1.9/flamingo/core/plugins/static.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/settings/__pycache__/defaults.cpython-310.pyc` & `flamingo-1.9/flamingo/core/settings/__pycache__/defaults.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/settings/__pycache__/defaults.cpython-35.pyc` & `flamingo-1.9/flamingo/core/settings/__pycache__/defaults.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/settings/__pycache__/defaults.cpython-37.pyc` & `flamingo-1.9/flamingo/core/settings/__pycache__/defaults.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/settings/__pycache__/defaults.cpython-39.pyc` & `flamingo-1.9/flamingo/core/settings/__pycache__/defaults.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/settings/__pycache__/settings.cpython-310.pyc` & `flamingo-1.9/flamingo/core/settings/__pycache__/settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/settings/__pycache__/settings.cpython-35.pyc` & `flamingo-1.9/flamingo/core/settings/__pycache__/settings.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/settings/__pycache__/settings.cpython-37.pyc` & `flamingo-1.9/flamingo/core/settings/__pycache__/settings.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/settings/__pycache__/settings.cpython-39.pyc` & `flamingo-1.9/flamingo/core/settings/__pycache__/settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/settings/defaults.py` & `flamingo-1.9/flamingo/core/settings/defaults.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/settings/settings.py` & `flamingo-1.9/flamingo/core/settings/settings.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/templating/__pycache__/base.cpython-310.pyc` & `flamingo-1.9/flamingo/core/templating/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/templating/__pycache__/base.cpython-35.pyc` & `flamingo-1.9/flamingo/core/templating/__pycache__/base.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/templating/__pycache__/base.cpython-37.pyc` & `flamingo-1.9/flamingo/core/templating/__pycache__/base.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/templating/__pycache__/base.cpython-39.pyc` & `flamingo-1.9/flamingo/core/templating/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/templating/__pycache__/jinja2.cpython-310.pyc` & `flamingo-1.9/flamingo/core/templating/__pycache__/jinja2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Apr  6 13:20:24 2022 UTC, .py size: 12416 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9893 4d62 8030 0000  o.........Mb.0..
+00000000: 6f0d 0d0a 0000 0000 853e 7d62 8030 0000  o........>}b.0..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 b401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c06 5a06 6400 6401 6c07 5a07 6400  d.l.Z.d.d.l.Z.d.
 00000070: 6402 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
@@ -235,15 +235,15 @@
 00000ea0: 0000 7247 0000 0072 1d00 0000 2907 7216  ..rG...r....).r.
 00000eb0: 0000 00da 0c67 6574 5f74 656d 706c 6174  .....get_templat
 00000ec0: 65da 1263 6f6d 7069 6c65 5f65 7870 7265  e..compile_expre
 00000ed0: 7373 696f 6eda 0464 6963 7472 5900 0000  ssion..dictrY...
 00000ee0: 723e 0000 00da 0945 7863 6570 7469 6f6e  r>.....Exception
 00000ef0: 2905 7218 0000 0072 1900 0000 721a 0000  ).r....r....r...
 00000f00: 00da 0d74 656d 706c 6174 655f 6e61 6d65  ...template_name
-00000f10: 5a0a 6578 7072 6573 7369 6f6e 721b 0000  Z.expressionr...
+00000f10: da0a 6578 7072 6573 7369 6f6e 721b 0000  ..expressionr...
 00000f20: 0072 1d00 0000 721e 0000 0072 5b00 0000  .r....r....r[...
 00000f30: af00 0000 7318 0000 0008 0108 0212 0102  ....s...........
 00000f40: 020a 011a 010c 0208 0102 ff04 0322 0112  ............."..
 00000f50: 027a 2046 6c61 6d69 6e67 6f45 6e76 6972  .z FlamingoEnvir
 00000f60: 6f6e 6d65 6e74 2e67 6574 5f74 656d 706c  onment.get_templ
 00000f70: 6174 6529 0672 1f00 0000 7220 0000 0072  ate).r....r ...r
 00000f80: 2100 0000 7217 0000 0072 5b00 0000 7222  !...r....r[...r"
@@ -285,84 +285,84 @@
 000011c0: 0000 7306 0000 0006 000e 0106 ff7a 234a  ..s..........z#J
 000011d0: 696e 6a61 322e 5f5f 696e 6974 5f5f 2e3c  inja2.__init__.<
 000011e0: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
 000011f0: 703e 2903 da06 6c6f 6164 6572 da08 6669  p>)...loader..fi
 00001200: 6e61 6c69 7a65 da0a 6578 7465 6e73 696f  nalize..extensio
 00001210: 6e73 7257 0000 00da 0669 6d70 6f72 7472  nsrW.....importr
 00001220: 3400 0000 7a10 7465 6d70 6c61 7465 732f  4...z.templates/
-00001230: 6a69 6e6a 6132 2903 7267 0000 00da 0a61  jinja2).rg.....a
-00001240: 7574 6f65 7363 6170 6572 6800 0000 da0b  utoescaperh.....
+00001230: 6a69 6e6a 6132 2903 7268 0000 00da 0a61  jinja2).rh.....a
+00001240: 7574 6f65 7363 6170 6572 6900 0000 da0b  utoescaperi.....
 00001250: 6765 6e5f 736e 6970 7065 7472 0a00 0000  gen_snippetr....
 00001260: 722c 0000 0029 1f72 1600 0000 7217 0000  r,...).r....r...
 00001270: 0072 5000 0000 da08 7465 6d70 6669 6c65  .rP.....tempfile
 00001280: da12 5465 6d70 6f72 6172 7944 6972 6563  ..TemporaryDirec
 00001290: 746f 7279 da07 7465 6d70 6469 72da 0b74  tory..tempdir..t
 000012a0: 6865 6d65 5f70 6174 6873 7236 0000 0072  heme_pathsr6...r
 000012b0: 5800 0000 7203 0000 0072 2600 0000 723e  X...r....r&...r>
 000012c0: 0000 00da 114a 494e 4a41 325f 4558 5445  .....JINJA2_EXTE
 000012d0: 4e53 494f 4e53 da03 656e 7672 5700 0000  NSIONS..envrW...
 000012e0: 7232 0000 0072 3500 0000 7234 0000 0072  r2...r5...r4...r
 000012f0: 3300 0000 723f 0000 00da 114a 494e 4a41  3...r?.....JINJA
 00001300: 325f 5452 4143 4542 4143 4b53 da1a 4a49  2_TRACEBACKS..JI
 00001310: 4e4a 4132 5f54 5241 4345 4241 434b 535f  NJA2_TRACEBACKS_
-00001320: 5059 474d 454e 5453 7202 0000 0072 6200  PYGMENTSr....rb.
+00001320: 5059 474d 454e 5453 7202 0000 0072 6300  PYGMENTSr....rc.
 00001330: 0000 723d 0000 0072 4e00 0000 720b 0000  ..r=...rN...r...
-00001340: 00da 0965 7272 6f72 5f65 6e76 726c 0000  ...error_envrl..
+00001340: 00da 0965 7272 6f72 5f65 6e76 726d 0000  ...error_envrm..
 00001350: 0072 0a00 0000 722c 0000 0029 0472 1800  .r....r,...).r..
 00001360: 0000 7233 0000 005a 0d74 656d 706c 6174  ..r3...Z.templat
-00001370: 655f 6469 7273 726b 0000 0072 1b00 0000  e_dirsrk...r....
+00001370: 655f 6469 7273 726c 0000 0072 1b00 0000  e_dirsrl...r....
 00001380: 721d 0000 0072 1e00 0000 7217 0000 00c3  r....r....r.....
 00001390: 0000 0073 4200 0000 0c01 0602 0a03 0603  ...sB...........
 000013a0: 0401 04ff 0802 04fe 0204 0201 0601 0201  ................
 000013b0: 0601 08fc 0c07 0c01 0c01 0a03 0801 02ff  ................
 000013c0: 0c03 0202 0201 0e01 02ff 0202 0201 08fc  ................
 000013d0: 0e07 0c01 0c01 1001 08f1 7a0f 4a69 6e6a  ..........z.Jinj
 000013e0: 6132 2e5f 5f69 6e69 745f 5f54 6304 0000  a2.__init__Tc...
 000013f0: 0000 0000 0000 0000 000d 0000 0008 0000  ................
 00001400: 0043 0000 0073 1c01 0000 7c00 6a00 6a01  .C...s....|.j.j.
 00001410: 6a02 7d04 7c02 6401 1800 7d05 7403 7c01  j.}.|.d...}.t.|.
 00001420: 6402 8302 a004 a100 a005 a100 7d06 7c06  d...........}.|.
 00001430: 7c05 7c04 1800 7c05 8502 1900 7d07 7c06  |.|...|.....}.|.
 00001440: 7c05 6401 1700 7c05 7c04 1700 6401 1700  |.d...|.|...d...
 00001450: 8502 1900 7d08 7c07 6400 6400 8502 1900  ....}.|.d.d.....
-00001460: 4400 5d0b 7d09 7c09 7232 0100 7138 7c07  D.].}.|.r2..q8|.
+00001460: 4400 5d0b 7d09 7c09 7232 0100 6e06 7c07  D.].}.|.r2..n.|.
 00001470: a006 7c09 a101 0100 712c 7c08 6400 6400  ..|.....q,|.d.d.
 00001480: 6403 8503 1900 4400 5d0a 7d09 7c09 7245  d.....D.].}.|.rE
-00001490: 0100 714a 7c08 a007 a100 0100 713f 6404  ..qJ|.......q?d.
+00001490: 0100 6e05 7c08 a007 a100 0100 713f 6404  ..n.|.......q?d.
 000014a0: a008 6700 7c07 a201 7c06 7c05 1900 9101  ..g.|...|.|.....
 000014b0: 7c08 a201 a101 7d0a 7a06 7409 7c01 8301  |.....}.z.t.|...
 000014c0: 7d0b 5700 6e0d 0400 740a 796a 0100 0100  }.W.n...t.yj....
 000014d0: 0100 740b 6405 8301 7d0b 5900 6e01 7700  ..t.d...}.Y.n.w.
 000014e0: 7c03 727e 740c 6406 740d 7c07 8301 6401  |.r~t.d.t.|...d.
 000014f0: 1700 6701 7c02 740d 7c07 8301 1800 6407  ..g.|.t.|.....d.
 00001500: 8d03 7d0c 6e0a 740c 740d 7c07 8301 6401  ..}.n.t.t.|...d.
 00001510: 1700 6701 6408 8d01 7d0c 740e 7c0a 7c0b  ..g.d...}.t.|.|.
 00001520: 7c0c 8303 5300 2909 4e72 4700 0000 da01  |...S.).NrG.....
 00001530: 72e9 ffff ffff da01 0ada 0474 6578 74da  r..........text.
 00001540: 0669 6e6c 696e 6529 03da 076c 696e 656e  .inline)...linen
 00001550: 6f73 da08 686c 5f6c 696e 6573 da0b 6c69  os..hl_lines..li
-00001560: 6e65 6e6f 7374 6172 7429 0172 7c00 0000  nenostart).r|...
+00001560: 6e65 6e6f 7374 6172 7429 0172 7d00 0000  nenostart).r}...
 00001570: 290f 7233 0000 0072 3e00 0000 da1f 4a49  ).r3...r>.....JI
 00001580: 4e4a 4132 5f54 5241 4345 4241 434b 535f  NJA2_TRACEBACKS_
 00001590: 434f 4e54 4558 545f 4c49 4e45 53da 046f  CONTEXT_LINES..o
 000015a0: 7065 6eda 0472 6561 64da 0a73 706c 6974  pen..read..split
 000015b0: 6c69 6e65 73da 0672 656d 6f76 65da 0370  lines..remove..p
 000015c0: 6f70 724e 0000 0072 0e00 0000 720f 0000  oprN...r....r...
 000015d0: 0072 0d00 0000 720c 0000 00da 036c 656e  .r....r......len
 000015e0: da12 7079 676d 656e 7473 5f68 6967 686c  ..pygments_highl
 000015f0: 6967 6874 290d 7218 0000 0072 3d00 0000  ight).r....r=...
 00001600: da06 6c69 6e65 6e6f 5a0c 7368 6f77 5f6c  ..linenoZ.show_l
-00001610: 696e 656e 6f73 5a0d 636f 6e74 6578 745f  inenosZ.context_
+00001610: 696e 656e 6f73 da0d 636f 6e74 6578 745f  inenos..context_
 00001620: 6c69 6e65 73da 0569 6e64 6578 da05 6c69  lines..index..li
 00001630: 6e65 735a 1163 6f6e 7465 7874 5f6c 696e  nesZ.context_lin
 00001640: 6573 5f74 6f70 5a14 636f 6e74 6578 745f  es_topZ.context_
 00001650: 6c69 6e65 735f 626f 7474 6f6d da04 6c69  lines_bottom..li
 00001660: 6e65 da07 736e 6970 7065 74da 056c 6578  ne..snippet..lex
 00001670: 6572 da09 666f 726d 6174 7465 7272 1d00  er..formatterr..
-00001680: 0000 721d 0000 0072 1e00 0000 726c 0000  ..r....r....rl..
+00001680: 0000 721d 0000 0072 1e00 0000 726d 0000  ..r....r....rm..
 00001690: 00ed 0000 0073 4600 0000 0a01 0801 1202  .....sF.........
 000016a0: 1002 1801 1002 0401 0401 0c02 1202 0401  ................
 000016b0: 0401 0a02 0602 0201 02ff 0602 02fe 0203  ................
 000016c0: 06fd 0206 0c01 0c02 0c01 02ff 0403 0201  ................
 000016d0: 0201 0c01 0a01 08fd 0207 0c01 06ff 0c04  ................
 000016e0: 7a12 4a69 6e6a 6132 2e67 656e 5f73 6e69  z.Jinja2.gen_sni
 000016f0: 7070 6574 6302 0000 0000 0000 0000 0000  ppetc...........
@@ -382,45 +382,45 @@
 000017d0: 7411 7412 6602 8302 726b 6406 6407 8400  t.t.f...rkd.d...
 000017e0: 7c02 4400 8301 7d02 7407 7c01 7411 8302  |.D...}.t.|.t...
 000017f0: 7284 7413 7c02 8301 6405 6b04 7284 7c02  r.t.|...d.k.r.|.
 00001800: 6408 1900 7c02 6401 1900 6b02 7284 7c02  d...|.d...k.r.|.
 00001810: 6400 6401 8502 1900 7d02 7c00 6a14 a015  d.d.....}.|.j...
 00001820: 6409 a101 7d07 7c07 6a16 7c00 6a0e 7c01  d...}.|.j.|.j.|.
 00001830: 7c02 7412 7417 7407 640a 8d06 5300 290b  |.t.t.t.d...S.).
-00001840: 4e72 7700 0000 7224 0000 0072 3d00 0000  Nrw...r$...r=...
+00001840: 4e72 7800 0000 7224 0000 0072 3d00 0000  Nrx...r$...r=...
 00001850: da0d 6f72 6967 696e 616c 5f70 6174 6872  ..original_pathr
 00001860: 4700 0000 6301 0000 0000 0000 0000 0000  G...c...........
 00001870: 0002 0000 0006 0000 0053 0000 0073 2800  .........S...s(.
 00001880: 0000 6700 7c00 5d10 7d01 7400 6a01 a002  ..g.|.].}.t.j...
 00001890: 7c01 6400 1900 a101 6401 1900 6402 6b03  |.d.....d...d.k.
 000018a0: 7202 7c01 9102 7102 5300 2903 7201 0000  r.|...q.S.).r...
-000018b0: 0072 4700 0000 7a03 2e70 7929 0372 6200  .rG...z..py).rb.
+000018b0: 0072 4700 0000 7a03 2e70 7929 0372 6300  .rG...z..py).rc.
 000018c0: 0000 723d 0000 00da 0873 706c 6974 6578  ..r=.....splitex
-000018d0: 7472 6300 0000 721d 0000 0072 1d00 0000  trc...r....r....
-000018e0: 721e 0000 0072 6600 0000 4c01 0000 730c  r....rf...L...s.
+000018d0: 7472 6400 0000 721d 0000 0072 1d00 0000  trd...r....r....
+000018e0: 721e 0000 0072 6700 0000 4c01 0000 730c  r....rg...L...s.
 000018f0: 0000 0006 0002 0116 0102 fe02 0106 ff7a  ...............z
 00001900: 2c4a 696e 6a61 322e 5f72 656e 6465 725f  ,Jinja2._render_
 00001910: 6578 6365 7074 696f 6e2e 3c6c 6f63 616c  exception.<local
 00001920: 733e 2e3c 6c69 7374 636f 6d70 3e72 0100  s>.<listcomp>r..
 00001930: 0000 7a0a 6572 726f 722e 6874 6d6c 2906  ..z.error.html).
 00001940: 7233 0000 00da 0965 7863 6570 7469 6f6e  r3.....exception
 00001950: da05 7374 6163 6b72 0500 0000 7223 0000  ..stackr....r#..
 00001960: 0072 2700 0000 2918 da09 7472 6163 6562  .r'...)...traceb
 00001970: 6163 6bda 0a65 7874 7261 6374 5f74 62da  ack..extract_tb.
 00001980: 0d5f 5f74 7261 6365 6261 636b 5f5f da08  .__traceback__..
 00001990: 6669 6c65 6e61 6d65 7250 0000 0072 4100  filenamerP...rA.
-000019a0: 0000 7286 0000 0072 2700 0000 7211 0000  ..r....r'...r...
-000019b0: 0072 1300 0000 7214 0000 0072 6200 0000  .r....r....rb...
+000019a0: 0000 7287 0000 0072 2700 0000 7211 0000  ..r....r'...r...
+000019b0: 0072 1300 0000 7214 0000 0072 6300 0000  .r....r....rc...
 000019c0: 723d 0000 0072 4e00 0000 7233 0000 0072  r=...rN...r3...r
 000019d0: 3e00 0000 da0c 434f 4e54 454e 545f 524f  >.....CONTENT_RO
-000019e0: 4f54 7206 0000 0072 0500 0000 7284 0000  OTr....r....r...
-000019f0: 0072 7500 0000 725b 0000 00da 0672 656e  .ru...r[.....ren
+000019e0: 4f54 7206 0000 0072 0500 0000 7285 0000  OTr....r....r...
+000019f0: 0072 7600 0000 725b 0000 00da 0672 656e  .rv...r[.....ren
 00001a00: 6465 7272 2300 0000 2908 7218 0000 0072  derr#...).r....r
-00001a10: 8f00 0000 7290 0000 00da 0566 7261 6d65  ....r......frame
-00001a20: 7294 0000 0072 1300 0000 5a0f 636f 6e74  r....r....Z.cont
+00001a10: 9100 0000 7292 0000 00da 0566 7261 6d65  ....r......frame
+00001a20: 7296 0000 0072 1300 0000 5a0f 636f 6e74  r....r....Z.cont
 00001a30: 656e 745f 6162 7370 6174 68da 0874 656d  ent_abspath..tem
 00001a40: 706c 6174 6572 1d00 0000 721d 0000 0072  plater....r....r
 00001a50: 1e00 0000 da11 5f72 656e 6465 725f 6578  ......_render_ex
 00001a60: 6365 7074 696f 6e1c 0100 0073 4c00 0000  ception....sL...
 00001a70: 0401 1a07 0601 0401 0a02 0e01 0402 0c01  ................
 00001a80: 02ff 0e03 0402 0a01 06ff 0a04 0c06 0601  ................
 00001a90: 0801 0401 04fe 0a06 06ff 0a05 0e02 0605  ................
@@ -447,34 +447,34 @@
 00001be0: 7e05 7c04 8201 6400 7d05 7e05 7701 7700  ~.|...d.}.~.w.w.
 00001bf0: 2908 4e54 723c 0000 00da 0e5f 7061 7273  ).NTr<....._pars
 00001c00: 696e 675f 6572 726f 7229 01da 0865 7863  ing_error)...exc
 00001c10: 5f69 6e66 6f46 7a25 4578 6365 7074 696f  _infoFz%Exceptio
 00001c20: 6e20 6f63 6375 7272 6564 2077 6869 6c65  n occurred while
 00001c30: 2072 656e 6465 7269 6e67 2025 7372 1d00   rendering %sr..
 00001c40: 0000 290c 7233 0000 0072 3e00 0000 723f  ..).r3...r>...r?
-00001c50: 0000 0072 7300 0000 7272 0000 0072 5b00  ...rs...rr...r[.
-00001c60: 0000 7296 0000 0072 5e00 0000 7242 0000  ..r....r^...rB..
-00001c70: 00da 0564 6562 7567 7299 0000 0072 4300  ...debugr....rC.
+00001c50: 0000 0072 7400 0000 7273 0000 0072 5b00  ...rt...rs...r[.
+00001c60: 0000 7298 0000 0072 5e00 0000 7242 0000  ..r....r^...rB..
+00001c70: 00da 0564 6562 7567 729b 0000 0072 4300  ...debugr....rC.
 00001c80: 0000 2906 7218 0000 0072 5f00 0000 da10  ..).r....r_.....
 00001c90: 7465 6d70 6c61 7465 5f63 6f6e 7465 7874  template_context
 00001ca0: da11 6861 6e64 6c65 5f65 7863 6570 7469  ..handle_excepti
-00001cb0: 6f6e 7372 8f00 0000 da01 6572 1d00 0000  onsr......er....
+00001cb0: 6f6e 7372 9100 0000 da01 6572 1d00 0000  onsr......er....
 00001cc0: 721d 0000 0072 1e00 0000 da07 5f72 656e  r....r......_ren
 00001cd0: 6465 7263 0100 0073 3e00 0000 0a01 0801  derc...s>.......
 00001ce0: 02ff 1203 0201 08ff 0803 0a01 02ff 0e03  ................
 00001cf0: 0403 0202 1201 0201 0aff 0e03 0e01 1001  ................
 00001d00: 0880 02fe 0404 0401 0202 1001 0e02 0601  ................
 00001d10: 0401 10ff 0403 0880 02fc 7a0e 4a69 6e6a  ..........z.Jinj
 00001d20: 6132 2e5f 7265 6e64 6572 6304 0000 0000  a2._renderc.....
 00001d30: 0000 0000 0000 0004 0000 0005 0000 0043  ...............C
 00001d40: 0000 0073 1200 0000 7c00 a000 7c01 7c02  ...s....|...|.|.
 00001d50: 7c03 a103 6401 1900 5300 2902 4e72 4700  |...d...S.).NrG.
-00001d60: 0000 2901 72a0 0000 0029 0472 1800 0000  ..).r....).r....
-00001d70: 725f 0000 0072 9d00 0000 729e 0000 0072  r_...r....r....r
-00001d80: 1d00 0000 721d 0000 0072 1e00 0000 7296  ....r....r....r.
+00001d60: 0000 2901 72a2 0000 0029 0472 1800 0000  ..).r....).r....
+00001d70: 725f 0000 0072 9f00 0000 72a0 0000 0072  r_...r....r....r
+00001d80: 1d00 0000 721d 0000 0072 1e00 0000 7298  ....r....r....r.
 00001d90: 0000 0086 0100 0073 0a00 0000 0401 0601  .......s........
 00001da0: 02ff 0201 04ff 7a0d 4a69 6e6a 6132 2e72  ......z.Jinja2.r
 00001db0: 656e 6465 7263 0300 0000 0000 0000 0000  enderc..........
 00001dc0: 0000 0800 0000 0900 0000 4300 0000 7350  ..........C...sP
 00001dd0: 0100 007c 0164 0119 0072 0a64 027c 0164  ...|.d...r.d.|.d
 00001de0: 0119 0076 0172 1064 037c 0164 0119 0066  ...v.r.d.|.d...f
 00001df0: 0253 007c 006a 006a 016a 0272 1a7c 006a  .S.|.j.j.j.r.|.j
@@ -494,70 +494,70 @@
 00001ed0: 0001 0059 0001 007c 00a0 187c 067c 02a1  ...Y...|...|.|..
 00001ee0: 0257 007c 0472 967c 047c 006a 1576 0072  .W.|.r.|.|.j.v.r
 00001ef0: 977c 006a 15a0 197c 04a1 0101 0053 0053  .|.j...|.....S.S
 00001f00: 0053 007c 0472 a67c 047c 006a 1576 0072  .S.|.r.|.|.j.v.r
 00001f10: a77c 006a 15a0 197c 04a1 0101 0077 0077  .|.j...|.....w.w
 00001f20: 0077 0029 0b4e da0c 636f 6e74 656e 745f  .w.).N..content_
 00001f30: 626f 6479 da01 7b54 7224 0000 0072 3d00  body..{Tr$...r=.
-00001f40: 0000 728d 0000 007a 047b 7d7b 7d72 4700  ..r....z.{}{}rG.
+00001f40: 0000 728f 0000 007a 047b 7d7b 7d72 4700  ..r....z.{}{}rG.
 00001f50: 0000 7a02 772b 721d 0000 0029 1a72 3300  ..z.w+r....).r3.
-00001f60: 0000 723e 0000 0072 3f00 0000 7273 0000  ..r>...r?...rs..
-00001f70: 0072 7200 0000 da0b 6672 6f6d 5f73 7472  .rr.....from_str
-00001f80: 696e 6772 9600 0000 724d 0000 00da 0768  ingr....rM.....h
+00001f60: 0000 723e 0000 0072 3f00 0000 7274 0000  ..r>...r?...rt..
+00001f70: 0072 7300 0000 da0b 6672 6f6d 5f73 7472  .rs.....from_str
+00001f80: 696e 6772 9800 0000 724d 0000 00da 0768  ingr....rM.....h
 00001f90: 6173 686c 6962 da03 6d64 3572 2800 0000  ashlib..md5r(...
 00001fa0: da08 6461 7465 7469 6d65 da03 6e6f 77da  ..datetime..now.
 00001fb0: 0665 6e63 6f64 65da 0968 6578 6469 6765  .encode..hexdige
-00001fc0: 7374 7262 0000 0072 3d00 0000 728e 0000  strb...r=...r...
-00001fd0: 0072 4e00 0000 726f 0000 0072 3600 0000  .rN...ro...r6...
-00001fe0: 7250 0000 0072 7f00 0000 da05 7772 6974  rP...r......writ
-00001ff0: 6572 a000 0000 7283 0000 0029 0872 1800  er....r....).r..
-00002000: 0000 723c 0000 0072 9d00 0000 7298 0000  ..r<...r....r...
+00001fc0: 7374 7263 0000 0072 3d00 0000 7290 0000  strc...r=...r...
+00001fd0: 0072 4e00 0000 7270 0000 0072 3600 0000  .rN...rp...r6...
+00001fe0: 7250 0000 0072 8000 0000 da05 7772 6974  rP...r......writ
+00001ff0: 6572 a200 0000 7284 0000 0029 0872 1800  er....r....).r..
+00002000: 0000 723c 0000 0072 9f00 0000 729a 0000  ..r<...r....r...
 00002010: 0072 3d00 0000 7213 0000 0072 3600 0000  .r=...r....r6...
 00002020: da01 6672 1d00 0000 721d 0000 0072 1e00  ..fr....r....r..
 00002030: 0000 da12 7072 655f 7265 6e64 6572 5f63  ....pre_render_c
 00002040: 6f6e 7465 6e74 8a01 0000 733a 0000 0014  ontent....s:....
 00002050: 010c 010a 0208 0102 ff10 0314 0204 0202  ................
 00002060: 0208 0104 0208 010a 0104 0304 021a 010e  ................
 00002070: 0104 fe12 050a 010c 0210 011c ff0c 030e  ................
 00002080: 030e 0112 ff0e 0104 ff7a 194a 696e 6a61  .........z.Jinja
 00002090: 322e 7072 655f 7265 6e64 6572 5f63 6f6e  2.pre_render_con
 000020a0: 7465 6e74 2901 5429 0a72 1f00 0000 7220  tent).T).r....r 
-000020b0: 0000 0072 2100 0000 7217 0000 0072 6c00  ...r!...r....rl.
-000020c0: 0000 7299 0000 0072 a000 0000 7296 0000  ..r....r....r...
-000020d0: 0072 ac00 0000 7222 0000 0072 1d00 0000  .r....r"...r....
+000020b0: 0000 0072 2100 0000 7217 0000 0072 6d00  ...r!...r....rm.
+000020c0: 0000 729b 0000 0072 a200 0000 7298 0000  ..r....r....r...
+000020d0: 0072 ae00 0000 7222 0000 0072 1d00 0000  .r....r"...r....
 000020e0: 721d 0000 0072 1b00 0000 721e 0000 0072  r....r....r....r
-000020f0: 6000 0000 c200 0000 730e 0000 0008 000c  `.......s.......
-00002100: 010a 2a08 2f0a 470a 2310 0472 6000 0000  ..*./.G.#..r`...
-00002110: 2935 7291 0000 0072 a600 0000 726d 0000  )5r....r....rm..
-00002120: 0072 a400 0000 da07 6c6f 6767 696e 6772  .r......loggingr
-00002130: 3100 0000 7229 0000 0072 6200 0000 da06  1...r)...rb.....
+000020f0: 6100 0000 c200 0000 730e 0000 0008 000c  a.......s.......
+00002100: 010a 2a08 2f0a 470a 2310 0472 6100 0000  ..*./.G.#..ra...
+00002110: 2935 7293 0000 0072 a800 0000 726e 0000  )5r....r....rn..
+00002120: 0072 a600 0000 da07 6c6f 6767 696e 6772  .r......loggingr
+00002130: 3100 0000 7229 0000 0072 6300 0000 da06  1...r)...rc.....
 00002140: 6a69 6e6a 6132 7202 0000 0072 0300 0000  jinja2r....r....
 00002150: 7204 0000 0072 0500 0000 7206 0000 005a  r....r....r....Z
 00002160: 1d66 6c61 6d69 6e67 6f2e 636f 7265 2e74  .flamingo.core.t
 00002170: 656d 706c 6174 696e 672e 6261 7365 7207  emplating.baser.
 00002180: 0000 00da 1b66 6c61 6d69 6e67 6f2e 636f  .....flamingo.co
 00002190: 7265 2e75 7469 6c73 2e69 6d70 6f72 7473  re.utils.imports
 000021a0: 7209 0000 00da 1a66 6c61 6d69 6e67 6f2e  r......flamingo.
 000021b0: 636f 7265 2e75 7469 6c73 2e70 7072 696e  core.utils.pprin
 000021c0: 7472 0a00 0000 da08 666c 616d 696e 676f  tr......flamingo
 000021d0: 720b 0000 005a 1370 7967 6d65 6e74 732e  r....Z.pygments.
 000021e0: 666f 726d 6174 7465 7273 720c 0000 00da  formattersr.....
 000021f0: 0f70 7967 6d65 6e74 732e 6c65 7865 7273  .pygments.lexers
 00002200: 720d 0000 0072 0e00 0000 da0d 7079 676d  r....r......pygm
 00002210: 656e 7473 2e75 7469 6c72 0f00 0000 da08  ents.utilr......
-00002220: 7079 676d 656e 7473 7210 0000 0072 8500  pygmentsr....r..
+00002220: 7079 676d 656e 7473 7210 0000 0072 8600  pygmentsr....r..
 00002230: 0000 5a08 5059 474d 454e 5453 da0b 496d  ..Z.PYGMENTS..Im
 00002240: 706f 7274 4572 726f 7272 2f00 0000 722e  portErrorr/...r.
 00002250: 0000 0072 3d00 0000 724e 0000 00da 0764  ...r=...rN.....d
 00002260: 6972 6e61 6d65 da08 5f5f 6669 6c65 5f5f  irname..__file__
 00002270: 5a0e 4552 524f 525f 5445 4d50 4c41 5445  Z.ERROR_TEMPLATE
 00002280: da09 6765 744c 6f67 6765 7272 4200 0000  ..getLoggerrB...
 00002290: 725e 0000 0072 1100 0000 7223 0000 0072  r^...r....r#...r
 000022a0: 2600 0000 722c 0000 0072 3400 0000 7235  &...r,...r4...r5
-000022b0: 0000 0072 5700 0000 7258 0000 0072 6000  ...rW...rX...r`.
+000022b0: 0000 0072 5700 0000 7258 0000 0072 6100  ...rW...rX...ra.
 000022c0: 0000 721d 0000 0072 1d00 0000 721d 0000  ..r....r....r...
 000022d0: 0072 1e00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
 000022e0: 0100 0000 7358 0000 0008 0008 0108 0108  ....sX..........
 000022f0: 0108 0108 0108 0108 0114 0210 010c 020c  ................
 00002300: 010c 010c 0102 020c 0110 010c 010c 0108  ................
 00002310: 020c 0208 0102 ff02 0308 0108 020c 0208  ................
 00002320: 0102 ff16 030a 0210 0310 0a08 0408 0702  ................
```

### Comparing `flamingo-1.8/flamingo/core/templating/__pycache__/jinja2.cpython-35.pyc` & `flamingo-1.9/flamingo/core/templating/__pycache__/jinja2.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/templating/__pycache__/jinja2.cpython-37.pyc` & `flamingo-1.9/flamingo/core/templating/__pycache__/jinja2.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/templating/__pycache__/jinja2.cpython-39.pyc` & `flamingo-1.9/flamingo/core/templating/__pycache__/jinja2.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr  6 13:20:24 2022 UTC, .py size: 12416 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 9893 4d62 8030 0000  a.........Mb.0..
+00000000: 610d 0d0a 0000 0000 5399 7c63 8530 0000  a.......S.|c.0..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 b601 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c06 5a06 6400 6401 6c07 5a07 6400  d.l.Z.d.d.l.Z.d.
 00000070: 6402 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
@@ -103,26 +103,26 @@
 00000660: 0000 010a 0108 0272 2c00 0000 6301 0000  .......r,...c...
 00000670: 0000 0000 0000 0000 0001 0000 0003 0000  ................
 00000680: 0043 0000 0073 2000 0000 7400 720e 7401  .C...s ...t.r.t.
 00000690: a002 a100 0100 6e0e 7403 6a04 7405 8300  ......n.t.j.t...
 000006a0: 6401 8d01 0100 6400 5300 2902 4e29 01da  d.....d.S.).N)..
 000006b0: 056c 6f63 616c 2906 da07 4950 5954 484f  .local)...IPYTHO
 000006c0: 4eda 0749 5079 7468 6f6e da05 656d 6265  N..IPython..embe
-000006d0: 64da 0463 6f64 65da 0869 6e74 6572 6163  d..code..interac
+000006d0: 64da 0463 6f64 655a 0869 6e74 6572 6163  d..codeZ.interac
 000006e0: 74da 0767 6c6f 6261 6c73 2901 da07 636f  t..globals)...co
 000006f0: 6e74 6578 7472 1d00 0000 721d 0000 0072  ntextr....r....r
 00000700: 1e00 0000 da06 5f73 6865 6c6c 4600 0000  ......_shellF...
-00000710: 7306 0000 0000 0204 010a 0372 3500 0000  s..........r5...
+00000710: 7306 0000 0000 0204 010a 0372 3400 0000  s..........r4...
 00000720: 6300 0000 0000 0000 0000 0000 0002 0000  c...............
 00000730: 0004 0000 004f 0000 0073 1200 0000 7400  .....O...s....t.
 00000740: 7c00 6900 7c01 a401 8e01 6401 1900 5300  |.i.|.....d...S.
 00000750: 2902 4e72 0100 0000 7208 0000 0029 0272  ).Nr....r....).r
 00000760: 1900 0000 721a 0000 0072 1d00 0000 721d  ....r....r....r.
 00000770: 0000 0072 1e00 0000 da07 5f69 6d70 6f72  ...r......_impor
-00000780: 744f 0000 0073 0200 0000 0001 7236 0000  tO...s......r6..
+00000780: 744f 0000 0073 0200 0000 0001 7235 0000  tO...s......r5..
 00000790: 0072 2400 0000 2906 da04 6e61 6d65 da04  .r$...)...name..
 000007a0: 6c61 6e67 da04 6931 386e da09 6669 6e64  lang..i18n..find
 000007b0: 5f6e 616d 65da 0d5f 636f 6e74 656e 745f  _name.._content_
 000007c0: 7061 7468 da0f 5f63 6f6e 7465 6e74 5f6c  path.._content_l
 000007d0: 696e 656e 6f63 0200 0000 0000 0000 0600  inenoc..........
 000007e0: 0000 0f00 0000 0700 0000 0f00 0000 7338  ..............s8
 000007f0: 0100 0087 0087 0187 0266 0364 0164 0284  .........f.d.d..
@@ -150,76 +150,76 @@
 00000950: 8801 8800 6401 8d03 7d01 8802 6402 1900  ....d...}...d...
 00000960: 6a01 6a02 721e 7c01 8201 8802 6402 1900  j.j.r.|.....d...
 00000970: 6a03 a004 7c01 a101 0100 8801 724e 8800  j...|.......rN..
 00000980: 724e 8802 6402 1900 6a05 a006 6403 8801  rN..d...j...d...
 00000990: 8800 7c00 a104 0100 6e1c 8802 6402 1900  ..|.....n...d...
 000009a0: 6a05 a006 6404 8802 6405 1900 6406 1900  j...d...d...d...
 000009b0: 7c00 a103 0100 6407 5300 2908 4e72 1200  |.....d.S.).Nr..
-000009c0: 0000 7234 0000 007a 1425 733a 2573 3a20  ..r4...z.%s:%s: 
+000009c0: 0000 7233 0000 007a 1425 733a 2573 3a20  ..r3...z.%s:%s: 
 000009d0: 4c69 6e6b 4572 726f 723a 2025 737a 1125  LinkError: %sz.%
 000009e0: 733a 204c 696e 6b45 7272 6f72 3a20 2573  s: LinkError: %s
 000009f0: da07 636f 6e74 656e 74da 0470 6174 6872  ..content..pathr
 00000a00: 2400 0000 2907 7223 0000 00da 0873 6574  $...).r#.....set
 00000a10: 7469 6e67 73da 134c 4956 455f 5345 5256  tings..LIVE_SERV
 00000a20: 4552 5f52 554e 4e49 4e47 da06 6572 726f  ER_RUNNING..erro
 00000a30: 7273 da06 6170 7065 6e64 da06 6c6f 6767  rs..append..logg
 00000a40: 6572 da05 6572 726f 7229 02da 076d 6573  er..error)...mes
-00000a50: 7361 6765 7244 0000 00a9 0372 3c00 0000  sagerD.....r<...
-00000a60: 723b 0000 0072 3400 0000 721d 0000 0072  r;...r4...r....r
+00000a50: 7361 6765 7243 0000 00a9 0372 3b00 0000  sagerC.....r;...
+00000a60: 723a 0000 0072 3300 0000 721d 0000 0072  r:...r3...r....r
 00000a70: 1e00 0000 da0b 5f6c 696e 6b5f 6572 726f  ......_link_erro
 00000a80: 7257 0000 0073 2a00 0000 0001 0201 0201  rW...s*.........
 00000a90: 0201 02fd 0607 0c01 0403 1002 0801 0a01  ................
 00000aa0: 0201 0201 0201 02fc 0608 0a01 0201 0a01  ................
 00000ab0: 02fd 0406 7a19 6c69 6e6b 2e3c 6c6f 6361  ....z.link.<loca
 00000ac0: 6c73 3e2e 5f6c 696e 6b5f 6572 726f 7272  ls>._link_errorr
 00000ad0: 0100 0000 e901 0000 007a 1575 6e6b 6e6f  .........z.unkno
 00000ae0: 776e 2061 7267 756d 656e 7473 3a20 7b7d  wn arguments: {}
 00000af0: 7a02 2c20 7a13 756e 6b6e 6f77 6e20 6f70  z., z.unknown op
-00000b00: 7469 6f6e 733a 207b 7d72 3400 0000 2901  tions: {}r4...).
-00000b10: 723e 0000 0029 0172 3d00 0000 7a20 6361  r>...).r=...z ca
+00000b00: 7469 6f6e 733a 207b 7d72 3300 0000 2901  tions: {}r3...).
+00000b10: 723d 0000 0029 0172 3c00 0000 7a20 6361  r=...).r<...z ca
 00000b20: 6e20 6e6f 7420 7265 736f 6c76 6520 6c69  n not resolve li
 00000b30: 6e6b 2074 6172 6765 7420 277b 7d27 7a15  nk target '{}'z.
 00000b40: 666c 616d 696e 676f 2e70 6c75 6769 6e73  flamingo.plugins
-00000b50: 2e49 3138 4e72 3d00 0000 7238 0000 00da  .I18Nr=...r8....
+00000b50: 2e49 3138 4e72 3c00 0000 7237 0000 00da  .I18Nr<...r7....
 00000b60: 1049 3138 4e5f 434f 4e54 454e 545f 4b45  .I18N_CONTENT_KE
 00000b70: 59da 0269 64da 0375 726c da05 7469 746c  Y..id..url..titl
 00000b80: 65da 0d63 6f6e 7465 6e74 5f74 6974 6c65  e..content_title
 00000b90: 7a13 3c61 2068 7265 663d 227b 7d22 3e7b  z.<a href="{}">{
 00000ba0: 7d3c 2f61 3e29 09da 0666 6f72 6d61 74da  }</a>)...format.
 00000bb0: 046a 6f69 6eda 046b 6579 73da 0863 6f6e  .join..keys..con
 00000bc0: 7465 6e74 73da 0367 6574 da14 7265 736f  tents..get..reso
 00000bd0: 6c76 655f 636f 6e74 656e 745f 7061 7468  lve_content_path
-00000be0: 723f 0000 00da 0750 4c55 4749 4e53 da07  r?.....PLUGINS..
-00000bf0: 6765 7461 7474 7229 0f72 3400 0000 723e  getattr).r4...r>
-00000c00: 0000 0072 3700 0000 7238 0000 0072 3900  ...r7...r8...r9.
-00000c10: 0000 723a 0000 0072 3b00 0000 723c 0000  ..r:...r;...r<..
-00000c20: 0072 1900 0000 721a 0000 0072 4700 0000  .r....r....rG...
+00000be0: 723e 0000 00da 0750 4c55 4749 4e53 da07  r>.....PLUGINS..
+00000bf0: 6765 7461 7474 7229 0f72 3300 0000 723d  getattr).r3...r=
+00000c00: 0000 0072 3600 0000 7237 0000 0072 3800  ...r6...r7...r8.
+00000c10: 0000 7239 0000 0072 3a00 0000 723b 0000  ..r9...r:...r;..
+00000c20: 0072 1900 0000 721a 0000 0072 4600 0000  .r....r....rF...
 00000c30: da0f 6375 7272 656e 745f 636f 6e74 656e  ..current_conten
-00000c40: 7472 3d00 0000 5a10 6931 386e 5f63 6f6e  tr=...Z.i18n_con
+00000c40: 7472 3c00 0000 5a10 6931 386e 5f63 6f6e  tr<...Z.i18n_con
 00000c50: 7465 6e74 5f6b 6579 da06 7461 7267 6574  tent_key..target
-00000c60: 721d 0000 0072 4600 0000 721e 0000 00da  r....rF...r.....
+00000c60: 721d 0000 0072 4500 0000 721e 0000 00da  r....rE...r.....
 00000c70: 046c 696e 6b53 0000 0073 4c00 0000 0004  .linkS...sL.....
 00000c80: 101f 0801 0801 0c02 0401 1402 0401 0201  ................
 00000c90: 12ff 0404 0402 0401 1202 0a01 02ff 0603  ................
 00000ca0: 0401 0201 08ff 0404 0601 0aff 0403 1002  ................
 00000cb0: 0201 0cff 0403 0c01 0a01 0801 04fe 0606  ................
-00000cc0: 0802 0601 1802 0601 0c02 7258 0000 0063  ..........rX...c
+00000cc0: 0802 0601 1802 0601 0c02 7257 0000 0063  ..........rW...c
 00000cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ce0: 0300 0000 0000 0000 7328 0000 0065 005a  ........s(...e.Z
 00000cf0: 0164 005a 0287 0066 0164 0164 0284 085a  .d.Z...f.d.d...Z
 00000d00: 0387 0066 0164 0364 0484 085a 0487 0004  ...f.d.d...Z....
 00000d10: 005a 0553 0029 05da 1346 6c61 6d69 6e67  .Z.S.)...Flaming
 00000d20: 6f45 6e76 6972 6f6e 6d65 6e74 6302 0000  oEnvironmentc...
 00000d30: 0000 0000 0000 0000 0004 0000 0004 0000  ................
 00000d40: 000f 0000 0073 1c00 0000 7c01 7c00 5f00  .....s....|.|._.
 00000d50: 7401 8300 6a02 7c02 6900 7c03 a401 8e01  t...j.|.i.|.....
 00000d60: 0100 6400 5300 7215 0000 0029 03da 1066  ..d.S.r....)...f
 00000d70: 6c61 6d69 6e67 6f5f 636f 6e74 6578 7472  lamingo_contextr
 00000d80: 1600 0000 7217 0000 0029 0472 1800 0000  ....r....).r....
-00000d90: 725a 0000 0072 1900 0000 721a 0000 0072  rZ...r....r....r
+00000d90: 7259 0000 0072 1900 0000 721a 0000 0072  rY...r....r....r
 00000da0: 1b00 0000 721d 0000 0072 1e00 0000 7217  ....r....r....r.
 00000db0: 0000 00aa 0000 0073 0400 0000 0001 0602  .......s........
 00000dc0: 7a1c 466c 616d 696e 676f 456e 7669 726f  z.FlamingoEnviro
 00000dd0: 6e6d 656e 742e 5f5f 696e 6974 5f5f 6301  nment.__init__c.
 00000de0: 0000 0000 0000 0000 0000 0005 0000 0008  ................
 00000df0: 0000 000f 0000 0073 9600 0000 7c01 6401  .......s....|.d.
 00000e00: 1900 7d03 6402 7c03 7600 7222 7400 8300  ..}.d.|.v.r"t...
@@ -228,32 +228,32 @@
 00000e30: 7403 7c00 6a04 6a05 8301 a401 8e01 7d03  t.|.j.j.......}.
 00000e40: 5700 6e16 0400 7406 795c 0100 0100 0100  W.n...t.y\......
 00000e50: 6403 7d03 5900 6e02 3000 7c03 7284 7400  d.}.Y.n.0.|.r.t.
 00000e60: 8300 6a01 7c03 6701 7c01 6404 6400 8502  ..j.|.g.|.d.d...
 00000e70: 1900 a201 5200 6900 7c02 a401 8e01 5300  ....R.i.|.....S.
 00000e80: 7400 8300 6a01 7c01 6900 7c02 a401 8e01  t...j.|.i.|.....
 00000e90: 5300 2905 4e72 0100 0000 da01 2e72 2400  S.).Nr.......r$.
-00000ea0: 0000 7248 0000 0029 0772 1600 0000 da0c  ..rH...).r......
+00000ea0: 0000 7247 0000 0029 0772 1600 0000 da0c  ..rG...).r......
 00000eb0: 6765 745f 7465 6d70 6c61 7465 da12 636f  get_template..co
 00000ec0: 6d70 696c 655f 6578 7072 6573 7369 6f6e  mpile_expression
-00000ed0: da04 6469 6374 725a 0000 0072 3f00 0000  ..dictrZ...r?...
+00000ed0: da04 6469 6374 7259 0000 0072 3e00 0000  ..dictrY...r>...
 00000ee0: da09 4578 6365 7074 696f 6e29 0572 1800  ..Exception).r..
 00000ef0: 0000 7219 0000 0072 1a00 0000 da0d 7465  ..r....r......te
 00000f00: 6d70 6c61 7465 5f6e 616d 65da 0a65 7870  mplate_name..exp
 00000f10: 7265 7373 696f 6e72 1b00 0000 721d 0000  ressionr....r...
-00000f20: 0072 1e00 0000 725c 0000 00af 0000 0073  .r....r\.......s
+00000f20: 0072 1e00 0000 725b 0000 00af 0000 0073  .r....r[.......s
 00000f30: 1600 0000 0001 0802 0801 1202 0201 0a01  ................
 00000f40: 1a02 0c01 0a02 0401 2202 7a20 466c 616d  ........".z Flam
 00000f50: 696e 676f 456e 7669 726f 6e6d 656e 742e  ingoEnvironment.
 00000f60: 6765 745f 7465 6d70 6c61 7465 2906 721f  get_template).r.
 00000f70: 0000 0072 2000 0000 7221 0000 0072 1700  ...r ...r!...r..
-00000f80: 0000 725c 0000 0072 2200 0000 721d 0000  ..r\...r"...r...
+00000f80: 0000 725b 0000 0072 2200 0000 721d 0000  ..r[...r"...r...
 00000f90: 0072 1d00 0000 721b 0000 0072 1e00 0000  .r....r....r....
-00000fa0: 7259 0000 00a9 0000 0073 0400 0000 0801  rY.......s......
-00000fb0: 0c05 7259 0000 0063 0000 0000 0000 0000  ..rY...c........
+00000fa0: 7258 0000 00a9 0000 0073 0400 0000 0801  rX.......s......
+00000fb0: 0c05 7258 0000 0063 0000 0000 0000 0000  ..rX...c........
 00000fc0: 0000 0000 0000 0000 0300 0000 0000 0000  ................
 00000fd0: 734a 0000 0065 005a 0164 005a 0287 0066  sJ...e.Z.d.Z...f
 00000fe0: 0164 0164 0284 085a 0364 0e64 0464 0584  .d.d...Z.d.d.d..
 00000ff0: 015a 0464 0664 0784 005a 0564 0f64 0864  .Z.d.d...Z.d.d.d
 00001000: 0984 015a 0664 1064 0a64 0b84 015a 0764  ...Z.d.d.d...Z.d
 00001010: 0c64 0d84 005a 0887 0004 005a 0953 0029  .d...Z.....Z.S.)
 00001020: 11da 064a 696e 6a61 3263 0200 0000 0000  ...Jinja2c......
@@ -274,45 +274,45 @@
 00001110: 0f64 0a3c 0074 1e7c 006a 1b6a 0f64 0b3c  .d.<.t.|.j.j.d.<
 00001120: 0074 117c 006a 1b6a 0f64 063c 0064 0053  .t.|.j.j.d.<.d.S
 00001130: 0029 0c4e 6301 0000 0000 0000 0000 0000  .).Nc...........
 00001140: 0002 0000 0006 0000 0053 0000 0073 1a00  .........S...s..
 00001150: 0000 6700 7c00 5d12 7d01 7400 6a01 a002  ..g.|.].}.t.j...
 00001160: 7c01 6400 a102 9102 7104 5300 2901 da09  |.d.....q.S.)...
 00001170: 7465 6d70 6c61 7465 7329 03da 026f 7372  templates)...osr
-00001180: 3e00 0000 724f 0000 00a9 02da 022e 30da  >...rO........0.
+00001180: 3d00 0000 724e 0000 00a9 02da 022e 30da  =...rN........0.
 00001190: 0169 721d 0000 0072 1d00 0000 721e 0000  .ir....r....r...
 000011a0: 00da 0a3c 6c69 7374 636f 6d70 3ecc 0000  ...<listcomp>...
 000011b0: 0073 0200 0000 0601 7a23 4a69 6e6a 6132  .s......z#Jinja2
 000011c0: 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63 616c  .__init__.<local
 000011d0: 733e 2e3c 6c69 7374 636f 6d70 3e29 03da  s>.<listcomp>)..
 000011e0: 066c 6f61 6465 72da 0866 696e 616c 697a  .loader..finaliz
-000011f0: 65da 0a65 7874 656e 7369 6f6e 7372 5800  e..extensionsrX.
-00001200: 0000 da06 696d 706f 7274 7235 0000 007a  ....importr5...z
+000011f0: 65da 0a65 7874 656e 7369 6f6e 7372 5700  e..extensionsrW.
+00001200: 0000 da06 696d 706f 7274 7234 0000 007a  ....importr4...z
 00001210: 1074 656d 706c 6174 6573 2f6a 696e 6a61  .templates/jinja
-00001220: 3229 0372 6900 0000 da0a 6175 746f 6573  2).ri.....autoes
-00001230: 6361 7065 726a 0000 00da 0b67 656e 5f73  caperj.....gen_s
+00001220: 3229 0372 6800 0000 da0a 6175 746f 6573  2).rh.....autoes
+00001230: 6361 7065 7269 0000 00da 0b67 656e 5f73  caperi.....gen_s
 00001240: 6e69 7070 6574 720a 0000 0072 2c00 0000  nippetr....r,...
-00001250: 291f 7216 0000 0072 1700 0000 7251 0000  ).r....r....rQ..
+00001250: 291f 7216 0000 0072 1700 0000 7250 0000  ).r....r....rP..
 00001260: 00da 0874 656d 7066 696c 65da 1254 656d  ...tempfile..Tem
 00001270: 706f 7261 7279 4469 7265 6374 6f72 79da  poraryDirectory.
 00001280: 0774 656d 7064 6972 da0b 7468 656d 655f  .tempdir..theme_
-00001290: 7061 7468 7372 3700 0000 7259 0000 0072  pathsr7...rY...r
-000012a0: 0300 0000 7226 0000 0072 3f00 0000 da11  ....r&...r?.....
+00001290: 7061 7468 7372 3600 0000 7258 0000 0072  pathsr6...rX...r
+000012a0: 0300 0000 7226 0000 0072 3e00 0000 da11  ....r&...r>.....
 000012b0: 4a49 4e4a 4132 5f45 5854 454e 5349 4f4e  JINJA2_EXTENSION
-000012c0: 53da 0365 6e76 7258 0000 0072 3300 0000  S..envrX...r3...
-000012d0: 7236 0000 0072 3500 0000 7234 0000 0072  r6...r5...r4...r
-000012e0: 4000 0000 da11 4a49 4e4a 4132 5f54 5241  @.....JINJA2_TRA
+000012c0: 53da 0365 6e76 7257 0000 0072 3200 0000  S..envrW...r2...
+000012d0: 7235 0000 0072 3400 0000 7233 0000 0072  r5...r4...r3...r
+000012e0: 3f00 0000 da11 4a49 4e4a 4132 5f54 5241  ?.....JINJA2_TRA
 000012f0: 4345 4241 434b 53da 1a4a 494e 4a41 325f  CEBACKS..JINJA2_
 00001300: 5452 4143 4542 4143 4b53 5f50 5947 4d45  TRACEBACKS_PYGME
-00001310: 4e54 5372 0200 0000 7264 0000 0072 3e00  NTSr....rd...r>.
-00001320: 0000 724f 0000 0072 0b00 0000 da09 6572  ..rO...r......er
-00001330: 726f 725f 656e 7672 6e00 0000 720a 0000  ror_envrn...r...
-00001340: 0072 2c00 0000 2904 7218 0000 0072 3400  .r,...).r....r4.
+00001310: 4e54 5372 0200 0000 7263 0000 0072 3d00  NTSr....rc...r=.
+00001320: 0000 724e 0000 0072 0b00 0000 da09 6572  ..rN...r......er
+00001330: 726f 725f 656e 7672 6d00 0000 720a 0000  ror_envrm...r...
+00001340: 0072 2c00 0000 2904 7218 0000 0072 3300  .r,...).r....r3.
 00001350: 0000 5a0d 7465 6d70 6c61 7465 5f64 6972  ..Z.template_dir
-00001360: 7372 6d00 0000 721b 0000 0072 1d00 0000  srm...r....r....
+00001360: 7372 6c00 0000 721b 0000 0072 1d00 0000  srl...r....r....
 00001370: 721e 0000 0072 1700 0000 c300 0000 7340  r....r........s@
 00001380: 0000 0000 010c 0206 030a 0306 0104 ff04  ................
 00001390: 0208 fe04 0402 0102 0106 0102 0106 fc08  ................
 000013a0: 070c 010c 010c 030a 0108 ff02 030c 0202  ................
 000013b0: 0102 010e ff02 0202 0102 fc08 070e 010c  ................
 000013c0: 010c 017a 0f4a 696e 6a61 322e 5f5f 696e  ...z.Jinja2.__in
 000013d0: 6974 5f5f 5463 0400 0000 0000 0000 0000  it__Tc..........
@@ -331,37 +331,37 @@
 000014a0: 0a7a 0c74 097c 0183 017d 0b57 006e 1a04  .z.t.|...}.W.n..
 000014b0: 0074 0a79 d401 0001 0001 0074 0b64 0583  .t.y.......t.d..
 000014c0: 017d 0b59 006e 0230 007c 0372 fc74 0c64  .}.Y.n.0.|.r.t.d
 000014d0: 0674 0d7c 0783 0164 0117 0067 017c 0274  .t.|...d...g.|.t
 000014e0: 0d7c 0783 0118 0064 078d 037d 0c6e 1474  .|.....d...}.n.t
 000014f0: 0c74 0d7c 0783 0164 0117 0067 0164 088d  .t.|...d...g.d..
 00001500: 017d 0c74 0e7c 0a7c 0b7c 0c83 0353 0029  .}.t.|.|.|...S.)
-00001510: 094e 7248 0000 00da 0172 e9ff ffff ffda  .NrH.....r......
+00001510: 094e 7247 0000 00da 0172 e9ff ffff ffda  .NrG.....r......
 00001520: 010a da04 7465 7874 da06 696e 6c69 6e65  ....text..inline
 00001530: 2903 da07 6c69 6e65 6e6f 73da 0868 6c5f  )...linenos..hl_
 00001540: 6c69 6e65 73da 0b6c 696e 656e 6f73 7461  lines..linenosta
-00001550: 7274 2901 727e 0000 0029 0f72 3400 0000  rt).r~...).r4...
-00001560: 723f 0000 00da 1f4a 494e 4a41 325f 5452  r?.....JINJA2_TR
+00001550: 7274 2901 727d 0000 0029 0f72 3300 0000  rt).r}...).r3...
+00001560: 723e 0000 00da 1f4a 494e 4a41 325f 5452  r>.....JINJA2_TR
 00001570: 4143 4542 4143 4b53 5f43 4f4e 5445 5854  ACEBACKS_CONTEXT
 00001580: 5f4c 494e 4553 da04 6f70 656e da04 7265  _LINES..open..re
 00001590: 6164 da0a 7370 6c69 746c 696e 6573 da06  ad..splitlines..
-000015a0: 7265 6d6f 7665 da03 706f 7072 4f00 0000  remove..poprO...
+000015a0: 7265 6d6f 7665 da03 706f 7072 4e00 0000  remove..poprN...
 000015b0: 720e 0000 0072 0f00 0000 720d 0000 0072  r....r....r....r
 000015c0: 0c00 0000 da03 6c65 6eda 1270 7967 6d65  ......len..pygme
 000015d0: 6e74 735f 6869 6768 6c69 6768 7429 0d72  nts_highlight).r
-000015e0: 1800 0000 723e 0000 00da 066c 696e 656e  ....r>.....linen
+000015e0: 1800 0000 723d 0000 00da 066c 696e 656e  ....r=.....linen
 000015f0: 6f5a 0c73 686f 775f 6c69 6e65 6e6f 73da  oZ.show_linenos.
 00001600: 0d63 6f6e 7465 7874 5f6c 696e 6573 da05  .context_lines..
 00001610: 696e 6465 78da 056c 696e 6573 5a11 636f  index..linesZ.co
 00001620: 6e74 6578 745f 6c69 6e65 735f 746f 705a  ntext_lines_topZ
 00001630: 1463 6f6e 7465 7874 5f6c 696e 6573 5f62  .context_lines_b
 00001640: 6f74 746f 6dda 046c 696e 65da 0773 6e69  ottom..line..sni
 00001650: 7070 6574 da05 6c65 7865 72da 0966 6f72  ppet..lexer..for
 00001660: 6d61 7474 6572 721d 0000 0072 1d00 0000  matterr....r....
-00001670: 721e 0000 0072 6e00 0000 ed00 0000 7344  r....rn.......sD
+00001670: 721e 0000 0072 6d00 0000 ed00 0000 7344  r....rm.......sD
 00001680: 0000 0000 010a 0108 0212 0210 0118 0210  ................
 00001690: 0104 0104 020c 0212 0104 0104 020a 0206  ................
 000016a0: 0102 ff02 0206 fe02 0302 fd06 0602 010c  ................
 000016b0: 020c 010e 0204 0102 0102 010c 010a fd08  ................
 000016c0: 0702 010c ff06 047a 124a 696e 6a61 322e  .......z.Jinja2.
 000016d0: 6765 6e5f 736e 6970 7065 7463 0200 0000  gen_snippetc....
 000016e0: 0000 0000 0000 0000 0800 0000 0800 0000  ................
@@ -380,45 +380,45 @@
 000017b0: 017d 0274 077c 0174 1174 1266 0283 0272  .}.t.|.t.t.f...r
 000017c0: d664 0664 0784 007c 0244 0083 017d 0274  .d.d...|.D...}.t
 000017d0: 077c 0174 1183 0290 0172 0e74 137c 0283  .|.t.....r.t.|..
 000017e0: 0164 056b 0490 0172 0e7c 0264 0819 007c  .d.k...r.|.d...|
 000017f0: 0264 0119 006b 0290 0172 0e7c 0264 0064  .d...k...r.|.d.d
 00001800: 0185 0219 007d 027c 006a 14a0 1564 09a1  .....}.|.j...d..
 00001810: 017d 077c 076a 167c 006a 0e7c 017c 0274  .}.|.j.|.j.|.|.t
-00001820: 1274 1774 0764 0a8d 0653 0029 0b4e 7279  .t.t.d...S.).Nry
-00001830: 0000 0072 2400 0000 723e 0000 00da 0d6f  ...r$...r>.....o
-00001840: 7269 6769 6e61 6c5f 7061 7468 7248 0000  riginal_pathrH..
+00001820: 1274 1774 0764 0a8d 0653 0029 0b4e 7278  .t.t.d...S.).Nrx
+00001830: 0000 0072 2400 0000 723d 0000 00da 0d6f  ...r$...r=.....o
+00001840: 7269 6769 6e61 6c5f 7061 7468 7247 0000  riginal_pathrG..
 00001850: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
 00001860: 0000 0600 0000 5300 0000 7328 0000 0067  ......S...s(...g
 00001870: 007c 005d 207d 0174 006a 01a0 027c 0164  .|.] }.t.j...|.d
 00001880: 0019 00a1 0164 0119 0064 026b 0372 047c  .....d...d.k.r.|
-00001890: 0191 0271 0453 0029 0372 0100 0000 7248  ...q.S.).r....rH
-000018a0: 0000 007a 032e 7079 2903 7264 0000 0072  ...z..py).rd...r
-000018b0: 3e00 0000 da08 7370 6c69 7465 7874 7265  >.....splitextre
+00001890: 0191 0271 0453 0029 0372 0100 0000 7247  ...q.S.).r....rG
+000018a0: 0000 007a 032e 7079 2903 7263 0000 0072  ...z..py).rc...r
+000018b0: 3d00 0000 da08 7370 6c69 7465 7874 7264  =.....splitextrd
 000018c0: 0000 0072 1d00 0000 721d 0000 0072 1e00  ...r....r....r..
-000018d0: 0000 7268 0000 004c 0100 0073 0600 0000  ..rh...L...s....
+000018d0: 0000 7267 0000 004c 0100 0073 0600 0000  ..rg...L...s....
 000018e0: 0601 0201 18ff 7a2c 4a69 6e6a 6132 2e5f  ......z,Jinja2._
 000018f0: 7265 6e64 6572 5f65 7863 6570 7469 6f6e  render_exception
 00001900: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
 00001910: 6f6d 703e 7201 0000 007a 0a65 7272 6f72  omp>r....z.error
-00001920: 2e68 746d 6c29 0672 3400 0000 da09 6578  .html).r4.....ex
+00001920: 2e68 746d 6c29 0672 3300 0000 da09 6578  .html).r3.....ex
 00001930: 6365 7074 696f 6eda 0573 7461 636b 7205  ception..stackr.
 00001940: 0000 0072 2300 0000 7227 0000 0029 18da  ...r#...r'...)..
 00001950: 0974 7261 6365 6261 636b da0a 6578 7472  .traceback..extr
 00001960: 6163 745f 7462 da0d 5f5f 7472 6163 6562  act_tb..__traceb
 00001970: 6163 6b5f 5fda 0866 696c 656e 616d 6572  ack__..filenamer
-00001980: 5100 0000 7242 0000 0072 8800 0000 7227  Q...rB...r....r'
+00001980: 5000 0000 7241 0000 0072 8700 0000 7227  P...rA...r....r'
 00001990: 0000 0072 1100 0000 7213 0000 0072 1400  ...r....r....r..
-000019a0: 0000 7264 0000 0072 3e00 0000 724f 0000  ..rd...r>...rO..
-000019b0: 0072 3400 0000 723f 0000 00da 0c43 4f4e  .r4...r?.....CON
+000019a0: 0000 7263 0000 0072 3d00 0000 724e 0000  ..rc...r=...rN..
+000019b0: 0072 3300 0000 723e 0000 00da 0c43 4f4e  .r3...r>.....CON
 000019c0: 5445 4e54 5f52 4f4f 5472 0600 0000 7205  TENT_ROOTr....r.
-000019d0: 0000 0072 8600 0000 7277 0000 0072 5c00  ...r....rw...r\.
+000019d0: 0000 0072 8500 0000 7276 0000 0072 5b00  ...r....rv...r[.
 000019e0: 0000 da06 7265 6e64 6572 7223 0000 0029  ....renderr#...)
-000019f0: 0872 1800 0000 7292 0000 0072 9300 0000  .r....r....r....
-00001a00: da05 6672 616d 6572 9700 0000 7213 0000  ..framer....r...
+000019f0: 0872 1800 0000 7291 0000 0072 9200 0000  .r....r....r....
+00001a00: da05 6672 616d 6572 9600 0000 7213 0000  ..framer....r...
 00001a10: 005a 0f63 6f6e 7465 6e74 5f61 6273 7061  .Z.content_abspa
 00001a20: 7468 da08 7465 6d70 6c61 7465 721d 0000  th..templater...
 00001a30: 0072 1d00 0000 721e 0000 00da 115f 7265  .r....r......_re
 00001a40: 6e64 6572 5f65 7863 6570 7469 6f6e 1c01  nder_exception..
 00001a50: 0000 734c 0000 0000 0104 071a 0106 0104  ..sL............
 00001a60: 020a 010e 0204 010c ff02 030e 0204 010a  ................
 00001a70: ff06 040a 060c 0106 0108 0104 fe04 060a  ................
@@ -440,40 +440,40 @@
 00001b70: 0457 0059 0064 007d 057e 056e 0a64 007d  .W.Y.d.}.~.n.d.}
 00001b80: 057e 0530 0030 007c 0373 b47c 0482 017a  .~.0.0.|.s.|...z
 00001b90: 1064 057c 00a0 0a7c 04a1 0166 0257 0053  .d.|...|...f.W.S
 00001ba0: 0004 0074 0790 0079 fa01 007d 0501 007a  ...t...y...}...z
 00001bb0: 1c74 086a 0b64 067c 0564 0164 048d 0301  .t.j.d.|.d.d....
 00001bc0: 0057 0059 0064 007d 057e 056e 0a64 007d  .W.Y.d.}.~.n.d.}
 00001bd0: 057e 0530 0030 007c 0482 0164 0053 0029  .~.0.0.|...d.S.)
-00001be0: 074e 5472 3d00 0000 da0e 5f70 6172 7369  .NTr=....._parsi
+00001be0: 074e 5472 3c00 0000 da0e 5f70 6172 7369  .NTr<....._parsi
 00001bf0: 6e67 5f65 7272 6f72 2901 da08 6578 635f  ng_error)...exc_
 00001c00: 696e 666f 467a 2545 7863 6570 7469 6f6e  infoFz%Exception
 00001c10: 206f 6363 7572 7265 6420 7768 696c 6520   occurred while 
-00001c20: 7265 6e64 6572 696e 6720 2573 290c 7234  rendering %s).r4
-00001c30: 0000 0072 3f00 0000 7240 0000 0072 7500  ...r?...r@...ru.
-00001c40: 0000 7274 0000 0072 5c00 0000 7299 0000  ..rt...r\...r...
-00001c50: 0072 5f00 0000 7243 0000 00da 0564 6562  .r_...rC.....deb
-00001c60: 7567 729c 0000 0072 4400 0000 2906 7218  ugr....rD...).r.
-00001c70: 0000 0072 6000 0000 da10 7465 6d70 6c61  ...r`.....templa
+00001c20: 7265 6e64 6572 696e 6720 2573 290c 7233  rendering %s).r3
+00001c30: 0000 0072 3e00 0000 723f 0000 0072 7400  ...r>...r?...rt.
+00001c40: 0000 7273 0000 0072 5b00 0000 7298 0000  ..rs...r[...r...
+00001c50: 0072 5e00 0000 7242 0000 00da 0564 6562  .r^...rB.....deb
+00001c60: 7567 729b 0000 0072 4300 0000 2906 7218  ugr....rC...).r.
+00001c70: 0000 0072 5f00 0000 da10 7465 6d70 6c61  ...r_.....templa
 00001c80: 7465 5f63 6f6e 7465 7874 da11 6861 6e64  te_context..hand
-00001c90: 6c65 5f65 7863 6570 7469 6f6e 7372 9200  le_exceptionsr..
+00001c90: 6c65 5f65 7863 6570 7469 6f6e 7372 9100  le_exceptionsr..
 00001ca0: 0000 da01 6572 1d00 0000 721d 0000 0072  ....er....r....r
 00001cb0: 1e00 0000 da07 5f72 656e 6465 7263 0100  ......_renderc..
 00001cc0: 0073 3600 0000 0001 0a01 08ff 0203 1201  .s6.............
 00001cd0: 02ff 0803 0801 0aff 0203 0e03 0402 0201  ................
 00001ce0: 1201 02ff 0a03 0e01 0e01 1a02 0401 0402  ................
 00001cf0: 0201 1002 1001 0601 04ff 1c03 7a0e 4a69  ............z.Ji
 00001d00: 6e6a 6132 2e5f 7265 6e64 6572 6304 0000  nja2._renderc...
 00001d10: 0000 0000 0000 0000 0004 0000 0005 0000  ................
 00001d20: 0043 0000 0073 1200 0000 7c00 a000 7c01  .C...s....|...|.
 00001d30: 7c02 7c03 a103 6401 1900 5300 2902 4e72  |.|...d...S.).Nr
-00001d40: 4800 0000 2901 72a3 0000 0029 0472 1800  H...).r....).r..
-00001d50: 0000 7260 0000 0072 a000 0000 72a1 0000  ..r`...r....r...
+00001d40: 4700 0000 2901 72a2 0000 0029 0472 1800  G...).r....).r..
+00001d50: 0000 725f 0000 0072 9f00 0000 72a0 0000  ..r_...r....r...
 00001d60: 0072 1d00 0000 721d 0000 0072 1e00 0000  .r....r....r....
-00001d70: 7299 0000 0086 0100 0073 0a00 0000 0001  r........s......
+00001d70: 7298 0000 0086 0100 0073 0a00 0000 0001  r........s......
 00001d80: 0401 06ff 0201 02ff 7a0d 4a69 6e6a 6132  ........z.Jinja2
 00001d90: 2e72 656e 6465 7263 0300 0000 0000 0000  .renderc........
 00001da0: 0000 0000 0800 0000 0900 0000 4300 0000  ............C...
 00001db0: 7356 0100 007c 0164 0119 0072 1464 027c  sV...|.d...r.d.|
 00001dc0: 0164 0119 0076 0172 2064 037c 0164 0119  .d...v.r d.|.d..
 00001dd0: 0066 0253 007c 006a 006a 016a 0272 347c  .f.S.|.j.j.j.r4|
 00001de0: 006a 006a 016a 0373 587c 006a 04a0 057c  .j.j.j.sX|.j...|
@@ -492,71 +492,71 @@
 00001eb0: 0001 0001 0059 0001 007c 00a0 187c 067c  .....Y...|...|.|
 00001ec0: 02a1 0257 007c 0490 0172 2e7c 047c 006a  ...W.|...r.|.|.j
 00001ed0: 1576 0090 0172 2e7c 006a 15a0 197c 04a1  .v...r.|.j...|..
 00001ee0: 0101 0053 006e 207c 0490 0172 507c 047c  ...S.n |...rP|.|
 00001ef0: 006a 1576 0090 0172 507c 006a 15a0 197c  .j.v...rP|.j...|
 00001f00: 04a1 0101 0030 0064 0053 0029 0a4e da0c  .....0.d.S.).N..
 00001f10: 636f 6e74 656e 745f 626f 6479 da01 7b54  content_body..{T
-00001f20: 7224 0000 0072 3e00 0000 7290 0000 007a  r$...r>...r....z
-00001f30: 047b 7d7b 7d72 4800 0000 7a02 772b 291a  .{}{}rH...z.w+).
-00001f40: 7234 0000 0072 3f00 0000 7240 0000 0072  r4...r?...r@...r
-00001f50: 7500 0000 7274 0000 00da 0b66 726f 6d5f  u...rt.....from_
-00001f60: 7374 7269 6e67 7299 0000 0072 4e00 0000  stringr....rN...
+00001f20: 7224 0000 0072 3d00 0000 728f 0000 007a  r$...r=...r....z
+00001f30: 047b 7d7b 7d72 4700 0000 7a02 772b 291a  .{}{}rG...z.w+).
+00001f40: 7233 0000 0072 3e00 0000 723f 0000 0072  r3...r>...r?...r
+00001f50: 7400 0000 7273 0000 00da 0b66 726f 6d5f  t...rs.....from_
+00001f60: 7374 7269 6e67 7298 0000 0072 4d00 0000  stringr....rM...
 00001f70: da07 6861 7368 6c69 62da 036d 6435 7228  ..hashlib..md5r(
 00001f80: 0000 00da 0864 6174 6574 696d 65da 036e  .....datetime..n
 00001f90: 6f77 da06 656e 636f 6465 da09 6865 7864  ow..encode..hexd
-00001fa0: 6967 6573 7472 6400 0000 723e 0000 0072  igestrd...r>...r
-00001fb0: 9100 0000 724f 0000 0072 7100 0000 7237  ....rO...rq...r7
-00001fc0: 0000 0072 5100 0000 7281 0000 00da 0577  ...rQ...r......w
-00001fd0: 7269 7465 72a3 0000 0072 8500 0000 2908  riter....r....).
-00001fe0: 7218 0000 0072 3d00 0000 72a0 0000 0072  r....r=...r....r
-00001ff0: 9b00 0000 723e 0000 0072 1300 0000 7237  ....r>...r....r7
+00001fa0: 6967 6573 7472 6300 0000 723d 0000 0072  igestrc...r=...r
+00001fb0: 9000 0000 724e 0000 0072 7000 0000 7236  ....rN...rp...r6
+00001fc0: 0000 0072 5000 0000 7280 0000 00da 0577  ...rP...r......w
+00001fd0: 7269 7465 72a2 0000 0072 8400 0000 2908  riter....r....).
+00001fe0: 7218 0000 0072 3c00 0000 729f 0000 0072  r....r<...r....r
+00001ff0: 9a00 0000 723d 0000 0072 1300 0000 7236  ....r=...r....r6
 00002000: 0000 00da 0166 721d 0000 0072 1d00 0000  .....fr....r....
 00002010: 721e 0000 00da 1270 7265 5f72 656e 6465  r......pre_rende
 00002020: 725f 636f 6e74 656e 748a 0100 0073 3c00  r_content....s<.
 00002030: 0000 0001 1401 0c02 0a01 08ff 0203 1002  ................
 00002040: 1402 0402 0201 0802 0401 0801 0a03 0402  ................
 00002050: 0401 1a01 0efe 0405 1201 0a02 0c01 2c02  ..............,.
 00002060: 0c03 1201 0cfc 0203 0001 02ff 1201 7a19  ..............z.
 00002070: 4a69 6e6a 6132 2e70 7265 5f72 656e 6465  Jinja2.pre_rende
 00002080: 725f 636f 6e74 656e 7429 0154 2901 5429  r_content).T).T)
 00002090: 0154 290a 721f 0000 0072 2000 0000 7221  .T).r....r ...r!
-000020a0: 0000 0072 1700 0000 726e 0000 0072 9c00  ...r....rn...r..
-000020b0: 0000 72a3 0000 0072 9900 0000 72af 0000  ..r....r....r...
+000020a0: 0000 0072 1700 0000 726d 0000 0072 9b00  ...r....rm...r..
+000020b0: 0000 72a2 0000 0072 9800 0000 72ae 0000  ..r....r....r...
 000020c0: 0072 2200 0000 721d 0000 0072 1d00 0000  .r"...r....r....
-000020d0: 721b 0000 0072 1e00 0000 7262 0000 00c2  r....r....rb....
+000020d0: 721b 0000 0072 1e00 0000 7261 0000 00c2  r....r....ra....
 000020e0: 0000 0073 0c00 0000 0801 0c2a 0a2f 0847  ...s.......*./.G
-000020f0: 0a23 0a04 7262 0000 0029 3572 9400 0000  .#..rb...)5r....
-00002100: 72a9 0000 0072 6f00 0000 72a7 0000 00da  r....ro...r.....
+000020f0: 0a23 0a04 7261 0000 0029 3572 9300 0000  .#..ra...)5r....
+00002100: 72a8 0000 0072 6e00 0000 72a6 0000 00da  r....rn...r.....
 00002110: 076c 6f67 6769 6e67 7231 0000 0072 2900  .loggingr1...r).
-00002120: 0000 7264 0000 00da 066a 696e 6a61 3272  ..rd.....jinja2r
+00002120: 0000 7263 0000 00da 066a 696e 6a61 3272  ..rc.....jinja2r
 00002130: 0200 0000 7203 0000 0072 0400 0000 7205  ....r....r....r.
 00002140: 0000 0072 0600 0000 5a1d 666c 616d 696e  ...r....Z.flamin
 00002150: 676f 2e63 6f72 652e 7465 6d70 6c61 7469  go.core.templati
 00002160: 6e67 2e62 6173 6572 0700 0000 da1b 666c  ng.baser......fl
 00002170: 616d 696e 676f 2e63 6f72 652e 7574 696c  amingo.core.util
 00002180: 732e 696d 706f 7274 7372 0900 0000 da1a  s.importsr......
 00002190: 666c 616d 696e 676f 2e63 6f72 652e 7574  flamingo.core.ut
 000021a0: 696c 732e 7070 7269 6e74 720a 0000 00da  ils.pprintr.....
 000021b0: 0866 6c61 6d69 6e67 6f72 0b00 0000 5a13  .flamingor....Z.
 000021c0: 7079 676d 656e 7473 2e66 6f72 6d61 7474  pygments.formatt
 000021d0: 6572 7372 0c00 0000 da0f 7079 676d 656e  ersr......pygmen
 000021e0: 7473 2e6c 6578 6572 7372 0d00 0000 720e  ts.lexersr....r.
 000021f0: 0000 00da 0d70 7967 6d65 6e74 732e 7574  .....pygments.ut
 00002200: 696c 720f 0000 00da 0870 7967 6d65 6e74  ilr......pygment
-00002210: 7372 1000 0000 7287 0000 005a 0850 5947  sr....r....Z.PYG
+00002210: 7372 1000 0000 7286 0000 005a 0850 5947  sr....r....Z.PYG
 00002220: 4d45 4e54 53da 0b49 6d70 6f72 7445 7272  MENTS..ImportErr
-00002230: 6f72 722f 0000 0072 2e00 0000 723e 0000  orr/...r....r>..
-00002240: 0072 4f00 0000 da07 6469 726e 616d 65da  .rO.....dirname.
+00002230: 6f72 722f 0000 0072 2e00 0000 723d 0000  orr/...r....r=..
+00002240: 0072 4e00 0000 da07 6469 726e 616d 65da  .rN.....dirname.
 00002250: 085f 5f66 696c 655f 5f5a 0e45 5252 4f52  .__file__Z.ERROR
 00002260: 5f54 454d 504c 4154 45da 0967 6574 4c6f  _TEMPLATE..getLo
-00002270: 6767 6572 7243 0000 0072 5f00 0000 7211  ggerrC...r_...r.
+00002270: 6767 6572 7242 0000 0072 5e00 0000 7211  ggerrB...r^...r.
 00002280: 0000 0072 2300 0000 7226 0000 0072 2c00  ...r#...r&...r,.
-00002290: 0000 7235 0000 0072 3600 0000 7258 0000  ..r5...r6...rX..
-000022a0: 0072 5900 0000 7262 0000 0072 1d00 0000  .rY...rb...r....
+00002290: 0000 7234 0000 0072 3500 0000 7257 0000  ..r4...r5...rW..
+000022a0: 0072 5800 0000 7261 0000 0072 1d00 0000  .rX...ra...r....
 000022b0: 721d 0000 0072 1d00 0000 721e 0000 00da  r....r....r.....
 000022c0: 083c 6d6f 6475 6c65 3e01 0000 0073 5200  .<module>....sR.
 000022d0: 0000 0801 0801 0801 0801 0801 0801 0801  ................
 000022e0: 0802 1401 1002 0c01 0c01 0c01 0c02 0201  ................
 000022f0: 0c01 1001 0c01 0c02 0802 0c01 0a02 0201  ................
 00002300: 0802 0802 0e01 0a02 1602 0a03 100a 1004  ................
 00002310: 0807 0807 0201 0a08 0804 0201 0801 04ff  ................
```

### Comparing `flamingo-1.8/flamingo/core/templating/base.py` & `flamingo-1.9/flamingo/core/templating/base.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/templating/jinja2.py` & `flamingo-1.9/flamingo/core/templating/jinja2.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,15 +213,15 @@
         )
 
         self.env.globals['link'] = link
         self.env.globals['import'] = _import
         self.env.globals['_shell'] = _shell
 
         # setup error env
-        if(self.context.settings. LIVE_SERVER_RUNNING and
+        if (self.context.settings. LIVE_SERVER_RUNNING and
            self.context.settings.JINJA2_TRACEBACKS):
 
             autoescape = not self.context.settings.JINJA2_TRACEBACKS_PYGMENTS
 
             self.error_env = Environment(
                 loader=FileSystemLoader(
                     [os.path.join(THEME_ROOT, 'templates/jinja2')]),
@@ -292,15 +292,15 @@
         for frame in traceback.extract_tb(exception.__traceback__)[::-1]:
             filename = frame.filename
             content_path = ''
 
             if filename in self.contents:
                 content_path = self.contents[filename]['path']
 
-                if(not content_path and
+                if (not content_path and
                    self.contents[filename]['original_path']):
 
                     content_path = self.contents[filename]['original_path']
 
             stack.append(
                 (filename, frame.lineno, content_path, )
             )
@@ -349,21 +349,21 @@
             stack=stack,
             TemplateNotFound=TemplateNotFound,
             LinkError=LinkError,
             isinstance=isinstance,
         )
 
     def _render(self, template_name, template_context, handle_exceptions=True):
-        if(not self.context.settings.LIVE_SERVER_RUNNING or
+        if (not self.context.settings.LIVE_SERVER_RUNNING or
            not self.context.settings.JINJA2_TRACEBACKS):
 
             return True, self.env.get_template(template_name).render(
                 **template_context)
 
-        if('content' in template_context and
+        if ('content' in template_context and
            '_parsing_error' in template_context['content']):
 
             exception = template_context['content']['_parsing_error']
 
         else:
             exception = None
 
@@ -391,15 +391,15 @@
         return self._render(
             template_name, template_context, handle_exceptions)[1]
 
     def pre_render_content(self, content, template_context):
         if not content['content_body'] or '{' not in content['content_body']:
             return True, content['content_body']
 
-        if(not self.context.settings.LIVE_SERVER_RUNNING or
+        if (not self.context.settings.LIVE_SERVER_RUNNING or
            not self.context.settings.JINJA2_TRACEBACKS):
 
             template = self.env.from_string(content['content_body'])
 
             return True, template.render(**template_context)
 
         path = ''
```

### Comparing `flamingo-1.8/flamingo/core/types.py` & `flamingo-1.9/flamingo/core/types.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/aiohttp.cpython-310.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/aiohttp.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/aiohttp.cpython-35.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/aiohttp.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/aiohttp.cpython-37.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/aiohttp.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/aiohttp.cpython-39.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/aiohttp.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/aionotify.cpython-35.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/aionotify.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/cli.cpython-310.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/cli.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/cli.cpython-35.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/cli.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/cli.cpython-37.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/cli.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/cli.cpython-39.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/cli.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/html.cpython-310.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/html.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/html.cpython-35.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/html.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/html.cpython-37.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/html.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/html.cpython-39.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/html.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/imports.cpython-310.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/imports.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/imports.cpython-35.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/imports.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/imports.cpython-37.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/imports.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/imports.cpython-39.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/imports.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/pagination.cpython-310.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/pagination.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/pagination.cpython-35.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/pagination.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/pagination.cpython-37.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/pagination.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/pagination.cpython-39.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/pagination.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/pprint.cpython-310.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/pprint.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/pprint.cpython-35.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/pprint.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/pprint.cpython-37.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/pprint.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/pprint.cpython-39.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/pprint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/string.cpython-310.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/string.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/string.cpython-35.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/string.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/string.cpython-37.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/string.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/__pycache__/string.cpython-39.pyc` & `flamingo-1.9/flamingo/core/utils/__pycache__/string.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/cli.py` & `flamingo-1.9/flamingo/core/utils/cli.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/html.py` & `flamingo-1.9/flamingo/core/utils/html.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/imports.py` & `flamingo-1.9/flamingo/core/utils/imports.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/pagination.py` & `flamingo-1.9/flamingo/core/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/pprint.py` & `flamingo-1.9/flamingo/core/utils/pprint.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/core/utils/string.py` & `flamingo-1.9/flamingo/core/utils/string.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__init__.py` & `flamingo-1.9/flamingo/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/__init__.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu May 12 16:46:39 2022 UTC, .py size: 1304 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ef39 7d62 1805 0000  o........9}b....
+00000000: 6f0d 0d0a 0000 0000 161c 6863 1805 0000  o.........hc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 a801 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 0100 6400 6405 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6400 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/__init__.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/__init__.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/__init__.cpython-37.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/__init__.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May 12 16:46:39 2022 UTC, .py size: 1304 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 ef39 7d62 1805 0000  a........9}b....
+00000000: 610d 0d0a 0000 0000 161c 6863 1805 0000  a.........hc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 b201 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 0100 6400 6405 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6400 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/authors.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/authors.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/feeds.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/feeds.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Dec  6 19:14:04 2021 UTC, .py size: 3352 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 fc60 ae61 180d 0000  o........`.a....
+00000000: 6f0d 0d0a 0000 0000 2518 6863 180d 0000  o.......%.hc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6500 a003 6403 a101 5a04 4700 6404  ..e...d...Z.G.d.
 00000050: 6405 8400 6405 8302 5a05 6401 5300 2906  d...d...Z.d.S.).
 00000060: e900 0000 004e 2901 da0d 4665 6564 4765  .....N)...FeedGe
 00000070: 6e65 7261 746f 727a 1666 6c61 6d69 6e67  neratorz.flaming
```

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/feeds.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/feeds.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/feeds.cpython-37.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/feeds.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/git.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/git.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/git.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/git.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/git.cpython-37.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/git.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/git.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/git.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/html.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/html.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/html.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/html.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/html.cpython-37.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/html.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/html.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/html.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/i18n.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/i18n.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/i18n.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/i18n.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/i18n.cpython-37.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/i18n.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/i18n.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/i18n.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/layers.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/layers.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/md.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/md.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/md.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/md.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/md.cpython-37.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/md.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/md.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/md.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/redirects.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/redirects.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/redirects.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/redirects.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/redirects.cpython-37.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/redirects.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/redirects.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/redirects.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/tags.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/tags.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/thumbnails.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/thumbnails.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/thumbnails.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/thumbnails.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/thumbnails.cpython-37.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/thumbnails.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/thumbnails.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/thumbnails.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Dec  6 19:14:04 2021 UTC, .py size: 9260 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 fc60 ae61 2c24 0000  a........`.a,$..
+00000000: 610d 0d0a 0000 0000 5399 7c63 2d24 0000  a.......S.|c-$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6400 6402 6c05 5a05 7a14 6400 6403  Z.d.d.l.Z.z.d.d.
 00000060: 6c06 6d07 5a07 0100 6404 5a08 5700 6e16  l.m.Z...d.Z.W.n.
 00000070: 0400 6509 7956 0100 0100 0100 6405 5a08  ..e.yV......d.Z.
```

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/time.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/time.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/time.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/time.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/time.cpython-37.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/time.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/time.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/time.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/yaml.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/yaml.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/yaml.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/yaml.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/yaml.cpython-37.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/yaml.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/__pycache__/yaml.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/__pycache__/yaml.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/authors/__pycache__/authors.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/authors/__pycache__/authors.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/authors/__pycache__/authors.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/authors/__pycache__/authors.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/authors/__pycache__/authors.cpython-37.pyc` & `flamingo-1.9/flamingo/plugins/authors/__pycache__/authors.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/authors/__pycache__/authors.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/authors/__pycache__/authors.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/authors/authors.py` & `flamingo-1.9/flamingo/plugins/authors/authors.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/__pycache__/plugins.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/bootstrap/__pycache__/plugins.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/__pycache__/plugins.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/bootstrap/__pycache__/plugins.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/__pycache__/plugins.cpython-37.pyc` & `flamingo-1.9/flamingo/plugins/bootstrap/__pycache__/plugins.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/__pycache__/plugins.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/bootstrap/__pycache__/plugins.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap-theme.css` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap-theme.css.map` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap-theme.min.css` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap-theme.min.css.map` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap-theme.min.css.map`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap.css` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap.css.map` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap.min.css` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap.min.css.map` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/fonts/glyphicons-halflings-regular.eot` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/fonts/glyphicons-halflings-regular.svg` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/fonts/glyphicons-halflings-regular.ttf` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/fonts/glyphicons-halflings-regular.woff` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/fonts/glyphicons-halflings-regular.woff2` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/js/bootstrap.js` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/js/bootstrap.min.js` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-3/static/bootstrap-3.4.1/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-grid.css` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-grid.css.map` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-grid.min.css` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-grid.min.css.map` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-reboot.css` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-reboot.css.map` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-reboot.min.css` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-reboot.min.css.map` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap.css` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap.css.map` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap.min.css` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap.min.css.map` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.bundle.js` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.bundle.js.map` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.bundle.min.js` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.bundle.min.js.map` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.js` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.js.map` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.min.js` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.min.js.map` & `flamingo-1.9/flamingo/plugins/bootstrap/theme/bootstrap-4/static/bootstrap-4.3.1/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/git.py` & `flamingo-1.9/flamingo/plugins/git.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/html.py` & `flamingo-1.9/flamingo/plugins/html.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/i18n.py` & `flamingo-1.9/flamingo/plugins/i18n.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/jquery/__pycache__/plugins.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/jquery/__pycache__/plugins.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/jquery/__pycache__/plugins.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/jquery/__pycache__/plugins.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/jquery/__pycache__/plugins.cpython-37.pyc` & `flamingo-1.9/flamingo/plugins/jquery/__pycache__/plugins.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/jquery/__pycache__/plugins.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/jquery/__pycache__/plugins.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/jquery/theme/jquery-1/static/jquery/jquery-1.12.4.js` & `flamingo-1.9/flamingo/plugins/jquery/theme/jquery-1/static/jquery/jquery-1.12.4.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/jquery/theme/jquery-1/static/jquery/jquery-1.12.4.min.js` & `flamingo-1.9/flamingo/plugins/jquery/theme/jquery-1/static/jquery/jquery-1.12.4.min.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/jquery/theme/jquery-2/static/jquery/jquery-2.2.4.js` & `flamingo-1.9/flamingo/plugins/jquery/theme/jquery-2/static/jquery/jquery-2.2.4.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/jquery/theme/jquery-2/static/jquery/jquery-2.2.4.min.js` & `flamingo-1.9/flamingo/plugins/jquery/theme/jquery-2/static/jquery/jquery-2.2.4.min.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/jquery/theme/jquery-3/static/jquery/jquery-3.4.1.js` & `flamingo-1.9/flamingo/plugins/jquery/theme/jquery-3/static/jquery/jquery-3.4.1.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/jquery/theme/jquery-3/static/jquery/jquery-3.4.1.min.js` & `flamingo-1.9/flamingo/plugins/jquery/theme/jquery-3/static/jquery/jquery-3.4.1.min.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/jquery/theme/jquery-3/static/jquery/jquery-3.4.1.slim.js` & `flamingo-1.9/flamingo/plugins/jquery/theme/jquery-3/static/jquery/jquery-3.4.1.slim.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/jquery/theme/jquery-3/static/jquery/jquery-3.4.1.slim.min.js` & `flamingo-1.9/flamingo/plugins/jquery/theme/jquery-3/static/jquery/jquery-3.4.1.slim.min.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/md.py` & `flamingo-1.9/flamingo/plugins/md.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/menu/__pycache__/menu.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/menu/__pycache__/menu.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/menu/__pycache__/menu.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/menu/__pycache__/menu.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/menu/__pycache__/menu.cpython-37.pyc` & `flamingo-1.9/flamingo/plugins/menu/__pycache__/menu.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/menu/__pycache__/menu.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/menu/__pycache__/menu.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Dec  6 19:14:04 2021 UTC, .py size: 5587 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 fc60 ae61 d315 0000  a........`.a....
+00000000: 610d 0d0a 0000 0000 5399 7c63 d415 0000  a.......S.|c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 6400 6404 6c07  m.Z.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6400 6405 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6502 a00c 6406 a101 5a0d  m.Z...e...d...Z.
```

### Comparing `flamingo-1.8/flamingo/plugins/menu/menu.py` & `flamingo-1.9/flamingo/plugins/menu/menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                     return True
 
         return False
 
     if isinstance(section, Section) and section.content is content:
         return True
 
-    if(isinstance(section, Section) and
+    if (isinstance(section, Section) and
        isinstance(content['menu_path'], list) and
        section in content['menu_path']):
 
         return True
 
     if isinstance(menu, Content):
         return menu is content
```

### Comparing `flamingo-1.8/flamingo/plugins/menu/theme/templates/menu/bootstrap3.html` & `flamingo-1.9/flamingo/plugins/menu/theme/templates/menu/bootstrap3.html`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/menu/theme/templates/menu/bootstrap4.html` & `flamingo-1.9/flamingo/plugins/menu/theme/templates/menu/bootstrap4.html`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/photoswipe/__pycache__/utils.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/photoswipe/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/photoswipe/__pycache__/utils.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/photoswipe/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/photoswipe/theme/static/photoswipe/default-skin/default-skin.css` & `flamingo-1.9/flamingo/plugins/photoswipe/theme/static/photoswipe/default-skin/default-skin.css`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/photoswipe/theme/static/photoswipe/default-skin/default-skin.png` & `flamingo-1.9/flamingo/plugins/photoswipe/theme/static/photoswipe/default-skin/default-skin.png`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/photoswipe/theme/static/photoswipe/default-skin/default-skin.svg` & `flamingo-1.9/flamingo/plugins/photoswipe/theme/static/photoswipe/default-skin/default-skin.svg`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/photoswipe/theme/static/photoswipe/default-skin/preloader.gif` & `flamingo-1.9/flamingo/plugins/photoswipe/theme/static/photoswipe/default-skin/preloader.gif`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/photoswipe/theme/static/photoswipe/photoswipe-init.js` & `flamingo-1.9/flamingo/plugins/photoswipe/theme/static/photoswipe/photoswipe-init.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/photoswipe/theme/static/photoswipe/photoswipe-ui-default.js` & `flamingo-1.9/flamingo/plugins/photoswipe/theme/static/photoswipe/photoswipe-ui-default.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/photoswipe/theme/static/photoswipe/photoswipe-ui-default.min.js` & `flamingo-1.9/flamingo/plugins/photoswipe/theme/static/photoswipe/photoswipe-ui-default.min.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/photoswipe/theme/static/photoswipe/photoswipe.css` & `flamingo-1.9/flamingo/plugins/photoswipe/theme/static/photoswipe/photoswipe.css`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/photoswipe/theme/static/photoswipe/photoswipe.js` & `flamingo-1.9/flamingo/plugins/photoswipe/theme/static/photoswipe/photoswipe.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/photoswipe/theme/static/photoswipe/photoswipe.min.js` & `flamingo-1.9/flamingo/plugins/photoswipe/theme/static/photoswipe/photoswipe.min.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/photoswipe/theme/templates/photoswipe/gallery.html` & `flamingo-1.9/flamingo/plugins/photoswipe/theme/templates/photoswipe/gallery.html`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/photoswipe/theme/templates/photoswipe/photoswipe.html` & `flamingo-1.9/flamingo/plugins/photoswipe/theme/templates/photoswipe/photoswipe.html`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/photoswipe/utils.py` & `flamingo-1.9/flamingo/plugins/photoswipe/utils.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/redirects.py` & `flamingo-1.9/flamingo/plugins/redirects.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/base.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/base.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/base.cpython-37.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/base.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/bootstrap3.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/bootstrap3.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/bootstrap3.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/bootstrap3.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/bootstrap3.cpython-37.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/bootstrap3.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/bootstrap3.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/bootstrap3.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/directives.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/directives.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/directives.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/directives.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/file.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/file.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/file.cpython-37.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/file.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/image.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/image.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/image.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/image.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/image.cpython-37.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/image.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/image.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/image.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/include.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/include.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/include.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/include.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/include.cpython-37.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/include.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/include.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/include.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Dec  6 19:14:04 2021 UTC, .py size: 4629 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 fc60 ae61 1512 0000  a........`.a....
+00000000: 610d 0d0a 0000 0000 5399 7c63 1612 0000  a.......S.|c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 6d0a 5a0a 0100 6400  d.l.m.Z.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 6d0d 5a0d 0100 6400  d.l.m.Z.m.Z...d.
```

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/link.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/link.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/link.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/link.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Aug 14 13:04:36 2020 UTC, .py size: 3360 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 e48b 365f 200d 0000  a.........6_ ...
+00000000: 610d 0d0a 0000 0000 5399 7c63 210d 0000  a.......S.|c!...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 0100 6404  Z.d.d.l.m.Z...d.
 00000050: 6405 6c05 6d06 5a06 6d07 5a07 6d08 5a08  d.l.m.Z.m.Z.m.Z.
 00000060: 0100 4700 6406 6407 8400 6407 8302 5a09  ..G.d.d...d...Z.
 00000070: 4700 6408 6409 8400 6409 8302 5a0a 6402  G.d.d...d...Z.d.
```

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/parser.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/parser.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/parser.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/parser.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/plugin.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/plugin.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/plugin.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/plugin.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Dec  6 19:14:04 2021 UTC, .py size: 2577 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 fc60 ae61 110a 0000  a........`.a....
+00000000: 610d 0d0a 0000 0000 5399 7c63 150a 0000  a.......S.|c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6400 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6500 a00b 6407 a101 5a0c 4700 6408  ..e...d...Z.G.d.
```

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/pygments.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/pygments.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/pygments.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/pygments.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/pygments.cpython-37.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/pygments.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/pygments.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/pygments.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/table.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/table.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/table.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/table.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/utils.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/__pycache__/utils.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/rst/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/bootstrap3.py` & `flamingo-1.9/flamingo/plugins/rst/bootstrap3.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/directives.py` & `flamingo-1.9/flamingo/plugins/rst/directives.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/image.py` & `flamingo-1.9/flamingo/plugins/rst/image.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/include.py` & `flamingo-1.9/flamingo/plugins/rst/include.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             context.content['related_paths'].append(content['path'])
 
             # parse included content if content_body is present yet
             if not content['content_body']:
                 context.parse(content)
 
             # check arguments
-            if('section' in self.options and
+            if ('section' in self.options and
                'title' in self.options):
 
                 logger.error(
                     "%s:%s has no ambiguous arguments",
                     context.content['path'],
                     lineno,
                 )
```

### Comparing `flamingo-1.8/flamingo/plugins/rst/link.py` & `flamingo-1.9/flamingo/plugins/rst/link.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                 format='html')
             ], []
 
         # handle internal links
         abs_lineno = self.rst_base_plugin.offsets.get(
             self.context.content['path'], 0) + lineno
 
-        if(not self.context.settings.PRE_RENDER_CONTENT or
+        if (not self.context.settings.PRE_RENDER_CONTENT or
            not self.context.content.get('is_template', True)):
 
             self.context.logger.error(
                 '%s:%s: LinkError: internal links depend on content pre rendering which is disabled by your %s',  # NOQA
                 self.context.content['path'],
                 abs_lineno,
                 ('settings'
```

### Comparing `flamingo-1.8/flamingo/plugins/rst/parser.py` & `flamingo-1.9/flamingo/plugins/rst/parser.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/plugin.py` & `flamingo-1.9/flamingo/plugins/rst/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,32 +51,32 @@
         register_directive('div', _Container)
 
     def rst_document_parsed(self, context, document):
         """
         This hook removes all docutils system messages from docutils documents
         """
 
-        if(not context.settings.get(
+        if (not context.settings.get(
                'RST_REMOVE_SYSTEM_MESSAGES_FROM_OUPUT', True)):
 
             return
 
         logger.debug('%s: removing system messages', context.content['path'])
 
         removed = [0]
 
         def remove_system_messages(children, removed):
             for child in children[::]:
                 if isinstance(child, system_message):
                     children.remove(child)
                     removed[0] += 1
 
-                elif(hasattr(child, 'attributes') and
-                     'classes' in child.attributes and
-                     'system-messages' in child.attributes['classes']):
+                elif (hasattr(child, 'attributes') and
+                      'classes' in child.attributes and
+                      'system-messages' in child.attributes['classes']):
 
                     children.remove(child)
                     removed[0] += 1
 
                 elif child.children:
                     remove_system_messages(child.children, removed)
```

### Comparing `flamingo-1.8/flamingo/plugins/rst/pygments.py` & `flamingo-1.9/flamingo/plugins/rst/pygments.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/table.py` & `flamingo-1.9/flamingo/plugins/rst/table.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rst/utils.py` & `flamingo-1.9/flamingo/plugins/rst/utils.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/__pycache__/plugin.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/rtd/__pycache__/plugin.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/__pycache__/plugin.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/rtd/__pycache__/plugin.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/__pycache__/plugin.cpython-37.pyc` & `flamingo-1.9/flamingo/plugins/rtd/__pycache__/plugin.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/__pycache__/plugin.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/rtd/__pycache__/plugin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/elasticlunr.js` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/elasticlunr.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/elasticlunr.min.js` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/elasticlunr.min.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/mark.js` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/mark.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/mark.min.js` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/mark.min.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/ractive.js` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/ractive.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/ractive.js.map` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/ractive.js.map`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/ractive.min.js` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/ractive.min.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/ractive.min.js.map` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/ractive.min.js.map`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/css/theme.css` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/css/theme.css`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/doctools.js` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/doctools.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bold.eot` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bold.eot`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bold.eot?` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bold.eot?`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bold.ttf` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bold.ttf`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bold.woff` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bold.woff2` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bolditalic.eot` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bolditalic.eot`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bolditalic.eot?` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bolditalic.eot?`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bolditalic.ttf` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bolditalic.ttf`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bolditalic.woff` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bolditalic.woff`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bolditalic.woff2` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-bolditalic.woff2`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-italic.eot` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-italic.eot`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-italic.eot?` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-italic.eot?`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-italic.ttf` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-italic.ttf`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-italic.woff` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-italic.woff`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-italic.woff2` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-italic.woff2`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-regular.eot` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-regular.eot`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-regular.eot?` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-regular.eot?`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-regular.ttf` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-regular.ttf`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-regular.woff` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-regular.woff`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-regular.woff2` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/Lato/lato-regular.woff2`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-bold.eot` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-bold.eot`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-bold.eot?` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-bold.eot?`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-bold.ttf` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-bold.ttf`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-bold.woff` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-bold.woff`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-bold.woff2` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-bold.woff2`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-regular.eot?` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-regular.eot?`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-regular.ttf` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-regular.ttf`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-regular.woff` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-regular.woff`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-regular.woff2` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/RobotoSlab/roboto-slab-v7-regular.woff2`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/fontawesome-webfont.eot` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/fontawesome-webfont.svg` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/fontawesome-webfont.ttf` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/fontawesome-webfont.woff` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/fonts/fontawesome-webfont.woff2` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/jquery.js` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/jquery.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/js/modernizr.min.js` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/js/modernizr.min.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/js/theme.js` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/js/theme.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/language_data.js` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/language_data.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/pygments.css` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/pygments.css`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/searchtools.js` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/searchtools.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/static/rtd/underscore.js` & `flamingo-1.9/flamingo/plugins/rtd/theme/static/rtd/underscore.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/templates/rtd/page.html` & `flamingo-1.9/flamingo/plugins/rtd/theme/templates/rtd/page.html`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/rtd/theme/templates/rtd/search.html` & `flamingo-1.9/flamingo/plugins/rtd/theme/templates/rtd/search.html`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/sphinx_themes/__pycache__/defaults.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/sphinx_themes/__pycache__/defaults.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu May 12 15:07:02 2022 UTC, .py size: 805 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9622 7d62 2503 0000  o........"}b%...
+00000000: 610d 0d0a 0000 0000 853e 7d62 2503 0000  a........>}b%...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 5a00 6900 5a01 6700 5a02 6700 5a03 6401  Z.i.Z.g.Z.g.Z.d.
 00000040: 5a04 6402 5a05 6403 5a06 6403 5a07 6403  Z.d.Z.d.Z.d.Z.d.
 00000050: 5a08 6403 5a09 6403 5a0a 6403 5a0b 6403  Z.d.Z.d.Z.d.Z.d.
 00000060: 5a0c 6403 5a0d 6403 5a0e 6403 5a0f 6403  Z.d.Z.d.Z.d.Z.d.
 00000070: 5a10 6403 5a11 6403 5a12 6404 5a13 6404  Z.d.Z.d.Z.d.Z.d.
@@ -19,15 +19,15 @@
 00000120: 0800 0000 fa54 2f68 6f6d 652f 6368 7269  .....T/home/chri
 00000130: 732f 776f 726b 2f50 726f 6a65 6374 732f  s/work/Projects/
 00000140: 6769 7468 7562 2f66 6c61 6d69 6e67 6f2f  github/flamingo/
 00000150: 666c 616d 696e 676f 2f70 6c75 6769 6e73  flamingo/plugins
 00000160: 2f73 7068 696e 785f 7468 656d 6573 2f64  /sphinx_themes/d
 00000170: 6566 6175 6c74 732e 7079 da15 5350 4849  efaults.py..SPHI
 00000180: 4e58 5f54 4845 4d45 535f 5645 5253 494f  NX_THEMES_VERSIO
-00000190: 4e1b 0000 0073 0200 0000 1001 720a 0000  N....s......r...
+00000190: 4e1b 0000 0073 0200 0000 0001 720a 0000  N....s......r...
 000001a0: 004e 2917 da18 5350 4849 4e58 5f54 4845  .N)...SPHINX_THE
 000001b0: 4d45 535f 4854 4d4c 5f54 4845 4d45 da20  MES_HTML_THEME. 
 000001c0: 5350 4849 4e58 5f54 4845 4d45 535f 4854  SPHINX_THEMES_HT
 000001d0: 4d4c 5f54 4845 4d45 5f4f 5054 494f 4e53  ML_THEME_OPTIONS
 000001e0: da1f 5350 4849 4e58 5f54 4845 4d45 535f  ..SPHINX_THEMES_
 000001f0: 4558 5452 415f 5354 594c 4553 4845 4554  EXTRA_STYLESHEET
 00000200: 53da 1b53 5048 494e 585f 5448 454d 4553  S..SPHINX_THEMES
@@ -59,11 +59,11 @@
 000003a0: 5448 454d 4553 5f53 484f 575f 434f 5059  THEMES_SHOW_COPY
 000003b0: 5249 4748 545a 1953 5048 494e 585f 5448  RIGHTZ.SPHINX_TH
 000003c0: 454d 4553 5f53 484f 575f 5350 4849 4e58  EMES_SHOW_SPHINX
 000003d0: 5a19 5350 4849 4e58 5f54 4845 4d45 535f  Z.SPHINX_THEMES_
 000003e0: 4449 5350 4c41 595f 544f 4372 0a00 0000  DISPLAY_TOCr....
 000003f0: 7208 0000 0072 0800 0000 7208 0000 0072  r....r....r....r
 00000400: 0900 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000410: 0000 732e 0000 0004 0004 0104 0104 0104  ..s.............
-00000420: 0104 0204 0204 0104 0104 0104 0104 0104  ................
+00000410: 0000 732c 0000 0004 0104 0104 0104 0104  ..s,............
+00000420: 0204 0204 0104 0104 0104 0104 0104 0104  ................
 00000430: 0104 0104 0104 0104 0104 0104 0104 0104  ................
-00000440: 0104 010c 03                             .....
+00000440: 0104 03                                  ...
```

### Comparing `flamingo-1.8/flamingo/plugins/sphinx_themes/__pycache__/defaults.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/sphinx_themes/__pycache__/defaults.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May 12 15:07:02 2022 UTC, .py size: 805 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 9622 7d62 2503 0000  a........"}b%...
+00000000: 6f0d 0d0a 0000 0000 853e 7d62 2503 0000  o........>}b%...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 5a00 6900 5a01 6700 5a02 6700 5a03 6401  Z.i.Z.g.Z.g.Z.d.
 00000040: 5a04 6402 5a05 6403 5a06 6403 5a07 6403  Z.d.Z.d.Z.d.Z.d.
 00000050: 5a08 6403 5a09 6403 5a0a 6403 5a0b 6403  Z.d.Z.d.Z.d.Z.d.
 00000060: 5a0c 6403 5a0d 6403 5a0e 6403 5a0f 6403  Z.d.Z.d.Z.d.Z.d.
 00000070: 5a10 6403 5a11 6403 5a12 6404 5a13 6404  Z.d.Z.d.Z.d.Z.d.
@@ -19,15 +19,15 @@
 00000120: 0800 0000 fa54 2f68 6f6d 652f 6368 7269  .....T/home/chri
 00000130: 732f 776f 726b 2f50 726f 6a65 6374 732f  s/work/Projects/
 00000140: 6769 7468 7562 2f66 6c61 6d69 6e67 6f2f  github/flamingo/
 00000150: 666c 616d 696e 676f 2f70 6c75 6769 6e73  flamingo/plugins
 00000160: 2f73 7068 696e 785f 7468 656d 6573 2f64  /sphinx_themes/d
 00000170: 6566 6175 6c74 732e 7079 da15 5350 4849  efaults.py..SPHI
 00000180: 4e58 5f54 4845 4d45 535f 5645 5253 494f  NX_THEMES_VERSIO
-00000190: 4e1b 0000 0073 0200 0000 0001 720a 0000  N....s......r...
+00000190: 4e1b 0000 0073 0200 0000 1001 720a 0000  N....s......r...
 000001a0: 004e 2917 da18 5350 4849 4e58 5f54 4845  .N)...SPHINX_THE
 000001b0: 4d45 535f 4854 4d4c 5f54 4845 4d45 da20  MES_HTML_THEME. 
 000001c0: 5350 4849 4e58 5f54 4845 4d45 535f 4854  SPHINX_THEMES_HT
 000001d0: 4d4c 5f54 4845 4d45 5f4f 5054 494f 4e53  ML_THEME_OPTIONS
 000001e0: da1f 5350 4849 4e58 5f54 4845 4d45 535f  ..SPHINX_THEMES_
 000001f0: 4558 5452 415f 5354 594c 4553 4845 4554  EXTRA_STYLESHEET
 00000200: 53da 1b53 5048 494e 585f 5448 454d 4553  S..SPHINX_THEMES
@@ -59,11 +59,11 @@
 000003a0: 5448 454d 4553 5f53 484f 575f 434f 5059  THEMES_SHOW_COPY
 000003b0: 5249 4748 545a 1953 5048 494e 585f 5448  RIGHTZ.SPHINX_TH
 000003c0: 454d 4553 5f53 484f 575f 5350 4849 4e58  EMES_SHOW_SPHINX
 000003d0: 5a19 5350 4849 4e58 5f54 4845 4d45 535f  Z.SPHINX_THEMES_
 000003e0: 4449 5350 4c41 595f 544f 4372 0a00 0000  DISPLAY_TOCr....
 000003f0: 7208 0000 0072 0800 0000 7208 0000 0072  r....r....r....r
 00000400: 0900 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000410: 0000 732c 0000 0004 0104 0104 0104 0104  ..s,............
-00000420: 0204 0204 0104 0104 0104 0104 0104 0104  ................
+00000410: 0000 732e 0000 0004 0004 0104 0104 0104  ..s.............
+00000420: 0104 0204 0204 0104 0104 0104 0104 0104  ................
 00000430: 0104 0104 0104 0104 0104 0104 0104 0104  ................
-00000440: 0104 03                                  ...
+00000440: 0104 010c 03                             .....
```

### Comparing `flamingo-1.8/flamingo/plugins/sphinx_themes/__pycache__/plugin.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/sphinx_themes/__pycache__/plugin.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu May 12 16:46:56 2022 UTC, .py size: 13861 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 003a 7d62 2536 0000  o........:}b%6..
+00000000: 6f0d 0d0a 0000 0000 2e1e 6863 2536 0000  o.........hc%6..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 e200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 5a04 6400  m.Z...d.d.l.Z.d.
 00000050: 6403 6c05 5a05 6400 6403 6c06 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6404 6c07 6d08 5a08 0100 6400 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6400 6406 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
@@ -283,15 +283,15 @@
 000011a0: 026a 036a 0464 043c 0074 057c 026a 036a  .j.j.d.<.t.|.j.j
 000011b0: 0464 053c 0074 067c 026a 036a 0464 063c  .d.<.t.|.j.j.d.<
 000011c0: 0074 0774 0883 017c 026a 036a 0964 073c  .t.t...|.j.j.d.<
 000011d0: 0064 0053 0029 084e 6301 0000 0000 0000  .d.S.).Nc.......
 000011e0: 0000 0000 0003 0000 0004 0000 0053 0000  .............S..
 000011f0: 0073 4000 0000 7c00 7304 6401 5300 7400  .s@...|.s.d.S.t.
 00001200: 7401 7c00 8301 6402 8302 7d01 0900 7c01  t.|...d...}...|.
-00001210: a002 6404 a101 7d02 7c02 7314 7119 7c02  ..d...}.|.s.q.|.
+00001210: a002 6404 a101 7d02 7c02 7314 6e05 7c02  ..d...}.|.s.n.|.
 00001220: a003 a100 0100 710c 7404 a005 7401 7c01  ......q.t...t.|.
 00001230: 8301 a101 5300 2905 4e7a 0222 227a 0b68  ....S.).Nz.""z.h
 00001240: 746d 6c2e 7061 7273 6572 54da 0673 6372  tml.parserT..scr
 00001250: 6970 7429 0672 0500 0000 da03 7374 72da  ipt).r......str.
 00001260: 0466 696e 64da 0964 6563 6f6d 706f 7365  .find..decompose
 00001270: da04 6a73 6f6e da05 6475 6d70 7329 03da  ..json..dumps)..
 00001280: 0468 746d 6cda 0473 6f75 7072 6900 0000  .html..soupri...
@@ -592,15 +592,15 @@
 000024f0: 7f08 1808 0908 0308 0408 030c 1172 2e00  .............r..
 00002500: 0000 2921 da08 7465 6d70 6669 6c65 7202  ..)!..tempfiler.
 00002510: 0000 00da 0463 6f70 7972 0300 0000 da07  .....copyr......
 00002520: 6c6f 6767 696e 6772 6d00 0000 7252 0000  loggingrm...rR..
 00002530: 005a 066a 696e 6a61 3272 0400 0000 da03  .Z.jinja2r......
 00002540: 6273 3472 0500 0000 5a11 7370 6869 6e78  bs4r....Z.sphinx
 00002550: 2e6a 696e 6a61 3267 6c75 6572 0600 0000  .jinja2gluer....
-00002560: 7207 0000 0072 0800 0000 7209 0000 005a  r....r....r....Z
+00002560: 7207 0000 0072 0800 0000 7209 0000 00da  r....r....r.....
 00002570: 0673 7068 696e 7872 0a00 0000 7293 0000  .sphinxr....r...
 00002580: 005a 1a66 6c61 6d69 6e67 6f2e 706c 7567  .Z.flamingo.plug
 00002590: 696e 732e 6d65 6e75 2e6d 656e 7572 0b00  ins.menu.menur..
 000025a0: 0000 da08 666c 616d 696e 676f 720c 0000  ....flamingor...
 000025b0: 0072 4600 0000 720e 0000 0072 1c00 0000  .rF...r....r....
 000025c0: 720f 0000 00da 0967 6574 4c6f 6767 6572  r......getLogger
 000025d0: 725d 0000 0072 1000 0000 721b 0000 0072  r]...r....r....r
```

### Comparing `flamingo-1.8/flamingo/plugins/sphinx_themes/__pycache__/plugin.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/sphinx_themes/__pycache__/plugin.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May 12 17:00:04 2022 UTC, .py size: 13861 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 143d 7d62 2536 0000  a........=}b%6..
+00000000: 610d 0d0a 0000 0000 7b3c 6963 2536 0000  a.......{<ic%6..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 e200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 5a04 6400  m.Z...d.d.l.Z.d.
 00000050: 6403 6c05 5a05 6400 6403 6c06 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6404 6c07 6d08 5a08 0100 6400 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6400 6406 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
@@ -175,15 +175,15 @@
 00000ae0: 7c01 8801 6a00 7c01 1900 6602 9102 7104  |...j.|...f...q.
 00000af0: 5300 7214 0000 0029 0172 2400 0000 723e  S.r....).r$...r>
 00000b00: 0000 00a9 02da 0669 676e 6f72 6572 1300  .......ignorer..
 00000b10: 0000 7214 0000 0072 1500 0000 7242 0000  ..r....r....rB..
 00000b20: 0060 0000 0073 0400 0000 0601 0aff 7a0c  .`...s........z.
 00000b30: 4854 4d4c 204f 7074 696f 6e73 290a da06  HTML Options)...
 00000b40: 736f 7274 6564 da0c 7370 6869 6e78 5f74  sorted..sphinx_t
-00000b50: 6865 6d65 5a03 6170 70da 0872 6567 6973  hemeZ.app..regis
+00000b50: 6865 6d65 da03 6170 70da 0872 6567 6973  heme..app..regis
 00000b60: 7472 795a 0b68 746d 6c5f 7468 656d 6573  tryZ.html_themes
 00000b70: da04 6b65 7973 7224 0000 00da 125f 7261  ..keysr$....._ra
 00000b80: 775f 7468 656d 655f 6f70 7469 6f6e 7372  w_theme_optionsr
 00000b90: 3600 0000 da06 6170 7065 6e64 2904 7213  6.....append).r.
 00000ba0: 0000 00da 076f 7074 696f 6e73 5a0d 7468  .....optionsZ.th
 00000bb0: 656d 655f 6f70 7469 6f6e 73da 036b 6579  eme_options..key
 00000bc0: 7214 0000 0072 4300 0000 7215 0000 00da  r....rC...r.....
@@ -214,24 +214,24 @@
 00000d50: 028d 0201 007c 006a 046a 067c 006a 0364  .....|.j.j.|.j.d
 00000d60: 0164 028d 0201 0074 077c 006a 087c 006a  .d.....t.|.j.|.j
 00000d70: 037c 006a 0964 038d 037c 005f 0a7c 006a  .|.j.d...|._.|.j
 00000d80: 0a6a 0ba0 0ca1 007c 005f 0d7c 006a 0a6a  .j.....|._.|.j.j
 00000d90: 0ba0 0ea1 007c 005f 0f7c 006a 0a6a 0ba0  .....|._.|.j.j..
 00000da0: 10a1 007c 005f 1164 0053 0029 044e 5429  ...|._.d.S.).NT)
 00000db0: 01da 0566 6f72 6365 2903 7238 0000 00da  ...force).r8....
-00000dc0: 0962 7569 6c64 5f64 6972 724b 0000 0029  .build_dirrK...)
+00000dc0: 0962 7569 6c64 5f64 6972 724c 0000 0029  .build_dirrL...)
 00000dd0: 12da 026f 73da 0470 6174 68da 0665 7869  ...os..path..exi
-00000de0: 7374 7372 5100 0000 7222 0000 00da 0572  stsrQ...r".....r
+00000de0: 7374 7372 5200 0000 7222 0000 00da 0572  stsrR...r".....r
 00000df0: 6d5f 7266 da07 6d6b 6469 725f 7072 0e00  m_rf..mkdir_pr..
 00000e00: 0000 7235 0000 0072 3600 0000 7246 0000  ..r5...r6...rF..
 00000e10: 00da 0663 6f6e 6669 675a 1067 6574 5f74  ...configZ.get_t
 00000e20: 6865 6d65 5f63 6f6e 6669 67da 0d5f 7468  heme_config.._th
 00000e30: 656d 655f 636f 6e66 6967 5a15 6765 745f  eme_configZ.get_
 00000e40: 7261 775f 7468 656d 655f 6f70 7469 6f6e  raw_theme_option
-00000e50: 7372 4900 0000 5a11 6765 745f 7468 656d  srI...Z.get_them
+00000e50: 7372 4a00 0000 5a11 6765 745f 7468 656d  srJ...Z.get_them
 00000e60: 655f 6f70 7469 6f6e 73da 0e5f 7468 656d  e_options.._them
 00000e70: 655f 6f70 7469 6f6e 7372 4100 0000 7214  e_optionsrA...r.
 00000e80: 0000 0072 1400 0000 7215 0000 0072 3700  ...r....r....r7.
 00000e90: 0000 8600 0000 7318 0000 0000 020e 0112  ......s.........
 00000ea0: 0212 0302 0104 0104 0104 fd08 070e 030a  ................
 00000eb0: ff04 037a 1253 7068 696e 7854 6865 6d65  ...z.SphinxTheme
 00000ec0: 732e 6275 696c 6463 0200 0000 0000 0000  s.buildc........
@@ -256,20 +256,20 @@
 00000ff0: 6e61 626c 696e 6720 4d45 4e55 5f43 5245  nabling MENU_CRE
 00001000: 4154 455f 494e 4449 4345 5354 7a13 7370  ATE_INDICESTz.sp
 00001010: 6869 6e78 2d74 6865 6d65 732f 7468 656d  hinx-themes/them
 00001020: 657a 0f6a 696e 6a61 322e 6578 742e 6931  ez.jinja2.ext.i1
 00001030: 386e da05 7468 656d 6529 1672 2200 0000  8n..theme).r"...
 00001040: 7224 0000 00da 0750 4c55 4749 4e53 da06  r$.....PLUGINS..
 00001050: 6c6f 6767 6572 da04 7761 726e da03 6765  logger..warn..ge
-00001060: 74da 0564 6562 7567 725a 0000 0072 0200  t..debugrZ...r..
-00001070: 0000 da08 7465 6d70 5f64 6972 7252 0000  ....temp_dirrR..
-00001080: 0072 5300 0000 da04 6a6f 696e 7238 0000  .rS.....joinr8..
-00001090: 0072 5100 0000 da19 4c49 5645 5f53 4552  .rQ.....LIVE_SER
+00001060: 74da 0564 6562 7567 725b 0000 0072 0200  t..debugr[...r..
+00001070: 0000 da08 7465 6d70 5f64 6972 7253 0000  ....temp_dirrS..
+00001080: 0072 5400 0000 da04 6a6f 696e 7238 0000  .rT.....joinr8..
+00001090: 0072 5200 0000 da19 4c49 5645 5f53 4552  .rR.....LIVE_SER
 000010a0: 5645 525f 4947 4e4f 5245 5f50 5245 4649  VER_IGNORE_PREFI
-000010b0: 5872 4a00 0000 da11 4a49 4e4a 4132 5f45  XrJ.....JINJA2_E
+000010b0: 5872 4b00 0000 da11 4a49 4e4a 4132 5f45  XrK.....JINJA2_E
 000010c0: 5854 454e 5349 4f4e 5372 3a00 0000 da07  XTENSIONSr:.....
 000010d0: 6469 726e 616d 65da 085f 5f66 696c 655f  dirname..__file_
 000010e0: 5fda 0b54 4845 4d45 5f50 4154 4853 2902  _..THEME_PATHS).
 000010f0: 7213 0000 0072 2200 0000 7214 0000 0072  r....r"...r....r
 00001100: 1400 0000 7215 0000 00da 0e73 6574 7469  ....r......setti
 00001110: 6e67 735f 7365 7475 709d 0000 0073 2200  ngs_setup....s".
 00001120: 0000 0001 0603 0c01 0c02 0e01 0a02 0803  ................
@@ -289,30 +289,30 @@
 00001200: 7d01 7c01 a002 6403 a101 7d02 7c02 7326  }.|...d...}.|.s&
 00001210: 7130 7c02 a003 a100 0100 7116 7404 a005  q0|.......q.t...
 00001220: 7401 7c01 8301 a101 5300 2904 4e7a 0222  t.|.....S.).Nz."
 00001230: 227a 0b68 746d 6c2e 7061 7273 6572 da06  "z.html.parser..
 00001240: 7363 7269 7074 2906 7205 0000 00da 0373  script).r......s
 00001250: 7472 da04 6669 6e64 da09 6465 636f 6d70  tr..find..decomp
 00001260: 6f73 65da 046a 736f 6eda 0564 756d 7073  ose..json..dumps
-00001270: 2903 da04 6874 6d6c da04 736f 7570 7269  )...html..soupri
+00001270: 2903 da04 6874 6d6c da04 736f 7570 726a  )...html..souprj
 00001280: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
 00001290: 0000 da0a 5f73 6166 655f 6475 6d70 be00  ...._safe_dump..
 000012a0: 0000 7310 0000 0000 0104 0104 020e 030a  ..s.............
 000012b0: 0204 0102 020a 027a 3853 7068 696e 7854  .......z8SphinxT
 000012c0: 6865 6d65 732e 7465 6d70 6c61 7469 6e67  hemes.templating
 000012d0: 5f65 6e67 696e 655f 7365 7475 702e 3c6c  _engine_setup.<l
 000012e0: 6f63 616c 733e 2e5f 7361 6665 5f64 756d  ocals>._safe_dum
 000012f0: 70da 0973 6166 655f 6475 6d70 5a06 746f  p..safe_dumpZ.to
 00001300: 626f 6f6c 5a05 746f 696e 745a 0574 6f64  boolZ.tointZ.tod
 00001310: 696d 7209 0000 0029 0a72 2400 0000 da0d  imr....).r$.....
 00001320: 4558 5452 415f 434f 4e54 4558 5472 0600  EXTRA_CONTEXTr..
 00001330: 0000 da03 656e 76da 0766 696c 7465 7273  ....env..filters
 00001340: 7208 0000 0072 0700 0000 7204 0000 0072  r....r....r....r
 00001350: 0900 0000 da07 676c 6f62 616c 7329 0472  ......globals).r
-00001360: 1300 0000 7222 0000 0072 2900 0000 7271  ....r"...r)...rq
+00001360: 1300 0000 7222 0000 0072 2900 0000 7272  ....r"...r)...rr
 00001370: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
 00001380: 0000 da17 7465 6d70 6c61 7469 6e67 5f65  ....templating_e
 00001390: 6e67 696e 655f 7365 7475 70bd 0000 0073  ngine_setup....s
 000013a0: 0c00 0000 0001 0810 0c02 0c01 0c01 0c02  ................
 000013b0: 7a24 5370 6869 6e78 5468 656d 6573 2e74  z$SphinxThemes.t
 000013c0: 656d 706c 6174 696e 675f 656e 6769 6e65  emplating_engine
 000013d0: 5f73 6574 7570 6305 0000 0000 0000 0000  _setupc.........
@@ -368,28 +368,28 @@
 000016f0: 5f74 6974 6c65 721d 0000 0063 0100 0000  _titler....c....
 00001700: 0000 0000 0000 0000 0300 0000 0500 0000  ................
 00001710: 5300 0000 7326 0000 0069 007c 005d 1e5c  S...s&...i.|.].\
 00001720: 027d 017d 027c 0174 0064 0083 0164 0185  .}.}.|.t.d...d..
 00001730: 0219 00a0 01a1 007c 0293 0271 0453 0029  .......|...q.S.)
 00001740: 025a 0e53 5048 494e 585f 5448 454d 4553  .Z.SPHINX_THEMES
 00001750: 5f4e 2902 da03 6c65 6eda 056c 6f77 6572  _N)...len..lower
-00001760: 2903 723f 0000 0072 4c00 0000 724e 0000  ).r?...rL...rN..
+00001760: 2903 723f 0000 0072 4d00 0000 724f 0000  ).r?...rM...rO..
 00001770: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
 00001780: da0a 3c64 6963 7463 6f6d 703e ee00 0000  ..<dictcomp>....
 00001790: 7304 0000 0006 0206 ff7a 3753 7068 696e  s........z7Sphin
 000017a0: 7854 6865 6d65 732e 7465 6d70 6c61 7465  xThemes.template
 000017b0: 5f63 6f6e 7465 7874 5f73 6574 7570 2e3c  _context_setup.<
 000017c0: 6c6f 6361 6c73 3e2e 3c64 6963 7463 6f6d  locals>.<dictcom
 000017d0: 703e 7a17 7370 6869 6e78 5f74 6865 6d65  p>z.sphinx_theme
 000017e0: 732f 626f 6479 2e68 746d 6c29 0272 2200  s/body.html).r".
 000017f0: 0000 7223 0000 0046 7225 0000 0072 1c00  ..r#...Fr%...r..
 00001800: 0000 7201 0000 00da 012e 720d 0000 00e9  ..r.......r.....
 00001810: 0200 0000 da19 5350 4849 4e58 5f54 4845  ......SPHINX_THE
 00001820: 4d45 535f 5348 4f57 5f53 4f55 5243 4572  MES_SHOW_SOURCEr
-00001830: 5300 0000 291a 5a08 656d 6265 6464 6564  S...).Z.embedded
+00001830: 5400 0000 291a 5a08 656d 6265 6464 6564  T...).Z.embedded
 00001840: 5a0e 7573 655f 6f70 656e 7365 6172 6368  Z.use_opensearch
 00001850: 5a0b 6669 6c65 5f73 7566 6669 785a 0b6c  Z.file_suffixZ.l
 00001860: 696e 6b5f 7375 6666 6978 da05 7374 796c  ink_suffix..styl
 00001870: 655a 0872 656c 6c69 6e6b 73da 0762 7569  eZ.rellinks..bui
 00001880: 6c64 6572 5a0d 6874 6d6c 355f 646f 6374  lderZ.html5_doct
 00001890: 7970 655a 0e73 7068 696e 785f 7665 7273  ypeZ.sphinx_vers
 000018a0: 696f 6eda 0a68 6173 5f73 6f75 7263 655a  ion..has_sourceZ
@@ -398,48 +398,48 @@
 000018d0: 0a73 6f75 7263 656e 616d 65da 0963 7373  .sourcename..css
 000018e0: 5f66 696c 6573 da0c 7363 7269 7074 5f66  _files..script_f
 000018f0: 696c 6573 da06 6861 7364 6f63 da07 6765  iles..hasdoc..ge
 00001900: 7474 6578 74da 0670 6174 6874 6fda 0763  ttext..pathto..c
 00001910: 7373 5f74 6167 da06 6a73 5f74 6167 da07  ss_tag..js_tag..
 00001920: 746f 6374 7265 65da 0770 6172 656e 7473  toctree..parents
 00001930: da03 746f 63da 0870 6167 656e 616d 6572  ..toc..pagenamer
-00001940: 1e00 0000 da04 626f 6479 7284 0000 007a  ......bodyr....z
+00001940: 1e00 0000 da04 626f 6479 7285 0000 007a  ......bodyr....z
 00001950: 072f 7374 6174 6963 da0a 7374 796c 6573  ./static..styles
 00001960: 6865 6574 5a17 7370 6869 6e78 5f74 6865  heetZ.sphinx_the
 00001970: 6d65 735f 6373 735f 6669 6c65 7372 3c00  mes_css_filesr<.
-00001980: 0000 7285 0000 007a 1f2f 7374 6174 6963  ..r....z./static
+00001980: 0000 7286 0000 007a 1f2f 7374 6174 6963  ..r....z./static
 00001990: 2f73 7068 696e 785f 7468 656d 6573 2f6a  /sphinx_themes/j
 000019a0: 7175 6572 792e 6a73 7a21 2f73 7461 7469  query.jsz!/stati
 000019b0: 632f 7370 6869 6e78 5f74 6865 6d65 732f  c/sphinx_themes/
 000019c0: 6d61 726b 2e6d 696e 2e6a 737a 1f2f 7374  mark.min.jsz./st
 000019d0: 6174 6963 2f73 7068 696e 785f 7468 656d  atic/sphinx_them
 000019e0: 6573 2f68 656c 7065 722e 6a73 7a14 2f73  es/helper.jsz./s
 000019f0: 6561 7263 685f 7661 7269 6162 6c65 732e  earch_variables.
 00001a00: 6a73 da1a 7370 6869 6e78 5f74 6865 6d65  js..sphinx_theme
 00001a10: 735f 7363 7269 7074 5f66 696c 6573 7a1d  s_script_filesz.
 00001a20: 2f73 7461 7469 632f 7370 6869 6e78 5f74  /static/sphinx_t
 00001a30: 6865 6d65 732f 6d61 696e 2e6a 7372 3b00  hemes/main.jsr;.
-00001a40: 0000 291e 7220 0000 0072 2400 0000 725f  ..).r ...r$...r_
+00001a40: 0000 291e 7220 0000 0072 2400 0000 7260  ..).r ...r$...r`
 00001a50: 0000 00da 0a69 7369 6e73 7461 6e63 6572  .....isinstancer
 00001a60: 0b00 0000 7238 0000 0072 2300 0000 720c  ....r8...r#...r.
-00001a70: 0000 0072 4a00 0000 721b 0000 00da 0569  ...rJ...r......i
+00001a70: 0000 0072 4b00 0000 721b 0000 00da 0569  ...rK...r......i
 00001a80: 7465 6d73 da08 6361 6c6c 6162 6c65 7229  tems..callabler)
 00001a90: 0000 0072 2a00 0000 da13 7370 6869 6e78  ...r*.....sphinx
-00001aa0: 5f76 6572 7369 6f6e 5f69 6e66 6f72 8600  _version_infor..
-00001ab0: 0000 7287 0000 0072 8800 0000 7289 0000  ..r....r....r...
-00001ac0: 0072 8a00 0000 7258 0000 0072 5900 0000  .r....rX...rY...
-00001ad0: 7210 0000 0072 5200 0000 7253 0000 0072  r....rR...rS...r
-00001ae0: 6200 0000 da04 6c69 7374 720f 0000 0072  b.....listr....r
+00001aa0: 5f76 6572 7369 6f6e 5f69 6e66 6f72 8700  _version_infor..
+00001ab0: 0000 7288 0000 0072 8900 0000 728a 0000  ..r....r....r...
+00001ac0: 0072 8b00 0000 7259 0000 0072 5a00 0000  .r....rY...rZ...
+00001ad0: 7210 0000 0072 5300 0000 7254 0000 0072  r....rS...rT...r
+00001ae0: 6300 0000 da04 6c69 7374 720f 0000 0072  c.....listr....r
 00001af0: 3c00 0000 723b 0000 0029 1272 1300 0000  <...r;...).r....
 00001b00: 7222 0000 0072 2300 0000 7226 0000 0072  r"...r#...r&...r
-00001b10: 2700 0000 728b 0000 0072 8c00 0000 da04  '...r....r......
+00001b10: 2700 0000 728c 0000 0072 8d00 0000 da04  '...r....r......
 00001b20: 6974 656d 721e 0000 0072 1f00 0000 7224  itemr....r....r$
-00001b30: 0000 0072 4c00 0000 724e 0000 0072 8f00  ...rL...rN...r..
+00001b30: 0000 0072 4d00 0000 724f 0000 0072 9000  ...rM...rO...r..
 00001b40: 0000 5a17 7370 6869 6e78 5f74 656d 706c  ..Z.sphinx_templ
-00001b50: 6174 655f 636f 6e74 6578 7472 5300 0000  ate_contextrS...
+00001b50: 6174 655f 636f 6e74 6578 7472 5400 0000  ate_contextrT...
 00001b60: 5a11 6578 7472 615f 7374 796c 6573 6865  Z.extra_styleshe
 00001b70: 6574 735a 0d65 7874 7261 5f73 6372 6970  etsZ.extra_scrip
 00001b80: 7473 7214 0000 0072 1400 0000 7215 0000  tsr....r....r...
 00001b90: 00da 1674 656d 706c 6174 655f 636f 6e74  ...template_cont
 00001ba0: 6578 745f 7365 7475 70d6 0000 0073 d800  ext_setup....s..
 00001bb0: 0000 0004 0201 0201 0201 04fd 0607 0402  ................
 00001bc0: 1001 0a01 0601 0c02 0a01 1002 1403 0602  ................
@@ -460,62 +460,62 @@
 00001cb0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
 00001cc0: 0200 0000 4300 0000 731c 0000 007c 0164  ....C...s....|.d
 00001cd0: 016b 0272 0c64 0253 007c 0164 0376 0072  .k.r.d.S.|.d.v.r
 00001ce0: 1864 0453 0064 0253 0029 054e da06 7365  .d.S.d.S.).N..se
 00001cf0: 6172 6368 5429 03da 0561 626f 7574 5a08  archT)...aboutZ.
 00001d00: 6765 6e69 6e64 6578 da09 636f 7079 7269  genindex..copyri
 00001d10: 6768 7446 7214 0000 0029 0272 1300 0000  ghtFr....).r....
-00001d20: 728e 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
-00001d30: 1500 0000 7286 0000 006d 0100 0073 0a00  ....r....m...s..
+00001d20: 728f 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
+00001d30: 1500 0000 7287 0000 006d 0100 0073 0a00  ....r....m...s..
 00001d40: 0000 0001 0801 0402 0801 0402 7a13 5370  ............z.Sp
 00001d50: 6869 6e78 5468 656d 6573 2e68 6173 646f  hinxThemes.hasdo
 00001d60: 6363 0200 0000 0000 0000 0000 0000 0300  cc..............
 00001d70: 0000 0100 0000 4b00 0000 7304 0000 007c  ......K...s....|
 00001d80: 0153 0072 1100 0000 7214 0000 0029 0372  .S.r....r....).r
 00001d90: 1300 0000 da06 7374 7269 6e67 722c 0000  ......stringr,..
 00001da0: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
-00001db0: 7287 0000 0076 0100 0073 0200 0000 0001  r....v...s......
+00001db0: 7288 0000 0076 0100 0073 0200 0000 0001  r....v...s......
 00001dc0: 7a14 5370 6869 6e78 5468 656d 6573 2e67  z.SphinxThemes.g
 00001dd0: 6574 7465 7874 6302 0000 0000 0000 0000  ettextc.........
 00001de0: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
 00001df0: 0c00 0000 6401 a000 7c01 6a01 a101 5300  ....d...|.j...S.
 00001e00: 2902 4e7a 333c 6c69 6e6b 2072 656c 3d22  ).Nz3<link rel="
 00001e10: 7374 796c 6573 6865 6574 2220 6872 6566  stylesheet" href
 00001e20: 3d22 7b7d 2220 7479 7065 3d22 7465 7874  ="{}" type="text
 00001e30: 2f63 7373 2220 2f3e a902 da06 666f 726d  /css" />....form
 00001e40: 6174 7212 0000 00a9 0272 1300 0000 5a0b  atr......r....Z.
 00001e50: 7374 6174 6963 5f66 696c 6572 1400 0000  static_filer....
-00001e60: 7214 0000 0072 1500 0000 7289 0000 0079  r....r....r....y
+00001e60: 7214 0000 0072 1500 0000 728a 0000 0079  r....r....r....y
 00001e70: 0100 0073 0600 0000 0001 0401 04ff 7a14  ...s..........z.
 00001e80: 5370 6869 6e78 5468 656d 6573 2e63 7373  SphinxThemes.css
 00001e90: 5f74 6167 6302 0000 0000 0000 0000 0000  _tagc...........
 00001ea0: 0002 0000 0003 0000 0043 0000 0073 0c00  .........C...s..
 00001eb0: 0000 6401 a000 7c01 6a01 a101 5300 2902  ..d...|.j...S.).
 00001ec0: 4e7a 1a3c 7363 7269 7074 2073 7263 3d22  Nz.<script src="
-00001ed0: 7b7d 223e 3c2f 7363 7269 7074 3e72 9d00  {}"></script>r..
-00001ee0: 0000 729f 0000 0072 1400 0000 7214 0000  ..r....r....r...
-00001ef0: 0072 1500 0000 728a 0000 007d 0100 0073  .r....r....}...s
+00001ed0: 7b7d 223e 3c2f 7363 7269 7074 3e72 9e00  {}"></script>r..
+00001ee0: 0000 72a0 0000 0072 1400 0000 7214 0000  ..r....r....r...
+00001ef0: 0072 1500 0000 728b 0000 007d 0100 0073  .r....r....}...s
 00001f00: 0200 0000 0001 7a13 5370 6869 6e78 5468  ......z.SphinxTh
 00001f10: 656d 6573 2e6a 735f 7461 6763 0200 0000  emes.js_tagc....
 00001f20: 0000 0000 0000 0000 0400 0000 0400 0000  ................
 00001f30: 4f00 0000 735c 0000 007c 0164 016b 0272  O...s\...|.d.k.r
 00001f40: 127c 006a 0064 0219 0053 0074 017c 0174  .|.j.d...S.t.|.t
 00001f50: 0283 0272 227c 016a 0353 0074 017c 0174  ...r"|.j.S.t.|.t
 00001f60: 0483 0272 587c 01a0 0564 03a1 0172 4664  ...rX|...d...rFd
 00001f70: 047c 0164 0564 0085 0219 0017 0053 007c  .|.d.d.......S.|
 00001f80: 01a0 0564 06a1 0172 5864 047c 0117 0053  ...d...rXd.|...S
-00001f90: 0064 0453 0029 074e 7299 0000 00da 1853  .d.S.).Nr......S
+00001f90: 0064 0453 0029 074e 729a 0000 00da 1853  .d.S.).Nr......S
 00001fa0: 5048 494e 585f 5448 454d 4553 5f53 4541  PHINX_THEMES_SEA
 00001fb0: 5243 485f 5552 4c5a 075f 7374 6174 6963  RCH_URLZ._static
 00001fc0: fa01 2f72 0d00 0000 5a08 5f73 6f75 7263  ../r....Z._sourc
-00001fd0: 6573 2906 7224 0000 0072 9200 0000 7210  es).r$...r....r.
-00001fe0: 0000 0072 1200 0000 726a 0000 0072 3300  ...r....rj...r3.
+00001fd0: 6573 2906 7224 0000 0072 9300 0000 7210  es).r$...r....r.
+00001fe0: 0000 0072 1200 0000 726b 0000 0072 3300  ...r....rk...r3.
 00001ff0: 0000 2904 7213 0000 005a 086f 7468 6572  ..).r....Z.other
 00002000: 7572 6972 2b00 0000 722c 0000 0072 1400  urir+...r,...r..
-00002010: 0000 7214 0000 0072 1500 0000 7288 0000  ..r....r....r...
+00002010: 0000 7214 0000 0072 1500 0000 7289 0000  ..r....r....r...
 00002020: 0080 0100 0073 1400 0000 0001 0801 0a02  .....s..........
 00002030: 0a01 0602 0a01 0a01 1002 0a01 0802 7a13  ..............z.
 00002040: 5370 6869 6e78 5468 656d 6573 2e70 6174  SphinxThemes.pat
 00002050: 6874 6f63 0200 0000 0000 0000 0000 0000  htoc............
 00002060: 0500 0000 0700 0000 4300 0000 73d2 0000  ........C...s...
 00002070: 007c 016a 006a 017c 016a 026a 037c 006a  .|.j.j.|.j.j.|.j
 00002080: 0264 0119 0064 0264 0085 0219 0064 0364  .d...d.d.....d.d
@@ -526,80 +526,80 @@
 000020d0: 007c 006a 0264 1019 0072 ce7c 016a 0044  .|.j.d...r.|.j.D
 000020e0: 005d 5c7d 037c 03a0 0564 1164 04a1 02a0  .]\}.|...d.d....
 000020f0: 0664 12a1 0173 8871 7064 137c 0364 143c  .d...s.qpd.|.d.<
 00002100: 0074 076a 08a0 097c 016a 026a 0a7c 0364  .t.j...|.j.j.|.d
 00002110: 1119 00a1 027d 047c 016a 006a 0164 1564  .....}.|.j.j.d.d
 00002120: 16a0 0b7c 0364 1119 00a1 0174 0c7c 0464  ...|.d.....t.|.d
 00002130: 1783 02a0 0da1 0064 188d 0301 0071 7064  .......d.....qpd
-00002140: 0053 0029 194e 72a0 0000 0072 0d00 0000  .S.).Nr....r....
+00002140: 0053 0029 194e 72a1 0000 0072 0d00 0000  .S.).Nr....r....
 00002150: 5a06 5365 6172 6368 721c 0000 0029 037a  Z.Searchr....).z
 00002160: 242f 7374 6174 6963 2f73 7068 696e 785f  $/static/sphinx_
 00002170: 7468 656d 6573 2f72 6163 7469 7665 2e6d  themes/ractive.m
 00002180: 696e 2e6a 737a 282f 7374 6174 6963 2f73  in.jsz(/static/s
 00002190: 7068 696e 785f 7468 656d 6573 2f65 6c61  phinx_themes/ela
 000021a0: 7374 6963 6c75 6e72 2e6d 696e 2e6a 737a  sticlunr.min.jsz
 000021b0: 0a2f 7365 6172 6368 2e6a 7329 05da 0874  ./search.js)...t
 000021c0: 656d 706c 6174 65da 066f 7574 7075 7472  emplate..outputr
-000021d0: 7a00 0000 da0c 636f 6e74 656e 745f 626f  z.....content_bo
-000021e0: 6479 7291 0000 007a 052e 626f 6479 da10  dyr....z..body..
+000021d0: 7b00 0000 da0c 636f 6e74 656e 745f 626f  {.....content_bo
+000021e0: 6479 7292 0000 007a 052e 626f 6479 5a10  dyr....z..bodyZ.
 000021f0: 7370 6869 6e78 5f72 7464 5f74 6865 6d65  sphinx_rtd_theme
 00002200: 7a0b 5b72 6f6c 653d 6d61 696e 5d7a 2173  z.[role=main]z!s
 00002210: 7068 696e 785f 7468 656d 6573 2f73 6561  phinx_themes/sea
 00002220: 7263 685f 7661 7269 6162 6c65 732e 6a73  rch_variables.js
 00002230: 7a13 7365 6172 6368 5f76 6172 6961 626c  z.search_variabl
-00002240: 6573 2e6a 7329 0372 a200 0000 72a3 0000  es.js).r....r...
+00002240: 6573 2e6a 7329 0372 a300 0000 72a4 0000  es.js).r....r...
 00002250: 00da 1e73 6561 7263 685f 7261 6374 6976  ...search_ractiv
 00002260: 655f 7461 7267 6574 5f73 656c 6563 746f  e_target_selecto
 00002270: 727a 1773 7068 696e 785f 7468 656d 6573  rz.sphinx_themes
 00002280: 2f73 6561 7263 682e 6a73 7a09 7365 6172  /search.jsz.sear
-00002290: 6368 2e6a 7329 0272 a200 0000 72a3 0000  ch.js).r....r...
-000022a0: 0072 8000 0000 7253 0000 007a 042e 7273  .r....rS...z..rs
-000022b0: 7454 7283 0000 007a 0c5f 736f 7572 6365  tTr....z._source
+00002290: 6368 2e6a 7329 0272 a300 0000 72a4 0000  ch.js).r....r...
+000022a0: 0072 8100 0000 7254 0000 007a 042e 7273  .r....rT...z..rs
+000022b0: 7454 7284 0000 007a 0c5f 736f 7572 6365  tTr....z._source
 000022c0: 2d66 696c 657a 0b5f 736f 7572 6365 732f  -filez._sources/
-000022d0: 7b7d da01 7229 03da 0474 7970 6572 a300  {}..r)...typer..
-000022e0: 0000 72a4 0000 0029 0eda 0863 6f6e 7465  ..r....)...conte
+000022d0: 7b7d da01 7229 03da 0474 7970 6572 a400  {}..r)...typer..
+000022e0: 0000 72a5 0000 0029 0eda 0863 6f6e 7465  ..r....)...conte
 000022f0: 6e74 73da 0361 6464 7224 0000 00da 1044  nts..addr$.....D
 00002300: 4546 4155 4c54 5f54 454d 504c 4154 4572  EFAULT_TEMPLATEr
-00002310: 3500 0000 725f 0000 00da 0865 6e64 7377  5...r_.....endsw
-00002320: 6974 6872 5200 0000 7253 0000 0072 6200  ithrR...rS...rb.
+00002310: 3500 0000 7260 0000 00da 0865 6e64 7377  5...r`.....endsw
+00002320: 6974 6872 5300 0000 7254 0000 0072 6300  ithrS...rT...rc.
 00002330: 0000 da0c 434f 4e54 454e 545f 524f 4f54  ....CONTENT_ROOT
-00002340: 729e 0000 00da 046f 7065 6eda 0472 6561  r......open..rea
+00002340: 729f 0000 00da 046f 7065 6eda 0472 6561  r......open..rea
 00002350: 6429 0572 1300 0000 7222 0000 0072 a600  d).r....r"...r..
 00002360: 0000 7223 0000 00da 0b73 6f75 7263 655f  ..r#.....source_
 00002370: 7061 7468 7214 0000 0072 1400 0000 7215  pathr....r....r.
 00002380: 0000 00da 0f63 6f6e 7465 6e74 735f 7061  .....contents_pa
 00002390: 7273 6564 9101 0000 7342 0000 0000 0206  rsed....sB......
 000023a0: 0106 0110 0102 0102 0106 fb06 0d04 020a  ................
 000023b0: 0104 0206 0102 0102 0102 fd06 0706 0102  ................
 000023c0: 0102 fe06 060a 010a 0112 0102 0208 0206  ................
 000023d0: 0106 0106 fe04 0506 0102 010c 010c fd7a  ...............z
 000023e0: 1c53 7068 696e 7854 6865 6d65 732e 636f  .SphinxThemes.co
 000023f0: 6e74 656e 7473 5f70 6172 7365 644e 2910  ntents_parsedN).
 00002400: 7218 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
-00002410: 3a00 0000 724d 0000 0072 4f00 0000 7237  :...rM...rO...r7
-00002420: 0000 0072 6800 0000 7277 0000 0072 9800  ...rh...rw...r..
-00002430: 0000 7286 0000 0072 8700 0000 7289 0000  ..r....r....r...
-00002440: 0072 8a00 0000 7288 0000 0072 b100 0000  .r....r....r....
+00002410: 3a00 0000 724e 0000 0072 5000 0000 7237  :...rN...rP...r7
+00002420: 0000 0072 6900 0000 7278 0000 0072 9900  ...ri...rx...r..
+00002430: 0000 7287 0000 0072 8800 0000 728a 0000  ..r....r....r...
+00002440: 0072 8b00 0000 7289 0000 0072 b100 0000  .r....r....r....
 00002450: 7214 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
 00002460: 1500 0000 722e 0000 0035 0000 0073 1c00  ....r....5...s..
 00002470: 0000 0802 081d 081d 0815 0817 0820 0819  ............. ..
 00002480: 087f 0018 0809 0803 0804 0803 0811 722e  ..............r.
 00002490: 0000 0029 21da 0874 656d 7066 696c 6572  ...)!..tempfiler
 000024a0: 0200 0000 da04 636f 7079 7203 0000 00da  ......copyr.....
-000024b0: 076c 6f67 6769 6e67 726d 0000 0072 5200  .loggingrm...rR.
-000024c0: 0000 5a06 6a69 6e6a 6132 7204 0000 00da  ..Z.jinja2r.....
+000024b0: 076c 6f67 6769 6e67 726e 0000 0072 5300  .loggingrn...rS.
+000024c0: 0000 da06 6a69 6e6a 6132 7204 0000 00da  ....jinja2r.....
 000024d0: 0362 7334 7205 0000 005a 1173 7068 696e  .bs4r....Z.sphin
 000024e0: 782e 6a69 6e6a 6132 676c 7565 7206 0000  x.jinja2gluer...
 000024f0: 0072 0700 0000 7208 0000 0072 0900 0000  .r....r....r....
-00002500: da06 7370 6869 6e78 720a 0000 0072 9500  ..sphinxr....r..
+00002500: da06 7370 6869 6e78 720a 0000 0072 9600  ..sphinxr....r..
 00002510: 0000 5a1a 666c 616d 696e 676f 2e70 6c75  ..Z.flamingo.plu
 00002520: 6769 6e73 2e6d 656e 752e 6d65 6e75 720b  gins.menu.menur.
 00002530: 0000 00da 0866 6c61 6d69 6e67 6f72 0c00  .....flamingor..
 00002540: 0000 7246 0000 0072 0e00 0000 721c 0000  ..rF...r....r...
 00002550: 0072 0f00 0000 da09 6765 744c 6f67 6765  .r......getLogge
-00002560: 7272 5d00 0000 7210 0000 0072 1b00 0000  rr]...r....r....
+00002560: 7272 5e00 0000 7210 0000 0072 1b00 0000  rr^...r....r....
 00002570: 7220 0000 0072 2e00 0000 7214 0000 0072  r ...r....r....r
 00002580: 1400 0000 7214 0000 0072 1500 0000 da08  ....r....r......
 00002590: 3c6d 6f64 756c 653e 0100 0000 7322 0000  <module>....s"..
 000025a0: 000c 010c 0108 0108 0108 020c 010c 0218  ................
 000025b0: 010c 020c 010c 020c 010c 020a 030e 050e  ................
 000025c0: 060e 14                                  ...
```

### Comparing `flamingo-1.8/flamingo/plugins/sphinx_themes/__pycache__/sphinx_theme.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/sphinx_themes/__pycache__/sphinx_theme.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu May 12 15:07:02 2022 UTC, .py size: 8762 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,456 +1,462 @@
-00000000: 6f0d 0d0a 0000 0000 9622 7d62 3a22 0000  o........"}b:"..
+00000000: 6f0d 0d0a 0000 0000 fb20 6863 b822 0000  o........ hc."..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 0001 0000 6400  .....@...s....d.
+00000020: 0005 0000 0040 0000 0073 0801 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 5a06 6400 6404 6c07  ..d.d.l.Z.d.d.l.
-00000060: 5a07 6400 6404 6c08 5a08 6400 6405 6c09  Z.d.d.l.Z.d.d.l.
-00000070: 6d0a 5a0a 6d0b 5a0b 0100 6400 6406 6c0c  m.Z.m.Z...d.d.l.
-00000080: 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 0100 6400  m.Z.m.Z.m.Z...d.
-00000090: 6407 6c10 6d11 5a11 6d12 5a12 0100 6400  d.l.m.Z.m.Z...d.
-000000a0: 6408 6c13 6d14 5a14 0100 6400 6409 6c15  d.l.m.Z...d.d.l.
-000000b0: 6d16 5a16 0100 6400 6404 6c17 5a17 6508  m.Z...d.d.l.Z.e.
-000000c0: 6a18 a019 6508 6a18 a01a 6517 6a1b a101  j...e.j...e.j...
-000000d0: 640a a102 5a1c 6506 a01d 640b a101 5a1e  d...Z.e...d...Z.
-000000e0: 4700 640c 640d 8400 640d 651f 8303 5a20  G.d.d...d.e...Z 
-000000f0: 4700 640e 640f 8400 640f 651f 8303 5a21  G.d.d...d.e...Z!
-00000100: 4700 6410 6411 8400 6411 8302 5a22 4700  G.d.d...d...Z"G.
-00000110: 6412 6413 8400 6413 8302 5a23 4700 6414  d.d...d...Z#G.d.
-00000120: 6415 8400 6415 8302 5a24 6404 5300 2916  d...d...Z$d.S.).
-00000130: e900 0000 0029 01da 1169 7465 725f 656e  .....)...iter_en
-00000140: 7472 795f 706f 696e 7473 2901 da0f 5261  try_points)...Ra
-00000150: 7743 6f6e 6669 6750 6172 7365 7229 01da  wConfigParser)..
-00000160: 0864 6565 7063 6f70 794e 2902 da0b 456e  .deepcopyN)...En
-00000170: 7669 726f 6e6d 656e 74da 1046 696c 6553  vironment..FileS
-00000180: 7973 7465 6d4c 6f61 6465 7229 03da 075f  ystemLoader)..._
-00000190: 746f 626f 6f6c da06 5f74 6f64 696d da06  tobool.._todim..
-000001a0: 5f74 6f69 6e74 2902 da10 4854 4d4c 5468  _toint)...HTMLTh
-000001b0: 656d 6546 6163 746f 7279 da05 5468 656d  emeFactory..Them
-000001c0: 6529 01da 1753 7068 696e 7843 6f6d 706f  e)...SphinxCompo
-000001d0: 6e65 6e74 5265 6769 7374 7279 2901 da06  nentRegistry)...
-000001e0: 436f 6e66 6967 da06 7468 656d 6573 7a1d  Config..themesz.
-000001f0: 666c 616d 696e 676f 2e70 6c75 6769 6e73  flamingo.plugins
-00000200: 2e53 7068 696e 7854 6865 6d65 7363 0000  .SphinxThemesc..
-00000210: 0000 0000 0000 0000 0000 0000 0000 0100  ................
-00000220: 0000 4000 0000 f30c 0000 0065 005a 0164  ..@........e.Z.d
-00000230: 005a 0264 0153 0029 02da 1853 7068 696e  .Z.d.S.)...Sphin
-00000240: 7854 6865 6d65 4e6f 7446 6f75 6e64 4572  xThemeNotFoundEr
-00000250: 726f 724e a903 da08 5f5f 6e61 6d65 5f5f  rorN....__name__
-00000260: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000270: 7175 616c 6e61 6d65 5f5f a900 7215 0000  qualname__..r...
-00000280: 0072 1500 0000 fa58 2f68 6f6d 652f 6368  .r.....X/home/ch
-00000290: 7269 732f 776f 726b 2f50 726f 6a65 6374  ris/work/Project
-000002a0: 732f 6769 7468 7562 2f66 6c61 6d69 6e67  s/github/flaming
-000002b0: 6f2f 666c 616d 696e 676f 2f70 6c75 6769  o/flamingo/plugi
-000002c0: 6e73 2f73 7068 696e 785f 7468 656d 6573  ns/sphinx_themes
-000002d0: 2f73 7068 696e 785f 7468 656d 652e 7079  /sphinx_theme.py
-000002e0: 7210 0000 0015 0000 00f3 0400 0000 0800  r...............
-000002f0: 0401 7210 0000 0063 0000 0000 0000 0000  ..r....c........
-00000300: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
-00000310: 720f 0000 0029 02da 1a53 7068 696e 7843  r....)...SphinxC
-00000320: 6f6e 6669 6752 6563 7572 7369 6f6e 4572  onfigRecursionEr
-00000330: 726f 724e 7211 0000 0072 1500 0000 7215  rorNr....r....r.
-00000340: 0000 0072 1500 0000 7216 0000 0072 1800  ...r....r....r..
-00000350: 0000 1900 0000 7217 0000 0072 1800 0000  ......r....r....
-00000360: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000370: 0002 0000 0040 0000 0073 1c00 0000 6500  .....@...s....e.
-00000380: 5a01 6400 5a02 6401 6402 8400 5a03 6403  Z.d.Z.d.d...Z.d.
-00000390: 6404 8400 5a04 6405 5300 2906 da09 5370  d...Z.d.S.)...Sp
-000003a0: 6869 6e78 4170 7063 0100 0000 0000 0000  hinxAppc........
-000003b0: 0000 0000 0300 0000 0600 0000 4300 0000  ............C...
-000003c0: 733c 0000 0074 0083 007c 005f 017c 00a0  s<...t...|._.|..
-000003d0: 02a1 007d 017c 01a0 03a1 0044 005d 0b7d  ...}.|.....D.].}
-000003e0: 027c 006a 01a0 047c 027c 017c 0219 00a1  .|.j...|.|.|....
-000003f0: 0201 0071 0c74 0583 007c 005f 0664 0053  ...q.t...|._.d.S
-00000400: 00a9 014e 2907 720c 0000 00da 0872 6567  ...N).r......reg
-00000410: 6973 7472 79da 0f64 6973 636f 7665 725f  istry..discover_
-00000420: 7468 656d 6573 da04 6b65 7973 da0e 6164  themes..keys..ad
-00000430: 645f 6874 6d6c 5f74 6865 6d65 720d 0000  d_html_themer...
-00000440: 00da 0663 6f6e 6669 6729 03da 0473 656c  ...config)...sel
-00000450: 6672 0e00 0000 da0a 7468 656d 655f 6e61  fr......theme_na
-00000460: 6d65 7215 0000 0072 1500 0000 7216 0000  mer....r....r...
-00000470: 00da 085f 5f69 6e69 745f 5f1e 0000 0073  ...__init__....s
-00000480: 0a00 0000 0801 0801 0c01 1401 0c01 7a12  ..............z.
-00000490: 5370 6869 6e78 4170 702e 5f5f 696e 6974  SphinxApp.__init
-000004a0: 5f5f 6301 0000 0000 0000 0000 0000 0006  __c.............
-000004b0: 0000 0007 0000 0043 0000 0073 8e00 0000  .......C...s....
-000004c0: 6900 7d01 7400 a001 6401 a101 0100 7402  i.}.t...d.....t.
-000004d0: a003 7404 a101 4400 5d14 7d02 7402 6a05  ..t...D.].}.t.j.
-000004e0: a006 7404 7c02 a102 7d03 7402 6a05 a007  ..t.|...}.t.j...
-000004f0: 7c03 a101 731c 710c 7c03 7c01 7c02 3c00  |...s.q.|.|.|.<.
-00000500: 710c 7408 6402 8301 4400 5d14 7d04 7c04  q.t.d...D.].}.|.
-00000510: 6a09 7d02 7c04 a00a a100 7d05 7402 6a05  j.}.|.....}.t.j.
-00000520: a00b 7c05 6a0c a101 7d03 7c03 7c01 7c02  ..|.j...}.|.|.|.
-00000530: 3c00 7125 7400 a001 6403 6404 a006 7c01  <.q%t...d.d...|.
-00000540: a00d a100 a101 a102 0100 7c01 5300 2905  ..........|.S.).
-00000550: 4e7a 1964 6973 636f 7665 7269 6e67 2073  Nz.discovering s
-00000560: 7068 696e 7820 7468 656d 6573 7a12 7370  phinx themesz.sp
-00000570: 6869 6e78 2e68 746d 6c5f 7468 656d 6573  hinx.html_themes
-00000580: 7a1c 6469 7363 6f76 6572 6564 2073 7068  z.discovered sph
-00000590: 696e 7820 7468 656d 6573 3a20 2573 fa02  inx themes: %s..
-000005a0: 2c20 290e da06 6c6f 6767 6572 da05 6465  , )...logger..de
-000005b0: 6275 67da 026f 73da 076c 6973 7464 6972  bug..os..listdir
-000005c0: da11 5350 4849 4e58 5f54 4845 4d45 5f52  ..SPHINX_THEME_R
-000005d0: 4f4f 54da 0470 6174 68da 046a 6f69 6eda  OOT..path..join.
-000005e0: 0569 7364 6972 7202 0000 00da 046e 616d  .isdirr......nam
-000005f0: 65da 046c 6f61 64da 0764 6972 6e61 6d65  e..load..dirname
-00000600: da08 5f5f 6669 6c65 5f5f 721d 0000 0029  ..__file__r....)
-00000610: 0672 2000 0000 720e 0000 0072 2c00 0000  .r ...r....r,...
-00000620: da0a 7468 656d 655f 7061 7468 da0b 656e  ..theme_path..en
-00000630: 7472 795f 706f 696e 74da 066d 6f64 756c  try_point..modul
-00000640: 6572 1500 0000 7215 0000 0072 1600 0000  er....r....r....
-00000650: 721c 0000 0025 0000 0073 1c00 0000 0401  r....%...s......
-00000660: 0a02 0e03 0e01 0c02 0201 0a02 0c03 0601  ................
-00000670: 0801 0e01 0a02 1602 0402 7a19 5370 6869  ..........z.Sphi
-00000680: 6e78 4170 702e 6469 7363 6f76 6572 5f74  nxApp.discover_t
-00000690: 6865 6d65 734e 2905 7212 0000 0072 1300  hemesN).r....r..
-000006a0: 0000 7214 0000 0072 2200 0000 721c 0000  ..r....r"...r...
-000006b0: 0072 1500 0000 7215 0000 0072 1500 0000  .r....r....r....
-000006c0: 7216 0000 0072 1900 0000 1d00 0000 7306  r....r........s.
-000006d0: 0000 0008 0008 010c 0772 1900 0000 6300  .........r....c.
-000006e0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-000006f0: 0000 0040 0000 0073 4000 0000 6500 5a01  ...@...s@...e.Z.
-00000700: 6400 5a02 6900 6601 6401 6402 8401 5a03  d.Z.i.f.d.d...Z.
-00000710: 6403 6404 8400 5a04 6405 6406 8400 5a05  d.d...Z.d.d...Z.
-00000720: 6407 6408 8400 5a06 6409 640a 8400 5a07  d.d...Z.d.d...Z.
-00000730: 640b 640c 8400 5a08 640d 5300 290e da11  d.d...Z.d.S.)...
-00000740: 5370 6869 6e78 5468 656d 6543 6f6e 6669  SphinxThemeConfi
-00000750: 6763 0400 0000 0000 0000 0000 0000 0600  gc..............
-00000760: 0000 0500 0000 4300 0000 7362 0000 0074  ......C...sb...t
-00000770: 00a0 0164 017c 01a1 0201 007c 017c 005f  ...d.|.....|.|._
-00000780: 027c 037c 005f 037c 027c 005f 047c 00a0  .|.|._.|.|._.|..
-00000790: 05a1 007c 005f 0674 0783 007c 005f 087c  ...|._.t...|._.|
-000007a0: 006a 0644 005d 137d 047c 00a0 097c 04a1  .j.D.].}.|...|..
-000007b0: 017d 0574 00a0 0164 027c 05a1 0201 007c  .}.t...d.|.....|
-000007c0: 006a 08a0 0a7c 05a1 0101 0071 1b64 0053  .j...|.....q.d.S
-000007d0: 0029 034e 7a27 7365 7474 696e 6720 7570  .).Nz'setting up
-000007e0: 2073 7068 696e 7820 7468 656d 6520 636f   sphinx theme co
-000007f0: 6e66 6967 2066 6f72 2027 2573 277a 0a72  nfig for '%s'z.r
-00000800: 6561 6469 6e67 2025 7329 0b72 2400 0000  eading %s).r$...
-00000810: 7225 0000 0072 2100 0000 da10 6f70 7469  r%...r!.....opti
-00000820: 6f6e 5f6f 7665 7272 6964 6573 da03 6170  on_overrides..ap
-00000830: 70da 0e5f 6765 6e5f 6869 6572 6172 6368  p.._gen_hierarch
-00000840: 79da 0968 6965 7261 7263 6879 7203 0000  y..hierarchyr...
-00000850: 0072 1f00 0000 da16 5f67 656e 5f74 6865  .r......_gen_the
-00000860: 6d65 5f63 6f6e 6669 675f 7061 7468 da04  me_config_path..
-00000870: 7265 6164 2906 7220 0000 0072 2100 0000  read).r ...r!...
-00000880: 7235 0000 0072 3400 0000 722c 0000 00da  r5...r4...r,....
-00000890: 0b63 6f6e 6669 675f 7061 7468 7215 0000  .config_pathr...
-000008a0: 0072 1500 0000 7216 0000 0072 2200 0000  .r....r....r"...
-000008b0: 4100 0000 7316 0000 000c 0106 0206 0106  A...s...........
-000008c0: 010a 0208 010a 020a 010c 020e 0204 fb7a  ...............z
-000008d0: 1a53 7068 696e 7854 6865 6d65 436f 6e66  .SphinxThemeConf
-000008e0: 6967 2e5f 5f69 6e69 745f 5f63 0200 0000  ig.__init__c....
-000008f0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00000900: 4300 0000 7318 0000 0074 006a 01a0 027c  C...s....t.j...|
-00000910: 006a 036a 046a 057c 0119 0064 01a1 0253  .j.j.j.|...d...S
-00000920: 0029 024e fa0a 7468 656d 652e 636f 6e66  .).N..theme.conf
-00000930: 2906 7226 0000 0072 2900 0000 722a 0000  ).r&...r)...r*..
-00000940: 0072 3500 0000 721b 0000 00da 0b68 746d  .r5...r......htm
-00000950: 6c5f 7468 656d 6573 2902 7220 0000 0072  l_themes).r ...r
-00000960: 2c00 0000 7215 0000 0072 1500 0000 7216  ,...r....r....r.
-00000970: 0000 0072 3800 0000 5200 0000 7302 0000  ...r8...R...s...
-00000980: 0018 017a 2853 7068 696e 7854 6865 6d65  ...z(SphinxTheme
-00000990: 436f 6e66 6967 2e5f 6765 6e5f 7468 656d  Config._gen_them
-000009a0: 655f 636f 6e66 6967 5f70 6174 6863 0100  e_config_pathc..
-000009b0: 0000 0000 0000 0000 0000 0500 0000 0500  ................
-000009c0: 0000 4300 0000 736c 0000 007c 006a 0067  ..C...sl...|.j.g
-000009d0: 017d 017c 006a 007d 0209 007c 00a0 017c  .}.|.j.}...|...|
-000009e0: 02a1 017d 0374 0283 007d 047c 04a0 037c  ...}.t...}.|...|
-000009f0: 03a1 0101 007c 04a0 0464 0264 03a1 027d  .....|...d.d...}
-00000a00: 027c 0264 046b 0272 217c 0153 007c 027c  .|.d.k.r!|.S.|.|
-00000a10: 0176 0072 2f74 0564 05a0 067c 017c 0267  .v.r/t.d...|.|.g
-00000a20: 0117 00a1 0183 0182 017c 01a0 0764 067c  .........|...d.|
-00000a30: 02a1 0201 0071 0829 074e 54da 0574 6865  .....q.).NT..the
-00000a40: 6d65 da07 696e 6865 7269 74da 046e 6f6e  me..inherit..non
-00000a50: 657a 0420 2d3e 2072 0100 0000 2908 7221  ez. -> r....).r!
-00000a60: 0000 0072 3800 0000 7203 0000 0072 3900  ...r8...r....r9.
-00000a70: 0000 da03 6765 7472 1800 0000 722a 0000  ....getr....r*..
-00000a80: 00da 0669 6e73 6572 7429 0572 2000 0000  ...insert).r ...
-00000a90: 7237 0000 0072 3e00 0000 723a 0000 0072  r7...r>...r:...r
-00000aa0: 1f00 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
-00000ab0: 0000 0072 3600 0000 5500 0000 731e 0000  ...r6...U...s...
-00000ac0: 0008 0106 0102 020a 0106 010a 020c 0208  ................
-00000ad0: 0204 0108 0202 010e 0104 ff0c 0302 f17a  ...............z
-00000ae0: 2053 7068 696e 7854 6865 6d65 436f 6e66   SphinxThemeConf
-00000af0: 6967 2e5f 6765 6e5f 6869 6572 6172 6368  ig._gen_hierarch
-00000b00: 7963 0100 0000 0000 0000 0000 0000 0100  yc..............
-00000b10: 0000 0600 0000 4300 0000 732e 0000 007c  ......C...s....|
-00000b20: 006a 00a0 0164 0164 02a1 0264 0364 0484  .j...d.d...d.d..
-00000b30: 007c 006a 00a0 0164 0164 05a1 02a0 0264  .|.j...d.d.....d
-00000b40: 06a1 0144 0083 0164 079c 0253 0029 084e  ...D...d...S.).N
-00000b50: 723d 0000 00da 0a73 7479 6c65 7368 6565  r=.....styleshee
-00000b60: 7463 0100 0000 0000 0000 0000 0000 0200  tc..............
-00000b70: 0000 0400 0000 5300 0000 7314 0000 0067  ......S...s....g
-00000b80: 007c 005d 067d 017c 01a0 00a1 0091 0271  .|.].}.|.......q
-00000b90: 0253 0072 1500 0000 2901 da05 7374 7269  .S.r....)...stri
-00000ba0: 70a9 02da 022e 30da 0169 7215 0000 0072  p.....0..ir....r
-00000bb0: 1500 0000 7216 0000 00da 0a3c 6c69 7374  ....r......<list
-00000bc0: 636f 6d70 3e6e 0000 0073 0800 0000 0600  comp>n...s......
-00000bd0: 0202 06ff 06ff 7a36 5370 6869 6e78 5468  ......z6SphinxTh
-00000be0: 656d 6543 6f6e 6669 672e 6765 745f 7468  emeConfig.get_th
-00000bf0: 656d 655f 636f 6e66 6967 2e3c 6c6f 6361  eme_config.<loca
-00000c00: 6c73 3e2e 3c6c 6973 7463 6f6d 703e da08  ls>.<listcomp>..
-00000c10: 7369 6465 6261 7273 fa01 2c29 0272 4200  sidebars..,).rB.
-00000c20: 0000 7248 0000 0029 0372 1f00 0000 7240  ..rH...).r....r@
-00000c30: 0000 00da 0573 706c 6974 a901 7220 0000  .....split..r ..
-00000c40: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
-00000c50: da10 6765 745f 7468 656d 655f 636f 6e66  ..get_theme_conf
-00000c60: 6967 6a00 0000 730a 0000 000c 0206 0212  igj...s.........
-00000c70: 0204 fe06 fd7a 2253 7068 696e 7854 6865  .....z"SphinxThe
-00000c80: 6d65 436f 6e66 6967 2e67 6574 5f74 6865  meConfig.get_the
-00000c90: 6d65 5f63 6f6e 6669 6763 0100 0000 0000  me_configc......
-00000ca0: 0000 0000 0000 0300 0000 0500 0000 4300  ..............C.
-00000cb0: 0000 7338 0000 0069 007d 017c 006a 00a0  ..s8...i.}.|.j..
-00000cc0: 0164 01a1 0144 005d 0b7d 027c 006a 00a0  .d...D.].}.|.j..
-00000cd0: 0264 017c 02a1 027c 017c 023c 0071 087c  .d.|...|.|.<.q.|
-00000ce0: 01a0 037c 006a 04a1 0101 007c 0153 0029  ...|.j.....|.S.)
-00000cf0: 024e da07 6f70 7469 6f6e 7329 0572 1f00  .N..options).r..
-00000d00: 0000 724d 0000 0072 4000 0000 da06 7570  ..rM...r@.....up
-00000d10: 6461 7465 7234 0000 0029 0372 2000 0000  dater4...).r ...
-00000d20: da0b 7261 775f 6f70 7469 6f6e 73da 0b6f  ..raw_options..o
-00000d30: 7074 696f 6e5f 6e61 6d65 7215 0000 0072  ption_namer....r
-00000d40: 1500 0000 7216 0000 00da 1567 6574 5f72  ....r......get_r
-00000d50: 6177 5f74 6865 6d65 5f6f 7074 696f 6e73  aw_theme_options
-00000d60: 7400 0000 730a 0000 0004 0110 0214 010c  t...s...........
-00000d70: 0204 027a 2753 7068 696e 7854 6865 6d65  ...z'SphinxTheme
-00000d80: 436f 6e66 6967 2e67 6574 5f72 6177 5f74  Config.get_raw_t
-00000d90: 6865 6d65 5f6f 7074 696f 6e73 6301 0000  heme_optionsc...
-00000da0: 0000 0000 0000 0000 0006 0000 0004 0000  ................
-00000db0: 0043 0000 0073 3400 0000 7c00 a000 a100  .C...s4...|.....
-00000dc0: 7d01 6900 7d02 7c01 a001 a100 4400 5d0d  }.i.}.|.....D.].
-00000dd0: 5c02 7d03 7d04 6401 a002 7c03 a101 7d05  \.}.}.d...|...}.
-00000de0: 7c04 7c02 7c05 3c00 710a 7c02 5300 2902  |.|.|.<.q.|.S.).
-00000df0: 4e7a 0874 6865 6d65 5f7b 7d29 0372 5100  Nz.theme_{}).rQ.
-00000e00: 0000 da05 6974 656d 73da 0666 6f72 6d61  ....items..forma
-00000e10: 7429 0672 2000 0000 724f 0000 0072 4d00  t).r ...rO...rM.
-00000e20: 0000 5a0f 7261 775f 6f70 7469 6f6e 5f6e  ..Z.raw_option_n
-00000e30: 616d 65da 0576 616c 7565 7250 0000 0072  ame..valuerP...r
-00000e40: 1500 0000 7215 0000 0072 1600 0000 da11  ....r....r......
-00000e50: 6765 745f 7468 656d 655f 6f70 7469 6f6e  get_theme_option
-00000e60: 737e 0000 0073 0c00 0000 0801 0401 1002  s~...s..........
-00000e70: 0a01 0a01 0402 7a23 5370 6869 6e78 5468  ......z#SphinxTh
-00000e80: 656d 6543 6f6e 6669 672e 6765 745f 7468  emeConfig.get_th
-00000e90: 656d 655f 6f70 7469 6f6e 734e 2909 7212  eme_optionsN).r.
-00000ea0: 0000 0072 1300 0000 7214 0000 0072 2200  ...r....r....r".
-00000eb0: 0000 7238 0000 0072 3600 0000 724c 0000  ..r8...r6...rL..
-00000ec0: 0072 5100 0000 7255 0000 0072 1500 0000  .rQ...rU...r....
-00000ed0: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00000ee0: 3300 0000 4000 0000 730e 0000 0008 000c  3...@...s.......
-00000ef0: 0108 1108 0308 1508 0a0c 0a72 3300 0000  ...........r3...
-00000f00: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000f10: 0003 0000 0040 0000 0073 4200 0000 6500  .....@...sB...e.
-00000f20: 5a01 6400 5a02 6401 6900 6602 6402 6403  Z.d.Z.d.i.f.d.d.
-00000f30: 8401 5a03 6404 6405 8400 5a04 6406 6407  ..Z.d.d...Z.d.d.
-00000f40: 8400 5a05 6408 6409 8400 5a06 640a 640b  ..Z.d.d...Z.d.d.
-00000f50: 8400 5a07 640c 640d 8400 5a08 640e 5300  ..Z.d.d...Z.d.S.
-00000f60: 290f da0b 5370 6869 6e78 5468 656d 6554  )...SphinxThemeT
-00000f70: 6305 0000 0000 0000 0000 0000 0005 0000  c...............
-00000f80: 0009 0000 0043 0000 0073 9c00 0000 7c01  .....C...s....|.
-00000f90: 7c00 5f00 7c02 7c00 5f01 7402 8300 7c00  |._.|.|._.t...|.
-00000fa0: 5f03 7c01 7c00 6a03 6a04 6a05 7601 7226  _.|.|.j.j.j.v.r&
-00000fb0: 7406 6401 a007 7c01 6402 a008 6403 6404  t.d...|.d...d.d.
-00000fc0: 8400 7c00 6a03 6a04 6a05 a009 a100 4400  ..|.j.j.j.....D.
-00000fd0: 8301 a101 a102 8301 8201 740a 7c01 7c00  ..........t.|.|.
-00000fe0: 6a03 7c04 6405 8d03 7c00 5f0b 740c 7c00  j.|.d...|._.t.|.
-00000ff0: 6a03 6406 8d01 7c00 5f0d 740e 7c01 7c00  j.d...|._.t.|.|.
-00001000: 6a03 6a04 6a05 7c01 1900 7c00 6a0d 6407  j.j.j.|...|.j.d.
-00001010: 8d03 7c00 5f0f 7c03 724c 7c00 a010 a100  ..|._.|.rL|.....
-00001020: 0100 6400 5300 6400 5300 2908 4e7a 3173  ..d.S.d.S.).Nz1s
-00001030: 7068 696e 7820 7468 656d 6520 277b 7d27  phinx theme '{}'
-00001040: 206e 6f74 2066 6f75 6e64 2e20 6176 6169   not found. avai
-00001050: 6c61 626c 6520 7468 656d 6573 3a20 7b7d  lable themes: {}
-00001060: 7223 0000 0063 0100 0000 0000 0000 0000  r#...c..........
-00001070: 0000 0200 0000 0500 0000 5300 0000 7316  ..........S...s.
-00001080: 0000 0067 007c 005d 077d 0164 00a0 007c  ...g.|.].}.d...|
-00001090: 01a1 0191 0271 0253 0029 017a 0427 7b7d  .....q.S.).z.'{}
-000010a0: 2729 0172 5300 0000 7244 0000 0072 1500  ').rS...rD...r..
-000010b0: 0000 7215 0000 0072 1600 0000 7247 0000  ..r....r....rG..
-000010c0: 0094 0000 0073 0600 0000 0600 0201 0eff  .....s..........
-000010d0: 7a28 5370 6869 6e78 5468 656d 652e 5f5f  z(SphinxTheme.__
-000010e0: 696e 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e  init__.<locals>.
-000010f0: 3c6c 6973 7463 6f6d 703e 2901 7234 0000  <listcomp>).r4..
-00001100: 0029 0172 3500 0000 2903 722c 0000 0072  .).r5...).r,...r
-00001110: 3000 0000 da07 6661 6374 6f72 7929 1172  0.....factory).r
-00001120: 2c00 0000 da09 6275 696c 645f 6469 7272  ,.....build_dirr
-00001130: 1900 0000 7235 0000 0072 1b00 0000 723c  ....r5...r....r<
-00001140: 0000 0072 1000 0000 7253 0000 0072 2a00  ...r....rS...r*.
-00001150: 0000 721d 0000 0072 3300 0000 721f 0000  ..r....r3...r...
-00001160: 0072 0a00 0000 7257 0000 0072 0b00 0000  .r....rW...r....
-00001170: 723d 0000 00da 0573 6574 7570 2905 7220  r=.....setup).r 
-00001180: 0000 0072 2c00 0000 7258 0000 0072 5900  ...r,...rX...rY.
-00001190: 0000 724d 0000 0072 1500 0000 7215 0000  ..rM...r....r...
-000011a0: 0072 1600 0000 7222 0000 008a 0000 0073  .r....r".......s
-000011b0: 3400 0000 0601 0601 0802 0e02 0201 0401  4...............
-000011c0: 0201 0a01 0c01 06ff 02fe 04ff 0208 0201  ................
-000011d0: 0401 0201 08fd 0e06 0202 0201 0c01 0401  ................
-000011e0: 08fd 0406 0c01 04ff 7a14 5370 6869 6e78  ........z.Sphinx
-000011f0: 5468 656d 652e 5f5f 696e 6974 5f5f 6302  Theme.__init__c.
-00001200: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00001210: 0000 0043 0000 0073 2c00 0000 7400 a001  ...C...s,...t...
-00001220: 6401 7c01 a102 0100 7402 6a03 a004 7c01  d.|.....t.j...|.
-00001230: a101 7211 7405 a006 7c01 a101 5300 7402  ..r.t...|...S.t.
-00001240: a007 7c01 a101 5300 2902 4e7a 0972 6d20  ..|...S.).Nz.rm 
-00001250: 2d72 6620 2573 2908 7224 0000 0072 2500  -rf %s).r$...r%.
-00001260: 0000 7226 0000 0072 2900 0000 722b 0000  ..r&...r)...r+..
-00001270: 00da 0673 6875 7469 6cda 0672 6d74 7265  ...shutil..rmtre
-00001280: 65da 0675 6e6c 696e 6b29 0272 2000 0000  e..unlink).r ...
-00001290: 7229 0000 0072 1500 0000 7215 0000 0072  r)...r....r....r
-000012a0: 1600 0000 da02 726d aa00 0000 7308 0000  ......rm....s...
-000012b0: 000c 010c 020a 010a 027a 0e53 7068 696e  .........z.Sphin
-000012c0: 7854 6865 6d65 2e72 6d63 0300 0000 0000  xTheme.rmc......
-000012d0: 0000 0000 0000 0300 0000 0500 0000 4300  ..............C.
-000012e0: 0000 7332 0000 0074 00a0 0164 017c 017c  ..s2...t...d.|.|
-000012f0: 02a1 0301 0074 026a 03a0 047c 01a1 0172  .....t.j...|...r
-00001300: 1374 05a0 067c 017c 02a1 0253 0074 05a0  .t...|.|...S.t..
-00001310: 077c 017c 02a1 0253 0029 024e 7a0b 6370  .|.|...S.).Nz.cp
-00001320: 202d 7220 2573 2025 7329 0872 2400 0000   -r %s %s).r$...
-00001330: 7225 0000 0072 2600 0000 7229 0000 0072  r%...r&...r)...r
-00001340: 2b00 0000 725a 0000 00da 0863 6f70 7974  +...rZ.....copyt
-00001350: 7265 65da 0463 6f70 7929 0372 2000 0000  ree..copy).r ...
-00001360: da06 736f 7572 6365 da0b 6465 7374 696e  ..source..destin
-00001370: 6174 696f 6e72 1500 0000 7215 0000 0072  ationr....r....r
-00001380: 1600 0000 da02 6370 b200 0000 7308 0000  ......cp....s...
-00001390: 000e 010c 020c 010c 027a 0e53 7068 696e  .........z.Sphin
-000013a0: 7854 6865 6d65 2e63 7063 0100 0000 0000  xTheme.cpc......
-000013b0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-000013c0: 0000 7320 0000 007c 006a 0073 0b69 007c  ..s ...|.j.s.i.|
-000013d0: 006a 01a0 02a1 00a5 017c 005f 0074 037c  .j.......|._.t.|
-000013e0: 006a 0083 0153 0072 1a00 0000 2904 da23  .j...S.r....)..#
-000013f0: 5f73 7461 7469 635f 6669 6c65 5f74 656d  _static_file_tem
-00001400: 706c 6174 655f 636f 6e74 6578 745f 6361  plate_context_ca
-00001410: 6368 6572 1f00 0000 7255 0000 0072 0400  cher....rU...r..
-00001420: 0000 724b 0000 0072 1500 0000 7215 0000  ..rK...r....r...
-00001430: 0072 1600 0000 da20 6765 6e5f 7374 6174  .r..... gen_stat
-00001440: 6963 5f66 696c 655f 7465 6d70 6c61 7465  ic_file_template
-00001450: 5f63 6f6e 7465 7874 ba00 0000 730a 0000  _context....s...
-00001460: 0006 0102 0108 0106 ff0a 047a 2c53 7068  ...........z,Sph
-00001470: 696e 7854 6865 6d65 2e67 656e 5f73 7461  inxTheme.gen_sta
-00001480: 7469 635f 6669 6c65 5f74 656d 706c 6174  tic_file_templat
-00001490: 655f 636f 6e74 6578 7463 0100 0000 0000  e_contextc......
-000014a0: 0000 0000 0000 1200 0000 0b00 0000 4300  ..............C.
-000014b0: 0000 7374 0200 0074 00a0 0164 01a1 0101  ..st...t...d....
-000014c0: 0074 026a 03a0 047c 006a 0564 02a1 027c  .t.j...|.j.d...|
-000014d0: 005f 0674 026a 03a0 047c 006a 0564 03a1  ._.t.j...|.j.d..
-000014e0: 027c 005f 0774 02a0 087c 006a 06a1 0101  .|._.t...|.j....
-000014f0: 0074 02a0 087c 006a 07a1 0101 0069 007c  .t...|.j.....i.|
-00001500: 005f 0974 0a74 0b7c 006a 0ca0 0da1 0064  ._.t.t.|.j.....d
-00001510: 0464 058d 0264 068d 017c 005f 0e74 0f7c  .d...d...|._.t.|
-00001520: 006a 0e6a 1064 073c 0074 117c 006a 0e6a  .j.j.d.<.t.|.j.j
-00001530: 1064 083c 0074 127c 006a 0e6a 1064 093c  .d.<.t.|.j.j.d.<
-00001540: 007c 006a 0ca0 0da1 0064 0064 0064 0a85  .|.j.....d.d.d..
-00001550: 0319 0044 005d e87d 0174 026a 03a0 137c  ...D.].}.t.j...|
-00001560: 01a1 017d 0274 026a 03a0 047c 006a 067c  ...}.t.j...|.j.|
-00001570: 02a1 027d 0374 14a0 157c 017c 03a1 0201  ...}.t...|.|....
-00001580: 0074 026a 03a0 047c 0364 03a1 027d 0474  .t.j...|.d...}.t
-00001590: 026a 03a0 047c 0364 0ba1 027d 0574 026a  .j...|.d...}.t.j
-000015a0: 03a0 167c 04a1 0172 7e7c 00a0 177c 04a1  ...|...r~|...|..
-000015b0: 0101 0074 026a 03a0 167c 05a1 0172 897c  ...t.j...|...r.|
-000015c0: 00a0 177c 05a1 0101 0074 02a0 187c 01a1  ...|.....t...|..
-000015d0: 0144 005d 1c7d 067c 0664 0c76 0072 9571  .D.].}.|.d.v.r.q
-000015e0: 8e74 026a 03a0 047c 017c 06a1 027d 0774  .t.j...|.|...}.t
-000015f0: 026a 03a0 047c 006a 067c 06a1 027d 087c  .j...|.j.|...}.|
-00001600: 00a0 197c 077c 08a1 0201 0071 8e74 026a  ...|.|.....q.t.j
-00001610: 03a0 047c 0164 03a1 027d 0974 026a 03a0  ...|.d...}.t.j..
-00001620: 167c 09a1 0173 b971 4f74 02a0 1a7c 09a1  .|...s.qOt...|..
-00001630: 0144 005d 785c 037d 0a7d 0b7d 0c7c 0c44  .D.]x\.}.}.}.|.D
-00001640: 005d 707d 0d74 026a 03a0 047c 0a7c 0da1  .]p}.t.j...|.|..
-00001650: 027d 0774 026a 03a0 047c 006a 0774 026a  .}.t.j...|.j.t.j
-00001660: 03a0 1b7c 077c 09a1 02a1 027d 0874 026a  ...|.|.....}.t.j
-00001670: 03a0 1c7c 08a1 017d 0e74 026a 03a0 167c  ...|...}.t.j...|
-00001680: 0ea1 0173 ec74 02a0 087c 0ea1 0101 007c  ...s.t...|.....|
-00001690: 07a0 1d64 0da1 0173 f87c 00a0 197c 077c  ...d...s.|...|.|
-000016a0: 08a1 0201 0071 c574 00a0 0164 0e7c 077c  .....q.t...d.|.|
-000016b0: 08a1 0301 0074 026a 03a0 1b7c 077c 01a1  .....t.j...|.|..
-000016c0: 027d 0f7c 006a 0ea0 1e7c 0fa1 017d 107c  .}.|.j...|...}.|
-000016d0: 00a0 1fa1 007d 1174 207c 0864 0064 0f85  .....}.t |.d.d..
-000016e0: 0219 0064 1083 028f 137d 0d7c 0da0 217c  ...d.....}.|..!|
-000016f0: 106a 2264 1169 007c 11a4 018e 01a1 0101  .j"d.i.|........
-00001700: 0057 0064 0004 0004 0083 0301 006e 0931  .W.d.........n.1
-00001710: 0090 0173 3077 0101 0001 0001 0059 0001  ...s0w.......Y..
-00001720: 0071 c571 be71 4f64 0053 0029 124e 7a19  .q.q.qOd.S.).Nz.
-00001730: 7365 7474 696e 6720 7570 2066 6c61 6d69  setting up flami
-00001740: 6e67 6f20 7468 656d 65da 0974 656d 706c  ngo theme..templ
-00001750: 6174 6573 da06 7374 6174 6963 5429 01da  ates..staticT)..
-00001760: 0b66 6f6c 6c6f 776c 696e 6b73 2901 da06  .followlinks)...
-00001770: 6c6f 6164 6572 da06 746f 626f 6f6c da05  loader..tobool..
-00001780: 746f 6469 6dda 0574 6f69 6e74 e9ff ffff  todim..toint....
-00001790: ff72 3b00 0000 2902 7266 0000 0072 3b00  .r;...).rf...r;.
-000017a0: 0000 5a02 5f74 7a12 7265 6e64 6572 696e  ..Z._tz.renderin
-000017b0: 6720 2573 202d 3e20 2573 e9fe ffff ff7a  g %s -> %s.....z
-000017c0: 0277 2b72 1500 0000 2923 7224 0000 0072  .w+r....)#r$...r
-000017d0: 2500 0000 7226 0000 0072 2900 0000 722a  %...r&...r)...r*
-000017e0: 0000 0072 5800 0000 da0d 7465 6d70 6c61  ...rX.....templa
-000017f0: 7465 5f72 6f6f 745a 0b73 7461 7469 635f  te_rootZ.static_
-00001800: 726f 6f74 da08 6d61 6b65 6469 7273 7263  root..makedirsrc
-00001810: 0000 0072 0500 0000 7206 0000 0072 3d00  ...r....r....r=.
-00001820: 0000 da0e 6765 745f 7468 656d 655f 6469  ....get_theme_di
-00001830: 7273 5a0a 6a69 6e6a 6132 5f65 6e76 7207  rsZ.jinja2_envr.
-00001840: 0000 00da 0766 696c 7465 7273 7208 0000  .....filtersr...
-00001850: 0072 0900 0000 da08 6261 7365 6e61 6d65  .r......basename
-00001860: 725a 0000 0072 5e00 0000 da06 6578 6973  rZ...r^.....exis
-00001870: 7473 725d 0000 0072 2700 0000 7262 0000  tsr]...r'...rb..
-00001880: 00da 0477 616c 6bda 0772 656c 7061 7468  ...walk..relpath
-00001890: 722e 0000 00da 0865 6e64 7377 6974 68da  r......endswith.
-000018a0: 0c67 6574 5f74 656d 706c 6174 6572 6400  .get_templaterd.
-000018b0: 0000 da04 6f70 656e da05 7772 6974 65da  ....open..write.
-000018c0: 0672 656e 6465 7229 1272 2000 0000 5a09  .render).r ...Z.
-000018d0: 7468 656d 655f 6469 7272 2100 0000 5a0c  theme_dirr!...Z.
-000018e0: 7468 656d 655f 6f75 7470 7574 5a10 7468  theme_outputZ.th
-000018f0: 656d 655f 7374 6174 6963 5f64 6972 5a0c  eme_static_dirZ.
-00001900: 7468 656d 655f 636f 6e66 6967 7246 0000  theme_configrF..
-00001910: 0072 6000 0000 7261 0000 00da 0a73 7461  .r`...ra.....sta
-00001920: 7469 635f 6469 72da 0472 6f6f 74da 0464  tic_dir..root..d
-00001930: 6972 73da 0566 696c 6573 da01 665a 1364  irs..files..fZ.d
-00001940: 6573 7469 6e61 7469 6f6e 5f64 6972 6e61  estination_dirna
-00001950: 6d65 da0d 7465 6d70 6c61 7465 5f6e 616d  me..template_nam
-00001960: 65da 0874 656d 706c 6174 65da 1074 656d  e..template..tem
-00001970: 706c 6174 655f 636f 6e74 6578 7472 1500  plate_contextr..
-00001980: 0000 7215 0000 0072 1600 0000 7259 0000  ..r....r....rY..
-00001990: 00c2 0000 0073 7400 0000 0a01 1203 1201  .....st.........
-000019a0: 0c02 0c01 0603 0202 0201 0801 0201 04fe  ................
-000019b0: 08ff 0c07 0c01 0c01 1803 0c05 1001 0c02  ................
-000019c0: 0e03 0e01 0c02 0a01 0c02 0a01 0e03 0801  ................
-000019d0: 0201 0e02 1001 0e02 0e03 0c02 0201 1402  ................
-000019e0: 0801 0e01 0602 0401 0c01 04fe 0c05 0c02  ................
-000019f0: 0a01 0a03 0c01 0202 0e03 0e02 0c01 0801  ................
-00001a00: 1402 1801 1eff 0203 02e3 02ff 04dc 7a11  ..............z.
-00001a10: 5370 6869 6e78 5468 656d 652e 7365 7475  SphinxTheme.setu
-00001a20: 7063 0100 0000 0000 0000 0000 0000 0100  pc..............
-00001a30: 0000 0400 0000 4300 0000 7310 0000 0064  ......C...s....d
-00001a40: 01a0 007c 006a 017c 006a 02a1 0253 0029  ...|.j.|.j...S.)
-00001a50: 024e 7a17 3c53 7068 696e 7854 6865 6d65  .Nz.<SphinxTheme
-00001a60: 2827 7b7d 272c 207b 7d29 3e29 0372 5300  ('{}', {})>).rS.
-00001a70: 0000 722c 0000 0072 5800 0000 724b 0000  ..r,...rX...rK..
-00001a80: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
-00001a90: da08 5f5f 7265 7072 5f5f 1f01 0000 7302  ..__repr__....s.
-00001aa0: 0000 0010 017a 1453 7068 696e 7854 6865  .....z.SphinxThe
-00001ab0: 6d65 2e5f 5f72 6570 725f 5f4e 2909 7212  me.__repr__N).r.
-00001ac0: 0000 0072 1300 0000 7214 0000 0072 2200  ...r....r....r".
-00001ad0: 0000 725d 0000 0072 6200 0000 7264 0000  ..r]...rb...rd..
-00001ae0: 0072 5900 0000 7283 0000 0072 1500 0000  .rY...r....r....
-00001af0: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00001b00: 5600 0000 8900 0000 730e 0000 0008 000e  V.......s.......
-00001b10: 0108 2008 0808 0808 080c 5d72 5600 0000  .. .......]rV...
-00001b20: 2925 da0d 706b 675f 7265 736f 7572 6365  )%..pkg_resource
-00001b30: 7372 0200 0000 da0c 636f 6e66 6967 7061  sr......configpa
-00001b40: 7273 6572 7203 0000 0072 5f00 0000 7204  rserr....r_...r.
-00001b50: 0000 00da 076c 6f67 6769 6e67 725a 0000  .....loggingrZ..
-00001b60: 0072 2600 0000 da06 6a69 6e6a 6132 7205  .r&.....jinja2r.
-00001b70: 0000 0072 0600 0000 da11 7370 6869 6e78  ...r......sphinx
-00001b80: 2e6a 696e 6a61 3267 6c75 6572 0700 0000  .jinja2gluer....
-00001b90: 7208 0000 0072 0900 0000 da0e 7370 6869  r....r......sphi
-00001ba0: 6e78 2e74 6865 6d69 6e67 720a 0000 0072  nx.themingr....r
-00001bb0: 0b00 0000 da0f 7370 6869 6e78 2e72 6567  ......sphinx.reg
-00001bc0: 6973 7472 7972 0c00 0000 da0d 7370 6869  istryr......sphi
-00001bd0: 6e78 2e63 6f6e 6669 6772 0d00 0000 da06  nx.configr......
-00001be0: 7370 6869 6e78 7229 0000 0072 2a00 0000  sphinxr)...r*...
-00001bf0: 722e 0000 0072 2f00 0000 7228 0000 00da  r....r/...r(....
-00001c00: 0967 6574 4c6f 6767 6572 7224 0000 00da  .getLoggerr$....
-00001c10: 0945 7863 6570 7469 6f6e 7210 0000 0072  .Exceptionr....r
-00001c20: 1800 0000 7219 0000 0072 3300 0000 7256  ....r....r3...rV
-00001c30: 0000 0072 1500 0000 7215 0000 0072 1500  ...r....r....r..
-00001c40: 0000 7216 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00001c50: 3e01 0000 0073 2600 0000 0c00 0c01 0c01  >....s&.........
-00001c60: 0801 0801 0801 1002 1402 1001 0c01 0c01  ................
-00001c70: 0801 1802 0a02 1003 1004 0e04 0e23 1249  .............#.I
+00000060: 5a07 6400 6404 6c08 5a08 6400 6404 6c09  Z.d.d.l.Z.d.d.l.
+00000070: 5a09 6400 6405 6c0a 6d0b 5a0b 6d0c 5a0c  Z.d.d.l.m.Z.m.Z.
+00000080: 0100 6400 6406 6c0d 6d0e 5a0e 6d0f 5a0f  ..d.d.l.m.Z.m.Z.
+00000090: 6d10 5a10 0100 6400 6407 6c11 6d12 5a12  m.Z...d.d.l.m.Z.
+000000a0: 6d13 5a13 0100 6400 6408 6c14 6d15 5a15  m.Z...d.d.l.m.Z.
+000000b0: 0100 6400 6409 6c16 6d17 5a17 0100 6400  ..d.d.l.m.Z...d.
+000000c0: 6404 6c18 5a18 6508 6a19 a01a 6508 6a19  d.l.Z.e.j...e.j.
+000000d0: a01b 6518 6a1c a101 640a a102 5a1d 6506  ..e.j...d...Z.e.
+000000e0: a01e 640b a101 5a1f 4700 640c 640d 8400  ..d...Z.G.d.d...
+000000f0: 640d 6520 8303 5a21 4700 640e 640f 8400  d.e ..Z!G.d.d...
+00000100: 640f 6520 8303 5a22 4700 6410 6411 8400  d.e ..Z"G.d.d...
+00000110: 6411 8302 5a23 4700 6412 6413 8400 6413  d...Z#G.d.d...d.
+00000120: 8302 5a24 4700 6414 6415 8400 6415 8302  ..Z$G.d.d...d...
+00000130: 5a25 6404 5300 2916 e900 0000 0029 01da  Z%d.S.)......)..
+00000140: 1169 7465 725f 656e 7472 795f 706f 696e  .iter_entry_poin
+00000150: 7473 2901 da0f 5261 7743 6f6e 6669 6750  ts)...RawConfigP
+00000160: 6172 7365 7229 01da 0864 6565 7063 6f70  arser)...deepcop
+00000170: 794e 2902 da0b 456e 7669 726f 6e6d 656e  yN)...Environmen
+00000180: 74da 1046 696c 6553 7973 7465 6d4c 6f61  t..FileSystemLoa
+00000190: 6465 7229 03da 075f 746f 626f 6f6c da06  der)..._tobool..
+000001a0: 5f74 6f64 696d da06 5f74 6f69 6e74 2902  _todim.._toint).
+000001b0: da10 4854 4d4c 5468 656d 6546 6163 746f  ..HTMLThemeFacto
+000001c0: 7279 da05 5468 656d 6529 01da 1753 7068  ry..Theme)...Sph
+000001d0: 696e 7843 6f6d 706f 6e65 6e74 5265 6769  inxComponentRegi
+000001e0: 7374 7279 2901 da06 436f 6e66 6967 da06  stry)...Config..
+000001f0: 7468 656d 6573 7a1d 666c 616d 696e 676f  themesz.flamingo
+00000200: 2e70 6c75 6769 6e73 2e53 7068 696e 7854  .plugins.SphinxT
+00000210: 6865 6d65 7363 0000 0000 0000 0000 0000  hemesc..........
+00000220: 0000 0000 0000 0100 0000 4000 0000 f30c  ..........@.....
+00000230: 0000 0065 005a 0164 005a 0264 0153 0029  ...e.Z.d.Z.d.S.)
+00000240: 02da 1853 7068 696e 7854 6865 6d65 4e6f  ...SphinxThemeNo
+00000250: 7446 6f75 6e64 4572 726f 724e a903 da08  tFoundErrorN....
+00000260: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00000270: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00000280: 5f5f a900 7215 0000 0072 1500 0000 fa58  __..r....r.....X
+00000290: 2f68 6f6d 652f 6368 7269 732f 776f 726b  /home/chris/work
+000002a0: 2f50 726f 6a65 6374 732f 6769 7468 7562  /Projects/github
+000002b0: 2f66 6c61 6d69 6e67 6f2f 666c 616d 696e  /flamingo/flamin
+000002c0: 676f 2f70 6c75 6769 6e73 2f73 7068 696e  go/plugins/sphin
+000002d0: 785f 7468 656d 6573 2f73 7068 696e 785f  x_themes/sphinx_
+000002e0: 7468 656d 652e 7079 7210 0000 0016 0000  theme.pyr.......
+000002f0: 00f3 0400 0000 0800 0401 7210 0000 0063  ..........r....c
+00000300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000310: 0100 0000 4000 0000 720f 0000 0029 02da  ....@...r....)..
+00000320: 1a53 7068 696e 7843 6f6e 6669 6752 6563  .SphinxConfigRec
+00000330: 7572 7369 6f6e 4572 726f 724e 7211 0000  ursionErrorNr...
+00000340: 0072 1500 0000 7215 0000 0072 1500 0000  .r....r....r....
+00000350: 7216 0000 0072 1800 0000 1a00 0000 7217  r....r........r.
+00000360: 0000 0072 1800 0000 6300 0000 0000 0000  ...r....c.......
+00000370: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
+00000380: 0073 1c00 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+00000390: 6402 8400 5a03 6403 6404 8400 5a04 6405  d...Z.d.d...Z.d.
+000003a0: 5300 2906 da09 5370 6869 6e78 4170 7063  S.)...SphinxAppc
+000003b0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+000003c0: 0600 0000 4300 0000 733c 0000 0074 0083  ....C...s<...t..
+000003d0: 007c 005f 017c 00a0 02a1 007d 017c 01a0  .|._.|.....}.|..
+000003e0: 03a1 0044 005d 0b7d 027c 006a 01a0 047c  ...D.].}.|.j...|
+000003f0: 027c 017c 0219 00a1 0201 0071 0c74 0583  .|.|.......q.t..
+00000400: 007c 005f 0664 0053 0029 014e 2907 720c  .|._.d.S.).N).r.
+00000410: 0000 00da 0872 6567 6973 7472 79da 0f64  .....registry..d
+00000420: 6973 636f 7665 725f 7468 656d 6573 da04  iscover_themes..
+00000430: 6b65 7973 da0e 6164 645f 6874 6d6c 5f74  keys..add_html_t
+00000440: 6865 6d65 720d 0000 00da 0663 6f6e 6669  hemer......confi
+00000450: 6729 03da 0473 656c 6672 0e00 0000 da0a  g)...selfr......
+00000460: 7468 656d 655f 6e61 6d65 7215 0000 0072  theme_namer....r
+00000470: 1500 0000 7216 0000 00da 085f 5f69 6e69  ....r......__ini
+00000480: 745f 5f1f 0000 0073 0a00 0000 0801 0801  t__....s........
+00000490: 0c01 1401 0c01 7a12 5370 6869 6e78 4170  ......z.SphinxAp
+000004a0: 702e 5f5f 696e 6974 5f5f 6301 0000 0000  p.__init__c.....
+000004b0: 0000 0000 0000 0006 0000 0007 0000 0043  ...............C
+000004c0: 0000 0073 8e00 0000 6900 7d01 7400 a001  ...s....i.}.t...
+000004d0: 6401 a101 0100 7402 a003 7404 a101 4400  d.....t...t...D.
+000004e0: 5d14 7d02 7402 6a05 a006 7404 7c02 a102  ].}.t.j...t.|...
+000004f0: 7d03 7402 6a05 a007 7c03 a101 731c 710c  }.t.j...|...s.q.
+00000500: 7c03 7c01 7c02 3c00 710c 7408 6402 8301  |.|.|.<.q.t.d...
+00000510: 4400 5d14 7d04 7c04 6a09 7d02 7c04 a00a  D.].}.|.j.}.|...
+00000520: a100 7d05 7402 6a05 a00b 7c05 6a0c a101  ..}.t.j...|.j...
+00000530: 7d03 7c03 7c01 7c02 3c00 7125 7400 a001  }.|.|.|.<.q%t...
+00000540: 6403 6404 a006 7c01 a00d a100 a101 a102  d.d...|.........
+00000550: 0100 7c01 5300 2905 4e7a 1964 6973 636f  ..|.S.).Nz.disco
+00000560: 7665 7269 6e67 2073 7068 696e 7820 7468  vering sphinx th
+00000570: 656d 6573 7a12 7370 6869 6e78 2e68 746d  emesz.sphinx.htm
+00000580: 6c5f 7468 656d 6573 7a1c 6469 7363 6f76  l_themesz.discov
+00000590: 6572 6564 2073 7068 696e 7820 7468 656d  ered sphinx them
+000005a0: 6573 3a20 2573 fa02 2c20 290e da06 6c6f  es: %s.., )...lo
+000005b0: 6767 6572 da05 6465 6275 67da 026f 73da  gger..debug..os.
+000005c0: 076c 6973 7464 6972 da11 5350 4849 4e58  .listdir..SPHINX
+000005d0: 5f54 4845 4d45 5f52 4f4f 54da 0470 6174  _THEME_ROOT..pat
+000005e0: 68da 046a 6f69 6eda 0569 7364 6972 7202  h..join..isdirr.
+000005f0: 0000 00da 046e 616d 65da 046c 6f61 64da  .....name..load.
+00000600: 0764 6972 6e61 6d65 da08 5f5f 6669 6c65  .dirname..__file
+00000610: 5f5f 721c 0000 0029 0672 1f00 0000 720e  __r....).r....r.
+00000620: 0000 0072 2b00 0000 da0a 7468 656d 655f  ...r+.....theme_
+00000630: 7061 7468 da0b 656e 7472 795f 706f 696e  path..entry_poin
+00000640: 74da 066d 6f64 756c 6572 1500 0000 7215  t..moduler....r.
+00000650: 0000 0072 1600 0000 721b 0000 0026 0000  ...r....r....&..
+00000660: 0073 1c00 0000 0401 0a02 0e03 0e01 0c02  .s..............
+00000670: 0201 0a02 0c03 0601 0801 0e01 0a02 1602  ................
+00000680: 0402 7a19 5370 6869 6e78 4170 702e 6469  ..z.SphinxApp.di
+00000690: 7363 6f76 6572 5f74 6865 6d65 734e 2905  scover_themesN).
+000006a0: 7212 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
+000006b0: 2100 0000 721b 0000 0072 1500 0000 7215  !...r....r....r.
+000006c0: 0000 0072 1500 0000 7216 0000 0072 1900  ...r....r....r..
+000006d0: 0000 1e00 0000 7306 0000 0008 0008 010c  ......s.........
+000006e0: 0772 1900 0000 6300 0000 0000 0000 0000  .r....c.........
+000006f0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
+00000700: 4000 0000 6500 5a01 6400 5a02 6900 6601  @...e.Z.d.Z.i.f.
+00000710: 6401 6402 8401 5a03 6403 6404 8400 5a04  d.d...Z.d.d...Z.
+00000720: 6405 6406 8400 5a05 6407 6408 8400 5a06  d.d...Z.d.d...Z.
+00000730: 6409 640a 8400 5a07 640b 640c 8400 5a08  d.d...Z.d.d...Z.
+00000740: 640d 5300 290e da11 5370 6869 6e78 5468  d.S.)...SphinxTh
+00000750: 656d 6543 6f6e 6669 6763 0400 0000 0000  emeConfigc......
+00000760: 0000 0000 0000 0600 0000 0500 0000 4300  ..............C.
+00000770: 0000 7362 0000 0074 00a0 0164 017c 01a1  ..sb...t...d.|..
+00000780: 0201 007c 017c 005f 027c 037c 005f 037c  ...|.|._.|.|._.|
+00000790: 027c 005f 047c 00a0 05a1 007c 005f 0674  .|._.|.....|._.t
+000007a0: 0783 007c 005f 087c 006a 0644 005d 137d  ...|._.|.j.D.].}
+000007b0: 047c 00a0 097c 04a1 017d 0574 00a0 0164  .|...|...}.t...d
+000007c0: 027c 05a1 0201 007c 006a 08a0 0a7c 05a1  .|.....|.j...|..
+000007d0: 0101 0071 1b64 0053 0029 034e 7a27 7365  ...q.d.S.).Nz'se
+000007e0: 7474 696e 6720 7570 2073 7068 696e 7820  tting up sphinx 
+000007f0: 7468 656d 6520 636f 6e66 6967 2066 6f72  theme config for
+00000800: 2027 2573 277a 0a72 6561 6469 6e67 2025   '%s'z.reading %
+00000810: 7329 0b72 2300 0000 7224 0000 0072 2000  s).r#...r$...r .
+00000820: 0000 da10 6f70 7469 6f6e 5f6f 7665 7272  ....option_overr
+00000830: 6964 6573 da03 6170 70da 0e5f 6765 6e5f  ides..app.._gen_
+00000840: 6869 6572 6172 6368 79da 0968 6965 7261  hierarchy..hiera
+00000850: 7263 6879 7203 0000 0072 1e00 0000 da16  rchyr....r......
+00000860: 5f67 656e 5f74 6865 6d65 5f63 6f6e 6669  _gen_theme_confi
+00000870: 675f 7061 7468 da04 7265 6164 2906 721f  g_path..read).r.
+00000880: 0000 0072 2000 0000 7234 0000 0072 3300  ...r ...r4...r3.
+00000890: 0000 722b 0000 00da 0b63 6f6e 6669 675f  ..r+.....config_
+000008a0: 7061 7468 7215 0000 0072 1500 0000 7216  pathr....r....r.
+000008b0: 0000 0072 2100 0000 4200 0000 7316 0000  ...r!...B...s...
+000008c0: 000c 0106 0206 0106 010a 0208 010a 020a  ................
+000008d0: 010c 020e 0204 fb7a 1a53 7068 696e 7854  .......z.SphinxT
+000008e0: 6865 6d65 436f 6e66 6967 2e5f 5f69 6e69  hemeConfig.__ini
+000008f0: 745f 5f63 0200 0000 0000 0000 0000 0000  t__c............
+00000900: 0200 0000 0400 0000 4300 0000 7318 0000  ........C...s...
+00000910: 0074 006a 01a0 027c 006a 036a 046a 057c  .t.j...|.j.j.j.|
+00000920: 0119 0064 01a1 0253 0029 024e fa0a 7468  ...d...S.).N..th
+00000930: 656d 652e 636f 6e66 2906 7225 0000 0072  eme.conf).r%...r
+00000940: 2800 0000 7229 0000 0072 3400 0000 721a  (...r)...r4...r.
+00000950: 0000 00da 0b68 746d 6c5f 7468 656d 6573  .....html_themes
+00000960: 2902 721f 0000 0072 2b00 0000 7215 0000  ).r....r+...r...
+00000970: 0072 1500 0000 7216 0000 0072 3700 0000  .r....r....r7...
+00000980: 5300 0000 7302 0000 0018 017a 2853 7068  S...s......z(Sph
+00000990: 696e 7854 6865 6d65 436f 6e66 6967 2e5f  inxThemeConfig._
+000009a0: 6765 6e5f 7468 656d 655f 636f 6e66 6967  gen_theme_config
+000009b0: 5f70 6174 6863 0100 0000 0000 0000 0000  _pathc..........
+000009c0: 0000 0500 0000 0500 0000 4300 0000 736c  ..........C...sl
+000009d0: 0000 007c 006a 0067 017d 017c 006a 007d  ...|.j.g.}.|.j.}
+000009e0: 0209 007c 00a0 017c 02a1 017d 0374 0283  ...|...|...}.t..
+000009f0: 007d 047c 04a0 037c 03a1 0101 007c 04a0  .}.|...|.....|..
+00000a00: 0464 0264 03a1 027d 027c 0264 046b 0272  .d.d...}.|.d.k.r
+00000a10: 217c 0153 007c 027c 0176 0072 2f74 0564  !|.S.|.|.v.r/t.d
+00000a20: 05a0 067c 017c 0267 0117 00a1 0183 0182  ...|.|.g........
+00000a30: 017c 01a0 0764 067c 02a1 0201 0071 0829  .|...d.|.....q.)
+00000a40: 074e 54da 0574 6865 6d65 da07 696e 6865  .NT..theme..inhe
+00000a50: 7269 74da 046e 6f6e 657a 0420 2d3e 2072  rit..nonez. -> r
+00000a60: 0100 0000 2908 7220 0000 0072 3700 0000  ....).r ...r7...
+00000a70: 7203 0000 0072 3800 0000 da03 6765 7472  r....r8.....getr
+00000a80: 1800 0000 7229 0000 00da 0669 6e73 6572  ....r).....inser
+00000a90: 7429 0572 1f00 0000 7236 0000 0072 3d00  t).r....r6...r=.
+00000aa0: 0000 7239 0000 0072 1e00 0000 7215 0000  ..r9...r....r...
+00000ab0: 0072 1500 0000 7216 0000 0072 3500 0000  .r....r....r5...
+00000ac0: 5600 0000 731e 0000 0008 0106 0102 020a  V...s...........
+00000ad0: 0106 010a 020c 0208 0204 0108 0202 010e  ................
+00000ae0: 0104 ff0c 0302 f17a 2053 7068 696e 7854  .......z SphinxT
+00000af0: 6865 6d65 436f 6e66 6967 2e5f 6765 6e5f  hemeConfig._gen_
+00000b00: 6869 6572 6172 6368 7963 0100 0000 0000  hierarchyc......
+00000b10: 0000 0000 0000 0100 0000 0600 0000 4300  ..............C.
+00000b20: 0000 732e 0000 007c 006a 00a0 0164 0164  ..s....|.j...d.d
+00000b30: 02a1 0264 0364 0484 007c 006a 00a0 0164  ...d.d...|.j...d
+00000b40: 0164 05a1 02a0 0264 06a1 0144 0083 0164  .d.....d...D...d
+00000b50: 079c 0253 0029 084e 723c 0000 00da 0a73  ...S.).Nr<.....s
+00000b60: 7479 6c65 7368 6565 7463 0100 0000 0000  tylesheetc......
+00000b70: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
+00000b80: 0000 7314 0000 0067 007c 005d 067d 017c  ..s....g.|.].}.|
+00000b90: 01a0 00a1 0091 0271 0253 0072 1500 0000  .......q.S.r....
+00000ba0: 2901 da05 7374 7269 70a9 02da 022e 30da  )...strip.....0.
+00000bb0: 0169 7215 0000 0072 1500 0000 7216 0000  .ir....r....r...
+00000bc0: 00da 0a3c 6c69 7374 636f 6d70 3e6f 0000  ...<listcomp>o..
+00000bd0: 0073 0800 0000 0600 0202 06ff 06ff 7a36  .s............z6
+00000be0: 5370 6869 6e78 5468 656d 6543 6f6e 6669  SphinxThemeConfi
+00000bf0: 672e 6765 745f 7468 656d 655f 636f 6e66  g.get_theme_conf
+00000c00: 6967 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  ig.<locals>.<lis
+00000c10: 7463 6f6d 703e da08 7369 6465 6261 7273  tcomp>..sidebars
+00000c20: fa01 2c29 0272 4100 0000 7247 0000 0029  ..,).rA...rG...)
+00000c30: 0372 1e00 0000 723f 0000 00da 0573 706c  .r....r?.....spl
+00000c40: 6974 a901 721f 0000 0072 1500 0000 7215  it..r....r....r.
+00000c50: 0000 0072 1600 0000 da10 6765 745f 7468  ...r......get_th
+00000c60: 656d 655f 636f 6e66 6967 6b00 0000 730a  eme_configk...s.
+00000c70: 0000 000c 0206 0212 0204 fe06 fd7a 2253  .............z"S
+00000c80: 7068 696e 7854 6865 6d65 436f 6e66 6967  phinxThemeConfig
+00000c90: 2e67 6574 5f74 6865 6d65 5f63 6f6e 6669  .get_theme_confi
+00000ca0: 6763 0100 0000 0000 0000 0000 0000 0300  gc..............
+00000cb0: 0000 0500 0000 4300 0000 7338 0000 0069  ......C...s8...i
+00000cc0: 007d 017c 006a 00a0 0164 01a1 0144 005d  .}.|.j...d...D.]
+00000cd0: 0b7d 027c 006a 00a0 0264 017c 02a1 027c  .}.|.j...d.|...|
+00000ce0: 017c 023c 0071 087c 01a0 037c 006a 04a1  .|.<.q.|...|.j..
+00000cf0: 0101 007c 0153 0029 024e da07 6f70 7469  ...|.S.).N..opti
+00000d00: 6f6e 7329 0572 1e00 0000 724c 0000 0072  ons).r....rL...r
+00000d10: 3f00 0000 da06 7570 6461 7465 7233 0000  ?.....updater3..
+00000d20: 0029 0372 1f00 0000 da0b 7261 775f 6f70  .).r......raw_op
+00000d30: 7469 6f6e 73da 0b6f 7074 696f 6e5f 6e61  tions..option_na
+00000d40: 6d65 7215 0000 0072 1500 0000 7216 0000  mer....r....r...
+00000d50: 00da 1567 6574 5f72 6177 5f74 6865 6d65  ...get_raw_theme
+00000d60: 5f6f 7074 696f 6e73 7500 0000 730a 0000  _optionsu...s...
+00000d70: 0004 0110 0214 010c 0204 027a 2753 7068  ...........z'Sph
+00000d80: 696e 7854 6865 6d65 436f 6e66 6967 2e67  inxThemeConfig.g
+00000d90: 6574 5f72 6177 5f74 6865 6d65 5f6f 7074  et_raw_theme_opt
+00000da0: 696f 6e73 6301 0000 0000 0000 0000 0000  ionsc...........
+00000db0: 0006 0000 0004 0000 0043 0000 0073 3400  .........C...s4.
+00000dc0: 0000 7c00 a000 a100 7d01 6900 7d02 7c01  ..|.....}.i.}.|.
+00000dd0: a001 a100 4400 5d0d 5c02 7d03 7d04 6401  ....D.].\.}.}.d.
+00000de0: a002 7c03 a101 7d05 7c04 7c02 7c05 3c00  ..|...}.|.|.|.<.
+00000df0: 710a 7c02 5300 2902 4e7a 0874 6865 6d65  q.|.S.).Nz.theme
+00000e00: 5f7b 7d29 0372 5000 0000 da05 6974 656d  _{}).rP.....item
+00000e10: 73da 0666 6f72 6d61 7429 0672 1f00 0000  s..format).r....
+00000e20: 724e 0000 0072 4c00 0000 5a0f 7261 775f  rN...rL...Z.raw_
+00000e30: 6f70 7469 6f6e 5f6e 616d 65da 0576 616c  option_name..val
+00000e40: 7565 724f 0000 0072 1500 0000 7215 0000  uerO...r....r...
+00000e50: 0072 1600 0000 da11 6765 745f 7468 656d  .r......get_them
+00000e60: 655f 6f70 7469 6f6e 737f 0000 0073 0c00  e_options....s..
+00000e70: 0000 0801 0401 1002 0a01 0a01 0402 7a23  ..............z#
+00000e80: 5370 6869 6e78 5468 656d 6543 6f6e 6669  SphinxThemeConfi
+00000e90: 672e 6765 745f 7468 656d 655f 6f70 7469  g.get_theme_opti
+00000ea0: 6f6e 734e 2909 7212 0000 0072 1300 0000  onsN).r....r....
+00000eb0: 7214 0000 0072 2100 0000 7237 0000 0072  r....r!...r7...r
+00000ec0: 3500 0000 724b 0000 0072 5000 0000 7254  5...rK...rP...rT
+00000ed0: 0000 0072 1500 0000 7215 0000 0072 1500  ...r....r....r..
+00000ee0: 0000 7216 0000 0072 3200 0000 4100 0000  ..r....r2...A...
+00000ef0: 730e 0000 0008 000c 0108 1108 0308 1508  s...............
+00000f00: 0a0c 0a72 3200 0000 6300 0000 0000 0000  ...r2...c.......
+00000f10: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+00000f20: 0073 4200 0000 6500 5a01 6400 5a02 6401  .sB...e.Z.d.Z.d.
+00000f30: 6900 6602 6402 6403 8401 5a03 6404 6405  i.f.d.d...Z.d.d.
+00000f40: 8400 5a04 6406 6407 8400 5a05 6408 6409  ..Z.d.d...Z.d.d.
+00000f50: 8400 5a06 640a 640b 8400 5a07 640c 640d  ..Z.d.d...Z.d.d.
+00000f60: 8400 5a08 640e 5300 290f da0b 5370 6869  ..Z.d.S.)...Sphi
+00000f70: 6e78 5468 656d 6554 6305 0000 0000 0000  nxThemeTc.......
+00000f80: 0000 0000 0005 0000 0009 0000 0043 0000  .............C..
+00000f90: 0073 9c00 0000 7c01 7c00 5f00 7c02 7c00  .s....|.|._.|.|.
+00000fa0: 5f01 7402 8300 7c00 5f03 7c01 7c00 6a03  _.t...|._.|.|.j.
+00000fb0: 6a04 6a05 7601 7226 7406 6401 a007 7c01  j.j.v.r&t.d...|.
+00000fc0: 6402 a008 6403 6404 8400 7c00 6a03 6a04  d...d.d...|.j.j.
+00000fd0: 6a05 a009 a100 4400 8301 a101 a102 8301  j.....D.........
+00000fe0: 8201 740a 7c01 7c00 6a03 7c04 6405 8d03  ..t.|.|.j.|.d...
+00000ff0: 7c00 5f0b 740c 7c00 6a03 6406 8d01 7c00  |._.t.|.j.d...|.
+00001000: 5f0d 740e 7c01 7c00 6a03 6a04 6a05 7c01  _.t.|.|.j.j.j.|.
+00001010: 1900 7c00 6a0d 6407 8d03 7c00 5f0f 7c03  ..|.j.d...|._.|.
+00001020: 724c 7c00 a010 a100 0100 6400 5300 6400  rL|.......d.S.d.
+00001030: 5300 2908 4e7a 3173 7068 696e 7820 7468  S.).Nz1sphinx th
+00001040: 656d 6520 277b 7d27 206e 6f74 2066 6f75  eme '{}' not fou
+00001050: 6e64 2e20 6176 6169 6c61 626c 6520 7468  nd. available th
+00001060: 656d 6573 3a20 7b7d 7222 0000 0063 0100  emes: {}r"...c..
+00001070: 0000 0000 0000 0000 0000 0200 0000 0500  ................
+00001080: 0000 5300 0000 7316 0000 0067 007c 005d  ..S...s....g.|.]
+00001090: 077d 0164 00a0 007c 01a1 0191 0271 0253  .}.d...|.....q.S
+000010a0: 0029 017a 0427 7b7d 2729 0172 5200 0000  .).z.'{}').rR...
+000010b0: 7243 0000 0072 1500 0000 7215 0000 0072  rC...r....r....r
+000010c0: 1600 0000 7246 0000 0095 0000 0073 0600  ....rF.......s..
+000010d0: 0000 0600 0201 0eff 7a28 5370 6869 6e78  ........z(Sphinx
+000010e0: 5468 656d 652e 5f5f 696e 6974 5f5f 2e3c  Theme.__init__.<
+000010f0: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00001100: 703e 2901 7233 0000 0029 0172 3400 0000  p>).r3...).r4...
+00001110: 2903 722b 0000 0072 2f00 0000 da07 6661  ).r+...r/.....fa
+00001120: 6374 6f72 7929 1172 2b00 0000 da09 6275  ctory).r+.....bu
+00001130: 696c 645f 6469 7272 1900 0000 7234 0000  ild_dirr....r4..
+00001140: 0072 1a00 0000 723b 0000 0072 1000 0000  .r....r;...r....
+00001150: 7252 0000 0072 2900 0000 721c 0000 0072  rR...r)...r....r
+00001160: 3200 0000 721e 0000 0072 0a00 0000 7256  2...r....r....rV
+00001170: 0000 0072 0b00 0000 723c 0000 00da 0573  ...r....r<.....s
+00001180: 6574 7570 2905 721f 0000 0072 2b00 0000  etup).r....r+...
+00001190: 7257 0000 0072 5800 0000 724c 0000 0072  rW...rX...rL...r
+000011a0: 1500 0000 7215 0000 0072 1600 0000 7221  ....r....r....r!
+000011b0: 0000 008b 0000 0073 3400 0000 0601 0601  .......s4.......
+000011c0: 0802 0e02 0201 0401 0201 0a01 0c01 06ff  ................
+000011d0: 02fe 04ff 0208 0201 0401 0201 08fd 0e06  ................
+000011e0: 0202 0201 0c01 0401 08fd 0406 0c01 04ff  ................
+000011f0: 7a14 5370 6869 6e78 5468 656d 652e 5f5f  z.SphinxTheme.__
+00001200: 696e 6974 5f5f 6302 0000 0000 0000 0000  init__c.........
+00001210: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
+00001220: 2c00 0000 7400 a001 6401 7c01 a102 0100  ,...t...d.|.....
+00001230: 7402 6a03 a004 7c01 a101 7211 7405 a006  t.j...|...r.t...
+00001240: 7c01 a101 5300 7402 a007 7c01 a101 5300  |...S.t...|...S.
+00001250: 2902 4e7a 0972 6d20 2d72 6620 2573 2908  ).Nz.rm -rf %s).
+00001260: 7223 0000 0072 2400 0000 7225 0000 0072  r#...r$...r%...r
+00001270: 2800 0000 722a 0000 00da 0673 6875 7469  (...r*.....shuti
+00001280: 6cda 0672 6d74 7265 65da 0675 6e6c 696e  l..rmtree..unlin
+00001290: 6b29 0272 1f00 0000 7228 0000 0072 1500  k).r....r(...r..
+000012a0: 0000 7215 0000 0072 1600 0000 da02 726d  ..r....r......rm
+000012b0: ab00 0000 7308 0000 000c 010c 020a 010a  ....s...........
+000012c0: 027a 0e53 7068 696e 7854 6865 6d65 2e72  .z.SphinxTheme.r
+000012d0: 6d63 0300 0000 0000 0000 0000 0000 0300  mc..............
+000012e0: 0000 0500 0000 4300 0000 7332 0000 0074  ......C...s2...t
+000012f0: 00a0 0164 017c 017c 02a1 0301 0074 026a  ...d.|.|.....t.j
+00001300: 03a0 047c 01a1 0172 1374 05a0 067c 017c  ...|...r.t...|.|
+00001310: 02a1 0253 0074 05a0 077c 017c 02a1 0253  ...S.t...|.|...S
+00001320: 0029 024e 7a0b 6370 202d 7220 2573 2025  .).Nz.cp -r %s %
+00001330: 7329 0872 2300 0000 7224 0000 0072 2500  s).r#...r$...r%.
+00001340: 0000 7228 0000 0072 2a00 0000 7259 0000  ..r(...r*...rY..
+00001350: 00da 0863 6f70 7974 7265 65da 0463 6f70  ...copytree..cop
+00001360: 7929 0372 1f00 0000 da06 736f 7572 6365  y).r......source
+00001370: da0b 6465 7374 696e 6174 696f 6e72 1500  ..destinationr..
+00001380: 0000 7215 0000 0072 1600 0000 da02 6370  ..r....r......cp
+00001390: b300 0000 7308 0000 000e 010c 020c 010c  ....s...........
+000013a0: 027a 0e53 7068 696e 7854 6865 6d65 2e63  .z.SphinxTheme.c
+000013b0: 7063 0100 0000 0000 0000 0000 0000 0100  pc..............
+000013c0: 0000 0300 0000 4300 0000 7334 0000 007c  ......C...s4...|
+000013d0: 006a 0073 1569 007c 006a 01a0 02a1 00a5  .j.s.i.|.j......
+000013e0: 017c 005f 0074 036a 0464 0064 0185 0219  .|._.t.j.d.d....
+000013f0: 007c 006a 0064 023c 0074 057c 006a 0083  .|.j.d.<.t.|.j..
+00001400: 0153 0029 034e e905 0000 005a 1564 6f63  .S.).N.....Z.doc
+00001410: 7574 696c 735f 7665 7273 696f 6e5f 696e  utils_version_in
+00001420: 666f 2906 da23 5f73 7461 7469 635f 6669  fo)..#_static_fi
+00001430: 6c65 5f74 656d 706c 6174 655f 636f 6e74  le_template_cont
+00001440: 6578 745f 6361 6368 6572 1e00 0000 7254  ext_cacher....rT
+00001450: 0000 00da 0864 6f63 7574 696c 73da 105f  .....docutils.._
+00001460: 5f76 6572 7369 6f6e 5f69 6e66 6f5f 5f72  _version_info__r
+00001470: 0400 0000 724a 0000 0072 1500 0000 7215  ....rJ...r....r.
+00001480: 0000 0072 1600 0000 da20 6765 6e5f 7374  ...r..... gen_st
+00001490: 6174 6963 5f66 696c 655f 7465 6d70 6c61  atic_file_templa
+000014a0: 7465 5f63 6f6e 7465 7874 bb00 0000 730c  te_context....s.
+000014b0: 0000 0006 0102 0108 0106 ff14 030a 027a  ...............z
+000014c0: 2c53 7068 696e 7854 6865 6d65 2e67 656e  ,SphinxTheme.gen
+000014d0: 5f73 7461 7469 635f 6669 6c65 5f74 656d  _static_file_tem
+000014e0: 706c 6174 655f 636f 6e74 6578 7463 0100  plate_contextc..
+000014f0: 0000 0000 0000 0000 0000 1200 0000 0b00  ................
+00001500: 0000 4300 0000 7374 0200 0074 00a0 0164  ..C...st...t...d
+00001510: 01a1 0101 0074 026a 03a0 047c 006a 0564  .....t.j...|.j.d
+00001520: 02a1 027c 005f 0674 026a 03a0 047c 006a  ...|._.t.j...|.j
+00001530: 0564 03a1 027c 005f 0774 02a0 087c 006a  .d...|._.t...|.j
+00001540: 06a1 0101 0074 02a0 087c 006a 07a1 0101  .....t...|.j....
+00001550: 0069 007c 005f 0974 0a74 0b7c 006a 0ca0  .i.|._.t.t.|.j..
+00001560: 0da1 0064 0464 058d 0264 068d 017c 005f  ...d.d...d...|._
+00001570: 0e74 0f7c 006a 0e6a 1064 073c 0074 117c  .t.|.j.j.d.<.t.|
+00001580: 006a 0e6a 1064 083c 0074 127c 006a 0e6a  .j.j.d.<.t.|.j.j
+00001590: 1064 093c 007c 006a 0ca0 0da1 0064 0064  .d.<.|.j.....d.d
+000015a0: 0064 0a85 0319 0044 005d e87d 0174 026a  .d.....D.].}.t.j
+000015b0: 03a0 137c 01a1 017d 0274 026a 03a0 047c  ...|...}.t.j...|
+000015c0: 006a 067c 02a1 027d 0374 14a0 157c 017c  .j.|...}.t...|.|
+000015d0: 03a1 0201 0074 026a 03a0 047c 0364 03a1  .....t.j...|.d..
+000015e0: 027d 0474 026a 03a0 047c 0364 0ba1 027d  .}.t.j...|.d...}
+000015f0: 0574 026a 03a0 167c 04a1 0172 7e7c 00a0  .t.j...|...r~|..
+00001600: 177c 04a1 0101 0074 026a 03a0 167c 05a1  .|.....t.j...|..
+00001610: 0172 897c 00a0 177c 05a1 0101 0074 02a0  .r.|...|.....t..
+00001620: 187c 01a1 0144 005d 1c7d 067c 0664 0c76  .|...D.].}.|.d.v
+00001630: 0072 9571 8e74 026a 03a0 047c 017c 06a1  .r.q.t.j...|.|..
+00001640: 027d 0774 026a 03a0 047c 006a 067c 06a1  .}.t.j...|.j.|..
+00001650: 027d 087c 00a0 197c 077c 08a1 0201 0071  .}.|...|.|.....q
+00001660: 8e74 026a 03a0 047c 0164 03a1 027d 0974  .t.j...|.d...}.t
+00001670: 026a 03a0 167c 09a1 0173 b971 4f74 02a0  .j...|...s.qOt..
+00001680: 1a7c 09a1 0144 005d 785c 037d 0a7d 0b7d  .|...D.]x\.}.}.}
+00001690: 0c7c 0c44 005d 707d 0d74 026a 03a0 047c  .|.D.]p}.t.j...|
+000016a0: 0a7c 0da1 027d 0774 026a 03a0 047c 006a  .|...}.t.j...|.j
+000016b0: 0774 026a 03a0 1b7c 077c 09a1 02a1 027d  .t.j...|.|.....}
+000016c0: 0874 026a 03a0 1c7c 08a1 017d 0e74 026a  .t.j...|...}.t.j
+000016d0: 03a0 167c 0ea1 0173 ec74 02a0 087c 0ea1  ...|...s.t...|..
+000016e0: 0101 007c 07a0 1d64 0da1 0173 f87c 00a0  ...|...d...s.|..
+000016f0: 197c 077c 08a1 0201 0071 c574 00a0 0164  .|.|.....q.t...d
+00001700: 0e7c 077c 08a1 0301 0074 026a 03a0 1b7c  .|.|.....t.j...|
+00001710: 077c 01a1 027d 0f7c 006a 0ea0 1e7c 0fa1  .|...}.|.j...|..
+00001720: 017d 107c 00a0 1fa1 007d 1174 207c 0864  .}.|.....}.t |.d
+00001730: 0064 0f85 0219 0064 1083 028f 137d 0d7c  .d.....d.....}.|
+00001740: 0da0 217c 106a 2264 1169 007c 11a4 018e  ..!|.j"d.i.|....
+00001750: 01a1 0101 0057 0064 0004 0004 0083 0301  .....W.d........
+00001760: 006e 0931 0090 0173 3077 0101 0001 0001  .n.1...s0w......
+00001770: 0059 0001 0071 c571 be71 4f64 0053 0029  .Y...q.q.qOd.S.)
+00001780: 124e 7a19 7365 7474 696e 6720 7570 2066  .Nz.setting up f
+00001790: 6c61 6d69 6e67 6f20 7468 656d 65da 0974  lamingo theme..t
+000017a0: 656d 706c 6174 6573 da06 7374 6174 6963  emplates..static
+000017b0: 5429 01da 0b66 6f6c 6c6f 776c 696e 6b73  T)...followlinks
+000017c0: 2901 da06 6c6f 6164 6572 da06 746f 626f  )...loader..tobo
+000017d0: 6f6c da05 746f 6469 6dda 0574 6f69 6e74  ol..todim..toint
+000017e0: e9ff ffff ff72 3a00 0000 2902 7268 0000  .....r:...).rh..
+000017f0: 0072 3a00 0000 5a02 5f74 7a12 7265 6e64  .r:...Z._tz.rend
+00001800: 6572 696e 6720 2573 202d 3e20 2573 e9fe  ering %s -> %s..
+00001810: ffff ff7a 0277 2b72 1500 0000 2923 7223  ...z.w+r....)#r#
+00001820: 0000 0072 2400 0000 7225 0000 0072 2800  ...r$...r%...r(.
+00001830: 0000 7229 0000 0072 5700 0000 da0d 7465  ..r)...rW.....te
+00001840: 6d70 6c61 7465 5f72 6f6f 745a 0b73 7461  mplate_rootZ.sta
+00001850: 7469 635f 726f 6f74 da08 6d61 6b65 6469  tic_root..makedi
+00001860: 7273 7263 0000 0072 0500 0000 7206 0000  rsrc...r....r...
+00001870: 0072 3c00 0000 da0e 6765 745f 7468 656d  .r<.....get_them
+00001880: 655f 6469 7273 5a0a 6a69 6e6a 6132 5f65  e_dirsZ.jinja2_e
+00001890: 6e76 7207 0000 00da 0766 696c 7465 7273  nvr......filters
+000018a0: 7208 0000 0072 0900 0000 da08 6261 7365  r....r......base
+000018b0: 6e61 6d65 7259 0000 0072 5d00 0000 da06  namerY...r].....
+000018c0: 6578 6973 7473 725c 0000 0072 2600 0000  existsr\...r&...
+000018d0: 7261 0000 00da 0477 616c 6bda 0772 656c  ra.....walk..rel
+000018e0: 7061 7468 722d 0000 00da 0865 6e64 7377  pathr-.....endsw
+000018f0: 6974 68da 0c67 6574 5f74 656d 706c 6174  ith..get_templat
+00001900: 6572 6600 0000 da04 6f70 656e da05 7772  erf.....open..wr
+00001910: 6974 65da 0672 656e 6465 7229 1272 1f00  ite..render).r..
+00001920: 0000 5a09 7468 656d 655f 6469 7272 2000  ..Z.theme_dirr .
+00001930: 0000 5a0c 7468 656d 655f 6f75 7470 7574  ..Z.theme_output
+00001940: 5a10 7468 656d 655f 7374 6174 6963 5f64  Z.theme_static_d
+00001950: 6972 5a0c 7468 656d 655f 636f 6e66 6967  irZ.theme_config
+00001960: 7245 0000 0072 5f00 0000 7260 0000 00da  rE...r_...r`....
+00001970: 0a73 7461 7469 635f 6469 72da 0472 6f6f  .static_dir..roo
+00001980: 74da 0464 6972 73da 0566 696c 6573 da01  t..dirs..files..
+00001990: 665a 1364 6573 7469 6e61 7469 6f6e 5f64  fZ.destination_d
+000019a0: 6972 6e61 6d65 da0d 7465 6d70 6c61 7465  irname..template
+000019b0: 5f6e 616d 65da 0874 656d 706c 6174 65da  _name..template.
+000019c0: 1074 656d 706c 6174 655f 636f 6e74 6578  .template_contex
+000019d0: 7472 1500 0000 7215 0000 0072 1600 0000  tr....r....r....
+000019e0: 7258 0000 00c4 0000 0073 7400 0000 0a01  rX.......st.....
+000019f0: 1203 1201 0c02 0c01 0603 0202 0201 0801  ................
+00001a00: 0201 04fe 08ff 0c07 0c01 0c01 1803 0c05  ................
+00001a10: 1001 0c02 0e03 0e01 0c02 0a01 0c02 0a01  ................
+00001a20: 0e03 0801 0201 0e02 1001 0e02 0e03 0c02  ................
+00001a30: 0201 1402 0801 0e01 0602 0401 0c01 04fe  ................
+00001a40: 0c05 0c02 0a01 0a03 0c01 0202 0e03 0e02  ................
+00001a50: 0c01 0801 1402 1801 1eff 0203 02e3 02ff  ................
+00001a60: 04dc 7a11 5370 6869 6e78 5468 656d 652e  ..z.SphinxTheme.
+00001a70: 7365 7475 7063 0100 0000 0000 0000 0000  setupc..........
+00001a80: 0000 0100 0000 0400 0000 4300 0000 7310  ..........C...s.
+00001a90: 0000 0064 01a0 007c 006a 017c 006a 02a1  ...d...|.j.|.j..
+00001aa0: 0253 0029 024e 7a17 3c53 7068 696e 7854  .S.).Nz.<SphinxT
+00001ab0: 6865 6d65 2827 7b7d 272c 207b 7d29 3e29  heme('{}', {})>)
+00001ac0: 0372 5200 0000 722b 0000 0072 5700 0000  .rR...r+...rW...
+00001ad0: 724a 0000 0072 1500 0000 7215 0000 0072  rJ...r....r....r
+00001ae0: 1600 0000 da08 5f5f 7265 7072 5f5f 2101  ......__repr__!.
+00001af0: 0000 7302 0000 0010 017a 1453 7068 696e  ..s......z.Sphin
+00001b00: 7854 6865 6d65 2e5f 5f72 6570 725f 5f4e  xTheme.__repr__N
+00001b10: 2909 7212 0000 0072 1300 0000 7214 0000  ).r....r....r...
+00001b20: 0072 2100 0000 725c 0000 0072 6100 0000  .r!...r\...ra...
+00001b30: 7266 0000 0072 5800 0000 7285 0000 0072  rf...rX...r....r
+00001b40: 1500 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
+00001b50: 0000 0072 5500 0000 8a00 0000 730e 0000  ...rU.......s...
+00001b60: 0008 000e 0108 2008 0808 0808 090c 5d72  ...... .......]r
+00001b70: 5500 0000 2926 da0d 706b 675f 7265 736f  U...)&..pkg_reso
+00001b80: 7572 6365 7372 0200 0000 da0c 636f 6e66  urcesr......conf
+00001b90: 6967 7061 7273 6572 7203 0000 0072 5e00  igparserr....r^.
+00001ba0: 0000 7204 0000 00da 076c 6f67 6769 6e67  ..r......logging
+00001bb0: 7259 0000 0072 2500 0000 7264 0000 00da  rY...r%...rd....
+00001bc0: 066a 696e 6a61 3272 0500 0000 7206 0000  .jinja2r....r...
+00001bd0: 00da 1173 7068 696e 782e 6a69 6e6a 6132  ...sphinx.jinja2
+00001be0: 676c 7565 7207 0000 0072 0800 0000 7209  gluer....r....r.
+00001bf0: 0000 00da 0e73 7068 696e 782e 7468 656d  .....sphinx.them
+00001c00: 696e 6772 0a00 0000 720b 0000 00da 0f73  ingr....r......s
+00001c10: 7068 696e 782e 7265 6769 7374 7279 720c  phinx.registryr.
+00001c20: 0000 00da 0d73 7068 696e 782e 636f 6e66  .....sphinx.conf
+00001c30: 6967 720d 0000 00da 0673 7068 696e 7872  igr......sphinxr
+00001c40: 2800 0000 7229 0000 0072 2d00 0000 722e  (...r)...r-...r.
+00001c50: 0000 0072 2700 0000 da09 6765 744c 6f67  ...r'.....getLog
+00001c60: 6765 7272 2300 0000 da09 4578 6365 7074  gerr#.....Except
+00001c70: 696f 6e72 1000 0000 7218 0000 0072 1900  ionr....r....r..
+00001c80: 0000 7232 0000 0072 5500 0000 7215 0000  ..r2...rU...r...
+00001c90: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
+00001ca0: da08 3c6d 6f64 756c 653e 0100 0000 7328  ..<module>....s(
+00001cb0: 0000 000c 000c 010c 0108 0108 0108 0108  ................
+00001cc0: 0110 0214 0210 010c 010c 0108 0118 020a  ................
+00001cd0: 0210 0310 040e 040e 2312 49              ........#.I
```

### Comparing `flamingo-1.8/flamingo/plugins/sphinx_themes/__pycache__/sphinx_theme.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/sphinx_themes/__pycache__/sphinx_theme.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May 12 15:07:02 2022 UTC, .py size: 8762 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,456 +1,462 @@
-00000000: 610d 0d0a 0000 0000 9622 7d62 3a22 0000  a........"}b:"..
+00000000: 610d 0d0a 0000 0000 5399 7c63 b822 0000  a.......S.|c."..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 0001 0000 6400  .....@...s....d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6404 6c06 5a06 6400 6404 6c07  ..d.d.l.Z.d.d.l.
-00000060: 5a07 6400 6404 6c08 5a08 6400 6405 6c09  Z.d.d.l.Z.d.d.l.
-00000070: 6d0a 5a0a 6d0b 5a0b 0100 6400 6406 6c0c  m.Z.m.Z...d.d.l.
-00000080: 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 0100 6400  m.Z.m.Z.m.Z...d.
-00000090: 6407 6c10 6d11 5a11 6d12 5a12 0100 6400  d.l.m.Z.m.Z...d.
-000000a0: 6408 6c13 6d14 5a14 0100 6400 6409 6c15  d.l.m.Z...d.d.l.
-000000b0: 6d16 5a16 0100 6400 6404 6c17 5a17 6508  m.Z...d.d.l.Z.e.
-000000c0: 6a18 a019 6508 6a18 a01a 6517 6a1b a101  j...e.j...e.j...
-000000d0: 640a a102 5a1c 6506 a01d 640b a101 5a1e  d...Z.e...d...Z.
-000000e0: 4700 640c 640d 8400 640d 651f 8303 5a20  G.d.d...d.e...Z 
-000000f0: 4700 640e 640f 8400 640f 651f 8303 5a21  G.d.d...d.e...Z!
-00000100: 4700 6410 6411 8400 6411 8302 5a22 4700  G.d.d...d...Z"G.
-00000110: 6412 6413 8400 6413 8302 5a23 4700 6414  d.d...d...Z#G.d.
-00000120: 6415 8400 6415 8302 5a24 6404 5300 2916  d...d...Z$d.S.).
-00000130: e900 0000 0029 01da 1169 7465 725f 656e  .....)...iter_en
-00000140: 7472 795f 706f 696e 7473 2901 da0f 5261  try_points)...Ra
-00000150: 7743 6f6e 6669 6750 6172 7365 7229 01da  wConfigParser)..
-00000160: 0864 6565 7063 6f70 794e 2902 da0b 456e  .deepcopyN)...En
-00000170: 7669 726f 6e6d 656e 74da 1046 696c 6553  vironment..FileS
-00000180: 7973 7465 6d4c 6f61 6465 7229 03da 075f  ystemLoader)..._
-00000190: 746f 626f 6f6c da06 5f74 6f64 696d da06  tobool.._todim..
-000001a0: 5f74 6f69 6e74 2902 da10 4854 4d4c 5468  _toint)...HTMLTh
-000001b0: 656d 6546 6163 746f 7279 da05 5468 656d  emeFactory..Them
-000001c0: 6529 01da 1753 7068 696e 7843 6f6d 706f  e)...SphinxCompo
-000001d0: 6e65 6e74 5265 6769 7374 7279 2901 da06  nentRegistry)...
-000001e0: 436f 6e66 6967 da06 7468 656d 6573 7a1d  Config..themesz.
-000001f0: 666c 616d 696e 676f 2e70 6c75 6769 6e73  flamingo.plugins
-00000200: 2e53 7068 696e 7854 6865 6d65 7363 0000  .SphinxThemesc..
-00000210: 0000 0000 0000 0000 0000 0000 0000 0100  ................
-00000220: 0000 4000 0000 730c 0000 0065 005a 0164  ..@...s....e.Z.d
-00000230: 005a 0264 0153 0029 02da 1853 7068 696e  .Z.d.S.)...Sphin
-00000240: 7854 6865 6d65 4e6f 7446 6f75 6e64 4572  xThemeNotFoundEr
-00000250: 726f 724e a903 da08 5f5f 6e61 6d65 5f5f  rorN....__name__
-00000260: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000270: 7175 616c 6e61 6d65 5f5f a900 7214 0000  qualname__..r...
-00000280: 0072 1400 0000 fa58 2f68 6f6d 652f 6368  .r.....X/home/ch
-00000290: 7269 732f 776f 726b 2f50 726f 6a65 6374  ris/work/Project
-000002a0: 732f 6769 7468 7562 2f66 6c61 6d69 6e67  s/github/flaming
-000002b0: 6f2f 666c 616d 696e 676f 2f70 6c75 6769  o/flamingo/plugi
-000002c0: 6e73 2f73 7068 696e 785f 7468 656d 6573  ns/sphinx_themes
-000002d0: 2f73 7068 696e 785f 7468 656d 652e 7079  /sphinx_theme.py
-000002e0: 720f 0000 0015 0000 0073 0200 0000 0801  r........s......
-000002f0: 720f 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00000300: 0000 0000 0000 0100 0000 4000 0000 730c  ..........@...s.
-00000310: 0000 0065 005a 0164 005a 0264 0153 0029  ...e.Z.d.Z.d.S.)
-00000320: 02da 1a53 7068 696e 7843 6f6e 6669 6752  ...SphinxConfigR
-00000330: 6563 7572 7369 6f6e 4572 726f 724e 7210  ecursionErrorNr.
-00000340: 0000 0072 1400 0000 7214 0000 0072 1400  ...r....r....r..
-00000350: 0000 7215 0000 0072 1600 0000 1900 0000  ..r....r........
-00000360: 7302 0000 0008 0172 1600 0000 6300 0000  s......r....c...
-00000370: 0000 0000 0000 0000 0000 0000 0002 0000  ................
-00000380: 0040 0000 0073 1c00 0000 6500 5a01 6400  .@...s....e.Z.d.
-00000390: 5a02 6401 6402 8400 5a03 6403 6404 8400  Z.d.d...Z.d.d...
-000003a0: 5a04 6405 5300 2906 da09 5370 6869 6e78  Z.d.S.)...Sphinx
-000003b0: 4170 7063 0100 0000 0000 0000 0000 0000  Appc............
-000003c0: 0300 0000 0600 0000 4300 0000 733c 0000  ........C...s<..
-000003d0: 0074 0083 007c 005f 017c 00a0 02a1 007d  .t...|._.|.....}
-000003e0: 017c 01a0 03a1 0044 005d 167d 027c 006a  .|.....D.].}.|.j
-000003f0: 01a0 047c 027c 017c 0219 00a1 0201 0071  ...|.|.|.......q
-00000400: 1874 0583 007c 005f 0664 0053 00a9 014e  .t...|._.d.S...N
-00000410: 2907 720c 0000 00da 0872 6567 6973 7472  ).r......registr
-00000420: 79da 0f64 6973 636f 7665 725f 7468 656d  y..discover_them
-00000430: 6573 da04 6b65 7973 da0e 6164 645f 6874  es..keys..add_ht
-00000440: 6d6c 5f74 6865 6d65 720d 0000 00da 0663  ml_themer......c
-00000450: 6f6e 6669 6729 03da 0473 656c 6672 0e00  onfig)...selfr..
-00000460: 0000 da0a 7468 656d 655f 6e61 6d65 7214  ....theme_namer.
-00000470: 0000 0072 1400 0000 7215 0000 00da 085f  ...r....r......_
-00000480: 5f69 6e69 745f 5f1e 0000 0073 0a00 0000  _init__....s....
-00000490: 0001 0801 0801 0c01 1401 7a12 5370 6869  ..........z.Sphi
-000004a0: 6e78 4170 702e 5f5f 696e 6974 5f5f 6301  nxApp.__init__c.
-000004b0: 0000 0000 0000 0000 0000 0006 0000 0007  ................
-000004c0: 0000 0043 0000 0073 8e00 0000 6900 7d01  ...C...s....i.}.
-000004d0: 7400 a001 6401 a101 0100 7402 a003 7404  t...d.....t...t.
-000004e0: a101 4400 5d28 7d02 7402 6a05 a006 7404  ..D.](}.t.j...t.
-000004f0: 7c02 a102 7d03 7402 6a05 a007 7c03 a101  |...}.t.j...|...
-00000500: 7338 7118 7c03 7c01 7c02 3c00 7118 7408  s8q.|.|.|.<.q.t.
-00000510: 6402 8301 4400 5d28 7d04 7c04 6a09 7d02  d...D.](}.|.j.}.
-00000520: 7c04 a00a a100 7d05 7402 6a05 a00b 7c05  |.....}.t.j...|.
-00000530: 6a0c a101 7d03 7c03 7c01 7c02 3c00 714a  j...}.|.|.|.<.qJ
-00000540: 7400 a001 6403 6404 a006 7c01 a00d a100  t...d.d...|.....
-00000550: a101 a102 0100 7c01 5300 2905 4e7a 1964  ......|.S.).Nz.d
-00000560: 6973 636f 7665 7269 6e67 2073 7068 696e  iscovering sphin
-00000570: 7820 7468 656d 6573 7a12 7370 6869 6e78  x themesz.sphinx
-00000580: 2e68 746d 6c5f 7468 656d 6573 7a1c 6469  .html_themesz.di
-00000590: 7363 6f76 6572 6564 2073 7068 696e 7820  scovered sphinx 
-000005a0: 7468 656d 6573 3a20 2573 fa02 2c20 290e  themes: %s.., ).
-000005b0: da06 6c6f 6767 6572 da05 6465 6275 67da  ..logger..debug.
-000005c0: 026f 73da 076c 6973 7464 6972 da11 5350  .os..listdir..SP
-000005d0: 4849 4e58 5f54 4845 4d45 5f52 4f4f 54da  HINX_THEME_ROOT.
-000005e0: 0470 6174 68da 046a 6f69 6eda 0569 7364  .path..join..isd
-000005f0: 6972 7202 0000 00da 046e 616d 65da 046c  irr......name..l
-00000600: 6f61 64da 0764 6972 6e61 6d65 da08 5f5f  oad..dirname..__
-00000610: 6669 6c65 5f5f 721b 0000 0029 0672 1e00  file__r....).r..
-00000620: 0000 720e 0000 0072 2a00 0000 da0a 7468  ..r....r*.....th
-00000630: 656d 655f 7061 7468 da0b 656e 7472 795f  eme_path..entry_
-00000640: 706f 696e 74da 066d 6f64 756c 6572 1400  point..moduler..
-00000650: 0000 7214 0000 0072 1500 0000 721a 0000  ..r....r....r...
-00000660: 0025 0000 0073 1c00 0000 0001 0402 0a03  .%...s..........
-00000670: 0e01 0e02 0c01 0202 0a03 0c01 0601 0801  ................
-00000680: 0e02 0a02 1602 7a19 5370 6869 6e78 4170  ......z.SphinxAp
-00000690: 702e 6469 7363 6f76 6572 5f74 6865 6d65  p.discover_theme
-000006a0: 734e 2905 7211 0000 0072 1200 0000 7213  sN).r....r....r.
-000006b0: 0000 0072 2000 0000 721a 0000 0072 1400  ...r ...r....r..
-000006c0: 0000 7214 0000 0072 1400 0000 7215 0000  ..r....r....r...
-000006d0: 0072 1700 0000 1d00 0000 7304 0000 0008  .r........s.....
-000006e0: 0108 0772 1700 0000 6300 0000 0000 0000  ...r....c.......
-000006f0: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00000700: 0073 4000 0000 6500 5a01 6400 5a02 6900  .s@...e.Z.d.Z.i.
-00000710: 6601 6401 6402 8401 5a03 6403 6404 8400  f.d.d...Z.d.d...
-00000720: 5a04 6405 6406 8400 5a05 6407 6408 8400  Z.d.d...Z.d.d...
-00000730: 5a06 6409 640a 8400 5a07 640b 640c 8400  Z.d.d...Z.d.d...
-00000740: 5a08 640d 5300 290e da11 5370 6869 6e78  Z.d.S.)...Sphinx
-00000750: 5468 656d 6543 6f6e 6669 6763 0400 0000  ThemeConfigc....
-00000760: 0000 0000 0000 0000 0600 0000 0500 0000  ................
-00000770: 4300 0000 7362 0000 0074 00a0 0164 017c  C...sb...t...d.|
-00000780: 01a1 0201 007c 017c 005f 027c 037c 005f  .....|.|._.|.|._
-00000790: 037c 027c 005f 047c 00a0 05a1 007c 005f  .|.|._.|.....|._
-000007a0: 0674 0783 007c 005f 087c 006a 0644 005d  .t...|._.|.j.D.]
-000007b0: 267d 047c 00a0 097c 04a1 017d 0574 00a0  &}.|...|...}.t..
-000007c0: 0164 027c 05a1 0201 007c 006a 08a0 0a7c  .d.|.....|.j...|
-000007d0: 05a1 0101 0071 3664 0053 0029 034e 7a27  .....q6d.S.).Nz'
-000007e0: 7365 7474 696e 6720 7570 2073 7068 696e  setting up sphin
-000007f0: 7820 7468 656d 6520 636f 6e66 6967 2066  x theme config f
-00000800: 6f72 2027 2573 277a 0a72 6561 6469 6e67  or '%s'z.reading
-00000810: 2025 7329 0b72 2200 0000 7223 0000 0072   %s).r"...r#...r
-00000820: 1f00 0000 da10 6f70 7469 6f6e 5f6f 7665  ......option_ove
-00000830: 7272 6964 6573 da03 6170 70da 0e5f 6765  rrides..app.._ge
-00000840: 6e5f 6869 6572 6172 6368 79da 0968 6965  n_hierarchy..hie
-00000850: 7261 7263 6879 7203 0000 0072 1d00 0000  rarchyr....r....
-00000860: da16 5f67 656e 5f74 6865 6d65 5f63 6f6e  .._gen_theme_con
-00000870: 6669 675f 7061 7468 da04 7265 6164 2906  fig_path..read).
-00000880: 721e 0000 0072 1f00 0000 7233 0000 0072  r....r....r3...r
-00000890: 3200 0000 722a 0000 00da 0b63 6f6e 6669  2...r*.....confi
-000008a0: 675f 7061 7468 7214 0000 0072 1400 0000  g_pathr....r....
-000008b0: 7215 0000 0072 2000 0000 4100 0000 7314  r....r ...A...s.
-000008c0: 0000 0000 010c 0206 0106 0106 020a 0108  ................
-000008d0: 020a 010a 020c 027a 1a53 7068 696e 7854  .......z.SphinxT
-000008e0: 6865 6d65 436f 6e66 6967 2e5f 5f69 6e69  hemeConfig.__ini
-000008f0: 745f 5f63 0200 0000 0000 0000 0000 0000  t__c............
-00000900: 0200 0000 0400 0000 4300 0000 7318 0000  ........C...s...
-00000910: 0074 006a 01a0 027c 006a 036a 046a 057c  .t.j...|.j.j.j.|
-00000920: 0119 0064 01a1 0253 0029 024e fa0a 7468  ...d...S.).N..th
-00000930: 656d 652e 636f 6e66 2906 7224 0000 0072  eme.conf).r$...r
-00000940: 2700 0000 7228 0000 0072 3300 0000 7219  '...r(...r3...r.
-00000950: 0000 00da 0b68 746d 6c5f 7468 656d 6573  .....html_themes
-00000960: 2902 721e 0000 0072 2a00 0000 7214 0000  ).r....r*...r...
-00000970: 0072 1400 0000 7215 0000 0072 3600 0000  .r....r....r6...
-00000980: 5200 0000 7302 0000 0000 017a 2853 7068  R...s......z(Sph
-00000990: 696e 7854 6865 6d65 436f 6e66 6967 2e5f  inxThemeConfig._
-000009a0: 6765 6e5f 7468 656d 655f 636f 6e66 6967  gen_theme_config
-000009b0: 5f70 6174 6863 0100 0000 0000 0000 0000  _pathc..........
-000009c0: 0000 0500 0000 0500 0000 4300 0000 736e  ..........C...sn
-000009d0: 0000 007c 006a 0067 017d 017c 006a 007d  ...|.j.g.}.|.j.}
-000009e0: 027c 00a0 017c 02a1 017d 0374 0283 007d  .|...|...}.t...}
-000009f0: 047c 04a0 037c 03a1 0101 007c 04a0 0464  .|...|.....|...d
-00000a00: 0164 02a1 027d 027c 0264 036b 0272 407c  .d...}.|.d.k.r@|
-00000a10: 0153 007c 027c 0176 0072 5c74 0564 04a0  .S.|.|.v.r\t.d..
-00000a20: 067c 017c 0267 0117 00a1 0183 0182 017c  .|.|.g.........|
-00000a30: 01a0 0764 057c 02a1 0201 0071 0e64 0053  ...d.|.....q.d.S
-00000a40: 0029 064e da05 7468 656d 65da 0769 6e68  .).N..theme..inh
-00000a50: 6572 6974 da04 6e6f 6e65 7a04 202d 3e20  erit..nonez. -> 
-00000a60: 7201 0000 0029 0872 1f00 0000 7236 0000  r....).r....r6..
-00000a70: 0072 0300 0000 7237 0000 00da 0367 6574  .r....r7.....get
-00000a80: 7216 0000 0072 2800 0000 da06 696e 7365  r....r(.....inse
-00000a90: 7274 2905 721e 0000 0072 3500 0000 723c  rt).r....r5...r<
-00000aa0: 0000 0072 3800 0000 721d 0000 0072 1400  ...r8...r....r..
-00000ab0: 0000 7214 0000 0072 1500 0000 7234 0000  ..r....r....r4..
-00000ac0: 0055 0000 0073 1a00 0000 0001 0801 0603  .U...s..........
-00000ad0: 0a01 0602 0a02 0c02 0801 0402 0801 0201  ................
-00000ae0: 0eff 0403 7a20 5370 6869 6e78 5468 656d  ....z SphinxThem
-00000af0: 6543 6f6e 6669 672e 5f67 656e 5f68 6965  eConfig._gen_hie
-00000b00: 7261 7263 6879 6301 0000 0000 0000 0000  rarchyc.........
-00000b10: 0000 0001 0000 0006 0000 0043 0000 0073  ...........C...s
-00000b20: 2e00 0000 7c00 6a00 a001 6401 6402 a102  ....|.j...d.d...
-00000b30: 6403 6404 8400 7c00 6a00 a001 6401 6405  d.d...|.j...d.d.
-00000b40: a102 a002 6406 a101 4400 8301 6407 9c02  ....d...D...d...
-00000b50: 5300 2908 4e72 3b00 0000 da0a 7374 796c  S.).Nr;.....styl
-00000b60: 6573 6865 6574 6301 0000 0000 0000 0000  esheetc.........
-00000b70: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
-00000b80: 1400 0000 6700 7c00 5d0c 7d01 7c01 a000  ....g.|.].}.|...
-00000b90: a100 9102 7104 5300 7214 0000 0029 01da  ....q.S.r....)..
-00000ba0: 0573 7472 6970 a902 da02 2e30 da01 6972  .strip.....0..ir
-00000bb0: 1400 0000 7214 0000 0072 1500 0000 da0a  ....r....r......
-00000bc0: 3c6c 6973 7463 6f6d 703e 6e00 0000 7304  <listcomp>n...s.
-00000bd0: 0000 0006 0202 ff7a 3653 7068 696e 7854  .......z6SphinxT
-00000be0: 6865 6d65 436f 6e66 6967 2e67 6574 5f74  hemeConfig.get_t
-00000bf0: 6865 6d65 5f63 6f6e 6669 672e 3c6c 6f63  heme_config.<loc
-00000c00: 616c 733e 2e3c 6c69 7374 636f 6d70 3eda  als>.<listcomp>.
-00000c10: 0873 6964 6562 6172 73fa 012c 2902 7240  .sidebars..,).r@
-00000c20: 0000 0072 4600 0000 2903 721d 0000 0072  ...rF...).r....r
-00000c30: 3e00 0000 da05 7370 6c69 74a9 0172 1e00  >.....split..r..
-00000c40: 0000 7214 0000 0072 1400 0000 7215 0000  ..r....r....r...
-00000c50: 00da 1067 6574 5f74 6865 6d65 5f63 6f6e  ...get_theme_con
-00000c60: 6669 676a 0000 0073 0a00 0000 0002 0c02  figj...s........
-00000c70: 0602 12fe 04fd 7a22 5370 6869 6e78 5468  ......z"SphinxTh
-00000c80: 656d 6543 6f6e 6669 672e 6765 745f 7468  emeConfig.get_th
-00000c90: 656d 655f 636f 6e66 6967 6301 0000 0000  eme_configc.....
-00000ca0: 0000 0000 0000 0003 0000 0005 0000 0043  ...............C
-00000cb0: 0000 0073 3800 0000 6900 7d01 7c00 6a00  ...s8...i.}.|.j.
-00000cc0: a001 6401 a101 4400 5d16 7d02 7c00 6a00  ..d...D.].}.|.j.
-00000cd0: a002 6401 7c02 a102 7c01 7c02 3c00 7110  ..d.|...|.|.<.q.
-00000ce0: 7c01 a003 7c00 6a04 a101 0100 7c01 5300  |...|.j.....|.S.
-00000cf0: 2902 4eda 076f 7074 696f 6e73 2905 721d  ).N..options).r.
-00000d00: 0000 0072 4b00 0000 723e 0000 00da 0675  ...rK...r>.....u
-00000d10: 7064 6174 6572 3200 0000 2903 721e 0000  pdater2...).r...
-00000d20: 00da 0b72 6177 5f6f 7074 696f 6e73 da0b  ...raw_options..
-00000d30: 6f70 7469 6f6e 5f6e 616d 6572 1400 0000  option_namer....
-00000d40: 7214 0000 0072 1500 0000 da15 6765 745f  r....r......get_
-00000d50: 7261 775f 7468 656d 655f 6f70 7469 6f6e  raw_theme_option
-00000d60: 7374 0000 0073 0a00 0000 0001 0402 1001  st...s..........
-00000d70: 1402 0c02 7a27 5370 6869 6e78 5468 656d  ....z'SphinxThem
-00000d80: 6543 6f6e 6669 672e 6765 745f 7261 775f  eConfig.get_raw_
-00000d90: 7468 656d 655f 6f70 7469 6f6e 7363 0100  theme_optionsc..
-00000da0: 0000 0000 0000 0000 0000 0600 0000 0400  ................
-00000db0: 0000 4300 0000 7334 0000 007c 00a0 00a1  ..C...s4...|....
-00000dc0: 007d 0169 007d 027c 01a0 01a1 0044 005d  .}.i.}.|.....D.]
-00000dd0: 1a5c 027d 037d 0464 01a0 027c 03a1 017d  .\.}.}.d...|...}
-00000de0: 057c 047c 027c 053c 0071 147c 0253 0029  .|.|.|.<.q.|.S.)
-00000df0: 024e 7a08 7468 656d 655f 7b7d 2903 724f  .Nz.theme_{}).rO
-00000e00: 0000 00da 0569 7465 6d73 da06 666f 726d  .....items..form
-00000e10: 6174 2906 721e 0000 0072 4d00 0000 724b  at).r....rM...rK
-00000e20: 0000 005a 0f72 6177 5f6f 7074 696f 6e5f  ...Z.raw_option_
-00000e30: 6e61 6d65 da05 7661 6c75 6572 4e00 0000  name..valuerN...
-00000e40: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
-00000e50: 1167 6574 5f74 6865 6d65 5f6f 7074 696f  .get_theme_optio
-00000e60: 6e73 7e00 0000 730c 0000 0000 0108 0104  ns~...s.........
-00000e70: 0210 010a 010a 027a 2353 7068 696e 7854  .......z#SphinxT
-00000e80: 6865 6d65 436f 6e66 6967 2e67 6574 5f74  hemeConfig.get_t
-00000e90: 6865 6d65 5f6f 7074 696f 6e73 4e29 0972  heme_optionsN).r
-00000ea0: 1100 0000 7212 0000 0072 1300 0000 7220  ....r....r....r 
-00000eb0: 0000 0072 3600 0000 7234 0000 0072 4a00  ...r6...r4...rJ.
-00000ec0: 0000 724f 0000 0072 5300 0000 7214 0000  ..rO...rS...r...
-00000ed0: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
-00000ee0: 7231 0000 0040 0000 0073 0c00 0000 0801  r1...@...s......
-00000ef0: 0c11 0803 0815 080a 080a 7231 0000 0063  ..........r1...c
-00000f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000f10: 0300 0000 4000 0000 7342 0000 0065 005a  ....@...sB...e.Z
-00000f20: 0164 005a 0264 0169 0066 0264 0264 0384  .d.Z.d.i.f.d.d..
-00000f30: 015a 0364 0464 0584 005a 0464 0664 0784  .Z.d.d...Z.d.d..
-00000f40: 005a 0564 0864 0984 005a 0664 0a64 0b84  .Z.d.d...Z.d.d..
-00000f50: 005a 0764 0c64 0d84 005a 0864 0e53 0029  .Z.d.d...Z.d.S.)
-00000f60: 0fda 0b53 7068 696e 7854 6865 6d65 5463  ...SphinxThemeTc
-00000f70: 0500 0000 0000 0000 0000 0000 0500 0000  ................
-00000f80: 0900 0000 4300 0000 7398 0000 007c 017c  ....C...s....|.|
-00000f90: 005f 007c 027c 005f 0174 0283 007c 005f  ._.|.|._.t...|._
-00000fa0: 037c 017c 006a 036a 046a 0576 0172 4c74  .|.|.j.j.j.v.rLt
-00000fb0: 0664 01a0 077c 0164 02a0 0864 0364 0484  .d...|.d...d.d..
-00000fc0: 007c 006a 036a 046a 05a0 09a1 0044 0083  .|.j.j.j.....D..
-00000fd0: 01a1 01a1 0283 0182 0174 0a7c 017c 006a  .........t.|.|.j
-00000fe0: 037c 0464 058d 037c 005f 0b74 0c7c 006a  .|.d...|._.t.|.j
-00000ff0: 0364 068d 017c 005f 0d74 0e7c 017c 006a  .d...|._.t.|.|.j
-00001000: 036a 046a 057c 0119 007c 006a 0d64 078d  .j.j.|...|.j.d..
-00001010: 037c 005f 0f7c 0372 947c 00a0 10a1 0001  .|._.|.r.|......
-00001020: 0064 0053 0029 084e 7a31 7370 6869 6e78  .d.S.).Nz1sphinx
-00001030: 2074 6865 6d65 2027 7b7d 2720 6e6f 7420   theme '{}' not 
-00001040: 666f 756e 642e 2061 7661 696c 6162 6c65  found. available
-00001050: 2074 6865 6d65 733a 207b 7d72 2100 0000   themes: {}r!...
-00001060: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00001070: 0005 0000 0053 0000 0073 1600 0000 6700  .....S...s....g.
-00001080: 7c00 5d0e 7d01 6400 a000 7c01 a101 9102  |.].}.d...|.....
-00001090: 7104 5300 2901 7a04 277b 7d27 2901 7251  q.S.).z.'{}').rQ
-000010a0: 0000 0072 4200 0000 7214 0000 0072 1400  ...rB...r....r..
-000010b0: 0000 7215 0000 0072 4500 0000 9400 0000  ..r....rE.......
-000010c0: 7304 0000 0006 0102 ff7a 2853 7068 696e  s........z(Sphin
-000010d0: 7854 6865 6d65 2e5f 5f69 6e69 745f 5f2e  xTheme.__init__.
-000010e0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-000010f0: 6d70 3e29 0172 3200 0000 2901 7233 0000  mp>).r2...).r3..
-00001100: 0029 0372 2a00 0000 722e 0000 00da 0766  .).r*...r......f
-00001110: 6163 746f 7279 2911 722a 0000 00da 0962  actory).r*.....b
-00001120: 7569 6c64 5f64 6972 7217 0000 0072 3300  uild_dirr....r3.
-00001130: 0000 7219 0000 0072 3a00 0000 720f 0000  ..r....r:...r...
-00001140: 0072 5100 0000 7228 0000 0072 1b00 0000  .rQ...r(...r....
-00001150: 7231 0000 0072 1d00 0000 720a 0000 0072  r1...r....r....r
-00001160: 5500 0000 720b 0000 0072 3b00 0000 da05  U...r....r;.....
-00001170: 7365 7475 7029 0572 1e00 0000 722a 0000  setup).r....r*..
-00001180: 0072 5600 0000 7257 0000 0072 4b00 0000  .rV...rW...rK...
-00001190: 7214 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
-000011a0: 2000 0000 8a00 0000 7332 0000 0000 0106   .......s2......
-000011b0: 0106 0208 020e 0102 0104 0102 010a 010c  ................
-000011c0: ff06 fe02 ff04 0802 0102 0104 0102 fd08  ................
-000011d0: 060e 0202 0102 010c 0104 fd08 0604 017a  ...............z
-000011e0: 1453 7068 696e 7854 6865 6d65 2e5f 5f69  .SphinxTheme.__i
-000011f0: 6e69 745f 5f63 0200 0000 0000 0000 0000  nit__c..........
-00001200: 0000 0200 0000 0400 0000 4300 0000 732c  ..........C...s,
-00001210: 0000 0074 00a0 0164 017c 01a1 0201 0074  ...t...d.|.....t
-00001220: 026a 03a0 047c 01a1 0172 2274 05a0 067c  .j...|...r"t...|
-00001230: 01a1 0153 0074 02a0 077c 01a1 0153 0029  ...S.t...|...S.)
-00001240: 024e 7a09 726d 202d 7266 2025 7329 0872  .Nz.rm -rf %s).r
-00001250: 2200 0000 7223 0000 0072 2400 0000 7227  "...r#...r$...r'
-00001260: 0000 0072 2900 0000 da06 7368 7574 696c  ...r).....shutil
-00001270: da06 726d 7472 6565 da06 756e 6c69 6e6b  ..rmtree..unlink
-00001280: 2902 721e 0000 0072 2700 0000 7214 0000  ).r....r'...r...
-00001290: 0072 1400 0000 7215 0000 00da 0272 6daa  .r....r......rm.
-000012a0: 0000 0073 0800 0000 0001 0c02 0c01 0a02  ...s............
-000012b0: 7a0e 5370 6869 6e78 5468 656d 652e 726d  z.SphinxTheme.rm
-000012c0: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-000012d0: 0005 0000 0043 0000 0073 3200 0000 7400  .....C...s2...t.
-000012e0: a001 6401 7c01 7c02 a103 0100 7402 6a03  ..d.|.|.....t.j.
-000012f0: a004 7c01 a101 7226 7405 a006 7c01 7c02  ..|...r&t...|.|.
-00001300: a102 5300 7405 a007 7c01 7c02 a102 5300  ..S.t...|.|...S.
-00001310: 2902 4e7a 0b63 7020 2d72 2025 7320 2573  ).Nz.cp -r %s %s
-00001320: 2908 7222 0000 0072 2300 0000 7224 0000  ).r"...r#...r$..
-00001330: 0072 2700 0000 7229 0000 0072 5800 0000  .r'...r)...rX...
-00001340: da08 636f 7079 7472 6565 da04 636f 7079  ..copytree..copy
-00001350: 2903 721e 0000 00da 0673 6f75 7263 65da  ).r......source.
-00001360: 0b64 6573 7469 6e61 7469 6f6e 7214 0000  .destinationr...
-00001370: 0072 1400 0000 7215 0000 00da 0263 70b2  .r....r......cp.
-00001380: 0000 0073 0800 0000 0001 0e02 0c01 0c02  ...s............
-00001390: 7a0e 5370 6869 6e78 5468 656d 652e 6370  z.SphinxTheme.cp
-000013a0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000013b0: 0003 0000 0043 0000 0073 2000 0000 7c00  .....C...s ...|.
-000013c0: 6a00 7316 6900 7c00 6a01 a002 a100 a501  j.s.i.|.j.......
-000013d0: 7c00 5f00 7403 7c00 6a00 8301 5300 7218  |._.t.|.j...S.r.
-000013e0: 0000 0029 04da 235f 7374 6174 6963 5f66  ...)..#_static_f
-000013f0: 696c 655f 7465 6d70 6c61 7465 5f63 6f6e  ile_template_con
-00001400: 7465 7874 5f63 6163 6865 721d 0000 0072  text_cacher....r
-00001410: 5300 0000 7204 0000 0072 4900 0000 7214  S...r....rI...r.
-00001420: 0000 0072 1400 0000 7215 0000 00da 2067  ...r....r..... g
-00001430: 656e 5f73 7461 7469 635f 6669 6c65 5f74  en_static_file_t
-00001440: 656d 706c 6174 655f 636f 6e74 6578 74ba  emplate_context.
-00001450: 0000 0073 0a00 0000 0001 0601 0201 08ff  ...s............
-00001460: 0604 7a2c 5370 6869 6e78 5468 656d 652e  ..z,SphinxTheme.
-00001470: 6765 6e5f 7374 6174 6963 5f66 696c 655f  gen_static_file_
-00001480: 7465 6d70 6c61 7465 5f63 6f6e 7465 7874  template_context
-00001490: 6301 0000 0000 0000 0000 0000 0012 0000  c...............
-000014a0: 000b 0000 0043 0000 0073 8e02 0000 7400  .....C...s....t.
-000014b0: a001 6401 a101 0100 7402 6a03 a004 7c00  ..d.....t.j...|.
-000014c0: 6a05 6402 a102 7c00 5f06 7402 6a03 a004  j.d...|._.t.j...
-000014d0: 7c00 6a05 6403 a102 7c00 5f07 7402 a008  |.j.d...|._.t...
-000014e0: 7c00 6a06 a101 0100 7402 a008 7c00 6a07  |.j.....t...|.j.
-000014f0: a101 0100 6900 7c00 5f09 740a 740b 7c00  ....i.|._.t.t.|.
-00001500: 6a0c a00d a100 6404 6405 8d02 6406 8d01  j.....d.d...d...
-00001510: 7c00 5f0e 740f 7c00 6a0e 6a10 6407 3c00  |._.t.|.j.j.d.<.
-00001520: 7411 7c00 6a0e 6a10 6408 3c00 7412 7c00  t.|.j.j.d.<.t.|.
-00001530: 6a0e 6a10 6409 3c00 7c00 6a0c a00d a100  j.j.d.<.|.j.....
-00001540: 6400 6400 640a 8503 1900 4400 9001 5de8  d.d.d.....D...].
-00001550: 7d01 7402 6a03 a013 7c01 a101 7d02 7402  }.t.j...|...}.t.
-00001560: 6a03 a004 7c00 6a06 7c02 a102 7d03 7414  j...|.j.|...}.t.
-00001570: a015 7c01 7c03 a102 0100 7402 6a03 a004  ..|.|.....t.j...
-00001580: 7c03 6403 a102 7d04 7402 6a03 a004 7c03  |.d...}.t.j...|.
-00001590: 640b a102 7d05 7402 6a03 a016 7c04 a101  d...}.t.j...|...
-000015a0: 72fe 7c00 a017 7c04 a101 0100 7402 6a03  r.|...|.....t.j.
-000015b0: a016 7c05 a101 9001 7216 7c00 a017 7c05  ..|.....r.|...|.
-000015c0: a101 0100 7402 a018 7c01 a101 4400 5d3e  ....t...|...D.]>
-000015d0: 7d06 7c06 640c 7600 9001 7232 9001 7120  }.|.d.v...r2..q 
-000015e0: 7402 6a03 a004 7c01 7c06 a102 7d07 7402  t.j...|.|...}.t.
-000015f0: 6a03 a004 7c00 6a06 7c06 a102 7d08 7c00  j...|.j.|...}.|.
-00001600: a019 7c07 7c08 a102 0100 9001 7120 7402  ..|.|.......q t.
-00001610: 6a03 a004 7c01 6403 a102 7d09 7402 6a03  j...|.d...}.t.j.
-00001620: a016 7c09 a101 9001 737e 719e 7402 a01a  ..|.....s~q.t...
-00001630: 7c09 a101 4400 5dfe 5c03 7d0a 7d0b 7d0c  |...D.].\.}.}.}.
-00001640: 7c0c 4400 5dec 7d0d 7402 6a03 a004 7c0a  |.D.].}.t.j...|.
-00001650: 7c0d a102 7d07 7402 6a03 a004 7c00 6a07  |...}.t.j...|.j.
-00001660: 7402 6a03 a01b 7c07 7c09 a102 a102 7d08  t.j...|.|.....}.
-00001670: 7402 6a03 a01c 7c08 a101 7d0e 7402 6a03  t.j...|...}.t.j.
-00001680: a016 7c0e a101 9001 73e6 7402 a008 7c0e  ..|.....s.t...|.
-00001690: a101 0100 7c07 a01d 640d a101 9002 7302  ....|...d.....s.
-000016a0: 7c00 a019 7c07 7c08 a102 0100 9001 7196  |...|.|.......q.
-000016b0: 7400 a001 640e 7c07 7c08 a103 0100 7402  t...d.|.|.....t.
-000016c0: 6a03 a01b 7c07 7c01 a102 7d0f 7c00 6a0e  j...|.|...}.|.j.
-000016d0: a01e 7c0f a101 7d10 7c00 a01f a100 7d11  ..|...}.|.....}.
-000016e0: 7420 7c08 6400 640f 8502 1900 6410 8302  t |.d.d.....d...
-000016f0: 8f26 7d0d 7c0d a021 7c10 6a22 6600 6900  .&}.|..!|.j"f.i.
-00001700: 7c11 a401 8e01 a101 0100 5700 6400 0400  |.........W.d...
-00001710: 0400 8303 0100 6e12 3100 9002 7372 3000  ......n.1...sr0.
-00001720: 0100 0100 0100 5900 0100 9001 7196 9001  ......Y.....q...
-00001730: 7196 9001 7188 719e 6400 5300 2911 4e7a  q...q.q.d.S.).Nz
-00001740: 1973 6574 7469 6e67 2075 7020 666c 616d  .setting up flam
-00001750: 696e 676f 2074 6865 6d65 da09 7465 6d70  ingo theme..temp
-00001760: 6c61 7465 73da 0673 7461 7469 6354 2901  lates..staticT).
-00001770: da0b 666f 6c6c 6f77 6c69 6e6b 7329 01da  ..followlinks)..
-00001780: 066c 6f61 6465 72da 0674 6f62 6f6f 6cda  .loader..tobool.
-00001790: 0574 6f64 696d da05 746f 696e 74e9 ffff  .todim..toint...
-000017a0: ffff 7239 0000 0029 0272 6400 0000 7239  ..r9...).rd...r9
-000017b0: 0000 005a 025f 747a 1272 656e 6465 7269  ...Z._tz.renderi
-000017c0: 6e67 2025 7320 2d3e 2025 73e9 feff ffff  ng %s -> %s.....
-000017d0: 7a02 772b 2923 7222 0000 0072 2300 0000  z.w+)#r"...r#...
-000017e0: 7224 0000 0072 2700 0000 7228 0000 0072  r$...r'...r(...r
-000017f0: 5600 0000 da0d 7465 6d70 6c61 7465 5f72  V.....template_r
-00001800: 6f6f 745a 0b73 7461 7469 635f 726f 6f74  ootZ.static_root
-00001810: da08 6d61 6b65 6469 7273 7261 0000 0072  ..makedirsra...r
-00001820: 0500 0000 7206 0000 0072 3b00 0000 da0e  ....r....r;.....
-00001830: 6765 745f 7468 656d 655f 6469 7273 5a0a  get_theme_dirsZ.
-00001840: 6a69 6e6a 6132 5f65 6e76 7207 0000 00da  jinja2_envr.....
-00001850: 0766 696c 7465 7273 7208 0000 0072 0900  .filtersr....r..
-00001860: 0000 da08 6261 7365 6e61 6d65 7258 0000  ....basenamerX..
-00001870: 0072 5c00 0000 da06 6578 6973 7473 725b  .r\.....existsr[
-00001880: 0000 0072 2500 0000 7260 0000 00da 0477  ...r%...r`.....w
-00001890: 616c 6bda 0772 656c 7061 7468 722c 0000  alk..relpathr,..
-000018a0: 00da 0865 6e64 7377 6974 68da 0c67 6574  ...endswith..get
-000018b0: 5f74 656d 706c 6174 6572 6200 0000 da04  _templaterb.....
-000018c0: 6f70 656e da05 7772 6974 65da 0672 656e  open..write..ren
-000018d0: 6465 7229 1272 1e00 0000 5a09 7468 656d  der).r....Z.them
-000018e0: 655f 6469 7272 1f00 0000 5a0c 7468 656d  e_dirr....Z.them
-000018f0: 655f 6f75 7470 7574 5a10 7468 656d 655f  e_outputZ.theme_
-00001900: 7374 6174 6963 5f64 6972 5a0c 7468 656d  static_dirZ.them
-00001910: 655f 636f 6e66 6967 7244 0000 0072 5e00  e_configrD...r^.
-00001920: 0000 725f 0000 00da 0a73 7461 7469 635f  ..r_.....static_
-00001930: 6469 72da 0472 6f6f 74da 0464 6972 73da  dir..root..dirs.
-00001940: 0566 696c 6573 da01 665a 1364 6573 7469  .files..fZ.desti
-00001950: 6e61 7469 6f6e 5f64 6972 6e61 6d65 da0d  nation_dirname..
-00001960: 7465 6d70 6c61 7465 5f6e 616d 65da 0874  template_name..t
-00001970: 656d 706c 6174 65da 1074 656d 706c 6174  emplate..templat
-00001980: 655f 636f 6e74 6578 7472 1400 0000 7214  e_contextr....r.
-00001990: 0000 0072 1500 0000 7257 0000 00c2 0000  ...r....rW......
-000019a0: 0073 6c00 0000 0001 0a03 1201 1202 0c01  .sl.............
-000019b0: 0c03 0602 0201 0201 0801 02fe 04ff 0807  ................
-000019c0: 0c01 0c01 0c03 1a05 0c01 1002 0c03 0e01  ................
-000019d0: 0e02 0c01 0a02 0e01 0a03 0e01 0a01 0402  ................
-000019e0: 0e01 1002 1003 0e02 0e01 0202 1401 0801  ................
-000019f0: 0e02 0601 0401 0cfe 0405 0c02 0e01 0a03  ................
-00001a00: 0c01 0c02 0403 0e02 0e01 0c01 0802 1401  ................
-00001a10: 3602 7a11 5370 6869 6e78 5468 656d 652e  6.z.SphinxTheme.
-00001a20: 7365 7475 7063 0100 0000 0000 0000 0000  setupc..........
-00001a30: 0000 0100 0000 0400 0000 4300 0000 7310  ..........C...s.
-00001a40: 0000 0064 01a0 007c 006a 017c 006a 02a1  ...d...|.j.|.j..
-00001a50: 0253 0029 024e 7a17 3c53 7068 696e 7854  .S.).Nz.<SphinxT
-00001a60: 6865 6d65 2827 7b7d 272c 207b 7d29 3e29  heme('{}', {})>)
-00001a70: 0372 5100 0000 722a 0000 0072 5600 0000  .rQ...r*...rV...
-00001a80: 7249 0000 0072 1400 0000 7214 0000 0072  rI...r....r....r
-00001a90: 1500 0000 da08 5f5f 7265 7072 5f5f 1f01  ......__repr__..
-00001aa0: 0000 7302 0000 0000 017a 1453 7068 696e  ..s......z.Sphin
-00001ab0: 7854 6865 6d65 2e5f 5f72 6570 725f 5f4e  xTheme.__repr__N
-00001ac0: 2909 7211 0000 0072 1200 0000 7213 0000  ).r....r....r...
-00001ad0: 0072 2000 0000 725b 0000 0072 6000 0000  .r ...r[...r`...
-00001ae0: 7262 0000 0072 5700 0000 7281 0000 0072  rb...rW...r....r
-00001af0: 1400 0000 7214 0000 0072 1400 0000 7215  ....r....r....r.
-00001b00: 0000 0072 5400 0000 8900 0000 730c 0000  ...rT.......s...
-00001b10: 0008 010e 2008 0808 0808 0808 5d72 5400  .... .......]rT.
-00001b20: 0000 2925 da0d 706b 675f 7265 736f 7572  ..)%..pkg_resour
-00001b30: 6365 7372 0200 0000 da0c 636f 6e66 6967  cesr......config
-00001b40: 7061 7273 6572 7203 0000 0072 5d00 0000  parserr....r]...
-00001b50: 7204 0000 00da 076c 6f67 6769 6e67 7258  r......loggingrX
-00001b60: 0000 0072 2400 0000 da06 6a69 6e6a 6132  ...r$.....jinja2
-00001b70: 7205 0000 0072 0600 0000 da11 7370 6869  r....r......sphi
-00001b80: 6e78 2e6a 696e 6a61 3267 6c75 6572 0700  nx.jinja2gluer..
-00001b90: 0000 7208 0000 0072 0900 0000 da0e 7370  ..r....r......sp
-00001ba0: 6869 6e78 2e74 6865 6d69 6e67 720a 0000  hinx.themingr...
-00001bb0: 0072 0b00 0000 da0f 7370 6869 6e78 2e72  .r......sphinx.r
-00001bc0: 6567 6973 7472 7972 0c00 0000 da0d 7370  egistryr......sp
-00001bd0: 6869 6e78 2e63 6f6e 6669 6772 0d00 0000  hinx.configr....
-00001be0: da06 7370 6869 6e78 7227 0000 0072 2800  ..sphinxr'...r(.
-00001bf0: 0000 722c 0000 0072 2d00 0000 7226 0000  ..r,...r-...r&..
-00001c00: 00da 0967 6574 4c6f 6767 6572 7222 0000  ...getLoggerr"..
-00001c10: 00da 0945 7863 6570 7469 6f6e 720f 0000  ...Exceptionr...
-00001c20: 0072 1600 0000 7217 0000 0072 3100 0000  .r....r....r1...
-00001c30: 7254 0000 0072 1400 0000 7214 0000 0072  rT...r....r....r
-00001c40: 1400 0000 7215 0000 00da 083c 6d6f 6475  ....r......<modu
-00001c50: 6c65 3e01 0000 0073 2400 0000 0c01 0c01  le>....s$.......
-00001c60: 0c01 0801 0801 0802 1002 1401 1001 0c01  ................
-00001c70: 0c01 0802 1802 0a03 1004 1004 0e23 0e49  .............#.I
+00000020: 0005 0000 0040 0000 0073 0801 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
+00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
+00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
+00000060: 6401 6c07 5a07 6400 6401 6c08 5a08 6400  d.l.Z.d.d.l.Z.d.
+00000070: 6404 6c09 6d0a 5a0a 6d0b 5a0b 0100 6400  d.l.m.Z.m.Z...d.
+00000080: 6405 6c0c 6d0d 5a0d 0100 6400 6406 6c0e  d.l.m.Z...d.d.l.
+00000090: 6d0f 5a0f 0100 6400 6407 6c10 6d11 5a11  m.Z...d.d.l.m.Z.
+000000a0: 6d12 5a12 6d13 5a13 0100 6400 6408 6c14  m.Z.m.Z...d.d.l.
+000000b0: 6d15 5a15 0100 6400 6409 6c16 6d17 5a17  m.Z...d.d.l.m.Z.
+000000c0: 6d18 5a18 0100 6501 6a19 a01a 6501 6a19  m.Z...e.j...e.j.
+000000d0: a01b 6508 6a1c a101 640a a102 5a1d 6500  ..e.j...d...Z.e.
+000000e0: a01e 640b a101 5a1f 4700 640c 640d 8400  ..d...Z.G.d.d...
+000000f0: 640d 6520 8303 5a21 4700 640e 640f 8400  d.e ..Z!G.d.d...
+00000100: 640f 6520 8303 5a22 4700 6410 6411 8400  d.e ..Z"G.d.d...
+00000110: 6411 8302 5a23 4700 6412 6413 8400 6413  d...Z#G.d.d...d.
+00000120: 8302 5a24 4700 6414 6415 8400 6415 8302  ..Z$G.d.d...d...
+00000130: 5a25 6401 5300 2916 e900 0000 004e 2901  Z%d.S.)......N).
+00000140: da0f 5261 7743 6f6e 6669 6750 6172 7365  ..RawConfigParse
+00000150: 7229 01da 0864 6565 7063 6f70 7929 02da  r)...deepcopy)..
+00000160: 0b45 6e76 6972 6f6e 6d65 6e74 da10 4669  .Environment..Fi
+00000170: 6c65 5379 7374 656d 4c6f 6164 6572 2901  leSystemLoader).
+00000180: da11 6974 6572 5f65 6e74 7279 5f70 6f69  ..iter_entry_poi
+00000190: 6e74 7329 01da 0643 6f6e 6669 6729 03da  nts)...Config)..
+000001a0: 075f 746f 626f 6f6c da06 5f74 6f64 696d  ._tobool.._todim
+000001b0: da06 5f74 6f69 6e74 2901 da17 5370 6869  .._toint)...Sphi
+000001c0: 6e78 436f 6d70 6f6e 656e 7452 6567 6973  nxComponentRegis
+000001d0: 7472 7929 02da 1048 544d 4c54 6865 6d65  try)...HTMLTheme
+000001e0: 4661 6374 6f72 79da 0554 6865 6d65 da06  Factory..Theme..
+000001f0: 7468 656d 6573 7a1d 666c 616d 696e 676f  themesz.flamingo
+00000200: 2e70 6c75 6769 6e73 2e53 7068 696e 7854  .plugins.SphinxT
+00000210: 6865 6d65 7363 0000 0000 0000 0000 0000  hemesc..........
+00000220: 0000 0000 0000 0100 0000 4000 0000 730c  ..........@...s.
+00000230: 0000 0065 005a 0164 005a 0264 0153 0029  ...e.Z.d.Z.d.S.)
+00000240: 02da 1853 7068 696e 7854 6865 6d65 4e6f  ...SphinxThemeNo
+00000250: 7446 6f75 6e64 4572 726f 724e a903 da08  tFoundErrorN....
+00000260: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00000270: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00000280: 5f5f a900 7214 0000 0072 1400 0000 fa58  __..r....r.....X
+00000290: 2f68 6f6d 652f 6368 7269 732f 776f 726b  /home/chris/work
+000002a0: 2f50 726f 6a65 6374 732f 6769 7468 7562  /Projects/github
+000002b0: 2f66 6c61 6d69 6e67 6f2f 666c 616d 696e  /flamingo/flamin
+000002c0: 676f 2f70 6c75 6769 6e73 2f73 7068 696e  go/plugins/sphin
+000002d0: 785f 7468 656d 6573 2f73 7068 696e 785f  x_themes/sphinx_
+000002e0: 7468 656d 652e 7079 720f 0000 0016 0000  theme.pyr.......
+000002f0: 0073 0200 0000 0801 720f 0000 0063 0000  .s......r....c..
+00000300: 0000 0000 0000 0000 0000 0000 0000 0100  ................
+00000310: 0000 4000 0000 730c 0000 0065 005a 0164  ..@...s....e.Z.d
+00000320: 005a 0264 0153 0029 02da 1a53 7068 696e  .Z.d.S.)...Sphin
+00000330: 7843 6f6e 6669 6752 6563 7572 7369 6f6e  xConfigRecursion
+00000340: 4572 726f 724e 7210 0000 0072 1400 0000  ErrorNr....r....
+00000350: 7214 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
+00000360: 1600 0000 1a00 0000 7302 0000 0008 0172  ........s......r
+00000370: 1600 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000380: 0000 0000 0002 0000 0040 0000 0073 1c00  .........@...s..
+00000390: 0000 6500 5a01 6400 5a02 6401 6402 8400  ..e.Z.d.Z.d.d...
+000003a0: 5a03 6403 6404 8400 5a04 6405 5300 2906  Z.d.d...Z.d.S.).
+000003b0: da09 5370 6869 6e78 4170 7063 0100 0000  ..SphinxAppc....
+000003c0: 0000 0000 0000 0000 0300 0000 0600 0000  ................
+000003d0: 4300 0000 733c 0000 0074 0083 007c 005f  C...s<...t...|._
+000003e0: 017c 00a0 02a1 007d 017c 01a0 03a1 0044  .|.....}.|.....D
+000003f0: 005d 167d 027c 006a 01a0 047c 027c 017c  .].}.|.j...|.|.|
+00000400: 0219 00a1 0201 0071 1874 0583 007c 005f  .......q.t...|._
+00000410: 0664 0053 0029 014e 2907 720b 0000 00da  .d.S.).N).r.....
+00000420: 0872 6567 6973 7472 79da 0f64 6973 636f  .registry..disco
+00000430: 7665 725f 7468 656d 6573 da04 6b65 7973  ver_themes..keys
+00000440: da0e 6164 645f 6874 6d6c 5f74 6865 6d65  ..add_html_theme
+00000450: 7207 0000 00da 0663 6f6e 6669 6729 03da  r......config)..
+00000460: 0473 656c 6672 0e00 0000 da0a 7468 656d  .selfr......them
+00000470: 655f 6e61 6d65 7214 0000 0072 1400 0000  e_namer....r....
+00000480: 7215 0000 00da 085f 5f69 6e69 745f 5f1f  r......__init__.
+00000490: 0000 0073 0a00 0000 0001 0801 0801 0c01  ...s............
+000004a0: 1401 7a12 5370 6869 6e78 4170 702e 5f5f  ..z.SphinxApp.__
+000004b0: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
+000004c0: 0000 0006 0000 0007 0000 0043 0000 0073  ...........C...s
+000004d0: 8e00 0000 6900 7d01 7400 a001 6401 a101  ....i.}.t...d...
+000004e0: 0100 7402 a003 7404 a101 4400 5d28 7d02  ..t...t...D.](}.
+000004f0: 7402 6a05 a006 7404 7c02 a102 7d03 7402  t.j...t.|...}.t.
+00000500: 6a05 a007 7c03 a101 7338 7118 7c03 7c01  j...|...s8q.|.|.
+00000510: 7c02 3c00 7118 7408 6402 8301 4400 5d28  |.<.q.t.d...D.](
+00000520: 7d04 7c04 6a09 7d02 7c04 a00a a100 7d05  }.|.j.}.|.....}.
+00000530: 7402 6a05 a00b 7c05 6a0c a101 7d03 7c03  t.j...|.j...}.|.
+00000540: 7c01 7c02 3c00 714a 7400 a001 6403 6404  |.|.<.qJt...d.d.
+00000550: a006 7c01 a00d a100 a101 a102 0100 7c01  ..|...........|.
+00000560: 5300 2905 4e7a 1964 6973 636f 7665 7269  S.).Nz.discoveri
+00000570: 6e67 2073 7068 696e 7820 7468 656d 6573  ng sphinx themes
+00000580: 7a12 7370 6869 6e78 2e68 746d 6c5f 7468  z.sphinx.html_th
+00000590: 656d 6573 7a1c 6469 7363 6f76 6572 6564  emesz.discovered
+000005a0: 2073 7068 696e 7820 7468 656d 6573 3a20   sphinx themes: 
+000005b0: 2573 fa02 2c20 290e da06 6c6f 6767 6572  %s.., )...logger
+000005c0: da05 6465 6275 67da 026f 73da 076c 6973  ..debug..os..lis
+000005d0: 7464 6972 da11 5350 4849 4e58 5f54 4845  tdir..SPHINX_THE
+000005e0: 4d45 5f52 4f4f 54da 0470 6174 68da 046a  ME_ROOT..path..j
+000005f0: 6f69 6eda 0569 7364 6972 7206 0000 00da  oin..isdirr.....
+00000600: 046e 616d 65da 046c 6f61 64da 0764 6972  .name..load..dir
+00000610: 6e61 6d65 da08 5f5f 6669 6c65 5f5f 721a  name..__file__r.
+00000620: 0000 0029 0672 1d00 0000 720e 0000 0072  ...).r....r....r
+00000630: 2900 0000 da0a 7468 656d 655f 7061 7468  ).....theme_path
+00000640: da0b 656e 7472 795f 706f 696e 74da 066d  ..entry_point..m
+00000650: 6f64 756c 6572 1400 0000 7214 0000 0072  oduler....r....r
+00000660: 1500 0000 7219 0000 0026 0000 0073 1c00  ....r....&...s..
+00000670: 0000 0001 0402 0a03 0e01 0e02 0c01 0202  ................
+00000680: 0a03 0c01 0601 0801 0e02 0a02 1602 7a19  ..............z.
+00000690: 5370 6869 6e78 4170 702e 6469 7363 6f76  SphinxApp.discov
+000006a0: 6572 5f74 6865 6d65 734e 2905 7211 0000  er_themesN).r...
+000006b0: 0072 1200 0000 7213 0000 0072 1f00 0000  .r....r....r....
+000006c0: 7219 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
+000006d0: 1400 0000 7215 0000 0072 1700 0000 1e00  ....r....r......
+000006e0: 0000 7304 0000 0008 0108 0772 1700 0000  ..s........r....
+000006f0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000700: 0003 0000 0040 0000 0073 4000 0000 6500  .....@...s@...e.
+00000710: 5a01 6400 5a02 6900 6601 6401 6402 8401  Z.d.Z.i.f.d.d...
+00000720: 5a03 6403 6404 8400 5a04 6405 6406 8400  Z.d.d...Z.d.d...
+00000730: 5a05 6407 6408 8400 5a06 6409 640a 8400  Z.d.d...Z.d.d...
+00000740: 5a07 640b 640c 8400 5a08 640d 5300 290e  Z.d.d...Z.d.S.).
+00000750: da11 5370 6869 6e78 5468 656d 6543 6f6e  ..SphinxThemeCon
+00000760: 6669 6763 0400 0000 0000 0000 0000 0000  figc............
+00000770: 0600 0000 0500 0000 4300 0000 7362 0000  ........C...sb..
+00000780: 0074 00a0 0164 017c 01a1 0201 007c 017c  .t...d.|.....|.|
+00000790: 005f 027c 037c 005f 037c 027c 005f 047c  ._.|.|._.|.|._.|
+000007a0: 00a0 05a1 007c 005f 0674 0783 007c 005f  .....|._.t...|._
+000007b0: 087c 006a 0644 005d 267d 047c 00a0 097c  .|.j.D.]&}.|...|
+000007c0: 04a1 017d 0574 00a0 0164 027c 05a1 0201  ...}.t...d.|....
+000007d0: 007c 006a 08a0 0a7c 05a1 0101 0071 3664  .|.j...|.....q6d
+000007e0: 0053 0029 034e 7a27 7365 7474 696e 6720  .S.).Nz'setting 
+000007f0: 7570 2073 7068 696e 7820 7468 656d 6520  up sphinx theme 
+00000800: 636f 6e66 6967 2066 6f72 2027 2573 277a  config for '%s'z
+00000810: 0a72 6561 6469 6e67 2025 7329 0b72 2100  .reading %s).r!.
+00000820: 0000 7222 0000 0072 1e00 0000 da10 6f70  ..r"...r......op
+00000830: 7469 6f6e 5f6f 7665 7272 6964 6573 da03  tion_overrides..
+00000840: 6170 70da 0e5f 6765 6e5f 6869 6572 6172  app.._gen_hierar
+00000850: 6368 79da 0968 6965 7261 7263 6879 7202  chy..hierarchyr.
+00000860: 0000 0072 1c00 0000 da16 5f67 656e 5f74  ...r......_gen_t
+00000870: 6865 6d65 5f63 6f6e 6669 675f 7061 7468  heme_config_path
+00000880: da04 7265 6164 2906 721d 0000 0072 1e00  ..read).r....r..
+00000890: 0000 7232 0000 0072 3100 0000 7229 0000  ..r2...r1...r)..
+000008a0: 00da 0b63 6f6e 6669 675f 7061 7468 7214  ...config_pathr.
+000008b0: 0000 0072 1400 0000 7215 0000 0072 1f00  ...r....r....r..
+000008c0: 0000 4200 0000 7314 0000 0000 010c 0206  ..B...s.........
+000008d0: 0106 0106 020a 0108 020a 010a 020c 027a  ...............z
+000008e0: 1a53 7068 696e 7854 6865 6d65 436f 6e66  .SphinxThemeConf
+000008f0: 6967 2e5f 5f69 6e69 745f 5f63 0200 0000  ig.__init__c....
+00000900: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00000910: 4300 0000 7318 0000 0074 006a 01a0 027c  C...s....t.j...|
+00000920: 006a 036a 046a 057c 0119 0064 01a1 0253  .j.j.j.|...d...S
+00000930: 0029 024e fa0a 7468 656d 652e 636f 6e66  .).N..theme.conf
+00000940: 2906 7223 0000 0072 2600 0000 7227 0000  ).r#...r&...r'..
+00000950: 0072 3200 0000 7218 0000 00da 0b68 746d  .r2...r......htm
+00000960: 6c5f 7468 656d 6573 2902 721d 0000 0072  l_themes).r....r
+00000970: 2900 0000 7214 0000 0072 1400 0000 7215  )...r....r....r.
+00000980: 0000 0072 3500 0000 5300 0000 7302 0000  ...r5...S...s...
+00000990: 0000 017a 2853 7068 696e 7854 6865 6d65  ...z(SphinxTheme
+000009a0: 436f 6e66 6967 2e5f 6765 6e5f 7468 656d  Config._gen_them
+000009b0: 655f 636f 6e66 6967 5f70 6174 6863 0100  e_config_pathc..
+000009c0: 0000 0000 0000 0000 0000 0500 0000 0500  ................
+000009d0: 0000 4300 0000 736e 0000 007c 006a 0067  ..C...sn...|.j.g
+000009e0: 017d 017c 006a 007d 027c 00a0 017c 02a1  .}.|.j.}.|...|..
+000009f0: 017d 0374 0283 007d 047c 04a0 037c 03a1  .}.t...}.|...|..
+00000a00: 0101 007c 04a0 0464 0164 02a1 027d 027c  ...|...d.d...}.|
+00000a10: 0264 036b 0272 407c 0153 007c 027c 0176  .d.k.r@|.S.|.|.v
+00000a20: 0072 5c74 0564 04a0 067c 017c 0267 0117  .r\t.d...|.|.g..
+00000a30: 00a1 0183 0182 017c 01a0 0764 057c 02a1  .......|...d.|..
+00000a40: 0201 0071 0e64 0053 0029 064e da05 7468  ...q.d.S.).N..th
+00000a50: 656d 65da 0769 6e68 6572 6974 da04 6e6f  eme..inherit..no
+00000a60: 6e65 7a04 202d 3e20 7201 0000 0029 0872  nez. -> r....).r
+00000a70: 1e00 0000 7235 0000 0072 0200 0000 7236  ....r5...r....r6
+00000a80: 0000 00da 0367 6574 7216 0000 0072 2700  .....getr....r'.
+00000a90: 0000 da06 696e 7365 7274 2905 721d 0000  ....insert).r...
+00000aa0: 0072 3400 0000 723b 0000 0072 3700 0000  .r4...r;...r7...
+00000ab0: 721c 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
+00000ac0: 1500 0000 7233 0000 0056 0000 0073 1a00  ....r3...V...s..
+00000ad0: 0000 0001 0801 0603 0a01 0602 0a02 0c02  ................
+00000ae0: 0801 0402 0801 0201 0eff 0403 7a20 5370  ............z Sp
+00000af0: 6869 6e78 5468 656d 6543 6f6e 6669 672e  hinxThemeConfig.
+00000b00: 5f67 656e 5f68 6965 7261 7263 6879 6301  _gen_hierarchyc.
+00000b10: 0000 0000 0000 0000 0000 0001 0000 0006  ................
+00000b20: 0000 0043 0000 0073 2e00 0000 7c00 6a00  ...C...s....|.j.
+00000b30: a001 6401 6402 a102 6403 6404 8400 7c00  ..d.d...d.d...|.
+00000b40: 6a00 a001 6401 6405 a102 a002 6406 a101  j...d.d.....d...
+00000b50: 4400 8301 6407 9c02 5300 2908 4e72 3a00  D...d...S.).Nr:.
+00000b60: 0000 da0a 7374 796c 6573 6865 6574 6301  ....stylesheetc.
+00000b70: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00000b80: 0000 0053 0000 0073 1400 0000 6700 7c00  ...S...s....g.|.
+00000b90: 5d0c 7d01 7c01 a000 a100 9102 7104 5300  ].}.|.......q.S.
+00000ba0: 7214 0000 0029 01da 0573 7472 6970 a902  r....)...strip..
+00000bb0: da02 2e30 da01 6972 1400 0000 7214 0000  ...0..ir....r...
+00000bc0: 0072 1500 0000 da0a 3c6c 6973 7463 6f6d  .r......<listcom
+00000bd0: 703e 6f00 0000 7304 0000 0006 0202 ff7a  p>o...s........z
+00000be0: 3653 7068 696e 7854 6865 6d65 436f 6e66  6SphinxThemeConf
+00000bf0: 6967 2e67 6574 5f74 6865 6d65 5f63 6f6e  ig.get_theme_con
+00000c00: 6669 672e 3c6c 6f63 616c 733e 2e3c 6c69  fig.<locals>.<li
+00000c10: 7374 636f 6d70 3eda 0873 6964 6562 6172  stcomp>..sidebar
+00000c20: 73fa 012c 2902 723f 0000 0072 4500 0000  s..,).r?...rE...
+00000c30: 2903 721c 0000 0072 3d00 0000 da05 7370  ).r....r=.....sp
+00000c40: 6c69 74a9 0172 1d00 0000 7214 0000 0072  lit..r....r....r
+00000c50: 1400 0000 7215 0000 00da 1067 6574 5f74  ....r......get_t
+00000c60: 6865 6d65 5f63 6f6e 6669 676b 0000 0073  heme_configk...s
+00000c70: 0a00 0000 0002 0c02 0602 12fe 04fd 7a22  ..............z"
+00000c80: 5370 6869 6e78 5468 656d 6543 6f6e 6669  SphinxThemeConfi
+00000c90: 672e 6765 745f 7468 656d 655f 636f 6e66  g.get_theme_conf
+00000ca0: 6967 6301 0000 0000 0000 0000 0000 0003  igc.............
+00000cb0: 0000 0005 0000 0043 0000 0073 3800 0000  .......C...s8...
+00000cc0: 6900 7d01 7c00 6a00 a001 6401 a101 4400  i.}.|.j...d...D.
+00000cd0: 5d16 7d02 7c00 6a00 a002 6401 7c02 a102  ].}.|.j...d.|...
+00000ce0: 7c01 7c02 3c00 7110 7c01 a003 7c00 6a04  |.|.<.q.|...|.j.
+00000cf0: a101 0100 7c01 5300 2902 4eda 076f 7074  ....|.S.).N..opt
+00000d00: 696f 6e73 2905 721c 0000 0072 4a00 0000  ions).r....rJ...
+00000d10: 723d 0000 00da 0675 7064 6174 6572 3100  r=.....updater1.
+00000d20: 0000 2903 721d 0000 00da 0b72 6177 5f6f  ..).r......raw_o
+00000d30: 7074 696f 6e73 da0b 6f70 7469 6f6e 5f6e  ptions..option_n
+00000d40: 616d 6572 1400 0000 7214 0000 0072 1500  amer....r....r..
+00000d50: 0000 da15 6765 745f 7261 775f 7468 656d  ....get_raw_them
+00000d60: 655f 6f70 7469 6f6e 7375 0000 0073 0a00  e_optionsu...s..
+00000d70: 0000 0001 0402 1001 1402 0c02 7a27 5370  ............z'Sp
+00000d80: 6869 6e78 5468 656d 6543 6f6e 6669 672e  hinxThemeConfig.
+00000d90: 6765 745f 7261 775f 7468 656d 655f 6f70  get_raw_theme_op
+00000da0: 7469 6f6e 7363 0100 0000 0000 0000 0000  tionsc..........
+00000db0: 0000 0600 0000 0400 0000 4300 0000 7334  ..........C...s4
+00000dc0: 0000 007c 00a0 00a1 007d 0169 007d 027c  ...|.....}.i.}.|
+00000dd0: 01a0 01a1 0044 005d 1a5c 027d 037d 0464  .....D.].\.}.}.d
+00000de0: 01a0 027c 03a1 017d 057c 047c 027c 053c  ...|...}.|.|.|.<
+00000df0: 0071 147c 0253 0029 024e 7a08 7468 656d  .q.|.S.).Nz.them
+00000e00: 655f 7b7d 2903 724e 0000 00da 0569 7465  e_{}).rN.....ite
+00000e10: 6d73 da06 666f 726d 6174 2906 721d 0000  ms..format).r...
+00000e20: 0072 4c00 0000 724a 0000 005a 0f72 6177  .rL...rJ...Z.raw
+00000e30: 5f6f 7074 696f 6e5f 6e61 6d65 da05 7661  _option_name..va
+00000e40: 6c75 6572 4d00 0000 7214 0000 0072 1400  luerM...r....r..
+00000e50: 0000 7215 0000 00da 1167 6574 5f74 6865  ..r......get_the
+00000e60: 6d65 5f6f 7074 696f 6e73 7f00 0000 730c  me_options....s.
+00000e70: 0000 0000 0108 0104 0210 010a 010a 027a  ...............z
+00000e80: 2353 7068 696e 7854 6865 6d65 436f 6e66  #SphinxThemeConf
+00000e90: 6967 2e67 6574 5f74 6865 6d65 5f6f 7074  ig.get_theme_opt
+00000ea0: 696f 6e73 4e29 0972 1100 0000 7212 0000  ionsN).r....r...
+00000eb0: 0072 1300 0000 721f 0000 0072 3500 0000  .r....r....r5...
+00000ec0: 7233 0000 0072 4900 0000 724e 0000 0072  r3...rI...rN...r
+00000ed0: 5200 0000 7214 0000 0072 1400 0000 7214  R...r....r....r.
+00000ee0: 0000 0072 1500 0000 7230 0000 0041 0000  ...r....r0...A..
+00000ef0: 0073 0c00 0000 0801 0c11 0803 0815 080a  .s..............
+00000f00: 080a 7230 0000 0063 0000 0000 0000 0000  ..r0...c........
+00000f10: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+00000f20: 7342 0000 0065 005a 0164 005a 0264 0169  sB...e.Z.d.Z.d.i
+00000f30: 0066 0264 0264 0384 015a 0364 0464 0584  .f.d.d...Z.d.d..
+00000f40: 005a 0464 0664 0784 005a 0564 0864 0984  .Z.d.d...Z.d.d..
+00000f50: 005a 0664 0a64 0b84 005a 0764 0c64 0d84  .Z.d.d...Z.d.d..
+00000f60: 005a 0864 0e53 0029 0fda 0b53 7068 696e  .Z.d.S.)...Sphin
+00000f70: 7854 6865 6d65 5463 0500 0000 0000 0000  xThemeTc........
+00000f80: 0000 0000 0500 0000 0900 0000 4300 0000  ............C...
+00000f90: 7398 0000 007c 017c 005f 007c 027c 005f  s....|.|._.|.|._
+00000fa0: 0174 0283 007c 005f 037c 017c 006a 036a  .t...|._.|.|.j.j
+00000fb0: 046a 0576 0172 4c74 0664 01a0 077c 0164  .j.v.rLt.d...|.d
+00000fc0: 02a0 0864 0364 0484 007c 006a 036a 046a  ...d.d...|.j.j.j
+00000fd0: 05a0 09a1 0044 0083 01a1 01a1 0283 0182  .....D..........
+00000fe0: 0174 0a7c 017c 006a 037c 0464 058d 037c  .t.|.|.j.|.d...|
+00000ff0: 005f 0b74 0c7c 006a 0364 068d 017c 005f  ._.t.|.j.d...|._
+00001000: 0d74 0e7c 017c 006a 036a 046a 057c 0119  .t.|.|.j.j.j.|..
+00001010: 007c 006a 0d64 078d 037c 005f 0f7c 0372  .|.j.d...|._.|.r
+00001020: 947c 00a0 10a1 0001 0064 0053 0029 084e  .|.......d.S.).N
+00001030: 7a31 7370 6869 6e78 2074 6865 6d65 2027  z1sphinx theme '
+00001040: 7b7d 2720 6e6f 7420 666f 756e 642e 2061  {}' not found. a
+00001050: 7661 696c 6162 6c65 2074 6865 6d65 733a  vailable themes:
+00001060: 207b 7d72 2000 0000 6301 0000 0000 0000   {}r ...c.......
+00001070: 0000 0000 0002 0000 0005 0000 0053 0000  .............S..
+00001080: 0073 1600 0000 6700 7c00 5d0e 7d01 6400  .s....g.|.].}.d.
+00001090: a000 7c01 a101 9102 7104 5300 2901 7a04  ..|.....q.S.).z.
+000010a0: 277b 7d27 2901 7250 0000 0072 4100 0000  '{}').rP...rA...
+000010b0: 7214 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
+000010c0: 4400 0000 9500 0000 7304 0000 0006 0102  D.......s.......
+000010d0: ff7a 2853 7068 696e 7854 6865 6d65 2e5f  .z(SphinxTheme._
+000010e0: 5f69 6e69 745f 5f2e 3c6c 6f63 616c 733e  _init__.<locals>
+000010f0: 2e3c 6c69 7374 636f 6d70 3e29 0172 3100  .<listcomp>).r1.
+00001100: 0000 2901 7232 0000 0029 0372 2900 0000  ..).r2...).r)...
+00001110: 722d 0000 00da 0766 6163 746f 7279 2911  r-.....factory).
+00001120: 7229 0000 00da 0962 7569 6c64 5f64 6972  r).....build_dir
+00001130: 7217 0000 0072 3200 0000 7218 0000 0072  r....r2...r....r
+00001140: 3900 0000 720f 0000 0072 5000 0000 7227  9...r....rP...r'
+00001150: 0000 0072 1a00 0000 7230 0000 0072 1c00  ...r....r0...r..
+00001160: 0000 720c 0000 0072 5400 0000 720d 0000  ..r....rT...r...
+00001170: 0072 3a00 0000 da05 7365 7475 7029 0572  .r:.....setup).r
+00001180: 1d00 0000 7229 0000 0072 5500 0000 7256  ....r)...rU...rV
+00001190: 0000 0072 4a00 0000 7214 0000 0072 1400  ...rJ...r....r..
+000011a0: 0000 7215 0000 0072 1f00 0000 8b00 0000  ..r....r........
+000011b0: 7332 0000 0000 0106 0106 0208 020e 0102  s2..............
+000011c0: 0104 0102 010a 010c ff06 fe02 ff04 0802  ................
+000011d0: 0102 0104 0102 fd08 060e 0202 0102 010c  ................
+000011e0: 0104 fd08 0604 017a 1453 7068 696e 7854  .......z.SphinxT
+000011f0: 6865 6d65 2e5f 5f69 6e69 745f 5f63 0200  heme.__init__c..
+00001200: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00001210: 0000 4300 0000 732c 0000 0074 00a0 0164  ..C...s,...t...d
+00001220: 017c 01a1 0201 0074 026a 03a0 047c 01a1  .|.....t.j...|..
+00001230: 0172 2274 05a0 067c 01a1 0153 0074 02a0  .r"t...|...S.t..
+00001240: 077c 01a1 0153 0029 024e 7a09 726d 202d  .|...S.).Nz.rm -
+00001250: 7266 2025 7329 0872 2100 0000 7222 0000  rf %s).r!...r"..
+00001260: 0072 2300 0000 7226 0000 0072 2800 0000  .r#...r&...r(...
+00001270: da06 7368 7574 696c da06 726d 7472 6565  ..shutil..rmtree
+00001280: da06 756e 6c69 6e6b 2902 721d 0000 0072  ..unlink).r....r
+00001290: 2600 0000 7214 0000 0072 1400 0000 7215  &...r....r....r.
+000012a0: 0000 00da 0272 6dab 0000 0073 0800 0000  .....rm....s....
+000012b0: 0001 0c02 0c01 0a02 7a0e 5370 6869 6e78  ........z.Sphinx
+000012c0: 5468 656d 652e 726d 6303 0000 0000 0000  Theme.rmc.......
+000012d0: 0000 0000 0003 0000 0005 0000 0043 0000  .............C..
+000012e0: 0073 3200 0000 7400 a001 6401 7c01 7c02  .s2...t...d.|.|.
+000012f0: a103 0100 7402 6a03 a004 7c01 a101 7226  ....t.j...|...r&
+00001300: 7405 a006 7c01 7c02 a102 5300 7405 a007  t...|.|...S.t...
+00001310: 7c01 7c02 a102 5300 2902 4e7a 0b63 7020  |.|...S.).Nz.cp 
+00001320: 2d72 2025 7320 2573 2908 7221 0000 0072  -r %s %s).r!...r
+00001330: 2200 0000 7223 0000 0072 2600 0000 7228  "...r#...r&...r(
+00001340: 0000 0072 5700 0000 da08 636f 7079 7472  ...rW.....copytr
+00001350: 6565 da04 636f 7079 2903 721d 0000 00da  ee..copy).r.....
+00001360: 0673 6f75 7263 65da 0b64 6573 7469 6e61  .source..destina
+00001370: 7469 6f6e 7214 0000 0072 1400 0000 7215  tionr....r....r.
+00001380: 0000 00da 0263 70b3 0000 0073 0800 0000  .....cp....s....
+00001390: 0001 0e02 0c01 0c02 7a0e 5370 6869 6e78  ........z.Sphinx
+000013a0: 5468 656d 652e 6370 6301 0000 0000 0000  Theme.cpc.......
+000013b0: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+000013c0: 0073 3400 0000 7c00 6a00 732a 6900 7c00  .s4...|.j.s*i.|.
+000013d0: 6a01 a002 a100 a501 7c00 5f00 7403 6a04  j.......|._.t.j.
+000013e0: 6400 6401 8502 1900 7c00 6a00 6402 3c00  d.d.....|.j.d.<.
+000013f0: 7405 7c00 6a00 8301 5300 2903 4ee9 0500  t.|.j...S.).N...
+00001400: 0000 5a15 646f 6375 7469 6c73 5f76 6572  ..Z.docutils_ver
+00001410: 7369 6f6e 5f69 6e66 6f29 06da 235f 7374  sion_info)..#_st
+00001420: 6174 6963 5f66 696c 655f 7465 6d70 6c61  atic_file_templa
+00001430: 7465 5f63 6f6e 7465 7874 5f63 6163 6865  te_context_cache
+00001440: 721c 0000 0072 5200 0000 da08 646f 6375  r....rR.....docu
+00001450: 7469 6c73 da10 5f5f 7665 7273 696f 6e5f  tils..__version_
+00001460: 696e 666f 5f5f 7203 0000 0072 4800 0000  info__r....rH...
+00001470: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
+00001480: 2067 656e 5f73 7461 7469 635f 6669 6c65   gen_static_file
+00001490: 5f74 656d 706c 6174 655f 636f 6e74 6578  _template_contex
+000014a0: 74bb 0000 0073 0c00 0000 0001 0601 0201  t....s..........
+000014b0: 08ff 0603 1402 7a2c 5370 6869 6e78 5468  ......z,SphinxTh
+000014c0: 656d 652e 6765 6e5f 7374 6174 6963 5f66  eme.gen_static_f
+000014d0: 696c 655f 7465 6d70 6c61 7465 5f63 6f6e  ile_template_con
+000014e0: 7465 7874 6301 0000 0000 0000 0000 0000  textc...........
+000014f0: 0012 0000 000b 0000 0043 0000 0073 8e02  .........C...s..
+00001500: 0000 7400 a001 6401 a101 0100 7402 6a03  ..t...d.....t.j.
+00001510: a004 7c00 6a05 6402 a102 7c00 5f06 7402  ..|.j.d...|._.t.
+00001520: 6a03 a004 7c00 6a05 6403 a102 7c00 5f07  j...|.j.d...|._.
+00001530: 7402 a008 7c00 6a06 a101 0100 7402 a008  t...|.j.....t...
+00001540: 7c00 6a07 a101 0100 6900 7c00 5f09 740a  |.j.....i.|._.t.
+00001550: 740b 7c00 6a0c a00d a100 6404 6405 8d02  t.|.j.....d.d...
+00001560: 6406 8d01 7c00 5f0e 740f 7c00 6a0e 6a10  d...|._.t.|.j.j.
+00001570: 6407 3c00 7411 7c00 6a0e 6a10 6408 3c00  d.<.t.|.j.j.d.<.
+00001580: 7412 7c00 6a0e 6a10 6409 3c00 7c00 6a0c  t.|.j.j.d.<.|.j.
+00001590: a00d a100 6400 6400 640a 8503 1900 4400  ....d.d.d.....D.
+000015a0: 9001 5de8 7d01 7402 6a03 a013 7c01 a101  ..].}.t.j...|...
+000015b0: 7d02 7402 6a03 a004 7c00 6a06 7c02 a102  }.t.j...|.j.|...
+000015c0: 7d03 7414 a015 7c01 7c03 a102 0100 7402  }.t...|.|.....t.
+000015d0: 6a03 a004 7c03 6403 a102 7d04 7402 6a03  j...|.d...}.t.j.
+000015e0: a004 7c03 640b a102 7d05 7402 6a03 a016  ..|.d...}.t.j...
+000015f0: 7c04 a101 72fe 7c00 a017 7c04 a101 0100  |...r.|...|.....
+00001600: 7402 6a03 a016 7c05 a101 9001 7216 7c00  t.j...|.....r.|.
+00001610: a017 7c05 a101 0100 7402 a018 7c01 a101  ..|.....t...|...
+00001620: 4400 5d3e 7d06 7c06 640c 7600 9001 7232  D.]>}.|.d.v...r2
+00001630: 9001 7120 7402 6a03 a004 7c01 7c06 a102  ..q t.j...|.|...
+00001640: 7d07 7402 6a03 a004 7c00 6a06 7c06 a102  }.t.j...|.j.|...
+00001650: 7d08 7c00 a019 7c07 7c08 a102 0100 9001  }.|...|.|.......
+00001660: 7120 7402 6a03 a004 7c01 6403 a102 7d09  q t.j...|.d...}.
+00001670: 7402 6a03 a016 7c09 a101 9001 737e 719e  t.j...|.....s~q.
+00001680: 7402 a01a 7c09 a101 4400 5dfe 5c03 7d0a  t...|...D.].\.}.
+00001690: 7d0b 7d0c 7c0c 4400 5dec 7d0d 7402 6a03  }.}.|.D.].}.t.j.
+000016a0: a004 7c0a 7c0d a102 7d07 7402 6a03 a004  ..|.|...}.t.j...
+000016b0: 7c00 6a07 7402 6a03 a01b 7c07 7c09 a102  |.j.t.j...|.|...
+000016c0: a102 7d08 7402 6a03 a01c 7c08 a101 7d0e  ..}.t.j...|...}.
+000016d0: 7402 6a03 a016 7c0e a101 9001 73e6 7402  t.j...|.....s.t.
+000016e0: a008 7c0e a101 0100 7c07 a01d 640d a101  ..|.....|...d...
+000016f0: 9002 7302 7c00 a019 7c07 7c08 a102 0100  ..s.|...|.|.....
+00001700: 9001 7196 7400 a001 640e 7c07 7c08 a103  ..q.t...d.|.|...
+00001710: 0100 7402 6a03 a01b 7c07 7c01 a102 7d0f  ..t.j...|.|...}.
+00001720: 7c00 6a0e a01e 7c0f a101 7d10 7c00 a01f  |.j...|...}.|...
+00001730: a100 7d11 7420 7c08 6400 640f 8502 1900  ..}.t |.d.d.....
+00001740: 6410 8302 8f26 7d0d 7c0d a021 7c10 6a22  d....&}.|..!|.j"
+00001750: 6600 6900 7c11 a401 8e01 a101 0100 5700  f.i.|.........W.
+00001760: 6400 0400 0400 8303 0100 6e12 3100 9002  d.........n.1...
+00001770: 7372 3000 0100 0100 0100 5900 0100 9001  sr0.......Y.....
+00001780: 7196 9001 7196 9001 7188 719e 6400 5300  q...q...q.q.d.S.
+00001790: 2911 4e7a 1973 6574 7469 6e67 2075 7020  ).Nz.setting up 
+000017a0: 666c 616d 696e 676f 2074 6865 6d65 da09  flamingo theme..
+000017b0: 7465 6d70 6c61 7465 73da 0673 7461 7469  templates..stati
+000017c0: 6354 2901 da0b 666f 6c6c 6f77 6c69 6e6b  cT)...followlink
+000017d0: 7329 01da 066c 6f61 6465 72da 0674 6f62  s)...loader..tob
+000017e0: 6f6f 6cda 0574 6f64 696d da05 746f 696e  ool..todim..toin
+000017f0: 74e9 ffff ffff 7238 0000 0029 0272 6600  t.....r8...).rf.
+00001800: 0000 7238 0000 005a 025f 747a 1272 656e  ..r8...Z._tz.ren
+00001810: 6465 7269 6e67 2025 7320 2d3e 2025 73e9  dering %s -> %s.
+00001820: feff ffff 7a02 772b 2923 7221 0000 0072  ....z.w+)#r!...r
+00001830: 2200 0000 7223 0000 0072 2600 0000 7227  "...r#...r&...r'
+00001840: 0000 0072 5500 0000 da0d 7465 6d70 6c61  ...rU.....templa
+00001850: 7465 5f72 6f6f 745a 0b73 7461 7469 635f  te_rootZ.static_
+00001860: 726f 6f74 da08 6d61 6b65 6469 7273 7261  root..makedirsra
+00001870: 0000 0072 0400 0000 7205 0000 0072 3a00  ...r....r....r:.
+00001880: 0000 da0e 6765 745f 7468 656d 655f 6469  ....get_theme_di
+00001890: 7273 5a0a 6a69 6e6a 6132 5f65 6e76 7208  rsZ.jinja2_envr.
+000018a0: 0000 00da 0766 696c 7465 7273 7209 0000  .....filtersr...
+000018b0: 0072 0a00 0000 da08 6261 7365 6e61 6d65  .r......basename
+000018c0: 7257 0000 0072 5b00 0000 da06 6578 6973  rW...r[.....exis
+000018d0: 7473 725a 0000 0072 2400 0000 725f 0000  tsrZ...r$...r_..
+000018e0: 00da 0477 616c 6bda 0772 656c 7061 7468  ...walk..relpath
+000018f0: 722b 0000 00da 0865 6e64 7377 6974 68da  r+.....endswith.
+00001900: 0c67 6574 5f74 656d 706c 6174 6572 6400  .get_templaterd.
+00001910: 0000 da04 6f70 656e da05 7772 6974 65da  ....open..write.
+00001920: 0672 656e 6465 7229 1272 1d00 0000 5a09  .render).r....Z.
+00001930: 7468 656d 655f 6469 7272 1e00 0000 5a0c  theme_dirr....Z.
+00001940: 7468 656d 655f 6f75 7470 7574 5a10 7468  theme_outputZ.th
+00001950: 656d 655f 7374 6174 6963 5f64 6972 5a0c  eme_static_dirZ.
+00001960: 7468 656d 655f 636f 6e66 6967 7243 0000  theme_configrC..
+00001970: 0072 5d00 0000 725e 0000 00da 0a73 7461  .r]...r^.....sta
+00001980: 7469 635f 6469 72da 0472 6f6f 74da 0464  tic_dir..root..d
+00001990: 6972 73da 0566 696c 6573 da01 665a 1364  irs..files..fZ.d
+000019a0: 6573 7469 6e61 7469 6f6e 5f64 6972 6e61  estination_dirna
+000019b0: 6d65 da0d 7465 6d70 6c61 7465 5f6e 616d  me..template_nam
+000019c0: 65da 0874 656d 706c 6174 65da 1074 656d  e..template..tem
+000019d0: 706c 6174 655f 636f 6e74 6578 7472 1400  plate_contextr..
+000019e0: 0000 7214 0000 0072 1500 0000 7256 0000  ..r....r....rV..
+000019f0: 00c4 0000 0073 6c00 0000 0001 0a03 1201  .....sl.........
+00001a00: 1202 0c01 0c03 0602 0201 0201 0801 02fe  ................
+00001a10: 04ff 0807 0c01 0c01 0c03 1a05 0c01 1002  ................
+00001a20: 0c03 0e01 0e02 0c01 0a02 0e01 0a03 0e01  ................
+00001a30: 0a01 0402 0e01 1002 1003 0e02 0e01 0202  ................
+00001a40: 1401 0801 0e02 0601 0401 0cfe 0405 0c02  ................
+00001a50: 0e01 0a03 0c01 0c02 0403 0e02 0e01 0c01  ................
+00001a60: 0802 1401 3602 7a11 5370 6869 6e78 5468  ....6.z.SphinxTh
+00001a70: 656d 652e 7365 7475 7063 0100 0000 0000  eme.setupc......
+00001a80: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
+00001a90: 0000 7310 0000 0064 01a0 007c 006a 017c  ..s....d...|.j.|
+00001aa0: 006a 02a1 0253 0029 024e 7a17 3c53 7068  .j...S.).Nz.<Sph
+00001ab0: 696e 7854 6865 6d65 2827 7b7d 272c 207b  inxTheme('{}', {
+00001ac0: 7d29 3e29 0372 5000 0000 7229 0000 0072  })>).rP...r)...r
+00001ad0: 5500 0000 7248 0000 0072 1400 0000 7214  U...rH...r....r.
+00001ae0: 0000 0072 1500 0000 da08 5f5f 7265 7072  ...r......__repr
+00001af0: 5f5f 2101 0000 7302 0000 0000 017a 1453  __!...s......z.S
+00001b00: 7068 696e 7854 6865 6d65 2e5f 5f72 6570  phinxTheme.__rep
+00001b10: 725f 5f4e 2909 7211 0000 0072 1200 0000  r__N).r....r....
+00001b20: 7213 0000 0072 1f00 0000 725a 0000 0072  r....r....rZ...r
+00001b30: 5f00 0000 7264 0000 0072 5600 0000 7283  _...rd...rV...r.
+00001b40: 0000 0072 1400 0000 7214 0000 0072 1400  ...r....r....r..
+00001b50: 0000 7215 0000 0072 5300 0000 8a00 0000  ..r....rS.......
+00001b60: 730c 0000 0008 010e 2008 0808 0808 0908  s....... .......
+00001b70: 5d72 5300 0000 2926 da07 6c6f 6767 696e  ]rS...)&..loggin
+00001b80: 6772 2300 0000 7257 0000 00da 0c63 6f6e  gr#...rW.....con
+00001b90: 6669 6770 6172 7365 7272 0200 0000 725c  figparserr....r\
+00001ba0: 0000 0072 0300 0000 7262 0000 00da 0673  ...r....rb.....s
+00001bb0: 7068 696e 78da 066a 696e 6a61 3272 0400  phinx..jinja2r..
+00001bc0: 0000 7205 0000 00da 0d70 6b67 5f72 6573  ..r......pkg_res
+00001bd0: 6f75 7263 6573 7206 0000 00da 0d73 7068  ourcesr......sph
+00001be0: 696e 782e 636f 6e66 6967 7207 0000 00da  inx.configr.....
+00001bf0: 1173 7068 696e 782e 6a69 6e6a 6132 676c  .sphinx.jinja2gl
+00001c00: 7565 7208 0000 0072 0900 0000 720a 0000  uer....r....r...
+00001c10: 00da 0f73 7068 696e 782e 7265 6769 7374  ...sphinx.regist
+00001c20: 7279 720b 0000 00da 0e73 7068 696e 782e  ryr......sphinx.
+00001c30: 7468 656d 696e 6772 0c00 0000 720d 0000  themingr....r...
+00001c40: 0072 2600 0000 7227 0000 0072 2b00 0000  .r&...r'...r+...
+00001c50: 722c 0000 0072 2500 0000 da09 6765 744c  r,...r%.....getL
+00001c60: 6f67 6765 7272 2100 0000 da09 4578 6365  oggerr!.....Exce
+00001c70: 7074 696f 6e72 0f00 0000 7216 0000 0072  ptionr....r....r
+00001c80: 1700 0000 7230 0000 0072 5300 0000 7214  ....r0...rS...r.
+00001c90: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
+00001ca0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00001cb0: 7326 0000 0008 0108 0108 010c 010c 0208  s&..............
+00001cc0: 0108 0110 010c 010c 0114 010c 0110 0318  ................
+00001cd0: 020a 0310 0410 040e 230e 49              ........#.I
```

### Comparing `flamingo-1.8/flamingo/plugins/sphinx_themes/defaults.py` & `flamingo-1.9/flamingo/plugins/sphinx_themes/defaults.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/sphinx_themes/plugin.py` & `flamingo-1.9/flamingo/plugins/sphinx_themes/plugin.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/sphinx_themes/sphinx_theme.py` & `flamingo-1.9/flamingo/plugins/sphinx_themes/sphinx_theme.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from pkg_resources import iter_entry_points
-from configparser import RawConfigParser
-from copy import deepcopy
 import logging
-import shutil
 import os
+import shutil
+from configparser import RawConfigParser
+from copy import deepcopy
 
+import docutils
+import sphinx
 from jinja2 import Environment, FileSystemLoader
-
+from pkg_resources import iter_entry_points
+from sphinx.config import Config
 from sphinx.jinja2glue import _tobool, _todim, _toint
-from sphinx.theming import HTMLThemeFactory, Theme
 from sphinx.registry import SphinxComponentRegistry
-from sphinx.config import Config
-import sphinx
+from sphinx.theming import HTMLThemeFactory, Theme
+
 
 SPHINX_THEME_ROOT = os.path.join(os.path.dirname(sphinx.__file__), 'themes')
 
 logger = logging.getLogger('flamingo.plugins.SphinxThemes')
 
 
 class SphinxThemeNotFoundError(Exception):
@@ -184,14 +185,15 @@
         return shutil.copy(source, destination)
 
     def gen_static_file_template_context(self):
         if not self._static_file_template_context_cache:
             self._static_file_template_context_cache = {
                 **self.config.get_theme_options(),
             }
+            self._static_file_template_context_cache['docutils_version_info'] = docutils.__version_info__[:5]
 
         return deepcopy(self._static_file_template_context_cache)
 
     def setup(self):
         logger.debug('setting up flamingo theme')
 
         # paths
```

### Comparing `flamingo-1.8/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/elasticlunr.js` & `flamingo-1.9/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/elasticlunr.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/elasticlunr.min.js` & `flamingo-1.9/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/elasticlunr.min.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/jquery.js` & `flamingo-1.9/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/jquery.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/mark.js` & `flamingo-1.9/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/mark.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/mark.min.js` & `flamingo-1.9/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/mark.min.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/ractive.js` & `flamingo-1.9/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/ractive.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/ractive.js.map` & `flamingo-1.9/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/ractive.js.map`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/ractive.min.js` & `flamingo-1.9/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/ractive.min.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/ractive.min.js.map` & `flamingo-1.9/flamingo/plugins/sphinx_themes/theme/static/sphinx_themes/ractive.min.js.map`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/sphinx_themes/theme/templates/sphinx_themes/search.js` & `flamingo-1.9/flamingo/plugins/sphinx_themes/theme/templates/sphinx_themes/search.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/sphinx_themes/theme/templates/sphinx_themes/toctree.html` & `flamingo-1.9/flamingo/plugins/sphinx_themes/theme/templates/sphinx_themes/toctree.html`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/tags/__pycache__/tags.cpython-310.pyc` & `flamingo-1.9/flamingo/plugins/tags/__pycache__/tags.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/tags/__pycache__/tags.cpython-35.pyc` & `flamingo-1.9/flamingo/plugins/tags/__pycache__/tags.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/tags/__pycache__/tags.cpython-37.pyc` & `flamingo-1.9/flamingo/plugins/tags/__pycache__/tags.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/tags/__pycache__/tags.cpython-39.pyc` & `flamingo-1.9/flamingo/plugins/tags/__pycache__/tags.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/tags/tags.py` & `flamingo-1.9/flamingo/plugins/tags/tags.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/thumbnails.py` & `flamingo-1.9/flamingo/plugins/thumbnails.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         if media_content['type'] != 'media/image':
             logger.debug(
                 "setup of thumbnail for %s:%s skipped: type is not 'media/image'",  # NOQA
                 content['path'], media_content['path'])
 
             return
 
-        if('thumbnail' in media_content and
+        if ('thumbnail' in media_content and
            not parse_bool(media_content['thumbnail'])):
 
             logger.debug(
                 'setup of thumbnail for %s:%s skipped: disabled by option',
                 content['path'], media_content['path'])
 
             return
```

### Comparing `flamingo-1.8/flamingo/plugins/time.py` & `flamingo-1.9/flamingo/plugins/time.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/plugins/yaml.py` & `flamingo-1.9/flamingo/plugins/yaml.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/project_templates/bootstrap4/Makefile.template` & `flamingo-1.9/flamingo/project_templates/bootstrap4/Makefile.template`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/project_templates/bootstrap4/overlay/favicon.ico` & `flamingo-1.9/flamingo/project_templates/bootstrap4/overlay/favicon.ico`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/project_templates/bootstrap4/settings.py.template` & `flamingo-1.9/flamingo/project_templates/bootstrap4/settings.py.template`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/project_templates/bootstrap4/theme/templates/base.html` & `flamingo-1.9/flamingo/project_templates/bootstrap4/theme/templates/base.html`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/project_templates/data.ini` & `flamingo-1.9/flamingo/project_templates/data.ini`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/project_templates/readthedocs/Makefile.template` & `flamingo-1.9/flamingo/project_templates/readthedocs/Makefile.template`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/project_templates/readthedocs/overlay/favicon.ico` & `flamingo-1.9/flamingo/project_templates/readthedocs/overlay/favicon.ico`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/pytest.py` & `flamingo-1.9/flamingo/pytest.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/__pycache__/build_environment.cpython-310.pyc` & `flamingo-1.9/flamingo/server/__pycache__/build_environment.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/__pycache__/build_environment.cpython-35.pyc` & `flamingo-1.9/flamingo/server/__pycache__/build_environment.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/__pycache__/build_environment.cpython-37.pyc` & `flamingo-1.9/flamingo/server/__pycache__/build_environment.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/__pycache__/build_environment.cpython-39.pyc` & `flamingo-1.9/flamingo/server/__pycache__/build_environment.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/__pycache__/exporter.cpython-310.pyc` & `flamingo-1.9/flamingo/server/__pycache__/exporter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/__pycache__/exporter.cpython-35.pyc` & `flamingo-1.9/flamingo/server/__pycache__/exporter.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/__pycache__/exporter.cpython-37.pyc` & `flamingo-1.9/flamingo/server/__pycache__/exporter.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/__pycache__/exporter.cpython-39.pyc` & `flamingo-1.9/flamingo/server/__pycache__/exporter.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Dec  6 19:14:04 2021 UTC, .py size: 10160 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 fc60 ae61 b027 0000  a........`.a.'..
+00000000: 610d 0d0a 0000 0000 9ef2 7063 b027 0000  a.........pc.'..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 9c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 0100 6400  m.Z.m.Z.m.Z...d.
 00000060: 6404 6c08 6d09 5a09 0100 6400 6405 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6400 6406 6c0d  m.Z.m.Z...d.d.l.
```

### Comparing `flamingo-1.8/flamingo/server/__pycache__/frontend_controller.cpython-310.pyc` & `flamingo-1.9/flamingo/server/__pycache__/frontend_controller.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/__pycache__/frontend_controller.cpython-35.pyc` & `flamingo-1.9/flamingo/server/__pycache__/frontend_controller.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/__pycache__/frontend_controller.cpython-37.pyc` & `flamingo-1.9/flamingo/server/__pycache__/frontend_controller.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/__pycache__/frontend_controller.cpython-39.pyc` & `flamingo-1.9/flamingo/server/__pycache__/frontend_controller.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/__pycache__/logging.cpython-310.pyc` & `flamingo-1.9/flamingo/server/__pycache__/logging.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/__pycache__/logging.cpython-35.pyc` & `flamingo-1.9/flamingo/server/__pycache__/logging.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/__pycache__/logging.cpython-37.pyc` & `flamingo-1.9/flamingo/server/__pycache__/logging.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/__pycache__/logging.cpython-39.pyc` & `flamingo-1.9/flamingo/server/__pycache__/logging.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Dec  6 19:14:04 2021 UTC, .py size: 5600 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 fc60 ae61 e015 0000  a........`.a....
+00000000: 610d 0d0a 0000 0000 9ef2 7063 e015 0000  a.........pc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c05 5a05 6400 6404 6c06  ..d.d.l.Z.d.d.l.
 00000060: 5a06 6400 6405 6c07 6d08 5a08 0100 4700  Z.d.d.l.m.Z...G.
 00000070: 6406 6407 8400 6407 6506 6a09 8303 5a0a  d.d...d.e.j...Z.
```

### Comparing `flamingo-1.8/flamingo/server/__pycache__/rpc.cpython-310.pyc` & `flamingo-1.9/flamingo/server/__pycache__/rpc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/__pycache__/rpc.cpython-35.pyc` & `flamingo-1.9/flamingo/server/__pycache__/rpc.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/__pycache__/rpc.cpython-37.pyc` & `flamingo-1.9/flamingo/server/__pycache__/rpc.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/__pycache__/rpc.cpython-39.pyc` & `flamingo-1.9/flamingo/server/__pycache__/rpc.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Dec  6 19:14:04 2021 UTC, .py size: 6730 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 fc60 ae61 4a1a 0000  a........`.aJ...
+00000000: 610d 0d0a 0000 0000 9ef2 7063 4a1a 0000  a.........pcJ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6400 6402 6c05 5a05 6400 6403 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 6d07 5a07 6d08 5a08 0100 6400 6404 6c09  m.Z.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6504 a00b 6405 a101 5a0c  m.Z...e...d...Z.
```

### Comparing `flamingo-1.8/flamingo/server/__pycache__/server.cpython-310.pyc` & `flamingo-1.9/flamingo/server/__pycache__/server.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/__pycache__/server.cpython-35.pyc` & `flamingo-1.9/flamingo/server/__pycache__/server.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/__pycache__/server.cpython-37.pyc` & `flamingo-1.9/flamingo/server/__pycache__/server.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/__pycache__/server.cpython-39.pyc` & `flamingo-1.9/flamingo/server/__pycache__/server.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Dec  6 19:14:04 2021 UTC, .py size: 17399 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 fc60 ae61 f743 0000  a........`.a.C..
+00000000: 610d 0d0a 0000 0000 9ef2 7063 f743 0000  a.........pc.C..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 7001 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 5a05 6400 6403 6c06 5a06 6400 6403 6c07  Z.d.d.l.Z.d.d.l.
 00000060: 5a07 6400 6404 6c08 6d09 5a09 6d0a 5a0a  Z.d.d.l.m.Z.m.Z.
 00000070: 0100 6400 6405 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
```

### Comparing `flamingo-1.8/flamingo/server/__pycache__/watcher.cpython-310.pyc` & `flamingo-1.9/flamingo/server/__pycache__/watcher.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/__pycache__/watcher.cpython-35.pyc` & `flamingo-1.9/flamingo/server/__pycache__/watcher.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/__pycache__/watcher.cpython-37.pyc` & `flamingo-1.9/flamingo/server/__pycache__/watcher.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/__pycache__/watcher.cpython-39.pyc` & `flamingo-1.9/flamingo/server/__pycache__/watcher.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Mar 21 08:11:37 2020 UTC, .py size: 6201 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 39cc 755e 3918 0000  a.......9.u^9...
+00000000: 610d 0d0a 0000 0000 9ef2 7063 3918 0000  a.........pc9...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c03 5a03 6400  m.Z...d.d.l.Z.d.
 00000050: 6403 6c04 5a04 4700 6404 6405 8400 6405  d.l.Z.G.d.d...d.
 00000060: 6501 8303 5a05 4700 6406 6407 8400 6407  e...Z.G.d.d...d.
 00000070: 8302 5a06 4700 6408 6409 8400 6409 6506  ..Z.G.d.d...d.e.
```

### Comparing `flamingo-1.8/flamingo/server/build_environment.py` & `flamingo-1.9/flamingo/server/build_environment.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/exporter.py` & `flamingo-1.9/flamingo/server/exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,15 +282,15 @@
 
             return Response(text='404: not found', status=404)
 
         def gen_response(path):
             content = self.resolve(path)
 
             # fallback
-            if(not content or
+            if (not content or
                isinstance(content, str) and os.path.isdir(content)):
 
                 # 404
                 if not self.directory_listing:
                     return _404()
 
                 # directory listing
```

### Comparing `flamingo-1.8/flamingo/server/frontend_controller.py` & `flamingo-1.9/flamingo/server/frontend_controller.py`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/logging.py` & `flamingo-1.9/flamingo/server/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,22 +49,22 @@
         if self.internal_level and record.levelno < self.internal_level:
             return
 
         # filter exceptions that flamingo server handles it self
         if record.exc_info:
 
             # OSErrors
-            if(isinstance(record.exc_info[1], OSError) and
+            if (isinstance(record.exc_info[1], OSError) and
                record.exc_info[1].errno in (13, 98)):
 
                 return
 
             # event loop exceptions
-            elif(isinstance(record.exc_info[1], RuntimeError) and
-                 record.exc_info[1].args[0] == 'Event loop is closed'):
+            elif (isinstance(record.exc_info[1], RuntimeError) and
+                  record.exc_info[1].args[0] == 'Event loop is closed'):
 
                 return
 
         # add record to ring buffer
         time_stamp = datetime.fromtimestamp(record.created)
         time_stamp_str = time_stamp.strftime('%H:%M:%S.%f')
 
@@ -78,15 +78,15 @@
         }
 
         # filter log if self.loggers is set
         if self.loggers and record_args['name'] not in self.loggers:
             return
 
         # find current hook name and content path
-        if(self.server and
+        if (self.server and
            self.server.build_environment and
            self.server.build_environment.context):
 
             context = self.server.build_environment.context
 
             if context.content:
                 record_args['content_path'] = context.content['path']
@@ -188,14 +188,14 @@
             'pre_build',
             'post_build',
             'render_content',
             'render_media_content',
         ]
 
         for record in self.buffer[::]:
-            if(record['hook'] in hooks or
+            if (record['hook'] in hooks or
                record['content_path'] in paths):
 
                 self.buffer.remove(record)
                 self.stats[record['level']] -= 1
 
         self._notify(records=self.buffer, initial=True)
```

### Comparing `flamingo-1.8/flamingo/server/rpc.py` & `flamingo-1.9/flamingo/server/rpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
                 result=result,
             ),
         )
 
         await self.send_str(websocket, message)
 
     async def __call__(self, http_request):
-        if(http_request.method != 'GET' or
+        if (http_request.method != 'GET' or
            http_request.headers.get('upgrade', '').lower() != 'websocket'):
 
             return Response(status=405)
 
         websocket = WebSocketResponse()
         await websocket.prepare(http_request)
```

### Comparing `flamingo-1.8/flamingo/server/server.py` & `flamingo-1.9/flamingo/server/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,16 +501,16 @@
         for flags, path in events:
             if Flags.CODE in flags:
                 continue
 
             if Flags.TEMPLATE in flags or Flags.STATIC in flags:
                 non_content_event = True
 
-            elif(os.path.splitext(path)[1].lower() in
-                 ('.jpg', '.jpeg', '.png', '.svg', )):
+            elif (os.path.splitext(path)[1].lower() in
+                  ('.jpg', '.jpeg', '.png', '.svg', )):
 
                 non_content_event = True
 
                 paths.append(
                     os.path.relpath(path, self.context.settings.CONTENT_ROOT)
                 )
```

### Comparing `flamingo-1.8/flamingo/server/static/lib/js.cookie-2.2.1.min.js` & `flamingo-1.9/flamingo/server/static/lib/js.cookie-2.2.1.min.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/static/lib/ractive.js` & `flamingo-1.9/flamingo/server/static/lib/ractive.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/static/lib/ractive.js.map` & `flamingo-1.9/flamingo/server/static/lib/ractive.js.map`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/static/lib/ractive.min.js` & `flamingo-1.9/flamingo/server/static/lib/ractive.min.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/static/lib/ractive.min.js.map` & `flamingo-1.9/flamingo/server/static/lib/ractive.min.js.map`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/static/lib/rpc.js` & `flamingo-1.9/flamingo/server/static/lib/rpc.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/static/main.js` & `flamingo-1.9/flamingo/server/static/main.js`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/static/style.css` & `flamingo-1.9/flamingo/server/static/style.css`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/templates/directory_list.html` & `flamingo-1.9/flamingo/server/templates/directory_list.html`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/templates/index.html` & `flamingo-1.9/flamingo/server/templates/index.html`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/templates/plugin_options.html` & `flamingo-1.9/flamingo/server/templates/plugin_options.html`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/server/watcher.py` & `flamingo-1.9/flamingo/server/watcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
                 notify(
                     (Flags.INFO, ), 'git merge detected. watching suspended',
                 )
 
             return False
 
-        if('rebase-apply' in git_dir_content or
+        if ('rebase-apply' in git_dir_content or
            'rebase-merge' in git_dir_content):
 
             if not self._git_is_locked:
                 self._git_is_locked = True
 
                 notify(
                     (Flags.INFO, ),
```

### Comparing `flamingo-1.8/flamingo/theme/templates/image.html` & `flamingo-1.9/flamingo/theme/templates/image.html`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo/theme/templates/jinja2/error.html` & `flamingo-1.9/flamingo/theme/templates/jinja2/error.html`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/flamingo.egg-info/PKG-INFO` & `flamingo-1.9/flamingo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamingo
-Version: 1.8
+Version: 1.9
 Summary: Flamingo is a python3-based, pelican-inspired static site generator
 Home-page: https://github.com/pengutronix/flamingo
 Author: Florian Scherf
 Author-email: python@pengutronix.de
 License: Apache License 2.0
 Description: flamingo
         ========
```

### Comparing `flamingo-1.8/flamingo.egg-info/SOURCES.txt` & `flamingo-1.9/flamingo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/setup.cfg` & `flamingo-1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `flamingo-1.8/setup.py` & `flamingo-1.9/setup.py`

 * *Files identical despite different names*


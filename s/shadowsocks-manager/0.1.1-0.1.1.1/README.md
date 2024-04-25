# Comparing `tmp/shadowsocks_manager-0.1.1.tar.gz` & `tmp/shadowsocks_manager-0.1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadowsocks_manager-0.1.1.tar", last modified: Mon Apr 22 18:27:39 2024, max compression
+gzip compressed data, was "shadowsocks_manager-0.1.1.1.tar", last modified: Thu Apr 25 15:15:13 2024, max compression
```

## Comparing `shadowsocks_manager-0.1.1.tar` & `shadowsocks_manager-0.1.1.1.tar`

### file list

```diff
@@ -1,116 +1,123 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-22 18:27:39.951819 shadowsocks_manager-0.1.1/
--rw-r--r--   0 alex       (501) staff       (20)     1067 2021-10-11 15:18:49.000000 shadowsocks_manager-0.1.1/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)    16285 2024-04-22 18:27:39.951723 shadowsocks_manager-0.1.1/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)    13563 2024-04-22 18:22:37.000000 shadowsocks_manager-0.1.1/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-22 18:27:39.938016 shadowsocks_manager-0.1.1/bin/
--rw-r--r--   0 alex       (501) staff       (20)      781 2024-04-14 15:00:19.000000 shadowsocks_manager-0.1.1/bin/ssm-dev-start
--rw-r--r--   0 alex       (501) staff       (20)      334 2024-04-14 15:00:19.000000 shadowsocks_manager-0.1.1/bin/ssm-dev-stop
--rw-r--r--   0 alex       (501) staff       (20)     5944 2024-04-14 15:00:19.000000 shadowsocks_manager-0.1.1/bin/ssm-setup
--rw-r--r--   0 alex       (501) staff       (20)     2254 2024-04-17 13:26:49.000000 shadowsocks_manager-0.1.1/bin/ssm-test
--rw-r--r--   0 alex       (501) staff       (20)       89 2024-04-22 13:19:13.000000 shadowsocks_manager-0.1.1/pyproject.toml
--rw-r--r--   0 alex       (501) staff       (20)     2721 2024-04-22 18:27:39.952142 shadowsocks_manager-0.1.1/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)       94 2024-04-14 15:00:19.000000 shadowsocks_manager-0.1.1/setup.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-22 18:27:39.938594 shadowsocks_manager-0.1.1/shadowsocks_manager/
--rw-r--r--   0 alex       (501) staff       (20)        0 2024-04-14 15:00:19.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1151 2024-04-18 07:06:29.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/__main__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-22 18:27:39.939472 shadowsocks_manager-0.1.1/shadowsocks_manager/args_formatter/
--rw-r--r--   0 alex       (501) staff       (20)     2714 2021-03-17 15:49:47.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/args_formatter/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1888 2021-03-17 16:47:15.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/args_formatter/tests.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-22 18:27:39.940617 shadowsocks_manager-0.1.1/shadowsocks_manager/domain/
--rw-r--r--   0 alex       (501) staff       (20)        0 2019-12-11 05:22:01.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/domain/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2502 2024-04-18 14:57:55.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/domain/admin.py
--rw-r--r--   0 alex       (501) staff       (20)      191 2021-03-13 19:27:15.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/domain/apps.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-22 18:27:39.940992 shadowsocks_manager-0.1.1/shadowsocks_manager/domain/migrations/
--rw-r--r--   0 alex       (501) staff       (20)     4046 2024-04-21 20:23:39.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/domain/migrations/0001_initial.py
--rw-r--r--   0 alex       (501) staff       (20)        0 2019-05-12 15:12:12.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/domain/migrations/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     8241 2021-04-03 18:22:01.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/domain/models.py
--rw-r--r--   0 alex       (501) staff       (20)      758 2021-04-03 18:22:01.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/domain/serializers.py
--rw-r--r--   0 alex       (501) staff       (20)     3926 2024-04-21 18:50:51.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/domain/tests.py
--rw-r--r--   0 alex       (501) staff       (20)      480 2021-03-13 19:27:15.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/domain/urls.py
--rw-r--r--   0 alex       (501) staff       (20)     1158 2021-04-03 18:23:45.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/domain/views.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-22 18:27:39.941642 shadowsocks_manager-0.1.1/shadowsocks_manager/dynamicmethod/
--rw-r--r--   0 alex       (501) staff       (20)        0 2019-06-02 20:22:59.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/dynamicmethod/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      167 2021-03-13 19:27:15.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/dynamicmethod/admin.py
--rw-r--r--   0 alex       (501) staff       (20)      205 2021-03-13 19:27:15.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/dynamicmethod/apps.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-22 18:27:39.941750 shadowsocks_manager-0.1.1/shadowsocks_manager/dynamicmethod/migrations/
--rw-r--r--   0 alex       (501) staff       (20)        0 2019-06-02 20:22:59.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/dynamicmethod/migrations/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2711 2021-04-03 16:59:06.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/dynamicmethod/models.py
--rw-r--r--   0 alex       (501) staff       (20)      164 2021-03-13 19:27:15.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/dynamicmethod/tests.py
--rw-r--r--   0 alex       (501) staff       (20)      167 2021-03-13 19:27:15.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/dynamicmethod/views.py
--rwxr-xr-x   0 alex       (501) staff       (20)      940 2024-04-21 20:11:55.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/manage.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-22 18:27:39.942763 shadowsocks_manager-0.1.1/shadowsocks_manager/notification/
--rw-r--r--   0 alex       (501) staff       (20)        0 2019-05-12 15:12:12.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/notification/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      470 2024-04-18 14:58:06.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/notification/admin.py
--rw-r--r--   0 alex       (501) staff       (20)      203 2021-03-13 19:27:15.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/notification/apps.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-22 18:27:39.942992 shadowsocks_manager-0.1.1/shadowsocks_manager/notification/migrations/
--rw-r--r--   0 alex       (501) staff       (20)     1362 2020-01-05 13:29:57.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/notification/migrations/0001_initial.py
--rw-r--r--   0 alex       (501) staff       (20)        0 2019-05-12 15:12:12.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/notification/migrations/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1798 2021-03-19 19:03:40.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/notification/models.py
--rw-r--r--   0 alex       (501) staff       (20)      368 2021-03-13 19:27:15.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/notification/serializers.py
--rw-r--r--   0 alex       (501) staff       (20)     2581 2024-04-21 18:49:59.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/notification/tests.py
--rw-r--r--   0 alex       (501) staff       (20)      372 2021-03-13 19:27:15.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/notification/urls.py
--rw-r--r--   0 alex       (501) staff       (20)      473 2021-03-13 19:27:15.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/notification/views.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-22 18:27:39.943194 shadowsocks_manager-0.1.1/shadowsocks_manager/retry/
--rw-r--r--   0 alex       (501) staff       (20)     2195 2021-03-17 19:32:26.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/retry/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1205 2024-04-21 18:55:16.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/retry/tests.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-22 18:27:39.943865 shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocks_manager/
--rw-r--r--   0 alex       (501) staff       (20)      242 2024-04-21 20:32:18.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocks_manager/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      870 2024-04-21 20:32:28.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocks_manager/celery.py
--rw-r--r--   0 alex       (501) staff       (20)     5771 2024-04-18 14:29:33.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocks_manager/settings.py
--rw-r--r--   0 alex       (501) staff       (20)     1121 2024-04-18 14:26:58.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocks_manager/urls.py
--rw-r--r--   0 alex       (501) staff       (20)      495 2024-04-09 15:55:16.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocks_manager/wsgi.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-22 18:27:39.946424 shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/
--rw-r--r--   0 alex       (501) staff       (20)        0 2024-04-04 17:40:19.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     6335 2024-04-18 15:01:10.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/admin.py
--rw-r--r--   0 alex       (501) staff       (20)      202 2024-04-18 14:29:48.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/apps.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-22 18:27:39.946686 shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/management/
--rw-r--r--   0 alex       (501) staff       (20)        0 2024-04-14 15:00:19.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/management/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-22 18:27:39.946879 shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/management/commands/
--rw-r--r--   0 alex       (501) staff       (20)        0 2024-04-14 15:00:19.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/management/commands/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1100 2024-04-18 14:43:51.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/management/commands/shadowsocks_config.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-22 18:27:39.947503 shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/migrations/
--rw-r--r--   0 alex       (501) staff       (20)     8298 2024-04-21 20:23:39.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/migrations/0001_initial.py
--rw-r--r--   0 alex       (501) staff       (20)        0 2019-05-30 21:03:07.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/migrations/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    36547 2024-04-21 14:16:15.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/models.py
--rw-r--r--   0 alex       (501) staff       (20)     1542 2022-04-12 11:12:03.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/serializers.py
--rw-r--r--   0 alex       (501) staff       (20)      410 2024-04-18 15:09:54.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/tasks.py
--rw-r--r--   0 alex       (501) staff       (20)    19241 2024-04-21 18:52:16.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/tests.py
--rw-r--r--   0 alex       (501) staff       (20)      626 2024-04-18 14:27:46.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/urls.py
--rw-r--r--   0 alex       (501) staff       (20)     1523 2022-04-12 11:12:03.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/views.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-22 18:27:39.948218 shadowsocks_manager-0.1.1/shadowsocks_manager/singleton/
--rw-r--r--   0 alex       (501) staff       (20)        0 2019-05-12 18:29:46.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/singleton/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      167 2021-03-13 19:27:15.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/singleton/admin.py
--rw-r--r--   0 alex       (501) staff       (20)      197 2021-03-13 19:27:15.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/singleton/apps.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-22 18:27:39.948345 shadowsocks_manager-0.1.1/shadowsocks_manager/singleton/migrations/
--rw-r--r--   0 alex       (501) staff       (20)        0 2019-05-12 18:29:46.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/singleton/migrations/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1052 2021-03-13 19:27:15.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/singleton/models.py
--rw-r--r--   0 alex       (501) staff       (20)      164 2021-03-13 19:27:15.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/singleton/tests.py
--rw-r--r--   0 alex       (501) staff       (20)      167 2021-03-13 19:27:15.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/singleton/views.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-22 18:27:39.949461 shadowsocks_manager-0.1.1/shadowsocks_manager/statistic/
--rw-r--r--   0 alex       (501) staff       (20)        0 2021-03-13 19:27:15.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/statistic/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2505 2024-04-18 15:00:12.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/statistic/admin.py
--rw-r--r--   0 alex       (501) staff       (20)      197 2021-03-13 19:27:15.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/statistic/apps.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-22 18:27:39.949867 shadowsocks_manager-0.1.1/shadowsocks_manager/statistic/migrations/
--rw-r--r--   0 alex       (501) staff       (20)     2513 2021-03-13 14:17:35.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/statistic/migrations/0001_initial.py
--rw-r--r--   0 alex       (501) staff       (20)      467 2021-03-13 17:16:50.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/statistic/migrations/0002_auto_20210313_1419.py
--rw-r--r--   0 alex       (501) staff       (20)        0 2021-03-13 19:27:15.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/statistic/migrations/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    10309 2024-04-19 16:37:02.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/statistic/models.py
--rw-r--r--   0 alex       (501) staff       (20)      576 2021-03-13 19:27:15.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/statistic/serializers.py
--rw-r--r--   0 alex       (501) staff       (20)      305 2024-04-18 15:00:27.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/statistic/tasks.py
--rw-r--r--   0 alex       (501) staff       (20)     2735 2024-04-21 18:49:42.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/statistic/tests.py
--rw-r--r--   0 alex       (501) staff       (20)      380 2021-03-13 19:27:15.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/statistic/urls.py
--rw-r--r--   0 alex       (501) staff       (20)      663 2021-03-13 19:27:15.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/statistic/views.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-22 18:27:39.951102 shadowsocks_manager-0.1.1/shadowsocks_manager/utils/
--rw-r--r--   0 alex       (501) staff       (20)        0 2024-04-14 15:00:19.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/utils/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      549 2024-04-18 07:09:03.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/utils/celery.py
--rw-r--r--   0 alex       (501) staff       (20)     1648 2024-04-21 20:25:04.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/utils/createsuperuser.py
--rw-r--r--   0 alex       (501) staff       (20)     1839 2024-04-18 08:16:45.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/utils/dotenv.py
--rw-r--r--   0 alex       (501) staff       (20)      610 2024-04-18 07:07:01.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/utils/manage.py
--rw-r--r--   0 alex       (501) staff       (20)      481 2024-04-18 07:07:23.000000 shadowsocks_manager-0.1.1/shadowsocks_manager/utils/uwsgi.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-22 18:27:39.951395 shadowsocks_manager-0.1.1/shadowsocks_manager.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)    16285 2024-04-22 18:27:39.000000 shadowsocks_manager-0.1.1/shadowsocks_manager.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     3810 2024-04-22 18:27:39.000000 shadowsocks_manager-0.1.1/shadowsocks_manager.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2024-04-22 18:27:39.000000 shadowsocks_manager-0.1.1/shadowsocks_manager.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)      329 2024-04-22 18:27:39.000000 shadowsocks_manager-0.1.1/shadowsocks_manager.egg-info/entry_points.txt
--rw-r--r--   0 alex       (501) staff       (20)      591 2024-04-22 18:27:39.000000 shadowsocks_manager-0.1.1/shadowsocks_manager.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       20 2024-04-22 18:27:39.000000 shadowsocks_manager-0.1.1/shadowsocks_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.514456 shadowsocks_manager-0.1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18976 2024-04-25 15:15:13.514456 shadowsocks_manager-0.1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.498456 shadowsocks_manager-0.1.1.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/bin/ssm-dev-start
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/bin/ssm-dev-stop
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/bin/ssm-setup
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/bin/ssm-test
+-rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-04-25 15:15:10.000000 shadowsocks_manager-0.1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:15:13.514456 shadowsocks_manager-0.1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.498456 shadowsocks_manager-0.1.1.1/shadowsocks_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/.env
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.502456 shadowsocks_manager-0.1.1.1/shadowsocks_manager/args_formatter/
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/args_formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/args_formatter/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.502456 shadowsocks_manager-0.1.1.1/shadowsocks_manager/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/domain/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/domain/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.502456 shadowsocks_manager-0.1.1.1/shadowsocks_manager/domain/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/domain/fixtures/nameserver.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.502456 shadowsocks_manager-0.1.1.1/shadowsocks_manager/domain/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/domain/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/domain/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/domain/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/domain/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/domain/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/domain/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.502456 shadowsocks_manager-0.1.1.1/shadowsocks_manager/dynamicmethod/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/dynamicmethod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/dynamicmethod/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/dynamicmethod/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.502456 shadowsocks_manager-0.1.1.1/shadowsocks_manager/dynamicmethod/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/dynamicmethod/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/dynamicmethod/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/dynamicmethod/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/dynamicmethod/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.502456 shadowsocks_manager-0.1.1.1/shadowsocks_manager/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/fixtures/auth.group.json
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/fixtures/django_celery_beat.intervalschedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/fixtures/sites.site.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      940 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.506456 shadowsocks_manager-0.1.1.1/shadowsocks_manager/notification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/notification/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/notification/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.506456 shadowsocks_manager-0.1.1.1/shadowsocks_manager/notification/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/notification/fixtures/template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.506456 shadowsocks_manager-0.1.1.1/shadowsocks_manager/notification/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/notification/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/notification/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/notification/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/notification/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/notification/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/notification/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.506456 shadowsocks_manager-0.1.1.1/shadowsocks_manager/retry/
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/retry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/retry/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.506456 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocks_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocks_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocks_manager/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocks_manager/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocks_manager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocks_manager/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.506456 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.506456 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/fixtures/config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.510456 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.510456 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/management/commands/shadowsocks_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.510456 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36547 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19241 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.510456 shadowsocks_manager-0.1.1.1/shadowsocks_manager/singleton/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/singleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/singleton/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/singleton/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.510456 shadowsocks_manager-0.1.1.1/shadowsocks_manager/singleton/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/singleton/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/singleton/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/singleton/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/singleton/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.510456 shadowsocks_manager-0.1.1.1/shadowsocks_manager/statistic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/statistic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/statistic/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/statistic/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.510456 shadowsocks_manager-0.1.1.1/shadowsocks_manager/statistic/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/statistic/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10309 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/statistic/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/statistic/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/statistic/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/statistic/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/statistic/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/statistic/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.510456 shadowsocks_manager-0.1.1.1/shadowsocks_manager/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/utils/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/utils/createsuperuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/utils/dotenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/utils/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-25 15:14:57.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager/utils/uwsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:13.510456 shadowsocks_manager-0.1.1.1/shadowsocks_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18976 2024-04-25 15:15:13.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-25 15:15:13.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:15:13.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-25 15:15:13.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-25 15:15:13.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-25 15:15:13.000000 shadowsocks_manager-0.1.1.1/shadowsocks_manager.egg-info/top_level.txt
```

### Comparing `shadowsocks_manager-0.1.1/LICENSE` & `shadowsocks_manager-0.1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/PKG-INFO` & `shadowsocks_manager-0.1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,37 @@
 Metadata-Version: 2.1
 Name: shadowsocks-manager
-Version: 0.1.1
+Version: 0.1.1.1
 Summary: A shadowsocks manager for multi-user and traffic statistics
-Home-page: https://github.com/alexzhangs/shadowsocks-manager
-Author: Alex
-Author-email: alexzhangs@gmail.com
-License: MIT
+Author-email: Alex <alexzhangs@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2021 Alex Zhang
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://www.0xbeta.com/shadowsocks-manager/
+Project-URL: repository, https://github.com/alexzhangs/shadowsocks-manager
+Project-URL: issues, https://github.com/alexzhangs/shadowsocks-manager/issues
 Keywords: shadowsocks,manager,django,web,statistics,cluster,celery,uwsgi,pypi,docker,github-actions
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
@@ -25,15 +47,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: Proxy Servers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: System :: Networking :: Firewalls
-Classifier: Topic :: System :: Systems Administration
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: future
 Requires-Dist: six
 Requires-Dist: boto3
 Requires-Dist: celery
@@ -58,23 +79,37 @@
 Requires-Dist: python-crontab; python_version > "2.7"
 Requires-Dist: python-decouple
 Requires-Dist: python-memcached==1.59
 Requires-Dist: pytz
 Requires-Dist: requests
 Requires-Dist: shadowsocks-alexforks
 Requires-Dist: uWSGI
+Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: bump-my-version; extra == "dev"
+Requires-Dist: codecov-cli; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: setuptools; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: wheel; extra == "dev"
 
-[![GitHub tag](https://img.shields.io/github/v/tag/alexzhangs/shadowsocks-manager?sort=date)](https://github.com/alexzhangs/shadowsocks-manager/tags)
-[![GitHub](https://img.shields.io/github/license/alexzhangs/shadowsocks-manager.svg?style=flat-square)](https://github.com/alexzhangs/shadowsocks-manager/)
+[![License](https://img.shields.io/github/license/alexzhangs/shadowsocks-manager.svg?style=flat-square)](https://github.com/alexzhangs/shadowsocks-manager/)
 [![GitHub last commit](https://img.shields.io/github/last-commit/alexzhangs/shadowsocks-manager.svg?style=flat-square)](https://github.com/alexzhangs/shadowsocks-manager/commits/master)
-
-[![Test shadowsocks-manager](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/main.yml/badge.svg)](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/main.yml)
-[![codecov](https://codecov.io/gh/alexzhangs/shadowsocks-manager/graph/badge.svg?token=KTI3TNRKAV)](https://codecov.io/gh/alexzhangs/shadowsocks-manager)
 [![GitHub issues](https://img.shields.io/github/issues/alexzhangs/shadowsocks-manager.svg?style=flat-square)](https://github.com/alexzhangs/shadowsocks-manager/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/alexzhangs/shadowsocks-manager.svg?style=flat-square)](https://github.com/alexzhangs/shadowsocks-manager/pulls)
+[![GitHub tag](https://img.shields.io/github/v/tag/alexzhangs/shadowsocks-manager?sort=date)](https://github.com/alexzhangs/shadowsocks-manager/tags)
+
+[![GitHub Actions - CI Unit test](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/ci-unittest.yml/badge.svg)](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/ci-unittest.yml)
+[![GitHub Actions - CI TestPyPI](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/ci-testpypi.yml/badge.svg)](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/ci-testpypi.yml)
+[![GitHub Actions - CI PyPI](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/ci-pypi.yml/badge.svg)](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/ci-pypi.yml)
+[![PyPI Package Version](https://badge.fury.io/py/shadowsocks-manager.svg)](https://pypi.org/project/shadowsocks-manager/)
+[![codecov](https://codecov.io/gh/alexzhangs/shadowsocks-manager/graph/badge.svg?token=KTI3TNRKAV)](https://codecov.io/gh/alexzhangs/shadowsocks-manager)
+
+[![GitHub Actions - CI Docker Build and Push](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/ci-docker.yml/badge.svg)](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/ci-docker.yml)
+[![Docker Image Version](https://img.shields.io/docker/v/alexzhangs/shadowsocks-manager?label=docker%20image)](https://hub.docker.com/r/alexzhangs/shadowsocks-manager)
 
 # shadowsocks-manager
 
 A web-based Shadowsocks management tool.
 
 Features:
 
@@ -97,18 +132,18 @@
         * Pre-installed, and have a builtin service manager.
 
 Code in Python, base on Django, Django REST framework, Celery, and SQLite.
 
 The development status can be found at: [project home](https://github.com/alexzhangs/shadowsocks-manager/projects/1).
 
 Node List:
-![Home › Shadowsocks › Shadowsocks Nodes](/assets/images/shadowsocks-node-list.png)
+![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-list.png)
 
 Node's Shadowsocks Manager:
-![Home › Shadowsocks › Shadowsocks Nodes](/assets/images/shadowsocks-node-ssmanager.png)
+![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-ssmanager.png)
 
 
 ## 1. Requirements
 
 * Python 2.7, Python 3.x
 * Django 1.11.x, Django 3.x
 * macOS Big Sur
@@ -416,15 +451,15 @@
     # install the package from the test pypi
     # --no-deps is used to skip installing dependencies for the test pypi
     pip install -i https://test.pypi.org/simple/ --no-deps shadowsocks-manager
 
     # install the package from the live pypi
     # --no-binary is used to force building the package from the source
     # --use-pep517 is used together to make sure the PEP 517 is tested
-    pip install --no-binary --use-pep517 shadowsocks-manager
+    pip install --no-binary shadowsocks-manager --use-pep517 shadowsocks-manager
     ```
 
 1. Build the docker image
 
     ```sh
     docker build -t alexzhangs/shadowsocks-manager .
     ```
```

### Comparing `shadowsocks_manager-0.1.1/README.md` & `shadowsocks_manager-0.1.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,21 @@
-[![GitHub tag](https://img.shields.io/github/v/tag/alexzhangs/shadowsocks-manager?sort=date)](https://github.com/alexzhangs/shadowsocks-manager/tags)
-[![GitHub](https://img.shields.io/github/license/alexzhangs/shadowsocks-manager.svg?style=flat-square)](https://github.com/alexzhangs/shadowsocks-manager/)
+[![License](https://img.shields.io/github/license/alexzhangs/shadowsocks-manager.svg?style=flat-square)](https://github.com/alexzhangs/shadowsocks-manager/)
 [![GitHub last commit](https://img.shields.io/github/last-commit/alexzhangs/shadowsocks-manager.svg?style=flat-square)](https://github.com/alexzhangs/shadowsocks-manager/commits/master)
-
-[![Test shadowsocks-manager](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/main.yml/badge.svg)](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/main.yml)
-[![codecov](https://codecov.io/gh/alexzhangs/shadowsocks-manager/graph/badge.svg?token=KTI3TNRKAV)](https://codecov.io/gh/alexzhangs/shadowsocks-manager)
 [![GitHub issues](https://img.shields.io/github/issues/alexzhangs/shadowsocks-manager.svg?style=flat-square)](https://github.com/alexzhangs/shadowsocks-manager/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/alexzhangs/shadowsocks-manager.svg?style=flat-square)](https://github.com/alexzhangs/shadowsocks-manager/pulls)
+[![GitHub tag](https://img.shields.io/github/v/tag/alexzhangs/shadowsocks-manager?sort=date)](https://github.com/alexzhangs/shadowsocks-manager/tags)
+
+[![GitHub Actions - CI Unit test](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/ci-unittest.yml/badge.svg)](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/ci-unittest.yml)
+[![GitHub Actions - CI TestPyPI](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/ci-testpypi.yml/badge.svg)](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/ci-testpypi.yml)
+[![GitHub Actions - CI PyPI](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/ci-pypi.yml/badge.svg)](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/ci-pypi.yml)
+[![PyPI Package Version](https://badge.fury.io/py/shadowsocks-manager.svg)](https://pypi.org/project/shadowsocks-manager/)
+[![codecov](https://codecov.io/gh/alexzhangs/shadowsocks-manager/graph/badge.svg?token=KTI3TNRKAV)](https://codecov.io/gh/alexzhangs/shadowsocks-manager)
+
+[![GitHub Actions - CI Docker Build and Push](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/ci-docker.yml/badge.svg)](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/ci-docker.yml)
+[![Docker Image Version](https://img.shields.io/docker/v/alexzhangs/shadowsocks-manager?label=docker%20image)](https://hub.docker.com/r/alexzhangs/shadowsocks-manager)
 
 # shadowsocks-manager
 
 A web-based Shadowsocks management tool.
 
 Features:
 
@@ -32,18 +38,18 @@
         * Pre-installed, and have a builtin service manager.
 
 Code in Python, base on Django, Django REST framework, Celery, and SQLite.
 
 The development status can be found at: [project home](https://github.com/alexzhangs/shadowsocks-manager/projects/1).
 
 Node List:
-![Home › Shadowsocks › Shadowsocks Nodes](/assets/images/shadowsocks-node-list.png)
+![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-list.png)
 
 Node's Shadowsocks Manager:
-![Home › Shadowsocks › Shadowsocks Nodes](/assets/images/shadowsocks-node-ssmanager.png)
+![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-ssmanager.png)
 
 
 ## 1. Requirements
 
 * Python 2.7, Python 3.x
 * Django 1.11.x, Django 3.x
 * macOS Big Sur
@@ -351,15 +357,15 @@
     # install the package from the test pypi
     # --no-deps is used to skip installing dependencies for the test pypi
     pip install -i https://test.pypi.org/simple/ --no-deps shadowsocks-manager
 
     # install the package from the live pypi
     # --no-binary is used to force building the package from the source
     # --use-pep517 is used together to make sure the PEP 517 is tested
-    pip install --no-binary --use-pep517 shadowsocks-manager
+    pip install --no-binary shadowsocks-manager --use-pep517 shadowsocks-manager
     ```
 
 1. Build the docker image
 
     ```sh
     docker build -t alexzhangs/shadowsocks-manager .
     ```
```

### Comparing `shadowsocks_manager-0.1.1/bin/ssm-dev-start` & `shadowsocks_manager-0.1.1.1/bin/ssm-dev-start`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/bin/ssm-setup` & `shadowsocks_manager-0.1.1.1/bin/ssm-setup`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/bin/ssm-test` & `shadowsocks_manager-0.1.1.1/bin/ssm-test`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/__main__.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/__main__.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/args_formatter/__init__.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/args_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/args_formatter/tests.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/args_formatter/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/domain/admin.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/domain/admin.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/domain/models.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/domain/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/domain/serializers.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/domain/serializers.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/domain/tests.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/domain/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/domain/views.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/domain/views.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/dynamicmethod/models.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/dynamicmethod/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/manage.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/manage.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/notification/models.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/notification/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/notification/tests.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/notification/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/retry/__init__.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/retry/__init__.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/retry/tests.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/retry/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocks_manager/celery.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocks_manager/celery.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocks_manager/settings.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocks_manager/settings.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocks_manager/urls.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocks_manager/urls.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/admin.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/admin.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/management/commands/shadowsocks_config.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/management/commands/shadowsocks_config.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/models.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/serializers.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/serializers.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/tests.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/urls.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/urls.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/shadowsocksz/views.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/shadowsocksz/views.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/singleton/models.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/singleton/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/statistic/admin.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/statistic/admin.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/statistic/models.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/statistic/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/statistic/serializers.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/statistic/serializers.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/statistic/tests.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/statistic/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/statistic/views.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/statistic/views.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/utils/celery.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/utils/celery.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/utils/createsuperuser.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/utils/createsuperuser.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/utils/dotenv.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/utils/dotenv.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager/utils/manage.py` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager/utils/manage.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager.egg-info/PKG-INFO` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,37 @@
 Metadata-Version: 2.1
 Name: shadowsocks-manager
-Version: 0.1.1
+Version: 0.1.1.1
 Summary: A shadowsocks manager for multi-user and traffic statistics
-Home-page: https://github.com/alexzhangs/shadowsocks-manager
-Author: Alex
-Author-email: alexzhangs@gmail.com
-License: MIT
+Author-email: Alex <alexzhangs@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2021 Alex Zhang
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://www.0xbeta.com/shadowsocks-manager/
+Project-URL: repository, https://github.com/alexzhangs/shadowsocks-manager
+Project-URL: issues, https://github.com/alexzhangs/shadowsocks-manager/issues
 Keywords: shadowsocks,manager,django,web,statistics,cluster,celery,uwsgi,pypi,docker,github-actions
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
@@ -25,15 +47,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: Proxy Servers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: System :: Networking :: Firewalls
-Classifier: Topic :: System :: Systems Administration
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: future
 Requires-Dist: six
 Requires-Dist: boto3
 Requires-Dist: celery
@@ -58,23 +79,37 @@
 Requires-Dist: python-crontab; python_version > "2.7"
 Requires-Dist: python-decouple
 Requires-Dist: python-memcached==1.59
 Requires-Dist: pytz
 Requires-Dist: requests
 Requires-Dist: shadowsocks-alexforks
 Requires-Dist: uWSGI
+Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: bump-my-version; extra == "dev"
+Requires-Dist: codecov-cli; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: setuptools; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: wheel; extra == "dev"
 
-[![GitHub tag](https://img.shields.io/github/v/tag/alexzhangs/shadowsocks-manager?sort=date)](https://github.com/alexzhangs/shadowsocks-manager/tags)
-[![GitHub](https://img.shields.io/github/license/alexzhangs/shadowsocks-manager.svg?style=flat-square)](https://github.com/alexzhangs/shadowsocks-manager/)
+[![License](https://img.shields.io/github/license/alexzhangs/shadowsocks-manager.svg?style=flat-square)](https://github.com/alexzhangs/shadowsocks-manager/)
 [![GitHub last commit](https://img.shields.io/github/last-commit/alexzhangs/shadowsocks-manager.svg?style=flat-square)](https://github.com/alexzhangs/shadowsocks-manager/commits/master)
-
-[![Test shadowsocks-manager](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/main.yml/badge.svg)](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/main.yml)
-[![codecov](https://codecov.io/gh/alexzhangs/shadowsocks-manager/graph/badge.svg?token=KTI3TNRKAV)](https://codecov.io/gh/alexzhangs/shadowsocks-manager)
 [![GitHub issues](https://img.shields.io/github/issues/alexzhangs/shadowsocks-manager.svg?style=flat-square)](https://github.com/alexzhangs/shadowsocks-manager/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/alexzhangs/shadowsocks-manager.svg?style=flat-square)](https://github.com/alexzhangs/shadowsocks-manager/pulls)
+[![GitHub tag](https://img.shields.io/github/v/tag/alexzhangs/shadowsocks-manager?sort=date)](https://github.com/alexzhangs/shadowsocks-manager/tags)
+
+[![GitHub Actions - CI Unit test](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/ci-unittest.yml/badge.svg)](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/ci-unittest.yml)
+[![GitHub Actions - CI TestPyPI](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/ci-testpypi.yml/badge.svg)](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/ci-testpypi.yml)
+[![GitHub Actions - CI PyPI](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/ci-pypi.yml/badge.svg)](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/ci-pypi.yml)
+[![PyPI Package Version](https://badge.fury.io/py/shadowsocks-manager.svg)](https://pypi.org/project/shadowsocks-manager/)
+[![codecov](https://codecov.io/gh/alexzhangs/shadowsocks-manager/graph/badge.svg?token=KTI3TNRKAV)](https://codecov.io/gh/alexzhangs/shadowsocks-manager)
+
+[![GitHub Actions - CI Docker Build and Push](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/ci-docker.yml/badge.svg)](https://github.com/alexzhangs/shadowsocks-manager/actions/workflows/ci-docker.yml)
+[![Docker Image Version](https://img.shields.io/docker/v/alexzhangs/shadowsocks-manager?label=docker%20image)](https://hub.docker.com/r/alexzhangs/shadowsocks-manager)
 
 # shadowsocks-manager
 
 A web-based Shadowsocks management tool.
 
 Features:
 
@@ -97,18 +132,18 @@
         * Pre-installed, and have a builtin service manager.
 
 Code in Python, base on Django, Django REST framework, Celery, and SQLite.
 
 The development status can be found at: [project home](https://github.com/alexzhangs/shadowsocks-manager/projects/1).
 
 Node List:
-![Home › Shadowsocks › Shadowsocks Nodes](/assets/images/shadowsocks-node-list.png)
+![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-list.png)
 
 Node's Shadowsocks Manager:
-![Home › Shadowsocks › Shadowsocks Nodes](/assets/images/shadowsocks-node-ssmanager.png)
+![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-ssmanager.png)
 
 
 ## 1. Requirements
 
 * Python 2.7, Python 3.x
 * Django 1.11.x, Django 3.x
 * macOS Big Sur
@@ -416,15 +451,15 @@
     # install the package from the test pypi
     # --no-deps is used to skip installing dependencies for the test pypi
     pip install -i https://test.pypi.org/simple/ --no-deps shadowsocks-manager
 
     # install the package from the live pypi
     # --no-binary is used to force building the package from the source
     # --use-pep517 is used together to make sure the PEP 517 is tested
-    pip install --no-binary --use-pep517 shadowsocks-manager
+    pip install --no-binary shadowsocks-manager --use-pep517 shadowsocks-manager
     ```
 
 1. Build the docker image
 
     ```sh
     docker build -t alexzhangs/shadowsocks-manager .
     ```
```

### Comparing `shadowsocks_manager-0.1.1/shadowsocks_manager.egg-info/SOURCES.txt` & `shadowsocks_manager-0.1.1.1/shadowsocks_manager.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
-setup.py
 bin/ssm-dev-start
 bin/ssm-dev-stop
 bin/ssm-setup
 bin/ssm-test
+shadowsocks_manager/.env
 shadowsocks_manager/__init__.py
 shadowsocks_manager/__main__.py
 shadowsocks_manager/manage.py
 shadowsocks_manager.egg-info/PKG-INFO
 shadowsocks_manager.egg-info/SOURCES.txt
 shadowsocks_manager.egg-info/dependency_links.txt
 shadowsocks_manager.egg-info/entry_points.txt
@@ -22,32 +21,37 @@
 shadowsocks_manager/domain/admin.py
 shadowsocks_manager/domain/apps.py
 shadowsocks_manager/domain/models.py
 shadowsocks_manager/domain/serializers.py
 shadowsocks_manager/domain/tests.py
 shadowsocks_manager/domain/urls.py
 shadowsocks_manager/domain/views.py
-shadowsocks_manager/domain/migrations/0001_initial.py
+shadowsocks_manager/domain/fixtures/nameserver.json
 shadowsocks_manager/domain/migrations/__init__.py
 shadowsocks_manager/dynamicmethod/__init__.py
 shadowsocks_manager/dynamicmethod/admin.py
 shadowsocks_manager/dynamicmethod/apps.py
 shadowsocks_manager/dynamicmethod/models.py
 shadowsocks_manager/dynamicmethod/tests.py
 shadowsocks_manager/dynamicmethod/views.py
 shadowsocks_manager/dynamicmethod/migrations/__init__.py
+shadowsocks_manager/fixtures/auth.group.json
+shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json
+shadowsocks_manager/fixtures/django_celery_beat.intervalschedule.json
+shadowsocks_manager/fixtures/django_celery_beat.periodictask.json
+shadowsocks_manager/fixtures/sites.site.json
 shadowsocks_manager/notification/__init__.py
 shadowsocks_manager/notification/admin.py
 shadowsocks_manager/notification/apps.py
 shadowsocks_manager/notification/models.py
 shadowsocks_manager/notification/serializers.py
 shadowsocks_manager/notification/tests.py
 shadowsocks_manager/notification/urls.py
 shadowsocks_manager/notification/views.py
-shadowsocks_manager/notification/migrations/0001_initial.py
+shadowsocks_manager/notification/fixtures/template.json
 shadowsocks_manager/notification/migrations/__init__.py
 shadowsocks_manager/retry/__init__.py
 shadowsocks_manager/retry/tests.py
 shadowsocks_manager/shadowsocks_manager/__init__.py
 shadowsocks_manager/shadowsocks_manager/celery.py
 shadowsocks_manager/shadowsocks_manager/settings.py
 shadowsocks_manager/shadowsocks_manager/urls.py
@@ -57,18 +61,18 @@
 shadowsocks_manager/shadowsocksz/apps.py
 shadowsocks_manager/shadowsocksz/models.py
 shadowsocks_manager/shadowsocksz/serializers.py
 shadowsocks_manager/shadowsocksz/tasks.py
 shadowsocks_manager/shadowsocksz/tests.py
 shadowsocks_manager/shadowsocksz/urls.py
 shadowsocks_manager/shadowsocksz/views.py
+shadowsocks_manager/shadowsocksz/fixtures/config.json
 shadowsocks_manager/shadowsocksz/management/__init__.py
 shadowsocks_manager/shadowsocksz/management/commands/__init__.py
 shadowsocks_manager/shadowsocksz/management/commands/shadowsocks_config.py
-shadowsocks_manager/shadowsocksz/migrations/0001_initial.py
 shadowsocks_manager/shadowsocksz/migrations/__init__.py
 shadowsocks_manager/singleton/__init__.py
 shadowsocks_manager/singleton/admin.py
 shadowsocks_manager/singleton/apps.py
 shadowsocks_manager/singleton/models.py
 shadowsocks_manager/singleton/tests.py
 shadowsocks_manager/singleton/views.py
@@ -78,16 +82,14 @@
 shadowsocks_manager/statistic/apps.py
 shadowsocks_manager/statistic/models.py
 shadowsocks_manager/statistic/serializers.py
 shadowsocks_manager/statistic/tasks.py
 shadowsocks_manager/statistic/tests.py
 shadowsocks_manager/statistic/urls.py
 shadowsocks_manager/statistic/views.py
-shadowsocks_manager/statistic/migrations/0001_initial.py
-shadowsocks_manager/statistic/migrations/0002_auto_20210313_1419.py
 shadowsocks_manager/statistic/migrations/__init__.py
 shadowsocks_manager/utils/__init__.py
 shadowsocks_manager/utils/celery.py
 shadowsocks_manager/utils/createsuperuser.py
 shadowsocks_manager/utils/dotenv.py
 shadowsocks_manager/utils/manage.py
 shadowsocks_manager/utils/uwsgi.py
```


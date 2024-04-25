# Comparing `tmp/my_quart_app-1.1.1.tar.gz` & `tmp/my_quart_app-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_quart_app-1.1.1.tar", last modified: Thu Apr 25 12:07:24 2024, max compression
+gzip compressed data, was "my_quart_app-1.1.2.tar", last modified: Thu Apr 25 12:10:07 2024, max compression
```

## Comparing `my_quart_app-1.1.1.tar` & `my_quart_app-1.1.2.tar`

### file list

```diff
@@ -1,108 +1,109 @@
-drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:07:24.445267 my_quart_app-1.1.1/
--rw-r--r--   0 tanyagoel   (501) staff       (20)       86 2024-04-25 11:30:29.000000 my_quart_app-1.1.1/MANIFEST.in
--rw-r--r--   0 tanyagoel   (501) staff       (20)     2021 2024-04-25 12:07:24.445036 my_quart_app-1.1.1/PKG-INFO
--rw-r--r--   0 tanyagoel   (501) staff       (20)      278 2021-08-18 13:16:12.000000 my_quart_app-1.1.1/README.md
-drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:07:24.416172 my_quart_app-1.1.1/app/
--rw-r--r--   0 tanyagoel   (501) staff       (20)       24 2024-04-25 12:05:58.000000 my_quart_app-1.1.1/app/__init__.py
-drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:07:24.425364 my_quart_app-1.1.1/app/__pycache__/
--rw-r--r--   0 tanyagoel   (501) staff       (20)     1311 2021-11-18 12:05:41.000000 my_quart_app-1.1.1/app/__pycache__/_choices.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     2390 2023-06-06 06:56:14.000000 my_quart_app-1.1.1/app/__pycache__/cg_celery.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     2386 2023-06-06 06:27:22.000000 my_quart_app-1.1.1/app/__pycache__/cg_celery.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    12332 2023-06-13 07:41:27.000000 my_quart_app-1.1.1/app/__pycache__/choices.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    11460 2023-06-06 06:27:23.000000 my_quart_app-1.1.1/app/__pycache__/choices.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    53016 2023-06-14 16:21:08.000000 my_quart_app-1.1.1/app/__pycache__/routes.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    52882 2023-06-06 06:27:23.000000 my_quart_app-1.1.1/app/__pycache__/routes.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     6127 2023-06-14 16:26:26.000000 my_quart_app-1.1.1/app/__pycache__/server.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     6318 2023-06-06 06:26:49.000000 my_quart_app-1.1.1/app/__pycache__/server.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    38311 2023-06-14 16:21:09.000000 my_quart_app-1.1.1/app/__pycache__/service.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    13954 2022-12-28 05:43:17.000000 my_quart_app-1.1.1/app/__pycache__/service.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     4815 2023-06-14 16:45:54.000000 my_quart_app-1.1.1/app/__pycache__/settings.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     4765 2023-06-06 06:26:49.000000 my_quart_app-1.1.1/app/__pycache__/settings.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    17073 2023-06-06 06:56:15.000000 my_quart_app-1.1.1/app/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    17038 2023-06-06 06:27:23.000000 my_quart_app-1.1.1/app/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    17339 2023-06-06 07:01:22.000000 my_quart_app-1.1.1/app/__pycache__/validator.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    17550 2022-08-06 17:56:30.000000 my_quart_app-1.1.1/app/__pycache__/validator.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    19773 2023-06-06 06:56:15.000000 my_quart_app-1.1.1/app/__pycache__/validator_new.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    20489 2023-06-06 06:27:23.000000 my_quart_app-1.1.1/app/__pycache__/validator_new.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     2802 2023-05-01 08:09:22.000000 my_quart_app-1.1.1/app/cg_celery.py
--rw-r--r--   0 tanyagoel   (501) staff       (20)    13926 2024-01-08 08:22:26.000000 my_quart_app-1.1.1/app/choices.py
--rw-r--r--   0 tanyagoel   (501) staff       (20)     9225 2024-01-08 08:22:26.000000 my_quart_app-1.1.1/app/permissions.json
--rw-r--r--   0 tanyagoel   (501) staff       (20)    99419 2024-01-08 08:22:26.000000 my_quart_app-1.1.1/app/routes.py
--rw-r--r--   0 tanyagoel   (501) staff       (20)      100 2024-04-25 12:05:32.000000 my_quart_app-1.1.1/app/run_server.py
--rw-r--r--   0 tanyagoel   (501) staff       (20)     7862 2023-06-15 06:28:10.000000 my_quart_app-1.1.1/app/server.py
--rw-r--r--   0 tanyagoel   (501) staff       (20)    88045 2024-01-08 08:22:26.000000 my_quart_app-1.1.1/app/service.py
-drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:07:24.425607 my_quart_app-1.1.1/app/services/
-drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:07:24.425915 my_quart_app-1.1.1/app/services/__pycache__/
--rw-r--r--   0 tanyagoel   (501) staff       (20)     1552 2023-06-13 07:41:28.000000 my_quart_app-1.1.1/app/services/__pycache__/user_service.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     1707 2024-01-08 08:22:26.000000 my_quart_app-1.1.1/app/services/user_service.py
--rw-r--r--   0 tanyagoel   (501) staff       (20)     7164 2024-01-08 08:22:26.000000 my_quart_app-1.1.1/app/settings.py
-drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:07:24.428624 my_quart_app-1.1.1/app/tasks/
-drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:07:24.436746 my_quart_app-1.1.1/app/tasks/__pycache__/
--rw-r--r--   0 tanyagoel   (501) staff       (20)     4855 2023-06-06 07:01:23.000000 my_quart_app-1.1.1/app/tasks/__pycache__/callback.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     4859 2022-11-23 05:08:14.000000 my_quart_app-1.1.1/app/tasks/__pycache__/callback.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     5834 2023-06-06 07:01:23.000000 my_quart_app-1.1.1/app/tasks/__pycache__/delegator.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     5822 2022-12-28 05:43:18.000000 my_quart_app-1.1.1/app/tasks/__pycache__/delegator.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    93922 2023-06-14 16:21:09.000000 my_quart_app-1.1.1/app/tasks/__pycache__/execution.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    82135 2022-12-23 02:34:11.000000 my_quart_app-1.1.1/app/tasks/__pycache__/execution.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     3470 2023-06-13 07:41:28.000000 my_quart_app-1.1.1/app/tasks/__pycache__/helpers.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     3307 2022-12-23 02:34:12.000000 my_quart_app-1.1.1/app/tasks/__pycache__/helpers.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     8209 2022-12-23 07:43:22.000000 my_quart_app-1.1.1/app/tasks/__pycache__/invoice_automation.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     3424 2023-06-06 06:56:24.000000 my_quart_app-1.1.1/app/tasks/__pycache__/notice_preview.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     3338 2022-12-28 05:43:18.000000 my_quart_app-1.1.1/app/tasks/__pycache__/notice_preview.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    23219 2022-03-25 07:01:46.000000 my_quart_app-1.1.1/app/tasks/__pycache__/physical_notice.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    32423 2023-06-08 10:50:58.000000 my_quart_app-1.1.1/app/tasks/__pycache__/report.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    34421 2022-12-28 05:43:18.000000 my_quart_app-1.1.1/app/tasks/__pycache__/report.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     5862 2022-12-23 07:57:02.000000 my_quart_app-1.1.1/app/tasks/__pycache__/reports.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     7061 2021-09-28 11:11:40.000000 my_quart_app-1.1.1/app/tasks/__pycache__/result_tasks.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    16475 2023-06-06 07:01:22.000000 my_quart_app-1.1.1/app/tasks/__pycache__/tasks.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    16403 2022-11-23 05:08:13.000000 my_quart_app-1.1.1/app/tasks/__pycache__/tasks.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     7122 2024-01-08 08:22:26.000000 my_quart_app-1.1.1/app/tasks/callback.py
--rw-r--r--   0 tanyagoel   (501) staff       (20)    11541 2024-01-08 08:22:26.000000 my_quart_app-1.1.1/app/tasks/delegator.py
--rw-r--r--   0 tanyagoel   (501) staff       (20)   185677 2024-01-08 08:22:26.000000 my_quart_app-1.1.1/app/tasks/execution.py
--rw-r--r--   0 tanyagoel   (501) staff       (20)     5373 2023-07-10 12:28:29.000000 my_quart_app-1.1.1/app/tasks/helpers.py
-drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:07:24.438611 my_quart_app-1.1.1/app/tasks/notice/
-drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:07:24.441547 my_quart_app-1.1.1/app/tasks/notice/__pycache__/
--rw-r--r--   0 tanyagoel   (501) staff       (20)      655 2022-08-09 18:21:50.000000 my_quart_app-1.1.1/app/tasks/notice/__pycache__/custom_exception.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     7298 2023-06-06 06:56:24.000000 my_quart_app-1.1.1/app/tasks/notice/__pycache__/digital_notice.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     6692 2022-12-23 02:34:11.000000 my_quart_app-1.1.1/app/tasks/notice/__pycache__/digital_notice.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    14725 2023-06-06 06:56:23.000000 my_quart_app-1.1.1/app/tasks/notice/__pycache__/helpers.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    14681 2022-11-23 05:04:46.000000 my_quart_app-1.1.1/app/tasks/notice/__pycache__/helpers.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     2753 2023-06-06 06:56:24.000000 my_quart_app-1.1.1/app/tasks/notice/__pycache__/loan_service.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     2795 2022-11-23 05:04:46.000000 my_quart_app-1.1.1/app/tasks/notice/__pycache__/loan_service.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    30962 2023-06-06 06:56:24.000000 my_quart_app-1.1.1/app/tasks/notice/__pycache__/notice_service.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    27758 2022-12-23 02:34:11.000000 my_quart_app-1.1.1/app/tasks/notice/__pycache__/notice_service.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     7409 2023-06-06 07:01:22.000000 my_quart_app-1.1.1/app/tasks/notice/__pycache__/physical_notice.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     6795 2022-12-23 02:34:11.000000 my_quart_app-1.1.1/app/tasks/notice/__pycache__/physical_notice.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    12574 2023-07-10 12:28:29.000000 my_quart_app-1.1.1/app/tasks/notice/digital_notice.py
--rw-r--r--   0 tanyagoel   (501) staff       (20)    25232 2023-07-10 12:28:29.000000 my_quart_app-1.1.1/app/tasks/notice/helpers.py
--rw-r--r--   0 tanyagoel   (501) staff       (20)     3273 2023-07-10 12:28:29.000000 my_quart_app-1.1.1/app/tasks/notice/loan_service.py
-drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:07:24.442075 my_quart_app-1.1.1/app/tasks/notice/notice_callback/
-drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:07:24.443281 my_quart_app-1.1.1/app/tasks/notice/notice_callback/__pycache__/
--rw-r--r--   0 tanyagoel   (501) staff       (20)    23087 2023-06-14 16:21:09.000000 my_quart_app-1.1.1/app/tasks/notice/notice_callback/__pycache__/commons.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    22704 2022-12-23 02:34:11.000000 my_quart_app-1.1.1/app/tasks/notice/notice_callback/__pycache__/commons.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     1080 2023-06-06 06:56:24.000000 my_quart_app-1.1.1/app/tasks/notice/notice_callback/__pycache__/digital_notice.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     1078 2022-11-23 05:04:46.000000 my_quart_app-1.1.1/app/tasks/notice/notice_callback/__pycache__/digital_notice.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     6604 2023-06-06 07:01:22.000000 my_quart_app-1.1.1/app/tasks/notice/notice_callback/__pycache__/physical_notice.cpython-310.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     6571 2022-11-23 05:08:13.000000 my_quart_app-1.1.1/app/tasks/notice/notice_callback/__pycache__/physical_notice.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)    37169 2023-07-10 12:28:29.000000 my_quart_app-1.1.1/app/tasks/notice/notice_callback/commons.py
--rw-r--r--   0 tanyagoel   (501) staff       (20)      990 2023-07-10 12:28:29.000000 my_quart_app-1.1.1/app/tasks/notice/notice_callback/digital_notice.py
--rw-r--r--   0 tanyagoel   (501) staff       (20)    12068 2023-07-10 12:28:29.000000 my_quart_app-1.1.1/app/tasks/notice/notice_callback/physical_notice.py
--rw-r--r--   0 tanyagoel   (501) staff       (20)    62348 2023-07-10 12:28:29.000000 my_quart_app-1.1.1/app/tasks/notice/notice_service.py
--rw-r--r--   0 tanyagoel   (501) staff       (20)    13164 2023-07-10 12:28:29.000000 my_quart_app-1.1.1/app/tasks/notice/physical_notice.py
-drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:07:24.410940 my_quart_app-1.1.1/app/tasks/notice_helpers/
-drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:07:24.443500 my_quart_app-1.1.1/app/tasks/notice_helpers/__pycache__/
--rw-r--r--   0 tanyagoel   (501) staff       (20)    45559 2022-03-25 07:01:47.000000 my_quart_app-1.1.1/app/tasks/notice_helpers/__pycache__/notice_helper.cpython-39.pyc
--rw-r--r--   0 tanyagoel   (501) staff       (20)     5260 2023-07-10 12:28:29.000000 my_quart_app-1.1.1/app/tasks/notice_preview.py
--rw-r--r--   0 tanyagoel   (501) staff       (20)    66519 2024-01-08 08:22:26.000000 my_quart_app-1.1.1/app/tasks/report.py
--rw-r--r--   0 tanyagoel   (501) staff       (20)    16596 2024-01-08 08:22:26.000000 my_quart_app-1.1.1/app/tasks/tasks.py
--rw-r--r--   0 tanyagoel   (501) staff       (20)    22524 2024-01-08 08:22:26.000000 my_quart_app-1.1.1/app/utils.py
--rw-r--r--   0 tanyagoel   (501) staff       (20)    20431 2023-05-23 10:51:19.000000 my_quart_app-1.1.1/app/validator.py
--rw-r--r--   0 tanyagoel   (501) staff       (20)    22651 2024-01-08 08:22:26.000000 my_quart_app-1.1.1/app/validator_new.py
-drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:07:24.444629 my_quart_app-1.1.1/my_quart_app.egg-info/
--rw-r--r--   0 tanyagoel   (501) staff       (20)     2021 2024-04-25 12:07:24.000000 my_quart_app-1.1.1/my_quart_app.egg-info/PKG-INFO
--rw-r--r--   0 tanyagoel   (501) staff       (20)     3730 2024-04-25 12:07:24.000000 my_quart_app-1.1.1/my_quart_app.egg-info/SOURCES.txt
--rw-r--r--   0 tanyagoel   (501) staff       (20)        1 2024-04-25 12:07:24.000000 my_quart_app-1.1.1/my_quart_app.egg-info/dependency_links.txt
--rw-r--r--   0 tanyagoel   (501) staff       (20)     1035 2024-04-25 12:07:24.000000 my_quart_app-1.1.1/my_quart_app.egg-info/requires.txt
--rw-r--r--   0 tanyagoel   (501) staff       (20)        4 2024-04-25 12:07:24.000000 my_quart_app-1.1.1/my_quart_app.egg-info/top_level.txt
--rw-r--r--   0 tanyagoel   (501) staff       (20)       38 2024-04-25 12:07:24.445306 my_quart_app-1.1.1/setup.cfg
--rw-r--r--   0 tanyagoel   (501) staff       (20)      398 2024-04-25 12:07:01.000000 my_quart_app-1.1.1/setup.py
+drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:10:07.108274 my_quart_app-1.1.2/
+-rw-r--r--   0 tanyagoel   (501) staff       (20)       86 2024-04-25 11:30:29.000000 my_quart_app-1.1.2/MANIFEST.in
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     2021 2024-04-25 12:10:07.108044 my_quart_app-1.1.2/PKG-INFO
+-rw-r--r--   0 tanyagoel   (501) staff       (20)      278 2021-08-18 13:16:12.000000 my_quart_app-1.1.2/README.md
+drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:10:07.076111 my_quart_app-1.1.2/app/
+-rw-r--r--   0 tanyagoel   (501) staff       (20)       24 2024-04-25 12:05:58.000000 my_quart_app-1.1.2/app/__init__.py
+drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:10:07.083142 my_quart_app-1.1.2/app/__pycache__/
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     1311 2021-11-18 12:05:41.000000 my_quart_app-1.1.2/app/__pycache__/_choices.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     2390 2023-06-06 06:56:14.000000 my_quart_app-1.1.2/app/__pycache__/cg_celery.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     2386 2023-06-06 06:27:22.000000 my_quart_app-1.1.2/app/__pycache__/cg_celery.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    12332 2023-06-13 07:41:27.000000 my_quart_app-1.1.2/app/__pycache__/choices.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    11460 2023-06-06 06:27:23.000000 my_quart_app-1.1.2/app/__pycache__/choices.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    53016 2023-06-14 16:21:08.000000 my_quart_app-1.1.2/app/__pycache__/routes.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    52882 2023-06-06 06:27:23.000000 my_quart_app-1.1.2/app/__pycache__/routes.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     6127 2023-06-14 16:26:26.000000 my_quart_app-1.1.2/app/__pycache__/server.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     6318 2023-06-06 06:26:49.000000 my_quart_app-1.1.2/app/__pycache__/server.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    38311 2023-06-14 16:21:09.000000 my_quart_app-1.1.2/app/__pycache__/service.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    13954 2022-12-28 05:43:17.000000 my_quart_app-1.1.2/app/__pycache__/service.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     4815 2023-06-14 16:45:54.000000 my_quart_app-1.1.2/app/__pycache__/settings.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     4765 2023-06-06 06:26:49.000000 my_quart_app-1.1.2/app/__pycache__/settings.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    17073 2023-06-06 06:56:15.000000 my_quart_app-1.1.2/app/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    17038 2023-06-06 06:27:23.000000 my_quart_app-1.1.2/app/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    17339 2023-06-06 07:01:22.000000 my_quart_app-1.1.2/app/__pycache__/validator.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    17550 2022-08-06 17:56:30.000000 my_quart_app-1.1.2/app/__pycache__/validator.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    19773 2023-06-06 06:56:15.000000 my_quart_app-1.1.2/app/__pycache__/validator_new.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    20489 2023-06-06 06:27:23.000000 my_quart_app-1.1.2/app/__pycache__/validator_new.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     2802 2023-05-01 08:09:22.000000 my_quart_app-1.1.2/app/cg_celery.py
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    13926 2024-01-08 08:22:26.000000 my_quart_app-1.1.2/app/choices.py
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     9225 2024-01-08 08:22:26.000000 my_quart_app-1.1.2/app/permissions.json
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    99419 2024-01-08 08:22:26.000000 my_quart_app-1.1.2/app/routes.py
+-rw-r--r--   0 tanyagoel   (501) staff       (20)      100 2024-04-25 12:05:32.000000 my_quart_app-1.1.2/app/run_server.py
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     7862 2023-06-15 06:28:10.000000 my_quart_app-1.1.2/app/server.py
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    88045 2024-01-08 08:22:26.000000 my_quart_app-1.1.2/app/service.py
+drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:10:07.083321 my_quart_app-1.1.2/app/services/
+drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:10:07.083439 my_quart_app-1.1.2/app/services/__pycache__/
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     1552 2023-06-13 07:41:28.000000 my_quart_app-1.1.2/app/services/__pycache__/user_service.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     1707 2024-01-08 08:22:26.000000 my_quart_app-1.1.2/app/services/user_service.py
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     7164 2024-01-08 08:22:26.000000 my_quart_app-1.1.2/app/settings.py
+drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:10:07.084998 my_quart_app-1.1.2/app/tasks/
+drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:10:07.092009 my_quart_app-1.1.2/app/tasks/__pycache__/
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     4855 2023-06-06 07:01:23.000000 my_quart_app-1.1.2/app/tasks/__pycache__/callback.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     4859 2022-11-23 05:08:14.000000 my_quart_app-1.1.2/app/tasks/__pycache__/callback.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     5834 2023-06-06 07:01:23.000000 my_quart_app-1.1.2/app/tasks/__pycache__/delegator.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     5822 2022-12-28 05:43:18.000000 my_quart_app-1.1.2/app/tasks/__pycache__/delegator.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    93922 2023-06-14 16:21:09.000000 my_quart_app-1.1.2/app/tasks/__pycache__/execution.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    82135 2022-12-23 02:34:11.000000 my_quart_app-1.1.2/app/tasks/__pycache__/execution.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     3470 2023-06-13 07:41:28.000000 my_quart_app-1.1.2/app/tasks/__pycache__/helpers.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     3307 2022-12-23 02:34:12.000000 my_quart_app-1.1.2/app/tasks/__pycache__/helpers.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     8209 2022-12-23 07:43:22.000000 my_quart_app-1.1.2/app/tasks/__pycache__/invoice_automation.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     3424 2023-06-06 06:56:24.000000 my_quart_app-1.1.2/app/tasks/__pycache__/notice_preview.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     3338 2022-12-28 05:43:18.000000 my_quart_app-1.1.2/app/tasks/__pycache__/notice_preview.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    23219 2022-03-25 07:01:46.000000 my_quart_app-1.1.2/app/tasks/__pycache__/physical_notice.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    32423 2023-06-08 10:50:58.000000 my_quart_app-1.1.2/app/tasks/__pycache__/report.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    34421 2022-12-28 05:43:18.000000 my_quart_app-1.1.2/app/tasks/__pycache__/report.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     5862 2022-12-23 07:57:02.000000 my_quart_app-1.1.2/app/tasks/__pycache__/reports.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     7061 2021-09-28 11:11:40.000000 my_quart_app-1.1.2/app/tasks/__pycache__/result_tasks.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    16475 2023-06-06 07:01:22.000000 my_quart_app-1.1.2/app/tasks/__pycache__/tasks.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    16403 2022-11-23 05:08:13.000000 my_quart_app-1.1.2/app/tasks/__pycache__/tasks.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     7122 2024-01-08 08:22:26.000000 my_quart_app-1.1.2/app/tasks/callback.py
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    11541 2024-01-08 08:22:26.000000 my_quart_app-1.1.2/app/tasks/delegator.py
+-rw-r--r--   0 tanyagoel   (501) staff       (20)   185677 2024-01-08 08:22:26.000000 my_quart_app-1.1.2/app/tasks/execution.py
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     5373 2023-07-10 12:28:29.000000 my_quart_app-1.1.2/app/tasks/helpers.py
+drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:10:07.101714 my_quart_app-1.1.2/app/tasks/notice/
+drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:10:07.104744 my_quart_app-1.1.2/app/tasks/notice/__pycache__/
+-rw-r--r--   0 tanyagoel   (501) staff       (20)      655 2022-08-09 18:21:50.000000 my_quart_app-1.1.2/app/tasks/notice/__pycache__/custom_exception.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     7298 2023-06-06 06:56:24.000000 my_quart_app-1.1.2/app/tasks/notice/__pycache__/digital_notice.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     6692 2022-12-23 02:34:11.000000 my_quart_app-1.1.2/app/tasks/notice/__pycache__/digital_notice.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    14725 2023-06-06 06:56:23.000000 my_quart_app-1.1.2/app/tasks/notice/__pycache__/helpers.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    14681 2022-11-23 05:04:46.000000 my_quart_app-1.1.2/app/tasks/notice/__pycache__/helpers.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     2753 2023-06-06 06:56:24.000000 my_quart_app-1.1.2/app/tasks/notice/__pycache__/loan_service.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     2795 2022-11-23 05:04:46.000000 my_quart_app-1.1.2/app/tasks/notice/__pycache__/loan_service.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    30962 2023-06-06 06:56:24.000000 my_quart_app-1.1.2/app/tasks/notice/__pycache__/notice_service.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    27758 2022-12-23 02:34:11.000000 my_quart_app-1.1.2/app/tasks/notice/__pycache__/notice_service.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     7409 2023-06-06 07:01:22.000000 my_quart_app-1.1.2/app/tasks/notice/__pycache__/physical_notice.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     6795 2022-12-23 02:34:11.000000 my_quart_app-1.1.2/app/tasks/notice/__pycache__/physical_notice.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    12574 2023-07-10 12:28:29.000000 my_quart_app-1.1.2/app/tasks/notice/digital_notice.py
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    25232 2023-07-10 12:28:29.000000 my_quart_app-1.1.2/app/tasks/notice/helpers.py
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     3273 2023-07-10 12:28:29.000000 my_quart_app-1.1.2/app/tasks/notice/loan_service.py
+drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:10:07.105243 my_quart_app-1.1.2/app/tasks/notice/notice_callback/
+drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:10:07.106304 my_quart_app-1.1.2/app/tasks/notice/notice_callback/__pycache__/
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    23087 2023-06-14 16:21:09.000000 my_quart_app-1.1.2/app/tasks/notice/notice_callback/__pycache__/commons.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    22704 2022-12-23 02:34:11.000000 my_quart_app-1.1.2/app/tasks/notice/notice_callback/__pycache__/commons.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     1080 2023-06-06 06:56:24.000000 my_quart_app-1.1.2/app/tasks/notice/notice_callback/__pycache__/digital_notice.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     1078 2022-11-23 05:04:46.000000 my_quart_app-1.1.2/app/tasks/notice/notice_callback/__pycache__/digital_notice.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     6604 2023-06-06 07:01:22.000000 my_quart_app-1.1.2/app/tasks/notice/notice_callback/__pycache__/physical_notice.cpython-310.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     6571 2022-11-23 05:08:13.000000 my_quart_app-1.1.2/app/tasks/notice/notice_callback/__pycache__/physical_notice.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    37169 2023-07-10 12:28:29.000000 my_quart_app-1.1.2/app/tasks/notice/notice_callback/commons.py
+-rw-r--r--   0 tanyagoel   (501) staff       (20)      990 2023-07-10 12:28:29.000000 my_quart_app-1.1.2/app/tasks/notice/notice_callback/digital_notice.py
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    12068 2023-07-10 12:28:29.000000 my_quart_app-1.1.2/app/tasks/notice/notice_callback/physical_notice.py
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    62348 2023-07-10 12:28:29.000000 my_quart_app-1.1.2/app/tasks/notice/notice_service.py
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    13164 2023-07-10 12:28:29.000000 my_quart_app-1.1.2/app/tasks/notice/physical_notice.py
+drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:10:07.072381 my_quart_app-1.1.2/app/tasks/notice_helpers/
+drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:10:07.106474 my_quart_app-1.1.2/app/tasks/notice_helpers/__pycache__/
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    45559 2022-03-25 07:01:47.000000 my_quart_app-1.1.2/app/tasks/notice_helpers/__pycache__/notice_helper.cpython-39.pyc
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     5260 2023-07-10 12:28:29.000000 my_quart_app-1.1.2/app/tasks/notice_preview.py
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    66519 2024-01-08 08:22:26.000000 my_quart_app-1.1.2/app/tasks/report.py
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    16596 2024-01-08 08:22:26.000000 my_quart_app-1.1.2/app/tasks/tasks.py
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    22524 2024-01-08 08:22:26.000000 my_quart_app-1.1.2/app/utils.py
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    20431 2023-05-23 10:51:19.000000 my_quart_app-1.1.2/app/validator.py
+-rw-r--r--   0 tanyagoel   (501) staff       (20)    22651 2024-01-08 08:22:26.000000 my_quart_app-1.1.2/app/validator_new.py
+drwxr-xr-x   0 tanyagoel   (501) staff       (20)        0 2024-04-25 12:10:07.107662 my_quart_app-1.1.2/my_quart_app.egg-info/
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     2021 2024-04-25 12:10:07.000000 my_quart_app-1.1.2/my_quart_app.egg-info/PKG-INFO
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     3769 2024-04-25 12:10:07.000000 my_quart_app-1.1.2/my_quart_app.egg-info/SOURCES.txt
+-rw-r--r--   0 tanyagoel   (501) staff       (20)        1 2024-04-25 12:10:07.000000 my_quart_app-1.1.2/my_quart_app.egg-info/dependency_links.txt
+-rw-r--r--   0 tanyagoel   (501) staff       (20)       53 2024-04-25 12:10:07.000000 my_quart_app-1.1.2/my_quart_app.egg-info/entry_points.txt
+-rw-r--r--   0 tanyagoel   (501) staff       (20)     1035 2024-04-25 12:10:07.000000 my_quart_app-1.1.2/my_quart_app.egg-info/requires.txt
+-rw-r--r--   0 tanyagoel   (501) staff       (20)        4 2024-04-25 12:10:07.000000 my_quart_app-1.1.2/my_quart_app.egg-info/top_level.txt
+-rw-r--r--   0 tanyagoel   (501) staff       (20)       38 2024-04-25 12:10:07.108312 my_quart_app-1.1.2/setup.cfg
+-rw-r--r--   0 tanyagoel   (501) staff       (20)      388 2024-04-25 12:09:54.000000 my_quart_app-1.1.2/setup.py
```

### Comparing `my_quart_app-1.1.1/PKG-INFO` & `my_quart_app-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my_quart_app
-Version: 1.1.1
+Version: 1.1.2
 Requires-Dist: aiofiles==0.8.0
 Requires-Dist: aioredis==1.3.1
 Requires-Dist: amqp==2.6.1
 Requires-Dist: asyncpg==0.26.0
 Requires-Dist: billiard==3.6.4.0
 Requires-Dist: black==20.8b1
 Requires-Dist: blinker==1.4
```

### Comparing `my_quart_app-1.1.1/app/__pycache__/_choices.cpython-39.pyc` & `my_quart_app-1.1.2/app/__pycache__/_choices.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/__pycache__/cg_celery.cpython-310.pyc` & `my_quart_app-1.1.2/app/__pycache__/cg_celery.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/__pycache__/cg_celery.cpython-39.pyc` & `my_quart_app-1.1.2/app/__pycache__/cg_celery.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/__pycache__/choices.cpython-310.pyc` & `my_quart_app-1.1.2/app/__pycache__/choices.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/__pycache__/choices.cpython-39.pyc` & `my_quart_app-1.1.2/app/__pycache__/choices.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/__pycache__/routes.cpython-310.pyc` & `my_quart_app-1.1.2/app/__pycache__/routes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/__pycache__/routes.cpython-39.pyc` & `my_quart_app-1.1.2/app/__pycache__/routes.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/__pycache__/server.cpython-310.pyc` & `my_quart_app-1.1.2/app/__pycache__/server.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/__pycache__/server.cpython-39.pyc` & `my_quart_app-1.1.2/app/__pycache__/server.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/__pycache__/service.cpython-310.pyc` & `my_quart_app-1.1.2/app/__pycache__/service.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/__pycache__/service.cpython-39.pyc` & `my_quart_app-1.1.2/app/__pycache__/service.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/__pycache__/settings.cpython-310.pyc` & `my_quart_app-1.1.2/app/__pycache__/settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/__pycache__/settings.cpython-39.pyc` & `my_quart_app-1.1.2/app/__pycache__/settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/__pycache__/utils.cpython-310.pyc` & `my_quart_app-1.1.2/app/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/__pycache__/utils.cpython-39.pyc` & `my_quart_app-1.1.2/app/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/__pycache__/validator.cpython-310.pyc` & `my_quart_app-1.1.2/app/__pycache__/validator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/__pycache__/validator.cpython-39.pyc` & `my_quart_app-1.1.2/app/__pycache__/validator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/__pycache__/validator_new.cpython-310.pyc` & `my_quart_app-1.1.2/app/__pycache__/validator_new.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/__pycache__/validator_new.cpython-39.pyc` & `my_quart_app-1.1.2/app/__pycache__/validator_new.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/cg_celery.py` & `my_quart_app-1.1.2/app/cg_celery.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/choices.py` & `my_quart_app-1.1.2/app/choices.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/permissions.json` & `my_quart_app-1.1.2/app/permissions.json`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/routes.py` & `my_quart_app-1.1.2/app/routes.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/server.py` & `my_quart_app-1.1.2/app/server.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/service.py` & `my_quart_app-1.1.2/app/service.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/services/__pycache__/user_service.cpython-310.pyc` & `my_quart_app-1.1.2/app/services/__pycache__/user_service.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/services/user_service.py` & `my_quart_app-1.1.2/app/services/user_service.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/settings.py` & `my_quart_app-1.1.2/app/settings.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/__pycache__/callback.cpython-310.pyc` & `my_quart_app-1.1.2/app/tasks/__pycache__/callback.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/__pycache__/callback.cpython-39.pyc` & `my_quart_app-1.1.2/app/tasks/__pycache__/callback.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/__pycache__/delegator.cpython-310.pyc` & `my_quart_app-1.1.2/app/tasks/__pycache__/delegator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/__pycache__/delegator.cpython-39.pyc` & `my_quart_app-1.1.2/app/tasks/__pycache__/delegator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/__pycache__/execution.cpython-310.pyc` & `my_quart_app-1.1.2/app/tasks/__pycache__/execution.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/__pycache__/execution.cpython-39.pyc` & `my_quart_app-1.1.2/app/tasks/__pycache__/execution.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/__pycache__/helpers.cpython-310.pyc` & `my_quart_app-1.1.2/app/tasks/__pycache__/helpers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/__pycache__/helpers.cpython-39.pyc` & `my_quart_app-1.1.2/app/tasks/__pycache__/helpers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/__pycache__/invoice_automation.cpython-39.pyc` & `my_quart_app-1.1.2/app/tasks/__pycache__/invoice_automation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/__pycache__/notice_preview.cpython-310.pyc` & `my_quart_app-1.1.2/app/tasks/__pycache__/notice_preview.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/__pycache__/notice_preview.cpython-39.pyc` & `my_quart_app-1.1.2/app/tasks/__pycache__/notice_preview.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/__pycache__/physical_notice.cpython-39.pyc` & `my_quart_app-1.1.2/app/tasks/__pycache__/physical_notice.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/__pycache__/report.cpython-310.pyc` & `my_quart_app-1.1.2/app/tasks/__pycache__/report.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/__pycache__/report.cpython-39.pyc` & `my_quart_app-1.1.2/app/tasks/__pycache__/report.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/__pycache__/reports.cpython-39.pyc` & `my_quart_app-1.1.2/app/tasks/__pycache__/reports.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/__pycache__/result_tasks.cpython-39.pyc` & `my_quart_app-1.1.2/app/tasks/__pycache__/result_tasks.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/__pycache__/tasks.cpython-310.pyc` & `my_quart_app-1.1.2/app/tasks/__pycache__/tasks.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/__pycache__/tasks.cpython-39.pyc` & `my_quart_app-1.1.2/app/tasks/__pycache__/tasks.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/callback.py` & `my_quart_app-1.1.2/app/tasks/callback.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/delegator.py` & `my_quart_app-1.1.2/app/tasks/delegator.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/execution.py` & `my_quart_app-1.1.2/app/tasks/execution.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/helpers.py` & `my_quart_app-1.1.2/app/tasks/helpers.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/__pycache__/custom_exception.cpython-39.pyc` & `my_quart_app-1.1.2/app/tasks/notice/__pycache__/custom_exception.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/__pycache__/digital_notice.cpython-310.pyc` & `my_quart_app-1.1.2/app/tasks/notice/__pycache__/digital_notice.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/__pycache__/digital_notice.cpython-39.pyc` & `my_quart_app-1.1.2/app/tasks/notice/__pycache__/digital_notice.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/__pycache__/helpers.cpython-310.pyc` & `my_quart_app-1.1.2/app/tasks/notice/__pycache__/helpers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/__pycache__/helpers.cpython-39.pyc` & `my_quart_app-1.1.2/app/tasks/notice/__pycache__/helpers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/__pycache__/loan_service.cpython-310.pyc` & `my_quart_app-1.1.2/app/tasks/notice/__pycache__/loan_service.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/__pycache__/loan_service.cpython-39.pyc` & `my_quart_app-1.1.2/app/tasks/notice/__pycache__/loan_service.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/__pycache__/notice_service.cpython-310.pyc` & `my_quart_app-1.1.2/app/tasks/notice/__pycache__/notice_service.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/__pycache__/notice_service.cpython-39.pyc` & `my_quart_app-1.1.2/app/tasks/notice/__pycache__/notice_service.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/__pycache__/physical_notice.cpython-310.pyc` & `my_quart_app-1.1.2/app/tasks/notice/__pycache__/physical_notice.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/__pycache__/physical_notice.cpython-39.pyc` & `my_quart_app-1.1.2/app/tasks/notice/__pycache__/physical_notice.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/digital_notice.py` & `my_quart_app-1.1.2/app/tasks/notice/digital_notice.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/helpers.py` & `my_quart_app-1.1.2/app/tasks/notice/helpers.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/loan_service.py` & `my_quart_app-1.1.2/app/tasks/notice/loan_service.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/notice_callback/__pycache__/commons.cpython-310.pyc` & `my_quart_app-1.1.2/app/tasks/notice/notice_callback/__pycache__/commons.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/notice_callback/__pycache__/commons.cpython-39.pyc` & `my_quart_app-1.1.2/app/tasks/notice/notice_callback/__pycache__/commons.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/notice_callback/__pycache__/digital_notice.cpython-310.pyc` & `my_quart_app-1.1.2/app/tasks/notice/notice_callback/__pycache__/digital_notice.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/notice_callback/__pycache__/digital_notice.cpython-39.pyc` & `my_quart_app-1.1.2/app/tasks/notice/notice_callback/__pycache__/digital_notice.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/notice_callback/__pycache__/physical_notice.cpython-310.pyc` & `my_quart_app-1.1.2/app/tasks/notice/notice_callback/__pycache__/physical_notice.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/notice_callback/__pycache__/physical_notice.cpython-39.pyc` & `my_quart_app-1.1.2/app/tasks/notice/notice_callback/__pycache__/physical_notice.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/notice_callback/commons.py` & `my_quart_app-1.1.2/app/tasks/notice/notice_callback/commons.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/notice_callback/digital_notice.py` & `my_quart_app-1.1.2/app/tasks/notice/notice_callback/digital_notice.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/notice_callback/physical_notice.py` & `my_quart_app-1.1.2/app/tasks/notice/notice_callback/physical_notice.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/notice_service.py` & `my_quart_app-1.1.2/app/tasks/notice/notice_service.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice/physical_notice.py` & `my_quart_app-1.1.2/app/tasks/notice/physical_notice.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice_helpers/__pycache__/notice_helper.cpython-39.pyc` & `my_quart_app-1.1.2/app/tasks/notice_helpers/__pycache__/notice_helper.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/notice_preview.py` & `my_quart_app-1.1.2/app/tasks/notice_preview.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/report.py` & `my_quart_app-1.1.2/app/tasks/report.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/tasks/tasks.py` & `my_quart_app-1.1.2/app/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/utils.py` & `my_quart_app-1.1.2/app/utils.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/validator.py` & `my_quart_app-1.1.2/app/validator.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/app/validator_new.py` & `my_quart_app-1.1.2/app/validator_new.py`

 * *Files identical despite different names*

### Comparing `my_quart_app-1.1.1/my_quart_app.egg-info/PKG-INFO` & `my_quart_app-1.1.2/my_quart_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my_quart_app
-Version: 1.1.1
+Version: 1.1.2
 Requires-Dist: aiofiles==0.8.0
 Requires-Dist: aioredis==1.3.1
 Requires-Dist: amqp==2.6.1
 Requires-Dist: asyncpg==0.26.0
 Requires-Dist: billiard==3.6.4.0
 Requires-Dist: black==20.8b1
 Requires-Dist: blinker==1.4
```

### Comparing `my_quart_app-1.1.1/my_quart_app.egg-info/SOURCES.txt` & `my_quart_app-1.1.2/my_quart_app.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -84,9 +84,10 @@
 app/tasks/notice/notice_callback/__pycache__/digital_notice.cpython-39.pyc
 app/tasks/notice/notice_callback/__pycache__/physical_notice.cpython-310.pyc
 app/tasks/notice/notice_callback/__pycache__/physical_notice.cpython-39.pyc
 app/tasks/notice_helpers/__pycache__/notice_helper.cpython-39.pyc
 my_quart_app.egg-info/PKG-INFO
 my_quart_app.egg-info/SOURCES.txt
 my_quart_app.egg-info/dependency_links.txt
+my_quart_app.egg-info/entry_points.txt
 my_quart_app.egg-info/requires.txt
 my_quart_app.egg-info/top_level.txt
```

### Comparing `my_quart_app-1.1.1/my_quart_app.egg-info/requires.txt` & `my_quart_app-1.1.2/my_quart_app.egg-info/requires.txt`

 * *Files identical despite different names*


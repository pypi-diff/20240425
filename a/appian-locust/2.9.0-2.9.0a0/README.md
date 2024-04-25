# Comparing `tmp/appian-locust-2.9.0.tar.gz` & `tmp/appian-locust-2.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appian-locust-2.9.0.tar", last modified: Wed Jan 10 16:58:05 2024, max compression
+gzip compressed data, was "appian-locust-2.9.0a0.tar", last modified: Tue Jan  9 15:57:03 2024, max compression
```

## Comparing `appian-locust-2.9.0.tar` & `appian-locust-2.9.0a0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 16:58:05.409665 appian-locust-2.9.0/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2024-01-10 16:57:56.000000 appian-locust-2.9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5111 2024-01-10 16:58:05.409665 appian-locust-2.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4539 2024-01-10 16:57:56.000000 appian-locust-2.9.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 16:58:05.403665 appian-locust-2.9.0/appian_locust/
--rw-rw-rw-   0 root         (0) root         (0)      263 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9361 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/_actions.py
--rw-rw-rw-   0 root         (0) root         (0)      784 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/_admin.py
--rw-rw-rw-   0 root         (0) root         (0)     2498 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/_base.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/_data_fabric.py
--rw-rw-rw-   0 root         (0) root         (0)    10165 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/_design.py
--rw-rw-rw-   0 root         (0) root         (0)     6244 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/_feature_toggle_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     8571 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/_grid_interactor.py
--rw-rw-rw-   0 root         (0) root         (0)    60658 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/_interactor.py
--rw-rw-rw-   0 root         (0) root         (0)     2565 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/_locust_error_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     7955 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/_news.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/_portals.py
--rw-rw-rw-   0 root         (0) root         (0)    15540 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/_rdo_interactor.py
--rw-rw-rw-   0 root         (0) root         (0)    15177 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/_records.py
--rw-rw-rw-   0 root         (0) root         (0)     7063 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/_records_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     7216 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/_reports.py
--rw-rw-rw-   0 root         (0) root         (0)     2711 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/_save_request_builder.py
--rw-rw-rw-   0 root         (0) root         (0)    10298 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/_sites.py
--rw-rw-rw-   0 root         (0) root         (0)     4533 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/_task_opener.py
--rw-rw-rw-   0 root         (0) root         (0)     7522 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2365 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/_ui_reconciler.py
--rw-rw-rw-   0 root         (0) root         (0)     7150 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/appian_client.py
--rw-rw-rw-   0 root         (0) root         (0)     5724 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/appian_task_set.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 16:58:05.404666 appian-locust-2.9.0/appian_locust/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/exceptions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1544 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/exceptions/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1792 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/feature_flag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 16:58:05.405665 appian-locust-2.9.0/appian_locust/info/
--rw-rw-rw-   0 root         (0) root         (0)      214 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1637 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/info/actions_info.py
--rw-rw-rw-   0 root         (0) root         (0)     3738 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/info/news_info.py
--rw-rw-rw-   0 root         (0) root         (0)      957 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/info/records_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1713 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/info/reports_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1258 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/info/sites_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1612 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/info/tasks_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 16:58:05.406665 appian-locust-2.9.0/appian_locust/objects/
--rw-rw-rw-   0 root         (0) root         (0)      196 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/objects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      144 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/objects/ai_skill.py
--rw-rw-rw-   0 root         (0) root         (0)      144 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/objects/ai_skill_type.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/objects/application.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/objects/design_object.py
--rw-rw-rw-   0 root         (0) root         (0)      546 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/objects/page.py
--rw-rw-rw-   0 root         (0) root         (0)      463 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/objects/site.py
--rw-rw-rw-   0 root         (0) root         (0)     4817 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/system_operator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 16:58:05.408666 appian-locust-2.9.0/appian_locust/uiform/
--rw-rw-rw-   0 root         (0) root         (0)      305 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/uiform/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4240 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/uiform/ai_skill_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)     6133 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/uiform/application_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)      991 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/uiform/design_object_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)     6238 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/uiform/design_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)     4593 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/uiform/record_list_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)     1322 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/uiform/record_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)    84937 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/uiform/uiform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 16:58:05.409665 appian-locust-2.9.0/appian_locust/utilities/
--rw-rw-rw-   0 root         (0) root         (0)      145 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3367 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/utilities/credentials.py
--rw-rw-rw-   0 root         (0) root         (0)    17411 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/utilities/helper.py
--rwxrwxrwx   0 root         (0) root         (0)     1393 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/utilities/loadDriverUtils.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/utilities/logger.py
--rw-rw-rw-   0 root         (0) root         (0)    20139 2024-01-10 16:57:56.000000 appian-locust-2.9.0/appian_locust/visitor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 16:58:05.404666 appian-locust-2.9.0/appian_locust.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5111 2024-01-10 16:58:05.000000 appian-locust-2.9.0/appian_locust.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2035 2024-01-10 16:58:05.000000 appian-locust-2.9.0/appian_locust.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-10 16:58:05.000000 appian-locust-2.9.0/appian_locust.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-01-10 16:58:05.000000 appian-locust-2.9.0/appian_locust.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-01-10 16:58:05.000000 appian-locust-2.9.0/appian_locust.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      595 2024-01-10 16:58:05.409665 appian-locust-2.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-01-10 16:57:56.000000 appian-locust-2.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 15:57:03.095363 appian-locust-2.9.0a0/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5113 2024-01-09 15:57:03.095363 appian-locust-2.9.0a0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4539 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 15:57:03.090364 appian-locust-2.9.0a0/appian_locust/
+-rw-rw-rw-   0 root         (0) root         (0)      263 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9361 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/_actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      784 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2498 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/_data_fabric.py
+-rw-rw-rw-   0 root         (0) root         (0)    10165 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/_design.py
+-rw-rw-rw-   0 root         (0) root         (0)     6244 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/_feature_toggle_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     8571 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/_grid_interactor.py
+-rw-rw-rw-   0 root         (0) root         (0)    60658 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/_interactor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2565 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/_locust_error_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     7955 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/_news.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/_portals.py
+-rw-rw-rw-   0 root         (0) root         (0)    15540 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/_rdo_interactor.py
+-rw-rw-rw-   0 root         (0) root         (0)    15177 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/_records.py
+-rw-rw-rw-   0 root         (0) root         (0)     7063 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/_records_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     7216 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)     2711 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/_save_request_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    10298 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/_sites.py
+-rw-rw-rw-   0 root         (0) root         (0)     4533 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/_task_opener.py
+-rw-rw-rw-   0 root         (0) root         (0)     7522 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2365 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/_ui_reconciler.py
+-rw-rw-rw-   0 root         (0) root         (0)     7131 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/appian_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     5724 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/appian_task_set.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 15:57:03.091364 appian-locust-2.9.0a0/appian_locust/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/exceptions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/exceptions/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/feature_flag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 15:57:03.092363 appian-locust-2.9.0a0/appian_locust/info/
+-rw-rw-rw-   0 root         (0) root         (0)      214 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1637 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/info/actions_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     3738 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/info/news_info.py
+-rw-rw-rw-   0 root         (0) root         (0)      957 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/info/records_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/info/reports_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1258 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/info/sites_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/info/tasks_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 15:57:03.093364 appian-locust-2.9.0a0/appian_locust/objects/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/objects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      144 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/objects/ai_skill.py
+-rw-rw-rw-   0 root         (0) root         (0)      144 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/objects/ai_skill_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/objects/application.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/objects/design_object.py
+-rw-rw-rw-   0 root         (0) root         (0)      546 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/objects/page.py
+-rw-rw-rw-   0 root         (0) root         (0)      463 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/objects/site.py
+-rw-rw-rw-   0 root         (0) root         (0)     4817 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/system_operator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 15:57:03.094364 appian-locust-2.9.0a0/appian_locust/uiform/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/uiform/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4240 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/uiform/ai_skill_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)     6133 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/uiform/application_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)      991 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/uiform/design_object_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)     6238 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/uiform/design_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)     4593 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/uiform/record_list_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)     1322 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/uiform/record_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)    84937 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/uiform/uiform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 15:57:03.095363 appian-locust-2.9.0a0/appian_locust/utilities/
+-rw-rw-rw-   0 root         (0) root         (0)      145 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/utilities/credentials.py
+-rw-rw-rw-   0 root         (0) root         (0)    17411 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/utilities/helper.py
+-rwxrwxrwx   0 root         (0) root         (0)     1393 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/utilities/loadDriverUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/utilities/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)    20139 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/appian_locust/visitor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 15:57:03.091364 appian-locust-2.9.0a0/appian_locust.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5113 2024-01-09 15:57:03.000000 appian-locust-2.9.0a0/appian_locust.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2035 2024-01-09 15:57:03.000000 appian-locust-2.9.0a0/appian_locust.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-09 15:57:03.000000 appian-locust-2.9.0a0/appian_locust.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-01-09 15:57:03.000000 appian-locust-2.9.0a0/appian_locust.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-01-09 15:57:03.000000 appian-locust-2.9.0a0/appian_locust.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      595 2024-01-09 15:57:03.096363 appian-locust-2.9.0a0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-01-09 15:56:53.000000 appian-locust-2.9.0a0/setup.py
```

### Comparing `appian-locust-2.9.0/LICENSE` & `appian-locust-2.9.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/PKG-INFO` & `appian-locust-2.9.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appian-locust
-Version: 2.9.0
+Version: 2.9.0a0
 Summary: Tools and functions to make testing Appian with Locust easier
 Home-page: https://gitlab.com/appian-oss/appian-locust
 Author: Appian Performance & Reliability Engineering Squad
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `appian-locust-2.9.0/README.rst` & `appian-locust-2.9.0a0/README.rst`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/_actions.py` & `appian-locust-2.9.0a0/appian_locust/_actions.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/_admin.py` & `appian-locust-2.9.0a0/appian_locust/_admin.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/_base.py` & `appian-locust-2.9.0a0/appian_locust/_base.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/_data_fabric.py` & `appian-locust-2.9.0a0/appian_locust/_data_fabric.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/_design.py` & `appian-locust-2.9.0a0/appian_locust/_design.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/_feature_toggle_helper.py` & `appian-locust-2.9.0a0/appian_locust/_feature_toggle_helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/_grid_interactor.py` & `appian-locust-2.9.0a0/appian_locust/_grid_interactor.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/_interactor.py` & `appian-locust-2.9.0a0/appian_locust/_interactor.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/_locust_error_handler.py` & `appian-locust-2.9.0a0/appian_locust/_locust_error_handler.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/_news.py` & `appian-locust-2.9.0a0/appian_locust/_news.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/_portals.py` & `appian-locust-2.9.0a0/appian_locust/_portals.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/_rdo_interactor.py` & `appian-locust-2.9.0a0/appian_locust/_rdo_interactor.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/_records.py` & `appian-locust-2.9.0a0/appian_locust/_records.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/_records_helper.py` & `appian-locust-2.9.0a0/appian_locust/_records_helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/_reports.py` & `appian-locust-2.9.0a0/appian_locust/_reports.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/_save_request_builder.py` & `appian-locust-2.9.0a0/appian_locust/_save_request_builder.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/_sites.py` & `appian-locust-2.9.0a0/appian_locust/_sites.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/_task_opener.py` & `appian-locust-2.9.0a0/appian_locust/_task_opener.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/_tasks.py` & `appian-locust-2.9.0a0/appian_locust/_tasks.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/_ui_reconciler.py` & `appian-locust-2.9.0a0/appian_locust/_ui_reconciler.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/appian_client.py` & `appian-locust-2.9.0a0/appian_locust/appian_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         )
 
         headers = self._interactor.setup_request_headers(logout_uri)
         if hasattr(greenlet.getcurrent(), "minimal_ident"):
             log.info(f"Logging out user {self._interactor.auth[0]} from greenlet id {greenlet.getcurrent().minimal_ident}")
         else:
             log.info(f"Logging out user {self._interactor.auth[0]} from {greenlet.getcurrent()}")
-        self._interactor.post_page(logout_uri, headers=headers, label="Logout.LoadUi", raise_error=False, check_login=False)
+        self._interactor.post_page(logout_uri, headers=headers, label="Logout.LoadUi", raise_error=False)
         self.client.cookies.clear()
 
     def get_client_feature_toggles(self) -> None:
         self.client.feature_flag, self.client.feature_flag_extended = ("7ffceebc", "1bff7f49dc1fffceebc") if self.portals_mode else (
             get_client_feature_toggles(self._interactor, self.client)
         )
```

### Comparing `appian-locust-2.9.0/appian_locust/appian_task_set.py` & `appian-locust-2.9.0a0/appian_locust/appian_task_set.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/exceptions/exceptions.py` & `appian-locust-2.9.0a0/appian_locust/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/feature_flag.py` & `appian-locust-2.9.0a0/appian_locust/feature_flag.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/info/actions_info.py` & `appian-locust-2.9.0a0/appian_locust/info/actions_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/info/news_info.py` & `appian-locust-2.9.0a0/appian_locust/info/news_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/info/records_info.py` & `appian-locust-2.9.0a0/appian_locust/info/records_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/info/reports_info.py` & `appian-locust-2.9.0a0/appian_locust/info/reports_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/info/sites_info.py` & `appian-locust-2.9.0a0/appian_locust/info/sites_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/info/tasks_info.py` & `appian-locust-2.9.0a0/appian_locust/info/tasks_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/objects/design_object.py` & `appian-locust-2.9.0a0/appian_locust/objects/design_object.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/objects/page.py` & `appian-locust-2.9.0a0/appian_locust/objects/page.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/system_operator.py` & `appian-locust-2.9.0a0/appian_locust/system_operator.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/uiform/ai_skill_uiform.py` & `appian-locust-2.9.0a0/appian_locust/uiform/ai_skill_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/uiform/application_uiform.py` & `appian-locust-2.9.0a0/appian_locust/uiform/application_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/uiform/design_object_uiform.py` & `appian-locust-2.9.0a0/appian_locust/uiform/design_object_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/uiform/design_uiform.py` & `appian-locust-2.9.0a0/appian_locust/uiform/design_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/uiform/record_list_uiform.py` & `appian-locust-2.9.0a0/appian_locust/uiform/record_list_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/uiform/record_uiform.py` & `appian-locust-2.9.0a0/appian_locust/uiform/record_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/uiform/uiform.py` & `appian-locust-2.9.0a0/appian_locust/uiform/uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/utilities/credentials.py` & `appian-locust-2.9.0a0/appian_locust/utilities/credentials.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/utilities/helper.py` & `appian-locust-2.9.0a0/appian_locust/utilities/helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/utilities/loadDriverUtils.py` & `appian-locust-2.9.0a0/appian_locust/utilities/loadDriverUtils.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/utilities/logger.py` & `appian-locust-2.9.0a0/appian_locust/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust/visitor.py` & `appian-locust-2.9.0a0/appian_locust/visitor.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/appian_locust.egg-info/PKG-INFO` & `appian-locust-2.9.0a0/appian_locust.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appian-locust
-Version: 2.9.0
+Version: 2.9.0a0
 Summary: Tools and functions to make testing Appian with Locust easier
 Home-page: https://gitlab.com/appian-oss/appian-locust
 Author: Appian Performance & Reliability Engineering Squad
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `appian-locust-2.9.0/appian_locust.egg-info/SOURCES.txt` & `appian-locust-2.9.0a0/appian_locust.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/setup.cfg` & `appian-locust-2.9.0a0/setup.cfg`

 * *Files identical despite different names*

### Comparing `appian-locust-2.9.0/setup.py` & `appian-locust-2.9.0a0/setup.py`

 * *Files identical despite different names*


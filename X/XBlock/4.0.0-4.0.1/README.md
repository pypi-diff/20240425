# Comparing `tmp/XBlock-4.0.0.tar.gz` & `tmp/XBlock-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XBlock-4.0.0.tar", last modified: Fri Apr 19 13:41:59 2024, max compression
+gzip compressed data, was "XBlock-4.0.1.tar", last modified: Thu Apr 25 06:49:31 2024, max compression
```

## Comparing `XBlock-4.0.0.tar` & `XBlock-4.0.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:41:59.147510 XBlock-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-19 13:41:57.000000 XBlock-4.0.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-19 13:41:57.000000 XBlock-4.0.0/LICENSE.TXT
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-19 13:41:57.000000 XBlock-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-19 13:41:57.000000 XBlock-4.0.0/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-19 13:41:59.147510 XBlock-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-19 13:41:57.000000 XBlock-4.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:41:59.139510 XBlock-4.0.0/XBlock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-19 13:41:58.000000 XBlock-4.0.0/XBlock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-19 13:41:59.000000 XBlock-4.0.0/XBlock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:41:58.000000 XBlock-4.0.0/XBlock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-19 13:41:58.000000 XBlock-4.0.0/XBlock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 13:41:58.000000 XBlock-4.0.0/XBlock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-19 13:41:59.147510 XBlock-4.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2098 2024-04-19 13:41:57.000000 XBlock-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:41:59.143510 XBlock-4.0.0/xblock/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/completable.py
--rw-r--r--   0 runner    (1001) docker     (127)    37579 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:41:59.143510 XBlock-4.0.0/xblock/django/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/django/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/field_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    39181 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/fragment.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6676 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:41:59.143510 XBlock-4.0.0/xblock/reference/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/reference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/reference/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/reference/user_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/run_script.py
--rw-r--r--   0 runner    (1001) docker     (127)    48451 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/scorable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:41:59.147510 XBlock-4.0.0/xblock/test/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:41:59.147510 XBlock-4.0.0/xblock/test/django/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/django/test_field_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/django/test_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:41:59.139510 XBlock-4.0.0/xblock/test/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:41:59.139510 XBlock-4.0.0/xblock/test/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:41:59.147510 XBlock-4.0.0/xblock/test/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/test_asides.py
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/test_completable.py
--rw-r--r--   0 runner    (1001) docker     (127)    43488 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/test_core_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/test_field_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    31443 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    18963 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/test_fields_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/test_fragment.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/test_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/test_json_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    17603 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    27535 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/test_scorable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/test_test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/test_user_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/toy_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:41:59.147510 XBlock-4.0.0/xblock/test/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:41:59.139510 XBlock-4.0.0/xblock/test/utils/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:41:59.139510 XBlock-4.0.0/xblock/test/utils/data/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:41:59.139510 XBlock-4.0.0/xblock/test/utils/data/translations/eo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:41:59.147510 XBlock-4.0.0/xblock/test/utils/data/translations/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/utils/data/translations/eo/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/utils/data/translations/eo/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/utils/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/utils/test_publish_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/utils/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/test/utils/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:41:59.147510 XBlock-4.0.0/xblock/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/utils/publish_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/utils/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    22298 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/utils/studio_editable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-19 13:41:57.000000 XBlock-4.0.0/xblock/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:49:31.095775 XBlock-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-25 06:49:29.000000 XBlock-4.0.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-25 06:49:29.000000 XBlock-4.0.1/LICENSE.TXT
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 06:49:29.000000 XBlock-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-25 06:49:29.000000 XBlock-4.0.1/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-25 06:49:31.095775 XBlock-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-25 06:49:29.000000 XBlock-4.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:49:31.087775 XBlock-4.0.1/XBlock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-25 06:49:31.000000 XBlock-4.0.1/XBlock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-25 06:49:31.000000 XBlock-4.0.1/XBlock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 06:49:31.000000 XBlock-4.0.1/XBlock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-25 06:49:31.000000 XBlock-4.0.1/XBlock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 06:49:31.000000 XBlock-4.0.1/XBlock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-25 06:49:31.095775 XBlock-4.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2098 2024-04-25 06:49:29.000000 XBlock-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:49:31.087775 XBlock-4.0.1/xblock/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/completable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37579 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:49:31.087775 XBlock-4.0.1/xblock/django/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/django/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/field_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39181 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/fragment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6676 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:49:31.091775 XBlock-4.0.1/xblock/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/reference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/reference/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/reference/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/run_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48451 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/scorable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:49:31.091775 XBlock-4.0.1/xblock/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:49:31.091775 XBlock-4.0.1/xblock/test/django/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/django/test_field_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/django/test_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:49:31.083775 XBlock-4.0.1/xblock/test/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:49:31.083775 XBlock-4.0.1/xblock/test/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:49:31.091775 XBlock-4.0.1/xblock/test/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/test_asides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/test_completable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43488 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/test_core_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/test_field_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31443 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18963 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/test_fields_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/test_fragment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/test_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/test_json_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17603 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27535 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/test_scorable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/test_test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/test_user_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/toy_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:49:31.095775 XBlock-4.0.1/xblock/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:49:31.087775 XBlock-4.0.1/xblock/test/utils/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:49:31.087775 XBlock-4.0.1/xblock/test/utils/data/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:49:31.087775 XBlock-4.0.1/xblock/test/utils/data/translations/eo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:49:31.095775 XBlock-4.0.1/xblock/test/utils/data/translations/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/utils/data/translations/eo/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/utils/data/translations/eo/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/utils/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/utils/test_publish_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/utils/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/test/utils/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:49:31.095775 XBlock-4.0.1/xblock/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/utils/publish_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/utils/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22298 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/utils/studio_editable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-25 06:49:29.000000 XBlock-4.0.1/xblock/validation.py
```

### Comparing `XBlock-4.0.0/AUTHORS` & `XBlock-4.0.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/LICENSE.TXT` & `XBlock-4.0.1/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/NOTICE.txt` & `XBlock-4.0.1/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/PKG-INFO` & `XBlock-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XBlock
-Version: 4.0.0
+Version: 4.0.1
 Summary: XBlock Core Library
 Home-page: https://github.com/openedx/XBlock
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `XBlock-4.0.0/README.rst` & `XBlock-4.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/XBlock.egg-info/PKG-INFO` & `XBlock-4.0.1/XBlock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XBlock
-Version: 4.0.0
+Version: 4.0.1
 Summary: XBlock Core Library
 Home-page: https://github.com/openedx/XBlock
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `XBlock-4.0.0/XBlock.egg-info/SOURCES.txt` & `XBlock-4.0.1/XBlock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/setup.py` & `XBlock-4.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/completable.py` & `XBlock-4.0.1/xblock/completable.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/core.py` & `XBlock-4.0.1/xblock/core.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/django/request.py` & `XBlock-4.0.1/xblock/django/request.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/exceptions.py` & `XBlock-4.0.1/xblock/exceptions.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/field_data.py` & `XBlock-4.0.1/xblock/field_data.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/fields.py` & `XBlock-4.0.1/xblock/fields.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/fragment.py` & `XBlock-4.0.1/xblock/fragment.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/internal.py` & `XBlock-4.0.1/xblock/internal.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/plugin.py` & `XBlock-4.0.1/xblock/plugin.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/reference/plugins.py` & `XBlock-4.0.1/xblock/reference/plugins.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/reference/user_service.py` & `XBlock-4.0.1/xblock/reference/user_service.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/runtime.py` & `XBlock-4.0.1/xblock/runtime.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/scorable.py` & `XBlock-4.0.1/xblock/scorable.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/django/test_field_translation.py` & `XBlock-4.0.1/xblock/test/django/test_field_translation.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/django/test_request.py` & `XBlock-4.0.1/xblock/test/django/test_request.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/locale/de/LC_MESSAGES/django.po` & `XBlock-4.0.1/xblock/test/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/settings.py` & `XBlock-4.0.1/xblock/test/settings.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/test_asides.py` & `XBlock-4.0.1/xblock/test/test_asides.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/test_completable.py` & `XBlock-4.0.1/xblock/test/test_completable.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/test_core.py` & `XBlock-4.0.1/xblock/test/test_core.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/test_core_capabilities.py` & `XBlock-4.0.1/xblock/test/test_core_capabilities.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/test_field_data.py` & `XBlock-4.0.1/xblock/test/test_field_data.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/test_fields.py` & `XBlock-4.0.1/xblock/test/test_fields.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/test_fields_api.py` & `XBlock-4.0.1/xblock/test/test_fields_api.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/test_fragment.py` & `XBlock-4.0.1/xblock/test/test_fragment.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/test_internal.py` & `XBlock-4.0.1/xblock/test/test_internal.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/test_json_conversion.py` & `XBlock-4.0.1/xblock/test/test_json_conversion.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/test_parsing.py` & `XBlock-4.0.1/xblock/test/test_parsing.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/test_plugin.py` & `XBlock-4.0.1/xblock/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/test_runtime.py` & `XBlock-4.0.1/xblock/test/test_runtime.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/test_scorable.py` & `XBlock-4.0.1/xblock/test/test_scorable.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/test_test_tools.py` & `XBlock-4.0.1/xblock/test/test_test_tools.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/test_user_service.py` & `XBlock-4.0.1/xblock/test/test_user_service.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/test_validation.py` & `XBlock-4.0.1/xblock/test/test_validation.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/tools.py` & `XBlock-4.0.1/xblock/test/tools.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/toy_runtime.py` & `XBlock-4.0.1/xblock/test/toy_runtime.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/utils/data/translations/eo/LC_MESSAGES/text.po` & `XBlock-4.0.1/xblock/test/utils/data/translations/eo/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/utils/test_helpers.py` & `XBlock-4.0.1/xblock/test/utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/utils/test_publish_event.py` & `XBlock-4.0.1/xblock/test/utils/test_publish_event.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/utils/test_resources.py` & `XBlock-4.0.1/xblock/test/utils/test_resources.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/test/utils/test_settings.py` & `XBlock-4.0.1/xblock/test/utils/test_settings.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/utils/helpers.py` & `XBlock-4.0.1/xblock/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/utils/publish_event.py` & `XBlock-4.0.1/xblock/utils/publish_event.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/utils/resources.py` & `XBlock-4.0.1/xblock/utils/resources.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/utils/settings.py` & `XBlock-4.0.1/xblock/utils/settings.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/utils/studio_editable.py` & `XBlock-4.0.1/xblock/utils/studio_editable.py`

 * *Files identical despite different names*

### Comparing `XBlock-4.0.0/xblock/validation.py` & `XBlock-4.0.1/xblock/validation.py`

 * *Files identical despite different names*


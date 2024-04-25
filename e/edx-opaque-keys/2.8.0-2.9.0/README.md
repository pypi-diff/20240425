# Comparing `tmp/edx-opaque-keys-2.8.0.tar.gz` & `tmp/edx_opaque_keys-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-opaque-keys-2.8.0.tar", last modified: Mon Apr 22 13:58:35 2024, max compression
+gzip compressed data, was "edx_opaque_keys-2.9.0.tar", last modified: Thu Apr 25 12:32:02 2024, max compression
```

## Comparing `edx-opaque-keys-2.8.0.tar` & `edx_opaque_keys-2.9.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:58:35.984694 edx-opaque-keys-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34499 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-22 13:58:35.984694 edx-opaque-keys-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:58:35.984694 edx-opaque-keys-2.8.0/edx_opaque_keys.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-22 13:58:35.000000 edx-opaque-keys-2.8.0/edx_opaque_keys.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-22 13:58:35.000000 edx-opaque-keys-2.8.0/edx_opaque_keys.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 13:58:35.000000 edx-opaque-keys-2.8.0/edx_opaque_keys.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-22 13:58:35.000000 edx-opaque-keys-2.8.0/edx_opaque_keys.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-22 13:58:35.000000 edx-opaque-keys-2.8.0/edx_opaque_keys.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 13:58:35.000000 edx-opaque-keys-2.8.0/edx_opaque_keys.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:58:35.976694 edx-opaque-keys-2.8.0/opaque_keys/
--rw-r--r--   0 runner    (1001) docker     (127)    15106 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:58:35.980694 edx-opaque-keys-2.8.0/opaque_keys/edx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/edx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/edx/asides.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/edx/block_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:58:35.980694 edx-opaque-keys-2.8.0/opaque_keys/edx/django/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/edx/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/edx/django/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:58:35.980694 edx-opaque-keys-2.8.0/opaque_keys/edx/django/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/edx/django/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/edx/django/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/edx/django/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/edx/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     9935 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/edx/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)    61345 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/edx/locator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:58:35.980694 edx-opaque-keys-2.8.0/opaque_keys/edx/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/edx/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/edx/tests/test_aside_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/edx/tests/test_asset_locators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/edx/tests/test_block_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    14989 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/edx/tests/test_block_usage_locators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/edx/tests/test_course_locators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/edx/tests/test_default_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/edx/tests/test_deprecated_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/edx/tests/test_is_course.py
--rw-r--r--   0 runner    (1001) docker     (127)    12203 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/edx/tests/test_library_locators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10268 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/edx/tests/test_library_usage_locators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/edx/tests/test_locators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/edx/tests/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:58:35.984694 edx-opaque-keys-2.8.0/opaque_keys/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12411 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)     9796 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/opaque_keys/tests/test_opaque_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:58:35.984694 edx-opaque-keys-2.8.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/requirements/django.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:58:35.984694 edx-opaque-keys-2.8.0/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/settings/test.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 13:58:35.984694 edx-opaque-keys-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-04-22 13:58:31.000000 edx-opaque-keys-2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:32:02.756558 edx_opaque_keys-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34499 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-25 12:32:02.756558 edx_opaque_keys-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:32:02.756558 edx_opaque_keys-2.9.0/edx_opaque_keys.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-25 12:32:02.000000 edx_opaque_keys-2.9.0/edx_opaque_keys.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-25 12:32:02.000000 edx_opaque_keys-2.9.0/edx_opaque_keys.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 12:32:02.000000 edx_opaque_keys-2.9.0/edx_opaque_keys.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-25 12:32:02.000000 edx_opaque_keys-2.9.0/edx_opaque_keys.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-25 12:32:02.000000 edx_opaque_keys-2.9.0/edx_opaque_keys.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 12:32:02.000000 edx_opaque_keys-2.9.0/edx_opaque_keys.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:32:02.748558 edx_opaque_keys-2.9.0/opaque_keys/
+-rw-r--r--   0 runner    (1001) docker     (127)    15106 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:32:02.752558 edx_opaque_keys-2.9.0/opaque_keys/edx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/edx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/edx/asides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/edx/block_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:32:02.752558 edx_opaque_keys-2.9.0/opaque_keys/edx/django/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/edx/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/edx/django/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:32:02.752558 edx_opaque_keys-2.9.0/opaque_keys/edx/django/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/edx/django/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/edx/django/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/edx/django/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/edx/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9935 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/edx/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61379 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/edx/locator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:32:02.752558 edx_opaque_keys-2.9.0/opaque_keys/edx/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/edx/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/edx/tests/test_aside_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/edx/tests/test_asset_locators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/edx/tests/test_block_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14995 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/edx/tests/test_block_usage_locators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/edx/tests/test_course_locators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/edx/tests/test_default_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/edx/tests/test_deprecated_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/edx/tests/test_is_course.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12203 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/edx/tests/test_library_locators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10268 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/edx/tests/test_library_usage_locators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/edx/tests/test_locators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/edx/tests/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:32:02.752558 edx_opaque_keys-2.9.0/opaque_keys/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12411 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9796 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/opaque_keys/tests/test_opaque_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:32:02.752558 edx_opaque_keys-2.9.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/requirements/django.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:32:02.756558 edx_opaque_keys-2.9.0/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/settings/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 12:32:02.756558 edx_opaque_keys-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-04-25 12:31:59.000000 edx_opaque_keys-2.9.0/setup.py
```

### Comparing `edx-opaque-keys-2.8.0/CHANGELOG.rst` & `edx_opaque_keys-2.9.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# 2.9.0
+
+* Upgrade pymongo to 4.4. It contains few breaking changes.
+
 # 2.6.0
 
 * Added support for python 3.12
 * Dropped support for django 3.2
 
 
 # 2.5.1
```

### Comparing `edx-opaque-keys-2.8.0/LICENSE` & `edx_opaque_keys-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/PKG-INFO` & `edx_opaque_keys-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-opaque-keys
-Version: 2.8.0
+Version: 2.9.0
 Home-page: https://github.com/openedx/opaque-keys
 Author: edX
 License: AGPL-3.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: pymongo<4.0,>=2.7.2
+Requires-Dist: pymongo<4.4.1,>=2.7.2
 Requires-Dist: stevedore>=0.14.1
 Requires-Dist: typing-extensions
 Provides-Extra: django
 
 Part of `edX code`_.
 
 .. _`edX code`: http://code.edx.org/
```

### Comparing `edx-opaque-keys-2.8.0/README.rst` & `edx_opaque_keys-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/edx_opaque_keys.egg-info/PKG-INFO` & `edx_opaque_keys-2.9.0/edx_opaque_keys.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-opaque-keys
-Version: 2.8.0
+Version: 2.9.0
 Home-page: https://github.com/openedx/opaque-keys
 Author: edX
 License: AGPL-3.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: pymongo<4.0,>=2.7.2
+Requires-Dist: pymongo<4.4.1,>=2.7.2
 Requires-Dist: stevedore>=0.14.1
 Requires-Dist: typing-extensions
 Provides-Extra: django
 
 Part of `edX code`_.
 
 .. _`edX code`: http://code.edx.org/
```

### Comparing `edx-opaque-keys-2.8.0/edx_opaque_keys.egg-info/SOURCES.txt` & `edx_opaque_keys-2.9.0/edx_opaque_keys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/edx_opaque_keys.egg-info/entry_points.txt` & `edx_opaque_keys-2.9.0/edx_opaque_keys.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/opaque_keys/__init__.py` & `edx_opaque_keys-2.9.0/opaque_keys/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from abc import ABCMeta, abstractmethod
 from collections import defaultdict
 from functools import total_ordering
 
 from stevedore.enabled import EnabledExtensionManager
 from typing_extensions import Self  # For python 3.11 plus, can just use "from typing import Self"
 
-__version__ = '2.8.0'
+__version__ = '2.9.0'
 
 
 class InvalidKeyError(Exception):
     """
     Raised to indicated that a serialized key isn't valid (wasn't able to be parsed
     by any available providers).
     """
```

### Comparing `edx-opaque-keys-2.8.0/opaque_keys/edx/asides.py` & `edx_opaque_keys-2.9.0/opaque_keys/edx/asides.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/opaque_keys/edx/block_types.py` & `edx_opaque_keys-2.9.0/opaque_keys/edx/block_types.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/opaque_keys/edx/django/models.py` & `edx_opaque_keys-2.9.0/opaque_keys/edx/django/models.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/opaque_keys/edx/django/tests/models.py` & `edx_opaque_keys-2.9.0/opaque_keys/edx/django/tests/models.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/opaque_keys/edx/django/tests/test_models.py` & `edx_opaque_keys-2.9.0/opaque_keys/edx/django/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/opaque_keys/edx/keys.py` & `edx_opaque_keys-2.9.0/opaque_keys/edx/keys.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/opaque_keys/edx/locations.py` & `edx_opaque_keys-2.9.0/opaque_keys/edx/locations.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/opaque_keys/edx/locator.py` & `edx_opaque_keys-2.9.0/opaque_keys/edx/locator.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
         expects to find. Equivalent to version_guid.
         """
         warnings.warn(
             "version is no longer supported as a property of Locators. Please use the version_guid property.",
             DeprecationWarning,
             stacklevel=2
         )
-        return self.version_guid
+        return self.version_guid    # type: ignore
 
     @property
     def offering(self):
         """
         Deprecated. Use course and run independently.
         """
         warnings.warn(
@@ -470,15 +470,15 @@
             library = kwargs.pop('course')
 
         run = kwargs.pop('run', self.RUN)
         if run != self.RUN:
             raise ValueError(f"Invalid run. Should be '{self.RUN}' or None.")
 
         if version_guid:
-            version_guid = self.as_object_id(version_guid)
+            version_guid = self.as_object_id(version_guid)  # type: ignore
 
         for name, value in [['org', org], ['library', library], ['branch', branch]]:
             if not (value is None or self.ALLOWED_ID_RE.match(value)):
                 raise InvalidKeyError(self.__class__,
                                       f"Special characters not allowed in field {name}: '{value}'")
 
         if kwargs.get('deprecated', False):
```

### Comparing `edx-opaque-keys-2.8.0/opaque_keys/edx/tests/__init__.py` & `edx_opaque_keys-2.9.0/opaque_keys/edx/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/opaque_keys/edx/tests/test_aside_keys.py` & `edx_opaque_keys-2.9.0/opaque_keys/edx/tests/test_aside_keys.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/opaque_keys/edx/tests/test_asset_locators.py` & `edx_opaque_keys-2.9.0/opaque_keys/edx/tests/test_asset_locators.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         (AssetLocator, '_id.', 'c4x', (CourseLocator('org', 'course', 'run', 'rev', deprecated=True), 'ct', None)),
     )
     @ddt.unpack
     def test_deprecated_son(self, key_cls, prefix, tag, source):
         source_key = key_cls(*source, deprecated=True)
         son = source_key.to_deprecated_son(prefix=prefix, tag=tag)
         self.assertEqual(
-            son.keys(),
+            list(son.keys()),
             [prefix + key for key in ('tag', 'org', 'course', 'category', 'name', 'revision')]
         )
 
         self.assertEqual(son[prefix + 'tag'], tag)
         self.assertEqual(son[prefix + 'category'], source_key.block_type)
         self.assertEqual(son[prefix + 'name'], source_key.block_id)
```

### Comparing `edx-opaque-keys-2.8.0/opaque_keys/edx/tests/test_block_types.py` & `edx_opaque_keys-2.9.0/opaque_keys/edx/tests/test_block_types.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/opaque_keys/edx/tests/test_block_usage_locators.py` & `edx_opaque_keys-2.9.0/opaque_keys/edx/tests/test_block_usage_locators.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,15 +201,15 @@
         (BlockUsageLocator, '_id.', 'i4x', (CourseLocator('org', 'course', 'run', 'rev', deprecated=True), 'ct', 'n')),
         (BlockUsageLocator, '', 'i4x', (CourseLocator('org', 'course', 'run', 'rev', deprecated=True), 'ct', 'n')),
     )
     @ddt.unpack
     def test_to_deprecated_son(self, key_cls, prefix, tag, source):
         source_key = key_cls(*source, deprecated=True)
         son = source_key.to_deprecated_son(prefix=prefix, tag=tag)
-        self.assertEqual(son.keys(),
+        self.assertEqual(list(son.keys()),
                          [prefix + key for key in ('tag', 'org', 'course', 'category', 'name', 'revision')])
 
         self.assertEqual(son[prefix + 'tag'], tag)
         self.assertEqual(son[prefix + 'org'], source_key.course_key.org)
         self.assertEqual(son[prefix + 'course'], source_key.course_key.course)
         self.assertEqual(son[prefix + 'category'], source_key.block_type)
         self.assertEqual(son[prefix + 'name'], source_key.block_id)
```

### Comparing `edx-opaque-keys-2.8.0/opaque_keys/edx/tests/test_course_locators.py` & `edx_opaque_keys-2.9.0/opaque_keys/edx/tests/test_course_locators.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/opaque_keys/edx/tests/test_default_deprecated.py` & `edx_opaque_keys-2.9.0/opaque_keys/edx/tests/test_default_deprecated.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/opaque_keys/edx/tests/test_deprecated_locations.py` & `edx_opaque_keys-2.9.0/opaque_keys/edx/tests/test_deprecated_locations.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/opaque_keys/edx/tests/test_is_course.py` & `edx_opaque_keys-2.9.0/opaque_keys/edx/tests/test_is_course.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/opaque_keys/edx/tests/test_library_locators.py` & `edx_opaque_keys-2.9.0/opaque_keys/edx/tests/test_library_locators.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/opaque_keys/edx/tests/test_library_usage_locators.py` & `edx_opaque_keys-2.9.0/opaque_keys/edx/tests/test_library_usage_locators.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/opaque_keys/edx/tests/test_locators.py` & `edx_opaque_keys-2.9.0/opaque_keys/edx/tests/test_locators.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/opaque_keys/edx/tests/test_properties.py` & `edx_opaque_keys-2.9.0/opaque_keys/edx/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/opaque_keys/tests/strategies.py` & `edx_opaque_keys-2.9.0/opaque_keys/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/opaque_keys/tests/test_opaque_keys.py` & `edx_opaque_keys-2.9.0/opaque_keys/tests/test_opaque_keys.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/settings/base.py` & `edx_opaque_keys-2.9.0/settings/base.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.8.0/setup.py` & `edx_opaque_keys-2.9.0/setup.py`

 * *Files identical despite different names*


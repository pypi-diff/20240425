# Comparing `tmp/ckanext_collection-0.1.2.tar.gz` & `tmp/ckanext_collection-0.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext_collection-0.1.2.tar", last modified: Mon Apr 22 16:00:51 2024, max compression
+gzip compressed data, was "ckanext_collection-0.1.21.tar", last modified: Thu Apr 25 09:42:45 2024, max compression
```

## Comparing `ckanext_collection-0.1.2.tar` & `ckanext_collection-0.1.21.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-22 16:00:51.438549 ckanext_collection-0.1.2/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2024-01-15 13:59:08.000000 ckanext_collection-0.1.2/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      212 2024-01-15 13:59:08.000000 ckanext_collection-0.1.2/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)    29646 2024-04-22 16:00:51.438549 ckanext_collection-0.1.2/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)    28729 2024-03-03 13:26:30.000000 ckanext_collection-0.1.2/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-22 16:00:51.431882 ckanext_collection-0.1.2/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      202 2024-01-15 13:59:08.000000 ckanext_collection-0.1.2/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-22 16:00:51.431882 ckanext_collection-0.1.2/ckanext/collection/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-15 13:59:08.000000 ckanext_collection-0.1.2/ckanext/collection/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      625 2024-01-28 01:35:15.000000 ckanext_collection-0.1.2/ckanext/collection/ap_config.yaml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-22 16:00:51.431882 ckanext_collection-0.1.2/ckanext/collection/assets/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-22 16:00:51.431882 ckanext_collection-0.1.2/ckanext/collection/assets/js/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      315 2024-01-24 19:39:40.000000 ckanext_collection-0.1.2/ckanext/collection/assets/js/htmx-init-ckan-modules.js
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-22 16:00:51.431882 ckanext_collection-0.1.2/ckanext/collection/assets/vendor/
--rw-r--r--   0 sergey    (1000) sergey    (1000)   160923 2024-01-15 13:59:08.000000 ckanext_collection-0.1.2/ckanext/collection/assets/vendor/htmx.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)      283 2024-01-24 19:43:49.000000 ckanext_collection-0.1.2/ckanext/collection/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      543 2024-01-15 13:59:08.000000 ckanext_collection-0.1.2/ckanext/collection/cli.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      972 2024-01-26 16:51:55.000000 ckanext_collection-0.1.2/ckanext/collection/config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1711 2024-01-28 01:22:07.000000 ckanext_collection-0.1.2/ckanext/collection/config_declaration.yaml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      372 2024-01-24 22:27:36.000000 ckanext_collection-0.1.2/ckanext/collection/helpers.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      557 2024-01-15 13:59:08.000000 ckanext_collection-0.1.2/ckanext/collection/interfaces.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-22 16:00:51.431882 ckanext_collection-0.1.2/ckanext/collection/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-15 13:59:08.000000 ckanext_collection-0.1.2/ckanext/collection/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      730 2024-01-15 13:59:08.000000 ckanext_collection-0.1.2/ckanext/collection/logic/auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3682 2024-03-06 23:15:38.000000 ckanext_collection-0.1.2/ckanext/collection/plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7822 2024-03-03 11:24:50.000000 ckanext_collection-0.1.2/ckanext/collection/shared.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-22 16:00:51.431882 ckanext_collection-0.1.2/ckanext/collection/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-22 16:00:51.428549 ckanext_collection-0.1.2/ckanext/collection/templates/collection/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-22 16:00:51.428549 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-22 16:00:51.431882 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/collection_explorer/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       56 2024-01-27 22:45:13.000000 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/collection_explorer/main.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-22 16:00:51.431882 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/db_explorer/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       56 2024-01-27 22:45:20.000000 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/db_explorer/main.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-22 16:00:51.431882 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/explorer/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1941 2024-01-27 23:16:14.000000 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/explorer/main.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-22 16:00:51.431882 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/html/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      153 2024-01-15 13:59:08.000000 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/html/main.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      119 2024-01-24 11:45:25.000000 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/html/record.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-22 16:00:51.435216 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/htmx_table/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       56 2024-01-24 13:21:04.000000 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/htmx_table/counter.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)       55 2024-01-24 16:42:00.000000 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/htmx_table/filter.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1586 2024-01-27 12:05:44.000000 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/htmx_table/form.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)       53 2024-01-24 13:20:37.000000 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/htmx_table/main.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      892 2024-01-24 15:47:44.000000 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/htmx_table/pager.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)       55 2024-01-24 13:20:58.000000 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/htmx_table/record.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1041 2024-01-24 15:51:55.000000 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/htmx_table/table.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-22 16:00:51.435216 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/table/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      251 2024-01-15 13:59:08.000000 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/table/counter.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2203 2024-01-28 23:43:20.000000 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/table/filter.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      812 2024-01-24 19:57:38.000000 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/table/form.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      883 2024-02-27 14:00:04.000000 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/table/main.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2223 2024-02-27 14:01:07.000000 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/table/pager.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      646 2024-01-29 12:45:09.000000 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/table/record.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2333 2024-01-24 19:17:41.000000 ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/table/table.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      314 2024-01-24 19:43:40.000000 ckanext_collection-0.1.2/ckanext/collection/templates/page.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-22 16:00:51.435216 ckanext_collection-0.1.2/ckanext/collection/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-15 13:59:08.000000 ckanext_collection-0.1.2/ckanext/collection/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      232 2024-01-26 16:51:55.000000 ckanext_collection-0.1.2/ckanext/collection/tests/conftest.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      210 2024-01-15 13:59:08.000000 ckanext_collection-0.1.2/ckanext/collection/tests/test_plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4879 2024-03-03 11:25:47.000000 ckanext_collection-0.1.2/ckanext/collection/tests/test_readme.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4714 2024-01-15 13:59:08.000000 ckanext_collection-0.1.2/ckanext/collection/tests/test_shared.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-22 16:00:51.435216 ckanext_collection-0.1.2/ckanext/collection/tests/utils/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-15 13:59:08.000000 ckanext_collection-0.1.2/ckanext/collection/tests/utils/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2396 2024-01-27 23:57:34.000000 ckanext_collection-0.1.2/ckanext/collection/tests/utils/test_collection.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1150 2024-01-15 13:59:08.000000 ckanext_collection-0.1.2/ckanext/collection/tests/utils/test_columns.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7367 2024-04-22 15:57:32.000000 ckanext_collection-0.1.2/ckanext/collection/tests/utils/test_data.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      500 2024-01-15 13:59:08.000000 ckanext_collection-0.1.2/ckanext/collection/tests/utils/test_filters.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1040 2024-01-15 13:59:08.000000 ckanext_collection-0.1.2/ckanext/collection/tests/utils/test_pager.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3731 2024-02-02 15:35:30.000000 ckanext_collection-0.1.2/ckanext/collection/tests/utils/test_serializer.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5305 2024-02-01 18:23:15.000000 ckanext_collection-0.1.2/ckanext/collection/types.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-22 16:00:51.435216 ckanext_collection-0.1.2/ckanext/collection/utils/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1791 2024-01-28 01:49:08.000000 ckanext_collection-0.1.2/ckanext/collection/utils/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-22 16:00:51.435216 ckanext_collection-0.1.2/ckanext/collection/utils/collection/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      591 2024-02-01 18:20:35.000000 ckanext_collection-0.1.2/ckanext/collection/utils/collection/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      353 2024-02-01 18:18:39.000000 ckanext_collection-0.1.2/ckanext/collection/utils/collection/api.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5994 2024-02-01 18:19:44.000000 ckanext_collection-0.1.2/ckanext/collection/utils/collection/base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      842 2024-02-01 18:20:08.000000 ckanext_collection-0.1.2/ckanext/collection/utils/collection/db.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7847 2024-02-01 18:20:23.000000 ckanext_collection-0.1.2/ckanext/collection/utils/collection/explorer.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      183 2024-02-01 18:20:45.000000 ckanext_collection-0.1.2/ckanext/collection/utils/collection/model.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3228 2024-02-02 15:34:16.000000 ckanext_collection-0.1.2/ckanext/collection/utils/columns.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-22 16:00:51.435216 ckanext_collection-0.1.2/ckanext/collection/utils/data/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1044 2024-01-27 23:57:34.000000 ckanext_collection-0.1.2/ckanext/collection/utils/data/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3977 2024-01-27 01:47:32.000000 ckanext_collection-0.1.2/ckanext/collection/utils/data/api.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1548 2024-02-01 18:23:34.000000 ckanext_collection-0.1.2/ckanext/collection/utils/data/base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1082 2024-01-30 14:08:30.000000 ckanext_collection-0.1.2/ckanext/collection/utils/data/db.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9651 2024-04-22 15:57:50.000000 ckanext_collection-0.1.2/ckanext/collection/utils/data/model.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1260 2024-02-02 15:30:15.000000 ckanext_collection-0.1.2/ckanext/collection/utils/db_connection.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3538 2024-01-28 17:22:03.000000 ckanext_collection-0.1.2/ckanext/collection/utils/filters.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1310 2024-01-15 13:59:08.000000 ckanext_collection-0.1.2/ckanext/collection/utils/pager.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-22 16:00:51.435216 ckanext_collection-0.1.2/ckanext/collection/utils/serialize/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9922 2024-03-03 13:25:29.000000 ckanext_collection-0.1.2/ckanext/collection/utils/serialize/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2321 2024-02-01 14:43:13.000000 ckanext_collection-0.1.2/ckanext/collection/views.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-22 16:00:51.438549 ckanext_collection-0.1.2/ckanext_collection.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    29646 2024-04-22 16:00:51.000000 ckanext_collection-0.1.2/ckanext_collection.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3534 2024-04-22 16:00:51.000000 ckanext_collection-0.1.2/ckanext_collection.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-22 16:00:51.000000 ckanext_collection-0.1.2/ckanext_collection.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      128 2024-04-22 16:00:51.000000 ckanext_collection-0.1.2/ckanext_collection.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-04-22 16:00:51.000000 ckanext_collection-0.1.2/ckanext_collection.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       98 2024-04-22 16:00:51.000000 ckanext_collection-0.1.2/ckanext_collection.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-04-22 16:00:51.000000 ckanext_collection-0.1.2/ckanext_collection.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4256 2024-04-22 15:59:02.000000 ckanext_collection-0.1.2/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-15 13:59:08.000000 ckanext_collection-0.1.2/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1754 2024-04-22 16:00:51.438549 ckanext_collection-0.1.2/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      505 2024-01-15 13:59:08.000000 ckanext_collection-0.1.2/setup.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/
+-rw-r--r--   0 berry     (1000) berry     (1000)    34500 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/LICENSE
+-rw-r--r--   0 berry     (1000) berry     (1000)      212 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/MANIFEST.in
+-rw-r--r--   0 berry     (1000) berry     (1000)    29647 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/PKG-INFO
+-rw-r--r--   0 berry     (1000) berry     (1000)    28729 2024-04-25 09:22:49.000000 ckanext_collection-0.1.21/README.md
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/ckanext/
+-rw-r--r--   0 berry     (1000) berry     (1000)      202 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/__init__.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/ckanext/collection/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      625 2024-04-22 13:23:28.000000 ckanext_collection-0.1.21/ckanext/collection/ap_config.yaml
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/ckanext/collection/assets/
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/ckanext/collection/assets/js/
+-rw-r--r--   0 berry     (1000) berry     (1000)      315 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/assets/js/htmx-init-ckan-modules.js
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/ckanext/collection/assets/vendor/
+-rw-r--r--   0 berry     (1000) berry     (1000)   160923 2024-04-25 09:07:58.000000 ckanext_collection-0.1.21/ckanext/collection/assets/vendor/htmx.js
+-rw-r--r--   0 berry     (1000) berry     (1000)      283 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/assets/webassets.yml
+-rw-r--r--   0 berry     (1000) berry     (1000)      543 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/cli.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      972 2024-04-25 09:08:26.000000 ckanext_collection-0.1.21/ckanext/collection/config.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1711 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/config_declaration.yaml
+-rw-r--r--   0 berry     (1000) berry     (1000)      372 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/helpers.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      557 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/interfaces.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/ckanext/collection/logic/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/logic/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      730 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/logic/auth.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     3682 2024-04-22 17:58:25.000000 ckanext_collection-0.1.21/ckanext/collection/plugin.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     7822 2024-04-22 17:58:25.000000 ckanext_collection-0.1.21/ckanext/collection/shared.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/ckanext/collection/templates/
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/ckanext/collection/templates/collection/
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/collection_explorer/
+-rw-r--r--   0 berry     (1000) berry     (1000)       56 2024-04-22 13:23:21.000000 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/collection_explorer/main.html
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/db_explorer/
+-rw-r--r--   0 berry     (1000) berry     (1000)       56 2024-04-22 13:23:21.000000 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/db_explorer/main.html
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/explorer/
+-rw-r--r--   0 berry     (1000) berry     (1000)     1941 2024-04-22 13:23:21.000000 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/explorer/main.html
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/html/
+-rw-r--r--   0 berry     (1000) berry     (1000)      153 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/html/main.html
+-rw-r--r--   0 berry     (1000) berry     (1000)      119 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/html/record.html
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/htmx_table/
+-rw-r--r--   0 berry     (1000) berry     (1000)       56 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/htmx_table/counter.html
+-rw-r--r--   0 berry     (1000) berry     (1000)       55 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/htmx_table/filter.html
+-rw-r--r--   0 berry     (1000) berry     (1000)     1586 2024-04-22 18:43:51.000000 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/htmx_table/form.html
+-rw-r--r--   0 berry     (1000) berry     (1000)       53 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/htmx_table/main.html
+-rw-r--r--   0 berry     (1000) berry     (1000)      912 2024-04-25 09:24:10.000000 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/htmx_table/pager.html
+-rw-r--r--   0 berry     (1000) berry     (1000)       55 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/htmx_table/record.html
+-rw-r--r--   0 berry     (1000) berry     (1000)     1041 2024-04-25 06:15:30.000000 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/htmx_table/table.html
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/table/
+-rw-r--r--   0 berry     (1000) berry     (1000)      251 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/table/counter.html
+-rw-r--r--   0 berry     (1000) berry     (1000)     2203 2024-04-22 17:58:25.000000 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/table/filter.html
+-rw-r--r--   0 berry     (1000) berry     (1000)      812 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/table/form.html
+-rw-r--r--   0 berry     (1000) berry     (1000)      883 2024-04-22 17:58:25.000000 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/table/main.html
+-rw-r--r--   0 berry     (1000) berry     (1000)     2228 2024-04-25 09:24:10.000000 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/table/pager.html
+-rw-r--r--   0 berry     (1000) berry     (1000)      646 2024-04-22 17:58:25.000000 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/table/record.html
+-rw-r--r--   0 berry     (1000) berry     (1000)     2333 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/table/table.html
+-rw-r--r--   0 berry     (1000) berry     (1000)      314 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/templates/page.html
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/ckanext/collection/tests/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/tests/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      232 2024-04-22 13:22:52.000000 ckanext_collection-0.1.21/ckanext/collection/tests/conftest.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      210 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/tests/test_plugin.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     4879 2024-04-22 17:58:25.000000 ckanext_collection-0.1.21/ckanext/collection/tests/test_readme.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     4714 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/tests/test_shared.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/ckanext/collection/tests/utils/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/tests/utils/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     2396 2024-04-22 13:23:21.000000 ckanext_collection-0.1.21/ckanext/collection/tests/utils/test_collection.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1150 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/tests/utils/test_columns.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     7367 2024-04-25 09:22:49.000000 ckanext_collection-0.1.21/ckanext/collection/tests/utils/test_data.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      500 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/tests/utils/test_filters.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1040 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/tests/utils/test_pager.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     3731 2024-04-22 17:58:25.000000 ckanext_collection-0.1.21/ckanext/collection/tests/utils/test_serializer.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     5305 2024-04-22 17:58:25.000000 ckanext_collection-0.1.21/ckanext/collection/types.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/ckanext/collection/utils/
+-rw-r--r--   0 berry     (1000) berry     (1000)     1791 2024-04-22 13:23:28.000000 ckanext_collection-0.1.21/ckanext/collection/utils/__init__.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/ckanext/collection/utils/collection/
+-rw-r--r--   0 berry     (1000) berry     (1000)      591 2024-04-22 17:58:25.000000 ckanext_collection-0.1.21/ckanext/collection/utils/collection/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      353 2024-04-22 17:58:25.000000 ckanext_collection-0.1.21/ckanext/collection/utils/collection/api.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     5994 2024-04-22 17:58:25.000000 ckanext_collection-0.1.21/ckanext/collection/utils/collection/base.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      842 2024-04-22 17:58:25.000000 ckanext_collection-0.1.21/ckanext/collection/utils/collection/db.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     7847 2024-04-22 17:58:25.000000 ckanext_collection-0.1.21/ckanext/collection/utils/collection/explorer.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      183 2024-04-22 17:58:25.000000 ckanext_collection-0.1.21/ckanext/collection/utils/collection/model.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     3228 2024-04-22 17:58:25.000000 ckanext_collection-0.1.21/ckanext/collection/utils/columns.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/ckanext/collection/utils/data/
+-rw-r--r--   0 berry     (1000) berry     (1000)     1044 2024-04-22 13:23:21.000000 ckanext_collection-0.1.21/ckanext/collection/utils/data/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     3977 2024-04-22 13:23:11.000000 ckanext_collection-0.1.21/ckanext/collection/utils/data/api.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1548 2024-04-22 17:58:25.000000 ckanext_collection-0.1.21/ckanext/collection/utils/data/base.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1082 2024-04-22 17:58:25.000000 ckanext_collection-0.1.21/ckanext/collection/utils/data/db.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     9651 2024-04-22 17:58:25.000000 ckanext_collection-0.1.21/ckanext/collection/utils/data/model.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1260 2024-04-22 17:58:25.000000 ckanext_collection-0.1.21/ckanext/collection/utils/db_connection.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     3538 2024-04-22 17:58:25.000000 ckanext_collection-0.1.21/ckanext/collection/utils/filters.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1310 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/ckanext/collection/utils/pager.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/ckanext/collection/utils/serialize/
+-rw-r--r--   0 berry     (1000) berry     (1000)     9922 2024-04-22 17:58:25.000000 ckanext_collection-0.1.21/ckanext/collection/utils/serialize/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     2321 2024-04-22 17:58:25.000000 ckanext_collection-0.1.21/ckanext/collection/views.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/ckanext_collection.egg-info/
+-rw-r--r--   0 berry     (1000) berry     (1000)    29647 2024-04-25 09:42:45.000000 ckanext_collection-0.1.21/ckanext_collection.egg-info/PKG-INFO
+-rw-r--r--   0 berry     (1000) berry     (1000)     3534 2024-04-25 09:42:45.000000 ckanext_collection-0.1.21/ckanext_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)        1 2024-04-25 09:42:45.000000 ckanext_collection-0.1.21/ckanext_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)      128 2024-04-25 09:42:45.000000 ckanext_collection-0.1.21/ckanext_collection.egg-info/entry_points.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)        8 2024-04-25 09:42:45.000000 ckanext_collection-0.1.21/ckanext_collection.egg-info/namespace_packages.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)       98 2024-04-25 09:42:45.000000 ckanext_collection-0.1.21/ckanext_collection.egg-info/requires.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)        8 2024-04-25 09:42:45.000000 ckanext_collection-0.1.21/ckanext_collection.egg-info/top_level.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)     4256 2024-04-25 09:22:49.000000 ckanext_collection-0.1.21/pyproject.toml
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/requirements.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)     1755 2024-04-25 09:42:45.715155 ckanext_collection-0.1.21/setup.cfg
+-rw-r--r--   0 berry     (1000) berry     (1000)      505 2024-04-18 11:38:00.000000 ckanext_collection-0.1.21/setup.py
```

### Comparing `ckanext_collection-0.1.2/LICENSE` & `ckanext_collection-0.1.21/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/PKG-INFO` & `ckanext_collection-0.1.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-collection
-Version: 0.1.2
+Version: 0.1.21
 Home-page: https://github.com/DataShades/ckanext-collection
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext_collection-0.1.2/README.md` & `ckanext_collection-0.1.21/README.md`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/ap_config.yaml` & `ckanext_collection-0.1.21/ckanext/collection/ap_config.yaml`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/assets/vendor/htmx.js` & `ckanext_collection-0.1.21/ckanext/collection/assets/vendor/htmx.js`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/cli.py` & `ckanext_collection-0.1.21/ckanext/collection/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/config.py` & `ckanext_collection-0.1.21/ckanext/collection/config.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/config_declaration.yaml` & `ckanext_collection-0.1.21/ckanext/collection/config_declaration.yaml`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/interfaces.py` & `ckanext_collection-0.1.21/ckanext/collection/interfaces.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/logic/auth.py` & `ckanext_collection-0.1.21/ckanext/collection/logic/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/plugin.py` & `ckanext_collection-0.1.21/ckanext/collection/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/shared.py` & `ckanext_collection-0.1.21/ckanext/collection/shared.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/explorer/main.html` & `ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/explorer/main.html`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/htmx_table/form.html` & `ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/htmx_table/form.html`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/htmx_table/pager.html` & `ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/htmx_table/pager.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 {% extends "collection/serialize/table/pager.html" %}
 
 {% set form_id = collection.serializer.form_id %}
 
 {% block prev_page_link %}
-    <button class="pagination--switch-button" name="{{ collection.name }}:page" form="{{ form_id }}"
+    <button class="pagination--switch-button btn" name="{{ collection.name }}:page" form="{{ form_id }}"
             type="submit" value="{{ prev_page_number }}"
             {% if current_page_number == 1 %} disabled{% endif %}
     >
         {% block prev_page %}
             <span>&larr;</span>
         {% endblock prev_page %}
     </button>
 {% endblock prev_page_link %}
 
 {% block next_page_link %}
-    <button class="pagination--switch-button" name="{{ collection.name }}:page" form="{{ form_id }}"
+    <button class="pagination--switch-button btn btn-primary" name="{{ collection.name }}:page" form="{{ form_id }}"
             type="submit" value="{{ next_page_number }}"
             {% if pos_last >= total %} disabled{% endif %}
     >
         {% block next_page %}
             <span>&rarr;</span>
         {% endblock next_page %}
     </button>
```

### Comparing `ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/htmx_table/table.html` & `ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/htmx_table/table.html`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/table/filter.html` & `ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/table/filter.html`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/table/form.html` & `ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/table/form.html`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/table/main.html` & `ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/table/main.html`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/table/pager.html` & `ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/table/pager.html`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                 <option{% if size == collection.pager.size %} selected{% endif %}>{{ size }}</option>
             {% endfor %}
         </select>
     </div>
 {% endblock %}
 
 {% block page_navigation %}
-    <div class="pagination--pages">
+    <div class="pagination--pages mt-3">
 
         {% block position %}
             <span class="pagination--position">{{ pos_first }} - {{ pos_last }} out of {{ total }}</span>
         {% endblock position %}
 
 
         {% block prev_page_link %}
```

### Comparing `ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/table/record.html` & `ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/table/record.html`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/templates/collection/serialize/table/table.html` & `ckanext_collection-0.1.21/ckanext/collection/templates/collection/serialize/table/table.html`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/tests/test_readme.py` & `ckanext_collection-0.1.21/ckanext/collection/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/tests/test_shared.py` & `ckanext_collection-0.1.21/ckanext/collection/tests/test_shared.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/tests/utils/test_collection.py` & `ckanext_collection-0.1.21/ckanext/collection/tests/utils/test_collection.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/tests/utils/test_columns.py` & `ckanext_collection-0.1.21/ckanext/collection/tests/utils/test_columns.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/tests/utils/test_data.py` & `ckanext_collection-0.1.21/ckanext/collection/tests/utils/test_data.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/tests/utils/test_pager.py` & `ckanext_collection-0.1.21/ckanext/collection/tests/utils/test_pager.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/tests/utils/test_serializer.py` & `ckanext_collection-0.1.21/ckanext/collection/tests/utils/test_serializer.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/types.py` & `ckanext_collection-0.1.21/ckanext/collection/types.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/utils/__init__.py` & `ckanext_collection-0.1.21/ckanext/collection/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/utils/collection/__init__.py` & `ckanext_collection-0.1.21/ckanext/collection/utils/collection/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/utils/collection/base.py` & `ckanext_collection-0.1.21/ckanext/collection/utils/collection/base.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/utils/collection/db.py` & `ckanext_collection-0.1.21/ckanext/collection/utils/collection/db.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/utils/collection/explorer.py` & `ckanext_collection-0.1.21/ckanext/collection/utils/collection/explorer.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/utils/columns.py` & `ckanext_collection-0.1.21/ckanext/collection/utils/columns.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/utils/data/__init__.py` & `ckanext_collection-0.1.21/ckanext/collection/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/utils/data/api.py` & `ckanext_collection-0.1.21/ckanext/collection/utils/data/api.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/utils/data/base.py` & `ckanext_collection-0.1.21/ckanext/collection/utils/data/base.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/utils/data/db.py` & `ckanext_collection-0.1.21/ckanext/collection/utils/data/db.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/utils/data/model.py` & `ckanext_collection-0.1.21/ckanext/collection/utils/data/model.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/utils/db_connection.py` & `ckanext_collection-0.1.21/ckanext/collection/utils/db_connection.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/utils/filters.py` & `ckanext_collection-0.1.21/ckanext/collection/utils/filters.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/utils/pager.py` & `ckanext_collection-0.1.21/ckanext/collection/utils/pager.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/utils/serialize/__init__.py` & `ckanext_collection-0.1.21/ckanext/collection/utils/serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext/collection/views.py` & `ckanext_collection-0.1.21/ckanext/collection/views.py`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/ckanext_collection.egg-info/PKG-INFO` & `ckanext_collection-0.1.21/ckanext_collection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-collection
-Version: 0.1.2
+Version: 0.1.21
 Home-page: https://github.com/DataShades/ckanext-collection
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext_collection-0.1.2/ckanext_collection.egg-info/SOURCES.txt` & `ckanext_collection-0.1.21/ckanext_collection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/pyproject.toml` & `ckanext_collection-0.1.21/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext_collection-0.1.2/setup.cfg` & `ckanext_collection-0.1.21/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-collection
-version = 0.1.2
+version = 0.1.21
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-collection
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
```


# Comparing `tmp/pyvispr-2024.7.tar.gz` & `tmp/pyvispr-2024.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvispr-2024.7.tar", last modified: Mon Apr 22 12:37:14 2024, max compression
+gzip compressed data, was "pyvispr-2024.8.tar", last modified: Thu Apr 25 12:14:17 2024, max compression
```

## Comparing `pyvispr-2024.7.tar` & `pyvispr-2024.8.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 12:37:14.856403 pyvispr-2024.7/
--rwx------   0 eric      (1000) users      (984)      139 2024-04-05 18:00:47.000000 pyvispr-2024.7/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     5492 2024-04-22 12:37:14.856403 pyvispr-2024.7/PKG-INFO
--rwx------   0 eric      (1000) users      (984)      642 2024-02-07 09:03:58.000000 pyvispr-2024.7/README-COPYRIGHT-utf8.txt
--rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 pyvispr-2024.7/README-LICENCE-utf8.txt
--rwx------   0 eric      (1000) users      (984)     4434 2024-04-22 09:35:02.000000 pyvispr-2024.7/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 12:37:14.846403 pyvispr-2024.7/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 12:37:14.849737 pyvispr-2024.7/documentation/wiki/
--rwx------   0 eric      (1000) users      (984)     2421 2024-04-19 15:02:26.000000 pyvispr-2024.7/documentation/wiki/description.asciidoc
--rwx------   0 eric      (1000) users      (984)      112 2024-02-07 08:56:45.000000 pyvispr-2024.7/pyproject.toml
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 12:37:14.849737 pyvispr-2024.7/pyvispr/
--rwx------   0 eric      (1000) users      (984)     1594 2023-11-17 11:20:29.000000 pyvispr-2024.7/pyvispr/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 12:37:14.853070 pyvispr-2024.7/pyvispr/catalog/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 12:37:14.853070 pyvispr-2024.7/pyvispr/catalog/factory/
--rwx------   0 eric      (1000) users      (984)     1715 2024-04-19 07:34:07.000000 pyvispr-2024.7/pyvispr/catalog/factory/image_256.py
--rwx------   0 eric      (1000) users      (984)     1804 2024-01-19 10:13:27.000000 pyvispr-2024.7/pyvispr/catalog/factory/image_loader.py
--rwx------   0 eric      (1000) users      (984)    15854 2024-04-22 12:32:16.000000 pyvispr-2024.7/pyvispr/catalog/factory/image_viewer.py
--rwx------   0 eric      (1000) users      (984)     1975 2024-01-19 10:13:27.000000 pyvispr-2024.7/pyvispr/catalog/factory/numexpr_calculator.py
--rwx------   0 eric      (1000) users      (984)     1818 2024-01-19 10:18:15.000000 pyvispr-2024.7/pyvispr/catalog/factory/value.py
--rwx------   0 eric      (1000) users      (984)     5939 2024-04-21 14:27:40.000000 pyvispr-2024.7/pyvispr/catalog/factory/value_viewer.py
--rwx------   0 eric      (1000) users      (984)     7691 2024-04-11 08:05:54.000000 pyvispr-2024.7/pyvispr/catalog/installer.py
--rwx------   0 eric      (1000) users      (984)     4160 2024-04-19 07:40:32.000000 pyvispr-2024.7/pyvispr/catalog/parser.py
--rwx------   0 eric      (1000) users      (984)     2226 2024-04-10 14:04:29.000000 pyvispr-2024.7/pyvispr/catalog/type.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 12:37:14.853070 pyvispr-2024.7/pyvispr/config/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 12:37:14.853070 pyvispr-2024.7/pyvispr/config/appearance/
--rwx------   0 eric      (1000) users      (984)     1584 2024-04-10 13:34:33.000000 pyvispr-2024.7/pyvispr/config/appearance/backend.py
--rw-r--r--   0 eric      (1000) users      (984)     1611 2024-04-10 13:52:01.000000 pyvispr-2024.7/pyvispr/config/appearance/behavior.py
--rwx------   0 eric      (1000) users      (984)     2662 2024-04-19 14:06:18.000000 pyvispr-2024.7/pyvispr/config/appearance/color.py
--rwx------   0 eric      (1000) users      (984)     1727 2024-04-19 14:06:38.000000 pyvispr-2024.7/pyvispr/config/appearance/geometry.py
--rwx------   0 eric      (1000) users      (984)     1788 2024-04-10 14:04:53.000000 pyvispr-2024.7/pyvispr/config/path.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 12:37:14.853070 pyvispr-2024.7/pyvispr/constant/
--rw-r--r--   0 eric      (1000) users      (984)     1575 2024-04-10 14:04:29.000000 pyvispr-2024.7/pyvispr/constant/app.py
--rwx------   0 eric      (1000) users      (984)     1961 2024-01-22 14:35:46.000000 pyvispr-2024.7/pyvispr/constant/catalog.py
--rw-r--r--   0 eric      (1000) users      (984)     1654 2024-04-10 13:34:03.000000 pyvispr-2024.7/pyvispr/constant/function.py
--rw-r--r--   0 eric      (1000) users      (984)     1618 2024-04-10 13:51:28.000000 pyvispr-2024.7/pyvispr/constant/path.py
--rw-r--r--   0 eric      (1000) users      (984)     1610 2024-04-10 15:59:22.000000 pyvispr-2024.7/pyvispr/constant/socket.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 12:37:14.853070 pyvispr-2024.7/pyvispr/constant/widget/
--rw-r--r--   0 eric      (1000) users      (984)     1873 2024-04-10 14:04:53.000000 pyvispr-2024.7/pyvispr/constant/widget/function_header.py
--rw-r--r--   0 eric      (1000) users      (984)     1575 2024-04-10 13:59:48.000000 pyvispr-2024.7/pyvispr/constant/widget/list.py
--rw-r--r--   0 eric      (1000) users      (984)     1969 2024-04-11 12:23:33.000000 pyvispr-2024.7/pyvispr/constant/widget/node.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 12:37:14.853070 pyvispr-2024.7/pyvispr/extension/
--rwx------   0 eric      (1000) users      (984)    11886 2024-04-19 06:09:59.000000 pyvispr-2024.7/pyvispr/extension/function.py
--rwx------   0 eric      (1000) users      (984)     2907 2024-04-19 07:15:15.000000 pyvispr-2024.7/pyvispr/extension/module.py
--rwx------   0 eric      (1000) users      (984)     1986 2024-01-19 10:18:15.000000 pyvispr-2024.7/pyvispr/extension/qt6.py
--rwx------   0 eric      (1000) users      (984)     1723 2023-12-14 14:25:13.000000 pyvispr-2024.7/pyvispr/extension/string_.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 12:37:14.849737 pyvispr-2024.7/pyvispr/flow/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 12:37:14.853070 pyvispr-2024.7/pyvispr/flow/descriptive/
--rwx------   0 eric      (1000) users      (984)     7948 2024-04-19 07:15:25.000000 pyvispr-2024.7/pyvispr/flow/descriptive/node.py
--rwx------   0 eric      (1000) users      (984)     4489 2024-04-11 12:50:13.000000 pyvispr-2024.7/pyvispr/flow/descriptive/socket.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 12:37:14.853070 pyvispr-2024.7/pyvispr/flow/functional/
--rwx------   0 eric      (1000) users      (984)     4471 2024-04-19 13:44:55.000000 pyvispr-2024.7/pyvispr/flow/functional/graph.py
--rwx------   0 eric      (1000) users      (984)     4508 2024-04-19 14:19:48.000000 pyvispr-2024.7/pyvispr/flow/functional/link.py
--rwx------   0 eric      (1000) users      (984)    10587 2024-04-19 14:36:55.000000 pyvispr-2024.7/pyvispr/flow/functional/node_isolated.py
--rwx------   0 eric      (1000) users      (984)     5179 2024-04-19 14:41:22.000000 pyvispr-2024.7/pyvispr/flow/functional/node_linked.py
--rwx------   0 eric      (1000) users      (984)     2548 2024-04-19 14:19:48.000000 pyvispr-2024.7/pyvispr/flow/functional/socket.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 12:37:14.856403 pyvispr-2024.7/pyvispr/flow/visual/
--rwx------   0 eric      (1000) users      (984)    18596 2024-04-19 13:37:01.000000 pyvispr-2024.7/pyvispr/flow/visual/graph.py
--rw-r--r--   0 eric      (1000) users      (984)     1858 2024-04-10 15:51:00.000000 pyvispr-2024.7/pyvispr/flow/visual/ii_value.py
--rwx------   0 eric      (1000) users      (984)     6200 2024-04-11 08:06:24.000000 pyvispr-2024.7/pyvispr/flow/visual/link.py
--rwx------   0 eric      (1000) users      (984)    13289 2024-04-19 13:42:58.000000 pyvispr-2024.7/pyvispr/flow/visual/node.py
--rwx------   0 eric      (1000) users      (984)     1879 2024-04-10 14:04:53.000000 pyvispr-2024.7/pyvispr/flow/visual/socket.py
--rwx------   0 eric      (1000) users      (984)     7879 2024-04-19 13:11:30.000000 pyvispr-2024.7/pyvispr/flow/visual/whiteboard.py
--rwx------   0 eric      (1000) users      (984)     1917 2024-04-10 14:04:53.000000 pyvispr-2024.7/pyvispr/install.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 12:37:14.849737 pyvispr-2024.7/pyvispr/interface/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 12:37:14.856403 pyvispr-2024.7/pyvispr/interface/storage/
--rwx------   0 eric      (1000) users      (984)     3187 2024-04-19 06:39:34.000000 pyvispr-2024.7/pyvispr/interface/storage/loading.py
--rwx------   0 eric      (1000) users      (984)     3592 2024-04-19 14:39:57.000000 pyvispr-2024.7/pyvispr/interface/storage/stowing.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 12:37:14.856403 pyvispr-2024.7/pyvispr/interface/window/
--rwx------   0 eric      (1000) users      (984)    16232 2024-04-19 06:27:12.000000 pyvispr-2024.7/pyvispr/interface/window/installer.py
--rwx------   0 eric      (1000) users      (984)     7880 2024-04-18 07:10:06.000000 pyvispr-2024.7/pyvispr/interface/window/runner.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 12:37:14.856403 pyvispr-2024.7/pyvispr/interface/window/widget/
--rwx------   0 eric      (1000) users      (984)    16183 2024-04-18 07:10:09.000000 pyvispr-2024.7/pyvispr/interface/window/widget/function_header.py
--rwx------   0 eric      (1000) users      (984)     4147 2024-04-18 07:06:06.000000 pyvispr-2024.7/pyvispr/interface/window/widget/list.py
--rwx------   0 eric      (1000) users      (984)     2533 2024-01-16 14:25:32.000000 pyvispr-2024.7/pyvispr/interface/window/widget/list_file.py
--rwx------   0 eric      (1000) users      (984)     2710 2024-04-18 11:56:51.000000 pyvispr-2024.7/pyvispr/interface/window/widget/list_function.py
--rwx------   0 eric      (1000) users      (984)     1925 2024-04-10 14:04:53.000000 pyvispr-2024.7/pyvispr/interface/window/widget/list_module.py
--rwx------   0 eric      (1000) users      (984)     3942 2024-04-19 14:11:04.000000 pyvispr-2024.7/pyvispr/interface/window/widget/list_node.py
--rwx------   0 eric      (1000) users      (984)     2412 2024-04-18 07:06:19.000000 pyvispr-2024.7/pyvispr/interface/window/widget/menu.py
--rwx------   0 eric      (1000) users      (984)     1908 2024-04-11 10:07:56.000000 pyvispr-2024.7/pyvispr/run.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 12:37:14.856403 pyvispr-2024.7/pyvispr/runtime/
--rw-r--r--   0 eric      (1000) users      (984)     1713 2024-04-10 14:04:53.000000 pyvispr-2024.7/pyvispr/runtime/backend.py
--rw-r--r--   0 eric      (1000) users      (984)     1625 2024-04-10 13:44:05.000000 pyvispr-2024.7/pyvispr/runtime/catalog.py
--rw-r--r--   0 eric      (1000) users      (984)     1718 2024-04-10 14:44:38.000000 pyvispr-2024.7/pyvispr/runtime/socket.py
--rwx------   0 eric      (1000) users      (984)     1577 2024-04-22 12:37:00.000000 pyvispr-2024.7/pyvispr/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 12:37:14.856403 pyvispr-2024.7/pyvispr.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     5492 2024-04-22 12:37:14.000000 pyvispr-2024.7/pyvispr.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)     2224 2024-04-22 12:37:14.000000 pyvispr-2024.7/pyvispr.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2024-04-22 12:37:14.000000 pyvispr-2024.7/pyvispr.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)       87 2024-04-22 12:37:14.000000 pyvispr-2024.7/pyvispr.egg-info/entry_points.txt
--rw-r--r--   0 eric      (1000) users      (984)      113 2024-04-22 12:37:14.000000 pyvispr-2024.7/pyvispr.egg-info/requires.txt
--rw-r--r--   0 eric      (1000) users      (984)        8 2024-04-22 12:37:14.000000 pyvispr-2024.7/pyvispr.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) users      (984)      113 2024-04-17 16:13:58.000000 pyvispr-2024.7/requirements.txt
--rw-r--r--   0 eric      (1000) users      (984)       38 2024-04-22 12:37:14.856403 pyvispr-2024.7/setup.cfg
--rwx------   0 eric      (1000) users      (984)     8530 2024-04-11 11:30:02.000000 pyvispr-2024.7/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.818999 pyvispr-2024.8/
+-rwx------   0 eric      (1000) users      (984)      139 2024-04-05 18:00:47.000000 pyvispr-2024.8/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     5492 2024-04-25 12:14:17.818999 pyvispr-2024.8/PKG-INFO
+-rwx------   0 eric      (1000) users      (984)      642 2024-02-07 09:03:58.000000 pyvispr-2024.8/README-COPYRIGHT-utf8.txt
+-rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 pyvispr-2024.8/README-LICENCE-utf8.txt
+-rwx------   0 eric      (1000) users      (984)     4434 2024-04-22 09:35:02.000000 pyvispr-2024.8/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.798999 pyvispr-2024.8/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.802332 pyvispr-2024.8/documentation/wiki/
+-rwx------   0 eric      (1000) users      (984)     2421 2024-04-19 15:02:26.000000 pyvispr-2024.8/documentation/wiki/description.asciidoc
+-rwx------   0 eric      (1000) users      (984)      112 2024-02-07 08:56:45.000000 pyvispr-2024.8/pyproject.toml
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.802332 pyvispr-2024.8/pyvispr/
+-rwx------   0 eric      (1000) users      (984)     1594 2023-11-17 11:20:29.000000 pyvispr-2024.8/pyvispr/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.802332 pyvispr-2024.8/pyvispr/catalog/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.802332 pyvispr-2024.8/pyvispr/catalog/factory/
+-rwx------   0 eric      (1000) users      (984)     1715 2024-04-19 07:34:07.000000 pyvispr-2024.8/pyvispr/catalog/factory/image_256.py
+-rwx------   0 eric      (1000) users      (984)     1804 2024-01-19 10:13:27.000000 pyvispr-2024.8/pyvispr/catalog/factory/image_loader.py
+-rwx------   0 eric      (1000) users      (984)    15998 2024-04-25 12:10:02.000000 pyvispr-2024.8/pyvispr/catalog/factory/image_viewer.py
+-rwx------   0 eric      (1000) users      (984)     1975 2024-01-19 10:13:27.000000 pyvispr-2024.8/pyvispr/catalog/factory/numexpr_calculator.py
+-rwx------   0 eric      (1000) users      (984)     1818 2024-01-19 10:18:15.000000 pyvispr-2024.8/pyvispr/catalog/factory/value.py
+-rwx------   0 eric      (1000) users      (984)     5939 2024-04-21 14:27:40.000000 pyvispr-2024.8/pyvispr/catalog/factory/value_viewer.py
+-rwx------   0 eric      (1000) users      (984)     7691 2024-04-11 08:05:54.000000 pyvispr-2024.8/pyvispr/catalog/installer.py
+-rwx------   0 eric      (1000) users      (984)     4160 2024-04-19 07:40:32.000000 pyvispr-2024.8/pyvispr/catalog/parser.py
+-rwx------   0 eric      (1000) users      (984)     2226 2024-04-10 14:04:29.000000 pyvispr-2024.8/pyvispr/catalog/type.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.802332 pyvispr-2024.8/pyvispr/config/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.805666 pyvispr-2024.8/pyvispr/config/appearance/
+-rwx------   0 eric      (1000) users      (984)     1584 2024-04-10 13:34:33.000000 pyvispr-2024.8/pyvispr/config/appearance/backend.py
+-rw-r--r--   0 eric      (1000) users      (984)     1611 2024-04-10 13:52:01.000000 pyvispr-2024.8/pyvispr/config/appearance/behavior.py
+-rwx------   0 eric      (1000) users      (984)     2662 2024-04-19 14:06:18.000000 pyvispr-2024.8/pyvispr/config/appearance/color.py
+-rwx------   0 eric      (1000) users      (984)     1727 2024-04-19 14:06:38.000000 pyvispr-2024.8/pyvispr/config/appearance/geometry.py
+-rwx------   0 eric      (1000) users      (984)     1788 2024-04-10 14:04:53.000000 pyvispr-2024.8/pyvispr/config/path.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.805666 pyvispr-2024.8/pyvispr/constant/
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2024-04-10 14:04:29.000000 pyvispr-2024.8/pyvispr/constant/app.py
+-rwx------   0 eric      (1000) users      (984)     1961 2024-01-22 14:35:46.000000 pyvispr-2024.8/pyvispr/constant/catalog.py
+-rw-r--r--   0 eric      (1000) users      (984)     1654 2024-04-10 13:34:03.000000 pyvispr-2024.8/pyvispr/constant/function.py
+-rw-r--r--   0 eric      (1000) users      (984)     1618 2024-04-10 13:51:28.000000 pyvispr-2024.8/pyvispr/constant/path.py
+-rw-r--r--   0 eric      (1000) users      (984)     1610 2024-04-10 15:59:22.000000 pyvispr-2024.8/pyvispr/constant/socket.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.805666 pyvispr-2024.8/pyvispr/constant/widget/
+-rw-r--r--   0 eric      (1000) users      (984)     1873 2024-04-10 14:04:53.000000 pyvispr-2024.8/pyvispr/constant/widget/function_header.py
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2024-04-10 13:59:48.000000 pyvispr-2024.8/pyvispr/constant/widget/list.py
+-rw-r--r--   0 eric      (1000) users      (984)     1969 2024-04-11 12:23:33.000000 pyvispr-2024.8/pyvispr/constant/widget/node.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.808999 pyvispr-2024.8/pyvispr/extension/
+-rwx------   0 eric      (1000) users      (984)    11886 2024-04-19 06:09:59.000000 pyvispr-2024.8/pyvispr/extension/function.py
+-rwx------   0 eric      (1000) users      (984)     2907 2024-04-19 07:15:15.000000 pyvispr-2024.8/pyvispr/extension/module.py
+-rwx------   0 eric      (1000) users      (984)     1986 2024-01-19 10:18:15.000000 pyvispr-2024.8/pyvispr/extension/qt6.py
+-rwx------   0 eric      (1000) users      (984)     1723 2023-12-14 14:25:13.000000 pyvispr-2024.8/pyvispr/extension/string_.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.798999 pyvispr-2024.8/pyvispr/flow/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.808999 pyvispr-2024.8/pyvispr/flow/descriptive/
+-rwx------   0 eric      (1000) users      (984)     7948 2024-04-19 07:15:25.000000 pyvispr-2024.8/pyvispr/flow/descriptive/node.py
+-rwx------   0 eric      (1000) users      (984)     4489 2024-04-11 12:50:13.000000 pyvispr-2024.8/pyvispr/flow/descriptive/socket.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.812332 pyvispr-2024.8/pyvispr/flow/functional/
+-rwx------   0 eric      (1000) users      (984)     4471 2024-04-19 13:44:55.000000 pyvispr-2024.8/pyvispr/flow/functional/graph.py
+-rwx------   0 eric      (1000) users      (984)     4508 2024-04-19 14:19:48.000000 pyvispr-2024.8/pyvispr/flow/functional/link.py
+-rwx------   0 eric      (1000) users      (984)    10587 2024-04-19 14:36:55.000000 pyvispr-2024.8/pyvispr/flow/functional/node_isolated.py
+-rwx------   0 eric      (1000) users      (984)     5179 2024-04-19 14:41:22.000000 pyvispr-2024.8/pyvispr/flow/functional/node_linked.py
+-rwx------   0 eric      (1000) users      (984)     2548 2024-04-19 14:19:48.000000 pyvispr-2024.8/pyvispr/flow/functional/socket.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.812332 pyvispr-2024.8/pyvispr/flow/visual/
+-rwx------   0 eric      (1000) users      (984)    18596 2024-04-19 13:37:01.000000 pyvispr-2024.8/pyvispr/flow/visual/graph.py
+-rw-r--r--   0 eric      (1000) users      (984)     1858 2024-04-10 15:51:00.000000 pyvispr-2024.8/pyvispr/flow/visual/ii_value.py
+-rwx------   0 eric      (1000) users      (984)     6200 2024-04-11 08:06:24.000000 pyvispr-2024.8/pyvispr/flow/visual/link.py
+-rwx------   0 eric      (1000) users      (984)    13289 2024-04-19 13:42:58.000000 pyvispr-2024.8/pyvispr/flow/visual/node.py
+-rwx------   0 eric      (1000) users      (984)     1879 2024-04-10 14:04:53.000000 pyvispr-2024.8/pyvispr/flow/visual/socket.py
+-rwx------   0 eric      (1000) users      (984)     7879 2024-04-19 13:11:30.000000 pyvispr-2024.8/pyvispr/flow/visual/whiteboard.py
+-rwx------   0 eric      (1000) users      (984)     1917 2024-04-10 14:04:53.000000 pyvispr-2024.8/pyvispr/install.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.798999 pyvispr-2024.8/pyvispr/interface/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.815666 pyvispr-2024.8/pyvispr/interface/storage/
+-rwx------   0 eric      (1000) users      (984)     3187 2024-04-19 06:39:34.000000 pyvispr-2024.8/pyvispr/interface/storage/loading.py
+-rwx------   0 eric      (1000) users      (984)     3592 2024-04-19 14:39:57.000000 pyvispr-2024.8/pyvispr/interface/storage/stowing.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.815666 pyvispr-2024.8/pyvispr/interface/window/
+-rwx------   0 eric      (1000) users      (984)    16232 2024-04-19 06:27:12.000000 pyvispr-2024.8/pyvispr/interface/window/installer.py
+-rwx------   0 eric      (1000) users      (984)     7880 2024-04-18 07:10:06.000000 pyvispr-2024.8/pyvispr/interface/window/runner.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.818999 pyvispr-2024.8/pyvispr/interface/window/widget/
+-rwx------   0 eric      (1000) users      (984)    16183 2024-04-18 07:10:09.000000 pyvispr-2024.8/pyvispr/interface/window/widget/function_header.py
+-rwx------   0 eric      (1000) users      (984)     4147 2024-04-18 07:06:06.000000 pyvispr-2024.8/pyvispr/interface/window/widget/list.py
+-rwx------   0 eric      (1000) users      (984)     2533 2024-01-16 14:25:32.000000 pyvispr-2024.8/pyvispr/interface/window/widget/list_file.py
+-rwx------   0 eric      (1000) users      (984)     2710 2024-04-18 11:56:51.000000 pyvispr-2024.8/pyvispr/interface/window/widget/list_function.py
+-rwx------   0 eric      (1000) users      (984)     1925 2024-04-10 14:04:53.000000 pyvispr-2024.8/pyvispr/interface/window/widget/list_module.py
+-rwx------   0 eric      (1000) users      (984)     3942 2024-04-19 14:11:04.000000 pyvispr-2024.8/pyvispr/interface/window/widget/list_node.py
+-rwx------   0 eric      (1000) users      (984)     2412 2024-04-18 07:06:19.000000 pyvispr-2024.8/pyvispr/interface/window/widget/menu.py
+-rwx------   0 eric      (1000) users      (984)     1908 2024-04-11 10:07:56.000000 pyvispr-2024.8/pyvispr/run.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.818999 pyvispr-2024.8/pyvispr/runtime/
+-rw-r--r--   0 eric      (1000) users      (984)     1713 2024-04-10 14:04:53.000000 pyvispr-2024.8/pyvispr/runtime/backend.py
+-rw-r--r--   0 eric      (1000) users      (984)     1625 2024-04-10 13:44:05.000000 pyvispr-2024.8/pyvispr/runtime/catalog.py
+-rw-r--r--   0 eric      (1000) users      (984)     1718 2024-04-10 14:44:38.000000 pyvispr-2024.8/pyvispr/runtime/socket.py
+-rwx------   0 eric      (1000) users      (984)     1577 2024-04-25 12:13:54.000000 pyvispr-2024.8/pyvispr/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.818999 pyvispr-2024.8/pyvispr.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     5492 2024-04-25 12:14:17.000000 pyvispr-2024.8/pyvispr.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)     2224 2024-04-25 12:14:17.000000 pyvispr-2024.8/pyvispr.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2024-04-25 12:14:17.000000 pyvispr-2024.8/pyvispr.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)       87 2024-04-25 12:14:17.000000 pyvispr-2024.8/pyvispr.egg-info/entry_points.txt
+-rw-r--r--   0 eric      (1000) users      (984)      113 2024-04-25 12:14:17.000000 pyvispr-2024.8/pyvispr.egg-info/requires.txt
+-rw-r--r--   0 eric      (1000) users      (984)        8 2024-04-25 12:14:17.000000 pyvispr-2024.8/pyvispr.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) users      (984)      113 2024-04-17 16:13:58.000000 pyvispr-2024.8/requirements.txt
+-rw-r--r--   0 eric      (1000) users      (984)       38 2024-04-25 12:14:17.818999 pyvispr-2024.8/setup.cfg
+-rwx------   0 eric      (1000) users      (984)     8530 2024-04-11 11:30:02.000000 pyvispr-2024.8/setup.py
```

### Comparing `pyvispr-2024.7/PKG-INFO` & `pyvispr-2024.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvispr
-Version: 2024.7
+Version: 2024.8
 Summary: Visual Programming App for Python
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/pyvispr/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/pyvispr//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/pyvispr/
```

### Comparing `pyvispr-2024.7/README-COPYRIGHT-utf8.txt` & `pyvispr-2024.8/README-COPYRIGHT-utf8.txt`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/README-LICENCE-utf8.txt` & `pyvispr-2024.8/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/README.rst` & `pyvispr-2024.8/README.rst`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/documentation/wiki/description.asciidoc` & `pyvispr-2024.8/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/__init__.py` & `pyvispr-2024.8/pyvispr/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/catalog/factory/image_256.py` & `pyvispr-2024.8/pyvispr/catalog/factory/image_256.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/catalog/factory/image_loader.py` & `pyvispr-2024.8/pyvispr/catalog/factory/image_loader.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/catalog/factory/image_viewer.py` & `pyvispr-2024.8/pyvispr/catalog/factory/image_viewer.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,25 +34,64 @@
 
 import numpy
 import PyQt6.QtGui as qtui
 import PyQt6.QtWidgets as wdgt
 from pyvispr.extension.qt6 import ExecuteApp, QtApp
 from pyvispr.runtime.backend import SCREEN_BACKEND
 
-
 _IMG_FORMAT = {
     1: qtui.QImage.Format.Format_Indexed8,
     3: qtui.QImage.Format.Format_RGB888,
     4: qtui.QImage.Format.Format_RGBA8888,
 }
 _IMG_FORMAT_AS_STR = {1: "Grayscale 8 bits", 3: "RGB 8 bits", 4: "RGBA 8 bits"}
 
 
+class _image_container(wdgt.QLabel):
+    def __init__(self, image: numpy.ndarray, depth: int, status_bar: wdgt.QStatusBar, *args, **kwargs) -> None:
+        """"""
+        wdgt.QLabel.__init__(self, *args, **kwargs)
+        self.image = image
+        self.row_width = str(self.image.shape[0]).__len__()
+        self.col_width = str(self.image.shape[1]).__len__()
+        self.scale = 1.0
+        self.status_bar = status_bar
+        self.should_color_sb = (depth > 2) and numpy.issubdtype(image.dtype, numpy.integer) and (
+            not numpy.any(image < 0)) and (not numpy.any(image > 255))
+        self.setMouseTracking(True)
+
+    def mouseMoveEvent(self, event: qtui.QMoveEvent, /) -> None:
+        """"""
+        position = event.pos()
+        if self.scale > 0.0:
+            row = int(round(position.y() / self.scale))
+            col = int(round(position.x() / self.scale))
+        else:
+            row = int(round(position.y() * ((self.image.shape[0] - 1) / (self.height() - 1))))
+            col = int(round(position.x() * ((self.image.shape[1] - 1) / (self.width() - 1))))
+        color = self.image[row, col, ...]
+        if self.should_color_sb:
+            self.status_bar.setStyleSheet(
+                f"font-weight: bold; "
+                f"background-color: rgb({color[0]}, {color[1]}, {color[2]}); "
+                f"color: rgb({255 - color[0]}, {255 - color[1]}, {255 - color[2]})")
+        self.status_bar.showMessage(f"ROWxCOL:{row:{self.row_width}}x{col:{self.col_width}} = {color}")
+
+
 def pyVisprImageViewer(image: numpy.ndarray, /) -> None:
     """"""
+    if (not isinstance(image, numpy.ndarray)) or (image.size < 1) or numpy.any(numpy.isnan(image)) or numpy.any(
+        numpy.isinf(image)):
+        wdgt.QMessageBox.critical(
+            None,
+            f"{pyVisprImageViewer.__name__}: Error",
+            f"Image is empty or contains NaN or Inf.",
+        )
+        return
+
     img_shape = image.shape
     if 1 < len(img_shape) < 4:
         width = img_shape[1]
         height = img_shape[0]
         if len(img_shape) == 2:
             depth = 1
         else:
@@ -121,41 +160,38 @@
             depth,
             min_value,
             max_value,
             mean_value,
             median_value,
         )
 
-        self.image_container = wdgt.QLabel()
+        self.status_bar = wdgt.QStatusBar()
+        self.image_container = _image_container(image, depth, self.status_bar)
         self.image_container.setBackgroundRole(qtui.QPalette.ColorRole.Base)
         self.image_container.setSizePolicy(
             wdgt.QSizePolicy.Policy.Ignored, wdgt.QSizePolicy.Policy.Ignored
         )
         self.image_container.setScaledContents(True)
 
         self.scroll_area = wdgt.QScrollArea()
         self.scroll_area.setBackgroundRole(qtui.QPalette.ColorRole.Dark)
         self.scroll_area.setWidget(self.image_container)
 
-        self.scale_bars = _ScaleBars(min_value, max_value, depth)
-
-        layout = wdgt.QHBoxLayout()
+        layout = wdgt.QVBoxLayout()
         layout.setContentsMargins(0, 0, 0, 0)
         layout.addWidget(self.scroll_area)
-        for scale_bar in self.scale_bars:
-            layout.addWidget(scale_bar)
+        layout.addWidget(self.status_bar)
 
         central_widget = wdgt.QWidget()
         central_widget.setLayout(layout)
         self.setCentralWidget(central_widget)
 
-        image = _NewNImage_0_255(image, min_value, max_value, depth)
-        self.q_img, self.np_img = _NewQImage(image, width, height, depth)
+        image_0_255, depth_0_255 = _NewNImage_0_255(image, min_value, max_value, depth)
+        self.q_img, self.np_img = _NewQImage(image_0_255, width, height, depth_0_255)
         self.image_container.setPixmap(qtui.QPixmap.fromImage(self.q_img))
-        self.image_scale = 1.0
         self.fit_to_window_action.setEnabled(True)
         if not self.fit_to_window_action.isChecked():
             self.image_container.adjustSize()
 
     def _CreateMenus(
         self,
         width,
@@ -187,26 +223,22 @@
         menu.addAction(self.zoom_out_action)
         menu.addAction(self.original_size_action)
         menu.addSeparator()
         menu.addAction(self.fit_to_window_action)
         menu_bar.addMenu(menu)
 
         menu = wdgt.QMenu("Image I&nfo", self)
-        action = menu.addAction(f"WxH: {width}x{height}")
-        action.setEnabled(False)
+        menu.addAction(f"WxH: {width}x{height}")
         menu.addAction(_IMG_FORMAT_AS_STR[depth])
-        action.setEnabled(False)
         menu.addAction(f"min: {min_value}")
-        action.setEnabled(False)
         menu.addAction(f"max: {max_value}")
-        action.setEnabled(False)
         menu.addAction(f"mean: {mean_value}")
-        action.setEnabled(False)
         menu.addAction(f"median: {median_value}")
-        action.setEnabled(False)
+        for action in menu.actions():
+            action.setEnabled(False)
         menu_bar.addMenu(menu)
 
         self._UpdateActions()
 
     def _CreateActions(self) -> None:
         """"""
         attributes = (
@@ -270,35 +302,37 @@
 
     def ZoomImageOut(self) -> None:
         """"""
         self._ScaleImage(0.8)
 
     def _ScaleImage(self, factor: float, /) -> None:
         """"""
-        self.image_scale *= factor
+        self.image_container.scale *= factor
         self.image_container.resize(
-            self.image_scale * self.image_container.pixmap().size()
+            self.image_container.scale * self.image_container.pixmap().size()
         )
 
         _AdjustScrollBarPosition(self.scroll_area.horizontalScrollBar(), factor)
         _AdjustScrollBarPosition(self.scroll_area.verticalScrollBar(), factor)
 
-        self.zoom_in_action.setEnabled(self.image_scale < 3.0)
-        self.zoom_out_action.setEnabled(self.image_scale > 0.333)
+        self.zoom_in_action.setEnabled(self.image_container.scale < 3.0)
+        self.zoom_out_action.setEnabled(self.image_container.scale > 0.333)
 
     def RevertImageToOriginalSize(self) -> None:
         """"""
         self.image_container.adjustSize()
-        self.image_scale = 1.0
+        self.image_container.scale = 1.0
 
     def FitImageToWindow(self) -> None:
         """"""
         img_should_fit_to_wdw = self.fit_to_window_action.isChecked()
         self.scroll_area.setWidgetResizable(img_should_fit_to_wdw)
-        if not img_should_fit_to_wdw:
+        if img_should_fit_to_wdw:
+            self.image_container.scale = -1.0
+        else:
             self.RevertImageToOriginalSize()
 
         self._UpdateActions()
 
     def CopyImage(self) -> None:
         """"""
         wdgt.QApplication.clipboard().setImage(self.q_img)
@@ -373,38 +407,38 @@
 
 def _NewNImage_0_255(
     image: numpy.ndarray,
     min_value: int | float | numpy.ndarray,
     max_value: int | float | numpy.ndarray,
     depth: int,
     /,
-) -> numpy.ndarray:
+) -> tuple[numpy.ndarray, int]:
     """"""
-    if depth < 4:
-        only_colors = image
-    else:
-        only_colors = image[..., :3]
-
-    # Min and max ignoring alpha channel.
     if isinstance(min_value, numpy.ndarray):
-        global_min = numpy.amin(min_value[: min(depth, 3)])
-        global_max = numpy.amax(max_value[: min(depth, 3)])
+        if (depth == 4) and (min_value[3] == max_value[3]):
+            image = image[..., :3]
+            depth = 3
+            global_min = min(min_value[:3])
+            global_max = max(max_value[:3])
+        else:
+            global_min = min(min_value)
+            global_max = max(max_value)
     else:
         global_min, global_max = min_value, max_value
-    if (global_max > global_min) and ((global_min, global_max) != (0, 255)):
-        factor = 255.0 / (global_max - global_min)
-        with_min_zero = only_colors.astype(numpy.float64, copy=False) - global_min
-        only_colors = numpy.round(factor * with_min_zero)
+    if global_max == global_min:
+        return numpy.full_like(image, 255, dtype=numpy.uint8), depth
 
-    if depth < 4:
-        np_img = only_colors
+    if (global_min, global_max) != (0, 255):
+        factor = 255.0 / (global_max - global_min)
+        with_min_zero = image.astype(numpy.float64, copy=False) - global_min
+        output = numpy.round(factor * with_min_zero)
     else:
-        np_img = numpy.dstack((only_colors, image[..., 3]))
+        output = image
 
-    return np_img.astype(numpy.uint8, copy=False)
+    return output.astype(numpy.uint8, copy=False), depth
 
 
 def _NewQImage(
     image: numpy.ndarray,
     width: int,
     height: int,
     depth: int,
@@ -434,62 +468,7 @@
         int(factor * scroll_bar.value() + ((factor - 1) * scroll_bar.pageStep() / 2))
     )
 
 
 def _MakeImageFilterFromExtension(extension: str, /) -> str:
     """"""
     return f"{extension.upper()} Images (*.{extension})"
-
-
-def _ScaleBars(
-    min_value: int | float | numpy.ndarray,
-    max_value: int | float | numpy.ndarray,
-    depth: int,
-    /,
-) -> tuple[wdgt.QLabel, ...]:
-    """"""
-    output = []
-
-    for p_idx in range(depth):
-        scale_bar = wdgt.QLabel()
-        scale_bar.setBackgroundRole(qtui.QPalette.ColorRole.Base)
-        scale_bar.setSizePolicy(
-            wdgt.QSizePolicy.Policy.Fixed, wdgt.QSizePolicy.Policy.Ignored
-        )
-        scale_bar.setScaledContents(True)
-
-        if isinstance(min_value, numpy.ndarray):
-            current_min = min_value[p_idx]
-            current_max = max_value[p_idx]
-        else:
-            current_min = min_value
-            current_max = max_value
-
-        non_empty_plane = numpy.repeat(
-            numpy.flipud(numpy.linspace(current_min, current_max, num=256))[:, None],
-            20,
-            axis=1,
-        )
-        if (p_idx < 3) and (depth > 1):
-            n_planes = 3
-            img_format = qtui.QImage.Format.Format_RGB888
-            all_planes = numpy.zeros(
-                non_empty_plane.shape + (n_planes,), dtype=numpy.uint8
-            )
-            all_planes[..., p_idx] = non_empty_plane[...]
-        else:
-            n_planes = 1
-            img_format = qtui.QImage.Format.Format_Indexed8
-            all_planes = numpy.uint8(non_empty_plane)
-
-        q_scale_bar = qtui.QImage(
-            all_planes.data,
-            non_empty_plane.shape[1],
-            non_empty_plane.shape[0],
-            n_planes * non_empty_plane.shape[1],
-            img_format,
-        )
-        scale_bar.setPixmap(qtui.QPixmap.fromImage(q_scale_bar))
-
-        output.append(scale_bar)
-
-    return tuple(output)
```

### Comparing `pyvispr-2024.7/pyvispr/catalog/factory/numexpr_calculator.py` & `pyvispr-2024.8/pyvispr/catalog/factory/numexpr_calculator.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/catalog/factory/value.py` & `pyvispr-2024.8/pyvispr/catalog/factory/value.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/catalog/factory/value_viewer.py` & `pyvispr-2024.8/pyvispr/catalog/factory/value_viewer.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/catalog/installer.py` & `pyvispr-2024.8/pyvispr/catalog/installer.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/catalog/parser.py` & `pyvispr-2024.8/pyvispr/catalog/parser.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/catalog/type.py` & `pyvispr-2024.8/pyvispr/catalog/type.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/config/appearance/backend.py` & `pyvispr-2024.8/pyvispr/config/appearance/backend.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/config/appearance/behavior.py` & `pyvispr-2024.8/pyvispr/config/appearance/behavior.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/config/appearance/color.py` & `pyvispr-2024.8/pyvispr/config/appearance/color.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/config/appearance/geometry.py` & `pyvispr-2024.8/pyvispr/config/appearance/geometry.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/config/path.py` & `pyvispr-2024.8/pyvispr/config/path.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/constant/app.py` & `pyvispr-2024.8/pyvispr/constant/app.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/constant/catalog.py` & `pyvispr-2024.8/pyvispr/constant/catalog.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/constant/function.py` & `pyvispr-2024.8/pyvispr/constant/function.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/constant/path.py` & `pyvispr-2024.8/pyvispr/constant/path.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/constant/socket.py` & `pyvispr-2024.8/pyvispr/constant/socket.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/constant/widget/function_header.py` & `pyvispr-2024.8/pyvispr/constant/widget/function_header.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/constant/widget/list.py` & `pyvispr-2024.8/pyvispr/constant/widget/list.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/constant/widget/node.py` & `pyvispr-2024.8/pyvispr/constant/widget/node.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/extension/function.py` & `pyvispr-2024.8/pyvispr/extension/function.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/extension/module.py` & `pyvispr-2024.8/pyvispr/extension/module.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/extension/qt6.py` & `pyvispr-2024.8/pyvispr/extension/qt6.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/extension/string_.py` & `pyvispr-2024.8/pyvispr/extension/string_.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/flow/descriptive/node.py` & `pyvispr-2024.8/pyvispr/flow/descriptive/node.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/flow/descriptive/socket.py` & `pyvispr-2024.8/pyvispr/flow/descriptive/socket.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/flow/functional/graph.py` & `pyvispr-2024.8/pyvispr/flow/functional/graph.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/flow/functional/link.py` & `pyvispr-2024.8/pyvispr/flow/functional/link.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/flow/functional/node_isolated.py` & `pyvispr-2024.8/pyvispr/flow/functional/node_isolated.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/flow/functional/node_linked.py` & `pyvispr-2024.8/pyvispr/flow/functional/node_linked.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/flow/functional/socket.py` & `pyvispr-2024.8/pyvispr/flow/functional/socket.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/flow/visual/graph.py` & `pyvispr-2024.8/pyvispr/flow/visual/graph.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/flow/visual/ii_value.py` & `pyvispr-2024.8/pyvispr/flow/visual/ii_value.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/flow/visual/link.py` & `pyvispr-2024.8/pyvispr/flow/visual/link.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/flow/visual/node.py` & `pyvispr-2024.8/pyvispr/flow/visual/node.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/flow/visual/socket.py` & `pyvispr-2024.8/pyvispr/flow/visual/socket.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/flow/visual/whiteboard.py` & `pyvispr-2024.8/pyvispr/flow/visual/whiteboard.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/install.py` & `pyvispr-2024.8/pyvispr/install.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/interface/storage/loading.py` & `pyvispr-2024.8/pyvispr/interface/storage/loading.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/interface/storage/stowing.py` & `pyvispr-2024.8/pyvispr/interface/storage/stowing.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/interface/window/installer.py` & `pyvispr-2024.8/pyvispr/interface/window/installer.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/interface/window/runner.py` & `pyvispr-2024.8/pyvispr/interface/window/runner.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/interface/window/widget/function_header.py` & `pyvispr-2024.8/pyvispr/interface/window/widget/function_header.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/interface/window/widget/list.py` & `pyvispr-2024.8/pyvispr/interface/window/widget/list.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/interface/window/widget/list_file.py` & `pyvispr-2024.8/pyvispr/interface/window/widget/list_file.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/interface/window/widget/list_function.py` & `pyvispr-2024.8/pyvispr/interface/window/widget/list_function.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/interface/window/widget/list_module.py` & `pyvispr-2024.8/pyvispr/interface/window/widget/list_module.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/interface/window/widget/list_node.py` & `pyvispr-2024.8/pyvispr/interface/window/widget/list_node.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/interface/window/widget/menu.py` & `pyvispr-2024.8/pyvispr/interface/window/widget/menu.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/run.py` & `pyvispr-2024.8/pyvispr/run.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/runtime/backend.py` & `pyvispr-2024.8/pyvispr/runtime/backend.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/runtime/catalog.py` & `pyvispr-2024.8/pyvispr/runtime/catalog.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/runtime/socket.py` & `pyvispr-2024.8/pyvispr/runtime/socket.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/pyvispr/version.py` & `pyvispr-2024.8/pyvispr/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2024.7"
+__version__ = "2024.8"
```

### Comparing `pyvispr-2024.7/pyvispr.egg-info/PKG-INFO` & `pyvispr-2024.8/pyvispr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvispr
-Version: 2024.7
+Version: 2024.8
 Summary: Visual Programming App for Python
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/pyvispr/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/pyvispr//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/pyvispr/
```

### Comparing `pyvispr-2024.7/pyvispr.egg-info/SOURCES.txt` & `pyvispr-2024.8/pyvispr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.7/setup.py` & `pyvispr-2024.8/setup.py`

 * *Files identical despite different names*


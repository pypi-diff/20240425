# Comparing `tmp/feedback-xblock-1.5.0.tar.gz` & `tmp/feedback-xblock-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedback-xblock-1.5.0.tar", last modified: Thu Apr  4 04:44:54 2024, max compression
+gzip compressed data, was "feedback-xblock-1.6.0.tar", last modified: Thu Apr 25 07:15:29 2024, max compression
```

## Comparing `feedback-xblock-1.5.0.tar` & `feedback-xblock-1.6.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:44:54.405441 feedback-xblock-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34500 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-04-04 04:44:54.405441 feedback-xblock-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:44:54.397441 feedback-xblock-1.5.0/feedback/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:44:54.397441 feedback-xblock-1.5.0/feedback/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/extensions/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    17089 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/feedback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:44:54.393441 feedback-xblock-1.5.0/feedback/public/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:44:54.401441 feedback-xblock-1.5.0/feedback/public/default_icons/
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/aface1.png
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/aface2.png
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/aface3.png
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/aface4.png
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/aface5.png
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/amidface1.png
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/amidface2.png
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/amidface3.png
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/amidface4.png
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/amidface5.png
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/anum1.png
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/anum2.png
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/anum3.png
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/anum4.png
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/anum5.png
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/astar1.png
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/astar2.png
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/astar3.png
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/astar4.png
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/astar5.png
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/iface1.png
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/iface2.png
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/iface3.png
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/iface4.png
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/iface5.png
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/imidface1.png
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/imidface2.png
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/imidface3.png
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/imidface4.png
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/imidface5.png
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/inum1.png
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/inum2.png
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/inum3.png
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/inum4.png
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/inum5.png
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/istar1.png
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/istar2.png
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/istar3.png
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/istar4.png
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/public/default_icons/istar5.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:44:54.401441 feedback-xblock-1.5.0/feedback/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/settings/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:44:54.401441 feedback-xblock-1.5.0/feedback/static/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/static/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:44:54.401441 feedback-xblock-1.5.0/feedback/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/static/css/feedback.css
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/static/css/feedback_instructor.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:44:54.401441 feedback-xblock-1.5.0/feedback/static/html/
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/static/html/feedback_instructor.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:44:54.393441 feedback-xblock-1.5.0/feedback/static/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:44:54.401441 feedback-xblock-1.5.0/feedback/static/js/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/static/js/src/feedback.js
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/static/js/src/feedback_instructor.js
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/static/js/src/studio.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:44:54.393441 feedback-xblock-1.5.0/feedback/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:44:54.405441 feedback-xblock-1.5.0/feedback/templates/html/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/templates/html/feedback.html
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/templates/html/scale_item.html
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/templates/html/staff_item.html
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/templates/html/studio_view.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:44:54.405441 feedback-xblock-1.5.0/feedback/templates/instructor_dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/templates/instructor_dashboard/feedback_instructor.html
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/feedback/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:44:54.405441 feedback-xblock-1.5.0/feedback_xblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-04-04 04:44:54.000000 feedback-xblock-1.5.0/feedback_xblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-04 04:44:54.000000 feedback-xblock-1.5.0/feedback_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 04:44:54.000000 feedback-xblock-1.5.0/feedback_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-04 04:44:54.000000 feedback-xblock-1.5.0/feedback_xblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 04:44:54.000000 feedback-xblock-1.5.0/feedback_xblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 04:44:54.000000 feedback-xblock-1.5.0/feedback_xblock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:44:54.405441 feedback-xblock-1.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 04:44:54.405441 feedback-xblock-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-04 04:44:50.000000 feedback-xblock-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:29.179314 feedback-xblock-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34500 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-04-25 07:15:29.179314 feedback-xblock-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:29.171314 feedback-xblock-1.6.0/feedback/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:29.171314 feedback-xblock-1.6.0/feedback/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/extensions/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17089 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/feedback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:29.171314 feedback-xblock-1.6.0/feedback/public/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:29.175314 feedback-xblock-1.6.0/feedback/public/default_icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/aface1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/aface2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/aface3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/aface4.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/aface5.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/amidface1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/amidface2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/amidface3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/amidface4.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/amidface5.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/anum1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/anum2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/anum3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/anum4.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/anum5.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/astar1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/astar2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/astar3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/astar4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/astar5.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/iface1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/iface2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/iface3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/iface4.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/iface5.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/imidface1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/imidface2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/imidface3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/imidface4.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/imidface5.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/inum1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/inum2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/inum3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/inum4.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/inum5.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/istar1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/istar2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/istar3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/istar4.png
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/public/default_icons/istar5.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:29.179314 feedback-xblock-1.6.0/feedback/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/settings/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:29.179314 feedback-xblock-1.6.0/feedback/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/static/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:29.179314 feedback-xblock-1.6.0/feedback/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/static/css/feedback.css
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/static/css/feedback_instructor.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:29.179314 feedback-xblock-1.6.0/feedback/static/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/static/html/feedback_instructor.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:29.171314 feedback-xblock-1.6.0/feedback/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:29.179314 feedback-xblock-1.6.0/feedback/static/js/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/static/js/src/feedback.js
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/static/js/src/feedback_instructor.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/static/js/src/studio.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:29.171314 feedback-xblock-1.6.0/feedback/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:29.179314 feedback-xblock-1.6.0/feedback/templates/html/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/templates/html/feedback.html
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/templates/html/scale_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/templates/html/staff_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/templates/html/studio_view.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:29.179314 feedback-xblock-1.6.0/feedback/templates/instructor_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/templates/instructor_dashboard/feedback_instructor.html
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/feedback/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:29.179314 feedback-xblock-1.6.0/feedback_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-04-25 07:15:28.000000 feedback-xblock-1.6.0/feedback_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-25 07:15:29.000000 feedback-xblock-1.6.0/feedback_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:15:28.000000 feedback-xblock-1.6.0/feedback_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-25 07:15:28.000000 feedback-xblock-1.6.0/feedback_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 07:15:28.000000 feedback-xblock-1.6.0/feedback_xblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 07:15:28.000000 feedback-xblock-1.6.0/feedback_xblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:15:29.179314 feedback-xblock-1.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 07:15:29.179314 feedback-xblock-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-25 07:15:26.000000 feedback-xblock-1.6.0/setup.py
```

### Comparing `feedback-xblock-1.5.0/LICENSE` & `feedback-xblock-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/PKG-INFO` & `feedback-xblock-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedback-xblock
-Version: 1.5.0
+Version: 1.6.0
 Summary: XBlock for providing feedback on course content
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ##############
         FeedbackXBlock
         ##############
         | |License: AGPL v3| |Status| |Python CI| |Publish package to PyPi|
```

### Comparing `feedback-xblock-1.5.0/README.rst` & `feedback-xblock-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/apps.py` & `feedback-xblock-1.6.0/feedback/apps.py`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/extensions/filters.py` & `feedback-xblock-1.6.0/feedback/extensions/filters.py`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/feedback.py` & `feedback-xblock-1.6.0/feedback/feedback.py`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/aface1.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/aface1.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/aface2.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/aface2.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/aface3.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/aface3.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/aface4.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/aface4.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/aface5.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/aface5.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/amidface1.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/amidface1.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/amidface2.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/amidface2.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/amidface3.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/amidface3.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/amidface4.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/amidface4.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/amidface5.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/amidface5.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/anum1.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/anum1.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/anum2.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/anum2.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/anum3.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/anum3.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/anum4.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/anum4.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/anum5.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/anum5.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/astar1.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/astar1.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/astar2.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/astar2.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/astar3.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/astar3.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/astar4.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/astar4.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/astar5.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/astar5.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/iface1.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/iface1.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/iface2.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/iface2.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/iface3.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/iface3.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/iface4.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/iface4.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/iface5.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/iface5.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/imidface1.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/imidface1.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/imidface2.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/imidface2.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/imidface3.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/imidface3.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/imidface4.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/imidface4.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/imidface5.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/imidface5.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/inum1.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/inum1.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/inum2.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/inum2.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/inum3.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/inum3.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/inum4.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/inum4.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/inum5.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/inum5.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/istar1.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/istar1.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/istar2.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/istar2.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/istar3.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/istar3.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/istar4.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/istar4.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/public/default_icons/istar5.png` & `feedback-xblock-1.6.0/feedback/public/default_icons/istar5.png`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/settings/common.py` & `feedback-xblock-1.6.0/feedback/settings/common.py`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/settings/test.py` & `feedback-xblock-1.6.0/feedback/settings/test.py`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/static/README.txt` & `feedback-xblock-1.6.0/feedback/static/README.txt`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/static/css/feedback.css` & `feedback-xblock-1.6.0/feedback/static/css/feedback.css`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/static/html/feedback_instructor.html` & `feedback-xblock-1.6.0/feedback/static/html/feedback_instructor.html`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/static/js/src/feedback.js` & `feedback-xblock-1.6.0/feedback/static/js/src/feedback.js`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/static/js/src/studio.js` & `feedback-xblock-1.6.0/feedback/static/js/src/studio.js`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/templates/html/feedback.html` & `feedback-xblock-1.6.0/feedback/templates/html/feedback.html`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/templates/html/scale_item.html` & `feedback-xblock-1.6.0/feedback/templates/html/scale_item.html`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/templates/html/staff_item.html` & `feedback-xblock-1.6.0/feedback/templates/html/staff_item.html`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback/templates/html/studio_view.html` & `feedback-xblock-1.6.0/feedback/templates/html/studio_view.html`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/feedback_xblock.egg-info/PKG-INFO` & `feedback-xblock-1.6.0/feedback_xblock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedback-xblock
-Version: 1.5.0
+Version: 1.6.0
 Summary: XBlock for providing feedback on course content
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ##############
         FeedbackXBlock
         ##############
         | |License: AGPL v3| |Status| |Python CI| |Publish package to PyPi|
```

### Comparing `feedback-xblock-1.5.0/feedback_xblock.egg-info/SOURCES.txt` & `feedback-xblock-1.6.0/feedback_xblock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feedback-xblock-1.5.0/setup.py` & `feedback-xblock-1.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                 data.append(os.path.relpath(os.path.join(dirname, fname), pkg))
 
     return {pkg: data}
 
 
 setup(
     name='feedback-xblock',
-    version='1.5.0',
+    version='1.6.0',
     description='XBlock for providing feedback on course content',
     long_description=README,
     long_description_content_type='text/x-rst',
     packages=find_packages(
         include=[
             "feedback",
             "feedback.*",
```


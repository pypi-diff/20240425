# Comparing `tmp/pyside_app_core-0.1.9.tar.gz` & `tmp/pyside_app_core-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyside_app_core-0.1.9.tar", last modified: Sat Apr 20 20:34:53 2024, max compression
+gzip compressed data, was "pyside_app_core-0.2.0.tar", last modified: Thu Apr 25 15:28:07 2024, max compression
```

## Comparing `pyside_app_core-0.1.9.tar` & `pyside_app_core-0.2.0.tar`

### file list

```diff
@@ -1,96 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.818882 pyside_app_core-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    42650 2024-04-20 20:34:53.818882 pyside_app_core-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 20:34:53.818882 pyside_app_core-0.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.802882 pyside_app_core-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.806882 pyside_app_core-0.1.9/src/pyside_app_core/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.806882 pyside_app_core-0.1.9/src/pyside_app_core/errors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/errors/basic_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/errors/encode_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/errors/excepthook.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/errors/serial_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.810882 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/generate_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.810882 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/console.svg
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/down-arrow.svg
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/grab-corner.svg
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/reload.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/save.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.810882 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/spin-down/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/spin-down/disabled.svg
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/spin-down/normal.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.810882 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/spin-up/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/spin-up/disabled.svg
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/spin-up/normal.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/standard_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/style_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.810882 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/templates/resources.qrc.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/templates/style.qss.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.810882 pyside_app_core-0.1.9/src/pyside_app_core/log/
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/log/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.810882 pyside_app_core-0.1.9/src/pyside_app_core/qt/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/style.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.810882 pyside_app_core-0.1.9/src/pyside_app_core/qt/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/util/pixel_val.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/util/s_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/util/style_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.814882 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/about_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/base_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/error_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.814882 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/frameless/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/frameless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/frameless/base_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/frameless/base_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/frameless/main_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/frameless/window_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/frameless/window_shade.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/menu_ctx.py
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/multi_combo_box.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/object_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/settings_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/tool_bar_ctx.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/tool_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/tool_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/window_settings_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.814882 pyside_app_core-0.1.9/src/pyside_app_core/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/services/application_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/services/debug_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/services/platform_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.814882 pyside_app_core-0.1.9/src/pyside_app_core/services/serial_service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/services/serial_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/services/serial_service/serial_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.814882 pyside_app_core-0.1.9/src/pyside_app_core/services/serial_service/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/services/serial_service/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/services/serial_service/utils/abstract_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/services/serial_service/utils/conversion_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/services/serial_service/utils/float_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.818882 pyside_app_core-0.1.9/src/pyside_app_core/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/types/numeric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.818882 pyside_app_core-0.1.9/src/pyside_app_core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-20 20:34:46.000000 pyside_app_core-0.1.9/src/pyside_app_core/utils/compare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:34:53.818882 pyside_app_core-0.1.9/src/pyside_app_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42650 2024-04-20 20:34:53.000000 pyside_app_core-0.1.9/src/pyside_app_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-20 20:34:53.000000 pyside_app_core-0.1.9/src/pyside_app_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 20:34:53.000000 pyside_app_core-0.1.9/src/pyside_app_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 20:34:53.000000 pyside_app_core-0.1.9/src/pyside_app_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-20 20:34:53.000000 pyside_app_core-0.1.9/src/pyside_app_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-20 20:34:53.000000 pyside_app_core-0.1.9/src/pyside_app_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.094338 pyside_app_core-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    42650 2024-04-25 15:28:07.094338 pyside_app_core-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:28:07.094338 pyside_app_core-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.078338 pyside_app_core-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.082338 pyside_app_core-0.2.0/src/pyside_app_core/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.082338 pyside_app_core-0.2.0/src/pyside_app_core/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/errors/basic_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/errors/encode_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/errors/excepthook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/errors/serial_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.082338 pyside_app_core-0.2.0/src/pyside_app_core/frameless/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/frameless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/frameless/about_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/frameless/base_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/frameless/base_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/frameless/error_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/frameless/main_toolbar_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/frameless/window_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/frameless/window_shade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.086338 pyside_app_core-0.2.0/src/pyside_app_core/log/
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/log/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.086338 pyside_app_core-0.2.0/src/pyside_app_core/qt/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/application_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.086338 pyside_app_core-0.2.0/src/pyside_app_core/qt/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/util/style_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.086338 pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/base_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/menu_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/multi_combo_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/object_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/settings_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/tool_bar_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/tool_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/tool_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/window_settings_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.078338 pyside_app_core-0.2.0/src/pyside_app_core/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.086338 pyside_app_core-0.2.0/src/pyside_app_core/resources/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/resources/icons/console.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/resources/icons/down-arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/resources/icons/grab-corner.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/resources/icons/reload.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/resources/icons/save.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.086338 pyside_app_core-0.2.0/src/pyside_app_core/resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/resources/templates/resources.qrc.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/resources/templates/style.qss.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.090338 pyside_app_core-0.2.0/src/pyside_app_core/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/services/debug_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/services/platform_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.090338 pyside_app_core-0.2.0/src/pyside_app_core/services/serial_service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/services/serial_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/services/serial_service/serial_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.090338 pyside_app_core-0.2.0/src/pyside_app_core/services/serial_service/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/services/serial_service/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/services/serial_service/utils/abstract_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/services/serial_service/utils/conversion_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/services/serial_service/utils/float_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.090338 pyside_app_core-0.2.0/src/pyside_app_core/style/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/style/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/style/pixel_val.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/style/s_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/style/theme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.090338 pyside_app_core-0.2.0/src/pyside_app_core/theme_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/theme_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/theme_generator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/theme_generator/generate_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/theme_generator/standard_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/theme_generator/style_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.090338 pyside_app_core-0.2.0/src/pyside_app_core/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/types/numeric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.090338 pyside_app_core-0.2.0/src/pyside_app_core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/utils/compare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.090338 pyside_app_core-0.2.0/src/pyside_app_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42650 2024-04-25 15:28:07.000000 pyside_app_core-0.2.0/src/pyside_app_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-25 15:28:07.000000 pyside_app_core-0.2.0/src/pyside_app_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:28:07.000000 pyside_app_core-0.2.0/src/pyside_app_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 15:28:07.000000 pyside_app_core-0.2.0/src/pyside_app_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-25 15:28:07.000000 pyside_app_core-0.2.0/src/pyside_app_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-25 15:28:07.000000 pyside_app_core-0.2.0/src/pyside_app_core.egg-info/top_level.txt
```

### Comparing `pyside_app_core-0.1.9/LICENSE` & `pyside_app_core-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyside_app_core-0.1.9/PKG-INFO` & `pyside_app_core-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyside-app-core
-Version: 0.1.9
+Version: 0.2.0
 Summary: Framework for PySide Applications
 Author-email: Leo Covarrubias <leo@leocov.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -690,19 +690,20 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyside6<7.0.0,>=6.5.0
 Requires-Dist: jinja2~=3.1.2
 Provides-Extra: dev
-Requires-Dist: black~=23.3.0; extra == "dev"
-Requires-Dist: pytest~=7.3.1; extra == "dev"
-Requires-Dist: pytest_mock~=3.10.0; extra == "dev"
-Requires-Dist: pre-commit~=3.3.1; extra == "dev"
-Requires-Dist: import-linter~=1.9.0; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest_mock; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: import-linter~=2.0.0; extra == "dev"
 Requires-Dist: bumpver~=2023.1121; extra == "dev"
 
 # pyside-app-core
 
 Custom style, widgets, and utilities for cross-platform PySide 6.5 applications with a focus on 'frameless' styling.
 
 > This project should be considered experimental and subject to breaking changes until a 1.0.0 release.
@@ -714,29 +715,29 @@
 $ pip install pyside-app-core
 ```
 
 
 ### Run example application
 
 ```shell
-$ python -m examples.simple_app --generate-rcc
+$ python -m examples.toolbar_app --generate-rcc
 ```
 
 ### Generate resources files
 
 Resource files MUST be generated at least once for stylesheets and icons to function.
 
 ```shell
 # from repo with this lib installed
-$ compile-pyside-theme <target directory>
+compile-pyside-theme a/target/directory
 
 # custom QssTheme subclass where `./theme.py` has `THEME = CustomTheme()`
-$ compile-pyside-theme \
+compile-pyside-theme \
     --custom-theme-pypath theme.THEME \
-    <target directory> 
+    a/target/directory
 
 # if needed to resolve python modules you can include pypath updates
-$ compile-pyside-theme \
+compile-pyside-theme \
     --extra-python-path ./src \
     --custom-theme-pypath src.example_app.theme.THEME \
-    <target directory>
+    a/target/directory
 ```
```

### Comparing `pyside_app_core-0.1.9/README.md` & `pyside_app_core-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 $ pip install pyside-app-core
 ```
 
 
 ### Run example application
 
 ```shell
-$ python -m examples.simple_app --generate-rcc
+$ python -m examples.toolbar_app --generate-rcc
 ```
 
 ### Generate resources files
 
 Resource files MUST be generated at least once for stylesheets and icons to function.
 
 ```shell
 # from repo with this lib installed
-$ compile-pyside-theme <target directory>
+compile-pyside-theme a/target/directory
 
 # custom QssTheme subclass where `./theme.py` has `THEME = CustomTheme()`
-$ compile-pyside-theme \
+compile-pyside-theme \
     --custom-theme-pypath theme.THEME \
-    <target directory> 
+    a/target/directory
 
 # if needed to resolve python modules you can include pypath updates
-$ compile-pyside-theme \
+compile-pyside-theme \
     --extra-python-path ./src \
     --custom-theme-pypath src.example_app.theme.THEME \
-    <target directory>
+    a/target/directory
 ```
```

### Comparing `pyside_app_core-0.1.9/pyproject.toml` & `pyside_app_core-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyside-app-core"
-version = "0.1.9"
+version = "0.2.0"
 description = "Framework for PySide Applications"
 readme = "README.md"
 authors = [{ name = "Leo Covarrubias", email = "leo@leocov.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Development Status :: 2 - Pre-Alpha",
@@ -16,69 +16,101 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Typing :: Typed",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 keywords = ["pyside", "pyside6", "frameless", "app", "style"]
+requires-python = ">=3.11"
 dependencies = [
     "pyside6 >=6.5.0,<7.0.0",
     "jinja2 ~= 3.1.2",
 ]
-requires-python = ">=3.11"
 
 [project.optional-dependencies]
 dev = [
-    "black ~= 23.3.0",
-    "pytest ~= 7.3.1",
-    "pytest_mock ~= 3.10.0",
-    "pre-commit ~= 3.3.1",
-    "import-linter ~= 1.9.0",
-    "bumpver ~= 2023.1121"
+    "black",
+    "pytest",
+    "pytest_mock",
+    "mypy",
+    "pre-commit",
+    "import-linter ~= 2.0.0",
+    "bumpver ~= 2023.1121",
 ]
 
 [project.urls]
 Homepage = "https://github.com/leocov-dev/pyside-app-core"
 
 [project.scripts]
 compile-pyside-theme = "pyside_app_core.generator_utils.__main__:main"
 
+[tool.setuptools.package-data]
+"pyside_app_core" = ["py.typed"]
+"pyside_app_core.resources" = [
+    "icons/*",
+    "templates/*",
+]
+
+# ------------------------------
+# testing
 [tool.pytest.ini_options]
 pythonpath = ["src"]
 
+# ------------------------------
+# linting
 [tool.black]
 line-length = 88
 
-[tool.importlinter]
-root_packages = [
-    "src.pyside_app_core",
-    "examples.simple_app",
-]
-include_external_packages = true
-
-[[tool.importlinter.contracts]]
-name = "Don't import from examples"
-type = "forbidden"
-source_modules = [
-    "src.pyside_app_core",
-]
-forbidden_modules = [
-    "examples.simple_app",
-]
+[tool.mypy]
+mypy_path = "$MYPY_CONFIG_FILE_DIR/src"
+packages = ["pyside_app_core"]
+follow_imports = "skip"
+follow_imports_for_stubs = true
+check_untyped_defs = true
 
+# ------------------------------
+# version managment
 [tool.bumpver]
-current_version = "0.1.9"
+current_version = "0.2.0"
 version_pattern = "MAJOR.MINOR.PATCH"
-commit_message  = "Bump version {old_version} -> {new_version}"
-commit          = true
-tag             = true
-push            = true
+commit_message = "Bump version {old_version} -> {new_version}"
+commit = true
+tag = true
+push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
     'version = "{version}"',
 ]
 "src/pyside_app_core/__init__.py" = [
     "{version}"
 ]
 
+# ------------------------------
+# import linter config and rules
+[tool.importlinter]
+root_packages = [
+    "pyside_app_core",
+]
+include_external_packages = true
+
+[[tool.importlinter.contracts]]
+name = "Module Layering"
+type = "layers"
+layers = [
+    "frameless",
+    "qt",
+    "theme_generator",
+    "style",
+    "services",
+    "utils",
+    "errors",
+    "log",
+    "constants",
+    "types",
+]
+containers = ["pyside_app_core"]
+exhaustive = true
+
+
+# ------------------------------
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/constants.py` & `pyside_app_core-0.2.0/src/pyside_app_core/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from typing import Literal
+
 from pyside_app_core.types.numeric import FloatPrecision
 
 # ------------------------------------------------------------------------------
 # defined values
-DATA_ENCODING_ENDIAN = "little"
+DATA_ENCODING_ENDIAN: Literal["little"] = "little"
 LIST_DATA_LEN_BYTES = 2
 FLOAT_PRECISION: FloatPrecision = "single"
 
 # ------------------------------------------------------------------------------
 # calculated values
 DATA_STRUCT_ENDIAN = "<" if DATA_ENCODING_ENDIAN == "little" else ">"
 STRUCT_FLOAT_FMT = "f" if FLOAT_PRECISION == "single" else "d"
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/errors/serial_errors.py` & `pyside_app_core-0.2.0/src/pyside_app_core/errors/serial_errors.py`

 * *Files identical despite different names*

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/__main__.py` & `pyside_app_core-0.2.0/src/pyside_app_core/theme_generator/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import importlib
 import os.path
 import sys
 from pathlib import Path
 
-from pyside_app_core.generator_utils import compile_qrc_to_resources
-from pyside_app_core.qt.style import DEFAULT_THEME
+from pyside_app_core.theme_generator import compile_qrc_to_resources
+from pyside_app_core.style.theme import DEFAULT_THEME
 
 
 def main():
     parser = argparse.ArgumentParser("compile-pyside-theme")
 
     parser.add_argument(
         "--extra-python-path",
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/generate_resources.py` & `pyside_app_core-0.2.0/src/pyside_app_core/theme_generator/generate_resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import subprocess
 import tempfile
 from pathlib import Path
 from typing import List, Literal, Type
 
 from jinja2 import ChoiceLoader, Environment, FileSystemLoader, PackageLoader
 
-from pyside_app_core.generator_utils.standard_resources import STANDARD_RESOURCES
-from pyside_app_core.generator_utils.style_types import QtResourceGroup
-from pyside_app_core.qt.style import DEFAULT_THEME, QssTheme
+from pyside_app_core.theme_generator.standard_resources import STANDARD_RESOURCES
+from pyside_app_core.theme_generator.style_types import QtResourceGroup
+from pyside_app_core.style.theme import DEFAULT_THEME, QssTheme
 
 
 def _compose_template_environment(*extra_template_files: Path) -> Environment:
-    loaders = [PackageLoader("pyside_app_core.generator_utils")]
+    loaders = [PackageLoader("pyside_app_core.resources")]
 
     if extra_template_files:
         dirs = list(set([str(p.parent) for p in extra_template_files]))
         loaders.append(FileSystemLoader(dirs))
 
     return Environment(loader=ChoiceLoader(loaders), autoescape=False)
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/console.svg` & `pyside_app_core-0.2.0/src/pyside_app_core/resources/icons/console.svg`

 * *Files identical despite different names*

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/reload.svg` & `pyside_app_core-0.2.0/src/pyside_app_core/resources/icons/reload.svg`

 * *Files identical despite different names*

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/icons/save.svg` & `pyside_app_core-0.2.0/src/pyside_app_core/resources/icons/save.svg`

 * *Files identical despite different names*

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/standard_resources.py` & `pyside_app_core-0.2.0/src/pyside_app_core/theme_generator/standard_resources.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 from pathlib import Path
 from typing import List
 
-from pyside_app_core.generator_utils.style_types import QtResourceFile, QtResourceGroup
+from pyside_app_core.theme_generator.style_types import QtResourceFile, QtResourceGroup
+
+__resources = Path(__file__).parent.parent / "resources"
 
-__root = Path(__file__).parent
 
 STANDARD_RESOURCES: List[QtResourceGroup] = [
-    QtResourceGroup(files=[QtResourceFile("style.qss")]),
-    QtResourceGroup(
+    QtResourceGroup(files=[QtResourceFile("style.qss")]),  # type: ignore[call-arg]
+    QtResourceGroup(  # type: ignore[call-arg]
         prefix="std/",
         files=[
             QtResourceFile(
-                str(__root / "icons" / "console.svg"), alias="icons/console"
+                str(__resources / "icons" / "console.svg"), alias="icons/console"
+            ),
+            QtResourceFile(
+                str(__resources / "icons" / "down-arrow.svg"), alias="icons/down-arrow"
             ),
             QtResourceFile(
-                str(__root / "icons" / "down-arrow.svg"), alias="icons/down-arrow"
+                str(__resources / "icons" / "grab-corner.svg"),
+                alias="icons/grab-corner",
             ),
             QtResourceFile(
-                str(__root / "icons" / "grab-corner.svg"), alias="icons/grab-corner"
+                str(__resources / "icons" / "reload.svg"), alias="icons/reload"
             ),
-            QtResourceFile(str(__root / "icons" / "reload.svg"), alias="icons/reload"),
-            QtResourceFile(str(__root / "icons" / "save.svg"), alias="icons/save"),
+            QtResourceFile(str(__resources / "icons" / "save.svg"), alias="icons/save"),
             QtResourceFile(
-                str(__root / "icons" / "spin-down/normal.svg"),
+                str(__resources / "icons" / "spin-down/normal.svg"),
                 alias="icons/spin-down/normal",
             ),
             QtResourceFile(
-                str(__root / "icons" / "spin-down/disabled.svg"),
+                str(__resources / "icons" / "spin-down/disabled.svg"),
                 alias="icons/spin-down/disabled",
             ),
             QtResourceFile(
-                str(__root / "icons" / "spin-up/normal.svg"),
+                str(__resources / "icons" / "spin-up/normal.svg"),
                 alias="icons/spin-up/normal",
             ),
             QtResourceFile(
-                str(__root / "icons" / "spin-up/disabled.svg"),
+                str(__resources / "icons" / "spin-up/disabled.svg"),
                 alias="icons/spin-up/disabled",
             ),
         ],
     ),
 ]
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/generator_utils/templates/style.qss.jinja2` & `pyside_app_core-0.2.0/src/pyside_app_core/resources/templates/style.qss.jinja2`

 * *Files identical despite different names*

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/log/__init__.py` & `pyside_app_core-0.2.0/src/pyside_app_core/log/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     else:
         lg = logging.getLogger(name)
         __logger_cache[name] = lg
 
     return lg
 
 
-def set_level(name: str = None, lvl: int = None):
+def set_level(name: str | None = None, lvl: int | None = None):
     """set the logger level"""
     if not name:
         name = _get_caller_name()
     if not lvl:
         raise ValueError(f"Please set '{name}' logger level explicitly.")
     lg = _get_cached_logger(name)
     lg.setLevel(lvl)
@@ -87,11 +87,12 @@
     name = _get_caller_name()
     lg = _get_cached_logger(name)
     lg.exception(msg, *args, **kwargs)
 
 
 def set_all_level(lvl: int):
     """set level of all loggers"""
-    for _, lg in sorted(__logger_cache):
+    for key in sorted(__logger_cache.keys()):
+        lg = __logger_cache[key]
         if not isinstance(lg, PACLogger):
             continue
         lg.setLevel(lvl)
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/log/logger.py` & `pyside_app_core-0.2.0/src/pyside_app_core/log/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 class PACLogger(logging.Logger):
     def __init__(self, name: str, level: int = logging.INFO):
         super(PACLogger, self).__init__(name=name, level=level)
         self.addHandler(get_handler())
 
     def findCaller(
-        self, stack_info: bool = ..., stacklevel: int = ...
+        self, stack_info: bool = False, stacklevel: int = 1
     ) -> tuple[str, int, str, str | None]:
         """
         Find the stack frame of the caller so that we can note the source
         file name, line number and function name.
         """
         f = inspect.currentframe()
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/qt/style.py` & `pyside_app_core-0.2.0/src/pyside_app_core/style/theme.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from pyside_app_core.qt.util.pixel_val import PixelVal
-from pyside_app_core.qt.util.s_color import SColor
+from pyside_app_core.style.pixel_val import PixelVal
+from pyside_app_core.style.s_color import SColor
 from pyside_app_core.services import platform_service
 
 
 class QssTheme:
     """
     Theme configuration object with default values.
     Will be used for both static qss style and dynamic widget style.
@@ -33,15 +33,17 @@
     widget_hover_color = SColor(95)
 
     input_background_color = SColor(95)
     input_background_color_inactive = SColor(85)
 
     tooltip_background_color = SColor(85)
 
-    win_close = SColor(120) if platform_service.is_windows else SColor(237, 107, 95)
+    win_close = (
+        SColor(232, 16, 32) if platform_service.is_windows else SColor(237, 107, 95)
+    )
     win_minimize = SColor(120) if platform_service.is_windows else SColor(245, 191, 79)
     win_maximize = SColor(120) if platform_service.is_windows else SColor(98, 197, 84)
     win_action_inactive = SColor(85)
 
     def __setattr__(self, key, value):
         raise NotImplementedError(
             f'Can\'t update property "{self.__class__.__name__}.{key}". QssThemes are immutable.'
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/qt/util/s_color.py` & `pyside_app_core-0.2.0/src/pyside_app_core/style/s_color.py`

 * *Files identical despite different names*

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/qt/util/style_sheet.py` & `pyside_app_core-0.2.0/src/pyside_app_core/qt/util/style_sheet.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 class CanSetStyleSheet(Protocol):
     def setStyleSheet(self, stylesheet: str) -> None:
         ...
 
 
 def apply_style_sheet(qss_file: str, widget: CanSetStyleSheet) -> None:
-    qss_file = QFile(qss_file)
-    qss_file.open(QFile.OpenModeFlag.ReadOnly | QFile.OpenModeFlag.Text)
-    ts = QTextStream(qss_file)
+    qfile = QFile(qss_file)
+    qfile.open(QFile.OpenModeFlag.ReadOnly | QFile.OpenModeFlag.Text)
+    ts = QTextStream(qfile)
     widget.setStyleSheet(ts.readAll())
 
 
 def assert_resources_file(rcc: Path | None) -> Path:
     """if the given rcc file is None or not found then will try to get a 'default' resource file"""
     if rcc and rcc.exists():
         return rcc
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/base_app.py` & `pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/base_app.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 
 from PySide6.QtCore import Qt
-from PySide6.QtWidgets import QApplication
+from PySide6.QtWidgets import QApplication, QMainWindow
 
 from pyside_app_core.errors.basic_errors import ApplicationError
 from pyside_app_core.qt.util.style_sheet import (
     apply_style_sheet,
     register_resource_file,
 )
 
@@ -19,17 +19,18 @@
         )
 
         register_resource_file(resources_rcc)
 
         apply_style_sheet(":/style.qss", self)
 
         # override in subclass
-        self._main_window = None
+        self._main_window: QMainWindow = None
 
     def launch(self) -> int:
         if not self._main_window:
             raise ApplicationError(
                 f"Must subclass {self.__class__.__name__} and define a main window"
             )
 
         self._main_window.show()
+        self._main_window.devicePixelRatio()
         return self.exec()
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py` & `pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py`

 * *Files identical despite different names*

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/error_dialog.py` & `pyside_app_core-0.2.0/src/pyside_app_core/frameless/error_dialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from PySide6.QtGui import QClipboard
 from PySide6.QtWidgets import QApplication, QLabel, QPlainTextEdit
 
-from pyside_app_core.qt.widgets.frameless.base_dialog import (
+from pyside_app_core.frameless.base_dialog import (
     FramelessBaseDialog,
     StandardButton,
 )
 
 
 class ErrorDialog(FramelessBaseDialog):
     def __init__(self, message: str, detailed: str | None = None):
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/frameless/base_dialog.py` & `pyside_app_core-0.2.0/src/pyside_app_core/frameless/base_dialog.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+from typing import TypeAlias
+
 from PySide6.QtCore import Qt, Signal
 from PySide6.QtGui import QIcon
 from PySide6.QtWidgets import (
     QAbstractButton,
     QDialog,
     QDialogButtonBox,
     QHBoxLayout,
     QLabel,
     QPushButton,
     QVBoxLayout,
     QWidget,
 )
 
-from pyside_app_core.qt.widgets.frameless.base_window import FramelessBaseMixin
+from pyside_app_core.frameless.base_window import FramelessBaseMixin
 
-StandardButton = QDialogButtonBox.StandardButton
-ButtonRole = QDialogButtonBox.ButtonRole
+StandardButton: TypeAlias = QDialogButtonBox.StandardButton
+ButtonRole: TypeAlias = QDialogButtonBox.ButtonRole
 
 
 class FramelessBaseDialog(FramelessBaseMixin, QDialog):
     clicked = Signal(QAbstractButton)
 
     def __init__(self, icon: QIcon | None = None):
         super().__init__(parent=None, f=Qt.WindowType.WindowCloseButtonHint)
@@ -62,12 +64,12 @@
         std_button = self.button(button)
         std_button.setDefault(True)
 
     def setButtonText(self, button: StandardButton, text: str):
         std_button = self.button(button)
         std_button.setText(text)
 
-    def button(self, button: StandardButton) -> QPushButton | None:
+    def button(self, button: StandardButton) -> QPushButton:
         return self._button_box.button(button)
 
     def buttonRole(self, button: QAbstractButton) -> ButtonRole:
         return self._button_box.buttonRole(button)
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/frameless/base_window.py` & `pyside_app_core-0.2.0/src/pyside_app_core/frameless/base_window.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,128 +1,135 @@
-from typing import Tuple
+from typing import cast
 
 from PySide6.QtCore import QPoint, QRect, QSize, Qt, Signal
 from PySide6.QtGui import (
     QBrush,
     QMouseEvent,
     QPainter,
     QPainterPath,
     QPaintEvent,
     QPen,
     QResizeEvent,
 )
-from PySide6.QtWidgets import QLabel, QSizePolicy, QVBoxLayout
+from PySide6.QtWidgets import QLabel, QMainWindow, QSizePolicy, QVBoxLayout, QWidget
 
-from pyside_app_core.qt.widgets.frameless.window_actions import WindowActions
-from pyside_app_core.qt.widgets.frameless.window_shade import FramelessWindowShade
-from pyside_app_core.services import application_service, platform_service
+from pyside_app_core.frameless.window_actions import WindowActions
+from pyside_app_core.frameless.window_shade import FramelessWindowShade
+from pyside_app_core.qt import application_service
 
 
 class FramelessBaseMixin:
     close_window = Signal()
 
     def __init__(
         self,
         *args,
         **kwargs,
     ):
         super(FramelessBaseMixin, self).__init__(*args, **kwargs)
 
-        self.setWindowFlags(self.windowFlags() | Qt.WindowType.FramelessWindowHint)
-        self.setAttribute(Qt.WidgetAttribute.WA_TranslucentBackground)
-        self.setMouseTracking(True)
-        self.setMinimumSize(300, 128)
+        cast(QWidget, self).setWindowFlags(
+            cast(QWidget, self).windowFlags() | Qt.WindowType.FramelessWindowHint
+        )
+        cast(QWidget, self).setAttribute(Qt.WidgetAttribute.WA_TranslucentBackground)
+        cast(QWidget, self).setMouseTracking(True)
+        cast(QWidget, self).setMinimumSize(300, 128)
 
         self._theme = application_service.get_app_theme()
 
         self._top_layout = QVBoxLayout()
         self._top_layout.setContentsMargins(5, 0, 5, 5)
-        self._title = QLabel("", parent=self)
+        self._title = QLabel("", parent=cast(QWidget, self))
         self._title.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self._title.setSizePolicy(
             QSizePolicy.Policy.Fixed,
             QSizePolicy.Policy.MinimumExpanding,
         )
         self._title.setFixedHeight(32)
         self._top_layout.addWidget(
             self._title,
             alignment=Qt.AlignmentFlag.AlignTop,
         )
 
-        self.setLayout(self._top_layout)
+        cast(QWidget, self).setLayout(self._top_layout)
 
         self._moving = False
         self._screen_number: int = 0
         self._move_offset = QPoint(0, 0)
-        self._move_corner = self.window().rect().bottomRight()
+        self._move_corner = cast(QWidget, self).window().rect().bottomRight()
         self._can_minimize = True
         self._can_maximize = True
 
-        self._window_actions = WindowActions(parent=self)
-        self._window_actions.close_clicked.connect(self.close)
+        self._window_actions = WindowActions(parent=cast(QWidget, self))
+        self._window_actions.close_clicked.connect(cast(QWidget, self).close)
         self._window_actions.minimize_clicked.connect(self._on_minimize)
         self._window_actions.maximize_clicked.connect(self._on_maximize)
 
-        self._window_shade = FramelessWindowShade(parent=self)
+        self._window_shade = FramelessWindowShade(parent=cast(QWidget, self))
 
     @property
     def window_bar_geo(self) -> QRect:
         return QRect(
-            0, 0, self.rect().width(), self._window_actions.geometry().height()
+            0,
+            0,
+            cast(QWidget, self).rect().width(),
+            self._window_actions.geometry().height(),
         )
 
     def setWindowTitle(self, title: str):
         self._title.setText(title)
-        super().setWindowTitle(title)
+        cast(QWidget, super()).setWindowTitle(title)
 
     def layout(self) -> QVBoxLayout:
-        return super().layout()
+        return cast(QWidget, super()).layout()
 
     def setFixedSize(self, *args):
         if not args:
             raise ValueError
 
         if len(args) == 1 and isinstance(args[0], QSize):
-            super().setFixedSize(args[0])
+            cast(QWidget, super()).setFixedSize(args[0])
             self._can_maximize = False
             return
 
         elif len(args) == 2 and isinstance(args[0], int) and isinstance(args[1], int):
-            super().setFixedSize(args[0], args[1])
+            cast(QWidget, super()).setFixedSize(args[0], args[1])
             self._can_maximize = False
             return
 
         raise ValueError
 
     def paintEvent(self, event: QPaintEvent) -> None:
         event.accept()
 
-        p = QPainter(self)
+        p = QPainter(cast(QWidget, self))
         p.setRenderHint(QPainter.RenderHint.Antialiasing)
 
         p.setPen(Qt.GlobalColor.transparent)
         p.setBrush(self._theme.background_color)
 
         p.drawRoundedRect(
-            self.rect(), self._theme.win_corner_radius, self._theme.win_corner_radius
+            cast(QWidget, self).rect(),
+            self._theme.win_corner_radius,
+            self._theme.win_corner_radius,
         )
 
-        self._draw_border(p, self.rect())
+        self._draw_border(p, cast(QWidget, self).rect())
 
         # TODO: a bit crude - we want the border to be on top of everything, but no need to call
         #  every time - how to call after all subclasses have added edited widgets? unknown...
         self._window_shade.raise_()
         self._window_actions.raise_()
 
         p.end()
 
     def resizeEvent(self, event: QResizeEvent) -> None:
-        self._title.setFixedWidth(self.rect().width())
+        self._title.setFixedWidth(cast(QWidget, self).rect().width())
         self._window_actions.resizeEvent(event)
-        super().resizeEvent(event)
+        cast(QWidget, super()).resizeEvent(event)
 
     def _draw_border(self, p: QPainter, rect: QRect):
         # outline
         p.setBrush(QBrush(Qt.GlobalColor.transparent))
 
         draw_rect = rect.adjusted(1, 1, -1, -1)
 
@@ -148,53 +155,53 @@
             draw_rect,
             self._theme.win_corner_radius - 2,
             self._theme.win_corner_radius - 2,
         )
         p.setClipping(False)
 
     def _on_maximize(self):
-        if self.isMaximized():
-            self.setWindowState(Qt.WindowState.WindowNoState)
+        if cast(QWidget, self).isMaximized():
+            cast(QWidget, self).setWindowState(Qt.WindowState.WindowNoState)
         else:
-            self.setWindowState(Qt.WindowState.WindowMaximized)
+            cast(QWidget, self).setWindowState(Qt.WindowState.WindowMaximized)
 
     def _on_minimize(self):
-        self.setWindowState(Qt.WindowState.WindowMinimized)
+        cast(QWidget, self).setWindowState(Qt.WindowState.WindowMinimized)
 
     def mouseMoveEvent(self, event: QMouseEvent) -> None:
         if self._moving:
-            win = self.window()
+            win = cast(QWidget, self).window()
             pos = win.mapToGlobal(event.pos())
             target = pos - self._move_offset
             win.move(target)
 
-            self.update()
+            cast(QWidget, self).update()
 
-        super().mouseMoveEvent(event)
+        cast(QWidget, super()).mouseMoveEvent(event)
 
     def mousePressEvent(self, event: QMouseEvent) -> None:
         if (
             (event.buttons() & Qt.MouseButton.LeftButton) == Qt.MouseButton.LeftButton
             and self.window_bar_geo.contains(event.pos())
             and not self._window_actions.geometry().contains(event.pos())
         ):
             self._moving = True
 
-            win = self.window()
+            win = cast(QWidget, self).window()
             rect = win.rect()
             pos: QPoint = win.mapToGlobal(event.pos())
             corner: QPoint = win.mapToGlobal(rect.topLeft())
             self._move_offset = pos - corner
             self._move_corner = rect.bottomRight()
 
-        super().mousePressEvent(event)
+        cast(QWidget, super()).mousePressEvent(event)
 
     def mouseReleaseEvent(self, event: QMouseEvent) -> None:
         self._moving = False
-        self.update()
+        cast(QWidget, self).update()
 
-        super().mouseReleaseEvent(event)
+        cast(QWidget, super()).mouseReleaseEvent(event)
 
     def mouseDoubleClickEvent(self, event: QMouseEvent) -> None:
         self._on_maximize()
 
-        super().mouseReleaseEvent(event)
+        cast(QWidget, super()).mouseReleaseEvent(event)
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/frameless/main_window.py` & `pyside_app_core-0.2.0/src/pyside_app_core/frameless/main_toolbar_window.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from PySide6.QtCore import QPoint, QRect, Qt
 from PySide6.QtGui import QAction
 from PySide6.QtWidgets import QMainWindow, QWidget
 
-from pyside_app_core.qt.widgets.about_dialog import AboutDialog
-from pyside_app_core.qt.widgets.frameless.base_window import FramelessBaseMixin
+from pyside_app_core.frameless.about_dialog import AboutDialog
+from pyside_app_core.frameless.base_window import FramelessBaseMixin
 from pyside_app_core.qt.widgets.menu_ctx import MenuBarContext
 from pyside_app_core.qt.widgets.tool_bar_ctx import ToolBarContext
 from pyside_app_core.qt.widgets.window_settings_mixin import WindowSettingsMixin
 from pyside_app_core.services import platform_service
 
 
-class FramelessMainWindow(WindowSettingsMixin, FramelessBaseMixin, QMainWindow):
+class FramelessMainToolbarWindow(WindowSettingsMixin, FramelessBaseMixin, QMainWindow):
     def __init__(self):
-        super(FramelessMainWindow, self).__init__(parent=None)
+        super(FramelessMainToolbarWindow, self).__init__(parent=None)
 
         self._about_dialog = AboutDialog()
 
         self._central = QWidget(parent=self)
         self._central.setStyleSheet("""background-color: none;""")
         self.setCentralWidget(self._central)
 
         # must call in order to show grab handle
         self.statusBar().show()
 
         self._menu_bar = MenuBarContext(
             self,
-            border_width=0
-            if platform_service.is_macos
-            else self._theme.win_divider_width,
+            border_width=(
+                0 if platform_service.is_macos else self._theme.win_divider_width
+            ),
             border_color=self._theme.win_divider_color,
         )
 
         self._menu_bar.setNativeMenuBar(platform_service.is_macos)
         self.setMenuWidget(self._menu_bar)
 
         with self._menu_bar.add_menu(self.tr("File")) as file_menu:
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/frameless/window_actions.py` & `pyside_app_core-0.2.0/src/pyside_app_core/frameless/window_actions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from enum import IntEnum
+from enum import auto, Enum, IntEnum
 from typing import Callable, NamedTuple, Tuple
 
 from PySide6.QtCore import QEvent, QLine, QPoint, QRect, Qt, Signal
 from PySide6.QtGui import (
     QBrush,
     QColor,
     QMouseEvent,
@@ -10,22 +10,23 @@
     QPainterPath,
     QPaintEvent,
     QPen,
     QResizeEvent,
 )
 from PySide6.QtWidgets import QWidget
 
-from pyside_app_core.services import application_service, platform_service
+from pyside_app_core.services import platform_service
+from pyside_app_core.qt import application_service
 
 
-class Action(IntEnum):
-    NONE = 0
-    CLOSE = 1
-    MINIMIZE = 2
-    MAXIMIZE = 3
+class Action(Enum):
+    NONE = auto()
+    CLOSE = auto()
+    MINIMIZE = auto()
+    MAXIMIZE = auto()
 
 
 ShapeFunc = Callable[[QPainter, QRect, QColor, Action], None]
 EnabledFunc = Callable[[], bool]
 
 
 class ButtonData(NamedTuple):
@@ -69,15 +70,15 @@
         if platform_service.is_macos:
             _width = 13
             _height = 13
             _spacing = 7
         elif platform_service.is_windows:
             _width = 45
             _height = 35
-            _spacing = 3
+            _spacing = 0
         else:
             _width = 17
             _height = 17
             _spacing = 8
 
         self._a_rect = QRect(self._side_offset, _top_offset, _width, _height)
         self._b_rect = self._a_rect.translated(_width + _spacing, 0)
@@ -148,17 +149,14 @@
 
     def paintEvent(self, event: QPaintEvent) -> None:
         event.accept()
 
         p = QPainter(self)
         p.setRenderHint(QPainter.RenderHint.Antialiasing)
 
-        # p.setPen(Qt.GlobalColor.transparent)
-        # p.setBrush(Qt.GlobalColor.transparent)
-
         for rect, data in self._rect_map:
             enabled = self.isActiveWindow() and data.enabled_fn()
 
             self._draw_button(p, rect, data.color, data.action, enabled)
 
             if platform_service.is_macos and not enabled:
                 pass
@@ -236,26 +234,28 @@
                 self.contentsMargins().top(),
                 self.width(),
                 self.height(),
             )
 
         super().resizeEvent(event)
 
-    def _get_button_color(self, color: QColor, is_enabled: bool) -> QColor:
+    def _get_button_color(
+        self, color: QColor, action: Action, is_enabled: bool
+    ) -> QColor:
         if platform_service.is_windows:
             return QColor(Qt.GlobalColor.transparent)
         else:
             return color if is_enabled else self._theme.win_action_inactive
 
     def _draw_button(
         self, p: QPainter, rect: QRect, color: QColor, action: Action, enabled: bool
     ):
         p.setPen(Qt.GlobalColor.transparent)
 
-        f_col = self._get_button_color(color, enabled)
+        f_col = self._get_button_color(color, action, enabled)
 
         if enabled:
             if self._hover == action:
                 f_col = color
             if self._press == action:
                 f_col = color.lighter(135)
 
@@ -281,17 +281,25 @@
         else:
             p.drawEllipse(rect)
 
     def _get_shape_tools(self, color: QColor, action: Action) -> Tuple[QPen, QBrush]:
         if self._press == action:
             color = color if platform_service.is_macos else color.lighter(200)
         elif self._hover == action:
-            color = color if platform_service.is_macos else color.lighter()
+            if platform_service.is_macos:
+                color = color
+            elif platform_service.is_windows:
+                color = color.lighter(200)
+            else:
+                color = color.lighter()
         else:
-            color = Qt.GlobalColor.transparent if platform_service.is_macos else color
+            if platform_service.is_macos:
+                color = Qt.GlobalColor.transparent
+            elif platform_service.is_windows:
+                color = Qt.GlobalColor.gray
 
         pen = QPen(color)
         pen.setWidth(3 if platform_service.is_windows else 2)
         pen.setCapStyle(Qt.PenCapStyle.RoundCap)
 
         brush = QBrush(color)
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/frameless/window_shade.py` & `pyside_app_core-0.2.0/src/pyside_app_core/frameless/window_shade.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QBrush, QPainter, QPaintEvent, QPen
 from PySide6.QtWidgets import QWidget
 
-from pyside_app_core.services import application_service
+from pyside_app_core.qt import application_service
 
 
 class FramelessWindowShade(QWidget):
     def __init__(
         self,
         parent: QWidget,
     ):
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/menu_ctx.py` & `pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/menu_ctx.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     QMenu,
     QMenuBar,
     QSizePolicy,
     QVBoxLayout,
     QWidget,
 )
 
-from pyside_app_core.qt.util.pixel_val import PixelVal
-from pyside_app_core.qt.util.s_color import SColor
+from pyside_app_core.style.pixel_val import PixelVal
+from pyside_app_core.style.s_color import SColor
 from pyside_app_core.qt.widgets.object_name_mixin import ObjectNameMixin
 
 
 class MenuContext(QMenu):
     @contextlib.contextmanager
     def add_menu(self, name: str) -> ContextManager["MenuContext"]:
         menu = MenuContext(name, self)
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/multi_combo_box.py` & `pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/multi_combo_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Adapted from:
 https://gis.stackexchange.com/questions/350148/qcombobox-multiple-selection-pyqt5
 """
+
 from typing import Generator, Generic, Tuple, TypeVar
 
 from PySide6.QtCore import QEvent, Qt, Signal
 from PySide6.QtGui import QFontMetrics, QStandardItem
 from PySide6.QtWidgets import QComboBox, QStyledItemDelegate, QWidget
 
 from pyside_app_core.qt.widgets.object_name_mixin import ObjectNameMixin
@@ -113,33 +114,35 @@
         # Compute elided text (with "...")
         metrics = QFontMetrics(self.lineEdit().font())
         text = metrics.elidedText(
             text, Qt.TextElideMode.ElideRight, self.lineEdit().width()
         )
         self.lineEdit().setText(text)
 
-    def addItem(self, text, userData: DT = None, isChecked=False, **kwargs):
+    def addItem(self, text, userData: DT | None = None, isChecked=False, **kwargs):
         item = QStandardItem()
         item.setText(text)
         if userData is None:
             item.setData(text, Qt.ItemDataRole.UserRole)
         else:
             item.setData(userData, Qt.ItemDataRole.UserRole)
 
         item.setFlags(Qt.ItemFlag.ItemIsEnabled | Qt.ItemFlag.ItemIsUserCheckable)
         item.setCheckState(
             Qt.CheckState.Checked if isChecked else Qt.CheckState.Unchecked
         )
 
         self.model().appendRow(item)
 
-    def addItems(self, texts: list[str], dataList: list[DT] = None, allChecked=False):
+    def addItems(
+        self, texts: list[str], dataList: list[DT] | None = None, allChecked=False
+    ):
         for i, text in enumerate(texts):
             try:
-                data = dataList[i]
+                data = (dataList or [])[i]
             except (TypeError, IndexError):
                 data = None
             self.addItem(text, data, isChecked=allChecked)
 
     def currentData(self, role: Qt.ItemDataRole = Qt.ItemDataRole.UserRole) -> list[DT]:
         res = []
         for item in self.modelItems():
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/object_name_mixin.py` & `pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/object_name_mixin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import cast
+
 from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QWidget
 
 
 class ObjectNameMixin:
     def __init__(self, *args, **kwargs):
         super(ObjectNameMixin, self).__init__(*args, **kwargs)
@@ -9,12 +11,12 @@
         if isinstance(self, QWidget):
             self.setAttribute(Qt.WidgetAttribute.WA_StyledBackground)
 
         obj_name = self.__class__.__name__
         if hasattr(self, "OBJECT_NAME"):
             obj_name = self.OBJECT_NAME.replace(" ", "_")
 
-        self.setObjectName(obj_name)
+        cast(QWidget, self).setObjectName(obj_name)
 
     @property
     def obj_name(self):
-        return self.objectName()
+        return cast(QWidget, self).objectName()
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/settings_mixin.py` & `pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/settings_mixin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
+from typing import cast
 
 from PySide6.QtCore import QCoreApplication, QObject, QSettings
 from PySide6.QtGui import QShowEvent
 from PySide6.QtWidgets import QWidget
 
-from pyside_app_core.services import application_service
+from pyside_app_core.qt import application_service
 
 
 class SettingsMixin:
     def __init__(self, parent: QObject, *args, **kwargs):
         super(SettingsMixin, self).__init__(*args, **kwargs)
 
         self._settings = QSettings(
@@ -23,14 +24,14 @@
 
     def showEvent(self, event: QShowEvent):
         if not self._restored:
             self._restore_state()
             self._restored = True
 
         if isinstance(self, QWidget):
-            super().showEvent(event)
+            cast(QWidget, super()).showEvent(event)
 
     def _restore_state(self):
         pass
 
     def _store_state(self):
         pass
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/tool_bar_ctx.py` & `pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/tool_bar_ctx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import contextlib
 from typing import ContextManager, List, Literal
 
-from PySide6 import QtGui
 from PySide6.QtCore import QSize, Qt
 from PySide6.QtGui import QAction, QIcon
 from PySide6.QtWidgets import QMainWindow, QToolBar, QToolButton
 
 from pyside_app_core.qt.widgets.object_name_mixin import ObjectNameMixin
-from pyside_app_core.services import application_service
+from pyside_app_core.qt import application_service
 
 ToolBarArea = Literal["top", "bottom", "left", "right"]
 
 _TOOL_BAR_AREA_MAP = {
     "top": Qt.ToolBarArea.TopToolBarArea,
     "bottom": Qt.ToolBarArea.BottomToolBarArea,
     "right": Qt.ToolBarArea.RightToolBarArea,
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/tool_button.py` & `pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/tool_button.py`

 * *Files identical despite different names*

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/tool_stack.py` & `pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/tool_stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from PySide6.QtGui import QAction, QIcon
 from PySide6.QtWidgets import QButtonGroup, QHBoxLayout, QMenu, QVBoxLayout, QWidget
 
 from pyside_app_core.qt.widgets.dynamic_stacked_widget import DynamicStackedWidget
 from pyside_app_core.qt.widgets.object_name_mixin import ObjectNameMixin
 from pyside_app_core.qt.widgets.settings_mixin import SettingsMixin
 from pyside_app_core.qt.widgets.tool_button import ToolButton
-from pyside_app_core.qt.style import QssTheme
+from pyside_app_core.style.theme import QssTheme
 
 ToolStackSide = Literal["right", "left"]
 
 
 class ToolStack(SettingsMixin, ObjectNameMixin, QWidget):
     def __init__(
         self,
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/qt/widgets/window_settings_mixin.py` & `pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/window_settings_mixin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,30 @@
+from typing import cast
+
 from PySide6.QtCore import QObject
-from PySide6.QtWidgets import QMainWindow
+from PySide6.QtWidgets import QMainWindow, QWidget
 
 from pyside_app_core.qt.widgets.object_name_mixin import ObjectNameMixin
 from pyside_app_core.qt.widgets.settings_mixin import SettingsMixin
 
 
 class WindowSettingsMixin(ObjectNameMixin, SettingsMixin):
     def __init__(self, parent: QObject, *args, **kwargs):
         super(WindowSettingsMixin, self).__init__(parent=parent, *args, **kwargs)
 
     def _store_state(self) -> None:
-        self._settings.setValue(f"{self.obj_name}_geometry", self.saveGeometry())
+        self._settings.setValue(
+            f"{self.obj_name}_geometry", cast(QWidget, self).saveGeometry()
+        )
 
         if isinstance(self, QMainWindow):
-            self._settings.setValue(f"{self.obj_name}_window_state", self.saveState())
+            cast(SettingsMixin, self)._settings.setValue(
+                f"{cast(ObjectNameMixin, self).obj_name}_window_state", self.saveState()
+            )
 
     def _restore_state(self) -> None:
-        self.restoreGeometry(self._settings.value(f"{self.obj_name}_geometry"))
+        cast(QWidget, self).restoreGeometry(
+            self._settings.value(f"{self.obj_name}_geometry")
+        )
 
         # if isinstance(self, QMainWindow):
         #     self.restoreState(self._settings.value(f"{self.obj_name}_window_state"))
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/services/application_service.py` & `pyside_app_core-0.2.0/src/pyside_app_core/qt/application_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Type
 
 from pyside_app_core.errors.basic_errors import ApplicationError
-from pyside_app_core.qt.style import QssTheme
+from pyside_app_core.style.theme import QssTheme
 
-__app_name = ""
-__app_id = ""
-__app_version = ""
-__app_theme = None
+__app_name: str
+__app_id: str
+__app_version: str
+__app_theme: QssTheme
 
 
 def set_app_name(app_name: str) -> None:
     global __app_name
     if __app_name:
         raise ApplicationError("Can't update app_name after its been set once.")
 
@@ -29,15 +29,15 @@
     global __app_version
     if __app_version:
         raise ApplicationError("Can't update app_version after its been set once.")
 
     __app_version = app_version
 
 
-def set_app_theme(app_theme: QssTheme | Type[QssTheme]) -> None:
+def set_app_theme(app_theme: QssTheme) -> None:
     global __app_theme
     if __app_theme:
         raise ApplicationError("Can't update app_theme after its been set once.")
 
     __app_theme = app_theme
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/services/serial_service/serial_service.py` & `pyside_app_core-0.2.0/src/pyside_app_core/services/serial_service/serial_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 from PySide6.QtCore import QIODevice, QObject, Qt, QTimer, Signal
 from PySide6.QtSerialPort import QSerialPort, QSerialPortInfo
 
 from pyside_app_core import log
 from pyside_app_core.errors.serial_errors import (
     SerialConnectionError,
     SerialDisconnectedError,
+    SerialError,
     SerialReadError,
     SerialUnknownError,
     SerialWriteError,
 )
-from pyside_app_core.qt.widgets.object_name_mixin import ObjectNameMixin
 from pyside_app_core.services.serial_service.utils.abstract_decoder import (
     CommandInterface,
     TranscoderInterface,
 )
 
 log.set_level(lvl=logging.DEBUG)
 
 
 class CanRegister(Protocol):
     def bind_serial_service(self, serial_service: "SerialService"):
         ...
 
 
-class SerialService(ObjectNameMixin, QObject):
+class SerialService(QObject):
     ports = Signal(list)
     com_connect = Signal(QSerialPort)
     com_disconnect = Signal()
     data = Signal(object)
     error = Signal(Exception)
 
     def __init__(self, transcoder: TranscoderInterface, parent: QObject):
@@ -133,14 +133,17 @@
         self._com = None
 
     def deleteLater(self) -> None:
         self.close_connection()
         super().deleteLater()
 
     def _on_data(self, *args, **kwargs) -> None:
+        if not self._com:
+            return
+
         read: bytes = self._com.readAll()
         data = bytearray(read)
         self._buffer.extend(data)
 
         if b"\x00" in self._buffer:
             chunks: list[bytearray]
             remainder: bytearray
@@ -155,14 +158,16 @@
 
                 self.data.emit(command)
 
             self._buffer.clear()
             self._buffer.extend(remainder)
 
     def _on_error(self, error: QSerialPort.SerialPortError | None) -> None:
+        exception: SerialError
+
         if error is None or error == QSerialPort.SerialPortError.NoError:
             return
         elif error == QSerialPort.SerialPortError.OpenError:
             exception = SerialConnectionError(self._com, error)
         elif error == QSerialPort.SerialPortError.ReadError:
             exception = SerialReadError(self._com, error)
         elif error == QSerialPort.SerialPortError.WriteError:
@@ -176,15 +181,15 @@
 
         QTimer.singleShot(3000, self.scan_for_ports)
 
         self.error.emit(exception)
         raise exception
 
     def _port_filter(self, p: QSerialPort) -> bool:
-        filters = [
+        filters: list[bool] = [
             # p.portName().startswith("cu."),
             # "bluetooth" not in p.portName().lower()
         ]
 
         return all(filters)
 
     def _debug_ports(self, ports: List[QSerialPortInfo]) -> None:
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/services/serial_service/utils/abstract_decoder.py` & `pyside_app_core-0.2.0/src/pyside_app_core/services/serial_service/utils/abstract_decoder.py`

 * *Files identical despite different names*

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/services/serial_service/utils/conversion_utils.py` & `pyside_app_core-0.2.0/src/pyside_app_core/services/serial_service/utils/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core/services/serial_service/utils/float_map.py` & `pyside_app_core-0.2.0/src/pyside_app_core/services/serial_service/utils/float_map.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 
     def __repr__(self):
         return self._data.__repr__()
 
     def __str__(self):
         return self._data.__str__()
 
-    def __eq__(self, other: Self) -> bool:
-        val_eq: List[bool] = []
+    def __eq__(self, other: Self) -> bool:  # type: ignore[override]
+        val_eq: list[bool] = []
         for k, v in self.items():
             other_v = other.get(k)
             if other_v:
                 val_eq.append(compare.float_approx(v, other_v))
 
         return all(
             [
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core.egg-info/PKG-INFO` & `pyside_app_core-0.2.0/src/pyside_app_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyside-app-core
-Version: 0.1.9
+Version: 0.2.0
 Summary: Framework for PySide Applications
 Author-email: Leo Covarrubias <leo@leocov.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -690,19 +690,20 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyside6<7.0.0,>=6.5.0
 Requires-Dist: jinja2~=3.1.2
 Provides-Extra: dev
-Requires-Dist: black~=23.3.0; extra == "dev"
-Requires-Dist: pytest~=7.3.1; extra == "dev"
-Requires-Dist: pytest_mock~=3.10.0; extra == "dev"
-Requires-Dist: pre-commit~=3.3.1; extra == "dev"
-Requires-Dist: import-linter~=1.9.0; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest_mock; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: import-linter~=2.0.0; extra == "dev"
 Requires-Dist: bumpver~=2023.1121; extra == "dev"
 
 # pyside-app-core
 
 Custom style, widgets, and utilities for cross-platform PySide 6.5 applications with a focus on 'frameless' styling.
 
 > This project should be considered experimental and subject to breaking changes until a 1.0.0 release.
@@ -714,29 +715,29 @@
 $ pip install pyside-app-core
 ```
 
 
 ### Run example application
 
 ```shell
-$ python -m examples.simple_app --generate-rcc
+$ python -m examples.toolbar_app --generate-rcc
 ```
 
 ### Generate resources files
 
 Resource files MUST be generated at least once for stylesheets and icons to function.
 
 ```shell
 # from repo with this lib installed
-$ compile-pyside-theme <target directory>
+compile-pyside-theme a/target/directory
 
 # custom QssTheme subclass where `./theme.py` has `THEME = CustomTheme()`
-$ compile-pyside-theme \
+compile-pyside-theme \
     --custom-theme-pypath theme.THEME \
-    <target directory> 
+    a/target/directory
 
 # if needed to resolve python modules you can include pypath updates
-$ compile-pyside-theme \
+compile-pyside-theme \
     --extra-python-path ./src \
     --custom-theme-pypath src.example_app.theme.THEME \
-    <target directory>
+    a/target/directory
 ```
```

### Comparing `pyside_app_core-0.1.9/src/pyside_app_core.egg-info/SOURCES.txt` & `pyside_app_core-0.2.0/src/pyside_app_core.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,71 @@
 LICENSE
-MANIFEST.in
 README.md
 pyproject.toml
 src/pyside_app_core/__init__.py
 src/pyside_app_core/constants.py
+src/pyside_app_core/py.typed
 src/pyside_app_core.egg-info/PKG-INFO
 src/pyside_app_core.egg-info/SOURCES.txt
 src/pyside_app_core.egg-info/dependency_links.txt
 src/pyside_app_core.egg-info/entry_points.txt
 src/pyside_app_core.egg-info/requires.txt
 src/pyside_app_core.egg-info/top_level.txt
 src/pyside_app_core/errors/__init__.py
 src/pyside_app_core/errors/basic_errors.py
 src/pyside_app_core/errors/encode_errors.py
 src/pyside_app_core/errors/excepthook.py
 src/pyside_app_core/errors/serial_errors.py
-src/pyside_app_core/generator_utils/__init__.py
-src/pyside_app_core/generator_utils/__main__.py
-src/pyside_app_core/generator_utils/generate_resources.py
-src/pyside_app_core/generator_utils/standard_resources.py
-src/pyside_app_core/generator_utils/style_types.py
-src/pyside_app_core/generator_utils/icons/console.svg
-src/pyside_app_core/generator_utils/icons/down-arrow.svg
-src/pyside_app_core/generator_utils/icons/grab-corner.svg
-src/pyside_app_core/generator_utils/icons/reload.svg
-src/pyside_app_core/generator_utils/icons/save.svg
-src/pyside_app_core/generator_utils/icons/spin-down/disabled.svg
-src/pyside_app_core/generator_utils/icons/spin-down/normal.svg
-src/pyside_app_core/generator_utils/icons/spin-up/disabled.svg
-src/pyside_app_core/generator_utils/icons/spin-up/normal.svg
-src/pyside_app_core/generator_utils/templates/resources.qrc.jinja2
-src/pyside_app_core/generator_utils/templates/style.qss.jinja2
+src/pyside_app_core/frameless/__init__.py
+src/pyside_app_core/frameless/about_dialog.py
+src/pyside_app_core/frameless/base_dialog.py
+src/pyside_app_core/frameless/base_window.py
+src/pyside_app_core/frameless/error_dialog.py
+src/pyside_app_core/frameless/main_toolbar_window.py
+src/pyside_app_core/frameless/window_actions.py
+src/pyside_app_core/frameless/window_shade.py
 src/pyside_app_core/log/__init__.py
 src/pyside_app_core/log/logger.py
 src/pyside_app_core/qt/__init__.py
-src/pyside_app_core/qt/style.py
+src/pyside_app_core/qt/application_service.py
 src/pyside_app_core/qt/util/__init__.py
-src/pyside_app_core/qt/util/pixel_val.py
-src/pyside_app_core/qt/util/s_color.py
 src/pyside_app_core/qt/util/style_sheet.py
 src/pyside_app_core/qt/widgets/__init__.py
-src/pyside_app_core/qt/widgets/about_dialog.py
 src/pyside_app_core/qt/widgets/base_app.py
 src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py
-src/pyside_app_core/qt/widgets/error_dialog.py
 src/pyside_app_core/qt/widgets/menu_ctx.py
 src/pyside_app_core/qt/widgets/multi_combo_box.py
 src/pyside_app_core/qt/widgets/object_name_mixin.py
 src/pyside_app_core/qt/widgets/settings_mixin.py
 src/pyside_app_core/qt/widgets/tool_bar_ctx.py
 src/pyside_app_core/qt/widgets/tool_button.py
 src/pyside_app_core/qt/widgets/tool_stack.py
 src/pyside_app_core/qt/widgets/window_settings_mixin.py
-src/pyside_app_core/qt/widgets/frameless/__init__.py
-src/pyside_app_core/qt/widgets/frameless/base_dialog.py
-src/pyside_app_core/qt/widgets/frameless/base_window.py
-src/pyside_app_core/qt/widgets/frameless/main_window.py
-src/pyside_app_core/qt/widgets/frameless/window_actions.py
-src/pyside_app_core/qt/widgets/frameless/window_shade.py
+src/pyside_app_core/resources/icons/console.svg
+src/pyside_app_core/resources/icons/down-arrow.svg
+src/pyside_app_core/resources/icons/grab-corner.svg
+src/pyside_app_core/resources/icons/reload.svg
+src/pyside_app_core/resources/icons/save.svg
+src/pyside_app_core/resources/templates/resources.qrc.jinja2
+src/pyside_app_core/resources/templates/style.qss.jinja2
 src/pyside_app_core/services/__init__.py
-src/pyside_app_core/services/application_service.py
 src/pyside_app_core/services/debug_service.py
 src/pyside_app_core/services/platform_service.py
 src/pyside_app_core/services/serial_service/__init__.py
 src/pyside_app_core/services/serial_service/serial_service.py
 src/pyside_app_core/services/serial_service/utils/__init__.py
 src/pyside_app_core/services/serial_service/utils/abstract_decoder.py
 src/pyside_app_core/services/serial_service/utils/conversion_utils.py
 src/pyside_app_core/services/serial_service/utils/float_map.py
+src/pyside_app_core/style/__init__.py
+src/pyside_app_core/style/pixel_val.py
+src/pyside_app_core/style/s_color.py
+src/pyside_app_core/style/theme.py
+src/pyside_app_core/theme_generator/__init__.py
+src/pyside_app_core/theme_generator/__main__.py
+src/pyside_app_core/theme_generator/generate_resources.py
+src/pyside_app_core/theme_generator/standard_resources.py
+src/pyside_app_core/theme_generator/style_types.py
 src/pyside_app_core/types/__init__.py
 src/pyside_app_core/types/numeric.py
 src/pyside_app_core/utils/__init__.py
 src/pyside_app_core/utils/compare.py
```


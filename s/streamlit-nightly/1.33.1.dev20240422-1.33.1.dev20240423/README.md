# Comparing `tmp/streamlit_nightly-1.33.1.dev20240422.tar.gz` & `tmp/streamlit_nightly-1.33.1.dev20240423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_nightly-1.33.1.dev20240422.tar", last modified: Tue Apr 23 07:03:28 2024, max compression
+gzip compressed data, was "streamlit_nightly-1.33.1.dev20240423.tar", last modified: Wed Apr 24 07:02:38 2024, max compression
```

## Comparing `streamlit_nightly-1.33.1.dev20240422.tar` & `streamlit_nightly-1.33.1.dev20240423.tar`

### file list

```diff
@@ -1,571 +1,571 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.939453 streamlit_nightly-1.33.1.dev20240422/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-23 07:03:28.939453 streamlit_nightly-1.33.1.dev20240422/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.811453 streamlit_nightly-1.33.1.dev20240422/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/bin/streamlit.cmd
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 07:03:28.939453 streamlit_nightly-1.33.1.dev20240422/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.815453 streamlit_nightly-1.33.1.dev20240422/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/case_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/cli_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/code_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/color_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/column_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.819453 streamlit_nightly-1.33.1.dev20240422/streamlit/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/commands/execution_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/commands/experimental_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/commands/page_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.819453 streamlit_nightly-1.33.1.dev20240422/streamlit/components/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.819453 streamlit_nightly-1.33.1.dev20240422/streamlit/components/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/components/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/components/lib/local_component_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.819453 streamlit_nightly-1.33.1.dev20240422/streamlit/components/types/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/components/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/components/types/base_component_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/components/types/base_custom_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.819453 streamlit_nightly-1.33.1.dev20240422/streamlit/components/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/components/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/components/v1/component_arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/components/v1/component_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/components/v1/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/components/v1/custom_component.py
--rw-r--r--   0 runner    (1001) docker     (127)    43895 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/config_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/config_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.819453 streamlit_nightly-1.33.1.dev20240422/streamlit/connections/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/connections/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/connections/snowflake_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/connections/snowpark_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12141 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/connections/sql_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/connections/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    33936 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/delta_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/deprecation_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/development.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/echo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.827453 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/altair_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)    57049 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/arrow_altair.py
--rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/arrow_vega_lite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/balloons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/bokeh_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/deck_gl_json_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/dialog_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/doc_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    12068 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/graphviz_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/heading.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/iframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    27373 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/layouts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.831453 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/lib/column_config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    51087 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/lib/column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/lib/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/lib/dicttools.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/lib/mutable_status_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/lib/pandas_styler_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/lib/streamlit_plotly_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/lib/subtitle_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    26886 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/plotly_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/pyplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/snow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/spinner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/toast.py
--rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.831453 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31409 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/camera_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    13445 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)    12139 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     8925 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)    35827 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/data_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17437 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/file_uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/multiselect.py
--rw-r--r--   0 runner    (1001) docker     (127)    17819 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/number_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    12608 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/radio.py
--rw-r--r--   0 runner    (1001) docker     (127)    13225 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/select_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)    11448 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/selectbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    26434 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)    21899 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/text_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    29620 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/time_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/elements/write.py
--rw-r--r--   0 runner    (1001) docker     (127)    73749 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/emojis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/env_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/error_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.831453 streamlit_nightly-1.33.1.dev20240422/streamlit/external/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.835453 streamlit_nightly-1.33.1.dev20240422/streamlit/external/langchain/
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/external/langchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/external/langchain/streamlit_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/folder_black_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/git_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.835453 streamlit_nightly-1.33.1.dev20240422/streamlit/hello/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/hello/Hello.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/hello/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.835453 streamlit_nightly-1.33.1.dev20240422/streamlit/hello/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/hello/pages/0_Animation_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/hello/pages/1_Plotting_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/hello/pages/2_Mapping_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/hello/pages/3_DataFrame_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/hello/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/js_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/net_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.863453 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Alert_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Alert_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/AppPage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/AppPage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ArrowNamedDataSet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ArrowNamedDataSet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ArrowVegaLiteChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ArrowVegaLiteChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Arrow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Arrow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Audio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Audio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/AutoRerun_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/AutoRerun_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/BackMsg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/BackMsg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Balloons_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Balloons_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Block_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Block_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/BokehChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/BokehChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Button_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Button_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/CameraInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/CameraInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ChatInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ChatInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Checkbox_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Checkbox_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ClientState_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ClientState_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Code_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Code_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ColorPicker_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ColorPicker_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Components_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Components_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/DataFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/DataFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/DateInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/DateInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/DeckGlJsonChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/DeckGlJsonChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Delta_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Delta_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/DocString_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/DocString_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/DownloadButton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/DownloadButton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Element_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Element_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Empty_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Empty_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Exception_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Exception_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Favicon_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Favicon_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/FileUploader_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/FileUploader_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ForwardMsg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ForwardMsg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/GitInfo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/GitInfo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/GraphVizChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/GraphVizChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Heading_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Heading_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Html_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Html_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/IFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/IFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Image_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Image_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Json_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Json_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/LabelVisibilityMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/LabelVisibilityMessage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/LinkButton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/LinkButton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Markdown_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Markdown_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Metric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Metric_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/MultiSelect_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/MultiSelect_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/NamedDataSet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/NamedDataSet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/NewSession_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/NewSession_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/NumberInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/NumberInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PageConfig_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PageConfig_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PageInfo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PageInfo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PageLink_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PageLink_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PageNotFound_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PageNotFound_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PageProfile_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PageProfile_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PagesChanged_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PagesChanged_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ParentMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ParentMessage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PlotlyChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PlotlyChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Progress_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Progress_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Radio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Radio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/RootContainer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/RootContainer_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Selectbox_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Selectbox_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/SessionEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/SessionEvent_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/SessionStatus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/SessionStatus_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Skeleton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Skeleton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Slider_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Slider_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Snow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Snow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Spinner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Spinner_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/TextArea_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/TextArea_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/TextInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/TextInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Text_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Text_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/TimeInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/TimeInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Toast_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Toast_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/VegaLiteChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/VegaLiteChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Video_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Video_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/WidgetStates_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/WidgetStates_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/openmetrics_data_model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-04-23 06:59:43.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/proto/openmetrics_data_model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.867453 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36802 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/app_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.867453 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/cache_data_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/cache_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    21616 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/cache_resource_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/cache_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    17527 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/cache_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17358 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/cached_message_replay.py
--rw-r--r--   0 runner    (1001) docker     (127)    18986 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.867453 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/storage/cache_storage_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/storage/dummy_cache_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/storage/local_disk_cache_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/connection_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/forward_msg_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/forward_msg_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/fragment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.871453 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/legacy_caching/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/legacy_caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27873 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/legacy_caching/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/legacy_caching/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/media_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/media_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/memory_media_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/memory_session_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/memory_uploaded_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/metrics_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    29567 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/runtime_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/script_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.871453 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/scriptrunner/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/scriptrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/scriptrunner/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/scriptrunner/magic_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/scriptrunner/script_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/scriptrunner/script_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/scriptrunner/script_run_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/scriptrunner/script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/session_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.871453 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/state/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/state/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/state/query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/state/query_params_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/state/safe_session_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    27500 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/state/session_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/state/session_state_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/state/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/uploaded_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/websocket_session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/source_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.871453 streamlit_nightly-1.33.1.dev20240422/streamlit/static/
--rw-r--r--   0 runner    (1001) docker     (127)    14380 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-23 07:00:13.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.807453 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.875453 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/css/2411.8b8f33d6.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/css/3092.95a45cfe.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/css/43.e3b876c5.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)    29048 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/css/main.bf304093.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.911453 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/1074.73973756.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/1168.1d6408e6.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/1307.8ea033f1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/1451.3b0a3e31.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/1479.6709db03.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/178.b5384fd0.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/1792.b8efa879.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    32468 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/2187.9469f035.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2090700 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/2411.a8823789.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/2411.a8823789.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/2469.3e9c3ce9.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/2634.1249dc7a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  3636801 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/2736.914069e5.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/2736.914069e5.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/3053.7e70ec3b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    43574 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/3092.152fd2b7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/3301.1d1b10bb.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/3513.e3e7300a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/3631.be5c35fa.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13223 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/3998.01237fcf.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/4113.1e7eff4d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/4132.49bf3f2c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/4177.69f9f18d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/4185.935c68ec.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   395952 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/4253.749d5244.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/4253.749d5244.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/43.b0aa5759.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/4319.a6745434.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    20661 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/4477.e10e4373.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/4500.b6f348d1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/4666.492dcf72.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/474.87506447.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/5106.44f0ff51.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/5117.04bfe5d3.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/5345.65c91ee7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/5379.6571574f.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   107585 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/5791.9a42fb4b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/6013.8e80e091.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2249519 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/6150.1294fa0d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/6405.ac5a6f23.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   840843 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/656.ae85f8f1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/656.ae85f8f1.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/6718.802da17e.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/6853.d999ac75.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    88545 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/7142.83028745.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/7175.be4076bc.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    65522 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/7217.d970c074.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  3383788 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/7323.2808d029.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/7323.2808d029.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/7602.6175e969.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/7805.51638fbc.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/8005.43974a35.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/8427.d30dffe1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/8477.e948c092.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    15492 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/8492.f56c9d4c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/8570.6de19120.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/8691.9ccf7f89.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/9330.d29313d4.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/9336.2d95d840.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/937.a1248039.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/9656.8c935274.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/9758.6e6d8662.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/9865.fd93213d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  4389164 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/main.8fc4565f.js
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/main.8fc4565f.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.927453 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff
--rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff
--rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff
--rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff
--rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff
--rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff
--rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff
--rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    74492 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    63060 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74052 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62988 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    76860 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44640 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44748 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77664 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77452 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    72892 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30756 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    68356 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    72668 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg
--rw-r--r--   0 runner    (1001) docker     (127)   101906 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif
--rw-r--r--   0 runner    (1001) docker     (127)    73528 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png
--rw-r--r--   0 runner    (1001) docker     (127)    86179 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png
--rw-r--r--   0 runner    (1001) docker     (127)    92182 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg
--rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-04-23 07:03:26.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/string_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/temporary_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.931453 streamlit_nightly-1.33.1.dev20240422/streamlit/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.931453 streamlit_nightly-1.33.1.dev20240422/streamlit/testing/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/testing/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36577 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/testing/v1/app_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    59854 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/testing/v1/element_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/testing/v1/local_script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/testing/v1/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/time_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    44770 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/type_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/url_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/user_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.931453 streamlit_nightly-1.33.1.dev20240422/streamlit/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.931453 streamlit_nightly-1.33.1.dev20240422/streamlit/vendor/ipython/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/vendor/ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/vendor/ipython/modified_sys_path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.931453 streamlit_nightly-1.33.1.dev20240422/streamlit/vendor/pympler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/vendor/pympler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    87925 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/vendor/pympler/asizeof.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.931453 streamlit_nightly-1.33.1.dev20240422/streamlit/watcher/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/watcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/watcher/event_based_path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/watcher/local_sources_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/watcher/path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/watcher/polling_path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/watcher/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.931453 streamlit_nightly-1.33.1.dev20240422/streamlit/web/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/web/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/web/cache_storage_manager_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/web/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.935453 streamlit_nightly-1.33.1.dev20240422/streamlit/web/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/web/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/web/server/app_static_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/web/server/browser_websocket_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/web/server/component_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/web/server/media_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/web/server/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/web/server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/web/server/server_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/web/server/stats_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/web/server/upload_file_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/streamlit/web/server/websocket_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.935453 streamlit_nightly-1.33.1.dev20240422/streamlit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-23 07:03:27.000000 streamlit_nightly-1.33.1.dev20240422/streamlit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23202 2024-04-23 07:03:27.000000 streamlit_nightly-1.33.1.dev20240422/streamlit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 07:03:27.000000 streamlit_nightly-1.33.1.dev20240422/streamlit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 07:03:27.000000 streamlit_nightly-1.33.1.dev20240422/streamlit_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 06:59:36.000000 streamlit_nightly-1.33.1.dev20240422/streamlit_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-23 07:03:27.000000 streamlit_nightly-1.33.1.dev20240422/streamlit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 07:03:27.000000 streamlit_nightly-1.33.1.dev20240422/streamlit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:03:28.935453 streamlit_nightly-1.33.1.dev20240422/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-23 06:57:47.000000 streamlit_nightly-1.33.1.dev20240422/tests/testutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.115748 streamlit_nightly-1.33.1.dev20240423/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-24 07:02:38.115748 streamlit_nightly-1.33.1.dev20240423/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:37.987748 streamlit_nightly-1.33.1.dev20240423/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/bin/streamlit.cmd
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 07:02:38.115748 streamlit_nightly-1.33.1.dev20240423/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:37.995748 streamlit_nightly-1.33.1.dev20240423/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/case_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/cli_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/code_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/color_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/column_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:37.995748 streamlit_nightly-1.33.1.dev20240423/streamlit/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/commands/execution_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/commands/experimental_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/commands/page_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:37.995748 streamlit_nightly-1.33.1.dev20240423/streamlit/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:37.995748 streamlit_nightly-1.33.1.dev20240423/streamlit/components/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/components/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/components/lib/local_component_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:37.995748 streamlit_nightly-1.33.1.dev20240423/streamlit/components/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/components/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/components/types/base_component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/components/types/base_custom_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:37.995748 streamlit_nightly-1.33.1.dev20240423/streamlit/components/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/components/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/components/v1/component_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/components/v1/component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/components/v1/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/components/v1/custom_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43895 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/config_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/config_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:37.999748 streamlit_nightly-1.33.1.dev20240423/streamlit/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/connections/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/connections/snowflake_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/connections/snowpark_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12141 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/connections/sql_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/connections/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33936 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/delta_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/deprecation_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/development.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/echo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.003748 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/altair_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57049 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/arrow_altair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/arrow_vega_lite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/balloons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/bokeh_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/deck_gl_json_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/dialog_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/doc_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12068 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/graphviz_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/heading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/iframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27373 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/layouts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.007748 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/lib/column_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51087 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/lib/column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/lib/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/lib/dicttools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/lib/mutable_status_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/lib/pandas_styler_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/lib/streamlit_plotly_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/lib/subtitle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29664 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/plotly_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/pyplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/snow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/toast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.007748 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31409 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/camera_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13445 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12139 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8925 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35827 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/data_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17437 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/file_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/multiselect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17819 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/number_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12608 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13225 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/select_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11448 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/selectbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26434 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21899 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/text_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29620 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/time_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/elements/write.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73749 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/env_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/error_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.007748 streamlit_nightly-1.33.1.dev20240423/streamlit/external/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.011748 streamlit_nightly-1.33.1.dev20240423/streamlit/external/langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/external/langchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/external/langchain/streamlit_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/folder_black_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/git_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.011748 streamlit_nightly-1.33.1.dev20240423/streamlit/hello/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/hello/Hello.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/hello/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.011748 streamlit_nightly-1.33.1.dev20240423/streamlit/hello/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/hello/pages/0_Animation_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/hello/pages/1_Plotting_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/hello/pages/2_Mapping_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/hello/pages/3_DataFrame_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/hello/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/js_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/net_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.039748 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Alert_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Alert_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/AppPage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/AppPage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ArrowNamedDataSet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ArrowNamedDataSet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ArrowVegaLiteChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ArrowVegaLiteChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Arrow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Arrow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Audio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Audio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/AutoRerun_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/AutoRerun_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/BackMsg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/BackMsg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Balloons_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Balloons_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Block_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Block_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/BokehChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/BokehChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Button_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Button_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/CameraInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/CameraInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ChatInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ChatInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Checkbox_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Checkbox_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ClientState_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ClientState_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Code_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Code_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ColorPicker_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ColorPicker_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Components_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Components_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/DataFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/DataFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/DateInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/DateInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/DeckGlJsonChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/DeckGlJsonChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Delta_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Delta_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/DocString_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/DocString_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/DownloadButton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/DownloadButton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Element_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Element_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Empty_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Empty_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Exception_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Exception_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Favicon_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Favicon_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/FileUploader_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/FileUploader_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ForwardMsg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ForwardMsg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/GitInfo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/GitInfo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/GraphVizChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/GraphVizChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Heading_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Heading_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Html_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Html_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/IFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/IFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Image_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Image_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Json_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Json_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/LabelVisibilityMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/LabelVisibilityMessage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/LinkButton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/LinkButton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Markdown_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Markdown_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Metric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Metric_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/MultiSelect_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/MultiSelect_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/NamedDataSet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/NamedDataSet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/NewSession_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/NewSession_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/NumberInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/NumberInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PageConfig_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PageConfig_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PageInfo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PageInfo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PageLink_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PageLink_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PageNotFound_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PageNotFound_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PageProfile_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PageProfile_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PagesChanged_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PagesChanged_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ParentMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ParentMessage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PlotlyChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PlotlyChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Progress_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Progress_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Radio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Radio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/RootContainer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/RootContainer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Selectbox_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Selectbox_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/SessionEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/SessionEvent_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/SessionStatus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/SessionStatus_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Skeleton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Skeleton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Slider_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Slider_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Snow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Snow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Spinner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Spinner_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/TextArea_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/TextArea_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/TextInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/TextInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Text_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Text_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/TimeInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/TimeInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Toast_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Toast_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/VegaLiteChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/VegaLiteChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Video_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Video_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/WidgetStates_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/WidgetStates_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/openmetrics_data_model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-04-24 06:58:52.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/proto/openmetrics_data_model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.043748 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36802 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/app_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.043748 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/cache_data_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/cache_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21616 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/cache_resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/cache_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17527 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/cache_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17358 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/cached_message_replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18986 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.043748 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/storage/cache_storage_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/storage/dummy_cache_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/storage/local_disk_cache_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/connection_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/forward_msg_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/forward_msg_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/fragment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.043748 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/legacy_caching/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/legacy_caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27873 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/legacy_caching/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/legacy_caching/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/media_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/media_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/memory_media_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/memory_session_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/memory_uploaded_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/metrics_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29567 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/runtime_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/script_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.047748 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/scriptrunner/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/scriptrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/scriptrunner/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/scriptrunner/magic_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/scriptrunner/script_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/scriptrunner/script_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/scriptrunner/script_run_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/scriptrunner/script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/session_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.047748 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/state/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/state/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/state/query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/state/query_params_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/state/safe_session_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27500 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/state/session_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/state/session_state_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/state/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/uploaded_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/websocket_session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/source_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.047748 streamlit_nightly-1.33.1.dev20240423/streamlit/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14380 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-24 06:59:23.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:37.987748 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.047748 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/css/2411.8b8f33d6.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/css/3092.95a45cfe.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/css/43.e3b876c5.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)    29048 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/css/main.bf304093.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.087748 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/1074.73973756.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/1168.1d6408e6.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/1307.8ea033f1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/1451.3b0a3e31.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/1479.6709db03.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/178.7bea8c5d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/1792.b8efa879.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    32468 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/2187.9469f035.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2090700 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/2411.a8823789.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/2411.a8823789.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/2469.3e9c3ce9.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/2634.1249dc7a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3636801 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/2736.914069e5.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/2736.914069e5.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/3053.7e70ec3b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    43574 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/3092.152fd2b7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/3301.1d1b10bb.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/3513.e3e7300a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/3631.be5c35fa.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13223 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/3998.01237fcf.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/4113.1e7eff4d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/4132.49bf3f2c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/4177.69f9f18d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/4185.935c68ec.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   395952 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/4253.749d5244.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/4253.749d5244.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/43.b0aa5759.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/4319.a6745434.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20661 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/4477.e10e4373.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/4500.b6f348d1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/4666.492dcf72.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/474.87506447.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/5106.44f0ff51.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/5117.04bfe5d3.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/5345.65c91ee7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/5379.6571574f.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   107585 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/5791.9a42fb4b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/6013.8e80e091.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2249519 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/6150.1294fa0d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/6405.ac5a6f23.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   840843 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/656.ae85f8f1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/656.ae85f8f1.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/6718.802da17e.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/6853.d999ac75.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    88545 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/7142.83028745.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/7175.be4076bc.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    65522 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/7217.d970c074.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3383788 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/7323.2808d029.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/7323.2808d029.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/7602.6175e969.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/7805.51638fbc.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/8005.43974a35.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/8427.d30dffe1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/8477.e948c092.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15492 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/8492.f56c9d4c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/8570.6de19120.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/8691.9ccf7f89.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/9330.2b4c99e0.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/9336.2d95d840.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/937.a1248039.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/9656.8c935274.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/9758.6e6d8662.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/9865.fd93213d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  4390905 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/main.d3201242.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/main.d3201242.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.107748 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    74492 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63060 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74052 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62988 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    76860 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44640 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44748 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77664 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77452 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    72892 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30756 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    68356 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    72668 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   101906 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    73528 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    86179 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92182 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-04-24 07:02:35.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/string_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/temporary_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.107748 streamlit_nightly-1.33.1.dev20240423/streamlit/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.107748 streamlit_nightly-1.33.1.dev20240423/streamlit/testing/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/testing/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36577 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/testing/v1/app_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59854 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/testing/v1/element_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/testing/v1/local_script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/testing/v1/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44770 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/type_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/url_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/user_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.107748 streamlit_nightly-1.33.1.dev20240423/streamlit/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.107748 streamlit_nightly-1.33.1.dev20240423/streamlit/vendor/ipython/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/vendor/ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/vendor/ipython/modified_sys_path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.107748 streamlit_nightly-1.33.1.dev20240423/streamlit/vendor/pympler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/vendor/pympler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    87925 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/vendor/pympler/asizeof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.107748 streamlit_nightly-1.33.1.dev20240423/streamlit/watcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/watcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/watcher/event_based_path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/watcher/local_sources_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/watcher/path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/watcher/polling_path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/watcher/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.111748 streamlit_nightly-1.33.1.dev20240423/streamlit/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/web/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/web/cache_storage_manager_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/web/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.111748 streamlit_nightly-1.33.1.dev20240423/streamlit/web/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/web/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/web/server/app_static_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/web/server/browser_websocket_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/web/server/component_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/web/server/media_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/web/server/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/web/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/web/server/server_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/web/server/stats_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/web/server/upload_file_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/streamlit/web/server/websocket_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.111748 streamlit_nightly-1.33.1.dev20240423/streamlit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-24 07:02:36.000000 streamlit_nightly-1.33.1.dev20240423/streamlit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23202 2024-04-24 07:02:36.000000 streamlit_nightly-1.33.1.dev20240423/streamlit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 07:02:36.000000 streamlit_nightly-1.33.1.dev20240423/streamlit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-24 07:02:36.000000 streamlit_nightly-1.33.1.dev20240423/streamlit_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 06:58:46.000000 streamlit_nightly-1.33.1.dev20240423/streamlit_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-24 07:02:36.000000 streamlit_nightly-1.33.1.dev20240423/streamlit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 07:02:36.000000 streamlit_nightly-1.33.1.dev20240423/streamlit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:02:38.111748 streamlit_nightly-1.33.1.dev20240423/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-24 06:56:58.000000 streamlit_nightly-1.33.1.dev20240423/tests/testutil.py
```

### Comparing `streamlit_nightly-1.33.1.dev20240422/PKG-INFO` & `streamlit_nightly-1.33.1.dev20240423/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nightly
-Version: 1.33.1.dev20240422
+Version: 1.33.1.dev20240423
 Summary: A faster way to build and share data apps
 Home-page: https://streamlit.io
 Author: Snowflake Inc
 Author-email: hello@streamlit.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/streamlit/streamlit
 Project-URL: Bug Tracker, https://github.com/streamlit/streamlit/issues
```

### Comparing `streamlit_nightly-1.33.1.dev20240422/bin/streamlit.cmd` & `streamlit_nightly-1.33.1.dev20240423/bin/streamlit.cmd`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/setup.py` & `streamlit_nightly-1.33.1.dev20240423/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 
 THIS_DIRECTORY = Path(__file__).parent
 
-VERSION = "1.33.1.dev20240422"  # PEP-440
+VERSION = "1.33.1.dev20240423"  # PEP-440
 
 # IMPORTANT: We should try very hard *not* to add dependencies to Streamlit.
 # And if you do add one, make the required version as general as possible:
 # - Include relevant lower bound for any features we use from our dependencies
 # - Always include the lower bound as >= VERSION, to keep testing min versions easy
 # - And include an upper bound that's < NEXT_MAJOR_VERSION
 INSTALL_REQUIRES = [
```

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/__main__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/__main__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/case_converters.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/case_converters.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/cli_util.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/cli_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/code_util.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/code_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/color_util.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/color_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/column_config.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/column_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/commands/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/commands/execution_control.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/commands/execution_control.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/commands/experimental_query_params.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/commands/experimental_query_params.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/commands/page_config.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/commands/page_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/components/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/components/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/components/lib/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/components/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/components/lib/local_component_registry.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/components/lib/local_component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/components/types/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/components/types/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/components/types/base_component_registry.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/components/types/base_component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/components/types/base_custom_component.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/components/types/base_custom_component.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/components/v1/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/components/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/components/v1/component_arrow.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/components/v1/component_arrow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/components/v1/component_registry.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/components/v1/component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/components/v1/components.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/components/v1/components.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/components/v1/custom_component.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/components/v1/custom_component.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/config.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/config_option.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/config_option.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/config_util.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/config_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/connections/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/connections/base_connection.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/connections/base_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/connections/snowflake_connection.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/connections/snowflake_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/connections/snowpark_connection.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/connections/snowpark_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/connections/sql_connection.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/connections/sql_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/connections/util.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/connections/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/constants.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/constants.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/cursor.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/cursor.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/delta_generator.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/delta_generator.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/deprecation_util.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/deprecation_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/development.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/development.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/echo.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/echo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/alert.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/alert.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/altair_utils.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/altair_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/arrow.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/arrow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/arrow_altair.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/arrow_altair.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/arrow_vega_lite.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/arrow_vega_lite.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/balloons.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/balloons.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/bokeh_chart.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/bokeh_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/code.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/code.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/deck_gl_json_chart.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/deck_gl_json_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/dialog_decorator.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/dialog_decorator.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/doc_string.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/doc_string.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/empty.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/empty.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/exception.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/exception.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/form.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/form.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/graphviz_chart.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/graphviz_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/heading.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/heading.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/html.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/html.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/iframe.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/iframe.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/image.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/image.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/json.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/json.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/layouts.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/layouts.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/lib/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/lib/column_config_utils.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/lib/column_config_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/lib/column_types.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/lib/column_types.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/lib/dialog.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/lib/dialog.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/lib/dicttools.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/lib/dicttools.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/lib/mutable_status_container.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/lib/mutable_status_container.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/lib/pandas_styler_utils.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/lib/pandas_styler_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/lib/streamlit_plotly_theme.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/lib/streamlit_plotly_theme.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/lib/subtitle_utils.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/lib/subtitle_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/map.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/map.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/markdown.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/markdown.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/media.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/media.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 from streamlit import runtime, type_util, url_util
 from streamlit.elements.lib.subtitle_utils import process_subtitle_data
 from streamlit.errors import StreamlitAPIException
 from streamlit.proto.Audio_pb2 import Audio as AudioProto
 from streamlit.proto.Video_pb2 import Video as VideoProto
 from streamlit.runtime import caching
 from streamlit.runtime.metrics_util import gather_metrics
+from streamlit.runtime.scriptrunner import get_script_run_ctx
+from streamlit.runtime.state.common import compute_widget_id
 from streamlit.time_util import time_to_seconds
 
 if TYPE_CHECKING:
     from typing import Any
 
     from numpy import typing as npt
 
@@ -65,14 +67,15 @@
         data: MediaData,
         format: str = "audio/wav",
         start_time: MediaTime = 0,
         *,
         sample_rate: int | None = None,
         end_time: MediaTime | None = None,
         loop: bool = False,
+        autoplay: bool = False,
     ) -> DeltaGenerator:
         """Display an audio player.
 
         Parameters
         ----------
         data : str, bytes, BytesIO, numpy.ndarray, or file
             Raw audio data, filename, or a URL pointing to the file to load.
@@ -114,14 +117,19 @@
               Timedelta constructor <https://pandas.pydata.org/docs/reference/api/pandas.Timedelta.html>`_,
               e.g. ``"2 minute"``, ``"20s"``, or ``"1m14s"``.
             * A ``timedelta`` object from `Python's built-in datetime library
               <https://docs.python.org/3/library/datetime.html#timedelta-objects>`_,
               e.g. ``timedelta(seconds=70)``.
         loop: bool
             Whether the audio should loop playback.
+        autoplay: bool
+            Whether the audio should start playing automatically.
+            Browsers will not autoplay audio files if the user has not interacted with
+            the page yet, for example by clicking on the page while it loads.
+            Defaults to False.
 
         Examples
         --------
         To display an audio player for a local file, specify the file's string
         path and format.
 
         >>> import streamlit as st
@@ -179,27 +187,30 @@
             audio_proto,
             data,
             format,
             start_time,
             sample_rate,
             end_time,
             loop,
+            autoplay,
         )
         return self.dg._enqueue("audio", audio_proto)
 
     @gather_metrics("video")
     def video(
         self,
         data: MediaData,
         format: str = "video/mp4",
         start_time: MediaTime = 0,
         *,  # keyword-only arguments:
         subtitles: SubtitleData = None,
         end_time: MediaTime | None = None,
         loop: bool = False,
+        autoplay: bool = False,
+        muted: bool = False,
     ) -> DeltaGenerator:
         """Display a video player.
 
         Parameters
         ----------
         data : str, bytes, io.BytesIO, numpy.ndarray, or file
             Raw video data, filename, or URL pointing to a video to load.
@@ -259,14 +270,23 @@
               Timedelta constructor <https://pandas.pydata.org/docs/reference/api/pandas.Timedelta.html>`_,
               e.g. ``"2 minute"``, ``"20s"``, or ``"1m14s"``.
             * A ``timedelta`` object from `Python's built-in datetime library
               <https://docs.python.org/3/library/datetime.html#timedelta-objects>`_,
               e.g. ``timedelta(seconds=70)``.
         loop: bool
             Whether the video should loop playback.
+        autoplay: bool
+            Whether the video should start playing automatically.
+            Browsers will not autoplay video files if the user has not interacted with
+            the page yet, for example by clicking on the page while it loads.
+            To enable autoplay without user interaction, you can set muted=True.
+            Defaults to False.
+        muted: bool
+            Whether the video should play with the audio silenced. This can be used to
+            enable autoplay without user interaction. Defaults to False.
 
         Example
         -------
         >>> import streamlit as st
         >>>
         >>> video_file = open('myvideo.mp4', 'rb')
         >>> video_bytes = video_file.read()
@@ -310,28 +330,29 @@
            Some videos may not display if they are encoded using MP4V (which is an export option in OpenCV), as this codec is
            not widely supported by browsers. Converting your video to H.264 will allow the video to be displayed in Streamlit.
            See this `StackOverflow post <https://stackoverflow.com/a/49535220/2394542>`_ or this
            `Streamlit forum post <https://discuss.streamlit.io/t/st-video-doesnt-show-opencv-generated-mp4/3193/2>`_
            for more information.
 
         """
-
         start_time, end_time = _parse_start_time_end_time(start_time, end_time)
 
         video_proto = VideoProto()
         coordinates = self.dg._get_delta_path_str()
         marshall_video(
             coordinates,
             video_proto,
             data,
             format,
             start_time,
             subtitles,
             end_time,
             loop,
+            autoplay,
+            muted,
         )
         return self.dg._enqueue("video", video_proto)
 
     @property
     def dg(self) -> DeltaGenerator:
         """Get our DeltaGenerator."""
         return cast("DeltaGenerator", self)
@@ -430,14 +451,16 @@
     proto: VideoProto,
     data: MediaData,
     mimetype: str = "video/mp4",
     start_time: int = 0,
     subtitles: SubtitleData = None,
     end_time: int | None = None,
     loop: bool = False,
+    autoplay: bool = False,
+    muted: bool = False,
 ) -> None:
     """Marshalls a video proto, using url processors as needed.
 
     Parameters
     ----------
     coordinates : str
     proto : the proto to fill. Must have a string field called "data".
@@ -463,20 +486,30 @@
         * io.BytesIO: A BytesIO stream that contains valid '.vtt' or '.srt' formatted subtitle data.
         When provided, subtitles are displayed by default. For multiple tracks, the first one is displayed by default.
         Not supported for YouTube videos.
     end_time: int
             The time at which this element should stop playing
     loop: bool
         Whether the video should loop playback.
+    autoplay: bool
+        Whether the video should start playing automatically.
+        Browsers will not autoplay video files if the user has not interacted with
+        the page yet, for example by clicking on the page while it loads.
+        To enable autoplay without user interaction, you can set muted=True.
+        Defaults to False.
+    muted: bool
+        Whether the video should play with the audio silenced. This can be used to
+        enable autoplay without user interaction. Defaults to False.
     """
 
     if start_time < 0 or (end_time is not None and end_time <= start_time):
         raise StreamlitAPIException("Invalid start_time and end_time combination.")
 
     proto.start_time = start_time
+    proto.muted = muted
 
     if end_time is not None:
         proto.end_time = end_time
     proto.loop = loop
 
     # "type" distinguishes between YouTube and non-YouTube links
     proto.type = VideoProto.Type.NATIVE
@@ -527,14 +560,31 @@
                     subtitle_coordinates, subtitle_data, label
                 )
             except (TypeError, ValueError) as original_err:
                 raise StreamlitAPIException(
                     f"Failed to process the provided subtitle: {label}"
                 ) from original_err
 
+    if autoplay:
+        ctx = get_script_run_ctx()
+        proto.autoplay = autoplay
+        id = compute_widget_id(
+            "video",
+            url=proto.url,
+            mimetype=mimetype,
+            start_time=start_time,
+            end_time=end_time,
+            loop=loop,
+            autoplay=autoplay,
+            muted=muted,
+            page=ctx.page_script_hash if ctx else None,
+        )
+
+        proto.id = id
+
 
 def _parse_start_time_end_time(
     start_time: MediaTime, end_time: MediaTime | None
 ) -> tuple[int, int | None]:
     """Parse start_time and end_time and return them as int."""
 
     try:
@@ -643,14 +693,15 @@
     proto: AudioProto,
     data: MediaData,
     mimetype: str = "audio/wav",
     start_time: int = 0,
     sample_rate: int | None = None,
     end_time: int | None = None,
     loop: bool = False,
+    autoplay: bool = False,
 ) -> None:
     """Marshalls an audio proto, using data and url processors as needed.
 
     Parameters
     ----------
     coordinates : str
     proto : The proto to fill. Must have a string field called "url".
@@ -666,14 +717,17 @@
         The time from which this element should start playing. (default: 0)
     sample_rate: int or None
         Optional param to provide sample_rate in case of numpy array
     end_time: int
         The time at which this element should stop playing
     loop: bool
         Whether the audio should loop playback.
+    autoplay : bool
+        Whether the audio should start playing automatically.
+        Browsers will not autoplay audio files if the user has not interacted with the page yet.
     """
 
     proto.start_time = start_time
     if end_time is not None:
         proto.end_time = end_time
     proto.loop = loop
 
@@ -681,7 +735,23 @@
         data, allowed_schemas=("http", "https", "data")
     ):
         proto.url = data
 
     else:
         data = _maybe_convert_to_wav_bytes(data, sample_rate)
         _marshall_av_media(coordinates, proto, data, mimetype)
+
+    if autoplay:
+        ctx = get_script_run_ctx()
+        proto.autoplay = autoplay
+        id = compute_widget_id(
+            "audio",
+            url=proto.url,
+            mimetype=mimetype,
+            start_time=start_time,
+            sample_rate=sample_rate,
+            end_time=end_time,
+            loop=loop,
+            autoplay=autoplay,
+            page=ctx.page_script_hash if ctx else None,
+        )
+        proto.id = id
```

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/metric.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/metric.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/plotly_chart.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/progress.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/progress.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/pyplot.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/pyplot.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/snow.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/snow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/spinner.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/spinner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/text.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/text.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/toast.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/toast.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/utils.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/button.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/button.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/camera_input.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/camera_input.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/chat.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/chat.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/checkbox.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/color_picker.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/color_picker.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/data_editor.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/data_editor.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/file_uploader.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/file_uploader.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/multiselect.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/multiselect.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/number_input.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/number_input.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/radio.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/select_slider.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/select_slider.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/selectbox.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/selectbox.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/slider.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/text_widgets.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/text_widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/widgets/time_widgets.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/widgets/time_widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/elements/write.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/elements/write.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/emojis.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/emojis.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/env_util.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/env_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/error_util.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/error_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/errors.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/errors.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/external/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/external/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/external/langchain/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/external/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/external/langchain/streamlit_callback_handler.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/external/langchain/streamlit_callback_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/file_util.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/file_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/folder_black_list.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/folder_black_list.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/git_util.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/git_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/hello/Hello.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/hello/Hello.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/hello/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/hello/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/hello/pages/0_Animation_Demo.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/hello/pages/0_Animation_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/hello/pages/1_Plotting_Demo.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/hello/pages/1_Plotting_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/hello/pages/2_Mapping_Demo.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/hello/pages/2_Mapping_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/hello/pages/3_DataFrame_Demo.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/hello/pages/3_DataFrame_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/hello/utils.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/hello/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/js_number.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/js_number.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/logger.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/logger.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/net_util.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/net_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/platform.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/platform.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Alert_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Alert_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Alert_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/AppPage_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/AppPage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/AppPage_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/AppPage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ArrowNamedDataSet_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ArrowNamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ArrowNamedDataSet_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ArrowNamedDataSet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ArrowVegaLiteChart_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ArrowVegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ArrowVegaLiteChart_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ArrowVegaLiteChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Arrow_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Arrow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Arrow_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Arrow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Audio_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Audio_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bstreamlit/proto/Audio.proto\"h\n\x05\x41udio\x12\x0b\n\x03url\x18\x05 \x01(\t\x12\x12\n\nstart_time\x18\x03 \x01(\x05\x12\x10\n\x08\x65nd_time\x18\x06 \x01(\x05\x12\x0c\n\x04loop\x18\x07 \x01(\x08J\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x04\x10\x05R\x04\x64\x61taR\x06\x66ormatB*\n\x1c\x63om.snowflake.apps.streamlitB\nAudioProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bstreamlit/proto/Audio.proto\"\x86\x01\n\x05\x41udio\x12\x0b\n\x03url\x18\x05 \x01(\t\x12\x12\n\nstart_time\x18\x03 \x01(\x05\x12\x10\n\x08\x65nd_time\x18\x06 \x01(\x05\x12\x0c\n\x04loop\x18\x07 \x01(\x08\x12\x10\n\x08\x61utoplay\x18\x08 \x01(\x08\x12\n\n\x02id\x18\t \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x04\x10\x05R\x04\x64\x61taR\x06\x66ormatB*\n\x1c\x63om.snowflake.apps.streamlitB\nAudioProtob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'streamlit.proto.Audio_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034com.snowflake.apps.streamlitB\nAudioProto'
-  _AUDIO._serialized_start=31
-  _AUDIO._serialized_end=135
+  _AUDIO._serialized_start=32
+  _AUDIO._serialized_end=166
 # @@protoc_insertion_point(module_scope)
```

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Audio_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Toast_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -24,32 +24,25 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class Audio(google.protobuf.message.Message):
+class Toast(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    URL_FIELD_NUMBER: builtins.int
-    START_TIME_FIELD_NUMBER: builtins.int
-    END_TIME_FIELD_NUMBER: builtins.int
-    LOOP_FIELD_NUMBER: builtins.int
-    url: builtins.str
-    start_time: builtins.int
-    """The currentTime attribute of the HTML <audio> tag's <source> subtag."""
-    end_time: builtins.int
-    """The time at which the audio should stop playing. If not specified, plays to the end."""
-    loop: builtins.bool
-    """Indicates whether the audio should start over from the beginning once it ends."""
+    BODY_FIELD_NUMBER: builtins.int
+    ICON_FIELD_NUMBER: builtins.int
+    body: builtins.str
+    """Display message"""
+    icon: builtins.str
+    """Emoji"""
     def __init__(
         self,
         *,
-        url: builtins.str = ...,
-        start_time: builtins.int = ...,
-        end_time: builtins.int = ...,
-        loop: builtins.bool = ...,
+        body: builtins.str = ...,
+        icon: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["end_time", b"end_time", "loop", b"loop", "start_time", b"start_time", "url", b"url"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["body", b"body", "icon", b"icon"]) -> None: ...
 
-global___Audio = Audio
+global___Toast = Toast
```

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/AutoRerun_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/AutoRerun_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/AutoRerun_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/AutoRerun_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/BackMsg_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/BackMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/BackMsg_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/BackMsg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Balloons_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Balloons_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Balloons_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Balloons_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Block_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Block_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Block_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Block_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/BokehChart_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/BokehChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/BokehChart_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/BokehChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Button_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Button_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Button_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Button_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/CameraInput_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/CameraInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/CameraInput_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/CameraInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ChatInput_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ChatInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ChatInput_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ChatInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Checkbox_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Checkbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Checkbox_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Checkbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ClientState_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ClientState_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ClientState_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ClientState_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Code_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Code_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Code_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ColorPicker_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ColorPicker_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ColorPicker_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ColorPicker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Common_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Common_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Common_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Components_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Components_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Components_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Components_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/DataFrame_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/DataFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/DataFrame_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/DataFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/DateInput_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/DateInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/DateInput_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/DateInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/DeckGlJsonChart_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/DeckGlJsonChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/DeckGlJsonChart_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/DeckGlJsonChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Delta_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Delta_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Delta_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Delta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/DocString_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/DocString_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/DocString_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/DocString_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/DownloadButton_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/DownloadButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/DownloadButton_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/DownloadButton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Element_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Element_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Element_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Element_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Empty_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Empty_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Empty_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Empty_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Exception_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Exception_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Exception_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Exception_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Favicon_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Favicon_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Favicon_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Favicon_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/FileUploader_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/FileUploader_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/FileUploader_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/FileUploader_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ForwardMsg_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ForwardMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ForwardMsg_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ForwardMsg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/GitInfo_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/GitInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/GitInfo_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/GitInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/GraphVizChart_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/GraphVizChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/GraphVizChart_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/GraphVizChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Heading_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Heading_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Heading_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Heading_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Html_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Html_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Html_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Html_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/IFrame_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/IFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/IFrame_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/IFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Image_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Image_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Image_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Image_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Json_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Json_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Json_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Json_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/LabelVisibilityMessage_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/LabelVisibilityMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/LabelVisibilityMessage_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/LabelVisibilityMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/LinkButton_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/LinkButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/LinkButton_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/LinkButton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Markdown_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Markdown_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Markdown_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Markdown_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Metric_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Metric_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Metric_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Metric_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/MultiSelect_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/MultiSelect_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/MultiSelect_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/MultiSelect_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/NamedDataSet_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/NamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/NamedDataSet_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/NamedDataSet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/NewSession_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/NewSession_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/NewSession_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/NewSession_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/NumberInput_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/NumberInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/NumberInput_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/NumberInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PageConfig_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PageConfig_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PageConfig_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PageConfig_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PageInfo_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PageInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PageInfo_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PageInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PageLink_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PageLink_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PageLink_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PageLink_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PageNotFound_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PageNotFound_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PageNotFound_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PageNotFound_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PageProfile_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PageProfile_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PageProfile_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PageProfile_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PagesChanged_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PagesChanged_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PagesChanged_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PagesChanged_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ParentMessage_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ParentMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/ParentMessage_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/ParentMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PlotlyChart_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PlotlyChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/PlotlyChart_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/PlotlyChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Progress_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Progress_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Progress_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Progress_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Radio_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Radio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Radio_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Radio_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/RootContainer_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/RootContainer_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/RootContainer_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/RootContainer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Selectbox_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Selectbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Selectbox_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Selectbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/SessionEvent_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/SessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/SessionEvent_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/SessionEvent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/SessionStatus_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/SessionStatus_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/SessionStatus_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/SessionStatus_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Skeleton_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Skeleton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Skeleton_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Skeleton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Slider_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Slider_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Slider_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Slider_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Snow_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Snow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Snow_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Snow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Spinner_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Spinner_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Spinner_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Spinner_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/TextArea_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/TextArea_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/TextArea_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/TextArea_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/TextInput_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/TextInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/TextInput_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/TextInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Text_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Text_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Text_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Text_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/TimeInput_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/TimeInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/TimeInput_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/TimeInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Toast_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Toast_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Toast_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Audio_pb2.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -24,25 +24,38 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class Toast(google.protobuf.message.Message):
+class Audio(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    BODY_FIELD_NUMBER: builtins.int
-    ICON_FIELD_NUMBER: builtins.int
-    body: builtins.str
-    """Display message"""
-    icon: builtins.str
-    """Emoji"""
+    URL_FIELD_NUMBER: builtins.int
+    START_TIME_FIELD_NUMBER: builtins.int
+    END_TIME_FIELD_NUMBER: builtins.int
+    LOOP_FIELD_NUMBER: builtins.int
+    AUTOPLAY_FIELD_NUMBER: builtins.int
+    ID_FIELD_NUMBER: builtins.int
+    url: builtins.str
+    start_time: builtins.int
+    """The currentTime attribute of the HTML <audio> tag's <source> subtag."""
+    end_time: builtins.int
+    """The time at which the audio should stop playing. If not specified, plays to the end."""
+    loop: builtins.bool
+    """Indicates whether the audio should start over from the beginning once it ends."""
+    autoplay: builtins.bool
+    id: builtins.str
     def __init__(
         self,
         *,
-        body: builtins.str = ...,
-        icon: builtins.str = ...,
+        url: builtins.str = ...,
+        start_time: builtins.int = ...,
+        end_time: builtins.int = ...,
+        loop: builtins.bool = ...,
+        autoplay: builtins.bool = ...,
+        id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["body", b"body", "icon", b"icon"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["autoplay", b"autoplay", "end_time", b"end_time", "id", b"id", "loop", b"loop", "start_time", b"start_time", "url", b"url"]) -> None: ...
 
-global___Toast = Toast
+global___Audio = Audio
```

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/VegaLiteChart_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/VegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/VegaLiteChart_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/VegaLiteChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Video_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Video_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bstreamlit/proto/Video.proto\"+\n\rSubtitleTrack\x12\r\n\x05label\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\"\xda\x01\n\x05Video\x12\x0b\n\x03url\x18\x06 \x01(\t\x12\x12\n\nstart_time\x18\x03 \x01(\x05\x12\x19\n\x04type\x18\x05 \x01(\x0e\x32\x0b.Video.Type\x12!\n\tsubtitles\x18\x07 \x03(\x0b\x32\x0e.SubtitleTrack\x12\x10\n\x08\x65nd_time\x18\x08 \x01(\x05\x12\x0c\n\x04loop\x18\t \x01(\x08\"2\n\x04Type\x12\n\n\x06UNUSED\x10\x00\x12\n\n\x06NATIVE\x10\x01\x12\x12\n\x0eYOUTUBE_IFRAME\x10\x02J\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x04\x10\x05R\x06\x66ormatR\x04\x64\x61taB*\n\x1c\x63om.snowflake.apps.streamlitB\nVideoProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bstreamlit/proto/Video.proto\"+\n\rSubtitleTrack\x12\r\n\x05label\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\"\x87\x02\n\x05Video\x12\x0b\n\x03url\x18\x06 \x01(\t\x12\x12\n\nstart_time\x18\x03 \x01(\x05\x12\x19\n\x04type\x18\x05 \x01(\x0e\x32\x0b.Video.Type\x12!\n\tsubtitles\x18\x07 \x03(\x0b\x32\x0e.SubtitleTrack\x12\x10\n\x08\x65nd_time\x18\x08 \x01(\x05\x12\x0c\n\x04loop\x18\t \x01(\x08\x12\x10\n\x08\x61utoplay\x18\n \x01(\x08\x12\r\n\x05muted\x18\x0b \x01(\x08\x12\n\n\x02id\x18\x0c \x01(\t\"2\n\x04Type\x12\n\n\x06UNUSED\x10\x00\x12\n\n\x06NATIVE\x10\x01\x12\x12\n\x0eYOUTUBE_IFRAME\x10\x02J\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x04\x10\x05R\x06\x66ormatR\x04\x64\x61taB*\n\x1c\x63om.snowflake.apps.streamlitB\nVideoProtob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'streamlit.proto.Video_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034com.snowflake.apps.streamlitB\nVideoProto'
   _SUBTITLETRACK._serialized_start=31
   _SUBTITLETRACK._serialized_end=74
   _VIDEO._serialized_start=77
-  _VIDEO._serialized_end=295
-  _VIDEO_TYPE._serialized_start=213
-  _VIDEO_TYPE._serialized_end=263
+  _VIDEO._serialized_end=340
+  _VIDEO_TYPE._serialized_start=258
+  _VIDEO_TYPE._serialized_end=308
 # @@protoc_insertion_point(module_scope)
```

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/Video_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/Video_pb2.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -72,33 +72,42 @@
 
     URL_FIELD_NUMBER: builtins.int
     START_TIME_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     SUBTITLES_FIELD_NUMBER: builtins.int
     END_TIME_FIELD_NUMBER: builtins.int
     LOOP_FIELD_NUMBER: builtins.int
+    AUTOPLAY_FIELD_NUMBER: builtins.int
+    MUTED_FIELD_NUMBER: builtins.int
+    ID_FIELD_NUMBER: builtins.int
     url: builtins.str
     """A url pointing to a video file"""
     start_time: builtins.int
     """The currentTime attribute of the HTML <video> tag's <source> subtag."""
     type: global___Video.Type.ValueType
     """Type affects how browser wraps the video in tags: plain HTML5, YouTube..."""
     @property
     def subtitles(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SubtitleTrack]:
         """Repeated field for subtitle tracks"""
     end_time: builtins.int
     """The time at which the video should stop playing. If not specified, plays to the end."""
     loop: builtins.bool
     """Indicates whether the video should start over from the beginning once it ends."""
+    autoplay: builtins.bool
+    muted: builtins.bool
+    id: builtins.str
     def __init__(
         self,
         *,
         url: builtins.str = ...,
         start_time: builtins.int = ...,
         type: global___Video.Type.ValueType = ...,
         subtitles: collections.abc.Iterable[global___SubtitleTrack] | None = ...,
         end_time: builtins.int = ...,
         loop: builtins.bool = ...,
+        autoplay: builtins.bool = ...,
+        muted: builtins.bool = ...,
+        id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["end_time", b"end_time", "loop", b"loop", "start_time", b"start_time", "subtitles", b"subtitles", "type", b"type", "url", b"url"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["autoplay", b"autoplay", "end_time", b"end_time", "id", b"id", "loop", b"loop", "muted", b"muted", "start_time", b"start_time", "subtitles", b"subtitles", "type", b"type", "url", b"url"]) -> None: ...
 
 global___Video = Video
```

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/WidgetStates_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/WidgetStates_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/WidgetStates_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/WidgetStates_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/openmetrics_data_model_pb2.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/openmetrics_data_model_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/proto/openmetrics_data_model_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240423/streamlit/proto/openmetrics_data_model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/app_session.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/app_session.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/cache_data_api.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/cache_data_api.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/cache_errors.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/cache_errors.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/cache_resource_api.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/cache_resource_api.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/cache_type.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/cache_type.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/cache_utils.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/cache_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/cached_message_replay.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/cached_message_replay.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/hashing.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/hashing.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/storage/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/storage/cache_storage_protocol.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/storage/cache_storage_protocol.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/storage/dummy_cache_storage.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/storage/dummy_cache_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/caching/storage/local_disk_cache_storage.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/caching/storage/local_disk_cache_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/connection_factory.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/connection_factory.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/credentials.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/credentials.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/forward_msg_cache.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/forward_msg_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/forward_msg_queue.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/forward_msg_queue.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/fragment.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/fragment.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/legacy_caching/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/legacy_caching/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/legacy_caching/caching.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/legacy_caching/caching.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/legacy_caching/hashing.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/legacy_caching/hashing.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/media_file_manager.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/media_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/media_file_storage.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/media_file_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/memory_media_file_storage.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/memory_media_file_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/memory_session_storage.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/memory_session_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/memory_uploaded_file_manager.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/memory_uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/metrics_util.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/metrics_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/runtime.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/runtime_util.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/runtime_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/script_data.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/script_data.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/scriptrunner/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/scriptrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/scriptrunner/magic.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/scriptrunner/magic.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/scriptrunner/magic_funcs.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/scriptrunner/magic_funcs.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/scriptrunner/script_cache.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/scriptrunner/script_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/scriptrunner/script_requests.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/scriptrunner/script_requests.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/scriptrunner/script_run_context.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/scriptrunner/script_run_context.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/scriptrunner/script_runner.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/scriptrunner/script_runner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/secrets.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/secrets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/session_manager.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/session_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/state/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/state/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/state/common.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/state/common.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/state/query_params.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/state/query_params.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/state/query_params_proxy.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/state/query_params_proxy.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/state/safe_session_state.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/state/safe_session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/state/session_state.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/state/session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/state/session_state_proxy.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/state/session_state_proxy.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/state/widgets.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/state/widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/stats.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/stats.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/uploaded_file_manager.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/runtime/websocket_session_manager.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/runtime/websocket_session_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/source_util.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/source_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/asset-manifest.json` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/asset-manifest.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8258830022075054%*

 * *Differences: {"'entrypoints'": "{insert: [(1, 'static/js/main.d3201242.js')], delete: [1]}",*

 * * "'files'": "{'main.js': './static/js/main.d3201242.js', 'static/js/9330.2b4c99e0.chunk.js': "*

 * *            "'./static/js/9330.2b4c99e0.chunk.js', 'static/js/178.7bea8c5d.chunk.js': "*

 * *            "'./static/js/178.7bea8c5d.chunk.js', delete: ['static/js/9330.d29313d4.chunk.js', "*

 * *            "'static/js/178.b5384fd0.chunk.js']}"}*

```diff
@@ -1,25 +1,25 @@
 {
     "entrypoints": [
         "static/css/main.bf304093.css",
-        "static/js/main.8fc4565f.js"
+        "static/js/main.d3201242.js"
     ],
     "files": {
         "index.html": "./index.html",
         "main.css": "./static/css/main.bf304093.css",
-        "main.js": "./static/js/main.8fc4565f.js",
+        "main.js": "./static/js/main.d3201242.js",
         "static/css/2411.8b8f33d6.chunk.css": "./static/css/2411.8b8f33d6.chunk.css",
         "static/css/3092.95a45cfe.chunk.css": "./static/css/3092.95a45cfe.chunk.css",
         "static/css/43.e3b876c5.chunk.css": "./static/css/43.e3b876c5.chunk.css",
         "static/js/1074.73973756.chunk.js": "./static/js/1074.73973756.chunk.js",
         "static/js/1168.1d6408e6.chunk.js": "./static/js/1168.1d6408e6.chunk.js",
         "static/js/1307.8ea033f1.chunk.js": "./static/js/1307.8ea033f1.chunk.js",
         "static/js/1451.3b0a3e31.chunk.js": "./static/js/1451.3b0a3e31.chunk.js",
         "static/js/1479.6709db03.chunk.js": "./static/js/1479.6709db03.chunk.js",
-        "static/js/178.b5384fd0.chunk.js": "./static/js/178.b5384fd0.chunk.js",
+        "static/js/178.7bea8c5d.chunk.js": "./static/js/178.7bea8c5d.chunk.js",
         "static/js/1792.b8efa879.chunk.js": "./static/js/1792.b8efa879.chunk.js",
         "static/js/2187.9469f035.chunk.js": "./static/js/2187.9469f035.chunk.js",
         "static/js/2411.a8823789.chunk.js": "./static/js/2411.a8823789.chunk.js",
         "static/js/2469.3e9c3ce9.chunk.js": "./static/js/2469.3e9c3ce9.chunk.js",
         "static/js/2634.1249dc7a.chunk.js": "./static/js/2634.1249dc7a.chunk.js",
         "static/js/2736.914069e5.chunk.js": "./static/js/2736.914069e5.chunk.js",
         "static/js/3053.7e70ec3b.chunk.js": "./static/js/3053.7e70ec3b.chunk.js",
@@ -58,15 +58,15 @@
         "static/js/7805.51638fbc.chunk.js": "./static/js/7805.51638fbc.chunk.js",
         "static/js/8005.43974a35.chunk.js": "./static/js/8005.43974a35.chunk.js",
         "static/js/8427.d30dffe1.chunk.js": "./static/js/8427.d30dffe1.chunk.js",
         "static/js/8477.e948c092.chunk.js": "./static/js/8477.e948c092.chunk.js",
         "static/js/8492.f56c9d4c.chunk.js": "./static/js/8492.f56c9d4c.chunk.js",
         "static/js/8570.6de19120.chunk.js": "./static/js/8570.6de19120.chunk.js",
         "static/js/8691.9ccf7f89.chunk.js": "./static/js/8691.9ccf7f89.chunk.js",
-        "static/js/9330.d29313d4.chunk.js": "./static/js/9330.d29313d4.chunk.js",
+        "static/js/9330.2b4c99e0.chunk.js": "./static/js/9330.2b4c99e0.chunk.js",
         "static/js/9336.2d95d840.chunk.js": "./static/js/9336.2d95d840.chunk.js",
         "static/js/937.a1248039.chunk.js": "./static/js/937.a1248039.chunk.js",
         "static/js/9656.8c935274.chunk.js": "./static/js/9656.8c935274.chunk.js",
         "static/js/9758.6e6d8662.chunk.js": "./static/js/9758.6e6d8662.chunk.js",
         "static/js/9865.fd93213d.chunk.js": "./static/js/9865.fd93213d.chunk.js",
         "static/media/KaTeX_AMS-Regular.ttf": "./static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf",
         "static/media/KaTeX_AMS-Regular.woff": "./static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff",
```

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/favicon.png` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/favicon.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/index.html` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no"/><link rel="shortcut icon" href="./favicon.png"/><link rel="preload" href="./static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2" as="font" type="font/woff2" crossorigin><title>Streamlit</title><script>window.prerenderReady=!1</script><script defer="defer" src="./static/js/main.8fc4565f.js"></script><link href="./static/css/main.bf304093.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no"/><link rel="shortcut icon" href="./favicon.png"/><link rel="preload" href="./static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2" as="font" type="font/woff2" crossorigin><title>Streamlit</title><script>window.prerenderReady=!1</script><script defer="defer" src="./static/js/main.d3201242.js"></script><link href="./static/css/main.bf304093.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/css/2411.8b8f33d6.chunk.css` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/css/2411.8b8f33d6.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/css/3092.95a45cfe.chunk.css` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/css/3092.95a45cfe.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/css/43.e3b876c5.chunk.css` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/css/43.e3b876c5.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/css/main.bf304093.css` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/css/main.bf304093.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/1074.73973756.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/1074.73973756.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/1168.1d6408e6.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/1168.1d6408e6.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/1307.8ea033f1.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/1307.8ea033f1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/1451.3b0a3e31.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/1451.3b0a3e31.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/1479.6709db03.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/1479.6709db03.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/1792.b8efa879.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/1792.b8efa879.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/2187.9469f035.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/2187.9469f035.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/2411.a8823789.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/2411.a8823789.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/2469.3e9c3ce9.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/2469.3e9c3ce9.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/2634.1249dc7a.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/2634.1249dc7a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/2736.914069e5.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/2736.914069e5.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/2736.914069e5.chunk.js.LICENSE.txt` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/2736.914069e5.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/3053.7e70ec3b.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/3053.7e70ec3b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/3092.152fd2b7.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/3092.152fd2b7.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/3301.1d1b10bb.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/3301.1d1b10bb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/3513.e3e7300a.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/3513.e3e7300a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/3631.be5c35fa.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/3631.be5c35fa.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/3998.01237fcf.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/3998.01237fcf.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/4113.1e7eff4d.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/4113.1e7eff4d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/4132.49bf3f2c.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/4132.49bf3f2c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/4177.69f9f18d.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/4177.69f9f18d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/4185.935c68ec.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/4185.935c68ec.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/4253.749d5244.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/4253.749d5244.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/43.b0aa5759.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/43.b0aa5759.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/4319.a6745434.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/4319.a6745434.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/4477.e10e4373.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/4477.e10e4373.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/4500.b6f348d1.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/4500.b6f348d1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/4666.492dcf72.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/4666.492dcf72.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/474.87506447.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/474.87506447.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/5106.44f0ff51.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/5106.44f0ff51.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/5117.04bfe5d3.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/5117.04bfe5d3.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/5345.65c91ee7.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/5345.65c91ee7.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/5379.6571574f.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/5379.6571574f.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/5791.9a42fb4b.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/5791.9a42fb4b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/6013.8e80e091.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/6013.8e80e091.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/6150.1294fa0d.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/6150.1294fa0d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/6405.ac5a6f23.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/6405.ac5a6f23.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/656.ae85f8f1.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/656.ae85f8f1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/6718.802da17e.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/6718.802da17e.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/6853.d999ac75.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/6853.d999ac75.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/7142.83028745.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/7142.83028745.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/7175.be4076bc.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/7175.be4076bc.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/7217.d970c074.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/7217.d970c074.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/7323.2808d029.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/7323.2808d029.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/7323.2808d029.chunk.js.LICENSE.txt` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/7323.2808d029.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/7602.6175e969.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/7602.6175e969.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/7805.51638fbc.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/7805.51638fbc.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/8005.43974a35.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/8005.43974a35.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/8427.d30dffe1.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/8427.d30dffe1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/8477.e948c092.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/8477.e948c092.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/8492.f56c9d4c.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/8492.f56c9d4c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/8570.6de19120.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/8570.6de19120.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/8691.9ccf7f89.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/8691.9ccf7f89.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/9330.d29313d4.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/9330.2b4c99e0.chunk.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,66 +1,74 @@
 "use strict";
 (self.webpackChunk_streamlit_app = self.webpackChunk_streamlit_app || []).push([
     [9330], {
         69330: (e, t, r) => {
             r.r(t), r.d(t, {
-                default: () => u
+                default: () => a
             });
             var n = r(66845),
-                s = r(40864);
+                u = r(40864);
 
-            function u(e) {
+            function a(e) {
                 let {
                     element: t,
                     width: r,
-                    endpoints: u
+                    endpoints: a,
+                    elementMgr: s
                 } = e;
-                const a = (0, n.useRef)(null),
+                const i = (0, n.useRef)(null),
                     {
                         startTime: d,
-                        endTime: i,
-                        loop: c
-                    } = t;
+                        endTime: c,
+                        loop: l,
+                        autoplay: o
+                    } = t,
+                    m = (0, n.useMemo)((() => {
+                        if (!t.id) return !0;
+                        const e = s.getElementState(t.id, "preventAutoplay");
+                        return e || s.setElementState(t.id, "preventAutoplay", !0), null !== e && void 0 !== e && e
+                    }), [t.id, s]);
                 (0, n.useEffect)((() => {
-                    a.current && (a.current.currentTime = d)
+                    i.current && (i.current.currentTime = d)
                 }), [d]), (0, n.useEffect)((() => {
-                    const e = a.current,
+                    const e = i.current,
                         r = () => {
                             e && (e.currentTime = t.startTime)
                         };
                     return e && e.addEventListener("loadedmetadata", r), () => {
                         e && e.removeEventListener("loadedmetadata", r)
                     }
                 }), [t]), (0, n.useEffect)((() => {
-                    const e = a.current;
+                    const e = i.current;
                     if (!e) return;
                     let t = !1;
                     const r = () => {
-                        i > 0 && e.currentTime >= i && (c ? (e.currentTime = d || 0, e.play()) : t || (t = !0, e.pause()))
+                        c > 0 && e.currentTime >= c && (l ? (e.currentTime = d || 0, e.play()) : t || (t = !0, e.pause()))
                     };
-                    return i > 0 && e.addEventListener("timeupdate", r), () => {
-                        e && i > 0 && e.removeEventListener("timeupdate", r)
+                    return c > 0 && e.addEventListener("timeupdate", r), () => {
+                        e && c > 0 && e.removeEventListener("timeupdate", r)
                     }
-                }), [i, c, d]), (0, n.useEffect)((() => {
-                    const e = a.current;
+                }), [c, l, d]), (0, n.useEffect)((() => {
+                    const e = i.current;
                     if (!e) return;
                     const t = () => {
-                        c && (e.currentTime = d || 0, e.play())
+                        l && (e.currentTime = d || 0, e.play())
                     };
                     return e.addEventListener("ended", t), () => {
                         e && e.removeEventListener("ended", t)
                     }
-                }), [c, d]);
-                const o = u.buildMediaURL(t.url);
-                return (0, s.jsx)("audio", {
+                }), [l, d]);
+                const p = a.buildMediaURL(t.url);
+                return (0, u.jsx)("audio", {
                     "data-testid": "stAudio",
                     id: "audio",
-                    ref: a,
+                    ref: i,
                     controls: !0,
-                    src: o,
+                    autoPlay: o && !m,
+                    src: p,
                     className: "stAudio",
                     style: {
                         width: r
                     }
                 })
             }
         }
```

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/9336.2d95d840.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/9336.2d95d840.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/937.a1248039.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/937.a1248039.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/9656.8c935274.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/9656.8c935274.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/9758.6e6d8662.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/9758.6e6d8662.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/9865.fd93213d.chunk.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/9865.fd93213d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/main.8fc4565f.js` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/main.d3201242.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.8fc4565f.js.LICENSE.txt */
+/*! For license information please see main.d3201242.js.LICENSE.txt */
 (() => {
     var __webpack_modules__ = {
             68785: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     B: () => i,
                     Id: () => r,
@@ -36667,18 +36667,18 @@
                             return void 0 === e && (e = "type.googleapis.com"), e + "/ArrowVegaLiteChart"
                         }, e
                     })(), s.Audio = (() => {
                         function e(e) {
                             if (e)
                                 for (let t = Object.keys(e), n = 0; n < t.length; ++n) null != e[t[n]] && (this[t[n]] = e[t[n]])
                         }
-                        return e.prototype.url = "", e.prototype.startTime = 0, e.prototype.endTime = 0, e.prototype.loop = !1, e.create = function(t) {
+                        return e.prototype.url = "", e.prototype.startTime = 0, e.prototype.endTime = 0, e.prototype.loop = !1, e.prototype.autoplay = !1, e.prototype.id = "", e.create = function(t) {
                             return new e(t)
                         }, e.encode = function(e, t) {
-                            return t || (t = i.create()), null != e.startTime && Object.hasOwnProperty.call(e, "startTime") && t.uint32(24).int32(e.startTime), null != e.url && Object.hasOwnProperty.call(e, "url") && t.uint32(42).string(e.url), null != e.endTime && Object.hasOwnProperty.call(e, "endTime") && t.uint32(48).int32(e.endTime), null != e.loop && Object.hasOwnProperty.call(e, "loop") && t.uint32(56).bool(e.loop), t
+                            return t || (t = i.create()), null != e.startTime && Object.hasOwnProperty.call(e, "startTime") && t.uint32(24).int32(e.startTime), null != e.url && Object.hasOwnProperty.call(e, "url") && t.uint32(42).string(e.url), null != e.endTime && Object.hasOwnProperty.call(e, "endTime") && t.uint32(48).int32(e.endTime), null != e.loop && Object.hasOwnProperty.call(e, "loop") && t.uint32(56).bool(e.loop), null != e.autoplay && Object.hasOwnProperty.call(e, "autoplay") && t.uint32(64).bool(e.autoplay), null != e.id && Object.hasOwnProperty.call(e, "id") && t.uint32(74).string(e.id), t
                         }, e.encodeDelimited = function(e, t) {
                             return this.encode(e, t).ldelim()
                         }, e.decode = function(e, t) {
                             e instanceof o || (e = o.create(e));
                             let n = void 0 === t ? e.len : e.pos + t,
                                 r = new s.Audio;
                             for (; e.pos < n;) {
@@ -36692,31 +36692,37 @@
                                         break;
                                     case 6:
                                         r.endTime = e.int32();
                                         break;
                                     case 7:
                                         r.loop = e.bool();
                                         break;
+                                    case 8:
+                                        r.autoplay = e.bool();
+                                        break;
+                                    case 9:
+                                        r.id = e.string();
+                                        break;
                                     default:
                                         e.skipType(7 & t)
                                 }
                             }
                             return r
                         }, e.decodeDelimited = function(e) {
                             return e instanceof o || (e = new o(e)), this.decode(e, e.uint32())
                         }, e.verify = function(e) {
-                            return "object" !== typeof e || null === e ? "object expected" : null != e.url && e.hasOwnProperty("url") && !a.isString(e.url) ? "url: string expected" : null != e.startTime && e.hasOwnProperty("startTime") && !a.isInteger(e.startTime) ? "startTime: integer expected" : null != e.endTime && e.hasOwnProperty("endTime") && !a.isInteger(e.endTime) ? "endTime: integer expected" : null != e.loop && e.hasOwnProperty("loop") && "boolean" !== typeof e.loop ? "loop: boolean expected" : null
+                            return "object" !== typeof e || null === e ? "object expected" : null != e.url && e.hasOwnProperty("url") && !a.isString(e.url) ? "url: string expected" : null != e.startTime && e.hasOwnProperty("startTime") && !a.isInteger(e.startTime) ? "startTime: integer expected" : null != e.endTime && e.hasOwnProperty("endTime") && !a.isInteger(e.endTime) ? "endTime: integer expected" : null != e.loop && e.hasOwnProperty("loop") && "boolean" !== typeof e.loop ? "loop: boolean expected" : null != e.autoplay && e.hasOwnProperty("autoplay") && "boolean" !== typeof e.autoplay ? "autoplay: boolean expected" : null != e.id && e.hasOwnProperty("id") && !a.isString(e.id) ? "id: string expected" : null
                         }, e.fromObject = function(e) {
                             if (e instanceof s.Audio) return e;
                             let t = new s.Audio;
-                            return null != e.url && (t.url = String(e.url)), null != e.startTime && (t.startTime = 0 | e.startTime), null != e.endTime && (t.endTime = 0 | e.endTime), null != e.loop && (t.loop = Boolean(e.loop)), t
+                            return null != e.url && (t.url = String(e.url)), null != e.startTime && (t.startTime = 0 | e.startTime), null != e.endTime && (t.endTime = 0 | e.endTime), null != e.loop && (t.loop = Boolean(e.loop)), null != e.autoplay && (t.autoplay = Boolean(e.autoplay)), null != e.id && (t.id = String(e.id)), t
                         }, e.toObject = function(e, t) {
                             t || (t = {});
                             let n = {};
-                            return t.defaults && (n.startTime = 0, n.url = "", n.endTime = 0, n.loop = !1), null != e.startTime && e.hasOwnProperty("startTime") && (n.startTime = e.startTime), null != e.url && e.hasOwnProperty("url") && (n.url = e.url), null != e.endTime && e.hasOwnProperty("endTime") && (n.endTime = e.endTime), null != e.loop && e.hasOwnProperty("loop") && (n.loop = e.loop), n
+                            return t.defaults && (n.startTime = 0, n.url = "", n.endTime = 0, n.loop = !1, n.autoplay = !1, n.id = ""), null != e.startTime && e.hasOwnProperty("startTime") && (n.startTime = e.startTime), null != e.url && e.hasOwnProperty("url") && (n.url = e.url), null != e.endTime && e.hasOwnProperty("endTime") && (n.endTime = e.endTime), null != e.loop && e.hasOwnProperty("loop") && (n.loop = e.loop), null != e.autoplay && e.hasOwnProperty("autoplay") && (n.autoplay = e.autoplay), null != e.id && e.hasOwnProperty("id") && (n.id = e.id), n
                         }, e.prototype.toJSON = function() {
                             return this.constructor.toObject(this, r.util.toJSONOptions)
                         }, e.getTypeUrl = function(e) {
                             return void 0 === e && (e = "type.googleapis.com"), e + "/Audio"
                         }, e
                     })(), s.AutoRerun = (() => {
                         function e(e) {
@@ -46497,20 +46503,20 @@
                             return void 0 === e && (e = "type.googleapis.com"), e + "/SubtitleTrack"
                         }, e
                     })(), s.Video = (() => {
                         function e(e) {
                             if (this.subtitles = [], e)
                                 for (let t = Object.keys(e), n = 0; n < t.length; ++n) null != e[t[n]] && (this[t[n]] = e[t[n]])
                         }
-                        return e.prototype.url = "", e.prototype.startTime = 0, e.prototype.type = 0, e.prototype.subtitles = a.emptyArray, e.prototype.endTime = 0, e.prototype.loop = !1, e.create = function(t) {
+                        return e.prototype.url = "", e.prototype.startTime = 0, e.prototype.type = 0, e.prototype.subtitles = a.emptyArray, e.prototype.endTime = 0, e.prototype.loop = !1, e.prototype.autoplay = !1, e.prototype.muted = !1, e.prototype.id = "", e.create = function(t) {
                             return new e(t)
                         }, e.encode = function(e, t) {
                             if (t || (t = i.create()), null != e.startTime && Object.hasOwnProperty.call(e, "startTime") && t.uint32(24).int32(e.startTime), null != e.type && Object.hasOwnProperty.call(e, "type") && t.uint32(40).int32(e.type), null != e.url && Object.hasOwnProperty.call(e, "url") && t.uint32(50).string(e.url), null != e.subtitles && e.subtitles.length)
                                 for (let n = 0; n < e.subtitles.length; ++n) s.SubtitleTrack.encode(e.subtitles[n], t.uint32(58).fork()).ldelim();
-                            return null != e.endTime && Object.hasOwnProperty.call(e, "endTime") && t.uint32(64).int32(e.endTime), null != e.loop && Object.hasOwnProperty.call(e, "loop") && t.uint32(72).bool(e.loop), t
+                            return null != e.endTime && Object.hasOwnProperty.call(e, "endTime") && t.uint32(64).int32(e.endTime), null != e.loop && Object.hasOwnProperty.call(e, "loop") && t.uint32(72).bool(e.loop), null != e.autoplay && Object.hasOwnProperty.call(e, "autoplay") && t.uint32(80).bool(e.autoplay), null != e.muted && Object.hasOwnProperty.call(e, "muted") && t.uint32(88).bool(e.muted), null != e.id && Object.hasOwnProperty.call(e, "id") && t.uint32(98).string(e.id), t
                         }, e.encodeDelimited = function(e, t) {
                             return this.encode(e, t).ldelim()
                         }, e.decode = function(e, t) {
                             e instanceof o || (e = o.create(e));
                             let n = void 0 === t ? e.len : e.pos + t,
                                 r = new s.Video;
                             for (; e.pos < n;) {
@@ -46530,14 +46536,23 @@
                                         break;
                                     case 8:
                                         r.endTime = e.int32();
                                         break;
                                     case 9:
                                         r.loop = e.bool();
                                         break;
+                                    case 10:
+                                        r.autoplay = e.bool();
+                                        break;
+                                    case 11:
+                                        r.muted = e.bool();
+                                        break;
+                                    case 12:
+                                        r.id = e.string();
+                                        break;
                                     default:
                                         e.skipType(7 & t)
                                 }
                             }
                             return r
                         }, e.decodeDelimited = function(e) {
                             return e instanceof o || (e = new o(e)), this.decode(e, e.uint32())
@@ -46555,15 +46570,15 @@
                             if (null != e.subtitles && e.hasOwnProperty("subtitles")) {
                                 if (!Array.isArray(e.subtitles)) return "subtitles: array expected";
                                 for (let t = 0; t < e.subtitles.length; ++t) {
                                     let n = s.SubtitleTrack.verify(e.subtitles[t]);
                                     if (n) return "subtitles." + n
                                 }
                             }
-                            return null != e.endTime && e.hasOwnProperty("endTime") && !a.isInteger(e.endTime) ? "endTime: integer expected" : null != e.loop && e.hasOwnProperty("loop") && "boolean" !== typeof e.loop ? "loop: boolean expected" : null
+                            return null != e.endTime && e.hasOwnProperty("endTime") && !a.isInteger(e.endTime) ? "endTime: integer expected" : null != e.loop && e.hasOwnProperty("loop") && "boolean" !== typeof e.loop ? "loop: boolean expected" : null != e.autoplay && e.hasOwnProperty("autoplay") && "boolean" !== typeof e.autoplay ? "autoplay: boolean expected" : null != e.muted && e.hasOwnProperty("muted") && "boolean" !== typeof e.muted ? "muted: boolean expected" : null != e.id && e.hasOwnProperty("id") && !a.isString(e.id) ? "id: string expected" : null
                         }, e.fromObject = function(e) {
                             if (e instanceof s.Video) return e;
                             let t = new s.Video;
                             switch (null != e.url && (t.url = String(e.url)), null != e.startTime && (t.startTime = 0 | e.startTime), e.type) {
                                 default:
                                     if ("number" === typeof e.type) {
                                         t.type = e.type;
@@ -46586,23 +46601,23 @@
                                 if (!Array.isArray(e.subtitles)) throw TypeError(".Video.subtitles: array expected");
                                 t.subtitles = [];
                                 for (let n = 0; n < e.subtitles.length; ++n) {
                                     if ("object" !== typeof e.subtitles[n]) throw TypeError(".Video.subtitles: object expected");
                                     t.subtitles[n] = s.SubtitleTrack.fromObject(e.subtitles[n])
                                 }
                             }
-                            return null != e.endTime && (t.endTime = 0 | e.endTime), null != e.loop && (t.loop = Boolean(e.loop)), t
+                            return null != e.endTime && (t.endTime = 0 | e.endTime), null != e.loop && (t.loop = Boolean(e.loop)), null != e.autoplay && (t.autoplay = Boolean(e.autoplay)), null != e.muted && (t.muted = Boolean(e.muted)), null != e.id && (t.id = String(e.id)), t
                         }, e.toObject = function(e, t) {
                             t || (t = {});
                             let n = {};
-                            if ((t.arrays || t.defaults) && (n.subtitles = []), t.defaults && (n.startTime = 0, n.type = t.enums === String ? "UNUSED" : 0, n.url = "", n.endTime = 0, n.loop = !1), null != e.startTime && e.hasOwnProperty("startTime") && (n.startTime = e.startTime), null != e.type && e.hasOwnProperty("type") && (n.type = t.enums === String ? void 0 === s.Video.Type[e.type] ? e.type : s.Video.Type[e.type] : e.type), null != e.url && e.hasOwnProperty("url") && (n.url = e.url), e.subtitles && e.subtitles.length) {
+                            if ((t.arrays || t.defaults) && (n.subtitles = []), t.defaults && (n.startTime = 0, n.type = t.enums === String ? "UNUSED" : 0, n.url = "", n.endTime = 0, n.loop = !1, n.autoplay = !1, n.muted = !1, n.id = ""), null != e.startTime && e.hasOwnProperty("startTime") && (n.startTime = e.startTime), null != e.type && e.hasOwnProperty("type") && (n.type = t.enums === String ? void 0 === s.Video.Type[e.type] ? e.type : s.Video.Type[e.type] : e.type), null != e.url && e.hasOwnProperty("url") && (n.url = e.url), e.subtitles && e.subtitles.length) {
                                 n.subtitles = [];
                                 for (let r = 0; r < e.subtitles.length; ++r) n.subtitles[r] = s.SubtitleTrack.toObject(e.subtitles[r], t)
                             }
-                            return null != e.endTime && e.hasOwnProperty("endTime") && (n.endTime = e.endTime), null != e.loop && e.hasOwnProperty("loop") && (n.loop = e.loop), n
+                            return null != e.endTime && e.hasOwnProperty("endTime") && (n.endTime = e.endTime), null != e.loop && e.hasOwnProperty("loop") && (n.loop = e.loop), null != e.autoplay && e.hasOwnProperty("autoplay") && (n.autoplay = e.autoplay), null != e.muted && e.hasOwnProperty("muted") && (n.muted = e.muted), null != e.id && e.hasOwnProperty("id") && (n.id = e.id), n
                         }, e.prototype.toJSON = function() {
                             return this.constructor.toObject(this, r.util.toJSONOptions)
                         }, e.getTypeUrl = function(e) {
                             return void 0 === e && (e = "type.googleapis.com"), e + "/Video"
                         }, e.Type = function() {
                             const e = {},
                                 t = Object.create(e);
@@ -115559,15 +115574,15 @@
     })(), __webpack_require__.d = (e, t) => {
         for (var n in t) __webpack_require__.o(t, n) && !__webpack_require__.o(e, n) && Object.defineProperty(e, n, {
             enumerable: !0,
             get: t[n]
         })
     }, __webpack_require__.f = {}, __webpack_require__.e = e => Promise.all(Object.keys(__webpack_require__.f).reduce(((t, n) => (__webpack_require__.f[n](e, t), t)), [])), __webpack_require__.u = e => "static/js/" + e + "." + {
         43: "b0aa5759",
-        178: "b5384fd0",
+        178: "7bea8c5d",
         474: "87506447",
         656: "ae85f8f1",
         937: "a1248039",
         1074: "73973756",
         1168: "1d6408e6",
         1307: "8ea033f1",
         1451: "3b0a3e31",
@@ -115611,15 +115626,15 @@
         7805: "51638fbc",
         8005: "43974a35",
         8427: "d30dffe1",
         8477: "e948c092",
         8492: "f56c9d4c",
         8570: "6de19120",
         8691: "9ccf7f89",
-        9330: "d29313d4",
+        9330: "2b4c99e0",
         9336: "2d95d840",
         9656: "8c935274",
         9758: "6e6d8662",
         9865: "fd93213d"
     } [e] + ".chunk.js", __webpack_require__.miniCssF = e => "static/css/" + e + "." + {
         43: "e3b876c5",
         2411: "8b8f33d6",
@@ -120722,15 +120737,16 @@
                             element: t.vegaLiteChartElement,
                             ...n
                         });
                     case "audio":
                         return (0, ze.jsx)(Ii, {
                             element: t.element.audio,
                             endpoints: e.endpoints,
-                            ...n
+                            ...n,
+                            elementMgr: e.widgetMgr
                         });
                     case "balloons":
                         return Oa(e.isStale, (0, ze.jsx)(Pi, {
                             scriptRunId: e.scriptRunId
                         }));
                     case "bokehChart":
                         return (0, ze.jsx)(Ui, {
@@ -120843,15 +120859,16 @@
                             element: t.element.text,
                             ...n
                         });
                     case "video":
                         return (0, ze.jsx)(Zi, {
                             element: t.element.video,
                             endpoints: e.endpoints,
-                            ...n
+                            ...n,
+                            elementMgr: e.widgetMgr
                         });
                     case "toast": {
                         const e = t.element.toast;
                         return (0, ze.jsx)(Fi, {
                             body: e.body,
                             icon: e.icon,
                             ...n
```

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/js/main.8fc4565f.js.LICENSE.txt` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/js/main.d3201242.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg` & `streamlit_nightly-1.33.1.dev20240423/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/string_util.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/string_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/temporary_directory.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/temporary_directory.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/testing/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/testing/v1/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/testing/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/testing/v1/app_test.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/testing/v1/app_test.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/testing/v1/element_tree.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/testing/v1/element_tree.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/testing/v1/local_script_runner.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/testing/v1/local_script_runner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/testing/v1/util.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/testing/v1/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/time_util.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/time_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/type_util.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/type_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/url_util.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/url_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/user_info.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/user_info.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/util.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/vendor/ipython/modified_sys_path.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/vendor/ipython/modified_sys_path.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/vendor/pympler/asizeof.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/vendor/pympler/asizeof.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/version.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/version.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/watcher/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/watcher/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/watcher/event_based_path_watcher.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/watcher/event_based_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/watcher/local_sources_watcher.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/watcher/local_sources_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/watcher/path_watcher.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/watcher/path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/watcher/polling_path_watcher.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/watcher/polling_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/watcher/util.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/watcher/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/web/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/web/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/web/bootstrap.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/web/bootstrap.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/web/cache_storage_manager_config.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/web/cache_storage_manager_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/web/cli.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/web/cli.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/web/server/__init__.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/web/server/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/web/server/app_static_file_handler.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/web/server/app_static_file_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/web/server/browser_websocket_handler.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/web/server/browser_websocket_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/web/server/component_request_handler.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/web/server/component_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/web/server/media_file_handler.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/web/server/media_file_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/web/server/routes.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/web/server/routes.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/web/server/server.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/web/server/server.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/web/server/server_util.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/web/server/server_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/web/server/stats_request_handler.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/web/server/stats_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/web/server/upload_file_request_handler.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/web/server/upload_file_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit/web/server/websocket_headers.py` & `streamlit_nightly-1.33.1.dev20240423/streamlit/web/server/websocket_headers.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit_nightly.egg-info/PKG-INFO` & `streamlit_nightly-1.33.1.dev20240423/streamlit_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nightly
-Version: 1.33.1.dev20240422
+Version: 1.33.1.dev20240423
 Summary: A faster way to build and share data apps
 Home-page: https://streamlit.io
 Author: Snowflake Inc
 Author-email: hello@streamlit.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/streamlit/streamlit
 Project-URL: Bug Tracker, https://github.com/streamlit/streamlit/issues
```

### Comparing `streamlit_nightly-1.33.1.dev20240422/streamlit_nightly.egg-info/SOURCES.txt` & `streamlit_nightly-1.33.1.dev20240423/streamlit_nightly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -338,15 +338,15 @@
 streamlit/static/static/css/43.e3b876c5.chunk.css
 streamlit/static/static/css/main.bf304093.css
 streamlit/static/static/js/1074.73973756.chunk.js
 streamlit/static/static/js/1168.1d6408e6.chunk.js
 streamlit/static/static/js/1307.8ea033f1.chunk.js
 streamlit/static/static/js/1451.3b0a3e31.chunk.js
 streamlit/static/static/js/1479.6709db03.chunk.js
-streamlit/static/static/js/178.b5384fd0.chunk.js
+streamlit/static/static/js/178.7bea8c5d.chunk.js
 streamlit/static/static/js/1792.b8efa879.chunk.js
 streamlit/static/static/js/2187.9469f035.chunk.js
 streamlit/static/static/js/2411.a8823789.chunk.js
 streamlit/static/static/js/2411.a8823789.chunk.js.LICENSE.txt
 streamlit/static/static/js/2469.3e9c3ce9.chunk.js
 streamlit/static/static/js/2634.1249dc7a.chunk.js
 streamlit/static/static/js/2736.914069e5.chunk.js
@@ -391,23 +391,23 @@
 streamlit/static/static/js/7805.51638fbc.chunk.js
 streamlit/static/static/js/8005.43974a35.chunk.js
 streamlit/static/static/js/8427.d30dffe1.chunk.js
 streamlit/static/static/js/8477.e948c092.chunk.js
 streamlit/static/static/js/8492.f56c9d4c.chunk.js
 streamlit/static/static/js/8570.6de19120.chunk.js
 streamlit/static/static/js/8691.9ccf7f89.chunk.js
-streamlit/static/static/js/9330.d29313d4.chunk.js
+streamlit/static/static/js/9330.2b4c99e0.chunk.js
 streamlit/static/static/js/9336.2d95d840.chunk.js
 streamlit/static/static/js/937.a1248039.chunk.js
 streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
 streamlit/static/static/js/9656.8c935274.chunk.js
 streamlit/static/static/js/9758.6e6d8662.chunk.js
 streamlit/static/static/js/9865.fd93213d.chunk.js
-streamlit/static/static/js/main.8fc4565f.js
-streamlit/static/static/js/main.8fc4565f.js.LICENSE.txt
+streamlit/static/static/js/main.d3201242.js
+streamlit/static/static/js/main.d3201242.js.LICENSE.txt
 streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
 streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
 streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
 streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
```

### Comparing `streamlit_nightly-1.33.1.dev20240422/tests/testutil.py` & `streamlit_nightly-1.33.1.dev20240423/tests/testutil.py`

 * *Files identical despite different names*


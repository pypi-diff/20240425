# Comparing `tmp/solara_ui-1.31.0.tar.gz` & `tmp/solara_ui-1.32.0.tar.gz`

## Comparing `solara_ui-1.31.0.tar` & `solara_ui-1.32.0.tar`

### file list

```diff
@@ -1,564 +1,578 @@
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 solara_ui-1.31.0/prefix/etc/jupyter/jupyter_notebook_config.d/solara.json
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 solara_ui-1.31.0/prefix/etc/jupyter/jupyter_server_config.d/solara.json
--rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/__init__.py
--rw-r--r--   0        0        0    23656 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/__main__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/alias.py
--rw-r--r--   0        0        0    22677 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/autorouting.py
--rw-r--r--   0        0        0    10500 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/cache.py
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/checks.html
--rw-r--r--   0        0        0     7563 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/checks.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/comm.py
--rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/datatypes.py
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/express.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/kitchensink.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/layout.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/lifecycle.py
--rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/minisettings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/py.typed
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/reactive.py
--rw-r--r--   0        0        0     9143 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/routing.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/settings.py
--rw-r--r--   0        0        0    29563 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/tasks.py
--rw-r--r--   0        0        0    23385 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/toestand.py
--rw-r--r--   0        0        0     8934 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/util.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/__init__.py
--rw-r--r--   0        0        0     5144 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/alert.py
--rw-r--r--   0        0        0    16355 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/applayout.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/button.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/card.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/checkbox.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/code_highlight_css.py
--rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/code_highlight_css.vue
--rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/columns.py
--rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/component_vue.py
--rw-r--r--   0        0        0    13663 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/cross_filter.py
--rw-r--r--   0        0        0    21033 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/dataframe.py
--rw-r--r--   0        0        0     8021 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/datatable.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/datatable.vue
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/details.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/download.vue
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/echarts.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/echarts.vue
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/figure_altair.py
--rw-r--r--   0        0        0     7410 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/file_browser.py
--rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/file_download.py
--rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/file_drop.py
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/file_drop.vue
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/file_list_widget.vue
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/head.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/head_tag.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/head_tag.vue
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/image.py
--rw-r--r--   0        0        0    14585 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/input.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/link.py
--rw-r--r--   0        0        0    12502 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/markdown.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/markdown_editor.py
--rw-r--r--   0        0        0     8864 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/markdown_editor.vue
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/matplotlib.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/meta.py
--rw-r--r--   0        0        0    12473 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/misc.py
--rw-r--r--   0        0        0     9938 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/pivot_table.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/pivot_table.vue
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/progress.py
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/select.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/select.vue
--rw-r--r--   0        0        0    13408 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/slider.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/slider_date.vue
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/spinner-solara.vue
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/spinner.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/sql_code.py
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/sql_code.vue
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/style.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/switch.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/tab_navigation.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/title.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/title.vue
--rw-r--r--   0        0        0     7717 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/togglebuttons.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/components/tooltip.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/hooks/__init__.py
--rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/hooks/dataframe.py
--rw-r--r--   0        0        0     7885 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/hooks/misc.py
--rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/hooks/use_reactive.py
--rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/hooks/use_thread.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/lab/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/lab/toestand.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/lab/components/__init__.py
--rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/lab/components/chat.py
--rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/lab/components/confirmation_dialog.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/lab/components/cross_filter.py
--rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/lab/components/input_date.py
--rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/lab/components/menu.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/lab/components/menu.vue
--rw-r--r--   0        0        0     9699 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/lab/components/tabs.py
--rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/lab/components/theming.py
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/lab/components/theming.vue
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/lab/hooks/__init__.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/lab/hooks/dataframe.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/lab/utils/__init__.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/lab/utils/cookies.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/lab/utils/dataframe.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/lab/utils/headers.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/scope/__init__.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/scope/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/__init__.py
--rw-r--r--   0        0        0    20336 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/app.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/cdn_helper.py
--rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/esm.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/fastapi.py
--rw-r--r--   0        0        0     9168 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/flask.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/jupytertools.py
--rw-r--r--   0        0        0    11092 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/kernel.py
--rw-r--r--   0        0        0    13816 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/kernel_context.py
--rw-r--r--   0        0        0    18788 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/patch.py
--rw-r--r--   0        0        0     9531 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/reload.py
--rw-r--r--   0        0        0    15585 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/server.py
--rw-r--r--   0        0        0     6394 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/settings.py
--rw-r--r--   0        0        0     8677 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/shell.py
--rw-r--r--   0        0        0    23715 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/starlette.py
--rw-r--r--   0        0        0     6038 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/telemetry.py
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/threaded.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/utils.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/websocket.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/assets/custom.css
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/assets/custom.js
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/assets/favicon.png
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/assets/favicon.svg
--rw-r--r--   0        0        0    40341 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/assets/style.css
--rw-r--r--   0        0        0    16733 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/assets/theme-dark.css
--rw-r--r--   0        0        0    15637 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/assets/theme-light.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/assets/theme.js
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/jupyter/__init__.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/jupyter/cdn_handler.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/jupyter/server_extension.py
--rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/static/ansi.js
--rw-r--r--   0        0        0     6809 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/static/highlight-dark.css
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/static/highlight.css
--rw-r--r--   0        0        0     8874 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/static/main-vuetify.js
--rw-r--r--   0        0        0     5679 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/static/main.js
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/static/solara_bootstrap.py
--rw-r--r--   0        0        0     6855 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/static/sun.svg
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/static/webworker.js
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/templates/index.html.j2
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/templates/loader-plain.css
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/templates/loader-plain.html
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/templates/loader-solara.css
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/templates/loader-solara.html
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/templates/plain.html
--rw-r--r--   0        0        0    19668 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/server/templates/solara.html.j2
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/template/button.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/template/markdown.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/template/portal/.flake8
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/template/portal/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/template/portal/LICENSE
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/template/portal/Procfile
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/template/portal/mypy.ini
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/template/portal/pyproject.toml
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/template/portal/solara_portal/__init__.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/template/portal/solara_portal/data.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/template/portal/solara_portal/components/__init__.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/template/portal/solara_portal/components/article.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/template/portal/solara_portal/components/data.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/template/portal/solara_portal/components/header.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/template/portal/solara_portal/components/layout.py
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/template/portal/solara_portal/content/articles/equis-in-vidi.md
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/template/portal/solara_portal/content/articles/substiterat-vati.md
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/template/portal/solara_portal/pages/__init__.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/template/portal/solara_portal/pages/tabular.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/template/portal/solara_portal/pages/article/__init__.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/template/portal/solara_portal/pages/viz/__init__.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/template/portal/solara_portal/pages/viz/overview.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/test/__init__.py
--rw-r--r--   0        0        0    26284 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/test/pytest_plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/__init__.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/utils.py
--rw-r--r--   0        0        0     9665 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/assets/custom.css
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/assets/theme.js
--rw-r--r--   0        0        0    86383 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/assets/images/logo-small.png
--rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/assets/images/logo.svg
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/assets/images/logo_white.svg
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/components/__init__.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/components/algolia.vue
--rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/components/algolia_api.vue
--rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/components/docs.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/components/header.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/components/hero.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/components/mailchimp.py
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/components/mailchimp.vue
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/components/markdown.py
--rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/components/notebook.py
--rw-r--r--   0        0        0    34120 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/__init__.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/doc_use_download.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/docutils.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/apps/__init__.py
--rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/apps/jupyter-dashboard-1.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/apps/layout-demo.py
--rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/apps/scatter.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/apps/scrolling.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/apps/tutorial-streamlit.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/apps/authorization/__init__.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/apps/authorization/admin.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/apps/authorization/users.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/apps/multipage/__init__.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/apps/multipage/page1.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/apps/multipage/page2.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/changelog/__init__.py
--rw-r--r--   0        0        0    11875 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/changelog/changelog.md
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/contact/__init__.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/contact/contact.md
--rw-r--r--   0        0        0    11379 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/__init__.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/__init__.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/00-overview.md
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/10-howto/00-overview.md
--rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/10-howto/10-multipage.md
--rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/10-howto/20-layout.md
--rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/10-howto/30-testing.md
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/10-howto/31-debugging.md
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/10-howto/40-embed.md
--rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/10-howto/50-ipywidget_libraries.md
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/15-reference/00-overview.md
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/15-reference/40-static_files.md
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/15-reference/41-asset-files.md
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/15-reference/60-static-site-generation.md
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/15-reference/70-search.md
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/15-reference/80-reloading.md
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/15-reference/90-notebook-support.md
--rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/15-reference/95-caching.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/20-understanding/00-introduction.md
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/20-understanding/05-ipywidgets.md
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/20-understanding/06-ipyvuetify.md
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/20-understanding/10-reacton.md
--rw-r--r--   0        0        0     5328 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/20-understanding/12-reacton-basics.md
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/20-understanding/15-anatomy.md
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/20-understanding/17-rules-of-hooks.md
--rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/20-understanding/18-containers.md
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/20-understanding/20-solara.md
--rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/20-understanding/40-routing.md
--rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/20-understanding/50-solara-server.md
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/20-understanding/60-voila.md
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/30-enterprise/00-overview.md
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/30-enterprise/10-oauth.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/40-development/00-overview.md
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/40-development/01-contribute.md
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/40-development/10-setup.md
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/cross_filter/__init__.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/cross_filter/cross_filter_dataframe.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/cross_filter/cross_filter_report.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/cross_filter/cross_filter_select.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/cross_filter/cross_filter_slider.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/hooks/__init__.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/hooks/use_cross_filter.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/hooks/use_dark_effective.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/hooks/use_effect.md
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/hooks/use_effect.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/hooks/use_exception.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/hooks/use_memo.md
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/hooks/use_memo.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/hooks/use_previous.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/hooks/use_reactive.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/hooks/use_state.py
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/hooks/use_state_or_update.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/hooks/use_thread.md
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/hooks/use_thread.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/hooks/use_trait_observe.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/routing/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/routing/generate_routes.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/routing/generate_routes_directory.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/routing/resolve_path.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/routing/route.py
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/routing/use_route.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/routing/use_router.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/utilities/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/utilities/component_vue.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/utilities/computed.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/utilities/display.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/utilities/get_kernel_id.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/utilities/get_session_id.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/utilities/memoize.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/utilities/on_kernel_start.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/utilities/reactive.py
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/api/utilities/widget.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/__init__.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/common.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/advanced/__init__.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/advanced/link.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/advanced/meta.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/advanced/style.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/data/__init__.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/data/dataframe.py
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/data/pivot_table.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/enterprise/__init__.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/enterprise/avatar.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/enterprise/avatar_menu.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/input/__init__.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/input/button.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/input/checkbox.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/input/file_browser.py
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/input/file_drop.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/input/input.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/input/select.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/input/slider.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/input/switch.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/input/togglebuttons.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/lab/__init__.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/lab/chat.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/lab/confirmation_dialog.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/lab/cookies_headers.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/lab/input_date.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/lab/menu.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/lab/tab.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/lab/tabs.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/lab/task.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/lab/theming.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/lab/use_task.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/layout/__init__.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/layout/app_bar.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/layout/app_bar_title.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/layout/app_layout.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/layout/card.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/layout/card_actions.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/layout/column.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/layout/columns.py
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/layout/columns_responsive.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/layout/griddraggable.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/layout/gridfixed.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/layout/hbox.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/layout/row.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/layout/sidebar.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/layout/vbox.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/output/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/output/file_download.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/output/html.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/output/image.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/output/markdown.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/output/markdown_editor.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/output/sql_code.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/output/tooltip.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/page/__init__.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/page/head.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/page/title.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/status/__init__.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/status/error.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/status/info.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/status/progress.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/status/spinner.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/status/success.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/status/warning.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/viz/__init__.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/viz/altair.py
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/viz/echarts.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/viz/matplotlib.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/viz/plotly.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/components/viz/plotly_express.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/__init__.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/ipycanvas.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/ai/__init__.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/ai/chatbot.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/ai/tokenizer.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/basics/__init__.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/basics/sine.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/fullscreen/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/fullscreen/authorization.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/fullscreen/layout_demo.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/fullscreen/multipage.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/fullscreen/scatter.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/fullscreen/scrolling.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/fullscreen/tutorial_streamlit.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/general/__init__.py
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/general/custom_storage.py
--rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/general/deploy_model.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/general/live_update.py
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/general/login_oauth.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/general/mycard.vue
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/general/pokemon_search.py
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/general/vue_component.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/libraries/__init__.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/libraries/altair.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/libraries/bqplot.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/libraries/ipyleaflet.py
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/libraries/ipyleaflet_advanced.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/utilities/__init__.py
--rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/utilities/calculator.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/utilities/countdown_timer.py
--rw-r--r--   0        0        0     6480 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/utilities/todo.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/visualization/__init__.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/visualization/annotator.py
--rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/visualization/linked_views.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/examples/visualization/plotly.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/faq/__init__.py
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/faq/content/99-faq.md
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/getting_started/__init__.py
--rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/00-quickstart.md
--rw-r--r--   0        0        0     6609 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/01-introduction.md
--rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/02-installing.md
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/80-what-is-lab.md
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/90-troubleshoot.md
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/04-tutorials/00-overview.md
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/04-tutorials/10_data_science.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/04-tutorials/20-web-app.md
--rw-r--r--   0        0        0     4577 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/04-tutorials/30-ipywidgets.md
--rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/04-tutorials/40-streamlit.md
--rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/04-tutorials/50-dash.md
--rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/04-tutorials/60-jupyter-dashboard-part1.py
--rw-r--r--   0        0        0   575276 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/04-tutorials/SF_crime_sample.csv.gz
--rw-r--r--   0        0        0    14031 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/04-tutorials/_data_science.ipynb
--rw-r--r--   0        0        0    57417 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/04-tutorials/_jupyter_dashboard_1.ipynb
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/05-fundamentals/00-overview.md
--rw-r--r--   0        0        0    13931 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/05-fundamentals/10-components.md
--rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/05-fundamentals/50-state-management.md
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/07-deploying/00-overview.md
--rw-r--r--   0        0        0     8982 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/07-deploying/10-self-hosted.md
--rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/07-deploying/20-cloud-hosted.md
--rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/showcase/__init__.py
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/showcase/domino_code_assist.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/showcase/planeto_tessa.py
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/showcase/solara_dev.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/showcase/solarathon_2023_team_2.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/showcase/solarathon_2023_team_4.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/showcase/solarathon_2023_team_5.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/showcase/solarathon_2023_team_6.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/pages/showcase/wanderlust.py
--rw-r--r--   0        0        0    37437 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/public/beach.jpeg
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/public/logo.svg
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/public/success.html
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/public/social/discord.svg
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/public/social/github.svg
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/public/social/twitter.svg
--rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/website/templates/index.html.j2
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/widgets/__init__.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/widgets/widgets.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/widgets/vue/gridlayout.vue
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/widgets/vue/html.vue
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/widgets/vue/navigator.vue
--rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 solara_ui-1.31.0/solara/widgets/vue/vegalite.vue
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/__init__.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/__init__.py
--rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/api_test.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/app_widget.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/async_test.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/cdn_test.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/cmdline_test.py
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/create_test.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/error_test.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/esm_test.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/file_download_test.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/flask_test.py
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/input_date_test.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/latex_test.py
--rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/lifecycle_test.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/markdown_test.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/menu_test.py
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/popout_test.py
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/reconnect_test.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/router_test.py
--rw-r--r--   0        0        0     7895 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/server_test.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/ssg_test.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/starlette_test.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/test.vue
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/testapp.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/widget_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/enterprise/__init__.py
--rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/enterprise/oauth_test.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/integration/reload/apps.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/ui/snapshots/tests/integration/latex_test.py/test_widget_latex_solara-flask-chromium-linux-ipywidgets-7-changed-reference.png
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/ui/snapshots/tests/integration/latex_test.py/test_widget_latex_solara-flask-chromium-linux-ipywidgets-7-reference.png
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/ui/snapshots/tests/integration/latex_test.py/test_widget_latex_solara-flask-chromium-linux-ipywidgets-8-changed-reference.png
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/ui/snapshots/tests/integration/latex_test.py/test_widget_latex_solara-flask-chromium-linux-ipywidgets-8-reference.png
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_lab-chromium-linux-ipywidgets-7-reference.png
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_lab-chromium-linux-ipywidgets-8-reference.png
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_notebook-chromium-linux-ipywidgets-7-reference.png
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_notebook-chromium-linux-ipywidgets-8-reference.png
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-solara-chromium-linux-ipywidgets-7-reference.png
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-solara-chromium-linux-ipywidgets-8-reference.png
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-voila-chromium-linux-ipywidgets-7-reference.png
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-voila-chromium-linux-ipywidgets-8-reference.png
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-starlette-solara-chromium-linux-ipywidgets-7-reference.png
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-starlette-solara-chromium-linux-ipywidgets-8-reference.png
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-jupyter_lab-chromium-linux-reference.png
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-jupyter_notebook-chromium-linux-reference.png
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-solara-chromium-linux-reference.png
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-voila-chromium-linux-reference.png
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-starlette-solara-chromium-linux-reference.png
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-flask-chromium-linux-ipyvuetify3-reference.png
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-flask-chromium-linux-reference.png
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-starlette-chromium-linux-ipyvuetify3-reference.png
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-starlette-chromium-linux-reference.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/__init__.py
--rw-r--r--   0        0        0     7898 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/app_test.py
--rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/applayout_test.py
--rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/autorouting_test.py
--rw-r--r--   0        0        0     7817 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/cache_test.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/cdn_helper_test.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/chat_test.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/checkbox_test.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/common.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/component_frontend_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/component_vue_test.vue
--rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/confirmation_dialog_test.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/conftest.py
--rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/cross_filter_component_test.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/cross_filter_test.py
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/dataframe_test.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/datatable_test.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/display_test.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/express_test.py
--rw-r--r--   0        0        0     7110 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/file_browser_test.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/file_download_test.py
--rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/hooks_test.py
--rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/input_date_test.py
--rw-r--r--   0        0        0     8001 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/input_test.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/kernel_test.py
--rw-r--r--   0        0        0     4250 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/lifecycle_test.py
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/matplotlib_test.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/no_solara_test.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/output_widget_test.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/patch_test.py
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/pivottable_test.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/reload_test.py
--rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/router_test.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/select_test.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/settings_test.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/shell_test.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/slider_test.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/switch_test.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/tabs_test.py
--rw-r--r--   0        0        0    17394 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/task_test.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/telemetry_tests.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/toestand_computed_reload.py
--rw-r--r--   0        0        0    37497 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/toestand_test.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/toggle_button_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/lab/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/kernel_start.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/notebookapp_component.ipynb
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/notebookapp_element.ipynb
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/notebookapp_widget.ipynb
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/single_file.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/single_file_multiple_routes.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/single_file_routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/food/__init__.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/food/food.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/food/index.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/multipage/01-home.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/multipage/02-my_fruit.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/multipage/03-some-markdown.md
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/multipage/05-and-notebooks.ipynb
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/multipage/06-custom-routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/multipage/99-some_other_python_script.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/multipage/some_other_file.txt
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/multipage/04-a_directory/00-another-markdown.md
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/multipage/04-a_directory/01-not-an-app.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/multipage/04-a_directory/__init__.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/multipage/10-single-file-directory/single-file.md
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/multipage-widgets/00-overview.md
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/multipage-widgets/01-views.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/multipage-widgets/02-likes.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/multipage-widgets/03-volume.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 solara_ui-1.31.0/tests/unit/solara_test_apps/multipage-widgets/04-color.ipynb
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 solara_ui-1.31.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 solara_ui-1.31.0/LICENSE
--rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 solara_ui-1.31.0/README.md
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 solara_ui-1.31.0/pyproject.toml
--rw-r--r--   0        0        0     7255 2020-02-02 00:00:00.000000 solara_ui-1.31.0/PKG-INFO
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 solara_ui-1.32.0/prefix/etc/jupyter/jupyter_notebook_config.d/solara.json
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 solara_ui-1.32.0/prefix/etc/jupyter/jupyter_server_config.d/solara.json
+-rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/__init__.py
+-rw-r--r--   0        0        0    23656 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/__main__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/alias.py
+-rw-r--r--   0        0        0    22677 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/autorouting.py
+-rw-r--r--   0        0        0    10500 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/cache.py
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/checks.html
+-rw-r--r--   0        0        0     7563 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/checks.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/comm.py
+-rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/datatypes.py
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/express.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/kitchensink.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/layout.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/lifecycle.py
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/minisettings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/py.typed
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/reactive.py
+-rw-r--r--   0        0        0     9143 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/routing.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/settings.py
+-rw-r--r--   0        0        0    30075 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/tasks.py
+-rw-r--r--   0        0        0    23570 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/toestand.py
+-rw-r--r--   0        0        0     8934 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/util.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/__init__.py
+-rw-r--r--   0        0        0     5144 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/alert.py
+-rw-r--r--   0        0        0    16621 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/applayout.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/button.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/card.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/checkbox.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/code_highlight_css.py
+-rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/code_highlight_css.vue
+-rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/columns.py
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/component_vue.py
+-rw-r--r--   0        0        0    13663 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/cross_filter.py
+-rw-r--r--   0        0        0    21033 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/dataframe.py
+-rw-r--r--   0        0        0     7836 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/datatable.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/datatable.vue
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/details.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/download.vue
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/echarts.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/echarts.vue
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/figure_altair.py
+-rw-r--r--   0        0        0     7410 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/file_browser.py
+-rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/file_download.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/file_drop.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/file_drop.vue
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/file_list_widget.vue
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/head.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/head_tag.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/head_tag.vue
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/image.py
+-rw-r--r--   0        0        0    14585 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/input.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/link.py
+-rw-r--r--   0        0        0    12502 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/markdown.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/markdown_editor.py
+-rw-r--r--   0        0        0     8864 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/markdown_editor.vue
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/matplotlib.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/meta.py
+-rw-r--r--   0        0        0    12473 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/misc.py
+-rw-r--r--   0        0        0     9938 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/pivot_table.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/pivot_table.vue
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/progress.py
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/select.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/select.vue
+-rw-r--r--   0        0        0    13408 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/slider.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/slider_date.vue
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/spinner-solara.vue
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/spinner.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/sql_code.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/sql_code.vue
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/style.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/switch.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/tab_navigation.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/title.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/title.vue
+-rw-r--r--   0        0        0     7717 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/togglebuttons.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/components/tooltip.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/hooks/__init__.py
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/hooks/dataframe.py
+-rw-r--r--   0        0        0     7885 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/hooks/misc.py
+-rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/hooks/use_reactive.py
+-rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/hooks/use_thread.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/lab/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/lab/toestand.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/lab/components/__init__.py
+-rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/lab/components/chat.py
+-rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/lab/components/confirmation_dialog.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/lab/components/cross_filter.py
+-rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/lab/components/input_date.py
+-rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/lab/components/menu.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/lab/components/menu.vue
+-rw-r--r--   0        0        0     9699 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/lab/components/tabs.py
+-rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/lab/components/theming.py
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/lab/components/theming.vue
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/lab/hooks/__init__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/lab/hooks/dataframe.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/lab/utils/__init__.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/lab/utils/cookies.py
+-rw-r--r--   0        0        0     4258 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/lab/utils/dataframe.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/lab/utils/headers.py
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/scope/__init__.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/scope/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/__init__.py
+-rw-r--r--   0        0        0    20336 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/app.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/cdn_helper.py
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/esm.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/fastapi.py
+-rw-r--r--   0        0        0     9027 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/flask.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/jupytertools.py
+-rw-r--r--   0        0        0    11092 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/kernel.py
+-rw-r--r--   0        0        0    16718 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/kernel_context.py
+-rw-r--r--   0        0        0    18788 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/patch.py
+-rw-r--r--   0        0        0     9531 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/reload.py
+-rw-r--r--   0        0        0    15746 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/server.py
+-rw-r--r--   0        0        0     7340 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/settings.py
+-rw-r--r--   0        0        0     8677 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/shell.py
+-rw-r--r--   0        0        0    23600 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/starlette.py
+-rw-r--r--   0        0        0     6038 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/telemetry.py
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/threaded.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/utils.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/websocket.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/assets/custom.css
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/assets/custom.js
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/assets/favicon.png
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/assets/favicon.svg
+-rw-r--r--   0        0        0    40341 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/assets/style.css
+-rw-r--r--   0        0        0    16733 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/assets/theme-dark.css
+-rw-r--r--   0        0        0    15637 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/assets/theme-light.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/assets/theme.js
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/jupyter/__init__.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/jupyter/cdn_handler.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/jupyter/server_extension.py
+-rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/static/ansi.js
+-rw-r--r--   0        0        0     6809 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/static/highlight-dark.css
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/static/highlight.css
+-rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/static/main-vuetify.js
+-rw-r--r--   0        0        0     5679 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/static/main.js
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/static/solara_bootstrap.py
+-rw-r--r--   0        0        0     6855 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/static/sun.svg
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/static/webworker.js
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/templates/index.html.j2
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/templates/loader-plain.css
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/templates/loader-plain.html
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/templates/loader-solara.css
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/templates/loader-solara.html
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/templates/plain.html
+-rw-r--r--   0        0        0    19668 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/server/templates/solara.html.j2
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/template/button.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/template/markdown.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/template/portal/.flake8
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/template/portal/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/template/portal/LICENSE
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/template/portal/Procfile
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/template/portal/mypy.ini
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/template/portal/pyproject.toml
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/template/portal/solara_portal/__init__.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/template/portal/solara_portal/data.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/template/portal/solara_portal/components/__init__.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/template/portal/solara_portal/components/article.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/template/portal/solara_portal/components/data.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/template/portal/solara_portal/components/header.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/template/portal/solara_portal/components/layout.py
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/template/portal/solara_portal/content/articles/equis-in-vidi.md
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/template/portal/solara_portal/content/articles/substiterat-vati.md
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/template/portal/solara_portal/pages/__init__.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/template/portal/solara_portal/pages/tabular.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/template/portal/solara_portal/pages/article/__init__.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/template/portal/solara_portal/pages/viz/__init__.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/template/portal/solara_portal/pages/viz/overview.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/test/__init__.py
+-rw-r--r--   0        0        0    26284 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/test/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/__init__.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/utils.py
+-rw-r--r--   0        0        0     9888 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/assets/custom.css
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/assets/theme.js
+-rw-r--r--   0        0        0    86383 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/assets/images/logo-small.png
+-rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/assets/images/logo.svg
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/assets/images/logo_white.svg
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/components/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/components/algolia.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/components/algolia.vue
+-rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/components/algolia_api.vue
+-rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/components/docs.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/components/header.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/components/hero.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/components/mailchimp.py
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/components/mailchimp.vue
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/components/markdown.py
+-rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/components/notebook.py
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/components/sidebar.py
+-rw-r--r--   0        0        0    31602 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/__init__.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/doc_use_download.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/docutils.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/apps/__init__.py
+-rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/apps/jupyter-dashboard-1.py
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/apps/layout-demo.py
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/apps/scatter.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/apps/scrolling.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/apps/tutorial-streamlit.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/apps/authorization/__init__.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/apps/authorization/admin.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/apps/authorization/users.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/apps/multipage/__init__.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/apps/multipage/page1.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/apps/multipage/page2.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/changelog/__init__.py
+-rw-r--r--   0        0        0    12455 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/changelog/changelog.md
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/contact/__init__.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/contact/contact.md
+-rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/__init__.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/__init__.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/00-overview.md
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/10-howto/00-overview.md
+-rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/10-howto/10-multipage.md
+-rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/10-howto/20-layout.md
+-rw-r--r--   0        0        0    19197 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/10-howto/30-testing.md
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/10-howto/31-debugging.md
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/10-howto/40-embed.md
+-rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/10-howto/50-ipywidget_libraries.md
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/15-reference/00-overview.md
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/15-reference/40-static_files.md
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/15-reference/41-asset-files.md
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/15-reference/60-static-site-generation.md
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/15-reference/70-search.md
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/15-reference/80-reloading.md
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/15-reference/90-notebook-support.md
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/15-reference/95-caching.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/20-understanding/00-introduction.md
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/20-understanding/05-ipywidgets.md
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/20-understanding/06-ipyvuetify.md
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/20-understanding/10-reacton.md
+-rw-r--r--   0        0        0     5328 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/20-understanding/12-reacton-basics.md
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/20-understanding/15-anatomy.md
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/20-understanding/17-rules-of-hooks.md
+-rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/20-understanding/18-containers.md
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/20-understanding/20-solara.md
+-rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/20-understanding/40-routing.md
+-rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/20-understanding/50-solara-server.md
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/20-understanding/60-voila.md
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/30-enterprise/00-overview.md
+-rw-r--r--   0        0        0     9095 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/30-enterprise/10-oauth.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/40-development/00-overview.md
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/40-development/01-contribute.md
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/40-development/10-setup.md
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/cross_filter/__init__.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/cross_filter/cross_filter_dataframe.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/cross_filter/cross_filter_report.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/cross_filter/cross_filter_select.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/cross_filter/cross_filter_slider.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/hooks/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/hooks/use_cross_filter.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/hooks/use_dark_effective.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/hooks/use_effect.md
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/hooks/use_effect.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/hooks/use_exception.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/hooks/use_memo.md
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/hooks/use_memo.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/hooks/use_previous.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/hooks/use_reactive.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/hooks/use_state.py
+-rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/hooks/use_state_or_update.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/hooks/use_thread.md
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/hooks/use_thread.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/hooks/use_trait_observe.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/routing/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/routing/generate_routes.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/routing/generate_routes_directory.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/routing/resolve_path.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/routing/route.py
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/routing/use_route.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/routing/use_router.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/utilities/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/utilities/component_vue.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/utilities/computed.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/utilities/display.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/utilities/get_kernel_id.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/utilities/get_session_id.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/utilities/memoize.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/utilities/on_kernel_start.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/utilities/reactive.py
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/api/utilities/widget.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/__init__.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/common.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/advanced/__init__.py
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/advanced/link.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/advanced/meta.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/advanced/style.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/data/__init__.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/data/dataframe.py
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/data/pivot_table.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/enterprise/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/enterprise/avatar.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/enterprise/avatar_menu.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/input/__init__.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/input/button.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/input/checkbox.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/input/file_browser.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/input/file_drop.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/input/input.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/input/select.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/input/slider.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/input/switch.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/input/togglebuttons.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/lab/__init__.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/lab/chat.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/lab/confirmation_dialog.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/lab/cookies_headers.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/lab/input_date.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/lab/menu.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/lab/tab.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/lab/tabs.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/lab/task.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/lab/theming.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/lab/use_task.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/layout/__init__.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/layout/app_bar.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/layout/app_bar_title.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/layout/app_layout.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/layout/card.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/layout/card_actions.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/layout/column.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/layout/columns.py
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/layout/columns_responsive.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/layout/griddraggable.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/layout/gridfixed.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/layout/hbox.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/layout/row.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/layout/sidebar.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/layout/vbox.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/output/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/output/file_download.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/output/html.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/output/image.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/output/markdown.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/output/markdown_editor.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/output/sql_code.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/output/tooltip.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/page/__init__.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/page/head.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/page/title.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/status/__init__.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/status/error.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/status/info.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/status/progress.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/status/spinner.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/status/success.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/status/warning.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/viz/__init__.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/viz/altair.py
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/viz/echarts.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/viz/matplotlib.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/viz/plotly.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/components/viz/plotly_express.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/__init__.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/ipycanvas.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/ai/__init__.py
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/ai/chatbot.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/ai/tokenizer.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/basics/__init__.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/basics/sine.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/fullscreen/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/fullscreen/authorization.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/fullscreen/layout_demo.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/fullscreen/multipage.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/fullscreen/scatter.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/fullscreen/scrolling.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/fullscreen/tutorial_streamlit.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/general/__init__.py
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/general/custom_storage.py
+-rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/general/deploy_model.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/general/live_update.py
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/general/login_oauth.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/general/mycard.vue
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/general/pokemon_search.py
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/general/vue_component.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/libraries/__init__.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/libraries/altair.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/libraries/bqplot.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/libraries/ipyleaflet.py
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/libraries/ipyleaflet_advanced.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/utilities/__init__.py
+-rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/utilities/calculator.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/utilities/countdown_timer.py
+-rw-r--r--   0        0        0     6480 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/utilities/todo.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/visualization/__init__.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/visualization/annotator.py
+-rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/visualization/linked_views.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/examples/visualization/plotly.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/faq/__init__.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/faq/content/99-faq.md
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/getting_started/__init__.py
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/00-quickstart.md
+-rw-r--r--   0        0        0     6609 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/01-introduction.md
+-rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/02-installing.md
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/80-what-is-lab.md
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/90-troubleshoot.md
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/04-tutorials/00-overview.md
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/04-tutorials/10_data_science.py
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/04-tutorials/20-web-app.md
+-rw-r--r--   0        0        0     4577 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/04-tutorials/30-ipywidgets.md
+-rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/04-tutorials/40-streamlit.md
+-rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/04-tutorials/50-dash.md
+-rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/04-tutorials/60-jupyter-dashboard-part1.py
+-rw-r--r--   0        0        0   575276 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/04-tutorials/SF_crime_sample.csv.gz
+-rw-r--r--   0        0        0    14031 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/04-tutorials/_data_science.ipynb
+-rw-r--r--   0        0        0    57417 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/04-tutorials/_jupyter_dashboard_1.ipynb
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/05-fundamentals/00-overview.md
+-rw-r--r--   0        0        0    13931 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/05-fundamentals/10-components.md
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/05-fundamentals/50-state-management.md
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/07-deploying/00-overview.md
+-rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/07-deploying/10-self-hosted.md
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/07-deploying/20-cloud-hosted.md
+-rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/showcase/__init__.py
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/showcase/domino_code_assist.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/showcase/planeto_tessa.py
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/showcase/solara_dev.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/showcase/solarathon_2023_team_2.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/showcase/solarathon_2023_team_4.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/showcase/solarathon_2023_team_5.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/showcase/solarathon_2023_team_6.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/pages/showcase/wanderlust.py
+-rw-r--r--   0        0        0    37437 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/public/beach.jpeg
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/public/logo.svg
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/public/success.html
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/public/social/discord.svg
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/public/social/github.svg
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/public/social/twitter.svg
+-rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/website/templates/index.html.j2
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/widgets/__init__.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/widgets/widgets.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/widgets/vue/gridlayout.vue
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/widgets/vue/html.vue
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/widgets/vue/navigator.vue
+-rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 solara_ui-1.32.0/solara/widgets/vue/vegalite.vue
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/__init__.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/conftest.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/docs/docs_howto_event_with_future_test.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/docs/docs_howto_event_with_polling_test.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/docs/docs_howto_no_browser_api_find_testing_test.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/docs/docs_howto_no_browser_testing_test.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/docs/docs_howto_no_browser_threaded_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/api_test.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/app_widget.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/assets_test.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/async_test.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/cdn_test.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/cmdline_test.py
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/conftest.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/create_test.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/error_test.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/esm_test.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/file_download_test.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/flask_test.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/input_date_test.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/latex_test.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/lifecycle_test.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/markdown_test.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/menu_test.py
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/popout_test.py
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/reconnect_test.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/router_test.py
+-rw-r--r--   0        0        0     7895 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/server_test.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/ssg_test.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/starlette_test.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/test.vue
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/testapp.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/widget_test.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/assets/assets1/common.js
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/assets/assets1/unique1.js
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/assets/assets2/common.js
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/assets/assets2/custom.css
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/assets/assets2/custom.js
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/assets/assets2/unique2.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/enterprise/__init__.py
+-rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/enterprise/oauth_test.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/integration/reload/apps.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/ui/snapshots/tests/integration/latex_test.py/test_widget_latex_solara-flask-chromium-linux-ipywidgets-7-changed-reference.png
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/ui/snapshots/tests/integration/latex_test.py/test_widget_latex_solara-flask-chromium-linux-ipywidgets-7-reference.png
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/ui/snapshots/tests/integration/latex_test.py/test_widget_latex_solara-flask-chromium-linux-ipywidgets-8-changed-reference.png
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/ui/snapshots/tests/integration/latex_test.py/test_widget_latex_solara-flask-chromium-linux-ipywidgets-8-reference.png
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_lab-chromium-linux-ipywidgets-7-reference.png
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_lab-chromium-linux-ipywidgets-8-reference.png
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_notebook-chromium-linux-ipywidgets-7-reference.png
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_notebook-chromium-linux-ipywidgets-8-reference.png
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-solara-chromium-linux-ipywidgets-7-reference.png
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-solara-chromium-linux-ipywidgets-8-reference.png
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-voila-chromium-linux-ipywidgets-7-reference.png
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-voila-chromium-linux-ipywidgets-8-reference.png
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-starlette-solara-chromium-linux-ipywidgets-7-reference.png
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-starlette-solara-chromium-linux-ipywidgets-8-reference.png
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-jupyter_lab-chromium-linux-reference.png
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-jupyter_notebook-chromium-linux-reference.png
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-solara-chromium-linux-reference.png
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-voila-chromium-linux-reference.png
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-starlette-solara-chromium-linux-reference.png
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-flask-chromium-linux-ipyvuetify3-reference.png
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-flask-chromium-linux-reference.png
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-starlette-chromium-linux-ipyvuetify3-reference.png
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-starlette-chromium-linux-reference.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     7898 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/app_test.py
+-rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/applayout_test.py
+-rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/autorouting_test.py
+-rw-r--r--   0        0        0     7817 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/cache_test.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/cdn_helper_test.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/chat_test.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/checkbox_test.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/common.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/component_frontend_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/component_vue_test.vue
+-rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/confirmation_dialog_test.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/conftest.py
+-rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/cross_filter_component_test.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/cross_filter_test.py
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/dataframe_test.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/datatable_test.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/display_test.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/express_test.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/file_browser_test.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/file_download_test.py
+-rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/hooks_test.py
+-rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/input_date_test.py
+-rw-r--r--   0        0        0     8001 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/input_test.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/kernel_test.py
+-rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/lifecycle_test.py
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/matplotlib_test.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/no_solara_test.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/output_widget_test.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/patch_test.py
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/pivottable_test.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/reload_test.py
+-rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/router_test.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/select_test.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/settings_test.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/shell_test.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/slider_test.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/switch_test.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/tabs_test.py
+-rw-r--r--   0        0        0    17581 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/task_test.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/telemetry_tests.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/toestand_computed_reload.py
+-rw-r--r--   0        0        0    38498 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/toestand_test.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/toggle_button_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/lab/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/kernel_start.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/notebookapp_component.ipynb
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/notebookapp_element.ipynb
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/notebookapp_widget.ipynb
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/single_file.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/single_file_multiple_routes.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/single_file_routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/food/__init__.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/food/food.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/food/index.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/multipage/01-home.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/multipage/02-my_fruit.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/multipage/03-some-markdown.md
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/multipage/05-and-notebooks.ipynb
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/multipage/06-custom-routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/multipage/99-some_other_python_script.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/multipage/some_other_file.txt
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/multipage/04-a_directory/00-another-markdown.md
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/multipage/04-a_directory/01-not-an-app.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/multipage/04-a_directory/__init__.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/multipage/10-single-file-directory/single-file.md
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/multipage-widgets/00-overview.md
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/multipage-widgets/01-views.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/multipage-widgets/02-likes.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/multipage-widgets/03-volume.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 solara_ui-1.32.0/tests/unit/solara_test_apps/multipage-widgets/04-color.ipynb
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 solara_ui-1.32.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 solara_ui-1.32.0/LICENSE
+-rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 solara_ui-1.32.0/README.md
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 solara_ui-1.32.0/pyproject.toml
+-rw-r--r--   0        0        0     7284 2020-02-02 00:00:00.000000 solara_ui-1.32.0/PKG-INFO
```

### Comparing `solara_ui-1.31.0/solara/__init__.py` & `solara_ui-1.32.0/solara/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Build webapps using IPywidgets"""
 
-__version__ = "1.31.0"
+__version__ = "1.32.0"
 github_url = "https://github.com/widgetti/solara"
 git_branch = "master"
 
 
 from . import comm  # noqa: F401
```

### Comparing `solara_ui-1.31.0/solara/__main__.py` & `solara_ui-1.32.0/solara/__main__.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/autorouting.py` & `solara_ui-1.32.0/solara/autorouting.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/cache.py` & `solara_ui-1.32.0/solara/cache.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/checks.html` & `solara_ui-1.32.0/solara/checks.html`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/checks.py` & `solara_ui-1.32.0/solara/checks.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/comm.py` & `solara_ui-1.32.0/solara/comm.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/datatypes.py` & `solara_ui-1.32.0/solara/datatypes.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/express.py` & `solara_ui-1.32.0/solara/express.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/layout.py` & `solara_ui-1.32.0/solara/layout.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/lifecycle.py` & `solara_ui-1.32.0/solara/lifecycle.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/minisettings.py` & `solara_ui-1.32.0/solara/minisettings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import inspect
 import os
 from pathlib import Path
-from typing import Any, Optional
+from typing import Any, Optional, List, Type
 
 # similar API to pydantic/pydantic-settings but we prefer not to have a dependency on pydantic
 # since we cannot be compatible with pydantic1 and 2
 # NOTE: not a public api
 
 
 def _get_type(annotation):
@@ -57,19 +58,24 @@
         return instance._values[self.name]
 
     def __set__(self, instance, value):
         instance._values[self.name] = value
 
 
 def convert(annotation, value: str) -> Any:
-    check_optional_types = [str, int, float, bool, Path]
-    for check_type in check_optional_types:
-        if annotation == Optional[check_type]:
-            annotation = check_type
+    check_sub_types: List[Type] = [str, int, float, bool, Path]
+    for sub_type in check_sub_types:
+        if annotation == Optional[sub_type]:
+            annotation = sub_type
             return convert(annotation, value)
+    for sub_type in check_sub_types:
+        if annotation == List[sub_type]:  # type: ignore
+            annotation = sub_type
+            values = value.split(",")
+            return [convert(sub_type, k) for k in values]
     if annotation == str:
         return value
     elif annotation == int:
         return int(value)
     elif annotation == float:
         return float(value)
     elif annotation == bool:
@@ -116,14 +122,16 @@
         cls.__fields__ = {}
         for key, field in cls.__dict__.items():
             if key.startswith("_"):
                 continue
             if key == "Config":
                 continue
             if not isinstance(field, _Field):
+                if inspect.isfunction(field):
+                    continue
                 field = Field(field)
                 setattr(cls, key, field)
                 field.__set_name__(cls, key)
             cls.__fields__[key] = field
 
     def dict(self, by_alias=True):
         values = self._values.copy()
```

### Comparing `solara_ui-1.31.0/solara/reactive.py` & `solara_ui-1.32.0/solara/reactive.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/routing.py` & `solara_ui-1.32.0/solara/routing.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/settings.py` & `solara_ui-1.32.0/solara/settings.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/tasks.py` & `solara_ui-1.32.0/solara/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import abc
 import asyncio
 import dataclasses
+import functools
 import inspect
 import logging
 import threading
 from enum import Enum
 from typing import (
     Any,
     Callable,
@@ -72,20 +73,21 @@
 
     @property
     def error(self):
         return self._state == TaskState.ERROR
 
 
 class Task(Generic[P, R], abc.ABC):
-    def __init__(self):
-        self._result = solara.reactive(
+    def __init__(self, key: str):
+        self._result = solara.Reactive(
             TaskResult[R](
                 value=None,
                 _state=TaskState.NOTCALLED,
-            )
+            ),
+            key="solara.tasks:TaskResult:" + key,
         )
         self._last_value: Optional[R] = None
         self._last_progress: Optional[float] = None
         self._latest = ref(self._result.fields.latest)
         self._value = ref(self._result.fields.value)
         self._error = ref(self._result.fields.error)
         self._finished = ref(self._result.fields.finished)
@@ -167,18 +169,18 @@
 
 class TaskAsyncio(Task[P, R]):
     current_task: Optional[asyncio.Task] = None
     current_future: Optional[asyncio.Future] = None
     _cancel: Optional[Callable[[], None]] = None
     _retry: Optional[Callable[[], None]] = None
 
-    def __init__(self, run_in_thread: bool, function: Callable[P, Coroutine[Any, Any, R]]):
+    def __init__(self, run_in_thread: bool, function: Callable[P, Coroutine[Any, Any, R]], key: str):
         self.run_in_thread = run_in_thread
         self.function = function
-        super().__init__()
+        super().__init__(key)
 
     def cancel(self) -> None:
         if self._cancel:
             self._cancel()
         else:
             raise RuntimeError("Cannot cancel task, never started")
 
@@ -286,16 +288,16 @@
 class TaskThreaded(Task[P, R]):
     _current_cancel_event: Optional[threading.Event] = None
     _current_thread: Optional[threading.Thread] = None
     _last_finished_event: Optional[threading.Event] = None
     _cancel: Optional[Callable[[], None]] = None
     _retry: Optional[Callable[[], None]] = None
 
-    def __init__(self, function: Callable[P, R]):
-        super().__init__()
+    def __init__(self, function: Callable[P, R], key: str):
+        super().__init__(key)
         self.__qualname__ = function.__qualname__
         self.function = function
         self.lock = threading.Lock()
 
     def cancel(self) -> None:
         if self._cancel:
             self._cancel()
@@ -663,19 +665,22 @@
         function will always run in the current event loop.
 
     ```
 
     """
 
     def wrapper(f: Union[None, Callable[P, Union[Coroutine[Any, Any, R], R]]]) -> Task[P, R]:
+        # we use wraps to make the key of the reactive variable more unique
+        # and less likely to mixup during hot reloads
+        @functools.wraps(f)  # type: ignore
         def create_task():
             if inspect.iscoroutinefunction(f):
-                return TaskAsyncio[P, R](prefer_threaded and has_threads, f)
+                return TaskAsyncio[P, R](prefer_threaded and has_threads, f, key=solara.toestand._create_key_callable(create_task))
             else:
-                return TaskThreaded[P, R](cast(Callable[P, R], f))
+                return TaskThreaded[P, R](cast(Callable[P, R], f), key=solara.toestand._create_key_callable(create_task))
 
         return cast(Task[P, R], Proxy(create_task))
 
     if f is None:
         return wrapper
     else:
         return wrapper(f)
@@ -802,15 +807,18 @@
         On platform where threads are not supported (like Pyodide / WASM / Emscripten / PyScript), a coroutine
         function will always run in the current event loop.
 
 
     """
 
     def wrapper(f):
-        task_instance = solara.use_memo(lambda: task(f, prefer_threaded=prefer_threaded), dependencies=[])
+        def create_task() -> Task[P, R]:
+            return task(f, prefer_threaded=prefer_threaded)
+
+        task_instance = solara.use_memo(create_task, dependencies=[])
         # we always update the function so we do not have stale data in the function
         task_instance.function = f  # type: ignore
 
         def _prestart():
             if dependencies is not None:
                 # we do not want to be in a state of .finished when the dependencies change
                 # otherwise user code might render a stale value with the new dependencies
@@ -824,14 +832,15 @@
                 # sure that if the user assigns to a task object, the function f
                 # starts after the assignment is executed
                 task_instance()
 
         solara.use_effect(run, dependencies=dependencies)
         if raise_error:
             if task_instance.error:
+                assert task_instance.exception is not None
                 raise task_instance.exception
         return task_instance
 
     if f is None:
         return wrapper
     else:
         return wrapper(f)
```

### Comparing `solara_ui-1.31.0/solara/toestand.py` & `solara_ui-1.32.0/solara/toestand.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,20 @@
     return use_sync_external_store(subscribe, lambda: selector(get_snapshot()))
 
 
 def merge_state(d1: S, **kwargs) -> S:
     if dataclasses.is_dataclass(d1):
         return dataclasses.replace(d1, **kwargs)  # type: ignore
     if "pydantic" in sys.modules and isinstance(d1, sys.modules["pydantic"].BaseModel):
-        return type(d1)(**{**d1.dict(), **kwargs})  # type: ignore
+        module = sys.modules["pydantic"]
+        version_major = int(module.__version__.split(".")[0])
+        if version_major >= 2:
+            return d1.model_copy(update=kwargs)
+        else:
+            return d1.copy(update=kwargs)
     return cast(S, {**cast(dict, d1), **kwargs})
 
 
 class ValueBase(Generic[T]):
     def __init__(self, merge: Callable = merge_state):
         self.merge = merge
         self.listeners: Dict[str, Set[Tuple[Callable[[T], None], Optional[ContextManager]]]] = defaultdict(set)
@@ -278,29 +283,33 @@
             key = cls.__module__ + ":" + cls.__name__ + ":" + str(index)
         super().__init__(key=key)
 
     def initial_value(self) -> S:
         return self.default_value
 
 
+def _create_key_callable(f: Callable[[], S]):
+    try:
+        prefix = f.__qualname__
+    except Exception:
+        prefix = repr(f)
+    with KernelStore.scope_lock:
+        index = KernelStore._type_counter[prefix]
+        KernelStore._type_counter[prefix] += 1
+    try:
+        key = f.__module__ + ":" + prefix + ":" + str(index)
+    except Exception:
+        key = prefix + ":" + str(index)
+    return key
+
+
 class KernelStoreFactory(KernelStore[S]):
     def __init__(self, factory: Callable[[], S], key=None):
         self.factory = factory
-        try:
-            prefix = factory.__qualname__
-        except Exception:
-            prefix = repr(factory)
-        if key is None:
-            with KernelStore.scope_lock:
-                index = self._type_counter[prefix]
-                self._type_counter[prefix] += 1
-            try:
-                key = factory.__module__ + ":" + prefix + ":" + str(index)
-            except Exception:
-                key = prefix + ":" + str(index)
+        key = key or _create_key_callable(factory)
         super().__init__(key=key)
 
     def initial_value(self) -> S:
         return self.factory()
 
 
 class Reactive(ValueBase[S]):
```

### Comparing `solara_ui-1.31.0/solara/util.py` & `solara_ui-1.32.0/solara/util.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/__init__.py` & `solara_ui-1.32.0/solara/components/__init__.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/alert.py` & `solara_ui-1.32.0/solara/components/alert.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/applayout.py` & `solara_ui-1.32.0/solara/components/applayout.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,16 +306,20 @@
                             close_on_content_click=False,
                         ):
                             pass
                             v.Sheet(children=children_sidebar, style_="padding: 12px; min-width: 400px")
                     if title or children_appbartitle:
                         v.ToolbarTitle(children=children_appbartitle or [title])
                     v.Spacer()
-                    for child in children_appbar:
-                        solara.display(child)
+                    for i, child in enumerate(children_appbar):
+                        # if the user already provided a key, don't override it
+                        if child._key is None:
+                            solara.display(child.key(f"app-layout-appbar-user-child-{i}"))
+                        else:
+                            solara.display(child)
                     solara.Button(icon_name="mdi-fullscreen", on_click=lambda: set_fullscreen(True), icon=True, dark=False)
             with v.Row(no_gutters=False, class_="solara-content-main"):
                 v.Col(cols=12, children=children_content)
     else:
         # this limits the height of the app to the height of the screen
         # and further down we use overflow: auto to add scrollbars to the main content
         # the navigation drawer adds it own scrollbars
```

### Comparing `solara_ui-1.31.0/solara/components/button.py` & `solara_ui-1.32.0/solara/components/button.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/card.py` & `solara_ui-1.32.0/solara/components/card.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/checkbox.py` & `solara_ui-1.32.0/solara/components/checkbox.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/code_highlight_css.vue` & `solara_ui-1.32.0/solara/components/code_highlight_css.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/columns.py` & `solara_ui-1.32.0/solara/components/columns.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/component_vue.py` & `solara_ui-1.32.0/solara/components/component_vue.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/cross_filter.py` & `solara_ui-1.32.0/solara/components/cross_filter.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/dataframe.py` & `solara_ui-1.32.0/solara/components/dataframe.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/datatable.py` & `solara_ui-1.32.0/solara/components/datatable.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import ipyvuetify as v
 import ipywidgets
 import solara
 import solara.hooks.dataframe
 import solara.lab
 import traitlets
 from solara.lab.hooks.dataframe import use_df_column_names
-from solara.lab.utils.dataframe import df_type
+from solara.lab.utils.dataframe import df_len, df_records, df_slice
 
 from .. import CellAction, ColumnAction
 
 
 def _ensure_dict(d):
     if dataclasses.is_dataclass(d):
         return dataclasses.asdict(d)
@@ -85,40 +85,33 @@
     format=None,
     column_actions: List[ColumnAction] = [],
     cell_actions: List[CellAction] = [],
     scrollable=False,
     on_column_header_hover: Optional[Callable[[Optional[str]], None]] = None,
     column_header_info: Optional[solara.Element] = None,
 ):
-    total_length = len(df)
+    total_length = df_len(df)
     options = {"descending": False, "page": page + 1, "itemsPerPage": items_per_page, "sortBy": [], "totalItems": total_length}
     options, set_options = solara.use_state(options, key="options")
     format = format or format_default
     # frontend does 1 base, we use 0 based
     page = options["page"] - 1
     items_per_page = options["itemsPerPage"]
     i1 = page * items_per_page
     i2 = min(total_length, (page + 1) * items_per_page)
 
     columns = use_df_column_names(df)
 
     items = []
-    column_data = {}
-    dfs = df[i1:i2]
-
-    if df_type(df) == "pandas":
-        column_data = dfs[columns].to_dict("records")
-    elif df_type(df) == "polars":
-        column_data = dfs[columns].to_dicts()
-    else:
-        column_data = dfs[columns].to_records()
+    dfs = df_slice(df, i1, i2)
+    records = df_records(dfs)
     for i in range(i2 - i1):
         item = {"__row__": i + i1}  # special key for the row number
         for column in columns:
-            item[column] = format(dfs, column, i + i1, column_data[i][column])
+            item[column] = format(dfs, column, i + i1, records[i][column])
         items.append(item)
 
     headers = [{"text": name, "value": name, "sortable": False} for name in columns]
     column_actions_callbacks = [k.on_click for k in column_actions]
     cell_actions_callbacks = [k.on_click for k in cell_actions]
     column_actions = [replace(k, on_click=None) for k in column_actions]
     cell_actions = [replace(k, on_click=None) for k in cell_actions]
```

### Comparing `solara_ui-1.31.0/solara/components/datatable.vue` & `solara_ui-1.32.0/solara/components/datatable.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/details.py` & `solara_ui-1.32.0/solara/components/details.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/download.vue` & `solara_ui-1.32.0/solara/components/download.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/echarts.py` & `solara_ui-1.32.0/solara/components/echarts.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/echarts.vue` & `solara_ui-1.32.0/solara/components/echarts.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/figure_altair.py` & `solara_ui-1.32.0/solara/components/figure_altair.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/file_browser.py` & `solara_ui-1.32.0/solara/components/file_browser.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/file_download.py` & `solara_ui-1.32.0/solara/components/file_download.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/file_drop.py` & `solara_ui-1.32.0/solara/components/file_drop.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/file_drop.vue` & `solara_ui-1.32.0/solara/components/file_drop.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/file_list_widget.vue` & `solara_ui-1.32.0/solara/components/file_list_widget.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/head.py` & `solara_ui-1.32.0/solara/components/head.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/head_tag.py` & `solara_ui-1.32.0/solara/components/head_tag.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/head_tag.vue` & `solara_ui-1.32.0/solara/components/head_tag.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/image.py` & `solara_ui-1.32.0/solara/components/image.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/input.py` & `solara_ui-1.32.0/solara/components/input.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/link.py` & `solara_ui-1.32.0/solara/components/link.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/markdown.py` & `solara_ui-1.32.0/solara/components/markdown.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/markdown_editor.py` & `solara_ui-1.32.0/solara/components/markdown_editor.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/markdown_editor.vue` & `solara_ui-1.32.0/solara/components/markdown_editor.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/matplotlib.py` & `solara_ui-1.32.0/solara/components/matplotlib.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/meta.py` & `solara_ui-1.32.0/solara/components/meta.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/misc.py` & `solara_ui-1.32.0/solara/components/misc.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/pivot_table.py` & `solara_ui-1.32.0/solara/components/pivot_table.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/pivot_table.vue` & `solara_ui-1.32.0/solara/components/pivot_table.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/progress.py` & `solara_ui-1.32.0/solara/components/progress.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/select.py` & `solara_ui-1.32.0/solara/components/select.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/select.vue` & `solara_ui-1.32.0/solara/components/select.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/slider.py` & `solara_ui-1.32.0/solara/components/slider.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/slider_date.vue` & `solara_ui-1.32.0/solara/components/slider_date.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/spinner-solara.vue` & `solara_ui-1.32.0/solara/components/spinner-solara.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/spinner.py` & `solara_ui-1.32.0/solara/components/spinner.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/sql_code.py` & `solara_ui-1.32.0/solara/components/sql_code.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/sql_code.vue` & `solara_ui-1.32.0/solara/components/sql_code.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/style.py` & `solara_ui-1.32.0/solara/components/style.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/switch.py` & `solara_ui-1.32.0/solara/components/switch.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/tab_navigation.py` & `solara_ui-1.32.0/solara/components/tab_navigation.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/title.py` & `solara_ui-1.32.0/solara/components/title.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/title.vue` & `solara_ui-1.32.0/solara/components/title.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/togglebuttons.py` & `solara_ui-1.32.0/solara/components/togglebuttons.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/components/tooltip.py` & `solara_ui-1.32.0/solara/components/tooltip.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/hooks/dataframe.py` & `solara_ui-1.32.0/solara/hooks/dataframe.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/hooks/misc.py` & `solara_ui-1.32.0/solara/hooks/misc.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/hooks/use_reactive.py` & `solara_ui-1.32.0/solara/hooks/use_reactive.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/hooks/use_thread.py` & `solara_ui-1.32.0/solara/hooks/use_thread.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/lab/__init__.py` & `solara_ui-1.32.0/solara/lab/__init__.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/lab/components/chat.py` & `solara_ui-1.32.0/solara/lab/components/chat.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/lab/components/confirmation_dialog.py` & `solara_ui-1.32.0/solara/lab/components/confirmation_dialog.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/lab/components/input_date.py` & `solara_ui-1.32.0/solara/lab/components/input_date.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/lab/components/menu.py` & `solara_ui-1.32.0/solara/lab/components/menu.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/lab/components/menu.vue` & `solara_ui-1.32.0/solara/lab/components/menu.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/lab/components/tabs.py` & `solara_ui-1.32.0/solara/lab/components/tabs.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/lab/components/theming.py` & `solara_ui-1.32.0/solara/lab/components/theming.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/lab/components/theming.vue` & `solara_ui-1.32.0/solara/lab/components/theming.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/lab/utils/dataframe.py` & `solara_ui-1.32.0/solara/lab/utils/dataframe.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,57 @@
+from typing import List
+
+
 def get_pandas_major():
     import pandas as pd
 
     return int(pd.__version__[0])
 
 
 def df_type(df):
     return df.__class__.__module__.split(".")[0]
 
 
+def df_len(df) -> int:
+    """Return the number of rows in a dataframe."""
+    return len(df)
+
+
+def df_columns(df) -> List[str]:
+    """Return a list of column names from a dataframe."""
+    if df_type(df) == "vaex":
+        return df.get_column_names()
+    elif df_type(df) == "pandas":
+        return df.columns.tolist()
+    elif df_type(df) == "polars":
+        return df.columns
+    else:
+        raise TypeError(f"{type(df)} not supported")
+
+
+def df_slice(df, start: int, stop: int):
+    """Return a subset of rows from a dataframe."""
+    if df_type(df) == "pandas":
+        return df.iloc[start:stop]
+    else:
+        return df[start:stop]
+
+
+def df_records(df) -> List[dict]:
+    """A list of records from a dataframe."""
+    if df_type(df) == "pandas":
+        return df.to_dict("records")
+    elif df_type(df) == "polars":
+        return df.to_dicts()
+    elif df_type(df) == "vaex":
+        return df.to_records()
+    else:
+        raise TypeError(f"{type(df)} not supported")
+
+
 def df_unique(df, column, limit=None):
     if df_type(df) == "vaex":
         return df.unique(column, limit=limit + 1 if limit else None, limit_raise=False)
     if df_type(df) == "pandas":
         x = df[column].unique()  # .to_numpy()
         return x[:limit]
     else:
```

### Comparing `solara_ui-1.31.0/solara/scope/__init__.py` & `solara_ui-1.32.0/solara/scope/__init__.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/scope/types.py` & `solara_ui-1.32.0/solara/scope/types.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/app.py` & `solara_ui-1.32.0/solara/server/app.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/cdn_helper.py` & `solara_ui-1.32.0/solara/server/cdn_helper.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/esm.py` & `solara_ui-1.32.0/solara/server/esm.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/flask.py` & `solara_ui-1.32.0/solara/server/flask.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,16 +158,16 @@
         logger.exception("Error in kernel handler")
         raise
 
 
 @blueprint.route("/_solara/api/close/<kernel_id>", methods=["GET", "POST"])
 def close(kernel_id: str):
     page_id = request.args["session_id"]
-    if kernel_id in kernel_context.contexts:
-        context = kernel_context.contexts[kernel_id]
+    context = kernel_context.contexts.get(kernel_id, None)
+    if context is not None:
         context.page_close(page_id)
     return ""
 
 
 @blueprint.route("/static/public/<path:path>")
 def public(path):
     if not allowed():
@@ -180,17 +180,15 @@
     return flask.Response("not found", status=404)
 
 
 @blueprint.route("/static/assets/<path:path>")
 def assets(path):
     if not allowed():
         abort(401)
-    overrides = [app.directory.parent / "assets" for app in appmod.apps.values()]
-    default = server.solara_static.parent / "assets"
-    directories = [*overrides, default]
+    directories = server.asset_directories()
     for directory in directories:
         file = directory / path
         if file.exists():
             return send_from_directory(directory, path)
     return flask.Response("not found", status=404)
```

### Comparing `solara_ui-1.31.0/solara/server/jupytertools.py` & `solara_ui-1.32.0/solara/server/jupytertools.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/kernel.py` & `solara_ui-1.32.0/solara/server/kernel.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/kernel_context.py` & `solara_ui-1.32.0/solara/server/kernel_context.py`

 * *Files 12% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     container: Optional[DOMWidget] = None
     # we track which pages are connected to implement kernel culling
     page_status: Dict[str, PageStatus] = dataclasses.field(default_factory=dict)
     # only used for testing
     _last_kernel_cull_task: "Optional[asyncio.Future[None]]" = None
     closed_event: threading.Event = dataclasses.field(default_factory=threading.Event)
     _on_close_callbacks: List[Callable[[], None]] = dataclasses.field(default_factory=list)
+    lock: threading.RLock = dataclasses.field(default_factory=threading.RLock)
 
     def __post_init__(self):
         with self:
             for f, *_ in lifecycle._on_kernel_start_callbacks:
                 cleanup = f()
                 if cleanup:
                     self.on_close(cleanup)
@@ -104,37 +105,38 @@
 
     def __exit__(self, *args):
         key = get_current_thread_key()
         assert local.kernel_context_stack is not None
         current_context[key] = local.kernel_context_stack.pop()
 
     def close(self):
-        if self.closed_event.is_set():
-            logger.error("Tried to close a kernel context that is already closed: %s", self.id)
-            return
-        logger.info("Shut down virtual kernel: %s", self.id)
-        with self:
+        with self, self.lock:
+            for key in self.page_status:
+                self.page_status[key] = PageStatus.CLOSED
+            if self.closed_event.is_set():
+                logger.error("Tried to close a kernel context that is already closed: %s", self.id)
+                return
+            logger.info("Shut down virtual kernel: %s", self.id)
             for f in reversed(self._on_close_callbacks):
                 f()
-        with self:
             if self.app_object is not None:
                 if isinstance(self.app_object, reacton.core._RenderContext):
                     try:
                         self.app_object.close()
                     except Exception as e:
                         logger.exception("Could not close render context: %s", e)
                         # we want to continue, so we at least close all widgets
             widgets.Widget.close_all()
             # what if we reference each other
             # import gc
             # gc.collect()
             self.kernel.session.close()
-        if self.id in contexts:
-            del contexts[self.id]
-        self.closed_event.set()
+            if self.id in contexts:
+                del contexts[self.id]
+            self.closed_event.set()
 
     def _state_reset(self):
         state_directory = Path(".") / "states"
         state_directory.mkdir(exist_ok=True)
         path = state_directory / f"{self.id}.pickle"
         path = path.absolute()
         try:
@@ -153,85 +155,133 @@
             state = render_context.state_get()
             with path.open("wb") as f:
                 logger.debug("State: %r", state)
                 pickle.dump(state, f)
 
     def page_connect(self, page_id: str):
         logger.info("Connect page %s for kernel %s", page_id, self.id)
-        assert self.page_status.get(page_id) != PageStatus.CLOSED, "cannot connect with the same page_id after a close"
-        self.page_status[page_id] = PageStatus.CONNECTED
-        if self._last_kernel_cull_task:
-            self._last_kernel_cull_task.cancel()
-
-    def page_disconnect(self, page_id: str) -> "asyncio.Future[None]":
-        """Signal that a page has disconnected, and schedule a kernel cull if needed.
-
-        During the kernel reconnect window, we will keep the kernel alive, even if all pages have disconnected.
-
-        Returns a future that is set when the kernel cull is done.
-        The scheduled kernel cull can be cancelled when a new page connects, a new disconnect is scheduled,
-        or a page if explicitly closed.
-        """
-        logger.info("Disconnect page %s for kernel %s", page_id, self.id)
-        future: "asyncio.Future[None]" = asyncio.Future()
-        self.page_status[page_id] = PageStatus.DISCONNECTED
-        current_event_loop = asyncio.get_event_loop()
+        with self.lock:
+            if self.closed_event.is_set():
+                raise RuntimeError("Cannot connect a page to a closed kernel")
+            if page_id in self.page_status and self.page_status.get(page_id) == PageStatus.CLOSED:
+                raise RuntimeError("Cannot connect a page that is already closed")
+            self.page_status[page_id] = PageStatus.CONNECTED
+            if self._last_kernel_cull_task:
+                logger.info("Cancelling previous kernel cull task for virtual kernel %s", self.id)
+                self._last_kernel_cull_task.cancel()
 
+    def _bump_kernel_cull(self):
         async def kernel_cull():
             try:
                 cull_timeout_sleep_seconds = solara.util.parse_timedelta(solara.server.settings.kernel.cull_timeout)
                 logger.info("Scheduling kernel cull, will wait for max %s before shutting down the virtual kernel %s", cull_timeout_sleep_seconds, self.id)
                 await asyncio.sleep(cull_timeout_sleep_seconds)
-                has_connected_pages = PageStatus.CONNECTED in self.page_status.values()
-                if has_connected_pages:
-                    logger.info("We have (re)connected pages, keeping the virtual kernel %s alive", self.id)
-                else:
-                    logger.info("No connected pages, and timeout reached, shutting down virtual kernel %s", self.id)
-                    self.close()
-                current_event_loop.call_soon_threadsafe(future.set_result, None)
+                logger.info("Timeout reached, checking if we should be shutting down virtual kernel %s", self.id)
+                with self.lock:
+                    has_connected_pages = PageStatus.CONNECTED in self.page_status.values()
+                    if has_connected_pages:
+                        logger.info("We have (re)connected pages, keeping the virtual kernel %s alive", self.id)
+                    else:
+                        logger.info("No connected pages, and timeout reached, shutting down virtual kernel %s", self.id)
+                        self.close()
+                if current_event_loop is not None and future is not None:
+                    current_event_loop.call_soon_threadsafe(future.set_result, None)
             except asyncio.CancelledError:
-                if sys.version_info >= (3, 9):
-                    current_event_loop.call_soon_threadsafe(future.cancel, "cancelled because a new cull task was scheduled")
-                else:
-                    current_event_loop.call_soon_threadsafe(future.cancel)
+                if current_event_loop is not None and future is not None:
+                    if sys.version_info >= (3, 9):
+                        current_event_loop.call_soon_threadsafe(future.cancel, "cancelled because a new cull task was scheduled")
+                    else:
+                        current_event_loop.call_soon_threadsafe(future.cancel)
                 raise
 
-        has_connected_pages = PageStatus.CONNECTED in self.page_status.values()
-        if not has_connected_pages:
-            # when we have no connected pages, we will schedule a kernel cull
+        async def create_task():
+            task = asyncio.create_task(kernel_cull())
+            # create a reference to the task so we can cancel it later
+            self._last_kernel_cull_task = task
+            await task
+
+        with self.lock:
+            future: "Optional[asyncio.Future[None]]" = None
+            current_event_loop: Optional[asyncio.AbstractEventLoop] = None
+            try:
+                future = asyncio.Future()
+                current_event_loop = asyncio.get_event_loop()
+            except RuntimeError:
+                pass
             if self._last_kernel_cull_task:
+                logger.info("Cancelling previous kernel cull tas for virtual kernel %s", self.id)
                 self._last_kernel_cull_task.cancel()
 
-            async def create_task():
-                task = asyncio.create_task(kernel_cull())
-                # create a reference to the task so we can cancel it later
-                self._last_kernel_cull_task = task
-                await task
-
+            logger.info("Scheduling kernel cull for virtual kernel %s", self.id)
             asyncio.run_coroutine_threadsafe(create_task(), keep_alive_event_loop)
-        else:
-            future.set_result(None)
-        return future
+            return future
+
+    def page_disconnect(self, page_id: str) -> "Optional[asyncio.Future[None]]":
+        """Signal that a page has disconnected, and schedule a kernel cull if needed.
+
+        During the kernel reconnect window, we will keep the kernel alive, even if all pages have disconnected.
+
+        Will return a future that is set when the kernel cull is done, when an event loop is available.
+        The scheduled kernel cull can be cancelled when a new page connects, a new disconnect is scheduled,
+        or a page if explicitly closed.
+        """
+
+        logger.info("Disconnect page %s for kernel %s", page_id, self.id)
+        future: "asyncio.Future[None]" = asyncio.Future()
+        with self.lock:
+            if self.page_status[page_id] == PageStatus.CLOSED:
+                # this happens when the close beackon call happens before the websocket disconnect
+                logger.info("Page %s already closed for kernel %s", page_id, self.id)
+                future.set_result(None)
+                return future
+            assert self.page_status[page_id] == PageStatus.CONNECTED, "cannot disconnect a page that is in state: %r" % self.page_status[page_id]
+            self.page_status[page_id] = PageStatus.DISCONNECTED
+            has_connected_pages = PageStatus.CONNECTED in self.page_status.values()
+            if not has_connected_pages:
+                # when we have no connected pages, we will schedule a kernel cull
+                future = self._bump_kernel_cull()
+            else:
+                logger.info("Still have connected pages, do nothing for kernel %s", self.id)
+                future.set_result(None)
+            return future
 
     def page_close(self, page_id: str):
-        """Signal that a page has closed, and close the context if needed.
+        """Signal that a page has closed, close the context if needed and schedule a kernel cull if needed.
 
         Closing the browser tab or a page navigation means an explicit close, which is
         different from a websocket/page disconnect, which we might want to recover from.
 
         """
-        self.page_status[page_id] = PageStatus.CLOSED
-        logger.info("Close page %s for kernel %s", page_id, self.id)
-        has_connected_pages = PageStatus.CONNECTED in self.page_status.values()
-        has_disconnected_pages = PageStatus.DISCONNECTED in self.page_status.values()
-        if not (has_connected_pages or has_disconnected_pages):
-            logger.info("No connected or disconnected pages, shutting down virtual kernel %s", self.id)
-            if self._last_kernel_cull_task:
-                self._last_kernel_cull_task.cancel()
-            self.close()
+        future: "Optional[asyncio.Future[None]]" = None
+
+        try:
+            future = asyncio.Future()
+        except RuntimeError:
+            pass
+        else:
+            future.set_result(None)
+        with self.lock:
+            if self.page_status[page_id] == PageStatus.CLOSED:
+                logger.info("Page %s already closed for kernel %s", page_id, self.id)
+                return
+            self.page_status[page_id] = PageStatus.CLOSED
+            logger.info("Close page %s for kernel %s", page_id, self.id)
+            has_connected_pages = PageStatus.CONNECTED in self.page_status.values()
+            has_disconnected_pages = PageStatus.DISCONNECTED in self.page_status.values()
+            # if we have disconnected pages, we may have cancelled the kernel cull task
+            # if we still have connected pages, it will go to a disconnected state again
+            # which will also trigger a new kernel cull
+            if has_disconnected_pages:
+                future = self._bump_kernel_cull()
+            if not (has_connected_pages or has_disconnected_pages):
+                logger.info("No connected or disconnected pages, shutting down virtual kernel %s", self.id)
+                self.close()
+            else:
+                logger.info("Still have connected or disconnected pages, keeping virtual kernel %s alive", self.id)
+        return future
 
 
 try:
     # Normal Python
     keep_alive_event_loop = asyncio.new_event_loop()
 
     def _run():
```

### Comparing `solara_ui-1.31.0/solara/server/patch.py` & `solara_ui-1.32.0/solara/server/patch.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/reload.py` & `solara_ui-1.32.0/solara/server/reload.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/server.py` & `solara_ui-1.32.0/solara/server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,14 +254,21 @@
         send_status("dead", parent=msg["header"])
         return False
     else:
         logger.error("Unsupported msg with msg_type %r", msg_type)
         return False
 
 
+def asset_directories():
+    application = [app.directory.parent / "assets" for app in app.apps.values()]
+    extra_paths = settings.assets.extra_paths()
+    solara_assets = solara_static.parent / "assets"
+    return [*application, *extra_paths, solara_assets]
+
+
 def read_root(
     path: str,
     root_path: str = "",
     render_kwargs={},
     use_nbextensions=True,
     ssg_data=None,
 ) -> Optional[str]:
@@ -288,18 +295,15 @@
     def resolve_static_path(path: str) -> Path:
         # this solve a similar problem as the starlette and flask endpoints
         # maybe this can be common code for all of them.
         if path.startswith("/static/public/"):
             directories = [default_app.directory.parent / "public"]
             filename = path[len("/static/public/") :]
         elif path.startswith("/static/assets/"):
-            directories = [
-                default_app.directory.parent / "assets",
-                solara_static.parent / "assets",
-            ]
+            directories = asset_directories()
             filename = path[len("/static/assets/") :]
         elif path.startswith("/static/"):
             directories = [solara_static.parent / "static"]
             filename = path[len("/static/") :]
         else:
             raise ValueError(f"invalid static path: {path}")
         for directory in directories:
```

### Comparing `solara_ui-1.31.0/solara/server/settings.py` & `solara_ui-1.32.0/solara/server/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
+import importlib
 import re
 import site
 import sys
 import uuid
 import warnings
 from enum import Enum
 from pathlib import Path
-from typing import Optional
+from typing import Optional, List
 
 try:
     from filelock import FileLock
 except ModuleNotFoundError:
     FileLock = None  # type: ignore
 
 import solara.util
@@ -75,14 +76,31 @@
         env_file = ".env"
 
 
 class Assets(BaseSettings):
     proxy_cache_dir: Path = Path(prefix + "/share/solara/cdn/")
     fontawesome_enabled: bool = True
     fontawesome_path: str = "/font-awesome@4.5.0/css/font-awesome.min.css"
+    extra_locations: List[str] = []
+
+    def extra_paths(self) -> List[Path]:
+        # translate locations (packages, directories) into list of paths
+        paths = []
+        for location in self.extra_locations:
+            if Path(location).exists():
+                paths.append(Path(location))
+            else:
+                try:
+                    package = importlib.import_module(location)
+                except ModuleNotFoundError:
+                    raise RuntimeError(f"Could not find {location} as a file or package (SOLARA_ASSETS_EXTRA_LOCATION={self.extra_locations!r}) ")
+                if not hasattr(package, "__path__"):
+                    raise RuntimeError(f"{location} is not a package (SOLARA_ASSETS_EXTRA_LOCATION={self.extra_locations!r}) ")
+                paths.append(Path(package.__path__[0]))
+        return paths
 
     class Config:
         env_prefix = "solara_assets_"
         case_sensitive = False
         env_file = ".env"
 
 
@@ -209,7 +227,11 @@
                 "You must set https_only for the session to True (recommended) or False in your are using your own oauth provider."
                 "Please set SOLARA_SESSION_HTTPS_ONLY in your environment to True or False"
             )
     else:
         # for the test accounts, this is fine
         if session.https_only is None:
             session.https_only = False
+
+
+# call early so a misconfiguration fails early
+assets.extra_paths()
```

### Comparing `solara_ui-1.31.0/solara/server/shell.py` & `solara_ui-1.32.0/solara/server/shell.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/starlette.py` & `solara_ui-1.32.0/solara/server/starlette.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,16 +307,16 @@
         except:  # noqa
             pass
 
 
 def close(request: Request):
     kernel_id = request.path_params["kernel_id"]
     page_id = request.query_params["session_id"]
-    if kernel_id in kernel_context.contexts:
-        context = kernel_context.contexts[kernel_id]
+    context = kernel_context.contexts.get(kernel_id, None)
+    if context is not None:
         context.page_close(page_id)
     response = HTMLResponse(content="", status_code=200)
     return response
 
 
 async def root(request: Request, fullpath: str = ""):
     if settings.oauth.private and not has_auth_support:
@@ -435,17 +435,16 @@
     def get_directories(
         self,
         directory: Union[str, "os.PathLike[str]", None] = None,
         packages=None,  # type: ignore
     ) -> List[Union[str, "os.PathLike[str]"]]:
         # we only know the .directory at runtime (after startup)
         # which means we cannot pass the directory to the StaticFiles constructor
-        overrides = [app.directory.parent / "assets" for app in appmod.apps.values()]
-        default = server.solara_static.parent / "assets"
-        return cast(List[Union[str, "os.PathLike[str]"]], [*overrides, default])
+        directories = server.asset_directories()
+        return cast(List[Union[str, "os.PathLike[str]"]], directories)
 
 
 class StaticCdn(StaticFilesOptionalAuth):
     def lookup_path(self, path: str) -> typing.Tuple[str, typing.Optional[os.stat_result]]:
         try:
             full_path = str(get_path(settings.assets.proxy_cache_dir, path))
         except Exception:
```

### Comparing `solara_ui-1.31.0/solara/server/telemetry.py` & `solara_ui-1.32.0/solara/server/telemetry.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/threaded.py` & `solara_ui-1.32.0/solara/server/threaded.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/utils.py` & `solara_ui-1.32.0/solara/server/utils.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/websocket.py` & `solara_ui-1.32.0/solara/server/websocket.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/assets/favicon.png` & `solara_ui-1.32.0/solara/server/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/assets/favicon.svg` & `solara_ui-1.32.0/solara/server/assets/favicon.svg`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/assets/style.css` & `solara_ui-1.32.0/solara/server/assets/style.css`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/assets/theme-dark.css` & `solara_ui-1.32.0/solara/server/assets/theme-dark.css`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/assets/theme-light.css` & `solara_ui-1.32.0/solara/server/assets/theme-light.css`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/jupyter/cdn_handler.py` & `solara_ui-1.32.0/solara/server/jupyter/cdn_handler.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/jupyter/server_extension.py` & `solara_ui-1.32.0/solara/server/jupyter/server_extension.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/static/ansi.js` & `solara_ui-1.32.0/solara/server/static/ansi.js`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/static/highlight-dark.css` & `solara_ui-1.32.0/solara/server/static/highlight-dark.css`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/static/highlight.css` & `solara_ui-1.32.0/solara/server/static/highlight.css`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/static/main-vuetify.js` & `solara_ui-1.32.0/solara/server/static/main-vuetify.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -131,15 +131,17 @@
     const close_url = `${solara.rootPath}/_solara/api/close/${kernelId}?session_id=${kernel.clientId}`;
     let skipReconnectedCheck = true;
     kernel.statusChanged.connect(() => {
         app.$data.kernelBusy = kernel.status == 'busy';
     });
 
     window.addEventListener('solara.router', function(event) {
-        app.$data.loadingPage = true;
+        if (kernel.status == 'busy') {
+            app.$data.loadingPage = true;
+        }
     });
     kernel.statusChanged.connect(() => {
         // the first idle after a loadingPage == true (a router event)
         // will be used as indicator that the page is loaded
         if (app.$data.loadingPage && kernel.status == 'idle') {
             app.$data.loadingPage = false;
         }
```

### Comparing `solara_ui-1.31.0/solara/server/static/main.js` & `solara_ui-1.32.0/solara/server/static/main.js`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/static/solara_bootstrap.py` & `solara_ui-1.32.0/solara/server/static/solara_bootstrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         "altair",
         "vega_datasets",
         "plotly",
         "ipycanvas",
     ]
     for dep in requirements:
         await micropip.install(dep, keep_going=True)
-    await micropip.install("/wheels/solara-1.31.0-py2.py3-none-any.whl", keep_going=True)
+    await micropip.install("/wheels/solara-1.32.0-py2.py3-none-any.whl", keep_going=True)
     import solara
 
     el = solara.Warning("lala")
     import solara
 
     solara.render_fixed(el)
     return el
```

### Comparing `solara_ui-1.31.0/solara/server/static/sun.svg` & `solara_ui-1.32.0/solara/server/static/sun.svg`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/static/webworker.js` & `solara_ui-1.32.0/solara/server/static/webworker.js`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/templates/loader-plain.html` & `solara_ui-1.32.0/solara/server/templates/loader-plain.html`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/templates/loader-solara.css` & `solara_ui-1.32.0/solara/server/templates/loader-solara.css`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/templates/loader-solara.html` & `solara_ui-1.32.0/solara/server/templates/loader-solara.html`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/templates/plain.html` & `solara_ui-1.32.0/solara/server/templates/plain.html`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/server/templates/solara.html.j2` & `solara_ui-1.32.0/solara/server/templates/solara.html.j2`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/template/markdown.py` & `solara_ui-1.32.0/solara/template/markdown.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/template/portal/.pre-commit-config.yaml` & `solara_ui-1.32.0/solara/template/portal/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/template/portal/LICENSE` & `solara_ui-1.32.0/solara/template/portal/LICENSE`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/template/portal/solara_portal/data.py` & `solara_ui-1.32.0/solara/template/portal/solara_portal/data.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/template/portal/solara_portal/components/article.py` & `solara_ui-1.32.0/solara/template/portal/solara_portal/components/article.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/template/portal/solara_portal/components/data.py` & `solara_ui-1.32.0/solara/template/portal/solara_portal/components/data.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/template/portal/solara_portal/content/articles/equis-in-vidi.md` & `solara_ui-1.32.0/solara/template/portal/solara_portal/content/articles/equis-in-vidi.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/template/portal/solara_portal/content/articles/substiterat-vati.md` & `solara_ui-1.32.0/solara/template/portal/solara_portal/content/articles/substiterat-vati.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/template/portal/solara_portal/pages/__init__.py` & `solara_ui-1.32.0/solara/template/portal/solara_portal/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/template/portal/solara_portal/pages/tabular.py` & `solara_ui-1.32.0/solara/template/portal/solara_portal/pages/tabular.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/template/portal/solara_portal/pages/article/__init__.py` & `solara_ui-1.32.0/solara/template/portal/solara_portal/pages/article/__init__.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/template/portal/solara_portal/pages/viz/__init__.py` & `solara_ui-1.32.0/solara/template/portal/solara_portal/pages/viz/__init__.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/test/pytest_plugin.py` & `solara_ui-1.32.0/solara/test/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/utils.py` & `solara_ui-1.32.0/solara/website/utils.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/assets/custom.css` & `solara_ui-1.32.0/solara/website/assets/custom.css`

 * *Files 2% similar despite different names*

```diff
@@ -235,14 +235,24 @@
     justify-content: center;
     align-items: center;
     width: 4rem;
     height: 4rem;
     border-radius: 8px;
 }
 
+.v-navigation-drawer__content .algolia {
+    padding: 0.35rem;
+}
+
+@media screen and (max-width: 960px) {
+    .header-logo-container{
+        justify-content: center !important;
+    }
+}
+
 /* vuetify component overrides */
 
 .v-btn.solara-docs-button {
     font-weight: bold;
     border-radius: 10px;
 }
 
@@ -258,14 +268,17 @@
 }
 
 .theme--dark.v-application .text--primary {
     color: var(--dark-color-primary-darker) !important;
 }
 
 /* header */
+.header-logo {
+    display: block;
+}
 .news {
     background-color: var(--color-primary);
     padding: 10px;
     font-size: 20px;
     display: flex;
     justify-content: center;
 }
```

### Comparing `solara_ui-1.31.0/solara/website/assets/images/logo-small.png` & `solara_ui-1.32.0/solara/website/assets/images/logo-small.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/assets/images/logo.svg` & `solara_ui-1.32.0/solara/website/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/assets/images/logo_white.svg` & `solara_ui-1.32.0/solara/website/assets/images/logo_white.svg`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/components/algolia_api.vue` & `solara_ui-1.32.0/solara/website/components/algolia_api.vue`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,18 @@
                     prepend-inner-icon="mdi-magnify"
                     hide-details
                     :placeholder="mac ? '⌘K to search' : 'Ctrl+K to search'"
                     outlined
                     rounded
                     clearable
                     ref="search"
-                    style="max-width: 50%; flex-grow: 1;"
+                    style="flex-grow: 1; max-width: 650px;"
                     @click="show($event, on);"
                     @keyup.enter="item = 0"
+                    class="algolia"
                 ></v-text-field>
         </template>
         <v-list v-if="results != null && results.length == 0">
             <v-list-item>
                 <v-list-item-content>
                     {{this.query == "" ? "Start Typing to Search" : "No search results found."}}
                 </v-list-item-content>
```

### Comparing `solara_ui-1.31.0/solara/website/components/docs.py` & `solara_ui-1.32.0/solara/website/components/docs.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/components/header.py` & `solara_ui-1.32.0/solara/website/components/header.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,207 +1,203 @@
 00000000: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
 00000010: 7274 2043 616c 6c61 626c 650a 0a69 6d70  rt Callable..imp
 00000020: 6f72 7420 736f 6c61 7261 0a69 6d70 6f72  ort solara.impor
 00000030: 7420 736f 6c61 7261 2e6c 6162 0a66 726f  t solara.lab.fro
 00000040: 6d20 736f 6c61 7261 2e61 6c69 6173 2069  m solara.alias i
 00000050: 6d70 6f72 7420 7276 0a66 726f 6d20 736f  mport rv.from so
 00000060: 6c61 7261 2e73 6572 7665 7220 696d 706f  lara.server impo
-00000070: 7274 2073 6574 7469 6e67 730a 0a0a 4073  rt settings...@s
-00000080: 6f6c 6172 612e 636f 6d70 6f6e 656e 745f  olara.component_
-00000090: 7675 6528 2261 6c67 6f6c 6961 5f61 7069  vue("algolia_api
-000000a0: 2e76 7565 2229 0a64 6566 2041 6c67 6f6c  .vue").def Algol
-000000b0: 6961 2829 3a0a 2020 2020 7061 7373 0a0a  ia():.    pass..
-000000c0: 0a40 736f 6c61 7261 2e63 6f6d 706f 6e65  .@solara.compone
-000000d0: 6e74 0a64 6566 2048 6561 6465 7228 0a20  nt.def Header(. 
-000000e0: 2020 206f 6e5f 746f 6767 6c65 5f6c 6566     on_toggle_lef
-000000f0: 745f 6d65 6e75 3a20 4361 6c6c 6162 6c65  t_menu: Callable
-00000100: 5b5b 5d2c 204e 6f6e 655d 203d 204e 6f6e  [[], None] = Non
-00000110: 652c 0a20 2020 206f 6e5f 746f 6767 6c65  e,.    on_toggle
-00000120: 5f72 6967 6874 5f6d 656e 753a 2043 616c  _right_menu: Cal
-00000130: 6c61 626c 655b 5b5d 2c20 4e6f 6e65 5d20  lable[[], None] 
-00000140: 3d20 4e6f 6e65 2c0a 293a 0a20 2020 2023  = None,.):.    #
-00000150: 2075 7365 2072 6f75 7465 7320 6f66 2070   use routes of p
-00000160: 6172 656e 7420 2861 7373 756d 696e 6720  arent (assuming 
-00000170: 7765 2061 7265 2061 2063 6869 6c64 206f  we are a child o
-00000180: 6620 6120 6c61 796f 7574 290a 2020 2020  f a layout).    
-00000190: 726f 7574 655f 6375 7272 656e 742c 2061  route_current, a
-000001a0: 6c6c 5f72 6f75 7465 7320 3d20 736f 6c61  ll_routes = sola
-000001b0: 7261 2e75 7365 5f72 6f75 7465 286c 6576  ra.use_route(lev
-000001c0: 656c 3d2d 3129 0a20 2020 2072 6f75 7465  el=-1).    route
-000001d0: 5f63 7572 7265 6e74 5f77 6974 685f 6368  _current_with_ch
-000001e0: 696c 6472 656e 2c20 616c 6c5f 726f 7574  ildren, all_rout
-000001f0: 6573 5f77 6974 685f 6368 696c 6472 656e  es_with_children
-00000200: 203d 2073 6f6c 6172 612e 7573 655f 726f   = solara.use_ro
-00000210: 7574 6528 290a 2020 2020 726f 7574 6572  ute().    router
-00000220: 203d 2073 6f6c 6172 612e 7573 655f 726f   = solara.use_ro
-00000230: 7574 6572 2829 0a20 2020 2064 6172 6b5f  uter().    dark_
-00000240: 6566 6665 6374 6976 6520 3d20 736f 6c61  effective = sola
-00000250: 7261 2e6c 6162 2e75 7365 5f64 6172 6b5f  ra.lab.use_dark_
-00000260: 6566 6665 6374 6976 6528 290a 0a20 2020  effective()..   
-00000270: 2023 2073 6574 2073 7461 7465 7320 666f   # set states fo
-00000280: 7220 6d65 6e75 0a20 2020 2077 6974 6820  r menu.    with 
-00000290: 736f 6c61 7261 2e43 6f6c 756d 6e28 6761  solara.Column(ga
-000002a0: 703d 2230 7078 2229 3a0a 2020 2020 2020  p="0px"):.      
-000002b0: 2020 7769 7468 2073 6f6c 6172 612e 4469    with solara.Di
-000002c0: 7628 636c 6173 7365 733d 5b22 6e65 7773  v(classes=["news
-000002d0: 225d 293a 0a20 2020 2020 2020 2020 2020  "]):.           
-000002e0: 2073 6f6c 6172 612e 4854 4d4c 280a 2020   solara.HTML(.  
-000002f0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00000300: 6976 222c 0a20 2020 2020 2020 2020 2020  iv",.           
-00000310: 2020 2020 2075 6e73 6166 655f 696e 6e65       unsafe_inne
-00000320: 7248 544d 4c3d 223c 6120 6872 6566 3d27  rHTML="<a href='
-00000330: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000340: 6f6d 2f77 6964 6765 7474 692f 736f 6c61  om/widgetti/sola
-00000350: 7261 2720 7461 7267 6574 3d27 5f62 6c61  ra' target='_bla
-00000360: 6e6b 2720 3e53 7461 7220 7573 206f 6e20  nk' >Star us on 
-00000370: 6769 7468 7562 20f0 9fa4 a93c 2f61 3e22  github ....</a>"
-00000380: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00000390: 2020 2020 2020 2020 7769 7468 2073 6f6c          with sol
-000003a0: 6172 612e 762e 4170 7042 6172 2874 6167  ara.v.AppBar(tag
-000003b0: 3d22 6865 6164 6572 222c 2066 6c61 743d  ="header", flat=
-000003c0: 5472 7565 2c20 636c 6173 735f 3d22 6267  True, class_="bg
-000003d0: 2d70 7269 6d61 7279 2d66 6164 6520 7061  -primary-fade pa
-000003e0: 6464 696e 672d 3430 222c 2068 6569 6768  dding-40", heigh
-000003f0: 743d 2261 7574 6f22 2c20 636c 6970 7065  t="auto", clippe
-00000400: 645f 6c65 6674 3d54 7275 6529 3a0a 2020  d_left=True):.  
-00000410: 2020 2020 2020 2020 2020 7769 7468 2072            with r
-00000420: 762e 546f 6f6c 6261 7254 6974 6c65 2863  v.ToolbarTitle(c
-00000430: 6c61 7373 5f3d 2264 2d66 6c65 7822 2c20  lass_="d-flex", 
-00000440: 7374 796c 655f 3d22 616c 6967 6e2d 6974  style_="align-it
-00000450: 656d 733a 6365 6e74 6572 2229 3a0a 2020  ems:center"):.  
-00000460: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00000470: 2072 6f75 7465 5f63 7572 7265 6e74 2061   route_current a
-00000480: 6e64 206c 656e 2872 6f75 7465 5f63 7572  nd len(route_cur
-00000490: 7265 6e74 2e63 6869 6c64 7265 6e29 203e  rent.children) >
-000004a0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-000004b0: 2020 2020 2020 2020 7769 7468 2073 6f6c          with sol
-000004c0: 6172 612e 4275 7474 6f6e 2869 636f 6e3d  ara.Button(icon=
-000004d0: 5472 7565 2c20 636c 6173 735f 3d22 6869  True, class_="hi
-000004e0: 6464 656e 2d6d 642d 616e 642d 7570 222c  dden-md-and-up",
-000004f0: 206f 6e5f 636c 6963 6b3d 6c61 6d62 6461   on_click=lambda
-00000500: 3a20 6f6e 5f74 6f67 676c 655f 6c65 6674  : on_toggle_left
-00000510: 5f6d 656e 7520 616e 6420 6f6e 5f74 6f67  _menu and on_tog
-00000520: 676c 655f 6c65 6674 5f6d 656e 7528 2929  gle_left_menu())
-00000530: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00000540: 2020 2020 2020 2020 2020 7276 2e49 636f            rv.Ico
-00000550: 6e28 6368 696c 6472 656e 3d5b 226d 6469  n(children=["mdi
-00000560: 2d6d 656e 7522 5d29 0a20 2020 2020 2020  -menu"]).       
-00000570: 2020 2020 2020 2020 2077 6974 6820 736f           with so
-00000580: 6c61 7261 2e4c 696e 6b28 7061 7468 5f6f  lara.Link(path_o
-00000590: 725f 726f 7574 653d 222f 2229 3a0a 2020  r_route="/"):.  
-000005a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005b0: 2020 736f 6c61 7261 2e49 6d61 6765 2872    solara.Image(r
-000005c0: 6f75 7465 722e 726f 6f74 5f70 6174 6820  outer.root_path 
-000005d0: 2b20 6622 2f73 7461 7469 632f 6173 7365  + f"/static/asse
-000005e0: 7473 2f69 6d61 6765 732f 6c6f 676f 7b27  ts/images/logo{'
-000005f0: 5f77 6869 7465 2720 6966 2064 6172 6b5f  _white' if dark_
-00000600: 6566 6665 6374 6976 6520 656c 7365 2027  effective else '
-00000610: 277d 2e73 7667 2229 0a20 2020 2020 2020  '}.svg").       
-00000620: 2020 2020 2072 762e 5370 6163 6572 2829       rv.Spacer()
-00000630: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00000640: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-00000650: 2020 2072 6f75 7465 5f63 7572 7265 6e74     route_current
-00000660: 5f77 6974 685f 6368 696c 6472 656e 2069  _with_children i
-00000670: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2020  s not None.     
-00000680: 2020 2020 2020 2020 2020 2061 6e64 2072             and r
-00000690: 6f75 7465 5f63 7572 7265 6e74 2069 7320  oute_current is 
-000006a0: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
-000006b0: 2020 2020 2020 2020 2061 6e64 2072 6f75           and rou
-000006c0: 7465 5f63 7572 7265 6e74 2e70 6174 6820  te_current.path 
-000006d0: 3d3d 2022 646f 6375 6d65 6e74 6174 696f  == "documentatio
-000006e0: 6e22 0a20 2020 2020 2020 2020 2020 2020  n".             
-000006f0: 2020 2061 6e64 2072 6f75 7465 5f63 7572     and route_cur
-00000700: 7265 6e74 5f77 6974 685f 6368 696c 6472  rent_with_childr
-00000710: 656e 2e70 6174 6820 3d3d 2022 2f22 0a20  en.path == "/". 
-00000720: 2020 2020 2020 2020 2020 2029 3a0a 2020             ):.  
-00000730: 2020 2020 2020 2020 2020 2020 2020 736f                so
-00000740: 6c61 7261 2e76 2e53 7061 6365 7228 290a  lara.v.Spacer().
-00000750: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00000760: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00000770: 2020 6966 2073 6574 7469 6e67 732e 7365    if settings.se
-00000780: 6172 6368 2e65 6e61 626c 6564 3a0a 2020  arch.enabled:.  
-00000790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007a0: 2020 6672 6f6d 2073 6f6c 6172 615f 656e    from solara_en
-000007b0: 7465 7270 7269 7365 2e73 6561 7263 682e  terprise.search.
-000007c0: 7365 6172 6368 2069 6d70 6f72 7420 5365  search import Se
-000007d0: 6172 6368 0a0a 2020 2020 2020 2020 2020  arch..          
-000007e0: 2020 2020 2020 2020 2020 5365 6172 6368            Search
-000007f0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00000800: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00000810: 2020 2020 2020 2020 2020 2020 2077 6974               wit
-00000820: 6820 736f 6c61 7261 2e52 6f77 286a 7573  h solara.Row(jus
-00000830: 7469 6679 3d22 656e 6422 2c20 7374 796c  tify="end", styl
-00000840: 653d 7b22 616c 6967 6e2d 6974 656d 7322  e={"align-items"
-00000850: 3a20 2263 656e 7465 7222 2c20 2266 6c65  : "center", "fle
-00000860: 782d 6772 6f77 223a 2022 3122 2c20 2262  x-grow": "1", "b
-00000870: 6163 6b67 726f 756e 642d 636f 6c6f 7222  ackground-color"
-00000880: 3a20 2274 7261 6e73 7061 7265 6e74 227d  : "transparent"}
-00000890: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000008a0: 2020 2020 2020 2020 2020 2041 6c67 6f6c             Algol
-000008b0: 6961 2829 0a20 2020 2020 2020 2020 2020  ia().           
-000008c0: 2077 6974 6820 7276 2e48 746d 6c28 7461   with rv.Html(ta
-000008d0: 673d 2275 6c22 2c20 636c 6173 735f 3d22  g="ul", class_="
-000008e0: 6d61 696e 2d6d 656e 7520 6d65 6e75 2064  main-menu menu d
-000008f0: 2d6e 6f6e 6520 642d 6d64 2d66 6c65 7822  -none d-md-flex"
-00000900: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00000910: 2020 2066 6f72 2072 6f75 7465 2069 6e20     for route in 
-00000920: 616c 6c5f 726f 7574 6573 3a0a 2020 2020  all_routes:.    
-00000930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000940: 6966 2072 6f75 7465 2e70 6174 6820 696e  if route.path in
-00000950: 205b 2261 7070 7322 2c20 2263 6f6e 7461   ["apps", "conta
-00000960: 6374 222c 2022 6368 616e 6765 6c6f 6722  ct", "changelog"
-00000970: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-00000980: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-00000990: 6e75 650a 2020 2020 2020 2020 2020 2020  nue.            
-000009a0: 2020 2020 2020 2020 6375 7272 656e 7420          current 
-000009b0: 3d20 726f 7574 655f 6375 7272 656e 7420  = route_current 
-000009c0: 3d3d 2072 6f75 7465 0a20 2020 2020 2020  == route.       
-000009d0: 2020 2020 2020 2020 2020 2020 2077 6974               wit
-000009e0: 6820 7276 2e48 746d 6c28 7461 673d 226c  h rv.Html(tag="l
-000009f0: 6922 2c20 636c 6173 735f 3d22 6163 7469  i", class_="acti
-00000a00: 7665 2220 6966 2063 7572 7265 6e74 2065  ve" if current e
-00000a10: 6c73 6520 4e6f 6e65 293a 0a20 2020 2020  lse None):.     
-00000a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a30: 2020 2073 6f6c 6172 612e 4c69 6e6b 2822     solara.Link("
-00000a40: 2f22 202b 2072 6f75 7465 2e70 6174 6820  /" + route.path 
-00000a50: 6966 2072 6f75 7465 2e70 6174 6820 213d  if route.path !=
-00000a60: 2022 2f22 2065 6c73 6520 222f 222c 2063   "/" else "/", c
-00000a70: 6869 6c64 7265 6e3d 5b72 6f75 7465 2e6c  hildren=[route.l
-00000a80: 6162 656c 5d29 0a20 2020 2020 2020 2020  abel]).         
-00000a90: 2020 2077 6974 6820 7276 2e42 746e 2869     with rv.Btn(i
-00000aa0: 636f 6e3d 5472 7565 2c20 7461 673d 2261  con=True, tag="a
-00000ab0: 222c 2063 6c61 7373 5f3d 2264 2d6e 6f6e  ", class_="d-non
-00000ac0: 6520 642d 6d64 2d66 6c65 7822 2c20 6174  e d-md-flex", at
-00000ad0: 7472 6962 7574 6573 3d7b 2268 7265 6622  tributes={"href"
-00000ae0: 3a20 736f 6c61 7261 2e67 6974 6875 625f  : solara.github_
-00000af0: 7572 6c2c 2022 7461 7267 6574 223a 2022  url, "target": "
-00000b00: 5f62 6c61 6e6b 227d 293a 0a20 2020 2020  _blank"}):.     
-00000b10: 2020 2020 2020 2020 2020 2072 762e 4963             rv.Ic
-00000b20: 6f6e 2863 6869 6c64 7265 6e3d 5b22 6d64  on(children=["md
-00000b30: 692d 6769 7468 7562 2d63 6972 636c 6522  i-github-circle"
-00000b40: 5d29 0a0a 2020 2020 2020 2020 2020 2020  ])..            
-00000b50: 7769 7468 2072 762e 4274 6e28 6963 6f6e  with rv.Btn(icon
-00000b60: 3d54 7275 652c 2074 6167 3d22 6122 2c20  =True, tag="a", 
-00000b70: 636c 6173 735f 3d22 642d 6e6f 6e65 2064  class_="d-none d
-00000b80: 2d6d 642d 666c 6578 222c 2061 7474 7269  -md-flex", attri
-00000b90: 6275 7465 733d 7b22 6872 6566 223a 2022  butes={"href": "
-00000ba0: 6874 7470 733a 2f2f 6469 7363 6f72 642e  https://discord.
-00000bb0: 736f 6c61 7261 2e64 6576 222c 2022 7461  solara.dev", "ta
-00000bc0: 7267 6574 223a 2022 5f62 6c61 6e6b 227d  rget": "_blank"}
-00000bd0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00000be0: 2020 2072 762e 4963 6f6e 2863 6869 6c64     rv.Icon(child
-00000bf0: 7265 6e3d 5b22 6d64 692d 6469 7363 6f72  ren=["mdi-discor
-00000c00: 6422 5d29 0a0a 2020 2020 2020 2020 2020  d"])..          
-00000c10: 2020 736f 6c61 7261 2e6c 6162 2e54 6865    solara.lab.The
-00000c20: 6d65 546f 6767 6c65 2829 0a0a 2020 2020  meToggle()..    
-00000c30: 2020 2020 2020 2020 7769 7468 2073 6f6c          with sol
-00000c40: 6172 612e 4275 7474 6f6e 2869 636f 6e3d  ara.Button(icon=
-00000c50: 5472 7565 2c20 636c 6173 735f 3d22 6869  True, class_="hi
-00000c60: 6464 656e 2d6d 642d 616e 642d 7570 222c  dden-md-and-up",
-00000c70: 206f 6e5f 636c 6963 6b3d 6c61 6d62 6461   on_click=lambda
-00000c80: 3a20 6f6e 5f74 6f67 676c 655f 7269 6768  : on_toggle_righ
-00000c90: 745f 6d65 6e75 2061 6e64 206f 6e5f 746f  t_menu and on_to
-00000ca0: 6767 6c65 5f72 6967 6874 5f6d 656e 7528  ggle_right_menu(
-00000cb0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-00000cc0: 2020 2020 7276 2e49 636f 6e28 6368 696c      rv.Icon(chil
-00000cd0: 6472 656e 3d5b 226d 6469 2d6d 656e 7522  dren=["mdi-menu"
-00000ce0: 5d29 0a                                  ]).
+00000070: 7274 2073 6574 7469 6e67 730a 6672 6f6d  rt settings.from
+00000080: 202e 616c 676f 6c69 6120 696d 706f 7274   .algolia import
+00000090: 2041 6c67 6f6c 6961 0a0a 0a40 736f 6c61   Algolia...@sola
+000000a0: 7261 2e63 6f6d 706f 6e65 6e74 0a64 6566  ra.component.def
+000000b0: 2048 6561 6465 7228 0a20 2020 206f 6e5f   Header(.    on_
+000000c0: 746f 6767 6c65 5f6c 6566 745f 6d65 6e75  toggle_left_menu
+000000d0: 3a20 4361 6c6c 6162 6c65 5b5b 5d2c 204e  : Callable[[], N
+000000e0: 6f6e 655d 203d 204e 6f6e 652c 0a20 2020  one] = None,.   
+000000f0: 206f 6e5f 746f 6767 6c65 5f72 6967 6874   on_toggle_right
+00000100: 5f6d 656e 753a 2043 616c 6c61 626c 655b  _menu: Callable[
+00000110: 5b5d 2c20 4e6f 6e65 5d20 3d20 4e6f 6e65  [], None] = None
+00000120: 2c0a 293a 0a20 2020 2023 2075 7365 2072  ,.):.    # use r
+00000130: 6f75 7465 7320 6f66 2070 6172 656e 7420  outes of parent 
+00000140: 2861 7373 756d 696e 6720 7765 2061 7265  (assuming we are
+00000150: 2061 2063 6869 6c64 206f 6620 6120 6c61   a child of a la
+00000160: 796f 7574 290a 2020 2020 726f 7574 655f  yout).    route_
+00000170: 6375 7272 656e 742c 2061 6c6c 5f72 6f75  current, all_rou
+00000180: 7465 7320 3d20 736f 6c61 7261 2e75 7365  tes = solara.use
+00000190: 5f72 6f75 7465 286c 6576 656c 3d2d 3129  _route(level=-1)
+000001a0: 0a20 2020 2072 6f75 7465 5f63 7572 7265  .    route_curre
+000001b0: 6e74 5f77 6974 685f 6368 696c 6472 656e  nt_with_children
+000001c0: 2c20 616c 6c5f 726f 7574 6573 5f77 6974  , all_routes_wit
+000001d0: 685f 6368 696c 6472 656e 203d 2073 6f6c  h_children = sol
+000001e0: 6172 612e 7573 655f 726f 7574 6528 290a  ara.use_route().
+000001f0: 2020 2020 726f 7574 6572 203d 2073 6f6c      router = sol
+00000200: 6172 612e 7573 655f 726f 7574 6572 2829  ara.use_router()
+00000210: 0a20 2020 2064 6172 6b5f 6566 6665 6374  .    dark_effect
+00000220: 6976 6520 3d20 736f 6c61 7261 2e6c 6162  ive = solara.lab
+00000230: 2e75 7365 5f64 6172 6b5f 6566 6665 6374  .use_dark_effect
+00000240: 6976 6528 290a 0a20 2020 2023 2073 6574  ive()..    # set
+00000250: 2073 7461 7465 7320 666f 7220 6d65 6e75   states for menu
+00000260: 0a20 2020 2077 6974 6820 736f 6c61 7261  .    with solara
+00000270: 2e43 6f6c 756d 6e28 6761 703d 2230 7078  .Column(gap="0px
+00000280: 2229 3a0a 2020 2020 2020 2020 7769 7468  "):.        with
+00000290: 2073 6f6c 6172 612e 4469 7628 636c 6173   solara.Div(clas
+000002a0: 7365 733d 5b22 6e65 7773 225d 293a 0a20  ses=["news"]):. 
+000002b0: 2020 2020 2020 2020 2020 2073 6f6c 6172             solar
+000002c0: 612e 4854 4d4c 280a 2020 2020 2020 2020  a.HTML(.        
+000002d0: 2020 2020 2020 2020 2264 6976 222c 0a20          "div",. 
+000002e0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+000002f0: 6e73 6166 655f 696e 6e65 7248 544d 4c3d  nsafe_innerHTML=
+00000300: 223c 6120 6872 6566 3d27 6874 7470 733a  "<a href='https:
+00000310: 2f2f 6769 7468 7562 2e63 6f6d 2f77 6964  //github.com/wid
+00000320: 6765 7474 692f 736f 6c61 7261 2720 7461  getti/solara' ta
+00000330: 7267 6574 3d27 5f62 6c61 6e6b 2720 3e53  rget='_blank' >S
+00000340: 7461 7220 7573 206f 6e20 6769 7468 7562  tar us on github
+00000350: 20f0 9fa4 a93c 2f61 3e22 2c0a 2020 2020   ....</a>",.    
+00000360: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00000370: 2020 7769 7468 2073 6f6c 6172 612e 762e    with solara.v.
+00000380: 4170 7042 6172 2874 6167 3d22 6865 6164  AppBar(tag="head
+00000390: 6572 222c 2066 6c61 743d 5472 7565 2c20  er", flat=True, 
+000003a0: 636c 6173 735f 3d22 6267 2d70 7269 6d61  class_="bg-prima
+000003b0: 7279 2d66 6164 6520 7061 6464 696e 672d  ry-fade padding-
+000003c0: 3430 222c 2068 6569 6768 743d 2261 7574  40", height="aut
+000003d0: 6f22 2c20 636c 6970 7065 645f 6c65 6674  o", clipped_left
+000003e0: 3d54 7275 6529 3a0a 2020 2020 2020 2020  =True):.        
+000003f0: 2020 2020 7769 7468 2072 762e 546f 6f6c      with rv.Tool
+00000400: 6261 7254 6974 6c65 2863 6c61 7373 5f3d  barTitle(class_=
+00000410: 2264 2d66 6c65 7822 2c20 7374 796c 655f  "d-flex", style_
+00000420: 3d22 616c 6967 6e2d 6974 656d 733a 6365  ="align-items:ce
+00000430: 6e74 6572 2229 3a0a 2020 2020 2020 2020  nter"):.        
+00000440: 2020 2020 2020 2020 6966 2072 6f75 7465          if route
+00000450: 5f63 7572 7265 6e74 2069 7320 6e6f 7420  _current is not 
+00000460: 4e6f 6e65 2061 6e64 2072 6f75 7465 5f63  None and route_c
+00000470: 7572 7265 6e74 2e6d 6f64 756c 6520 6973  urrent.module is
+00000480: 206e 6f74 204e 6f6e 6520 616e 6420 6861   not None and ha
+00000490: 7361 7474 7228 726f 7574 655f 6375 7272  sattr(route_curr
+000004a0: 656e 742e 6d6f 6475 6c65 2c20 2253 6964  ent.module, "Sid
+000004b0: 6562 6172 2229 3a0a 2020 2020 2020 2020  ebar"):.        
+000004c0: 2020 2020 2020 2020 2020 2020 7769 7468              with
+000004d0: 2073 6f6c 6172 612e 4275 7474 6f6e 2869   solara.Button(i
+000004e0: 636f 6e3d 5472 7565 2c20 636c 6173 735f  con=True, class_
+000004f0: 3d22 6869 6464 656e 2d6d 642d 616e 642d  ="hidden-md-and-
+00000500: 7570 222c 206f 6e5f 636c 6963 6b3d 6c61  up", on_click=la
+00000510: 6d62 6461 3a20 6f6e 5f74 6f67 676c 655f  mbda: on_toggle_
+00000520: 6c65 6674 5f6d 656e 7520 616e 6420 6f6e  left_menu and on
+00000530: 5f74 6f67 676c 655f 6c65 6674 5f6d 656e  _toggle_left_men
+00000540: 7528 2929 3a0a 2020 2020 2020 2020 2020  u()):.          
+00000550: 2020 2020 2020 2020 2020 2020 2020 7276                rv
+00000560: 2e49 636f 6e28 6368 696c 6472 656e 3d5b  .Icon(children=[
+00000570: 226d 6469 2d6d 656e 7522 5d29 0a0a 2020  "mdi-menu"])..  
+00000580: 2020 2020 2020 2020 2020 7769 7468 2073            with s
+00000590: 6f6c 6172 612e 526f 7728 0a20 2020 2020  olara.Row(.     
+000005a0: 2020 2020 2020 2020 2020 206a 7573 7469             justi
+000005b0: 6679 3d22 7374 6172 7422 2c20 636c 6173  fy="start", clas
+000005c0: 7365 733d 5b22 6865 6164 6572 2d6c 6f67  ses=["header-log
+000005d0: 6f2d 636f 6e74 6169 6e65 7222 5d2c 2073  o-container"], s
+000005e0: 7479 6c65 3d7b 2266 6c65 782d 6772 6f77  tyle={"flex-grow
+000005f0: 223a 2022 3122 2c20 2262 6163 6b67 726f  ": "1", "backgro
+00000600: 756e 642d 636f 6c6f 7222 3a20 2274 7261  und-color": "tra
+00000610: 6e73 7061 7265 6e74 222c 2022 616c 6967  nsparent", "alig
+00000620: 6e2d 6974 656d 7322 3a20 2263 656e 7465  n-items": "cente
+00000630: 7222 7d0a 2020 2020 2020 2020 2020 2020  r"}.            
+00000640: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00000650: 2020 2077 6974 6820 736f 6c61 7261 2e4c     with solara.L
+00000660: 696e 6b28 7061 7468 5f6f 725f 726f 7574  ink(path_or_rout
+00000670: 653d 222f 2229 3a0a 2020 2020 2020 2020  e="/"):.        
+00000680: 2020 2020 2020 2020 2020 2020 736f 6c61              sola
+00000690: 7261 2e49 6d61 6765 2872 6f75 7465 722e  ra.Image(router.
+000006a0: 726f 6f74 5f70 6174 6820 2b20 6622 2f73  root_path + f"/s
+000006b0: 7461 7469 632f 6173 7365 7473 2f69 6d61  tatic/assets/ima
+000006c0: 6765 732f 6c6f 676f 7b27 5f77 6869 7465  ges/logo{'_white
+000006d0: 2720 6966 2064 6172 6b5f 6566 6665 6374  ' if dark_effect
+000006e0: 6976 6520 656c 7365 2027 277d 2e73 7667  ive else ''}.svg
+000006f0: 222c 2063 6c61 7373 6573 3d5b 2268 6561  ", classes=["hea
+00000700: 6465 722d 6c6f 676f 225d 290a 0a20 2020  der-logo"])..   
+00000710: 2020 2020 2020 2020 2077 6974 6820 7276           with rv
+00000720: 2e48 746d 6c28 7461 673d 2275 6c22 2c20  .Html(tag="ul", 
+00000730: 636c 6173 735f 3d22 6d61 696e 2d6d 656e  class_="main-men
+00000740: 7520 6d65 6e75 2064 2d6e 6f6e 6520 642d  u menu d-none d-
+00000750: 6d64 2d66 6c65 7822 2c20 7374 796c 655f  md-flex", style_
+00000760: 3d22 666c 6578 2d67 726f 773a 2031 3b22  ="flex-grow: 1;"
+00000770: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00000780: 2020 2069 6620 7365 7474 696e 6773 2e73     if settings.s
+00000790: 6561 7263 682e 656e 6162 6c65 643a 0a20  earch.enabled:. 
+000007a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007b0: 2020 2066 726f 6d20 736f 6c61 7261 5f65     from solara_e
+000007c0: 6e74 6572 7072 6973 652e 7365 6172 6368  nterprise.search
+000007d0: 2e73 6561 7263 6820 696d 706f 7274 2053  .search import S
+000007e0: 6561 7263 680a 0a20 2020 2020 2020 2020  earch..         
+000007f0: 2020 2020 2020 2020 2020 2053 6561 7263             Searc
+00000800: 6828 290a 2020 2020 2020 2020 2020 2020  h().            
+00000810: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00000820: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+00000830: 7468 2073 6f6c 6172 612e 526f 7728 6a75  th solara.Row(ju
+00000840: 7374 6966 793d 2265 6e64 222c 2073 7479  stify="end", sty
+00000850: 6c65 3d7b 2261 6c69 676e 2d69 7465 6d73  le={"align-items
+00000860: 223a 2022 6365 6e74 6572 222c 2022 666c  ": "center", "fl
+00000870: 6578 2d67 726f 7722 3a20 2231 222c 2022  ex-grow": "1", "
+00000880: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
+00000890: 223a 2022 7472 616e 7370 6172 656e 7422  ": "transparent"
+000008a0: 7d29 3a0a 2020 2020 2020 2020 2020 2020  }):.            
+000008b0: 2020 2020 2020 2020 2020 2020 416c 676f              Algo
+000008c0: 6c69 6128 290a 0a20 2020 2020 2020 2020  lia()..         
+000008d0: 2020 2020 2020 2066 6f72 2072 6f75 7465         for route
+000008e0: 2069 6e20 616c 6c5f 726f 7574 6573 3a0a   in all_routes:.
+000008f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000900: 2020 2020 6966 2072 6f75 7465 2e70 6174      if route.pat
+00000910: 6820 696e 205b 2261 7070 7322 2c20 2263  h in ["apps", "c
+00000920: 6f6e 7461 6374 222c 2022 6368 616e 6765  ontact", "change
+00000930: 6c6f 6722 5d3a 0a20 2020 2020 2020 2020  log"]:.         
+00000940: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00000950: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
+00000960: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00000970: 656e 7420 3d20 726f 7574 655f 6375 7272  ent = route_curr
+00000980: 656e 7420 3d3d 2072 6f75 7465 0a20 2020  ent == route.   
+00000990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009a0: 2077 6974 6820 7276 2e48 746d 6c28 7461   with rv.Html(ta
+000009b0: 673d 226c 6922 2c20 636c 6173 735f 3d22  g="li", class_="
+000009c0: 6163 7469 7665 2220 6966 2063 7572 7265  active" if curre
+000009d0: 6e74 2065 6c73 6520 4e6f 6e65 293a 0a20  nt else None):. 
+000009e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009f0: 2020 2020 2020 2073 6f6c 6172 612e 4c69         solara.Li
+00000a00: 6e6b 2822 2f22 202b 2072 6f75 7465 2e70  nk("/" + route.p
+00000a10: 6174 6820 6966 2072 6f75 7465 2e70 6174  ath if route.pat
+00000a20: 6820 213d 2022 2f22 2065 6c73 6520 222f  h != "/" else "/
+00000a30: 222c 2063 6869 6c64 7265 6e3d 5b72 6f75  ", children=[rou
+00000a40: 7465 2e6c 6162 656c 5d29 0a20 2020 2020  te.label]).     
+00000a50: 2020 2020 2020 2077 6974 6820 7276 2e42         with rv.B
+00000a60: 746e 2869 636f 6e3d 5472 7565 2c20 7461  tn(icon=True, ta
+00000a70: 673d 2261 222c 2063 6c61 7373 5f3d 2264  g="a", class_="d
+00000a80: 2d6e 6f6e 6520 642d 6d64 2d66 6c65 7822  -none d-md-flex"
+00000a90: 2c20 6174 7472 6962 7574 6573 3d7b 2268  , attributes={"h
+00000aa0: 7265 6622 3a20 736f 6c61 7261 2e67 6974  ref": solara.git
+00000ab0: 6875 625f 7572 6c2c 2022 7461 7267 6574  hub_url, "target
+00000ac0: 223a 2022 5f62 6c61 6e6b 227d 293a 0a20  ": "_blank"}):. 
+00000ad0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00000ae0: 762e 4963 6f6e 2863 6869 6c64 7265 6e3d  v.Icon(children=
+00000af0: 5b22 6d64 692d 6769 7468 7562 2d63 6972  ["mdi-github-cir
+00000b00: 636c 6522 5d29 0a0a 2020 2020 2020 2020  cle"])..        
+00000b10: 2020 2020 7769 7468 2072 762e 4274 6e28      with rv.Btn(
+00000b20: 6963 6f6e 3d54 7275 652c 2074 6167 3d22  icon=True, tag="
+00000b30: 6122 2c20 636c 6173 735f 3d22 642d 6e6f  a", class_="d-no
+00000b40: 6e65 2064 2d6d 642d 666c 6578 222c 2061  ne d-md-flex", a
+00000b50: 7474 7269 6275 7465 733d 7b22 6872 6566  ttributes={"href
+00000b60: 223a 2022 6874 7470 733a 2f2f 6469 7363  ": "https://disc
+00000b70: 6f72 642e 736f 6c61 7261 2e64 6576 222c  ord.solara.dev",
+00000b80: 2022 7461 7267 6574 223a 2022 5f62 6c61   "target": "_bla
+00000b90: 6e6b 227d 293a 0a20 2020 2020 2020 2020  nk"}):.         
+00000ba0: 2020 2020 2020 2072 762e 4963 6f6e 2863         rv.Icon(c
+00000bb0: 6869 6c64 7265 6e3d 5b22 6d64 692d 6469  hildren=["mdi-di
+00000bc0: 7363 6f72 6422 5d29 0a0a 2020 2020 2020  scord"])..      
+00000bd0: 2020 2020 2020 736f 6c61 7261 2e6c 6162        solara.lab
+00000be0: 2e54 6865 6d65 546f 6767 6c65 2829 0a0a  .ThemeToggle()..
+00000bf0: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00000c00: 2073 6f6c 6172 612e 4275 7474 6f6e 2869   solara.Button(i
+00000c10: 636f 6e3d 5472 7565 2c20 636c 6173 735f  con=True, class_
+00000c20: 3d22 6869 6464 656e 2d6d 642d 616e 642d  ="hidden-md-and-
+00000c30: 7570 222c 206f 6e5f 636c 6963 6b3d 6c61  up", on_click=la
+00000c40: 6d62 6461 3a20 6f6e 5f74 6f67 676c 655f  mbda: on_toggle_
+00000c50: 7269 6768 745f 6d65 6e75 2061 6e64 206f  right_menu and o
+00000c60: 6e5f 746f 6767 6c65 5f72 6967 6874 5f6d  n_toggle_right_m
+00000c70: 656e 7528 2929 3a0a 2020 2020 2020 2020  enu()):.        
+00000c80: 2020 2020 2020 2020 7276 2e49 636f 6e28          rv.Icon(
+00000c90: 6368 696c 6472 656e 3d5b 226d 6469 2d6d  children=["mdi-m
+00000ca0: 656e 7522 5d29 0a                        enu"]).
```

### Comparing `solara_ui-1.31.0/solara/website/components/hero.py` & `solara_ui-1.32.0/solara/website/components/hero.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/components/mailchimp.vue` & `solara_ui-1.32.0/solara/website/components/mailchimp.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/components/markdown.py` & `solara_ui-1.32.0/solara/website/components/markdown.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/components/notebook.py` & `solara_ui-1.32.0/solara/website/components/notebook.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/__init__.py` & `solara_ui-1.32.0/solara/website/pages/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import contextlib
-
 import solara
 from solara import autorouting
 from solara.alias import rv
 from solara.components.title import Title
 from solara.server import server
+from solara.website.components.algolia import Algolia
 
 from ..components import Header, Hero
 from ..components.mailchimp import MailChimp
 
 title = "Home"
 
 route_order = ["/", "showcase", "documentation", "apps", "contact", "changelog"]
@@ -234,47 +233,14 @@
 
 @solara.component
 def List(children=[], class_: str = None):
     return rv.Html(tag="ul", children=children, attributes={"class": class_})
 
 
 @solara.component
-def Sidebar():
-    route_current, all_routes = solara.use_route()
-    router = solara.use_router()
-    selected = router.path
-    with rv.Col(tag="aside", md=4, lg=3, class_="sidebar bg-grey d-none d-md-block") as main:
-        with List():
-            for route in all_routes:
-                if route.children and route.data is None:
-                    path = solara.resolve_path(route.children[0])
-                    path = getattr(route.module, "redirect", path)
-                    path = getattr(route.children[0].module, "redirect", path)
-                    with solara.Link(path) if path is not None else contextlib.nullcontext():
-                        with SimpleListItem(route.label, class_="active" if path == selected else None):
-                            with List():
-                                for child in route.children[1:]:
-                                    path = solara.resolve_path(child)
-                                    path = getattr(child.module, "redirect", path)
-                                    with solara.Link(path) if path is not None else contextlib.nullcontext():
-                                        title = child.label or "no label"
-                                        if callable(title):
-                                            title = "Error: dynamic title"
-                                        SimpleListItem(title, class_="active" if path == selected else None)
-                else:
-                    path = solara.resolve_path(route)
-                    path = getattr(route.module, "redirect", path)
-                    if route.children:
-                        path = getattr(route.children[0].module, "redirect", path)
-                    with solara.Link(path) if path is not None else contextlib.nullcontext():
-                        SimpleListItem(route.label, class_="active" if path == selected else None)
-    return main
-
-
-@solara.component
 def Layout(children=[]):
     router = solara.use_router()
     route_current, all_routes = solara.use_route()
     route_sidebar_current, all_routes_sidebar = solara.use_route(1)
 
     show_left_menu, set_show_left_menu = solara.use_state(False)
     show_right_menu, set_show_right_menu = solara.use_state(False)
@@ -472,25 +438,30 @@
                         with solara.Div(style={"width": "80%"}):
                             MailChimp(location=router.path)
             else:
                 with rv.Row(
                     style_="flex-wrap: nowrap; margin: 0; min-height: calc(100vh - 215.5px);",
                     justify="center" if route_current is not None and route_current.path in ["documentation", "showcase"] else "start",
                 ):
-                    if route_current is not None and hasattr(route_current.module, "Sidebar"):
-                        route_current.module.Sidebar()  # type: ignore
-                    else:
-                        if route_current is not None and route_current.path not in ["documentation", "showcase", "contact", "changelog"]:
-                            Sidebar()
+                    if route_current is not None and route_current.module is not None and hasattr(route_current.module, "Sidebar"):
+                        with solara.v.NavigationDrawer(
+                            clipped=True,
+                            class_="d-none d-md-block",
+                            height="unset",
+                            style_="min-height: calc(100vh - 215.5px);",
+                            width="20rem",
+                            v_model=True,  # Forces menu to display even if it had somehow been closed
+                        ):
+                            route_current.module.Sidebar()
                     with rv.Col(
                         tag="main",
                         md=True,
                         class_="pa-0",
                         style_=f"""max-width: {'1024px' if route_current.path not in ['documentation', 'contact', 'changelog']
-                                               else 'unset'}; overflow: hidden auto;""",
+                                               else 'unset'}; overflow-x: hidden;""",
                     ):
                         if route_current is not None and route_current.path == "/":
                             with rv.Row(align="center"):
                                 pass
                         with solara.Row(
                             children=children,
                             justify="center",
@@ -508,48 +479,35 @@
                 absolute=True,
                 right=True,
                 hide_overlay=False,
                 overlay_color="#000000",
                 overlay_opacity=0.5,
                 style_="height: 100vh",
             ):
+                Algolia()
                 with rv.List(nav=True):
                     with rv.ListItemGroup(active_class="text--primary"):
                         for route in all_routes:
                             if route.path == "apps":
                                 continue
                             with solara.Link(route):
                                 solara.ListItem(route.label)
 
-            # Drawer navigation for sidebar
-            with rv.NavigationDrawer(
-                v_model=show_left_menu,
-                on_v_model=set_show_left_menu,
-                fixed=True,
-                absolute=True,
-                hide_overlay=False,
-                overlay_color="#000000",
-                overlay_opacity=0.5,
-                style_="height: 100vh",
-            ):
-                with rv.List(nav=True):
-                    current_path = router.path
-                    with rv.ListItemGroup(active_class="text--primary", v_model=current_path):
-                        for route in all_routes_sidebar:
-                            # this gets rid of the api/link child routes
-                            if len([k for k in route.children if k.label]) == 0:
-                                with solara.Link(route):
-                                    solara.ListItem(route.label, value=solara.resolve_path(route))
-                            else:
-                                with solara.ListItem(route.label or "no-title", value=solara.resolve_path(route) + "_no_select"):
-                                    for subroute in route.children:
-                                        if subroute.label:
-                                            with solara.Link(subroute):
-                                                with solara.ListItem(subroute.label, value=solara.resolve_path(subroute)):
-                                                    pass
+            if route_current is not None and route_current.module is not None and hasattr(route_current.module, "Sidebar"):
+                with solara.v.NavigationDrawer(
+                    absolute=True,
+                    clipped=True,
+                    class_="d-md-none d-block",
+                    height="unset",
+                    style_="min-height: 100vh;",
+                    v_model=show_left_menu,
+                    on_v_model=set_show_left_menu,
+                    width="20rem",
+                ):
+                    route_current.module.Sidebar()
 
     return main
 
 
 @solara.component
 def Testimonial(text, name, position, img):
     max_width = "300px"
```

### Comparing `solara_ui-1.31.0/solara/website/pages/doc_use_download.py` & `solara_ui-1.32.0/solara/website/pages/doc_use_download.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/docutils.py` & `solara_ui-1.32.0/solara/website/pages/docutils.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/apps/jupyter-dashboard-1.py` & `solara_ui-1.32.0/solara/website/pages/apps/jupyter-dashboard-1.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/apps/layout-demo.py` & `solara_ui-1.32.0/solara/website/pages/apps/layout-demo.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/apps/scatter.py` & `solara_ui-1.32.0/solara/website/pages/apps/scatter.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/apps/scrolling.py` & `solara_ui-1.32.0/solara/website/pages/apps/scrolling.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/apps/authorization/__init__.py` & `solara_ui-1.32.0/solara/website/pages/apps/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/apps/multipage/__init__.py` & `solara_ui-1.32.0/solara/website/pages/apps/multipage/__init__.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/apps/multipage/page1.py` & `solara_ui-1.32.0/solara/website/pages/apps/multipage/page1.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/apps/multipage/page2.py` & `solara_ui-1.32.0/solara/website/pages/apps/multipage/page2.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/changelog/changelog.md` & `solara_ui-1.32.0/solara/website/pages/changelog/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # Solara Changelog
 
+
+## Version 1.31
+
+We changed solara from a single package into multiple packages.
+
+The `solara` package is a meta package that installs all the necessary dependencies to get started with Solara. By default, we install:
+
+  * [`pip install "solara-ui[all]"`](https://pypi.org/project/solara-ui)
+  * [`pip install "solara-server[starlette,dev]"`](https://pypi.org/project/solara-ui)
+
+Notebook users can simply install `solara-ui` if they do not need the solara-server. Read our [installation guide](https://solara.dev/documentation/getting_started/installing) for more information.
+
 ## Version 1.30.1
 
 ### Details
 
    * Bug Fix: Serialization error from attempt to serialize default event handles in `component_vue`. [793cbb1](https://github.com/widgetti/solara/commit/793cbb19d8c361490b7e0b1e436a3e9ef3acea71)
    * Bug Fix: `on_kernel_start` callback cleanups could have been triggered multiple times. [4b75ca9](https://github.com/widgetti/solara/commit/4b75ca934f4e905a3592911bfca6657e491d1425)
    * Bug Fix: Autorender did not render child routes. [#575](https://github.com/widgetti/solara/pull/575)
```

### Comparing `solara_ui-1.31.0/solara/website/pages/contact/contact.md` & `solara_ui-1.32.0/solara/website/pages/contact/contact.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/10-howto/10-multipage.md` & `solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/10-howto/10-multipage.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/10-howto/20-layout.md` & `solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/10-howto/20-layout.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/10-howto/31-debugging.md` & `solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/10-howto/31-debugging.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/10-howto/40-embed.md` & `solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/10-howto/40-embed.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/10-howto/50-ipywidget_libraries.md` & `solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/10-howto/50-ipywidget_libraries.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/15-reference/40-static_files.md` & `solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/15-reference/40-static_files.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/15-reference/60-static-site-generation.md` & `solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/15-reference/60-static-site-generation.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/15-reference/70-search.md` & `solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/15-reference/70-search.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/15-reference/80-reloading.md` & `solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/15-reference/80-reloading.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/15-reference/95-caching.md` & `solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/15-reference/95-caching.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/20-understanding/00-introduction.md` & `solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/20-understanding/00-introduction.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/20-understanding/05-ipywidgets.md` & `solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/20-understanding/05-ipywidgets.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/20-understanding/06-ipyvuetify.md` & `solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/20-understanding/06-ipyvuetify.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/20-understanding/10-reacton.md` & `solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/20-understanding/10-reacton.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/20-understanding/12-reacton-basics.md` & `solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/20-understanding/12-reacton-basics.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/20-understanding/15-anatomy.md` & `solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/20-understanding/15-anatomy.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/20-understanding/18-containers.md` & `solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/20-understanding/18-containers.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/20-understanding/20-solara.md` & `solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/20-understanding/20-solara.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/20-understanding/40-routing.md` & `solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/20-understanding/40-routing.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/20-understanding/50-solara-server.md` & `solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/20-understanding/50-solara-server.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/20-understanding/60-voila.md` & `solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/20-understanding/60-voila.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/30-enterprise/10-oauth.md` & `solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/30-enterprise/10-oauth.md`

 * *Files 6% similar despite different names*

```diff
@@ -129,16 +129,16 @@
 
 ### Configuring Fief
 
 You can also configure Solara to use our Fief test account. To do this, you need to set the following environment variables:
 
 ```bash
 SOLARA_SESSION_SECRET_KEY="change me"  # required if you don't use the default test account
-SOLARA_OAUTH_CLIENT_ID="x2np62qgwp6hnEGTP4JYUE3igdZWhT-AvjpjwwDyKXU"  # found in the Auth0 dashboard Clients->General Tab->Secret
-SOLARA_OAUTH_CLIENT_SECRET="XQlByE1pVIz5h2SBN2GYDwT_ziqArHJgLD3KqMlCHjg" # found in the Auth0 dashboard Clients->General Tab->ID
+SOLARA_OAUTH_CLIENT_ID="x2np62qgwp6hnEGTP4JYUE3igdZWhT-AvjpjwwDyKXU"  # found in the Auth0 dashboard Clients->General Tab->ID
+SOLARA_OAUTH_CLIENT_SECRET="XQlByE1pVIz5h2SBN2GYDwT_ziqArHJgLD3KqMlCHjg" # found in the Auth0 dashboard Clients->General Tab->Secret
 SOLARA_OAUTH_API_BASE_URL="solara-dev.fief.dev"  # found in the Fief dashboard Tenants->Base URL
  # different from Solara's default
 SOLARA_OAUTH_LOGOUT_PATH="logout"
 ```
 
 ### Generating a secret key
 
@@ -165,7 +165,16 @@
 
 
 ## Possible issues
 
 ### Wrong redirection
 
 If the redirection back to solara return to the wrong address, it might be due to solara not choosing the right default for `SOLARA_BASE_URL`. For instance this variable could be set to `SOLARA_BASE_URL=https://solara.dev` for the solara.dev server. If you application runs behind a subpath, e.g. `/myapp`, you might have to set `SOLARA_ROOT_PATH=/myapp`.
+
+
+### Wrong schema detected for redirect URL
+
+Solara needs to give the OAuth providers a redirect URL to get back to your Solara application after navigating to the OAuth provider website. For our documentation server, we ask the OAuth provider to redirect to `https://solara.dev/_solara/auth/authorize`. The protocol part (`https`) and the domain name part (`solara.dev`) or this URL is constructed from the request URL (what the browser sends to the server).
+
+If you are running Aolara behind a reverse proxy server (like nginx), make sure that the `X-Forwarded-Proto` and `Host` headers are forwarded correctly so Solara can construct the correct redirect URL to send to the OAuth provider.
+
+See our [self hosted deployment](https://solara.dev/documentation/getting_started/deploying/self-hosted) for more information on how to configure your reverse proxy server.
```

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/40-development/01-contribute.md` & `solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/40-development/01-contribute.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/advanced/content/40-development/10-setup.md` & `solara_ui-1.32.0/solara/website/pages/documentation/advanced/content/40-development/10-setup.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 See also [the contributing guide](/documentation/advanced/development/contribute) for more information on how to contribute to Solara.
 ## Development setup
 
 Assuming you have created a virtual environment as described in [the installation guide](/documentation/getting_started/installing), you can install a development install of Solara using:
 
     $ git clone git@github.com:widgetti/solara.git
     $ cd solara
-    $ pip install ".[dev,documentation]"  # documentation is optional
+    $ pip install -r requirements-dev.txt
 
 
 ## Running Solara server in auto restart mode
 
 By passing the `--auto-restart/-a` flag, the solara server will automatically restart when the sourcecode of the solara server changes, which makes it friendlier for development
 
     $ solara run myscript.py -a
```

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/api/hooks/use_cross_filter.py` & `solara_ui-1.32.0/solara/website/pages/documentation/api/hooks/use_cross_filter.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/api/hooks/use_effect.md` & `solara_ui-1.32.0/solara/website/pages/documentation/api/hooks/use_effect.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/api/hooks/use_exception.py` & `solara_ui-1.32.0/solara/website/pages/documentation/api/hooks/use_exception.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/api/hooks/use_memo.md` & `solara_ui-1.32.0/solara/website/pages/documentation/api/hooks/use_memo.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/api/hooks/use_previous.py` & `solara_ui-1.32.0/solara/website/pages/documentation/api/hooks/use_previous.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/api/hooks/use_state_or_update.py` & `solara_ui-1.32.0/solara/website/pages/documentation/api/hooks/use_state_or_update.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/api/hooks/use_thread.md` & `solara_ui-1.32.0/solara/website/pages/documentation/api/hooks/use_thread.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/api/hooks/use_thread.py` & `solara_ui-1.32.0/solara/website/pages/documentation/api/hooks/use_thread.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/api/routing/resolve_path.py` & `solara_ui-1.32.0/solara/website/pages/documentation/api/routing/resolve_path.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/api/routing/route.py` & `solara_ui-1.32.0/solara/website/pages/documentation/api/routing/route.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/api/routing/use_route.py` & `solara_ui-1.32.0/solara/website/pages/documentation/api/routing/use_route.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/api/utilities/memoize.py` & `solara_ui-1.32.0/solara/website/pages/documentation/api/utilities/memoize.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/api/utilities/on_kernel_start.py` & `solara_ui-1.32.0/solara/website/pages/documentation/api/utilities/on_kernel_start.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/api/utilities/widget.py` & `solara_ui-1.32.0/solara/website/pages/documentation/api/utilities/widget.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/advanced/link.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/advanced/link.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/advanced/meta.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/advanced/meta.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/advanced/style.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/advanced/style.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/data/dataframe.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/data/dataframe.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/data/pivot_table.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/data/pivot_table.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/input/file_browser.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/input/file_browser.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/input/file_drop.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/input/file_drop.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/input/slider.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/input/slider.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/lab/chat.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/lab/chat.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/lab/confirmation_dialog.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/lab/confirmation_dialog.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/lab/cookies_headers.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/lab/cookies_headers.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/lab/tab.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/lab/tab.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/lab/tabs.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/lab/tabs.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/lab/theming.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/lab/theming.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/layout/column.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/layout/column.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/layout/columns.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/layout/columns.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/layout/columns_responsive.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/layout/columns_responsive.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/layout/griddraggable.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/layout/griddraggable.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/layout/row.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/layout/row.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/layout/sidebar.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/layout/sidebar.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/output/markdown.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/output/markdown.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/output/markdown_editor.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/output/markdown_editor.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/output/sql_code.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/output/sql_code.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/page/title.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/page/title.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/status/error.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/status/error.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/status/info.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/status/info.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/status/success.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/status/success.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/status/warning.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/status/warning.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/viz/altair.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/viz/altair.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/viz/echarts.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/viz/echarts.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/viz/matplotlib.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/viz/matplotlib.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/viz/plotly.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/viz/plotly.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/components/viz/plotly_express.py` & `solara_ui-1.32.0/solara/website/pages/documentation/components/viz/plotly_express.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/examples/__init__.py` & `solara_ui-1.32.0/solara/website/pages/documentation/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/examples/ipycanvas.py` & `solara_ui-1.32.0/solara/website/pages/documentation/examples/ipycanvas.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/examples/ai/chatbot.py` & `solara_ui-1.32.0/solara/website/pages/documentation/examples/ai/chatbot.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/examples/ai/tokenizer.py` & `solara_ui-1.32.0/solara/website/pages/documentation/examples/ai/tokenizer.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/examples/basics/sine.py` & `solara_ui-1.32.0/solara/website/pages/documentation/examples/basics/sine.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/examples/general/custom_storage.py` & `solara_ui-1.32.0/solara/website/pages/documentation/examples/general/custom_storage.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/examples/general/deploy_model.py` & `solara_ui-1.32.0/solara/website/pages/documentation/examples/general/deploy_model.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/examples/general/live_update.py` & `solara_ui-1.32.0/solara/website/pages/documentation/examples/general/live_update.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/examples/general/login_oauth.py` & `solara_ui-1.32.0/solara/website/pages/documentation/examples/general/login_oauth.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/examples/general/mycard.vue` & `solara_ui-1.32.0/solara/website/pages/documentation/examples/general/mycard.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/examples/general/pokemon_search.py` & `solara_ui-1.32.0/solara/website/pages/documentation/examples/general/pokemon_search.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/examples/general/vue_component.py` & `solara_ui-1.32.0/solara/website/pages/documentation/examples/general/vue_component.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/examples/libraries/altair.py` & `solara_ui-1.32.0/solara/website/pages/documentation/examples/libraries/altair.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/examples/libraries/bqplot.py` & `solara_ui-1.32.0/solara/website/pages/documentation/examples/libraries/bqplot.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/examples/libraries/ipyleaflet.py` & `solara_ui-1.32.0/solara/website/pages/documentation/examples/libraries/ipyleaflet.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/examples/libraries/ipyleaflet_advanced.py` & `solara_ui-1.32.0/solara/website/pages/documentation/examples/libraries/ipyleaflet_advanced.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/examples/utilities/calculator.py` & `solara_ui-1.32.0/solara/website/pages/documentation/examples/utilities/calculator.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/examples/utilities/countdown_timer.py` & `solara_ui-1.32.0/solara/website/pages/documentation/examples/utilities/countdown_timer.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/examples/utilities/todo.py` & `solara_ui-1.32.0/solara/website/pages/documentation/examples/utilities/todo.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/examples/visualization/annotator.py` & `solara_ui-1.32.0/solara/website/pages/documentation/examples/visualization/annotator.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/examples/visualization/linked_views.py` & `solara_ui-1.32.0/solara/website/pages/documentation/examples/visualization/linked_views.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/examples/visualization/plotly.py` & `solara_ui-1.32.0/solara/website/pages/documentation/examples/visualization/plotly.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/faq/content/99-faq.md` & `solara_ui-1.32.0/solara/website/pages/documentation/faq/content/99-faq.md`

 * *Files 14% similar despite different names*

```diff
@@ -70,7 +70,34 @@
    * SERVER_PORT (e.g. '8765')
    * SERVER_NAME (e.g. 'killerapp.com')
    * SCRIPT_NAME (only Voila, e.g. 'voila/render/notebook.ipynb')
    * PATH_TRANSLATED (only Solara e.g. '/mnt/someapp/app.py')
 
 Jupyter Notebook/Lab/Server do not set these variables. With this information,
 it should be possible to recognize in which environment you are running in.
+
+
+## I cannot find or run `solara` from the command line
+
+
+On Linux or OSX you might see
+
+```
+$ solara
+command not found: solara
+```
+
+On Windows you might see
+
+```
+C:Users\myusername> solara
+solara: The term 'solara' is not recognized as the name of a cdlet, function,
+script file, or operable program.
+```
+
+The solara command before version 1.30 was installed with the package `solara`, but now it is installed with the package `solara-server`.
+
+If you upgrade from an older version to 1.30 or later, the order in which pip installs packages can cause the `solara` command to be uninstalled. To fix this, reinstall the `solara-server` package:
+
+```bash
+$ pip install solara-server --force-reinstall
+```
```

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/00-quickstart.md` & `solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/00-quickstart.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/01-introduction.md` & `solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/01-introduction.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/02-installing.md` & `solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/02-installing.md`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 ```
 
 ## Solara subpackages
 
 The `solara` package is a meta package that installs all the necessary dependencies to get started with Solara. By default, we install:
 
   * [`pip install "solara-ui[all]"`](https://pypi.org/project/solara-ui)
-  * [`pip install "solara-server[starlette,dev]"`](https://pypi.org/project/solara-ui) -
+  * [`pip install "solara-server[starlette,dev]"`](https://pypi.org/project/solara-ui)
 
 Note that the solara (meta) package will pin exact versions of solara-ui and solara-server, which ensures you always get compatible version of the subpackages.
 For more flexibility, and control over what you install, you can install the subpackages directly.
 
 
 ### The `solara-ui` package
 
@@ -121,14 +121,14 @@
 
 
 
 
 ### The `pytest-ipywidgets` package
 
 This package is a plugin for pytest that lets you test ipywidgets with playwright. It is useful for testing your ipywidgets or solara applications in a (headless) browser.
-See [Our testing documentation](https://solara.dev/docs/advanced/testing) for more information.
+See [Our testing documentation](https://solara.dev/documentation/advanced/howto/testing) for more information.
 
  * `pip install "pytest-ipywidgets"` - Minimal installation for testing ipywidgets.
  * `pip install "pytest-ipywidgets[voila]"` - The above, with a compatible version of voila.
  * `pip install "pytest-ipywidgets[jupyterlab]"` - The above, with a compatible version of jupyterlab.
  * `pip install "pytest-ipywidgets[notebook]"` - The above, with a compatible version of notebook.
  * `pip install "pytest-ipywidgets[all]"` - Installs all optional dependencies.
```

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/90-troubleshoot.md` & `solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/90-troubleshoot.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/04-tutorials/00-overview.md` & `solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/04-tutorials/00-overview.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/04-tutorials/20-web-app.md` & `solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/04-tutorials/20-web-app.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/04-tutorials/30-ipywidgets.md` & `solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/04-tutorials/30-ipywidgets.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/04-tutorials/40-streamlit.md` & `solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/04-tutorials/40-streamlit.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/04-tutorials/50-dash.md` & `solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/04-tutorials/50-dash.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/04-tutorials/60-jupyter-dashboard-part1.py` & `solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/04-tutorials/60-jupyter-dashboard-part1.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/04-tutorials/SF_crime_sample.csv.gz` & `solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/04-tutorials/SF_crime_sample.csv.gz`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/04-tutorials/_data_science.ipynb` & `solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/04-tutorials/_data_science.ipynb`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/04-tutorials/_jupyter_dashboard_1.ipynb` & `solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/04-tutorials/_jupyter_dashboard_1.ipynb`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/05-fundamentals/10-components.md` & `solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/05-fundamentals/10-components.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/05-fundamentals/50-state-management.md` & `solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/05-fundamentals/50-state-management.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/07-deploying/10-self-hosted.md` & `solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/07-deploying/10-self-hosted.md`

 * *Files 4% similar despite different names*

```diff
@@ -222,39 +222,55 @@
 If you use Nginx as a (reverse) proxy in front of your Python web server, a minimal
 configuration would be:
 
 ```
 server {
     server_name widgetti.io;
     listen 80
-    location /solara/ {
+    location / {
             # the local solara server (could be using Starlette/uvicorn)
             proxy_pass http://localhost:8765/;
 
             proxy_set_header Host $host;
             proxy_set_header X-Real-IP $remote_addr;
             proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
-            proxy_set_header X-Script-Name /solara;  # informs solara to produce correct urls
+            proxy_set_header X-Forwarded-Proto $scheme;
 
             proxy_http_version 1.1;
             proxy_set_header Upgrade $http_upgrade;
             proxy_set_header Connection "upgrade";
             proxy_read_timeout 86400;
     }
+
+    # If you do not host solara on the root path, you can use the following
+    # location /solara/ {
+    #        ...
+    #        proxy_set_header X-Script-Name /solara;  # informs solara to produce correct urls
+    #        ...
+    # }
 }
 ```
 
-Note that if we use `location /` instead of `location /solara/`, we can skip the `proxy_set_header X-Script-Name /solara` line.
-
 An alternative to using the `X-Script-Name` header with uvicorn, would be to pass the `--root-path` flag, e.g.:
 
 ```
 $ SOLARA_APP=sol.py uvicorn --workers 1 --root-path /solara -b 0.0.0.0:8765 solara.server.flask:app
 ```
 
+In the case of an [OAuth setup](https://solara.dev/documentation/advanced/enterprise/oauth) it is important to make sure that the `X-Forwarded-Proto` and `Host` headers are forwarded correctly.
+If you are running uvicorn (the default if you use `solara run ...`) you will need to configure uvicorn to accept these headers using e.g.:
+
+```bash
+export UVICORN_PROXY_HEADERS=1
+export FORWARDED_ALLOW_IPS = "127.0.0.1"  # If your solara-server can *only* be reached by the proxy, you can set it to "*", otherwise put in the IP of the reverse proxy
+```
+
+Make sure you replace the IP with the correct IP of the reverse proxy server (instead of `127.0.0.1`). If you are sure that only the reverse proxy can reach the solara server, you can consider
+setting `FORWARDED_ALLOW_IPS="*"`.
+
 ## Docker
 
 There is nothing special about running Solara in Docker. The only things you probably need to change is the interface the server binds to.
 Solara by default binds to localhost, so that it is not accessible from the outside world. Apart from that localhost (or `::1` in case of IPv6)
 might not be available, you probably want the outside world to see your Solara app. For that, you can use `--host=0.0.0.0` or `--host=::` option to bind to all interfaces.
 
 Your Dockerfile could look like:
```

### Comparing `solara_ui-1.31.0/solara/website/pages/documentation/getting_started/content/07-deploying/20-cloud-hosted.md` & `solara_ui-1.32.0/solara/website/pages/documentation/getting_started/content/07-deploying/20-cloud-hosted.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/showcase/__init__.py` & `solara_ui-1.32.0/solara/website/pages/showcase/__init__.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/showcase/domino_code_assist.py` & `solara_ui-1.32.0/solara/website/pages/showcase/domino_code_assist.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/showcase/planeto_tessa.py` & `solara_ui-1.32.0/solara/website/pages/showcase/planeto_tessa.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/showcase/solara_dev.py` & `solara_ui-1.32.0/solara/website/pages/showcase/solara_dev.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/showcase/solarathon_2023_team_2.py` & `solara_ui-1.32.0/solara/website/pages/showcase/solarathon_2023_team_2.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/showcase/solarathon_2023_team_4.py` & `solara_ui-1.32.0/solara/website/pages/showcase/solarathon_2023_team_4.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/showcase/solarathon_2023_team_5.py` & `solara_ui-1.32.0/solara/website/pages/showcase/solarathon_2023_team_5.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/showcase/solarathon_2023_team_6.py` & `solara_ui-1.32.0/solara/website/pages/showcase/solarathon_2023_team_6.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/pages/showcase/wanderlust.py` & `solara_ui-1.32.0/solara/website/pages/showcase/wanderlust.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/public/beach.jpeg` & `solara_ui-1.32.0/solara/website/public/beach.jpeg`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/public/logo.svg` & `solara_ui-1.32.0/solara/website/public/logo.svg`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/public/success.html` & `solara_ui-1.32.0/solara/website/public/success.html`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/public/social/discord.svg` & `solara_ui-1.32.0/solara/website/public/social/discord.svg`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/public/social/github.svg` & `solara_ui-1.32.0/solara/website/public/social/github.svg`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/website/templates/index.html.j2` & `solara_ui-1.32.0/solara/website/templates/index.html.j2`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/widgets/widgets.py` & `solara_ui-1.32.0/solara/widgets/widgets.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/widgets/vue/gridlayout.vue` & `solara_ui-1.32.0/solara/widgets/vue/gridlayout.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/widgets/vue/navigator.vue` & `solara_ui-1.32.0/solara/widgets/vue/navigator.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/solara/widgets/vue/vegalite.vue` & `solara_ui-1.32.0/solara/widgets/vue/vegalite.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/conftest.py` & `solara_ui-1.32.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/integration/api_test.py` & `solara_ui-1.32.0/tests/integration/api_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/integration/async_test.py` & `solara_ui-1.32.0/tests/integration/async_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/integration/cdn_test.py` & `solara_ui-1.32.0/tests/integration/cdn_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/integration/cmdline_test.py` & `solara_ui-1.32.0/tests/integration/cmdline_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/integration/conftest.py` & `solara_ui-1.32.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/integration/create_test.py` & `solara_ui-1.32.0/tests/integration/create_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/integration/esm_test.py` & `solara_ui-1.32.0/tests/integration/esm_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/integration/file_download_test.py` & `solara_ui-1.32.0/tests/integration/file_download_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/integration/flask_test.py` & `solara_ui-1.32.0/tests/integration/flask_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/integration/input_date_test.py` & `solara_ui-1.32.0/tests/integration/input_date_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/integration/latex_test.py` & `solara_ui-1.32.0/tests/integration/latex_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/integration/markdown_test.py` & `solara_ui-1.32.0/tests/integration/markdown_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/integration/menu_test.py` & `solara_ui-1.32.0/tests/integration/menu_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/integration/popout_test.py` & `solara_ui-1.32.0/tests/integration/popout_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/integration/reconnect_test.py` & `solara_ui-1.32.0/tests/integration/reconnect_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/integration/router_test.py` & `solara_ui-1.32.0/tests/integration/router_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/integration/server_test.py` & `solara_ui-1.32.0/tests/integration/server_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/integration/ssg_test.py` & `solara_ui-1.32.0/tests/integration/ssg_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/integration/starlette_test.py` & `solara_ui-1.32.0/tests/integration/starlette_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/integration/testapp.py` & `solara_ui-1.32.0/tests/integration/testapp.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/integration/widget_test.py` & `solara_ui-1.32.0/tests/integration/widget_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/integration/enterprise/oauth_test.py` & `solara_ui-1.32.0/tests/integration/enterprise/oauth_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/ui/snapshots/tests/integration/latex_test.py/test_widget_latex_solara-flask-chromium-linux-ipywidgets-7-reference.png` & `solara_ui-1.32.0/tests/ui/snapshots/tests/integration/latex_test.py/test_widget_latex_solara-flask-chromium-linux-ipywidgets-7-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/ui/snapshots/tests/integration/latex_test.py/test_widget_latex_solara-flask-chromium-linux-ipywidgets-8-reference.png` & `solara_ui-1.32.0/tests/ui/snapshots/tests/integration/latex_test.py/test_widget_latex_solara-flask-chromium-linux-ipywidgets-8-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_lab-chromium-linux-ipywidgets-7-reference.png` & `solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_lab-chromium-linux-ipywidgets-7-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_lab-chromium-linux-ipywidgets-8-reference.png` & `solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_lab-chromium-linux-ipywidgets-8-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_notebook-chromium-linux-ipywidgets-7-reference.png` & `solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_notebook-chromium-linux-ipywidgets-7-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_notebook-chromium-linux-ipywidgets-8-reference.png` & `solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_notebook-chromium-linux-ipywidgets-8-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-solara-chromium-linux-ipywidgets-7-reference.png` & `solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-solara-chromium-linux-ipywidgets-7-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-solara-chromium-linux-ipywidgets-8-reference.png` & `solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-solara-chromium-linux-ipywidgets-8-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-voila-chromium-linux-ipywidgets-7-reference.png` & `solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-voila-chromium-linux-ipywidgets-7-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-starlette-solara-chromium-linux-ipywidgets-7-reference.png` & `solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-starlette-solara-chromium-linux-ipywidgets-7-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-starlette-solara-chromium-linux-ipywidgets-8-reference.png` & `solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-starlette-solara-chromium-linux-ipywidgets-8-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-jupyter_lab-chromium-linux-reference.png` & `solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-jupyter_lab-chromium-linux-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-jupyter_notebook-chromium-linux-reference.png` & `solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-jupyter_notebook-chromium-linux-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-solara-chromium-linux-reference.png` & `solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-solara-chromium-linux-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-voila-chromium-linux-reference.png` & `solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-voila-chromium-linux-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-starlette-solara-chromium-linux-reference.png` & `solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-starlette-solara-chromium-linux-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-flask-chromium-linux-ipyvuetify3-reference.png` & `solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-flask-chromium-linux-ipyvuetify3-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-flask-chromium-linux-reference.png` & `solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-flask-chromium-linux-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-starlette-chromium-linux-ipyvuetify3-reference.png` & `solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-starlette-chromium-linux-ipyvuetify3-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-starlette-chromium-linux-reference.png` & `solara_ui-1.32.0/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-starlette-chromium-linux-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/app_test.py` & `solara_ui-1.32.0/tests/unit/app_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/applayout_test.py` & `solara_ui-1.32.0/tests/unit/applayout_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/autorouting_test.py` & `solara_ui-1.32.0/tests/unit/autorouting_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/cache_test.py` & `solara_ui-1.32.0/tests/unit/cache_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/cdn_helper_test.py` & `solara_ui-1.32.0/tests/unit/cdn_helper_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/chat_test.py` & `solara_ui-1.32.0/tests/unit/chat_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/checkbox_test.py` & `solara_ui-1.32.0/tests/unit/checkbox_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/common.py` & `solara_ui-1.32.0/tests/unit/common.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/component_frontend_test.py` & `solara_ui-1.32.0/tests/unit/component_frontend_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/confirmation_dialog_test.py` & `solara_ui-1.32.0/tests/unit/confirmation_dialog_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/conftest.py` & `solara_ui-1.32.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/cross_filter_component_test.py` & `solara_ui-1.32.0/tests/unit/cross_filter_component_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/cross_filter_test.py` & `solara_ui-1.32.0/tests/unit/cross_filter_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/dataframe_test.py` & `solara_ui-1.32.0/tests/unit/dataframe_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/datatable_test.py` & `solara_ui-1.32.0/tests/unit/datatable_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/display_test.py` & `solara_ui-1.32.0/tests/unit/display_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/express_test.py` & `solara_ui-1.32.0/tests/unit/express_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/file_browser_test.py` & `solara_ui-1.32.0/tests/unit/file_browser_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         return solara.FileBrowser(HERE.parent.parent, filter=directory_filter)
 
     div, rc = solara.render_fixed(Test())
 
     list: solara.components.file_browser.FileListWidget = div.children[1]
     items = list.files
     names = {k["name"] for k in items}
-    assert names == {"unit", "ui", "integration", ".."}
+    assert names == {"unit", "ui", "docs", "integration", ".."}
 
 
 def test_file_browser_test_change_directory():
     div, rc = solara.render_fixed(solara.FileBrowser(HERE.parent))
     list: solara.components.file_browser.FileListWidget = div.children[1]
     assert "file_browser_test.py" in list
     rc.render(solara.FileBrowser(HERE.parent.parent))
@@ -208,15 +208,15 @@
 
     _, rc = solara.render(Page(), handle_error=False)
     file_list = rc.find(solara.components.file_browser.FileListWidget).widget
     mock = unittest.mock.MagicMock()
     file_list.observe(mock, "files")
     items = file_list.files
     names = {k["name"] for k in items}
-    assert names == {"unit", "ui", "integration", ".."}
+    assert names == {"unit", "ui", "docs", "integration", ".."}
     file_list.test_click("..")
     assert mock.call_count == 0
     file_list.test_click("integration")
     items = file_list.files
     names = {k["name"] for k in items}
-    assert names != {"unit", "ui", "integration", ".."}
+    assert names != {"unit", "ui", "docs", "integration", ".."}
     assert mock.call_count == 1
```

### Comparing `solara_ui-1.31.0/tests/unit/file_download_test.py` & `solara_ui-1.32.0/tests/unit/file_download_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/hooks_test.py` & `solara_ui-1.32.0/tests/unit/hooks_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/input_date_test.py` & `solara_ui-1.32.0/tests/unit/input_date_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/input_test.py` & `solara_ui-1.32.0/tests/unit/input_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/kernel_test.py` & `solara_ui-1.32.0/tests/unit/kernel_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/lifecycle_test.py` & `solara_ui-1.32.0/tests/unit/lifecycle_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,28 +80,29 @@
         assert context.closed_event.is_set()
 
 
 @pytest.mark.parametrize("close_first", [True, False])
 async def test_kernel_lifecycle_close_while_disconnected(close_first, short_cull_timeout):
     # a reconnect should be possible within the reconnect window
     websocket = Mock()
-    context = kernel_context.initialize_virtual_kernel("session-id-1", "kernel-id-1", websocket)
+    context = kernel_context.initialize_virtual_kernel(f"session-id-1-{close_first}", f"kernel-id-1-{close_first}", websocket)
     context.page_connect("page-id-1")
     cull_task_1 = context.page_disconnect("page-id-1")
     await asyncio.sleep(0.1)
     # after 0.1 we connect again, but close it directly
     context.page_connect("page-id-2")
     if close_first:
-        context.page_close("page-id-2")
+        cull_task_2 = context.page_close("page-id-2")
         await asyncio.sleep(0.01)
-        cull_task_2 = context.page_disconnect("page-id-2")
+        context.page_disconnect("page-id-2")
     else:
-        cull_task_2 = context.page_disconnect("page-id-2")
+        context.page_disconnect("page-id-2")
         await asyncio.sleep(0.01)
-        context.page_close("page-id-2")
+        cull_task_2 = context.page_close("page-id-2")
+    assert cull_task_2 is not None
     assert not context.closed_event.is_set()
     await asyncio.sleep(0.15)
     # but even though we closed, the first page is still in the disconnected state
     with pytest.raises(asyncio.CancelledError):
         await cull_task_1
     assert not context.closed_event.is_set()
     await cull_task_2
```

### Comparing `solara_ui-1.31.0/tests/unit/matplotlib_test.py` & `solara_ui-1.32.0/tests/unit/matplotlib_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/output_widget_test.py` & `solara_ui-1.32.0/tests/unit/output_widget_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/patch_test.py` & `solara_ui-1.32.0/tests/unit/patch_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/pivottable_test.py` & `solara_ui-1.32.0/tests/unit/pivottable_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/reload_test.py` & `solara_ui-1.32.0/tests/unit/reload_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/router_test.py` & `solara_ui-1.32.0/tests/unit/router_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/select_test.py` & `solara_ui-1.32.0/tests/unit/select_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/settings_test.py` & `solara_ui-1.32.0/tests/unit/settings_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/shell_test.py` & `solara_ui-1.32.0/tests/unit/shell_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/slider_test.py` & `solara_ui-1.32.0/tests/unit/slider_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/tabs_test.py` & `solara_ui-1.32.0/tests/unit/tabs_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/task_test.py` & `solara_ui-1.32.0/tests/unit/task_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,19 @@
             solara.Info("Cancelled")
         elif square.not_called:
             solara.Info("Not called yet")
         else:
             raise RuntimeError("should not happen")
 
 
+def test_task_key():
+    assert "something" in something._result._storage.storage_key  # type: ignore
+    assert "something" in something._instance._storage.storage_key  # type: ignore
+
+
 def test_task_basic():
     results = []
 
     def collect():
         results.append((square._result.value._state, square.latest))
 
     box, rc = solara.render(SquareButton(3, on_render=collect), handle_error=False)
```

### Comparing `solara_ui-1.31.0/tests/unit/telemetry_tests.py` & `solara_ui-1.32.0/tests/unit/telemetry_tests.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/toestand_test.py` & `solara_ui-1.32.0/tests/unit/toestand_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1200,7 +1200,36 @@
             text = rc.find(v.TextField)
             assert text.widget.v_model == "3.0"
             assert route.module is not module
             route.module.value_reactive.value = 3  # type: ignore
             assert text.widget.v_model == "4.0"
     finally:
         app.close()
+
+
+def test_pydantic_basic():
+    from pydantic import BaseModel
+
+    class Person(BaseModel):
+        name: str
+        height: float
+
+    person = Reactive[Person](Person(name="Jos", height=1.8))
+    assert person.get() == Person(name="Jos", height=1.8)
+    assert person.get().name == "Jos"
+    assert person.get().height == 1.8
+    assert Ref(person.fields.name).get() == "Jos"
+    assert Ref(person.fields.height).get() == 1.8
+
+    person.set(Person(name="Maria", height=1.7))
+    assert person.get() == Person(name="Maria", height=1.7)
+    assert person.get().name == "Maria"
+    assert person.get().height == 1.7
+    assert Ref(person.fields.name).get() == "Maria"
+    assert Ref(person.fields.height).get() == 1.7
+
+    Ref(person.fields.height).set(2.0)
+    assert person.get() == Person(name="Maria", height=2.0)
+    assert person.get().name == "Maria"
+    assert person.get().height == 2.0
+    assert Ref(person.fields.name).get() == "Maria"
+    assert Ref(person.fields.height).get() == 2.0
```

### Comparing `solara_ui-1.31.0/tests/unit/toggle_button_test.py` & `solara_ui-1.32.0/tests/unit/toggle_button_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/solara_test_apps/notebookapp_component.ipynb` & `solara_ui-1.32.0/tests/unit/solara_test_apps/notebookapp_component.ipynb`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/solara_test_apps/notebookapp_element.ipynb` & `solara_ui-1.32.0/tests/unit/solara_test_apps/notebookapp_element.ipynb`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/solara_test_apps/notebookapp_widget.ipynb` & `solara_ui-1.32.0/tests/unit/solara_test_apps/notebookapp_widget.ipynb`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/solara_test_apps/multipage/03-some-markdown.md` & `solara_ui-1.32.0/tests/unit/solara_test_apps/multipage/03-some-markdown.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/tests/unit/solara_test_apps/multipage-widgets/04-color.ipynb` & `solara_ui-1.32.0/tests/unit/solara_test_apps/multipage-widgets/04-color.ipynb`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/.gitignore` & `solara_ui-1.32.0/.gitignore`

 * *Files 15% similar despite different names*

```diff
@@ -78,12 +78,12 @@
 
 # output file from the docs
 build/
 
 ./tmp
 ./examples
 node_modules
-packages/assets/cdn
-packages/assets/dist/*
+packages/solara-assets/cdn
+packages/solara-assets/dist/*
 
 solara-env
 states
```

### Comparing `solara_ui-1.31.0/LICENSE` & `solara_ui-1.32.0/LICENSE`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/README.md` & `solara_ui-1.32.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -96,11 +96,11 @@
 
 ![jupyter](https://global.discourse-cdn.com/standard11/uploads/jupyter/original/2X/8/8bc875c0c3845ae077168575a4f8a49cf1b35bc6.gif)
 
 ## Resources
 
 Visit our main website or jump directly to the introduction
 
-[![Introduction](https://dabuttonfactory.com/button.png?t=Introduction&f=Open+Sans-Bold&ts=20&tc=fff&hp=45&vp=12&c=8&bgt=unicolored&bgc=f19f41)](https://solara.dev/documentation)
+[![Introduction](https://dabuttonfactory.com/button.png?t=Introduction&f=Open+Sans-Bold&ts=20&tc=fff&hp=45&vp=12&c=8&bgt=unicolored&bgc=f19f41)](https://solara.dev/documentation/getting_started/introduction)
 [![Quickstart](https://dabuttonfactory.com/button.png?t=Quickstart&f=Open+Sans-Bold&ts=20&tc=fff&hp=45&vp=12&c=8&bgt=unicolored&bgc=f19f41)](https://solara.dev/documentation/getting_started)
 
 *Note that the solara.dev website is created using Solara*
```

### Comparing `solara_ui-1.31.0/pyproject.toml` & `solara_ui-1.32.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `solara_ui-1.31.0/PKG-INFO` & `solara_ui-1.32.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: solara-ui
-Version: 1.31.0
+Version: 1.32.0
 Dynamic: Summary
 Project-URL: Home, https://www.github.com/widgetti/solara
 Project-URL: Documentation, https://solara.dev
 Author-email: "Maarten A. Breddels" <maartenbreddels@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2022 Maarten A. Breddels
@@ -148,11 +148,11 @@
 
 ![jupyter](https://global.discourse-cdn.com/standard11/uploads/jupyter/original/2X/8/8bc875c0c3845ae077168575a4f8a49cf1b35bc6.gif)
 
 ## Resources
 
 Visit our main website or jump directly to the introduction
 
-[![Introduction](https://dabuttonfactory.com/button.png?t=Introduction&f=Open+Sans-Bold&ts=20&tc=fff&hp=45&vp=12&c=8&bgt=unicolored&bgc=f19f41)](https://solara.dev/documentation)
+[![Introduction](https://dabuttonfactory.com/button.png?t=Introduction&f=Open+Sans-Bold&ts=20&tc=fff&hp=45&vp=12&c=8&bgt=unicolored&bgc=f19f41)](https://solara.dev/documentation/getting_started/introduction)
 [![Quickstart](https://dabuttonfactory.com/button.png?t=Quickstart&f=Open+Sans-Bold&ts=20&tc=fff&hp=45&vp=12&c=8&bgt=unicolored&bgc=f19f41)](https://solara.dev/documentation/getting_started)
 
 *Note that the solara.dev website is created using Solara*
```


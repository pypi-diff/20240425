# Comparing `tmp/pyodide_mkdocs_theme-0.3.2.tar.gz` & `tmp/pyodide_mkdocs_theme-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide_mkdocs_theme-0.3.2.tar", max compression
+gzip compressed data, was "pyodide_mkdocs_theme-0.3.3.tar", max compression
```

## Comparing `pyodide_mkdocs_theme-0.3.2.tar` & `pyodide_mkdocs_theme-0.3.3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-0.3.2/LICENSE
--rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-0.3.2/README.md
--rw-r--r--   0        0        0     1347 2024-04-24 20:07:39.566584 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/__init__.py
--rw-r--r--   0        0        0     2160 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/__main__.py
--rw-r--r--   0        0        0       22 2024-04-24 20:07:39.602585 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/__version__.py
--rw-r--r--   0        0        0      807 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/__init__.py
--rw-r--r--   0        0        0     1178 2024-04-24 20:07:39.554583 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/deprecation.py
--rw-r--r--   0        0        0      856 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
--rw-r--r--   0        0        0     1190 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
--rw-r--r--   0        0        0     4974 2024-04-11 09:41:00.019938 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
--rw-r--r--   0        0        0     4991 2024-04-24 20:05:58.907628 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py
--rw-r--r--   0        0        0    21241 2024-04-24 20:05:58.907628 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py
--rw-r--r--   0        0        0    14750 2024-04-24 20:05:58.907628 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py
--rw-r--r--   0        0        0      689 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
--rw-r--r--   0        0        0     6073 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
--rw-r--r--   0        0        0     4093 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
--rw-r--r--   0        0        0    11548 2024-04-24 20:05:58.907628 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
--rw-r--r--   0        0        0    13167 2024-04-18 21:29:06.622893 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/messages.py
--rw-r--r--   0        0        0     6945 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
--rw-r--r--   0        0        0     4237 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/parsing.py
--rw-r--r--   0        0        0     4462 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
--rw-r--r--   0        0        0    11593 2024-04-19 07:02:56.611776 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
--rw-r--r--   0        0        0    11690 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
--rw-r--r--   0        0        0    13035 2024-04-24 20:05:58.907628 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py
--rw-r--r--   0        0        0     1711 2024-04-24 20:05:58.907628 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
--rw-r--r--   0        0        0     2877 2024-04-19 06:57:28.632698 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
--rw-r--r--   0        0        0     9974 2024-04-14 21:38:49.051576 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
--rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
--rw-r--r--   0        0        0     1064 2024-04-24 20:07:39.558584 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
--rw-r--r--   0        0        0     6881 2024-04-19 06:57:41.645164 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
--rw-r--r--   0        0        0      690 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/scripts/__init__.py
--rw-r--r--   0        0        0     1001 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/scripts/custom_lang.py
--rw-r--r--   0        0        0     3983 2024-04-24 20:07:39.566584 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/scripts/custom_lang_src.py
--rw-r--r--   0        0        0     5490 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/__init__.py
--rw-r--r--   0        0        0     4510 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
--rw-r--r--   0        0        0     7349 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
--rw-r--r--   0        0        0     1675 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
--rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
--rw-r--r--   0        0        0     4320 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js
--rw-r--r--   0        0        0     3629 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
--rw-r--r--   0        0        0     1078 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css
--rw-r--r--   0        0        0     6426 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/main.html
--rw-r--r--   0        0        0     1924 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
--rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/partials/copyright.html
--rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/partials/footer.html
--rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/partials/social.html
--rw-r--r--   0        0        0     9780 2024-04-24 20:05:58.907628 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js
--rw-r--r--   0        0        0     5935 2024-04-04 09:56:58.174965 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js
--rw-r--r--   0        0        0     3459 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css
--rw-r--r--   0        0        0     1645 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png
--rw-r--r--   0        0        0     1328 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png
--rw-r--r--   0        0        0     1761 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png
--rw-r--r--   0        0        0     1283 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png
--rw-r--r--   0        0        0      952 2024-03-05 12:41:09.857670 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png
--rw-r--r--   0        0        0     1296 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png
--rw-r--r--   0        0        0     1702 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js
--rw-r--r--   0        0        0      823 2024-03-04 14:13:04.212401 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md
--rw-r--r--   0        0        0     6600 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js
--rw-r--r--   0        0        0    16559 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js
--rw-r--r--   0        0        0     9657 2024-04-04 09:56:58.138964 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js
--rw-r--r--   0        0        0      252 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/README.md
--rw-r--r--   0        0        0     1947 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css
--rw-r--r--   0        0        0     9150 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js
--rw-r--r--   0        0        0     3629 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css
--rw-r--r--   0        0        0     1651 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css
--rw-r--r--   0        0        0     5373 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js
--rw-r--r--   0        0        0     4218 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js
--rw-r--r--   0        0        0     1478 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js
--rw-r--r--   0        0        0     2857 2024-03-25 22:17:16.937424 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg
--rw-r--r--   0        0        0     3774 2024-04-14 12:10:19.820826 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css
--rw-r--r--   0        0        0    12716 2024-04-14 21:38:49.051576 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js
--rw-r--r--   0        0        0     1775 2024-04-24 20:07:36.178484 pyodide_mkdocs_theme-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-0.3.3/LICENSE
+-rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-0.3.3/README.md
+-rw-r--r--   0        0        0     1347 2024-04-24 20:11:45.697785 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/__init__.py
+-rw-r--r--   0        0        0     2160 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/__main__.py
+-rw-r--r--   0        0        0       22 2024-04-24 20:11:45.733786 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/__version__.py
+-rw-r--r--   0        0        0      807 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/__init__.py
+-rw-r--r--   0        0        0     1178 2024-04-24 20:11:45.689784 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/deprecation.py
+-rw-r--r--   0        0        0      856 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
+-rw-r--r--   0        0        0     1190 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
+-rw-r--r--   0        0        0     4974 2024-04-11 09:41:00.019938 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
+-rw-r--r--   0        0        0     4967 2024-04-24 20:10:35.611737 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py
+-rw-r--r--   0        0        0    21205 2024-04-24 20:10:35.611737 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py
+-rw-r--r--   0        0        0    14716 2024-04-24 20:10:35.615738 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py
+-rw-r--r--   0        0        0      689 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
+-rw-r--r--   0        0        0     6073 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
+-rw-r--r--   0        0        0     4093 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
+-rw-r--r--   0        0        0    11589 2024-04-24 20:10:35.615738 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
+-rw-r--r--   0        0        0    13167 2024-04-18 21:29:06.622893 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/messages.py
+-rw-r--r--   0        0        0     6945 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
+-rw-r--r--   0        0        0     4237 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/parsing.py
+-rw-r--r--   0        0        0     4462 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
+-rw-r--r--   0        0        0    11593 2024-04-19 07:02:56.611776 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
+-rw-r--r--   0        0        0    11690 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
+-rw-r--r--   0        0        0    13032 2024-04-24 20:10:35.615738 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py
+-rw-r--r--   0        0        0     1614 2024-04-24 20:10:35.615738 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
+-rw-r--r--   0        0        0     2877 2024-04-19 06:57:28.632698 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
+-rw-r--r--   0        0        0     9974 2024-04-14 21:38:49.051576 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
+-rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
+-rw-r--r--   0        0        0     1064 2024-04-24 20:11:45.689784 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
+-rw-r--r--   0        0        0     6881 2024-04-19 06:57:41.645164 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
+-rw-r--r--   0        0        0      690 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/scripts/__init__.py
+-rw-r--r--   0        0        0     1001 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/scripts/custom_lang.py
+-rw-r--r--   0        0        0     3983 2024-04-24 20:11:45.697785 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/scripts/custom_lang_src.py
+-rw-r--r--   0        0        0     5490 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/__init__.py
+-rw-r--r--   0        0        0     4510 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
+-rw-r--r--   0        0        0     7349 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
+-rw-r--r--   0        0        0     1675 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
+-rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
+-rw-r--r--   0        0        0     4320 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js
+-rw-r--r--   0        0        0     3629 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
+-rw-r--r--   0        0        0     1078 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css
+-rw-r--r--   0        0        0     6426 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/main.html
+-rw-r--r--   0        0        0     1924 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
+-rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/partials/copyright.html
+-rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/partials/footer.html
+-rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/partials/social.html
+-rw-r--r--   0        0        0     9776 2024-04-24 20:10:35.615738 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js
+-rw-r--r--   0        0        0     5935 2024-04-04 09:56:58.174965 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js
+-rw-r--r--   0        0        0     3459 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css
+-rw-r--r--   0        0        0     1645 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png
+-rw-r--r--   0        0        0     1328 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png
+-rw-r--r--   0        0        0     1761 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png
+-rw-r--r--   0        0        0     1283 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png
+-rw-r--r--   0        0        0      952 2024-03-05 12:41:09.857670 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png
+-rw-r--r--   0        0        0     1296 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png
+-rw-r--r--   0        0        0     1702 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js
+-rw-r--r--   0        0        0      823 2024-03-04 14:13:04.212401 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md
+-rw-r--r--   0        0        0     6600 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js
+-rw-r--r--   0        0        0    16559 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js
+-rw-r--r--   0        0        0     9657 2024-04-04 09:56:58.138964 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js
+-rw-r--r--   0        0        0      252 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/README.md
+-rw-r--r--   0        0        0     1947 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css
+-rw-r--r--   0        0        0     9150 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js
+-rw-r--r--   0        0        0     3629 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css
+-rw-r--r--   0        0        0     1651 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css
+-rw-r--r--   0        0        0     5373 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js
+-rw-r--r--   0        0        0     4218 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js
+-rw-r--r--   0        0        0     1478 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js
+-rw-r--r--   0        0        0     2857 2024-03-25 22:17:16.937424 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg
+-rw-r--r--   0        0        0     3774 2024-04-14 12:10:19.820826 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css
+-rw-r--r--   0        0        0    12716 2024-04-14 21:38:49.051576 pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js
+-rw-r--r--   0        0        0     1775 2024-04-24 20:11:43.145710 pyodide_mkdocs_theme-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-0.3.3/PKG-INFO
```

### Comparing `pyodide_mkdocs_theme-0.3.2/LICENSE` & `pyodide_mkdocs_theme-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/README.md` & `pyodide_mkdocs_theme-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/__init__.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/__main__.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/__main__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/__init__.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/deprecation.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/deprecation.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/exceptions.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 
 
 
 
 def _IDE_maker(env:MaestroIDE, mode:str):
     """
-    @script_name: Partial path from the directory holding the sujet.md file, to the one holding
+    @py_name: Partial path from the directory holding the sujet.md file, to the one holding
                   all the other required files, ending with the common prefix for the exercice.
                   Ex:   "exo" to extract:   "exo.py", "exo_corr.py", "exo_test.py", ...
                       "sub_exA/exo" for:  "sub_exA/exo.py", "sub_exA/exo_corr.py", ...
     @MAX:         Number of tries before the solution becomes visible (default: validations config)
     @SANS:        String of spaces or coma separated python functions or modules/packages the
                   user cannot use. By default, nothing is forbidden.
                       - Every string section that matches a builtin callable forbid that function
@@ -60,26 +60,26 @@
                   `mkdocs.yml`, to determine what to do (default=None).
     @REC_LIMIT:   Setup a specific recursion limit value for the runtime (-1 if not used)
     @TERM_H:      Number of lines to use for the terminal size (ignored for vertical terminals)
     """
 
     @wraps(_IDE_maker)
     def wrapped(
-        script_name: str = "",
+        py_name: str = "",
         MAX: Optional[Union[int, Literal["+"]]] = None,
         SANS: str = "",
         MAX_SIZE: int = 30,
         ID: Optional[int] = None,
         WHITE: str = "",
         LOGS: Optional[bool] = None,
         REC_LIMIT: int = -1,
         TERM_H: int = 10,
     ) -> str:
         return Ide(
-            env, script_name, mode, MAX, SANS, MAX_SIZE, WHITE, ID, LOGS, REC_LIMIT, TERM_H
+            env, py_name, mode, MAX, SANS, MAX_SIZE, WHITE, ID, LOGS, REC_LIMIT, TERM_H
         ).make_ide()
 
     wrapped.__name__ = wrapped.__qualname__ = 'IDE' + mode.strip('_')
     return wrapped
 
 
 
@@ -103,19 +103,19 @@
     """
     Insert the given section from the python file.
     Note: To use only on python scripts holding all the sections for the IDE macros. For regular
           files, use the `py` macro or regular code fences with file inclusions (for performances
           reasons).
     """
     @wraps(section)
-    def _section(script_name:str, section_name:ScriptSection, ID:Optional[int]=None):
-        file_data = IdeFilesExtractor(env, script_name)
+    def _section(py_name:str, section_name:ScriptSection, ID:Optional[int]=None):
+        file_data = IdeFilesExtractor(env, py_name)
         content = file_data.get_section(section_name)
 
         id_pattern = "" if ID is None else rf",\s*ID\s*=\s*{ ID }\b\s*"
-        macro_pattern = rf"""['"]{ script_name }['"]\s*,\s*['"]{ section_name }['"]{ id_pattern }"""
+        macro_pattern = rf"""['"]{ py_name }['"]\s*,\s*['"]{ section_name }['"]{ id_pattern }"""
         ide_jinja_reg = re.compile( rf"section\(\s*{ macro_pattern }" )
         indent = env.get_indent_in_current_page(ide_jinja_reg)
         out = build_code_fence(content, indent, lang='python')
         return out
 
     return _section
```

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     # Defined on instantiation:
     #--------------------------
 
     my_env: MaestroIDE
     """ The MaestroEnv singleton """
 
-    script_name: str
+    py_name: str
     """ Base name for the files to use (first argument passed to the macros)
         Partial path from the directory holding the sujet.md file, to the one holding all the
         other required files, ending with the common prefix for the exercice.
         Ex:   "exo" to extract:   "exo.py", "exo_corr.py", "exo_test.py", ...
                 "sub_exA/exo" for:  "sub_exA/exo.py", "sub_exA/exo_corr.py", ...
     """
 
@@ -167,20 +167,20 @@
 
 
     def __post_init__(self):
 
         if self.max_attempts is None:
             self.max_attempts = self.my_env.max_attempts_before_corr_available
 
-        self.files_data = IdeFilesExtractor(self.my_env, self.script_name, self.id)
+        self.files_data = IdeFilesExtractor(self.my_env, self.py_name, self.id)
 
         if 0 <= self.rec_limit < self.my_env.MIN_RECURSION_LIMIT:
             with_id = f' (ID={ self.id })' if self.id is not None else ''
             raise BuildError(
-                f"The recursion limit for {self.my_env.page.file.src_uri}:{self.script_name}"
+                f"The recursion limit for {self.my_env.page.file.src_uri}:{self.py_name}"
                 f"{with_id} is set too low and may causes runtime troubles. Please set it to "
                 f"at least { self.my_env.MIN_RECURSION_LIMIT }."
             )
 
         if self.id is not None and not isinstance(self.id, int):
             raise BuildError(f'The ID argument should be an integer, but was: {self.id!r}')
 
@@ -203,15 +203,15 @@
         excluded_methods = [ meth for meth in excluded if meth.startswith('.') ]
         excluded = [ no_meth for no_meth in excluded if not no_meth.startswith('.') ]
 
 
         # Search the indentation level for the current IDE:
         is_v = self.mode.strip('_')
         quotes = """['"]"""
-        script_pattern = "" if not self.script_name else f"{quotes}{ self.script_name }{quotes}"
+        script_pattern = "" if not self.py_name else f"{quotes}{ self.py_name }{quotes}"
         id_pattern = r'(?!.*?ID\s*=)' if self.id is None else rf".*?ID\s*=\s*{ self.id }\b"
 
         ide_jinja_reg = re.compile( rf"IDE{ is_v }\(\s*{ script_pattern }{ id_pattern }" )
         self.indentation = self.my_env.get_indent_in_current_page(ide_jinja_reg)
 
 
 
@@ -279,15 +279,15 @@
         id_ide = hashlib.sha1(path.encode("utf-8")).hexdigest()
 
         if not self.my_env.register_if_unique(id_ide):
             raise BuildError(
                 "The same editor ID got generated twice. If you are trying to use the same set"
                 "of files for different IDEs, use the ID argument to disambiguate their id.\n"
                f"  Problematic file:  { py_path }\n"
-               f"  Possible solution: { '{{' } IDE(\"{ self.script_name }\", ID=2) { '}}' }"
+               f"  Possible solution: { '{{' } IDE(\"{ self.py_name }\", ID=2) { '}}' }"
             )
         return id_ide
 
 
 
     def _define_max_attempts_symbols_and_value(self):
         """
@@ -318,15 +318,15 @@
     #-----------------------------------------------------------------------------
 
 
 
 
     def make_ide(self) -> str:
         """
-        Create an IDE (Editor+Terminal) within an Mkdocs document. {script_name}.py is loaded on
+        Create an IDE (Editor+Terminal) within an Mkdocs document. {py_name}.py is loaded on
         the editor if present.
         NOTES:
             - Two modes are available : vertical or horizontal. Buttons are added through
                 functional calls.
             - The last span hides the code content of the IDE when loaded.
         """
         # Mark the page as needing this kind of scripts in the body section:
@@ -360,15 +360,15 @@
             kls = f'{HtmlClass.comment} {HtmlClass.tooltip}',
         )
         editor_div = Html.div(
             id = self.editor_name,
             is_v = str(is_v).lower(),
             mode = self.mode,
             max_size = self.max_size,
-            script_name = self.script_name,
+            py_name = self.py_name,
         )
         editor_wrapper = Html.div(
             editor_div + shortcut_comment_asserts,
             kls = Prefix.comment_ + HtmlClass.py_mk_wrapper
         )
 
         separator = Html.div(
```

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,28 +42,28 @@
 
 
 
 
 @dataclass
 class IdeFilesExtractor:
     """
-    ENTRY POINT: takes a script_name (IDE macro first argument) and extract from that all
+    ENTRY POINT: takes a py_name (IDE macro first argument) and extract from that all
     the necessary data from the different files.
-    With `script_name` being denoted X and F being the stem of the current md file, the
+    With `py_name` being denoted X and F being the stem of the current md file, the
     extracted files may be:
         1. X.py and X_REM.md, where the py file contains all the needed python code, separated
             by the pyodide python tokens: `# --- PYODIDE:{kind} --- #` or so
         2. X.py, X_text.py, X_corr.py and X_REM.md
         3. scripts/F/X.py, scripts/F/X_text.py, scripts/F/X_corr.py and scripts/F/X_REM.md
 
     The order gives the precedence. Way "1" is excluding the 2 others (except for the REM file)
     """
 
     env: MaestroIDE
-    script_name: str
+    py_name: str
     id: Optional[int] = None
 
     #-----------------------------
 
     exo_py: Optional[Path] = None
     """ Path to the master python file (if any) """
 
@@ -121,17 +121,17 @@
 
 
 
 
     def __post_init__(self):
 
         self.exo_py: Optional[Path] = self.get_path_for_exo('.py')
-        if not self.exo_py and self.script_name:
+        if not self.exo_py and self.py_name:
             raise BuildError(
-                f"No python script for { self.script_name }, in { self.env.page.file.src_uri }"
+                f"No python script for { self.py_name }, in { self.env.page.file.src_uri }"
             )
 
         script_content = read_file(self.exo_py) if self.exo_py  else ""
 
         # Extract everything:
         if self.SECTION_TOKEN.search(script_content):
             self.extract_multi_sections(script_content)
@@ -141,18 +141,18 @@
         self.corr_rem_bit_mask = self.has_corr + self.has_rem * 2
 
         # Sanity check:
         if not self.has_test and (self.has_corr or self.has_rem):
             opn,clos = '{{','}}'
             maybe_id = "" if self.id is None else f", ID={ self.id }"
             location = self.env.page.file.src_uri
-            test_file = self.script_name + SiblingFile.test
+            test_file = self.py_name + SiblingFile.test
             msg = (
                 f'An invalid configuration of files has been found for {opn} IDE("'
-                f'{self.script_name}"{ maybe_id }, ...) {clos} in the page { location }: '
+                f'{self.py_name}"{ maybe_id }, ...) {clos} in the page { location }: '
                 f'a correction or remark file exists but there is no { test_file } file.'
             )
             if self.env._dev_mode:
                 logger.error('EXPECTED (1x) - ' + msg)
             else:
                 raise BuildError(msg)
 
@@ -164,15 +164,15 @@
         # self._cleanup_tests()
 
 
 
     def get_path_for_exo(self, tail:str) -> Optional[Path] :
         """ Build a sibling path fro the current page/script """
         return get_sibling_of_current_page(
-            self.env, self.env.docs_dir_path, self.script_name, tail=tail
+            self.env, self.env.docs_dir_path, self.py_name, tail=tail
         )
 
 
 
     def get_path_and_existence(self, tail:str):
         """
         Return a pair (bool, Path|None), the boolean telling if some data actually exist for
@@ -204,15 +204,15 @@
     def extract_multi_sections(self, script_content:str):
         """
         Extract all the python content from one unique file with different sections:
             - HDR: header content (optional)
             - user: starting code for the user (optional)
             - corr: ... (optional - must be defined before the tests...?)
             - tests: public tests (optional)
-            - secret: secret tests (optional)
+            - secrets: secrets tests (optional)
         Note that the REM content has to stay in a markdown file, so that it can contain macros
         and mkdocs will still interpret those (if it were containing only markdown, it could be
         inserted on the fly by a macro, but an "inner macro call" would be ignored).
         """
 
         chunks = self.SECTION_TOKEN.split(script_content)
         chunks = [*filter(bool, map(str.strip, chunks))]
@@ -310,15 +310,15 @@
 
     def check_python(self):
         """
         * hdr + corr + public + secret => pass
         * hdr + user + public => doesn't pass
         * hdr + user + secret => doesn't pass
         """
-        if not self.script_name or self.id is not None:
+        if not self.py_name or self.id is not None:
             return # skip
 
         src    = self.get_path_for_exo('.py')
         target = Path('___XXX_check_python.py')
         target.touch(exist_ok=True)
 
         to_check = [
```

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,16 @@
 
 
         output = '\n'.join(admonition_lst)
         output = f'\n\n{ output }\n\n'    # Enforce empty spaces around in the markdown admonition
 
         if DEBUG:
             # The user doesn't need to know about the CORRECT_CLOSE_P thing, so remove them first:
-            print(output.replace(FIX_CLOSE_P, ''))
+            to_print = output.replace(FIX_CLOSE_P, '')
+            print(to_print)
         return output
 
     return wrapped
 
 
 
 
@@ -256,15 +257,15 @@
 
 
 
 
 def qcm_format(msg:str):
     """ Use the natural/minimal indentation and strip spaces on both ends """
     bare = dedent(msg).strip()
-    return bare
+    return f"{ bare }\n"
 
 
 
 
 
 #---------------------------------------------------------------------------------
```

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/messages.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/messages.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/parsing.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/parsing.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
 
     def warn_unmaintained(self, that:str):
         """
         Generic warning message for people trying to used untested/unmaintained macros.
         """
         deprecation_warning(
             f"{ that.capitalize() } has not been maintained since the original pyodide-mkdocs "
-            "project, may not currently work, and will be deprecated in the future.\n"
+            "project, may not currently work, and will be removed in the future.\n"
             "Please open an issue on the pyodide-mkdocs-theme repository, if you need it.\n\n"
             f"\t{ self.pmt_url }"
         )
```

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,18 +12,14 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
-
-"""
-Define a class the can be passed to all macro functions, holding all the necessary data
-"""
 # pylint: disable=multiple-statements
 
 
 from mkdocs.config.defaults import MkDocsConfig
 
 from ..tools_and_constants import Prefix
 from .maestro_base_and_indent import BaseMaestro
```

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/scripts/__init__.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/scripts/custom_lang.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/scripts/custom_lang.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/scripts/custom_lang_src.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/scripts/custom_lang_src.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/__init__.py` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/main.html` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/main.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/mkdocs_theme.yml` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/mkdocs_theme.yml`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/partials/copyright.html` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/partials/copyright.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/partials/footer.html` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/partials/footer.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/partials/social.html` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/partials/social.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -125,15 +125,15 @@
 /**Download the current content of the editor to the download folder of the user.
  * */
 const download = (editorName) => withPyodideAsyncLock(async function() {
     await waitForPyodideReady();
     jsLogger("[Download]")
 
     const editor = ace.edit(editorName)
-    const scriptName = editor.container.getAttribute('script_name')
+    const scriptName = editor.container.getAttribute('py_name')
     const fileName = _generateDownloadName(scriptName)
     let ideContent = editor.getValue() + "" // enforce stringification in any case
 
     let link = document.createElement("a");
     let blob = new Blob([ideContent], {
         type: "text/plain"
     });
```

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js` & `pyodide_mkdocs_theme-0.3.3/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.2/pyproject.toml` & `pyodide_mkdocs_theme-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyodide-mkdocs-theme"
-version = "0.3.2"
+version = "0.3.3"
 description = "Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations"
 authors = ["Frédéric Zinelli <frederic.zinelli@gmail.com>"]
 readme = "README.md"
 keywords = [
     "mkdocs", "mkdocs-plugin", "pyodide", "IDE", "terminal"
 ]
 classifiers = [
```

### Comparing `pyodide_mkdocs_theme-0.3.2/PKG-INFO` & `pyodide_mkdocs_theme-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-mkdocs-theme
-Version: 0.3.2
+Version: 0.3.3
 Summary: Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations
 Keywords: mkdocs,mkdocs-plugin,pyodide,IDE,terminal
 Author: Frédéric Zinelli
 Author-email: frederic.zinelli@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```


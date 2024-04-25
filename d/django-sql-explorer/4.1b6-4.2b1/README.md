# Comparing `tmp/django_sql_explorer-4.1b6.tar.gz` & `tmp/django_sql_explorer-4.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_sql_explorer-4.1b6.tar", last modified: Tue Apr 23 02:38:17 2024, max compression
+gzip compressed data, was "django_sql_explorer-4.2b1.tar", last modified: Thu Apr 25 21:16:35 2024, max compression
```

## Comparing `django_sql_explorer-4.1b6.tar` & `django_sql_explorer-4.2b1.tar`

### file list

```diff
@@ -1,158 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.521280 django_sql_explorer-4.1b6/
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-23 02:38:17.521280 django_sql_explorer-4.1b6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.521280 django_sql_explorer-4.1b6/django_sql_explorer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-23 02:38:17.000000 django_sql_explorer-4.1b6/django_sql_explorer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-23 02:38:17.000000 django_sql_explorer-4.1b6/django_sql_explorer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 02:38:17.000000 django_sql_explorer-4.1b6/django_sql_explorer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 02:38:17.000000 django_sql_explorer-4.1b6/django_sql_explorer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-23 02:38:17.000000 django_sql_explorer-4.1b6/django_sql_explorer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 02:38:17.000000 django_sql_explorer-4.1b6/django_sql_explorer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.501280 django_sql_explorer-4.1b6/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.501280 django_sql_explorer-4.1b6/explorer/assistant/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/assistant/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/assistant/prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/assistant/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/assistant/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/assistant/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/charts.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.497280 django_sql_explorer-4.1b6/explorer/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.497280 django_sql_explorer-4.1b6/explorer/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.501280 django_sql_explorer-4.1b6/explorer/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10091 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.497280 django_sql_explorer-4.1b6/explorer/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.505280 django_sql_explorer-4.1b6/explorer/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.505280 django_sql_explorer-4.1b6/explorer/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0002_auto_20150501_1515.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0003_query_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0004_querylog_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0005_auto_20160105_2052.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0006_query_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0007_querylog_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0008_auto_20190308_1642.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0009_auto_20201009_0547.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0010_sql_required.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0011_query_favorites.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0012_alter_queryfavorite_query_alter_queryfavorite_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0013_querylog_error_querylog_success.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0014_promptlog.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.497280 django_sql_explorer-4.1b6/explorer/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.509280 django_sql_explorer-4.1b6/explorer/src/js/
--rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/js/assistant.js
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/js/codemirror-config.js
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/js/csrf.js
--rw-r--r--   0 runner    (1001) docker     (127)    13023 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/js/explorer.js
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/js/favorites.js
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/js/main.js
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/js/pivot-setup.js
--rw-r--r--   0 runner    (1001) docker     (127)    77235 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/js/pivot.js
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/js/query-list.js
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/js/schema.js
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/js/table-to-csv.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.509280 django_sql_explorer-4.1b6/explorer/src/scss/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/scss/assistant.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/scss/explorer.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/scss/pivot.css
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/scss/styles.scss
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/scss/variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.497280 django_sql_explorer-4.1b6/explorer/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.509280 django_sql_explorer-4.1b6/explorer/static/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)   176088 2024-04-23 02:38:14.000000 django_sql_explorer-4.1b6/explorer/static/explorer/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)   130648 2024-04-23 02:38:14.000000 django_sql_explorer-4.1b6/explorer/static/explorer/bootstrap-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   546399 2024-04-23 02:38:14.000000 django_sql_explorer-4.1b6/explorer/static/explorer/explorer.js
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-23 02:38:14.000000 django_sql_explorer-4.1b6/explorer/static/explorer/favorites.js
--rw-r--r--   0 runner    (1001) docker     (127)    18658 2024-04-23 02:38:14.000000 django_sql_explorer-4.1b6/explorer/static/explorer/index.js
--rw-r--r--   0 runner    (1001) docker     (127)    84338 2024-04-23 02:38:14.000000 django_sql_explorer-4.1b6/explorer/static/explorer/main.js
--rw-r--r--   0 runner    (1001) docker     (127)    66999 2024-04-23 02:38:14.000000 django_sql_explorer-4.1b6/explorer/static/explorer/pivot-setup.js
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-23 02:38:14.000000 django_sql_explorer-4.1b6/explorer/static/explorer/query-list.js
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-23 02:38:14.000000 django_sql_explorer-4.1b6/explorer/static/explorer/schema.js
--rw-r--r--   0 runner    (1001) docker     (127)   308829 2024-04-23 02:38:14.000000 django_sql_explorer-4.1b6/explorer/static/explorer/styles.css
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.497280 django_sql_explorer-4.1b6/explorer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.513280 django_sql_explorer-4.1b6/explorer/templates/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/assistant.html
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/export_buttons.html
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/fullscreen.html
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/params.html
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/pdf_template.html
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/play.html
--rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/preview_pane.html
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/query.html
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/query_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/query_favorite_button.html
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/query_favorites.html
--rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/query_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/querylog_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/schema.html
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/schema_building.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.513280 django_sql_explorer-4.1b6/explorer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templatetags/explorer_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templatetags/vite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.517280 django_sql_explorer-4.1b6/explorer/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/test_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/test_csrf_cookie_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/test_exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/test_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    32207 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.517280 django_sql_explorer-4.1b6/explorer/views/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/download.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/email.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/export.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/format_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/query_favorite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.517280 django_sql_explorer-4.1b6/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/requirements/dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.521280 django_sql_explorer-4.1b6/requirements/extra/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/requirements/extra/assistant.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/requirements/extra/charts.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/requirements/extra/snapshots.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/requirements/extra/xls.txt
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-23 02:38:17.521280 django_sql_explorer-4.1b6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/vite.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.202532 django_sql_explorer-4.2b1/
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-25 21:16:35.202532 django_sql_explorer-4.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.202532 django_sql_explorer-4.2b1/django_sql_explorer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-25 21:16:35.000000 django_sql_explorer-4.2b1/django_sql_explorer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-04-25 21:16:35.000000 django_sql_explorer-4.2b1/django_sql_explorer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:16:35.000000 django_sql_explorer-4.2b1/django_sql_explorer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:16:34.000000 django_sql_explorer-4.2b1/django_sql_explorer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-25 21:16:35.000000 django_sql_explorer-4.2b1/django_sql_explorer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 21:16:35.000000 django_sql_explorer-4.2b1/django_sql_explorer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.178532 django_sql_explorer-4.2b1/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.182532 django_sql_explorer-4.2b1/explorer/assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/assistant/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/assistant/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/assistant/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/assistant/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/assistant/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.170532 django_sql_explorer-4.2b1/explorer/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.170532 django_sql_explorer-4.2b1/explorer/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.182532 django_sql_explorer-4.2b1/explorer/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10091 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.170532 django_sql_explorer-4.2b1/explorer/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.182532 django_sql_explorer-4.2b1/explorer/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.186532 django_sql_explorer-4.2b1/explorer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0002_auto_20150501_1515.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0003_query_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0004_querylog_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0005_auto_20160105_2052.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0006_query_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0007_querylog_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0008_auto_20190308_1642.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0009_auto_20201009_0547.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0010_sql_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0011_query_favorites.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0012_alter_queryfavorite_query_alter_queryfavorite_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0013_querylog_error_querylog_success.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0014_promptlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0015_explorervalue.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12467 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.174532 django_sql_explorer-4.2b1/explorer/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.186532 django_sql_explorer-4.2b1/explorer/src/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/js/assistant.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/js/codemirror-config.js
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/js/csrf.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13023 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/js/explorer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/js/favorites.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/js/pivot-setup.js
+-rw-r--r--   0 runner    (1001) docker     (127)    77235 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/js/pivot.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/js/query-list.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/js/schema.js
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/js/table-to-csv.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.186532 django_sql_explorer-4.2b1/explorer/src/scss/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/scss/assistant.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/scss/explorer.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/scss/pivot.css
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/scss/styles.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/scss/variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.174532 django_sql_explorer-4.2b1/explorer/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.190532 django_sql_explorer-4.2b1/explorer/static/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)   176088 2024-04-25 21:16:31.000000 django_sql_explorer-4.2b1/explorer/static/explorer/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   130648 2024-04-25 21:16:31.000000 django_sql_explorer-4.2b1/explorer/static/explorer/bootstrap-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   546527 2024-04-25 21:16:31.000000 django_sql_explorer-4.2b1/explorer/static/explorer/explorer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-25 21:16:31.000000 django_sql_explorer-4.2b1/explorer/static/explorer/favorites.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18658 2024-04-25 21:16:31.000000 django_sql_explorer-4.2b1/explorer/static/explorer/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)    84338 2024-04-25 21:16:31.000000 django_sql_explorer-4.2b1/explorer/static/explorer/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)    66999 2024-04-25 21:16:31.000000 django_sql_explorer-4.2b1/explorer/static/explorer/pivot-setup.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-25 21:16:31.000000 django_sql_explorer-4.2b1/explorer/static/explorer/query-list.js
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-25 21:16:31.000000 django_sql_explorer-4.2b1/explorer/static/explorer/schema.js
+-rw-r--r--   0 runner    (1001) docker     (127)   308829 2024-04-25 21:16:31.000000 django_sql_explorer-4.2b1/explorer/static/explorer/styles.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.174532 django_sql_explorer-4.2b1/explorer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.194532 django_sql_explorer-4.2b1/explorer/templates/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/assistant.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/export_buttons.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/fullscreen.html
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/params.html
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/pdf_template.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/play.html
+-rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/preview_pane.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/query.html
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/query_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/query_favorite_button.html
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/query_favorites.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/query_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/querylog_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/schema.html
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/schema_building.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.194532 django_sql_explorer-4.2b1/explorer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templatetags/explorer_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templatetags/vite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.198532 django_sql_explorer-4.2b1/explorer/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/test_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/test_csrf_cookie_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/test_exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/test_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32205 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.202532 django_sql_explorer-4.2b1/explorer/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/format_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/query_favorite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.202532 django_sql_explorer-4.2b1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/requirements/dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.202532 django_sql_explorer-4.2b1/requirements/extra/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/requirements/extra/assistant.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/requirements/extra/charts.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/requirements/extra/snapshots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/requirements/extra/xls.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-25 21:16:35.206532 django_sql_explorer-4.2b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/vite.config.js
```

### Comparing `django_sql_explorer-4.1b6/AUTHORS` & `django_sql_explorer-4.2b1/AUTHORS`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/LICENSE` & `django_sql_explorer-4.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/PKG-INFO` & `django_sql_explorer-4.2b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sql-explorer
-Version: 4.1b6
+Version: 4.2b1
 Summary: A pluggable app that allows users (admins) to execute SQL, view, and export the results.
 Home-page: https://www.sqlexplorer.io
 Author: Chris Clark
 Author-email: chris@untrod.com
 Maintainer: Mark Walker
 Maintainer-email: theshow@gmail.com
 License: MIT
```

### Comparing `django_sql_explorer-4.1b6/README.rst` & `django_sql_explorer-4.2b1/README.rst`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/django_sql_explorer.egg-info/PKG-INFO` & `django_sql_explorer-4.2b1/django_sql_explorer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sql-explorer
-Version: 4.1b6
+Version: 4.2b1
 Summary: A pluggable app that allows users (admins) to execute SQL, view, and export the results.
 Home-page: https://www.sqlexplorer.io
 Author: Chris Clark
 Author-email: chris@untrod.com
 Maintainer: Mark Walker
 Maintainer-email: theshow@gmail.com
 License: MIT
```

### Comparing `django_sql_explorer-4.1b6/django_sql_explorer.egg-info/SOURCES.txt` & `django_sql_explorer-4.2b1/django_sql_explorer.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 explorer/connections.py
 explorer/exporters.py
 explorer/forms.py
 explorer/models.py
 explorer/permissions.py
 explorer/schema.py
 explorer/tasks.py
-explorer/tracker.py
+explorer/telemetry.py
 explorer/urls.py
 explorer/utils.py
 explorer/assistant/__init__.py
 explorer/assistant/models.py
 explorer/assistant/prompts.py
 explorer/assistant/tests.py
 explorer/assistant/utils.py
@@ -48,14 +48,15 @@
 explorer/migrations/0008_auto_20190308_1642.py
 explorer/migrations/0009_auto_20201009_0547.py
 explorer/migrations/0010_sql_required.py
 explorer/migrations/0011_query_favorites.py
 explorer/migrations/0012_alter_queryfavorite_query_alter_queryfavorite_user.py
 explorer/migrations/0013_querylog_error_querylog_success.py
 explorer/migrations/0014_promptlog.py
+explorer/migrations/0015_explorervalue.py
 explorer/migrations/__init__.py
 explorer/src/js/assistant.js
 explorer/src/js/codemirror-config.js
 explorer/src/js/csrf.js
 explorer/src/js/explorer.js
 explorer/src/js/favorites.js
 explorer/src/js/main.js
@@ -105,15 +106,15 @@
 explorer/tests/test_apps.py
 explorer/tests/test_csrf_cookie_name.py
 explorer/tests/test_exporters.py
 explorer/tests/test_forms.py
 explorer/tests/test_models.py
 explorer/tests/test_schema.py
 explorer/tests/test_tasks.py
-explorer/tests/test_tracker.py
+explorer/tests/test_telemetry.py
 explorer/tests/test_utils.py
 explorer/tests/test_views.py
 explorer/views/__init__.py
 explorer/views/auth.py
 explorer/views/create.py
 explorer/views/delete.py
 explorer/views/download.py
```

### Comparing `django_sql_explorer-4.1b6/explorer/__init__.py` & `django_sql_explorer-4.2b1/explorer/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 __version_info__ = {
     "major": 4,
-    "minor": 1,
+    "minor": 2,
     "patch": 0,
     "releaselevel": "beta",
-    "serial": 6
+    "serial": 1
 }
 
 
 def get_version(short=False):
     assert __version_info__["releaselevel"] in ("alpha", "beta", "final")
     vers = ["%(major)i.%(minor)i" % __version_info__, ]
     if __version_info__["patch"]:
```

### Comparing `django_sql_explorer-4.1b6/explorer/actions.py` & `django_sql_explorer-4.2b1/explorer/actions.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,18 +29,19 @@
 
 
 def _package(queries):
     ret = {}
     is_one = len(queries) == 1
     name_root = lambda n: f"attachment; filename={n}"  # noqa
     ret["content_type"] = (is_one and "text/csv") or "application/zip"
-
+    formatted = queries[0].title.replace(",", "")
+    day = date.today()
     ret["filename"] = (
-        is_one and name_root("%s.csv" % queries[0].title.replace(",", ""))
-    ) or name_root("Report_%s.zip" % date.today())
+        is_one and name_root(f"{formatted}.csv")
+    ) or name_root(f"Report_{day}.zip")
 
     ret["data"] = (
         is_one and CSVExporter(queries[0]).get_output()
     ) or _build_zip(queries)
 
     ret["length"] = (is_one and len(ret["data"]) or ret["data"].blksize)
     return ret
```

### Comparing `django_sql_explorer-4.1b6/explorer/app_settings.py` & `django_sql_explorer-4.2b1/explorer/app_settings.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/assistant/models.py` & `django_sql_explorer-4.2b1/explorer/assistant/models.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/assistant/prompts.py` & `django_sql_explorer-4.2b1/explorer/assistant/prompts.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/assistant/tests.py` & `django_sql_explorer-4.2b1/explorer/assistant/tests.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/assistant/utils.py` & `django_sql_explorer-4.2b1/explorer/assistant/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from explorer import app_settings
 from explorer.schema import schema_info
 from explorer.utils import get_valid_connection
-from sql_metadata import Parser
 from django.db.utils import OperationalError
 
-if app_settings.EXPLORER_AI_API_KEY:
-    import tiktoken
-    from openai import OpenAI
 
 OPENAI_MODEL = app_settings.EXPLORER_ASSISTANT_MODEL["name"]
 ROW_SAMPLE_SIZE = 2
 
 
 def openai_client():
+    from openai import OpenAI
     return OpenAI(
         api_key=app_settings.EXPLORER_AI_API_KEY,
         base_url=app_settings.EXPLORER_ASSISTANT_BASE_URL
     )
 
 
 def do_req(prompt):
@@ -69,25 +66,27 @@
     for row in rows[1:]:
         row_str = " | ".join(str(item) for item in row)
         ret += row_str + "\n"
     return ret
 
 
 def get_table_names_from_query(sql):
+    from sql_metadata import Parser
     if sql:
         try:
             parsed = Parser(sql)
             return parsed.tables
         except ValueError:
             return []
     return []
 
 
 def num_tokens_from_string(string: str) -> int:
     """Returns the number of tokens in a text string."""
+    import tiktoken
     encoding = tiktoken.encoding_for_model(OPENAI_MODEL)
     num_tokens = len(encoding.encode(string))
     return num_tokens
 
 
 def fits_in_window(string: str) -> bool:
     # Ratchet down by 5% to account for other boilerplate and system prompt
```

### Comparing `django_sql_explorer-4.1b6/explorer/assistant/views.py` & `django_sql_explorer-4.2b1/explorer/assistant/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.http import JsonResponse
 from django.utils import timezone
 from django.views.decorators.http import require_POST
 import json
 
-from explorer.tracker import Stat, StatNames
+from explorer.telemetry import Stat, StatNames
 from explorer.utils import get_valid_connection
 from explorer.assistant.models import PromptLog
 from explorer.assistant.prompts import primary_prompt
 from explorer.assistant.utils import (
     do_req, extract_response, tables_from_schema_info,
     get_table_names_from_query, sample_rows_from_tables,
     fits_in_window
```

### Comparing `django_sql_explorer-4.1b6/explorer/charts.py` & `django_sql_explorer-4.2b1/explorer/charts.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/connections.py` & `django_sql_explorer-4.2b1/explorer/connections.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/exporters.py` & `django_sql_explorer-4.2b1/explorer/exporters.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/forms.py` & `django_sql_explorer-4.2b1/explorer/forms.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/locale/ru/LC_MESSAGES/django.mo` & `django_sql_explorer-4.2b1/explorer/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/locale/ru/LC_MESSAGES/django.po` & `django_sql_explorer-4.2b1/explorer/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/locale/zh_Hans/LC_MESSAGES/django.mo` & `django_sql_explorer-4.2b1/explorer/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/locale/zh_Hans/LC_MESSAGES/django.po` & `django_sql_explorer-4.2b1/explorer/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/migrations/0001_initial.py` & `django_sql_explorer-4.2b1/explorer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/migrations/0009_auto_20201009_0547.py` & `django_sql_explorer-4.2b1/explorer/migrations/0009_auto_20201009_0547.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/migrations/0011_query_favorites.py` & `django_sql_explorer-4.2b1/explorer/migrations/0011_query_favorites.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/migrations/0012_alter_queryfavorite_query_alter_queryfavorite_user.py` & `django_sql_explorer-4.2b1/explorer/migrations/0012_alter_queryfavorite_query_alter_queryfavorite_user.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/migrations/0013_querylog_error_querylog_success.py` & `django_sql_explorer-4.2b1/explorer/migrations/0013_querylog_error_querylog_success.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/migrations/0014_promptlog.py` & `django_sql_explorer-4.2b1/explorer/migrations/0014_promptlog.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/models.py` & `django_sql_explorer-4.2b1/explorer/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
 from time import time
+import uuid
 
 from django.conf import settings
 from django.core.exceptions import ValidationError
 from django.db import DatabaseError, models, transaction
 from django.urls import reverse
 from django.utils.translation import gettext_lazy as _
 
 from explorer import app_settings
-from explorer.tracker import Stat, StatNames
+from explorer.telemetry import Stat, StatNames
 from explorer.utils import (
     extract_params, get_params_for_url, get_s3_bucket, get_valid_connection, passes_blacklist, s3_url,
     shared_dict_update, swap_params,
 )
 
 
 MSG_FAILED_BLACKLIST = "Query failed the SQL blacklist: %s"
@@ -389,7 +390,54 @@
 
     @property
     def stats(self):
         return {c.label: c.value for c in self._stats}
 
     def __str__(self):
         return str(self._header)
+
+
+class ExplorerValueManager(models.Manager):
+
+    def get_uuid(self):
+        # If blank or non-existing, generates a new UUID
+        uuid_obj, created = self.get_or_create(
+            key=ExplorerValue.INSTALL_UUID,
+            defaults={"value": str(uuid.uuid4())}
+        )
+        if created or uuid_obj.value is None:
+            uuid_obj.value = str(uuid.uuid4())
+            uuid_obj.save()
+        return uuid_obj.value
+
+    def get_startup_last_send(self):
+        # Stored as a Unix timestamp
+        try:
+            timestamp = self.get(key=ExplorerValue.STARTUP_METRIC_LAST_SEND).value
+            if timestamp:
+                return float(timestamp)
+            return None
+        except ExplorerValue.DoesNotExist:
+            return None
+
+    def set_startup_last_send(self, ts):
+        obj, created = self.get_or_create(
+            key=ExplorerValue.STARTUP_METRIC_LAST_SEND,
+            defaults={"value": str(ts)}
+        )
+        if not created:
+            obj.value = str(ts)
+            obj.save()
+
+
+class ExplorerValue(models.Model):
+    INSTALL_UUID = "UUID"
+    STARTUP_METRIC_LAST_SEND = "SMLS"
+    EXPLORER_SETTINGS_CHOICES = [
+        (INSTALL_UUID, "Install Unique ID"),
+        (STARTUP_METRIC_LAST_SEND, "Startup metric last send"),
+    ]
+
+    key = models.CharField(max_length=5, choices=EXPLORER_SETTINGS_CHOICES)
+    value = models.TextField(null=True, blank=True)
+
+    objects = ExplorerValueManager()
```

### Comparing `django_sql_explorer-4.1b6/explorer/permissions.py` & `django_sql_explorer-4.2b1/explorer/permissions.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/schema.py` & `django_sql_explorer-4.2b1/explorer/schema.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/src/js/assistant.js` & `django_sql_explorer-4.2b1/explorer/src/js/assistant.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -116,14 +116,15 @@
         sql: window.editor?.state.doc.toString() ?? null,
         connection: document.getElementById("id_connection")?.value ?? null,
         assistant_request: document.getElementById("id_assistant_input")?.value ?? null,
         selected_tables: selectedTables,
         db_error: getErrorMessage()
     };
 
+    document.getElementById("assistant_response").innerHTML = '';
     document.getElementById("response_block").classList.remove('d-none');
     document.getElementById("assistant_spinner").classList.remove('d-none');
 
     fetch('../assistant/', {
             method: 'POST',
             headers: {
                 'Content-Type': 'application/json',
@@ -136,14 +137,15 @@
                 throw new Error('Network response was not ok');
             }
             return response.json();
         })
         .then(data => {
             const output = DOMPurify.sanitize(marked.parse(data.message));
             document.getElementById("assistant_response").innerHTML = output;
+            document.getElementById("assistant_spinner").classList.add('d-none');
             setUpCopyButtons();
         })
         .catch(error => {
             console.error('Error:', error);
         });
 }
```

### Comparing `django_sql_explorer-4.1b6/explorer/src/js/codemirror-config.js` & `django_sql_explorer-4.2b1/explorer/src/js/codemirror-config.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/src/js/explorer.js` & `django_sql_explorer-4.2b1/explorer/src/js/explorer.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/src/js/favorites.js` & `django_sql_explorer-4.2b1/explorer/src/js/favorites.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/src/js/main.js` & `django_sql_explorer-4.2b1/explorer/src/js/main.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/src/js/pivot-setup.js` & `django_sql_explorer-4.2b1/explorer/src/js/pivot-setup.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/src/js/pivot.js` & `django_sql_explorer-4.2b1/explorer/src/js/pivot.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/src/js/query-list.js` & `django_sql_explorer-4.2b1/explorer/src/js/query-list.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/src/js/schema.js` & `django_sql_explorer-4.2b1/explorer/src/js/schema.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/src/js/table-to-csv.js` & `django_sql_explorer-4.2b1/explorer/src/js/table-to-csv.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/src/scss/assistant.scss` & `django_sql_explorer-4.2b1/explorer/src/scss/assistant.scss`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/src/scss/explorer.scss` & `django_sql_explorer-4.2b1/explorer/src/scss/explorer.scss`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/src/scss/pivot.css` & `django_sql_explorer-4.2b1/explorer/src/scss/pivot.css`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/static/explorer/bootstrap-icons.woff` & `django_sql_explorer-4.2b1/explorer/static/explorer/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/static/explorer/bootstrap-icons.woff2` & `django_sql_explorer-4.2b1/explorer/static/explorer/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/static/explorer/explorer.js` & `django_sql_explorer-4.2b1/explorer/static/explorer/explorer.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -22478,27 +22478,27 @@
         e = {
             sql: (i = (t = window.editor) == null ? void 0 : t.state.doc.toString()) != null ? i : null,
             connection: (s = (r = document.getElementById("id_connection")) == null ? void 0 : r.value) != null ? s : null,
             assistant_request: (l = (o = document.getElementById("id_assistant_input")) == null ? void 0 : o.value) != null ? l : null,
             selected_tables: n,
             db_error: dm()
         };
-    document.getElementById("response_block").classList.remove("d-none"), document.getElementById("assistant_spinner").classList.remove("d-none"), fetch("../assistant/", {
+    document.getElementById("assistant_response").innerHTML = "", document.getElementById("response_block").classList.remove("d-none"), document.getElementById("assistant_spinner").classList.remove("d-none"), fetch("../assistant/", {
         method: "POST",
         headers: {
             "Content-Type": "application/json",
             "X-CSRFToken": Uu()
         },
         body: JSON.stringify(e)
     }).then(h => {
         if (!h.ok) throw new Error("Network response was not ok");
         return h.json()
     }).then(h => {
         const f = IS.sanitize(Ne.parse(h.message));
-        document.getElementById("assistant_response").innerHTML = f, HS()
+        document.getElementById("assistant_response").innerHTML = f, document.getElementById("assistant_spinner").classList.add("d-none"), HS()
     }).catch(h => {
         console.error("Error:", h)
     })
 }
 
 function HS() {
     document.querySelectorAll("#assistant_response pre").forEach(n => {
```

### Comparing `django_sql_explorer-4.1b6/explorer/static/explorer/favorites.js` & `django_sql_explorer-4.2b1/explorer/static/explorer/favorites.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/static/explorer/index.js` & `django_sql_explorer-4.2b1/explorer/static/explorer/index.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/static/explorer/main.js` & `django_sql_explorer-4.2b1/explorer/static/explorer/main.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/static/explorer/pivot-setup.js` & `django_sql_explorer-4.2b1/explorer/static/explorer/pivot-setup.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/static/explorer/query-list.js` & `django_sql_explorer-4.2b1/explorer/static/explorer/query-list.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/static/explorer/schema.js` & `django_sql_explorer-4.2b1/explorer/static/explorer/schema.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/static/explorer/styles.css` & `django_sql_explorer-4.2b1/explorer/static/explorer/styles.css`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/tasks.py` & `django_sql_explorer-4.2b1/explorer/tasks.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/templates/explorer/assistant.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/assistant.html`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,16 @@
                         <button type="button" class="btn btn-outline-primary" id="ask_assistant_btn">Ask Assistant</button>
                     </div>
                 </div>
             </div>
 
 
             <div id="response_block" class="position-relative d-none">
-                <div class="mt-3 p-2 pt-4 rounded-2 border bg-light" id="assistant_response">
+                <div class="mt-3 p-2 pt-4 rounded-2 border bg-light">
+                    <div id="assistant_response"></div>
                     <p class="spinner-border text-primary d-none" id="assistant_spinner" role="status">
                         <span class="visually-hidden">Loading...</span>
                     </p>
                 </div>
             </div>
         </div>
     </div>
```

### Comparing `django_sql_explorer-4.1b6/explorer/templates/explorer/base.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/base.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/templates/explorer/export_buttons.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/export_buttons.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/templates/explorer/fullscreen.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/fullscreen.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/templates/explorer/params.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/params.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/templates/explorer/pdf_template.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/pdf_template.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/templates/explorer/play.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/play.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/templates/explorer/preview_pane.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/preview_pane.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/templates/explorer/query.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/query.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/templates/explorer/query_confirm_delete.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/query_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/templates/explorer/query_favorites.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/query_favorites.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/templates/explorer/query_list.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/query_list.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/templates/explorer/querylog_list.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/querylog_list.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/templates/explorer/schema.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/schema.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/templatetags/explorer_tags.py` & `django_sql_explorer-4.2b1/explorer/templatetags/explorer_tags.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/templatetags/vite.py` & `django_sql_explorer-4.2b1/explorer/templatetags/vite.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/tests/factories.py` & `django_sql_explorer-4.2b1/explorer/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/tests/settings.py` & `django_sql_explorer-4.2b1/explorer/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/tests/test_actions.py` & `django_sql_explorer-4.2b1/explorer/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/tests/test_apps.py` & `django_sql_explorer-4.2b1/explorer/tests/test_apps.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/tests/test_csrf_cookie_name.py` & `django_sql_explorer-4.2b1/explorer/tests/test_csrf_cookie_name.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/tests/test_exporters.py` & `django_sql_explorer-4.2b1/explorer/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/tests/test_forms.py` & `django_sql_explorer-4.2b1/explorer/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/tests/test_models.py` & `django_sql_explorer-4.2b1/explorer/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/tests/test_schema.py` & `django_sql_explorer-4.2b1/explorer/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/tests/test_tasks.py` & `django_sql_explorer-4.2b1/explorer/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/tests/test_utils.py` & `django_sql_explorer-4.2b1/explorer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/tests/test_views.py` & `django_sql_explorer-4.2b1/explorer/tests/test_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -544,15 +544,15 @@
     def test_downloading_from_playground(self):
         sql = "select 1;"
         resp = self.client.post(reverse("download_sql"), {"sql": sql})
         self.assertIn("attachment", resp["Content-Disposition"])
         self.assertEqual("text/csv", resp["content-type"])
         ql = QueryLog.objects.first()
         self.assertIn(
-            'filename="Playground-%s.csv"' % ql.id,
+            f'filename="Playground-{ql.id}.csv"',
             resp["Content-Disposition"]
         )
 
     def test_stream_csv_from_query(self):
         q = SimpleQueryFactory()
         resp = self.client.get(
             reverse("stream_query", kwargs={"query_id": q.id})
```

### Comparing `django_sql_explorer-4.1b6/explorer/urls.py` & `django_sql_explorer-4.2b1/explorer/urls.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/utils.py` & `django_sql_explorer-4.2b1/explorer/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,16 @@
 def param(name):
     return f"{EXPLORER_PARAM_TOKEN}{name}{EXPLORER_PARAM_TOKEN}"
 
 
 def swap_params(sql, params):
     p = params.items() if params else {}
     for k, v in p:
-        regex = re.compile(r"\$\$%s(?:\|([^\$\:]+))?(?:\:([^\$]+))?\$\$" % str(k).lower(), re.I)
+        fmt_k = re.escape(str(k).lower())
+        regex = re.compile(rf"\$\${fmt_k}(?:\|([^\$\:]+))?(?:\:([^\$]+))?\$\$", re.I)
         sql = regex.sub(str(v), sql)
     return sql
 
 
 def extract_params(text):
     regex = re.compile(r"\$\$([a-z0-9_]+)(?:\|([^\$\:]+))?(?:\:([^\$]+))?\$\$", re.IGNORECASE)
     params = re.findall(regex, text)
```

### Comparing `django_sql_explorer-4.1b6/explorer/views/__init__.py` & `django_sql_explorer-4.2b1/explorer/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/views/auth.py` & `django_sql_explorer-4.2b1/explorer/views/auth.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/views/create.py` & `django_sql_explorer-4.2b1/explorer/views/create.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/views/download.py` & `django_sql_explorer-4.2b1/explorer/views/download.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/views/email.py` & `django_sql_explorer-4.2b1/explorer/views/email.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/views/export.py` & `django_sql_explorer-4.2b1/explorer/views/export.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/views/list.py` & `django_sql_explorer-4.2b1/explorer/views/list.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/views/mixins.py` & `django_sql_explorer-4.2b1/explorer/views/mixins.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/views/query.py` & `django_sql_explorer-4.2b1/explorer/views/query.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/views/query_favorite.py` & `django_sql_explorer-4.2b1/explorer/views/query_favorite.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/views/schema.py` & `django_sql_explorer-4.2b1/explorer/views/schema.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/explorer/views/stream.py` & `django_sql_explorer-4.2b1/explorer/views/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from django.shortcuts import get_object_or_404
 from django.views import View
 
 from explorer.models import Query
 from explorer.views.auth import PermissionRequiredMixin
 from explorer.views.export import _export
-from explorer.tracker import Stat, StatNames
+from explorer.telemetry import Stat, StatNames
 
 
 class StreamQueryView(PermissionRequiredMixin, View):
 
     permission_required = "view_permission"
 
     def get(self, request, query_id, *args, **kwargs):
```

### Comparing `django_sql_explorer-4.1b6/explorer/views/utils.py` & `django_sql_explorer-4.2b1/explorer/views/utils.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/package.json` & `django_sql_explorer-4.2b1/package.json`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/setup.cfg` & `django_sql_explorer-4.2b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/setup.py` & `django_sql_explorer-4.2b1/setup.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b6/vite.config.js` & `django_sql_explorer-4.2b1/vite.config.js`

 * *Files identical despite different names*


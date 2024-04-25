# Comparing `tmp/django_glue-0.5.2.3.tar.gz` & `tmp/django_glue-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_glue-0.5.2.3.tar", last modified: Tue Apr 16 20:58:45 2024, max compression
+gzip compressed data, was "django_glue-0.5.3.tar", last modified: Thu Apr 25 19:54:19 2024, max compression
```

## Comparing `django_glue-0.5.2.3.tar` & `django_glue-0.5.3.tar`

### file list

```diff
@@ -1,85 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.667000 django_glue-0.5.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/CONTRIBUTORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-16 20:58:45.667000 django_glue-0.5.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.659000 django_glue-0.5.2.3/django_glue/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/context_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.663000 django_glue-0.5.2.3/django_glue/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/glue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.663000 django_glue-0.5.2.3/django_glue/services/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/services/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/services/model_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/services/query_sets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/services/services.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/services/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.655000 django_glue-0.5.2.3/django_glue/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.659000 django_glue-0.5.2.3/django_glue/static/django_glue/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.667000 django_glue-0.5.2.3/django_glue/static/django_glue/js/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_ajax.js
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_csrf.js
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_event.js
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_function.js
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_keep_live.js
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_message.js
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_model_object.js
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_query_set.js
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_response.js
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_shortcuts.js
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_template.js
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_utils.js
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_view.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.659000 django_glue-0.5.2.3/django_glue/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.667000 django_glue-0.5.2.3/django_glue/templates/django_glue/
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/templates/django_glue/django_glue.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.667000 django_glue-0.5.2.3/django_glue/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/templatetags/django_glue.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/django_glue/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.667000 django_glue-0.5.2.3/django_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-16 20:58:45.000000 django_glue-0.5.2.3/django_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-16 20:58:45.000000 django_glue-0.5.2.3/django_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:58:45.000000 django_glue-0.5.2.3/django_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:58:45.000000 django_glue-0.5.2.3/django_glue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 20:58:45.000000 django_glue-0.5.2.3/django_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 20:58:45.000000 django_glue-0.5.2.3/django_glue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-16 20:58:45.671000 django_glue-0.5.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.667000 django_glue-0.5.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:45.667000 django_glue-0.5.2.3/tests/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/migrations/0002_bigtestmodel_foreign_key_alter_testmodel_birth_date.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-16 20:58:36.000000 django_glue-0.5.2.3/tests/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.139330 django_glue-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-25 19:54:10.000000 django_glue-0.5.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-25 19:54:10.000000 django_glue-0.5.3/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-25 19:54:10.000000 django_glue-0.5.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-25 19:54:10.000000 django_glue-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-25 19:54:19.139330 django_glue-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-25 19:54:10.000000 django_glue-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.123330 django_glue-0.5.3/django_glue/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.123330 django_glue-0.5.3/django_glue/access/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/access/access.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/access/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/access/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/context_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.123330 django_glue-0.5.3/django_glue/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.123330 django_glue-0.5.3/django_glue/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/base_entity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.127330 django_glue-0.5.3/django_glue/entities/function/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/function/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/function/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/function/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/function/maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/function/post_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/function/response_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/function/session_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.127330 django_glue-0.5.3/django_glue/entities/model_object/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/model_object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/model_object/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/model_object/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/model_object/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/model_object/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/model_object/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/model_object/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/model_object/maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/model_object/response_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/model_object/session_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/post_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.131330 django_glue-0.5.3/django_glue/entities/query_set/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/query_set/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/query_set/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/query_set/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/query_set/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/query_set/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/query_set/maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/query_set/post_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/query_set/response_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/query_set/session_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.131330 django_glue-0.5.3/django_glue/entities/template/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/template/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/template/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/template/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/template/maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/template/post_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/template/response_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/template/session_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.131330 django_glue-0.5.3/django_glue/form/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/form/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/form/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/form/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/form/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/form/maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/form/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/glue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.131330 django_glue-0.5.3/django_glue/handler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/handler/body_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/handler/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/handler/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/handler/maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/handler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.131330 django_glue-0.5.3/django_glue/response/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/response/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/response/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/response/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.135330 django_glue-0.5.3/django_glue/session/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/session/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/session/glue_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/session/keep_alive_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/session/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.119330 django_glue-0.5.3/django_glue/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.119330 django_glue-0.5.3/django_glue/static/django_glue/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.135330 django_glue-0.5.3/django_glue/static/django_glue/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_ajax.js
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_csrf.js
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_event.js
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_function.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_keep_live.js
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_message.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_model_object.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_query_set.js
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_response.js
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_shortcuts.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_template.js
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_utils.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_view.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.119330 django_glue-0.5.3/django_glue/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.135330 django_glue-0.5.3/django_glue/templates/django_glue/
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/templates/django_glue/django_glue.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.135330 django_glue-0.5.3/django_glue/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/templatetags/django_glue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.139330 django_glue-0.5.3/django_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-25 19:54:19.000000 django_glue-0.5.3/django_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-25 19:54:19.000000 django_glue-0.5.3/django_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:54:19.000000 django_glue-0.5.3/django_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:54:19.000000 django_glue-0.5.3/django_glue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 19:54:19.000000 django_glue-0.5.3/django_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 19:54:19.000000 django_glue-0.5.3/django_glue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-25 19:54:10.000000 django_glue-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-25 19:54:19.139330 django_glue-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-25 19:54:10.000000 django_glue-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.139330 django_glue-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.139330 django_glue-0.5.3/tests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/migrations/0002_bigtestmodel_foreign_key_alter_testmodel_birth_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/wsgi.py
```

### Comparing `django_glue-0.5.2.3/CHANGELOG.md` & `django_glue-0.5.3/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 # Changelog for Django Glue
 
-## 0.5.2.3
 
+## 0.5.3
+### Changes
+- Created an extendable structure using glue entities as the base objects.
+- Removed meta and context keys from session data. 
+- Handler map based on action called from glue js objects to process response.
+- Dataclass structure for Response, Session and Post data. 
+
+### Bugs
+- Corrected issue on glue views that glue models. Encoded unique name is based on path the user requests the view from. 
+ 
+
+
+## 0.5.2.3
 ### Changes
 - Glue model object returns a null object if we try to find a id that does not exist.
 - Updated html attributes on glue model objects and added attributes to js model objects. 
 
 
 ## 0.5.2.2
```

### Comparing `django_glue-0.5.2.3/LICENSE.md` & `django_glue-0.5.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.2.3/PKG-INFO` & `django_glue-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-glue
-Version: 0.5.2.3
+Version: 0.5.3
 Summary: Industrial Strength Glue for Django Backends and Frontends!
 Home-page: https://github.com/stratusadv/django-glue
 Author: Nathan Johnson, Austin Sauer & Wesley Howery
 Author-email: info@stratusadv.com
 License: MIT
 Keywords: glue,django,backend,frontend,javascript,active server pages
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django_glue-0.5.2.3/README.md` & `django_glue-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.2.3/django_glue/context_processors.py` & `django_glue-0.5.3/django_glue/context_processors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 
 from django_glue.conf import settings
 from django_glue import __version__
-from django_glue.sessions import GlueSession
+from django_glue.session import GlueSession
 
 
 def glue(request):
     return {
         'DJANGO_GLUE_VERSION': __version__,
-        settings.DJANGO_GLUE_CONTEXT_NAME: request.session.get(settings.DJANGO_GLUE_SESSION_NAME, {}).get('context'),
+        settings.DJANGO_GLUE_CONTEXT_NAME: request.session.get(settings.DJANGO_GLUE_SESSION_NAME, {}),
         settings.DJANGO_GLUE_KEEP_LIVE_CONTEXT_NAME: request.session.get(settings.DJANGO_GLUE_KEEP_LIVE_SESSION_NAME, {}),
         'DJANGO_GLUE_KEEP_LIVE_INTERVAL_TIME_MILLISECONDS': settings.DJANGO_GLUE_KEEP_LIVE_INTERVAL_TIME_SECONDS * 1000,
         'GLUE_SESSION_DATA': json.dumps(GlueSession(request).session),
     }
```

### Comparing `django_glue-0.5.2.3/django_glue/core/decorators.py` & `django_glue-0.5.3/django_glue/core/decorators.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.2.3/django_glue/responses.py` & `django_glue-0.5.3/django_glue/response/responses.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,13 @@
 from typing import Optional
 
 from django.http import JsonResponse
 
-from django_glue.data_classes import GlueJsonResponseData, GlueJsonData
-from django_glue.enums import GlueJsonResponseType, GlueJsonResponseStatus
-
-
-def generate_json_200_response(
-        message_title: str,
-        message_body: str,
-        data: Optional[GlueJsonData] = None,
-        optional_message_data: Optional[dict] = None,
-) -> JsonResponse:
-
-    return generate_json_200_response_data(
-        message_title=message_title,
-        message_body=message_body,
-        data=data,
-        optional_message_data=optional_message_data,
-    ).to_django_json_response()
+from django_glue.response.data import GlueJsonData, GlueJsonResponseData
+from django_glue.response.enums import GlueJsonResponseStatus, GlueJsonResponseType
 
 
 def generate_json_200_response_data(
         message_title: str,
         message_body: str,
         data: Optional[GlueJsonData] = None,
         optional_message_data: Optional[dict] = None,
@@ -38,23 +23,25 @@
     )
 
 
 def generate_json_404_response(
         message_title: str = 'Request not Found',
         message_body: str = 'The requested information, object or view you are looking for was not found.',
 ) -> JsonResponse:
+
     return generate_json_404_response_data(
         message_title,
         message_body,
     ).to_django_json_response()
 
 
 def generate_json_404_response_data(
         message_title: str = 'Request not Found',
         message_body: str = 'The requested information, object or view you are looking for was not found.',
 ) -> GlueJsonResponseData:
+
     return GlueJsonResponseData(
         message_title=message_title,
         message_body=message_body,
         response_status=GlueJsonResponseStatus.ERROR,
         response_type=GlueJsonResponseType.ERROR,
     )
```

### Comparing `django_glue-0.5.2.3/django_glue/services/functions.py` & `django_glue-0.5.3/django_glue/entities/function/entities.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,43 @@
-from typing import Optional
-
-from django.contrib.contenttypes.models import ContentType
-from django.db.models import Model
-
-from django_glue.data_classes import GlueJsonResponseData, GlueJsonData, GlueBodyData, GlueMetaData
-from django_glue.responses import generate_json_200_response_data, generate_json_404_response_data
-from django_glue.services.services import Service
-from django_glue.utils import generate_simple_field_dict, get_field_names_from_model, check_valid_method_kwargs, \
-    type_set_method_kwargs, generate_field_dict
-
-
-class GlueFunctionService(Service):
-    def __init__(self, meta_data: GlueMetaData) -> None:
-        self.meta_data = meta_data
-        self.module_name = None
-        self.function = None
-
-    def load_function(self):
-        self.module_name = '.'.join(self.meta_data.function.split('.')[:-1])
-        self.function = self.meta_data.function.split('.')[-1]
-
-    def process_get_action(self, body_data: GlueBodyData) -> GlueJsonResponseData:
-        self.load_function()
-        kwargs = body_data['data']['kwargs']
-        function_return = None
-        module = __import__(self.module_name, fromlist=[self.function])
-
-        if hasattr(module, self.function):
-            function = getattr(module, self.function)
-
-            if check_valid_method_kwargs(function, kwargs):
-                type_set_kwargs = type_set_method_kwargs(function, kwargs)
-
-                function_return = function(**type_set_kwargs)
-            else:
-                return generate_json_404_response_data()
-        else:
-            return generate_json_404_response_data()
-
-        json_data = GlueJsonData()
-        json_data.function_return = function_return
-
-        return generate_json_200_response_data(
-            'FUNCTION CALL',
-            'this is a response from an function call!',
-            json_data
+from django_glue.access.access import GlueAccess
+from django_glue.entities.base_entity import GlueEntity
+from django_glue.entities.function.response_data import GlueFunctionJsonData
+from django_glue.entities.function.session_data import FunctionSessionData
+from django_glue.handler.enums import GlueConnection
+from django_glue.utils import check_valid_method_kwargs, type_set_method_kwargs
+
+
+class GlueFunction(GlueEntity):
+    def __init__(
+            self,
+            unique_name: str,
+            function_path: str,
+    ):
+        super().__init__(unique_name, GlueConnection.FUNCTION, GlueAccess.VIEW)
+        self.function_path = function_path
+
+        self.module_name = '.'.join(function_path.split('.')[:-1])
+        self.function_name = function_path.split('.')[-1]
+
+    def call(self, function_kwargs):
+        module = __import__(self.module_name, fromlist=[self.function_name])
+
+        if hasattr(module, self.function_name):
+            function = getattr(module, self.function_name)
+
+            if check_valid_method_kwargs(function, function_kwargs):
+                type_set_kwargs = type_set_method_kwargs(function, function_kwargs)
+
+                return function(**type_set_kwargs)
+
+        return None
+
+    def to_session_data(self) -> FunctionSessionData:
+        return FunctionSessionData(
+            unique_name=self.unique_name,
+            connection=self.connection,
+            access=self.access,
+            function_path=self.function_path
         )
+
+    def to_response_data(self, function_return) -> GlueFunctionJsonData:
+        return GlueFunctionJsonData(function_return)
```

### Comparing `django_glue-0.5.2.3/django_glue/services/query_sets.py` & `django_glue-0.5.3/django_glue/entities/query_set/handlers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,127 +1,131 @@
-from typing import Optional
+from django_glue.access.decorators import check_access
+from django_glue.entities.model_object.factories import glue_model_object_from_glue_query_set_session, \
+    glue_model_objects_from_query_set
+from django_glue.entities.model_object.response_data import GlueModelObjectJsonData, MethodGlueModelObjectJsonData
+from django_glue.entities.query_set.actions import GlueQuerySetAction
+from django_glue.entities.query_set.factories import glue_query_set_from_session_data
+from django_glue.entities.post_data import GetPostData, DeletePostData, UpdatePostData, MethodPostData
+from django_glue.entities.query_set.post_data import FilterGlueQuerySetPostData
+from django_glue.entities.query_set.response_data import GlueQuerySetJsonData, MethodGlueQuerySetJsonData
+
+from django_glue.entities.query_set.session_data import GlueQuerySetSessionData
+from django_glue.handler.handlers import GlueRequestHandler
+from django_glue.response.data import GlueJsonResponseData
+from django_glue.response.responses import generate_json_200_response_data
+
+
+class AllGlueQuerySetHandler(GlueRequestHandler):
+    action = GlueQuerySetAction.ALL
+    _session_data_class = GlueQuerySetSessionData
 
-from django.db.models import QuerySet
+    @check_access
+    def process_response_data(self) -> GlueJsonResponseData:
 
-from django_glue.data_classes import GlueJsonResponseData, GlueBodyData, GlueMetaData, GlueJsonData
-from django_glue.responses import generate_json_200_response_data, generate_json_404_response_data
-from django_glue.services.services import Service
-from django_glue.utils import decode_query_set_from_str, generate_simple_field_dict, get_field_names_from_model, \
-    check_valid_method_kwargs, type_set_method_kwargs, field_name_included
-
-
-class GlueQuerySetService(Service):
-    def __init__(self, meta_data: GlueMetaData) -> None:
-        self.meta_data = meta_data
-        # Query set is optional for lazy loading. Call load_query_set() before using it.
-        self.query_set: Optional[QuerySet] = None
-
-    def load_query_set(self):
-        self.query_set = decode_query_set_from_str(self.meta_data.query_set_str)
-
-    def process_get_action(self, body_data: GlueBodyData) -> GlueJsonResponseData:
-        self.load_query_set()
-
-        if 'filter_params' in body_data['data']:
-            data = []
-            for model_object in self.query_set.filter(**body_data['data']['filter_params']):
-                data.append(GlueJsonData(simple_fields=generate_simple_field_dict(
-                        model_object, self.meta_data.fields, self.meta_data.exclude)))
-
-        elif 'all' in body_data['data']:
-            data = []
-            for model_object in self.query_set.all():
-                data.append(GlueJsonData(
-                    simple_fields=generate_simple_field_dict(model_object, self.meta_data.fields, self.meta_data.exclude)
-                ))
-
-        else:
-            model_object = self.query_set.get(id=body_data['data']['id'])
-            data = GlueJsonData(
-                simple_fields=generate_simple_field_dict(model_object, self.meta_data.fields, self.meta_data.exclude)
-            )
+        glue_query_set = glue_query_set_from_session_data(self.session_data)
+        glue_model_objects = glue_model_objects_from_query_set(glue_query_set.query_set.all(), self.session_data)
 
         return generate_json_200_response_data(
-            'THE QUERY GET ACTION',
-            'this is a response from an query set get action',
-            data
+            message_title='Success',
+            message_body='Successfully retrieved model object!',
+            data=GlueQuerySetJsonData([GlueModelObjectJsonData(glue_model_object.fields) for glue_model_object in glue_model_objects])
         )
 
-    def process_update_action(self, body_data: GlueBodyData) -> GlueJsonResponseData:
-        self.load_query_set()
-
-        model_object = self.meta_data.model_class.objects.get(id=body_data['data']['id'])
 
-        # Todo: This is duplicated code
-        for field_name in get_field_names_from_model(self.meta_data.model_class):
-            if field_name in body_data['data'] and field_name != 'id' and field_name_included(field_name, self.meta_data.fields, self.meta_data.exclude):
-                model_object.__dict__[field_name] = body_data['data'][field_name]
+class DeleteGlueQuerySetHandler(GlueRequestHandler):
+    action = GlueQuerySetAction.DELETE
+    _session_data_class = GlueQuerySetSessionData
+    _post_data_class = DeletePostData
+
+    @check_access
+    def process_response_data(self) -> GlueJsonResponseData:
+        glue_query_set = glue_query_set_from_session_data(self.session_data)
 
-        model_object.save()
+        filtered_query_set = glue_query_set.query_set.filter(id__in=self.post_data.id)
+        filtered_query_set.delete()
 
         return generate_json_200_response_data(
-            'THE QUERY UPDATE ACTION',
-            'this is a response from an query set update action!'
+            message_title='Success',
+            message_body='Successfully deleted queryset!',
         )
 
-    def process_delete_action(self, body_data: GlueBodyData) -> GlueJsonResponseData:
-        self.load_query_set()
 
-        if isinstance(body_data['data']['id'], list) or isinstance(body_data['data']['id'], tuple):
-            self.query_set.filter(id__in=body_data['data']['id']).delete()
-
-        elif isinstance(body_data['data']['id'], int):
-            self.query_set.filter(id=body_data['data']['id']).delete()
-
-        else:
-            return generate_json_404_response_data()
+class FilterGlueQuerySetHandler(GlueRequestHandler):
+    action = GlueQuerySetAction.FILTER
+    _session_data_class = GlueQuerySetSessionData
+    _post_data_class = FilterGlueQuerySetPostData
+
+    @check_access
+    def process_response_data(self) -> GlueJsonResponseData:
+
+        glue_query_set = glue_query_set_from_session_data(self.session_data)
+        filtered_query_set = glue_query_set.query_set.filter(**self.post_data.filter_params)
+        glue_model_objects = glue_model_objects_from_query_set(filtered_query_set, self.session_data)
 
         return generate_json_200_response_data(
-            'THE QUERY DELETE ACTION',
-            'this is a response from an query set delete action!'
+            message_title='Success',
+            message_body='Successfully retrieved model object!',
+            data=GlueQuerySetJsonData([GlueModelObjectJsonData(glue_model_object.fields) for glue_model_object in glue_model_objects])
         )
 
-    def process_method_action(self, body_data: GlueBodyData) -> GlueJsonResponseData:
-        self.load_query_set()
 
-        if isinstance(body_data['data']['id'], list) or isinstance(body_data['data']['id'], tuple):
-            model_object = self.query_set.filter(id__in=body_data['data']['id'])
+class GetGlueQuerySetHandler(GlueRequestHandler):
+    action = GlueQuerySetAction.GET
+    _session_data_class = GlueQuerySetSessionData
+    _post_data_class = GetPostData
+
+    @check_access
+    def process_response_data(self) -> GlueJsonResponseData:
+        glue_query_set = glue_query_set_from_session_data(self.session_data)
 
-        elif isinstance(body_data['data']['id'], int):
-            model_object = self.query_set.get(id=body_data['data']['id'])
+        model_object = glue_query_set.query_set.get(id=self.post_data.id)
+        glue_model_object = glue_model_object_from_glue_query_set_session(model_object, self.session_data)
 
-        else:
-            return generate_json_404_response_data()
+        return generate_json_200_response_data(
+            message_title='Success',
+            message_body='Successfully retrieved model object!',
+            data=GlueQuerySetJsonData([GlueModelObjectJsonData(glue_model_object.fields)])
+        )
 
-        kwargs = body_data['data']['kwargs']
-        method_return = None
 
-        if body_data['data']['method'] in self.meta_data.methods and hasattr(self.meta_data.model_class, body_data['data']['method']):
-            if isinstance(model_object, QuerySet):
-                method_return = []
-                for object in model_object:
-                    method = getattr(object, body_data['data']['method'])
-                    if check_valid_method_kwargs(method, kwargs):
-                        type_set_kwargs = type_set_method_kwargs(method, kwargs)
-                        method_return.append(method(**type_set_kwargs))
+class UpdateGlueQuerySetHandler(GlueRequestHandler):
+    action = GlueQuerySetAction.UPDATE
+    _session_data_class = GlueQuerySetSessionData
+    _post_data_class = UpdatePostData
+
+    @check_access
+    def process_response_data(self) -> GlueJsonResponseData:
+        glue_query_set = glue_query_set_from_session_data(self.session_data)
 
-            elif isinstance(model_object, self.meta_data.model_class):
-                method = getattr(model_object, body_data['data']['method'])
+        model_object = glue_query_set.query_set.get(id=self.post_data.id)
 
-                if check_valid_method_kwargs(method, kwargs):
-                    type_set_kwargs = type_set_method_kwargs(method, kwargs)
-                    method_return = method(**type_set_kwargs)
+        glue_model_object = glue_model_object_from_glue_query_set_session(model_object, self.session_data)
+        glue_model_object.update(self.post_data.fields)
 
-            else:
-                return generate_json_404_response_data()
-        else:
-            return generate_json_404_response_data()
+        return generate_json_200_response_data(
+            message_title='Success',
+            message_body='Successfully updated model object!',
+            data=GlueQuerySetJsonData([GlueModelObjectJsonData(glue_model_object.fields)])
+        )
 
-        json_data = GlueJsonData()
 
-        json_data.method_return = method_return
+class MethodGlueQuerySetHandler(GlueRequestHandler):
+    action = GlueQuerySetAction.METHOD
+    _session_data_class = GlueQuerySetSessionData
+    _post_data_class = MethodPostData
+
+    def process_response_data(self) -> GlueJsonResponseData:
+        glue_query_set = glue_query_set_from_session_data(self.session_data)
+        filtered_query_set = glue_query_set.query_set.filter(id__in=self.post_data.id)
+
+        method_return_data = []
+
+        for model_object in filtered_query_set:
+            glue_model_object = glue_model_object_from_glue_query_set_session(model_object, self.session_data)
+            method_return = glue_model_object.call_method(self.post_data.method, self.post_data.kwargs)
+            method_return_data.append(MethodGlueModelObjectJsonData(method_return))
 
         return generate_json_200_response_data(
-            'THE METHOD ACTION',
-            'this is a response from an query set method action!',
-            json_data
-        )
+            message_title='Success',
+            message_body='Successfully updated model object!',
+            data=MethodGlueQuerySetJsonData(method_return_data)
+        )
```

### Comparing `django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_ajax.js` & `django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_ajax.js`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_event.js` & `django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_event.js`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_function.js` & `django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_function.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -7,17 +7,17 @@
     async call(kwargs = {}) {
         let data = {
             'kwargs': kwargs,
         }
 
         return await glue_ajax_request(
             this.unique_name,
-            'get',
+            'call',
             data
         ).then((response) => {
             console.log(response)
             glue_dispatch_response_event(response)
-            return response.data.function_return
+            return JSON.parse(response.data).function_return
         })
     }
 
 }
```

### Comparing `django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_keep_live.js` & `django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_keep_live.js`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_model_object.js` & `django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_model_object.js`

 * *Files 27% similar despite different names*

#### js-beautify {}

```diff
@@ -1,84 +1,113 @@
 class GlueModelObject {
+
     constructor(glue_unique_name) {
-        // Needs to be named glue_unique_name to avoid overriding the unique_name property
-        this.glue_unique_name = encodeUniqueName(glue_unique_name)
-        this['fields'] = {}
-        for (let key in window.glue_session_data['context'][this.glue_unique_name].fields) {
-            this[key] = window.glue_session_data['context'][this.glue_unique_name].fields[key].value
-            this['fields'][key] = window.glue_session_data['context'][this.glue_unique_name].fields[key]
+        // We are encoding the unique name twice when
+        this.glue_unique_name = glue_unique_name
+        this.glue_encoded_unique_name = encodeUniqueName(glue_unique_name)
+        this.glue_fields_set = false
+
+        // this['html_attr'] = {}
+        if (this.glue_encoded_unique_name in window.glue_session_data) {
+            this.set_fields(window.glue_session_data[this.glue_encoded_unique_name].fields)
         }
-        window.glue_keep_live.add_unique_name(this.glue_unique_name)
+
+        window.glue_keep_live.add_unique_name(this.glue_encoded_unique_name)
     }
 
     delete() {
         glue_ajax_request(
-            this.glue_unique_name,
-            'delete'
+            this.glue_encoded_unique_name,
+            'delete', {
+                'id': this.id
+            }
         ).then((response) => {
             console.log(response)
             glue_dispatch_response_event(response)
         }).catch((error) => {
             glue_dispatch_object_delete_error_event(error)
         })
     }
 
+    // Todo: Change this to load values.
     async get() {
         await glue_ajax_request(
-            this.glue_unique_name,
-            'get'
+            this.glue_encoded_unique_name,
+            'get', {
+                'id': this.id,
+            }
         ).then((response) => {
-            console.log(response)
             glue_dispatch_response_event(response)
-            this.set_properties(response.data.simple_fields)
+            this.set_properties(JSON.parse(response.data))
         }).catch((error) => {
             glue_dispatch_object_get_error_event(error)
         })
     }
 
     async method(method, kwargs = {}) {
         let data = {
+            'id': this.id,
             'method': method,
             'kwargs': kwargs,
         }
 
         return await glue_ajax_request(
-            this.glue_unique_name,
+            this.glue_encoded_unique_name,
             'method',
             data
         ).then((response) => {
-            console.log(response)
             glue_dispatch_response_event(response)
-            return response.data.method_return
+            return JSON.parse(response.data).method_return
         }).catch((error) => {
             glue_dispatch_object_method_error_event(error)
         })
     }
 
     async update(field = null) {
         await glue_ajax_request(
-            this.glue_unique_name,
-            'update',
-            this.get_properties()
+            this.glue_encoded_unique_name,
+            'update', {
+                'fields': this.get_properties(),
+                'id': this.id
+            }
         ).then((response) => {
             glue_dispatch_response_event(response)
             console.log(response)
+            glue_dispatch_response_event(response)
+            this.set_properties(JSON.parse(response.data))
+
         }).catch((error) => {
             glue_dispatch_object_update_error_event(error)
         })
     }
 
     get_properties() {
         let properties = {}
         Object.entries(this).forEach(([key, value]) => {
             properties[key] = value
         });
         return properties
     }
 
-    set_properties(properties) {
-        for (let key in properties) {
-            this[key] = properties[key]
+    set_properties(fields) {
+        // Only sets properties that are already initialized on the glue object model.
+        if (!this.glue_fields_set) {
+            this.set_fields(fields)
         }
+        let simple_fields = simplify_model_fields(fields)
+        for (let key in simple_fields) {
+            if (key in this) {
+                this[key] = simple_fields[key]
+            }
+        }
+    }
+
+    set_fields(fields) {
+        for (let key in fields) {
+            this[key] = ''
+            // this['form_fields'][key] = window.glue_session_data['context'][this.glue_encoded_unique_name].fields[key]
+        }
+        this.glue_fields_set = true
+
     }
 
 }
```

### Comparing `django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_query_set.js` & `django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_query_set.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -1,32 +1,33 @@
 class GlueQuerySet {
     constructor(glue_unique_name) {
-        this.glue_unique_name = encodeUniqueName(glue_unique_name)
+        this.glue_unique_name = glue_unique_name
+        this.glue_encoded_unique_name = encodeUniqueName(glue_unique_name)
 
         // We need this value on query to build GlueModelObjects
-        this.decoded_unique_name = glue_unique_name
-        for (let key in window.glue_session_data['context'][this.glue_unique_name].fields) {
-            this[key] = window.glue_session_data['context'][this.glue_unique_name].fields[key].value
-        }
+        // this.decoded_unique_name = glue_unique_name
+        // for (let key in window.glue_session_data['context'][this.glue_unique_name].fields) {
+        //     this[key] = window.glue_session_data['context'][this.glue_unique_name].fields[key].value
+        // }
 
-        window.glue_keep_live.add_unique_name(this.glue_unique_name)
+        window.glue_keep_live.add_unique_name(this.glue_encoded_unique_name)
     }
 
     async all() {
         let model_object_list = []
 
-        return await glue_ajax_request(this.glue_unique_name, 'get', {
+        return await glue_ajax_request(this.glue_encoded_unique_name, 'all', {
                 'all': true
             })
             .then((response) => {
-                console.log(response)
                 glue_dispatch_response_event(response)
-                for (let object in response.data) {
-                    let model_object = new GlueModelObject(this.decoded_unique_name);
-                    model_object.set_properties(response.data[object].simple_fields)
+                let glue_query_set = JSON.parse(response.data)
+                for (let object in glue_query_set) {
+                    let model_object = new GlueModelObject(this.glue_unique_name);
+                    model_object.set_properties(glue_query_set[object])
                     model_object_list.push(model_object)
                 }
                 return model_object_list
             });
     }
 
     async bulk_create(query_model_object_list) {
@@ -35,76 +36,77 @@
 
     async bulk_update(query_model_object_list) {
 
     }
 
     delete(id) {
         glue_ajax_request(
-            this.glue_unique_name,
+            this.glue_encoded_unique_name,
             'delete', {
                 'id': id
             }
         ).then((response) => {
             console.log(response)
             glue_dispatch_response_event(response)
         })
     }
 
     async filter(filter_params) {
         let model_object_list = []
 
-        return await glue_ajax_request(this.glue_unique_name, 'get', {
+        return await glue_ajax_request(this.glue_encoded_unique_name, 'filter', {
                 'filter_params': filter_params
             })
             .then((response) => {
                 console.log(response)
+                let glue_query_set = JSON.parse(response.data)
                 glue_dispatch_response_event(response)
-                for (let object in response.data) {
-                    let model_object = new GlueModelObject(this.decoded_unique_name);
-                    model_object.set_properties(response.data[object].simple_fields)
+                for (let object in glue_query_set) {
+                    let model_object = new GlueModelObject(this.glue_unique_name)
+                    model_object.set_properties(glue_query_set[object])
                     model_object_list.push(model_object)
                 }
 
                 return model_object_list
             });
     }
 
     async get(id) {
         let model_object = null
-        return await glue_ajax_request(this.glue_unique_name, 'get', {
+        return await glue_ajax_request(this.glue_encoded_unique_name, 'get', {
                 'id': id
             })
             .then((response) => {
-                console.log(response)
                 glue_dispatch_response_event(response)
-                model_object = new GlueModelObject(this.decoded_unique_name);
-                model_object.set_properties(response.data.simple_fields)
+                model_object = new GlueModelObject(this.glue_unique_name);
+                let glue_query_set = JSON.parse(response.data)
+                model_object.set_properties(glue_query_set[0])
                 return model_object
             });
     }
 
     async method(id, method, kwargs = {}) {
         // Todo: Should query sets be able to call methods?
         let data = {
             'id': id,
             'method': method,
             'kwargs': kwargs,
         }
-
         return await glue_ajax_request(
-            this.glue_unique_name,
+            this.glue_encoded_unique_name,
             'method',
             data
         ).then((response) => {
             console.log(response)
             glue_dispatch_response_event(response)
-            return response.data.method_return
+            return JSON.parse(response.data).method_return
         })
     }
 
+
     update(query_model_object, field = null) {
         // Todo: Update on queryset should take fields and update all the objects fields to that value.
         // Todo: Should only be able to update fields on the main table.
         // Todo: Be aware that it does not call the save method.
 
         let data = {}
 
@@ -112,15 +114,15 @@
             data[field] = query_model_object[field]
         } else {
             for (let key in query_model_object.context_data.fields) {
                 data[key] = query_model_object[key]
             }
         }
         glue_ajax_request(
-            this.glue_unique_name,
+            this.glue_encoded_unique_name,
             'update',
             data
         ).then((response) => {
             console.log(response)
             glue_dispatch_response_event(response)
         })
     }
```

### Comparing `django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_template.js` & `django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_template.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,46 +1,54 @@
 class GlueTemplate {
     constructor(unique_name, shared_context_data = {}) {
         this.unique_name = encodeUniqueName(unique_name)
         this.shared_context_data = shared_context_data
         window.glue_keep_live.add_unique_name(this.unique_name)
     }
 
-    //Todo: Make sure there is not change of injection attack and get understanding of context data in templates
-
+    //Todo: Make sure there is not chance of injection attack and get understanding of context data in templates
     async _render(context_data = {}) {
-        return glue_ajax_request(this.unique_name, 'get', {
-            ...context_data,
-            ...this.shared_context_data
-        }, 'text/html');
+        let combined_context_data = Object.assign({}, this.shared_context_data, context_data);
+
+
+        return await glue_ajax_request(
+            this.unique_name,
+            'get', {
+                'context_data': combined_context_data
+            }
+        ).then((response) => {
+            console.log(response)
+            glue_dispatch_response_event(response)
+            return response.data.rendered_template
+        })
     }
 
     render_inner(target_element, context_data = {}) {
         this._render(context_data).then((response) => {
             glue_dispatch_response_event(response)
-            return response.text()
+            return response
         }).then((html) => {
             target_element.innerHTML = html
         })
 
     }
 
     render_insert_adjacent(target_element, context_data = {}, position = 'beforeend') {
         this._render(context_data).then((response) => {
-            return response.text()
+            return response
         }).then((html) => {
             target_element.insertAdjacentHTML(position, html)
         })
 
     }
 
     render_outer(target_element, context_data = {}) {
         this._render(context_data).then((response) => {
             glue_dispatch_response_event(response)
-            return response.text()
+            return response
         }).then((html) => {
             target_element.outerHTML = html
         })
 
     }
 
 }
```

### Comparing `django_glue-0.5.2.3/django_glue/static/django_glue/js/django_glue_view.js` & `django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_view.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,16 @@
 class GlueView {
     constructor(url, shared_parameters = {}) {
-        this.url = url
+        // Need to send the current view path to encode the glue data on the server.
+        let config_url = new URL(window.location.origin + url)
+        config_url.searchParams.append('glue_encode_path', window.location.pathname)
+
+        this.url = config_url.pathname + config_url.search
         this.shared_parameters = shared_parameters
+
     }
 
     async _render(parameters = {}, method = 'POST', headers = {}) {
         const request_options = {
             method: method,
             headers: {
                 ...headers,
```

### Comparing `django_glue-0.5.2.3/django_glue/templates/django_glue/django_glue.html` & `django_glue-0.5.3/django_glue/templates/django_glue/django_glue.html`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.2.3/django_glue/templatetags/django_glue.py` & `django_glue-0.5.3/django_glue/templatetags/django_glue.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.2.3/django_glue/views.py` & `django_glue-0.5.3/django_glue/views.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import json
 import logging
 
 from django.http import JsonResponse
 from django.views.decorators.http import require_http_methods
 
-from django_glue.core.decorators import require_content_types, require_query_method
-from django_glue.data_classes import GlueBodyData
-from django_glue.handlers import GlueRequestHandler
-from django_glue.responses import generate_json_404_response
-from django_glue.sessions import GlueKeepLiveSession, GlueSession
+from django_glue.core.decorators import require_content_types
+from django_glue.handler.body_data import GlueBodyData
+from django_glue.handler.utils import process_glue_request
+from django_glue.response.responses import generate_json_404_response
+from django_glue.session import GlueKeepLiveSession, GlueSession
 
 
 @require_http_methods(["POST"])
 @require_content_types('application/json', 'text/html')
 def glue_data_ajax_handler_view(request):
     glue_session = GlueSession(request)
     glue_body_data = GlueBodyData(request.body)
 
-    if glue_session.has_unique_name(glue_body_data.unique_name):
+    if glue_body_data.unique_name in glue_session.session:
         logging.warning(request.body.decode('utf-8'))
-        return GlueRequestHandler(glue_session, glue_body_data).process_response()
+        return process_glue_request(glue_session, glue_body_data).to_django_json_response()
     else:
         return generate_json_404_response()
 
 
 def glue_keep_live_handler_view(request):
     data = json.loads(request.body.decode('utf-8'))
     unique_names = data['unique_names']
```

### Comparing `django_glue-0.5.2.3/django_glue.egg-info/PKG-INFO` & `django_glue-0.5.3/django_glue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-glue
-Version: 0.5.2.3
+Version: 0.5.3
 Summary: Industrial Strength Glue for Django Backends and Frontends!
 Home-page: https://github.com/stratusadv/django-glue
 Author: Nathan Johnson, Austin Sauer & Wesley Howery
 Author-email: info@stratusadv.com
 License: MIT
 Keywords: glue,django,backend,frontend,javascript,active server pages
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django_glue-0.5.2.3/setup.py` & `django_glue-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.2.3/tests/forms.py` & `django_glue-0.5.3/tests/forms.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.2.3/tests/manage.py` & `django_glue-0.5.3/tests/manage.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.2.3/tests/migrations/0001_initial.py` & `django_glue-0.5.3/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.2.3/tests/migrations/0002_bigtestmodel_foreign_key_alter_testmodel_birth_date.py` & `django_glue-0.5.3/tests/migrations/0002_bigtestmodel_foreign_key_alter_testmodel_birth_date.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.2.3/tests/models.py` & `django_glue-0.5.3/tests/models.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.2.3/tests/settings.py` & `django_glue-0.5.3/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.2.3/tests/test_views.py` & `django_glue-0.5.3/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.2.3/tests/urls.py` & `django_glue-0.5.3/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.2.3/tests/utils.py` & `django_glue-0.5.3/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.2.3/tests/views.py` & `django_glue-0.5.3/tests/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,16 +133,22 @@
 def view_view(request):
     return TemplateResponse(request, 'page/view_page.html')
 
 
 def view_card_view(request):
     test_model_object = generate_randomized_test_model()
 
-    glue_model(request, 'test_model_view_card', test_model_object, 'delete', exclude=('birth_date', 'anniversary_datetime'),
-             methods=['is_lighter_than', 'get_full_name'])
+    glue_model(
+        request=request,
+        unique_name='test_model_view_card',
+        target=test_model_object,
+        access='delete',
+        exclude=('birth_date', 'anniversary_datetime'),
+        methods=['is_lighter_than', 'get_full_name']
+    )
 
     return TemplateResponse(request, 'card/view_card.html')
 
 
 def template_view(request):
     glue_template(request, 'button_1', 'element/button_element.html')
```


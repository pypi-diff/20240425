# Comparing `tmp/wagtail_fedit-1.5.4rc8.tar.gz` & `tmp/wagtail_fedit-1.5.4rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.5.4rc8.tar", last modified: Tue Apr 23 20:18:30 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.5.4rc9.tar", last modified: Tue Apr 23 20:50:48 2024, max compression
```

## Comparing `wagtail_fedit-1.5.4rc8.tar` & `wagtail_fedit-1.5.4rc9.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.169221 wagtail_fedit-1.5.4rc8/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc8/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc8/MANIFEST.in
--rw-rw-rw-   0        0        0    21651 2024-04-23 20:18:30.169221 wagtail_fedit-1.5.4rc8/PKG-INFO
--rw-rw-rw-   0        0        0    20450 2024-04-23 11:23:03.000000 wagtail_fedit-1.5.4rc8/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc8/pyproject.toml
--rw-rw-rw-   0        0        0     1189 2024-04-23 20:18:30.183225 wagtail_fedit-1.5.4rc8/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.030471 wagtail_fedit-1.5.4rc8/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.069456 wagtail_fedit-1.5.4rc8/wagtail_fedit/adapters/
--rw-rw-rw-   0        0        0      532 2024-04-22 21:01:35.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/adapters/__init__.py
--rw-rw-rw-   0        0        0    14330 2024-04-23 15:34:38.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/adapters/base.py
--rw-rw-rw-   0        0        0     6524 2024-04-23 20:05:52.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/adapters/block.py
--rw-rw-rw-   0        0        0     8652 2024-04-23 18:12:26.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/adapters/field.py
--rw-rw-rw-   0        0        0     2671 2024-04-22 20:52:19.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/adapters/funcs.py
--rw-rw-rw-   0        0        0     2739 2024-04-23 14:30:53.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/adapters/misc.py
--rw-rw-rw-   0        0        0     4632 2024-04-23 15:46:14.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/adapters/models.py
--rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/adapters/registry.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.072452 wagtail_fedit-1.5.4rc8/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0      215 2024-04-23 13:02:23.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     3269 2024-04-23 13:28:56.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     4617 2024-04-21 02:08:33.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:29.988183 wagtail_fedit-1.5.4rc8/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:29.989184 wagtail_fedit-1.5.4rc8/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.074451 wagtail_fedit-1.5.4rc8/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7262 2024-04-23 15:50:58.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    13018 2024-04-23 15:50:49.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.075450 wagtail_fedit-1.5.4rc8/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.076451 wagtail_fedit-1.5.4rc8/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/models.py
--rw-rw-rw-   0        0        0     1585 2024-04-23 15:56:07.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:29.991428 wagtail_fedit-1.5.4rc8/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:29.992453 wagtail_fedit-1.5.4rc8/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.078450 wagtail_fedit-1.5.4rc8/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     5791 2024-04-23 18:28:37.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.079450 wagtail_fedit-1.5.4rc8/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    22454 2024-04-23 18:08:58.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:29.992453 wagtail_fedit-1.5.4rc8/wagtail_fedit/static/wagtail_fedit/vendor/
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.083452 wagtail_fedit-1.5.4rc8/wagtail_fedit/static/wagtail_fedit/vendor/tippy/
--rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/static/wagtail_fedit/vendor/tippy/LICENSE
--rw-rw-rw-   0        0        0    20122 2024-04-23 14:51:23.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/static/wagtail_fedit/vendor/tippy/popper.min.js
--rw-rw-rw-   0        0        0    25717 2024-04-23 14:51:31.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/static/wagtail_fedit/vendor/tippy/tippy-bundle.min.js
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:29.993451 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.085454 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/
--rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.087454 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.089451 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      929 2024-04-23 15:23:24.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
--rw-rw-rw-   0        0        0      991 2024-04-23 15:27:54.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
--rw-rw-rw-   0        0        0      571 2024-04-23 17:34:21.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.096454 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0      266 2024-04-21 21:15:09.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
--rw-rw-rw-   0        0        0      265 2024-04-21 21:23:24.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
--rw-rw-rw-   0        0        0      555 2024-04-21 21:13:45.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
--rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
--rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
--rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/editor/field.html
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.104452 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.106452 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.108451 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.109450 wagtail_fedit-1.5.4rc8/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.111451 wagtail_fedit-1.5.4rc8/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    12928 2024-04-23 20:05:43.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0     9725 2024-04-23 20:13:22.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.113452 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.119456 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/apps.py
--rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/context_processors.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.124220 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      509 2024-04-21 18:41:55.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/migrations/0002_basicmodel_related_field.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     6047 2024-04-23 13:09:46.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.132233 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     8475 2024-04-23 13:35:29.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0    22637 2024-04-23 12:36:52.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/tests/test_adapters.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     4865 2024-04-23 14:23:09.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/tests/test_model_edit.py
--rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.139220 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     2220 2024-04-23 14:21:34.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0     1196 2024-04-23 17:25:08.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    17176 2024-04-23 20:17:01.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.143217 wagtail_fedit-1.5.4rc8/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      215 2024-04-23 17:24:50.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     7388 2024-04-23 20:03:50.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/views/adapters.py
--rw-rw-rw-   0        0        0    17563 2024-04-21 20:25:17.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     1923 2024-04-21 20:29:01.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.168221 wagtail_fedit-1.5.4rc8/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0     2857 2024-04-23 15:56:51.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/wagtail_hooks/adapter_hooks.py
--rw-rw-rw-   0        0        0      328 2024-04-21 16:44:33.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/wagtail_hooks/adapter_registry.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     7637 2024-04-23 20:17:24.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:18:30.059473 wagtail_fedit-1.5.4rc8/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0    21651 2024-04-23 20:18:29.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4521 2024-04-23 20:18:29.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 20:18:29.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-23 20:18:29.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-23 20:18:29.000000 wagtail_fedit-1.5.4rc8/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.263680 wagtail_fedit-1.5.4rc9/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc9/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc9/MANIFEST.in
+-rw-rw-rw-   0        0        0    21651 2024-04-23 20:50:48.263680 wagtail_fedit-1.5.4rc9/PKG-INFO
+-rw-rw-rw-   0        0        0    20450 2024-04-23 11:23:03.000000 wagtail_fedit-1.5.4rc9/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc9/pyproject.toml
+-rw-rw-rw-   0        0        0     1189 2024-04-23 20:50:48.274174 wagtail_fedit-1.5.4rc9/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.075351 wagtail_fedit-1.5.4rc9/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.126731 wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      532 2024-04-22 21:01:35.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0    14330 2024-04-23 15:34:38.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/base.py
+-rw-rw-rw-   0        0        0     6524 2024-04-23 20:05:52.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/block.py
+-rw-rw-rw-   0        0        0     8652 2024-04-23 18:12:26.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     2671 2024-04-22 20:52:19.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/funcs.py
+-rw-rw-rw-   0        0        0     2739 2024-04-23 14:30:53.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/misc.py
+-rw-rw-rw-   0        0        0     4632 2024-04-23 15:46:14.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/models.py
+-rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/registry.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.132731 wagtail_fedit-1.5.4rc9/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0      215 2024-04-23 13:02:23.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     3269 2024-04-23 13:28:56.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     4617 2024-04-21 02:08:33.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.034404 wagtail_fedit-1.5.4rc9/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.034404 wagtail_fedit-1.5.4rc9/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.135730 wagtail_fedit-1.5.4rc9/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7262 2024-04-23 15:50:58.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    13018 2024-04-23 15:50:49.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.138732 wagtail_fedit-1.5.4rc9/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.139731 wagtail_fedit-1.5.4rc9/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/models.py
+-rw-rw-rw-   0        0        0     1585 2024-04-23 15:56:07.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.037413 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.039407 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.144728 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     5791 2024-04-23 18:28:37.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.146728 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    22454 2024-04-23 18:08:58.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.039407 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/vendor/
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.151729 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/vendor/tippy/
+-rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/vendor/tippy/LICENSE
+-rw-rw-rw-   0        0        0    20122 2024-04-23 14:51:23.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/vendor/tippy/popper.min.js
+-rw-rw-rw-   0        0        0    25717 2024-04-23 14:51:31.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/vendor/tippy/tippy-bundle.min.js
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.040651 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.154733 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/
+-rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.155728 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.158728 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      929 2024-04-23 15:23:24.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
+-rw-rw-rw-   0        0        0      991 2024-04-23 15:27:54.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      571 2024-04-23 17:34:21.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.170738 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      266 2024-04-21 21:15:09.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
+-rw-rw-rw-   0        0        0      265 2024-04-21 21:23:24.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
+-rw-rw-rw-   0        0        0      555 2024-04-21 21:13:45.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
+-rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
+-rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.177728 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.179728 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.182729 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.200749 wagtail_fedit-1.5.4rc9/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.203736 wagtail_fedit-1.5.4rc9/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    12928 2024-04-23 20:05:43.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10181 2024-04-23 20:50:38.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.207729 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.213728 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/apps.py
+-rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/context_processors.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.217728 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      509 2024-04-21 18:41:55.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/migrations/0002_basicmodel_related_field.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     6047 2024-04-23 13:09:46.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.231724 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     8475 2024-04-23 13:35:29.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0    22637 2024-04-23 12:36:52.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     4865 2024-04-23 14:23:09.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_model_edit.py
+-rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.240090 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     2220 2024-04-23 14:21:34.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0     1196 2024-04-23 17:25:08.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    17176 2024-04-23 20:17:01.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.246416 wagtail_fedit-1.5.4rc9/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      215 2024-04-23 17:24:50.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     7388 2024-04-23 20:03:50.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17563 2024-04-21 20:25:17.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     1923 2024-04-21 20:29:01.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.262678 wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0     2857 2024-04-23 15:56:51.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/adapter_hooks.py
+-rw-rw-rw-   0        0        0      328 2024-04-21 16:44:33.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/adapter_registry.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     7637 2024-04-23 20:17:24.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.110357 wagtail_fedit-1.5.4rc9/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0    21651 2024-04-23 20:50:47.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4521 2024-04-23 20:50:48.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 20:50:47.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-23 20:50:47.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-23 20:50:47.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.5.4rc8/LICENSE` & `wagtail_fedit-1.5.4rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/PKG-INFO` & `wagtail_fedit-1.5.4rc9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.5.4rc8
+Version: 1.5.4rc9
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.4rc8 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.4rc9 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
```

### Comparing `wagtail_fedit-1.5.4rc8/README.md` & `wagtail_fedit-1.5.4rc9/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/setup.cfg` & `wagtail_fedit-1.5.4rc9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 352e  ..version = 1.5.
-00000030: 3472 6338 0d0a 6465 7363 7269 7074 696f  4rc8..descriptio
+00000030: 3472 6339 0d0a 6465 7363 7269 7074 696f  4rc9..descriptio
 00000040: 6e20 3d20 4672 6f6e 7465 6e64 2065 6469  n = Frontend edi
 00000050: 7469 6e67 2066 6f72 2079 6f75 7220 5761  ting for your Wa
 00000060: 6774 6169 6c20 7369 7465 0d0a 6c6f 6e67  gtail site..long
 00000070: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000080: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000a0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type =
```

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/adapters/__init__.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/adapters/base.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/adapters/block.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/block.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/adapters/field.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/field.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/adapters/funcs.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/funcs.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/adapters/misc.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/misc.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/adapters/models.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/adapters/registry.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/hooks.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/models.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/settings.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/static/wagtail_fedit/vendor/tippy/LICENSE` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/vendor/tippy/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/static/wagtail_fedit/vendor/tippy/popper.min.js` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/vendor/tippy/popper.min.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/static/wagtail_fedit/vendor/tippy/tippy-bundle.min.js` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/vendor/tippy/tippy-bundle.min.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/templatetags/fedit.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,25 +12,30 @@
 from django.http import HttpRequest
 from django.utils.html import escape
 from django.utils.safestring import mark_safe
 from django.urls import reverse
 from django.core import signing
 
 from wagtail import hooks
+from wagtail.models import (
+    Page,
+    PAGE_TEMPLATE_VAR,
+)
 
 import warnings
 
 from ..adapters import (
     adapter_registry,
     RegistryLookUpError,
     BaseAdapter,
     AdapterError,
 )
 from ..utils import (
     wrap_adapter,
+    with_userbar_model,
     _can_edit,
     FEDIT_PREVIEW_VAR,
     TEMPLATE_TAG_NAME,
 )
 from ..hooks import (
     REGISTER_CSS,
     REGISTER_JS,
@@ -262,14 +267,21 @@
     attrs = " ".join(s)
 
     if not wrapping:
         return mark_safe(attrs)
     
     return mark_safe(f"<span {attrs}>{wrapping}</span>")
 
+@register.simple_tag(takes_context=True, name="fedit_userbar")
+def do_with_userbar_model(context, model: Any) -> str:
+    if "request" in context:
+        context["request"] = with_userbar_model(context["request"], model)
+    if PAGE_TEMPLATE_VAR in context and context[PAGE_TEMPLATE_VAR] != model:
+        context[PAGE_TEMPLATE_VAR] = model
+    return ""
 
 def get_kwargs(parser: Parser, tokens: list[str], kwarg_list: list[str] = None, absolute_tokens: list[str] = None, optional_tokens: dict[str, Any] = None) -> dict:
     had_kwargs = False
     kwargs = {}
 
     if not kwarg_list:
         kwarg_list = tuple()
```

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/tests/test_adapters.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/tests/test_model_edit.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_model_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/urls.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/utils.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/views/adapters.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/views/adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/wagtail_hooks/adapter_hooks.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/adapter_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.5.4rc9/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.5.4rc8
+Version: 1.5.4rc9
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.5.4rc8 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.5.4rc9 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
```

### Comparing `wagtail_fedit-1.5.4rc8/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.5.4rc9/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*


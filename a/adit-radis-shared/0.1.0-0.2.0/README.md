# Comparing `tmp/adit_radis_shared-0.1.0.tar.gz` & `tmp/adit_radis_shared-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adit_radis_shared-0.1.0.tar", max compression
+gzip compressed data, was "adit_radis_shared-0.2.0.tar", max compression
```

## Comparing `adit_radis_shared-0.1.0.tar` & `adit_radis_shared-0.2.0.tar`

### file list

```diff
@@ -1,160 +1,160 @@
--rw-r--r--   0        0        0    34862 2024-04-23 12:13:45.000000 adit_radis_shared-0.1.0/LICENSE
--rw-r--r--   0        0        0      182 2024-04-23 12:13:45.000000 adit_radis_shared-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/__init__.py
--rw-r--r--   0        0        0      826 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/admin.py
--rw-r--r--   0        0        0      109 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/apps.py
--rw-r--r--   0        0        0     1250 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/backends.py
--rw-r--r--   0        0        0     1443 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/factories.py
--rw-r--r--   0        0        0     2322 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/forms.py
--rw-r--r--   0        0        0      698 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/middlewares.py
--rw-r--r--   0        0        0     3079 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/migrations/0001_initial.py
--rw-r--r--   0        0        0      431 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/migrations/0002_alter_user_id.py
--rw-r--r--   0        0        0      368 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/migrations/0003_rename_misc_settings_user_preferences.py
--rw-r--r--   0        0        0      407 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/migrations/0004_alter_user_preferences.py
--rw-r--r--   0        0        0      979 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/migrations/0005_institute.py
--rw-r--r--   0        0        0      639 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/migrations/0006_user_active_group.py
--rw-r--r--   0        0        0     1323 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/migrations/0007_convert_institutes_to_groups.py
--rw-r--r--   0        0        0      340 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/migrations/0008_remove_institute_users.py
--rw-r--r--   0        0        0      302 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/migrations/0009_delete_institute.py
--rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/migrations/__init__.py
--rw-r--r--   0        0        0      886 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/models.py
--rw-r--r--   0        0        0      723 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/templates/accounts/_active_group_selector.html
--rw-r--r--   0        0        0       42 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/templates/accounts/accounts_layout.html
--rw-r--r--   0        0        0     1580 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/templates/accounts/profile.html
--rw-r--r--   0        0        0      205 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/tests/integration/conftest.py
--rw-r--r--   0        0        0      317 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/tests/integration/test_login.py
--rw-r--r--   0        0        0     1201 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/tests/test_migrations.py
--rw-r--r--   0        0        0      329 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/urls.py
--rw-r--r--   0        0        0     1136 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/accounts/views.py
--rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/__init__.py
--rw-r--r--   0        0        0      118 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/admin.py
--rw-r--r--   0        0        0      105 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/apps.py
--rw-r--r--   0        0        0     1383 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/decorators.py
--rw-r--r--   0        0        0      296 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/factories.py
--rw-r--r--   0        0        0     3285 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/forms.py
--rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/management/base/__init__.py
--rw-r--r--   0        0        0     1427 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/management/base/celery_beat.py
--rw-r--r--   0        0        0     1762 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/management/base/celery_worker.py
--rw-r--r--   0        0        0      889 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/management/base/hard_reset_migrations.py
--rw-r--r--   0        0        0     4889 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/management/base/server_command.py
--rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/management/commands/__init__.py
--rw-r--r--   0        0        0     1267 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/management/commands/create_admin.py
--rw-r--r--   0        0        0      558 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/management/commands/example_async_server.py
--rw-r--r--   0        0        0      536 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/management/commands/example_server.py
--rw-r--r--   0        0        0     3664 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/management/commands/generate_cert.py
--rw-r--r--   0        0        0      743 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/management/commands/send_test_mail.py
--rw-r--r--   0        0        0     2144 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/middlewares.py
--rw-r--r--   0        0        0      977 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/migrations/0001_initial.py
--rw-r--r--   0        0        0      688 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/migrations/0002_update_or_create_site.py
--rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/migrations/__init__.py
--rw-r--r--   0        0        0     4865 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/mixins.py
--rw-r--r--   0        0        0     2449 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/models.py
--rw-r--r--   0        0        0     1355 2024-04-23 21:50:39.602820 adit_radis_shared-0.1.0/adit_radis_shared/common/site.py
--rw-r--r--   0        0        0     2651 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/static/common/common.css
--rw-r--r--   0        0        0     5574 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/static/common/common.js
--rw-r--r--   0        0        0     2958 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/static/common/theme.js
--rw-r--r--   0        0        0    11306 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/static/vendor/alpine-morph.js
--rw-r--r--   0        0        0   108425 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/static/vendor/alpine.js
--rw-r--r--   0        0        0  1098145 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/static/vendor/bootstrap-icons.svg
--rw-r--r--   0        0        0   207819 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/static/vendor/bootstrap.bundle.js
--rw-r--r--   0        0        0   444579 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/static/vendor/bootstrap.bundle.js.map
--rw-r--r--   0        0        0   281758 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/static/vendor/bootstrap.css
--rw-r--r--   0        0        0      532 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/static/vendor/htmx-alpine-morph.js
--rw-r--r--   0        0        0    13641 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/static/vendor/htmx-ws.js
--rw-r--r--   0        0        0   162018 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/static/vendor/htmx.js
--rw-r--r--   0        0        0      504 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/_alert_icons.html
--rw-r--r--   0        0        0      196 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/_bootstrap_icon.html
--rw-r--r--   0        0        0      537 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/_filter_set_field.html
--rw-r--r--   0        0        0      276 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/_footer.html
--rw-r--r--   0        0        0      907 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/_messages_panel.html
--rw-r--r--   0        0        0      789 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/_navbar.html
--rw-r--r--   0        0        0      616 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/_navbar_actions.html
--rw-r--r--   0        0        0      471 2024-04-23 21:51:07.430796 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/_navbar_links.html
--rw-r--r--   0        0        0     2141 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/_navbar_theme_switcher.html
--rw-r--r--   0        0        0     1342 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/_navbar_user_manager.html
--rw-r--r--   0        0        0     1276 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/_pagination.html
--rw-r--r--   0        0        0      407 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/_theme_icons.html
--rw-r--r--   0        0        0     1283 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/_toasts_panel.html
--rw-r--r--   0        0        0      482 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/broadcast.html
--rw-r--r--   0        0        0     3406 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/common_layout.html
--rw-r--r--   0        0        0      359 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/maintenance.html
--rw-r--r--   0        0        0      327 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/section_locked.html
--rw-r--r--   0        0        0      270 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/README.md
--rwxr-xr-x   0        0        0      606 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/activate.html
--rwxr-xr-x   0        0        0      695 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/activation_complete.html
--rw-r--r--   0        0        0      743 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/activation_complete_admin_pending.html
--rw-r--r--   0        0        0     2970 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/activation_email.html
--rw-r--r--   0        0        0     2088 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/activation_email.txt
--rw-r--r--   0        0        0     1083 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/activation_email_subject.txt
--rw-r--r--   0        0        0      478 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/admin_approve.html
--rw-r--r--   0        0        0     1207 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/admin_approve_complete.html
--rw-r--r--   0        0        0      928 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/admin_approve_complete_email.html
--rw-r--r--   0        0        0      507 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/admin_approve_complete_email.txt
--rw-r--r--   0        0        0      943 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/admin_approve_complete_email_subject.txt
--rw-r--r--   0        0        0     2855 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/admin_approve_email.html
--rw-r--r--   0        0        0      459 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/admin_approve_email.txt
--rw-r--r--   0        0        0       76 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/admin_approve_email_subject.txt
--rwxr-xr-x   0        0        0     2310 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/login.html
--rwxr-xr-x   0        0        0      449 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/logout.html
--rwxr-xr-x   0        0        0      381 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/password_change_done.html
--rwxr-xr-x   0        0        0      631 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/password_change_form.html
--rwxr-xr-x   0        0        0      503 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/password_reset_complete.html
--rwxr-xr-x   0        0        0      960 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/password_reset_confirm.html
--rwxr-xr-x   0        0        0      536 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/password_reset_done.html
--rwxr-xr-x   0        0        0     1007 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/password_reset_email.html
--rwxr-xr-x   0        0        0      774 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/password_reset_form.html
--rwxr-xr-x   0        0        0       46 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/registration_base.html
--rwxr-xr-x   0        0        0      384 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/registration_closed.html
--rwxr-xr-x   0        0        0      671 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/registration_complete.html
--rwxr-xr-x   0        0        0      791 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/registration_form.html
--rw-r--r--   0        0        0      713 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/resend_activation_complete.html
--rw-r--r--   0        0        0      951 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/resend_activation_form.html
--rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templatetags/__init__.py
--rw-r--r--   0        0        0     1928 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/templatetags/common_extras.py
--rw-r--r--   0        0        0      445 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/types.py
--rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/utils/__init__.py
--rw-r--r--   0        0        0      451 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/utils/async_utils.py
--rw-r--r--   0        0        0     1157 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/utils/auth_utils.py
--rw-r--r--   0        0        0      818 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/utils/debounce.py
--rw-r--r--   0        0        0      627 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/utils/htmx_triggers.py
--rw-r--r--   0        0        0     1236 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/utils/mail.py
--rw-r--r--   0        0        0     1832 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/utils/testing.py
--rw-r--r--   0        0        0     3977 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/common/views.py
--rw-r--r--   0        0        0     1697 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/conftest.py
--rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/__init__.py
--rw-r--r--   0        0        0      390 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/admin.py
--rw-r--r--   0        0        0      132 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/apps.py
--rw-r--r--   0        0        0     2718 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/auth.py
--rw-r--r--   0        0        0      715 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/factories.py
--rw-r--r--   0        0        0     1828 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/forms.py
--rw-r--r--   0        0        0     2529 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/migrations/0001_initial.py
--rw-r--r--   0        0        0      596 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/migrations/0002_token_fraction_alter_token_token_string.py
--rw-r--r--   0        0        0      432 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/migrations/0003_alter_token_client.py
--rw-r--r--   0        0        0      386 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/migrations/0004_rename_token_string_token_token_hashed.py
--rw-r--r--   0        0        0      795 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/migrations/0005_alter_token_options_remove_token_expires_and_more.py
--rw-r--r--   0        0        0      411 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/migrations/0006_rename_expiry_time_token_expires.py
--rw-r--r--   0        0        0      426 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/migrations/0007_alter_token_last_used.py
--rw-r--r--   0        0        0      420 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/migrations/0008_alter_token_token_hashed.py
--rw-r--r--   0        0        0      768 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/migrations/0009_rename_author_token_owner_alter_token_client_and_more.py
--rw-r--r--   0        0        0      606 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/migrations/0010_alter_token_unique_together_and_more.py
--rw-r--r--   0        0        0      818 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/migrations/0011_delete_tokensettings_alter_token_client_and_more.py
--rw-r--r--   0        0        0      532 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/migrations/0012_remove_token_unique_client_per_user_and_more.py
--rw-r--r--   0        0        0      441 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/migrations/0013_alter_token_description.py
--rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/migrations/__init__.py
--rw-r--r--   0        0        0     1846 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/models.py
--rw-r--r--   0        0        0      423 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/static/token_authentication/token_authentication.js
--rw-r--r--   0        0        0      689 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/templates/token_authentication/_token_authentication_help.html
--rw-r--r--   0        0        0      223 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/templates/token_authentication/token_authentication_layout.html
--rw-r--r--   0        0        0     3690 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/templates/token_authentication/token_dashboard.html
--rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/tests/__init__.py
--rw-r--r--   0        0        0      463 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/tests/conftest.py
--rw-r--r--   0        0        0      205 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/tests/integration/conftest.py
--rw-r--r--   0        0        0     1666 2024-04-23 22:08:26.985907 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/tests/integration/test_token_authentication.py
--rw-r--r--   0        0        0      646 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/urls.py
--rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/utils/__init__.py
--rw-r--r--   0        0        0      508 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/utils/crypto.py
--rw-r--r--   0        0        0     2619 2024-04-23 12:13:46.000000 adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/views.py
--rw-r--r--   0        0        0     3064 2024-04-23 22:27:55.868909 adit_radis_shared-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1702 1970-01-01 00:00:00.000000 adit_radis_shared-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34862 2024-04-23 12:13:45.000000 adit_radis_shared-0.2.0/LICENSE
+-rw-r--r--   0        0        0      557 2024-04-23 22:42:20.000000 adit_radis_shared-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/__init__.py
+-rw-r--r--   0        0        0      826 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/admin.py
+-rw-r--r--   0        0        0      109 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/apps.py
+-rw-r--r--   0        0        0     1250 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/backends.py
+-rw-r--r--   0        0        0     1443 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/factories.py
+-rw-r--r--   0        0        0     2322 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/forms.py
+-rw-r--r--   0        0        0      698 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/middlewares.py
+-rw-r--r--   0        0        0     3079 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/migrations/0001_initial.py
+-rw-r--r--   0        0        0      431 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/migrations/0002_alter_user_id.py
+-rw-r--r--   0        0        0      368 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/migrations/0003_rename_misc_settings_user_preferences.py
+-rw-r--r--   0        0        0      407 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/migrations/0004_alter_user_preferences.py
+-rw-r--r--   0        0        0      979 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/migrations/0005_institute.py
+-rw-r--r--   0        0        0      639 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/migrations/0006_user_active_group.py
+-rw-r--r--   0        0        0     1323 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/migrations/0007_convert_institutes_to_groups.py
+-rw-r--r--   0        0        0      340 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/migrations/0008_remove_institute_users.py
+-rw-r--r--   0        0        0      302 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/migrations/0009_delete_institute.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/migrations/__init__.py
+-rw-r--r--   0        0        0      886 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/models.py
+-rw-r--r--   0        0        0      723 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/templates/accounts/_active_group_selector.html
+-rw-r--r--   0        0        0       42 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/templates/accounts/accounts_layout.html
+-rw-r--r--   0        0        0     1580 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/templates/accounts/profile.html
+-rw-r--r--   0        0        0      205 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/tests/integration/conftest.py
+-rw-r--r--   0        0        0      317 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/tests/integration/test_login.py
+-rw-r--r--   0        0        0     1201 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/tests/test_migrations.py
+-rw-r--r--   0        0        0      329 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/urls.py
+-rw-r--r--   0        0        0     1136 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/accounts/views.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/__init__.py
+-rw-r--r--   0        0        0      118 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/admin.py
+-rw-r--r--   0        0        0      105 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/apps.py
+-rw-r--r--   0        0        0     1383 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/decorators.py
+-rw-r--r--   0        0        0      296 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/factories.py
+-rw-r--r--   0        0        0     3285 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/forms.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/management/base/__init__.py
+-rw-r--r--   0        0        0     1427 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/management/base/celery_beat.py
+-rw-r--r--   0        0        0     1762 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/management/base/celery_worker.py
+-rw-r--r--   0        0        0      889 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/management/base/hard_reset_migrations.py
+-rw-r--r--   0        0        0     4889 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/management/base/server_command.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/management/commands/__init__.py
+-rw-r--r--   0        0        0     1267 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/management/commands/create_admin.py
+-rw-r--r--   0        0        0      558 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/management/commands/example_async_server.py
+-rw-r--r--   0        0        0      536 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/management/commands/example_server.py
+-rw-r--r--   0        0        0     3664 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/management/commands/generate_cert.py
+-rw-r--r--   0        0        0      743 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/management/commands/send_test_mail.py
+-rw-r--r--   0        0        0     2144 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/middlewares.py
+-rw-r--r--   0        0        0      977 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/migrations/0001_initial.py
+-rw-r--r--   0        0        0      688 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/migrations/0002_update_or_create_site.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/migrations/__init__.py
+-rw-r--r--   0        0        0     4865 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/mixins.py
+-rw-r--r--   0        0        0     2449 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/models.py
+-rw-r--r--   0        0        0     1333 2024-04-24 19:55:06.902493 adit_radis_shared-0.2.0/adit_radis_shared/common/site.py
+-rw-r--r--   0        0        0     2651 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/static/common/common.css
+-rw-r--r--   0        0        0     5574 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/static/common/common.js
+-rw-r--r--   0        0        0     2958 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/static/common/theme.js
+-rw-r--r--   0        0        0    11306 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/static/vendor/alpine-morph.js
+-rw-r--r--   0        0        0   108425 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/static/vendor/alpine.js
+-rw-r--r--   0        0        0  1098145 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/static/vendor/bootstrap-icons.svg
+-rw-r--r--   0        0        0   207819 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/static/vendor/bootstrap.bundle.js
+-rw-r--r--   0        0        0   444579 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/static/vendor/bootstrap.bundle.js.map
+-rw-r--r--   0        0        0   281758 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/static/vendor/bootstrap.css
+-rw-r--r--   0        0        0      532 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/static/vendor/htmx-alpine-morph.js
+-rw-r--r--   0        0        0    13641 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/static/vendor/htmx-ws.js
+-rw-r--r--   0        0        0   162018 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/static/vendor/htmx.js
+-rw-r--r--   0        0        0      504 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/_alert_icons.html
+-rw-r--r--   0        0        0      196 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/_bootstrap_icon.html
+-rw-r--r--   0        0        0      537 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/_filter_set_field.html
+-rw-r--r--   0        0        0      276 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/_footer.html
+-rw-r--r--   0        0        0      907 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/_messages_panel.html
+-rw-r--r--   0        0        0      789 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/_navbar.html
+-rw-r--r--   0        0        0      616 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/_navbar_actions.html
+-rw-r--r--   0        0        0      471 2024-04-23 21:51:07.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/_navbar_links.html
+-rw-r--r--   0        0        0     2141 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/_navbar_theme_switcher.html
+-rw-r--r--   0        0        0     1342 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/_navbar_user_manager.html
+-rw-r--r--   0        0        0     1276 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/_pagination.html
+-rw-r--r--   0        0        0      407 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/_theme_icons.html
+-rw-r--r--   0        0        0     1283 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/_toasts_panel.html
+-rw-r--r--   0        0        0      482 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/broadcast.html
+-rw-r--r--   0        0        0     3406 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/common_layout.html
+-rw-r--r--   0        0        0      359 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/maintenance.html
+-rw-r--r--   0        0        0      327 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/section_locked.html
+-rw-r--r--   0        0        0      270 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/README.md
+-rwxr-xr-x   0        0        0      606 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/activate.html
+-rwxr-xr-x   0        0        0      695 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/activation_complete.html
+-rw-r--r--   0        0        0      743 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/activation_complete_admin_pending.html
+-rw-r--r--   0        0        0     2970 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/activation_email.html
+-rw-r--r--   0        0        0     2088 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/activation_email.txt
+-rw-r--r--   0        0        0     1083 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/activation_email_subject.txt
+-rw-r--r--   0        0        0      478 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/admin_approve.html
+-rw-r--r--   0        0        0     1207 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/admin_approve_complete.html
+-rw-r--r--   0        0        0      928 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/admin_approve_complete_email.html
+-rw-r--r--   0        0        0      507 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/admin_approve_complete_email.txt
+-rw-r--r--   0        0        0      943 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/admin_approve_complete_email_subject.txt
+-rw-r--r--   0        0        0     2855 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/admin_approve_email.html
+-rw-r--r--   0        0        0      459 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/admin_approve_email.txt
+-rw-r--r--   0        0        0       76 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/admin_approve_email_subject.txt
+-rwxr-xr-x   0        0        0     2310 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/login.html
+-rwxr-xr-x   0        0        0      449 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/logout.html
+-rwxr-xr-x   0        0        0      381 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/password_change_done.html
+-rwxr-xr-x   0        0        0      631 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/password_change_form.html
+-rwxr-xr-x   0        0        0      503 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/password_reset_complete.html
+-rwxr-xr-x   0        0        0      960 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/password_reset_confirm.html
+-rwxr-xr-x   0        0        0      536 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/password_reset_done.html
+-rwxr-xr-x   0        0        0     1007 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/password_reset_email.html
+-rwxr-xr-x   0        0        0      774 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/password_reset_form.html
+-rwxr-xr-x   0        0        0       46 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/registration_base.html
+-rwxr-xr-x   0        0        0      384 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/registration_closed.html
+-rwxr-xr-x   0        0        0      671 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/registration_complete.html
+-rwxr-xr-x   0        0        0      791 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/registration_form.html
+-rw-r--r--   0        0        0      713 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/resend_activation_complete.html
+-rw-r--r--   0        0        0      951 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/resend_activation_form.html
+-rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templatetags/__init__.py
+-rw-r--r--   0        0        0     1928 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/templatetags/common_extras.py
+-rw-r--r--   0        0        0      445 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/types.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/utils/__init__.py
+-rw-r--r--   0        0        0      451 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/utils/async_utils.py
+-rw-r--r--   0        0        0     1157 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/utils/auth_utils.py
+-rw-r--r--   0        0        0      818 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/utils/debounce.py
+-rw-r--r--   0        0        0      627 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/utils/htmx_triggers.py
+-rw-r--r--   0        0        0     1236 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/utils/mail.py
+-rw-r--r--   0        0        0     1832 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/utils/testing.py
+-rw-r--r--   0        0        0     3977 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/common/views.py
+-rw-r--r--   0        0        0     1697 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/__init__.py
+-rw-r--r--   0        0        0      390 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/admin.py
+-rw-r--r--   0        0        0      132 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/apps.py
+-rw-r--r--   0        0        0     2718 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/auth.py
+-rw-r--r--   0        0        0      715 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/factories.py
+-rw-r--r--   0        0        0     1828 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/forms.py
+-rw-r--r--   0        0        0     2529 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/migrations/0001_initial.py
+-rw-r--r--   0        0        0      596 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/migrations/0002_token_fraction_alter_token_token_string.py
+-rw-r--r--   0        0        0      432 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/migrations/0003_alter_token_client.py
+-rw-r--r--   0        0        0      386 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/migrations/0004_rename_token_string_token_token_hashed.py
+-rw-r--r--   0        0        0      795 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/migrations/0005_alter_token_options_remove_token_expires_and_more.py
+-rw-r--r--   0        0        0      411 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/migrations/0006_rename_expiry_time_token_expires.py
+-rw-r--r--   0        0        0      426 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/migrations/0007_alter_token_last_used.py
+-rw-r--r--   0        0        0      420 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/migrations/0008_alter_token_token_hashed.py
+-rw-r--r--   0        0        0      768 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/migrations/0009_rename_author_token_owner_alter_token_client_and_more.py
+-rw-r--r--   0        0        0      606 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/migrations/0010_alter_token_unique_together_and_more.py
+-rw-r--r--   0        0        0      818 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/migrations/0011_delete_tokensettings_alter_token_client_and_more.py
+-rw-r--r--   0        0        0      532 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/migrations/0012_remove_token_unique_client_per_user_and_more.py
+-rw-r--r--   0        0        0      441 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/migrations/0013_alter_token_description.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/migrations/__init__.py
+-rw-r--r--   0        0        0     1846 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/models.py
+-rw-r--r--   0        0        0      423 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/static/token_authentication/token_authentication.js
+-rw-r--r--   0        0        0      689 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/templates/token_authentication/_token_authentication_help.html
+-rw-r--r--   0        0        0      223 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/templates/token_authentication/token_authentication_layout.html
+-rw-r--r--   0        0        0     3690 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/templates/token_authentication/token_dashboard.html
+-rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/tests/__init__.py
+-rw-r--r--   0        0        0      463 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/tests/conftest.py
+-rw-r--r--   0        0        0      205 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/tests/integration/conftest.py
+-rw-r--r--   0        0        0     1666 2024-04-23 22:08:26.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/tests/integration/test_token_authentication.py
+-rw-r--r--   0        0        0      646 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/urls.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/utils/__init__.py
+-rw-r--r--   0        0        0      508 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/utils/crypto.py
+-rw-r--r--   0        0        0     2619 2024-04-23 12:13:46.000000 adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/views.py
+-rw-r--r--   0        0        0     3064 2024-04-24 19:57:46.666352 adit_radis_shared-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2077 1970-01-01 00:00:00.000000 adit_radis_shared-0.2.0/PKG-INFO
```

### Comparing `adit_radis_shared-0.1.0/LICENSE` & `adit_radis_shared-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/accounts/admin.py` & `adit_radis_shared-0.2.0/adit_radis_shared/accounts/admin.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/accounts/backends.py` & `adit_radis_shared-0.2.0/adit_radis_shared/accounts/backends.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/accounts/factories.py` & `adit_radis_shared-0.2.0/adit_radis_shared/accounts/factories.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/accounts/forms.py` & `adit_radis_shared-0.2.0/adit_radis_shared/accounts/forms.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/accounts/middlewares.py` & `adit_radis_shared-0.2.0/adit_radis_shared/accounts/middlewares.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/accounts/migrations/0001_initial.py` & `adit_radis_shared-0.2.0/adit_radis_shared/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/accounts/migrations/0005_institute.py` & `adit_radis_shared-0.2.0/adit_radis_shared/accounts/migrations/0005_institute.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/accounts/migrations/0006_user_active_group.py` & `adit_radis_shared-0.2.0/adit_radis_shared/accounts/migrations/0006_user_active_group.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/accounts/migrations/0007_convert_institutes_to_groups.py` & `adit_radis_shared-0.2.0/adit_radis_shared/accounts/migrations/0007_convert_institutes_to_groups.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/accounts/models.py` & `adit_radis_shared-0.2.0/adit_radis_shared/accounts/models.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/accounts/templates/accounts/_active_group_selector.html` & `adit_radis_shared-0.2.0/adit_radis_shared/accounts/templates/accounts/_active_group_selector.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/accounts/templates/accounts/profile.html` & `adit_radis_shared-0.2.0/adit_radis_shared/accounts/templates/accounts/profile.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/accounts/tests/test_migrations.py` & `adit_radis_shared-0.2.0/adit_radis_shared/accounts/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/accounts/views.py` & `adit_radis_shared-0.2.0/adit_radis_shared/accounts/views.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/decorators.py` & `adit_radis_shared-0.2.0/adit_radis_shared/common/decorators.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/forms.py` & `adit_radis_shared-0.2.0/adit_radis_shared/common/forms.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/management/base/celery_beat.py` & `adit_radis_shared-0.2.0/adit_radis_shared/common/management/base/celery_beat.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/management/base/celery_worker.py` & `adit_radis_shared-0.2.0/adit_radis_shared/common/management/base/celery_worker.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/management/base/hard_reset_migrations.py` & `adit_radis_shared-0.2.0/adit_radis_shared/common/management/base/hard_reset_migrations.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/management/base/server_command.py` & `adit_radis_shared-0.2.0/adit_radis_shared/common/management/base/server_command.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/management/commands/create_admin.py` & `adit_radis_shared-0.2.0/adit_radis_shared/common/management/commands/create_admin.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/management/commands/example_async_server.py` & `adit_radis_shared-0.2.0/adit_radis_shared/common/management/commands/example_async_server.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/management/commands/example_server.py` & `adit_radis_shared-0.2.0/adit_radis_shared/common/management/commands/example_server.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/management/commands/generate_cert.py` & `adit_radis_shared-0.2.0/adit_radis_shared/common/management/commands/generate_cert.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/management/commands/send_test_mail.py` & `adit_radis_shared-0.2.0/adit_radis_shared/common/management/commands/send_test_mail.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/middlewares.py` & `adit_radis_shared-0.2.0/adit_radis_shared/common/middlewares.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/migrations/0001_initial.py` & `adit_radis_shared-0.2.0/adit_radis_shared/common/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/migrations/0002_update_or_create_site.py` & `adit_radis_shared-0.2.0/adit_radis_shared/common/migrations/0002_update_or_create_site.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/mixins.py` & `adit_radis_shared-0.2.0/adit_radis_shared/common/mixins.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/models.py` & `adit_radis_shared-0.2.0/adit_radis_shared/common/models.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/site.py` & `adit_radis_shared-0.2.0/adit_radis_shared/common/site.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     order: int = 1
     staff_only: bool = False
 
 
 main_menu_items: list[MainMenuItem] = []
 
 
-def register_main_menu_item(url_name: str, label: str) -> None:
-    main_menu_items.append(MainMenuItem(url_name, label))
+def register_main_menu_item(menu_item: MainMenuItem) -> None:
+    main_menu_items.append(menu_item)
     main_menu_items.sort(key=lambda x: x.order)
 
 
 def base_context_processor(request: HttpRequest) -> dict[str, Any]:
     from .utils.auth_utils import is_logged_in_user
 
     theme = "auto"
```

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/static/common/common.css` & `adit_radis_shared-0.2.0/adit_radis_shared/common/static/common/common.css`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/static/common/common.js` & `adit_radis_shared-0.2.0/adit_radis_shared/common/static/common/common.js`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/static/common/theme.js` & `adit_radis_shared-0.2.0/adit_radis_shared/common/static/common/theme.js`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/static/vendor/alpine-morph.js` & `adit_radis_shared-0.2.0/adit_radis_shared/common/static/vendor/alpine-morph.js`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/static/vendor/alpine.js` & `adit_radis_shared-0.2.0/adit_radis_shared/common/static/vendor/alpine.js`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/static/vendor/bootstrap-icons.svg` & `adit_radis_shared-0.2.0/adit_radis_shared/common/static/vendor/bootstrap-icons.svg`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/static/vendor/bootstrap.bundle.js` & `adit_radis_shared-0.2.0/adit_radis_shared/common/static/vendor/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/static/vendor/bootstrap.bundle.js.map` & `adit_radis_shared-0.2.0/adit_radis_shared/common/static/vendor/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/static/vendor/bootstrap.css` & `adit_radis_shared-0.2.0/adit_radis_shared/common/static/vendor/bootstrap.css`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/static/vendor/htmx-alpine-morph.js` & `adit_radis_shared-0.2.0/adit_radis_shared/common/static/vendor/htmx-alpine-morph.js`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/static/vendor/htmx-ws.js` & `adit_radis_shared-0.2.0/adit_radis_shared/common/static/vendor/htmx-ws.js`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/static/vendor/htmx.js` & `adit_radis_shared-0.2.0/adit_radis_shared/common/static/vendor/htmx.js`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/_filter_set_field.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/_filter_set_field.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/_messages_panel.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/_messages_panel.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/_navbar.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/_navbar.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/_navbar_actions.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/_navbar_actions.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/_navbar_theme_switcher.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/_navbar_theme_switcher.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/_navbar_user_manager.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/_navbar_user_manager.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/_pagination.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/_pagination.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/_toasts_panel.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/_toasts_panel.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/common/common_layout.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/common/common_layout.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/activate.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/activate.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/activation_complete.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/activation_complete.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/activation_complete_admin_pending.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/activation_complete_admin_pending.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/activation_email.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/activation_email.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/activation_email.txt` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/activation_email.txt`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/activation_email_subject.txt` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/activation_email_subject.txt`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/admin_approve_complete.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/admin_approve_complete.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/admin_approve_complete_email.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/admin_approve_complete_email.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/admin_approve_complete_email_subject.txt` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/admin_approve_complete_email_subject.txt`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/admin_approve_email.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/admin_approve_email.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/login.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/password_change_form.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/password_reset_confirm.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/password_reset_done.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/password_reset_email.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/password_reset_form.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/registration_complete.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/registration_complete.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/registration_form.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/registration_form.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/resend_activation_complete.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/resend_activation_complete.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templates/registration/resend_activation_form.html` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templates/registration/resend_activation_form.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/templatetags/common_extras.py` & `adit_radis_shared-0.2.0/adit_radis_shared/common/templatetags/common_extras.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/utils/auth_utils.py` & `adit_radis_shared-0.2.0/adit_radis_shared/common/utils/auth_utils.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/utils/debounce.py` & `adit_radis_shared-0.2.0/adit_radis_shared/common/utils/debounce.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/utils/htmx_triggers.py` & `adit_radis_shared-0.2.0/adit_radis_shared/common/utils/htmx_triggers.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/utils/mail.py` & `adit_radis_shared-0.2.0/adit_radis_shared/common/utils/mail.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/utils/testing.py` & `adit_radis_shared-0.2.0/adit_radis_shared/common/utils/testing.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/common/views.py` & `adit_radis_shared-0.2.0/adit_radis_shared/common/views.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/conftest.py` & `adit_radis_shared-0.2.0/adit_radis_shared/conftest.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/auth.py` & `adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/auth.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/factories.py` & `adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/factories.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/forms.py` & `adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/forms.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/migrations/0001_initial.py` & `adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/migrations/0002_token_fraction_alter_token_token_string.py` & `adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/migrations/0002_token_fraction_alter_token_token_string.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/migrations/0005_alter_token_options_remove_token_expires_and_more.py` & `adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/migrations/0005_alter_token_options_remove_token_expires_and_more.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/migrations/0009_rename_author_token_owner_alter_token_client_and_more.py` & `adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/migrations/0009_rename_author_token_owner_alter_token_client_and_more.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/migrations/0010_alter_token_unique_together_and_more.py` & `adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/migrations/0010_alter_token_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/migrations/0011_delete_tokensettings_alter_token_client_and_more.py` & `adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/migrations/0011_delete_tokensettings_alter_token_client_and_more.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/migrations/0012_remove_token_unique_client_per_user_and_more.py` & `adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/migrations/0012_remove_token_unique_client_per_user_and_more.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/models.py` & `adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/models.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/templates/token_authentication/_token_authentication_help.html` & `adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/templates/token_authentication/_token_authentication_help.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/templates/token_authentication/token_dashboard.html` & `adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/templates/token_authentication/token_dashboard.html`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/tests/integration/test_token_authentication.py` & `adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/tests/integration/test_token_authentication.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/urls.py` & `adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/urls.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/adit_radis_shared/token_authentication/views.py` & `adit_radis_shared-0.2.0/adit_radis_shared/token_authentication/views.py`

 * *Files identical despite different names*

### Comparing `adit_radis_shared-0.1.0/pyproject.toml` & `adit_radis_shared-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "adit-radis-shared"
-version = "0.1.0"
+version = "0.2.0"
 description = "Shared Django apps between ADIT and RADIS"
 authors = ["Kai Schlamp <kai.schlamp@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 channels = "^4.0.0"
```

### Comparing `adit_radis_shared-0.1.0/PKG-INFO` & `adit_radis_shared-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adit-radis-shared
-Version: 0.1.0
+Version: 0.2.0
 Summary: Shared Django apps between ADIT and RADIS
 License: GPL-3.0-or-later
 Author: Kai Schlamp
 Author-email: kai.schlamp@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -30,17 +30,32 @@
 Requires-Dist: pytz (>=2024.1,<2025.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: wait-for-it (>=2.2.2,<3.0.0)
 Requires-Dist: watchfiles (>=0.21.0,<0.22.0)
 Requires-Dist: whitenoise (>=6.0.0,<7.0.0)
 Description-Content-Type: text/markdown
 
-# ADIT RADIS Shared Subrepo
+# ADIT RADIS Shared
 
 ## About
 
-Shared resources between ADIT and RADIS managed as a [git-subrepo](https://github.com/ingydotnet/git-subrepo).
+Shared Django apps between ADIT and RADIS.
+
+## Available apps
+
+### adit_radis_shared.common
+
+Contains common stuff as well as the vendor statics and overwritten templates of the registration app.
+Therefore it must be added directly before `registration` in `INSTALLED_APPS`.
+
+### adit_radis_shared.accounts
+
+Contains the custom user model and user profile stuff.
+
+### adit_radis_shared.token_authentication
+
+Token authentication support to access the API of ADIT and RADIS by using a REST API.
 
 ## License
 
 - GPL 3.0 or later
```


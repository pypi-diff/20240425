# Comparing `tmp/dj_stripe-2.8.3.tar.gz` & `tmp/dj_stripe-2.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_stripe-2.8.3.tar", max compression
+gzip compressed data, was "dj_stripe-2.8.4.tar", max compression
```

## Comparing `dj_stripe-2.8.3.tar` & `dj_stripe-2.8.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     1105 2022-12-18 16:39:44.777998 dj_stripe-2.8.3/LICENSE
--rw-r--r--   0        0        0        0 2023-01-23 10:39:38.183166 dj_stripe-2.8.3/djstripe/__init__.py
--rw-r--r--   0        0        0      134 2023-01-23 10:43:08.416007 dj_stripe-2.8.3/djstripe/admin/__init__.py
--rw-r--r--   0        0        0     4333 2023-02-08 11:19:52.979141 dj_stripe-2.8.3/djstripe/admin/actions.py
--rw-r--r--   0        0        0    26729 2023-10-10 09:15:02.307581 dj_stripe-2.8.3/djstripe/admin/admin.py
--rw-r--r--   0        0        0     2473 2023-01-26 13:35:12.323654 dj_stripe-2.8.3/djstripe/admin/admin_inline.py
--rw-r--r--   0        0        0     2861 2023-10-10 09:15:02.307581 dj_stripe-2.8.3/djstripe/admin/filters.py
--rw-r--r--   0        0        0     9817 2023-10-10 09:15:02.307581 dj_stripe-2.8.3/djstripe/admin/forms.py
--rw-r--r--   0        0        0      910 2023-01-23 10:43:08.416007 dj_stripe-2.8.3/djstripe/admin/utils.py
--rw-r--r--   0        0        0     4769 2023-01-23 10:43:08.416007 dj_stripe-2.8.3/djstripe/admin/views.py
--rw-r--r--   0        0        0      754 2023-08-15 14:48:38.651082 dj_stripe-2.8.3/djstripe/apps.py
--rw-r--r--   0        0        0    14315 2023-10-10 09:15:02.307581 dj_stripe-2.8.3/djstripe/checks.py
--rw-r--r--   0        0        0    27168 2023-10-10 09:15:02.307581 dj_stripe-2.8.3/djstripe/enums.py
--rw-r--r--   0        0        0    16030 2023-06-28 16:43:05.256299 dj_stripe-2.8.3/djstripe/event_handlers.py
--rw-r--r--   0        0        0      667 2023-01-23 10:43:08.416007 dj_stripe-2.8.3/djstripe/exceptions.py
--rw-r--r--   0        0        0     6138 2023-10-10 09:15:02.307581 dj_stripe-2.8.3/djstripe/fields.py
--rw-r--r--   0        0        0    18691 2022-12-18 16:39:44.777998 dj_stripe-2.8.3/djstripe/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    21056 2022-12-18 16:39:44.777998 dj_stripe-2.8.3/djstripe/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-01-23 10:39:38.193166 dj_stripe-2.8.3/djstripe/management/__init__.py
--rw-r--r--   0        0        0        0 2023-01-23 10:39:38.193166 dj_stripe-2.8.3/djstripe/management/commands/__init__.py
--rw-r--r--   0        0        0      281 2023-01-23 10:43:08.416007 dj_stripe-2.8.3/djstripe/management/commands/djstripe_clear_expired_idempotency_keys.py
--rw-r--r--   0        0        0     1044 2023-01-23 10:43:08.416007 dj_stripe-2.8.3/djstripe/management/commands/djstripe_init_customers.py
--rw-r--r--   0        0        0     4199 2023-01-23 10:43:08.416007 dj_stripe-2.8.3/djstripe/management/commands/djstripe_process_events.py
--rw-r--r--   0        0        0      889 2023-01-23 10:43:08.416007 dj_stripe-2.8.3/djstripe/management/commands/djstripe_sync_customers.py
--rw-r--r--   0        0        0    22919 2023-08-29 16:08:42.273260 dj_stripe-2.8.3/djstripe/management/commands/djstripe_sync_models.py
--rw-r--r--   0        0        0     2971 2023-01-23 10:43:08.416007 dj_stripe-2.8.3/djstripe/management/commands/djstripe_update_invoiceitem_ids.py
--rw-r--r--   0        0        0     3369 2023-01-23 10:43:08.416007 dj_stripe-2.8.3/djstripe/managers.py
--rw-r--r--   0        0        0   229743 2023-10-10 09:15:02.307581 dj_stripe-2.8.3/djstripe/migrations/0001_initial.py
--rw-r--r--   0        0        0    12750 2023-10-10 09:15:02.307581 dj_stripe-2.8.3/djstripe/migrations/0008_2_5.py
--rw-r--r--   0        0        0    14990 2023-10-10 09:15:02.317581 dj_stripe-2.8.3/djstripe/migrations/0009_2_6.py
--rw-r--r--   0        0        0      471 2023-10-10 09:15:02.317581 dj_stripe-2.8.3/djstripe/migrations/0010_alter_customer_balance.py
--rw-r--r--   0        0        0    20038 2023-10-10 09:15:02.317581 dj_stripe-2.8.3/djstripe/migrations/0011_2_7.py
--rw-r--r--   0        0        0    31037 2023-10-10 09:15:02.317581 dj_stripe-2.8.3/djstripe/migrations/0012_2_8.py
--rw-r--r--   0        0        0        0 2023-01-23 10:39:38.193166 dj_stripe-2.8.3/djstripe/migrations/__init__.py
--rw-r--r--   0        0        0     1059 2023-10-10 09:15:02.317581 dj_stripe-2.8.3/djstripe/migrations/sql/migrate_mysql_backward.sql
--rw-r--r--   0        0        0     1085 2023-10-10 09:15:02.317581 dj_stripe-2.8.3/djstripe/migrations/sql/migrate_mysql_forward.sql
--rw-r--r--   0        0        0     1446 2023-10-10 09:15:02.317581 dj_stripe-2.8.3/djstripe/migrations/sql/migrate_postgresql_backward.sql
--rw-r--r--   0        0        0     1216 2023-10-10 09:15:02.317581 dj_stripe-2.8.3/djstripe/migrations/sql/migrate_postgresql_forward.sql
--rw-r--r--   0        0        0     5867 2023-10-10 09:15:02.317581 dj_stripe-2.8.3/djstripe/migrations/sql/migrate_sqlite_backward.sql
--rw-r--r--   0        0        0     3269 2023-10-10 09:15:02.317581 dj_stripe-2.8.3/djstripe/migrations/sql/migrate_sqlite_forward.sql
--rw-r--r--   0        0        0     2034 2023-01-23 10:43:08.416007 dj_stripe-2.8.3/djstripe/mixins.py
--rw-r--r--   0        0        0     2153 2023-10-10 09:15:02.317581 dj_stripe-2.8.3/djstripe/models/__init__.py
--rw-r--r--   0        0        0    10319 2023-10-10 09:15:02.317581 dj_stripe-2.8.3/djstripe/models/account.py
--rw-r--r--   0        0        0     4290 2023-10-10 09:15:02.317581 dj_stripe-2.8.3/djstripe/models/api.py
--rw-r--r--   0        0        0    41776 2023-10-10 09:16:01.537086 dj_stripe-2.8.3/djstripe/models/base.py
--rw-r--r--   0        0        0   104191 2023-10-10 09:16:01.537086 dj_stripe-2.8.3/djstripe/models/billing.py
--rw-r--r--   0        0        0     7709 2023-10-10 09:15:02.317581 dj_stripe-2.8.3/djstripe/models/checkout.py
--rw-r--r--   0        0        0    13569 2023-10-10 09:16:01.537086 dj_stripe-2.8.3/djstripe/models/connect.py
--rw-r--r--   0        0        0    88141 2023-10-10 09:15:02.317581 dj_stripe-2.8.3/djstripe/models/core.py
--rw-r--r--   0        0        0        0 2023-01-23 10:39:38.193166 dj_stripe-2.8.3/djstripe/models/fraud.py
--rw-r--r--   0        0        0     1381 2023-04-18 15:20:04.974188 dj_stripe-2.8.3/djstripe/models/identity.py
--rw-r--r--   0        0        0     8809 2023-10-10 09:15:02.317581 dj_stripe-2.8.3/djstripe/models/orders.py
--rw-r--r--   0        0        0    42466 2023-10-10 09:16:01.537086 dj_stripe-2.8.3/djstripe/models/payment_methods.py
--rw-r--r--   0        0        0     1558 2023-06-28 16:43:05.267132 dj_stripe-2.8.3/djstripe/models/sigma.py
--rw-r--r--   0        0        0    12582 2023-10-10 09:15:02.317581 dj_stripe-2.8.3/djstripe/models/webhooks.py
--rw-r--r--   0        0        0     8205 2023-10-10 09:15:02.317581 dj_stripe-2.8.3/djstripe/settings.py
--rw-r--r--   0        0        0     8324 2023-06-28 16:43:05.267132 dj_stripe-2.8.3/djstripe/signals.py
--rw-r--r--   0        0        0      599 2023-01-23 10:43:08.416007 dj_stripe-2.8.3/djstripe/sync.py
--rw-r--r--   0        0        0      258 2022-12-18 16:39:44.788832 dj_stripe-2.8.3/djstripe/templates/djstripe/admin/add_form.html
--rw-r--r--   0        0        0     1019 2022-12-18 16:39:44.788832 dj_stripe-2.8.3/djstripe/templates/djstripe/admin/change_form.html
--rw-r--r--   0        0        0     2863 2022-12-18 16:39:44.788832 dj_stripe-2.8.3/djstripe/templates/djstripe/admin/confirm_action.html
--rw-r--r--   0        0        0      256 2022-12-18 16:39:44.788832 dj_stripe-2.8.3/djstripe/templates/djstripe/admin/webhook_endpoint/add_form.html
--rw-r--r--   0        0        0      233 2022-12-18 16:39:44.788832 dj_stripe-2.8.3/djstripe/templates/djstripe/admin/webhook_endpoint/change_form.html
--rw-r--r--   0        0        0     1303 2022-12-18 16:39:44.788832 dj_stripe-2.8.3/djstripe/templates/djstripe/admin/webhook_endpoint/delete_confirmation.html
--rw-r--r--   0        0        0      679 2023-10-10 09:15:02.317581 dj_stripe-2.8.3/djstripe/urls.py
--rw-r--r--   0        0        0     3486 2023-02-08 11:19:52.979141 dj_stripe-2.8.3/djstripe/utils.py
--rw-r--r--   0        0        0     2158 2023-10-10 09:15:02.327581 dj_stripe-2.8.3/djstripe/views.py
--rw-r--r--   0        0        0     3143 2023-01-23 10:43:08.416007 dj_stripe-2.8.3/djstripe/webhooks.py
--rw-r--r--   0        0        0     3635 2023-06-28 16:43:05.267132 dj_stripe-2.8.3/docs/README.md
--rw-r--r--   0        0        0     4708 2023-10-10 09:17:27.707583 dj_stripe-2.8.3/pyproject.toml
--rw-r--r--   0        0        0     5076 1970-01-01 00:00:00.000000 dj_stripe-2.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1105 2022-12-18 16:39:44.777998 dj_stripe-2.8.4/LICENSE
+-rw-r--r--   0        0        0        0 2023-01-23 10:39:38.183166 dj_stripe-2.8.4/djstripe/__init__.py
+-rw-r--r--   0        0        0      134 2023-01-23 10:43:08.416007 dj_stripe-2.8.4/djstripe/admin/__init__.py
+-rw-r--r--   0        0        0     4333 2023-02-08 11:19:52.979141 dj_stripe-2.8.4/djstripe/admin/actions.py
+-rw-r--r--   0        0        0    26729 2024-04-16 11:26:34.540198 dj_stripe-2.8.4/djstripe/admin/admin.py
+-rw-r--r--   0        0        0     2473 2023-01-26 13:35:12.323654 dj_stripe-2.8.4/djstripe/admin/admin_inline.py
+-rw-r--r--   0        0        0     2861 2024-04-16 11:26:34.540198 dj_stripe-2.8.4/djstripe/admin/filters.py
+-rw-r--r--   0        0        0     9817 2024-04-16 11:26:34.540198 dj_stripe-2.8.4/djstripe/admin/forms.py
+-rw-r--r--   0        0        0      910 2023-01-23 10:43:08.416007 dj_stripe-2.8.4/djstripe/admin/utils.py
+-rw-r--r--   0        0        0     4769 2023-01-23 10:43:08.416007 dj_stripe-2.8.4/djstripe/admin/views.py
+-rw-r--r--   0        0        0      754 2023-08-15 14:48:38.651082 dj_stripe-2.8.4/djstripe/apps.py
+-rw-r--r--   0        0        0    14315 2024-04-16 11:26:34.540198 dj_stripe-2.8.4/djstripe/checks.py
+-rw-r--r--   0        0        0    27168 2024-04-16 11:26:34.540198 dj_stripe-2.8.4/djstripe/enums.py
+-rw-r--r--   0        0        0    16030 2024-04-16 11:26:34.540198 dj_stripe-2.8.4/djstripe/event_handlers.py
+-rw-r--r--   0        0        0      667 2023-01-23 10:43:08.416007 dj_stripe-2.8.4/djstripe/exceptions.py
+-rw-r--r--   0        0        0     6138 2024-04-16 11:26:34.540198 dj_stripe-2.8.4/djstripe/fields.py
+-rw-r--r--   0        0        0    18691 2022-12-18 16:39:44.777998 dj_stripe-2.8.4/djstripe/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    21056 2022-12-18 16:39:44.777998 dj_stripe-2.8.4/djstripe/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-01-23 10:39:38.193166 dj_stripe-2.8.4/djstripe/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-23 10:39:38.193166 dj_stripe-2.8.4/djstripe/management/commands/__init__.py
+-rw-r--r--   0        0        0      281 2023-01-23 10:43:08.416007 dj_stripe-2.8.4/djstripe/management/commands/djstripe_clear_expired_idempotency_keys.py
+-rw-r--r--   0        0        0     1044 2023-01-23 10:43:08.416007 dj_stripe-2.8.4/djstripe/management/commands/djstripe_init_customers.py
+-rw-r--r--   0        0        0     4199 2023-01-23 10:43:08.416007 dj_stripe-2.8.4/djstripe/management/commands/djstripe_process_events.py
+-rw-r--r--   0        0        0      889 2023-01-23 10:43:08.416007 dj_stripe-2.8.4/djstripe/management/commands/djstripe_sync_customers.py
+-rw-r--r--   0        0        0    22919 2023-08-29 16:08:42.273260 dj_stripe-2.8.4/djstripe/management/commands/djstripe_sync_models.py
+-rw-r--r--   0        0        0     2971 2023-01-23 10:43:08.416007 dj_stripe-2.8.4/djstripe/management/commands/djstripe_update_invoiceitem_ids.py
+-rw-r--r--   0        0        0     3369 2023-01-23 10:43:08.416007 dj_stripe-2.8.4/djstripe/managers.py
+-rw-r--r--   0        0        0   229743 2024-04-16 11:26:34.540198 dj_stripe-2.8.4/djstripe/migrations/0001_initial.py
+-rw-r--r--   0        0        0    12750 2024-04-16 11:26:34.540198 dj_stripe-2.8.4/djstripe/migrations/0008_2_5.py
+-rw-r--r--   0        0        0    14990 2024-04-16 11:26:34.540198 dj_stripe-2.8.4/djstripe/migrations/0009_2_6.py
+-rw-r--r--   0        0        0      471 2024-04-16 11:26:34.540198 dj_stripe-2.8.4/djstripe/migrations/0010_alter_customer_balance.py
+-rw-r--r--   0        0        0    20038 2024-04-16 11:26:34.540198 dj_stripe-2.8.4/djstripe/migrations/0011_2_7.py
+-rw-r--r--   0        0        0    31037 2024-04-16 11:26:34.540198 dj_stripe-2.8.4/djstripe/migrations/0012_2_8.py
+-rw-r--r--   0        0        0        0 2023-01-23 10:39:38.193166 dj_stripe-2.8.4/djstripe/migrations/__init__.py
+-rw-r--r--   0        0        0     1059 2024-04-16 11:26:34.540198 dj_stripe-2.8.4/djstripe/migrations/sql/migrate_mysql_backward.sql
+-rw-r--r--   0        0        0     1085 2024-04-16 11:26:34.540198 dj_stripe-2.8.4/djstripe/migrations/sql/migrate_mysql_forward.sql
+-rw-r--r--   0        0        0     1446 2024-04-16 11:26:34.540198 dj_stripe-2.8.4/djstripe/migrations/sql/migrate_postgresql_backward.sql
+-rw-r--r--   0        0        0     1216 2024-04-16 11:26:34.540198 dj_stripe-2.8.4/djstripe/migrations/sql/migrate_postgresql_forward.sql
+-rw-r--r--   0        0        0     5867 2024-04-16 11:26:34.540198 dj_stripe-2.8.4/djstripe/migrations/sql/migrate_sqlite_backward.sql
+-rw-r--r--   0        0        0     3269 2024-04-16 11:26:34.540198 dj_stripe-2.8.4/djstripe/migrations/sql/migrate_sqlite_forward.sql
+-rw-r--r--   0        0        0     2034 2023-01-23 10:43:08.416007 dj_stripe-2.8.4/djstripe/mixins.py
+-rw-r--r--   0        0        0     2153 2024-04-16 11:26:34.540198 dj_stripe-2.8.4/djstripe/models/__init__.py
+-rw-r--r--   0        0        0    10319 2024-04-16 11:26:34.540198 dj_stripe-2.8.4/djstripe/models/account.py
+-rw-r--r--   0        0        0     4290 2024-04-16 11:26:34.540198 dj_stripe-2.8.4/djstripe/models/api.py
+-rw-r--r--   0        0        0    41776 2024-04-16 11:26:34.540198 dj_stripe-2.8.4/djstripe/models/base.py
+-rw-r--r--   0        0        0   104191 2024-04-16 11:26:34.550198 dj_stripe-2.8.4/djstripe/models/billing.py
+-rw-r--r--   0        0        0     7709 2024-04-16 11:26:34.550198 dj_stripe-2.8.4/djstripe/models/checkout.py
+-rw-r--r--   0        0        0    13569 2023-10-10 09:16:01.537086 dj_stripe-2.8.4/djstripe/models/connect.py
+-rw-r--r--   0        0        0    88141 2024-04-16 11:26:34.550198 dj_stripe-2.8.4/djstripe/models/core.py
+-rw-r--r--   0        0        0        0 2023-01-23 10:39:38.193166 dj_stripe-2.8.4/djstripe/models/fraud.py
+-rw-r--r--   0        0        0     1424 2024-03-20 23:19:52.783116 dj_stripe-2.8.4/djstripe/models/identity.py
+-rw-r--r--   0        0        0     8809 2024-04-16 11:26:34.550198 dj_stripe-2.8.4/djstripe/models/orders.py
+-rw-r--r--   0        0        0    42466 2024-04-16 11:26:34.550198 dj_stripe-2.8.4/djstripe/models/payment_methods.py
+-rw-r--r--   0        0        0     1558 2023-06-28 16:43:05.267132 dj_stripe-2.8.4/djstripe/models/sigma.py
+-rw-r--r--   0        0        0    12582 2024-04-16 11:26:34.550198 dj_stripe-2.8.4/djstripe/models/webhooks.py
+-rw-r--r--   0        0        0     8205 2024-04-16 11:26:34.550198 dj_stripe-2.8.4/djstripe/settings.py
+-rw-r--r--   0        0        0     8324 2024-04-16 11:26:34.550198 dj_stripe-2.8.4/djstripe/signals.py
+-rw-r--r--   0        0        0      599 2023-01-23 10:43:08.416007 dj_stripe-2.8.4/djstripe/sync.py
+-rw-r--r--   0        0        0      258 2022-12-18 16:39:44.788832 dj_stripe-2.8.4/djstripe/templates/djstripe/admin/add_form.html
+-rw-r--r--   0        0        0     1019 2022-12-18 16:39:44.788832 dj_stripe-2.8.4/djstripe/templates/djstripe/admin/change_form.html
+-rw-r--r--   0        0        0     2863 2022-12-18 16:39:44.788832 dj_stripe-2.8.4/djstripe/templates/djstripe/admin/confirm_action.html
+-rw-r--r--   0        0        0      256 2022-12-18 16:39:44.788832 dj_stripe-2.8.4/djstripe/templates/djstripe/admin/webhook_endpoint/add_form.html
+-rw-r--r--   0        0        0      233 2022-12-18 16:39:44.788832 dj_stripe-2.8.4/djstripe/templates/djstripe/admin/webhook_endpoint/change_form.html
+-rw-r--r--   0        0        0     1303 2022-12-18 16:39:44.788832 dj_stripe-2.8.4/djstripe/templates/djstripe/admin/webhook_endpoint/delete_confirmation.html
+-rw-r--r--   0        0        0      679 2024-04-16 11:26:34.550198 dj_stripe-2.8.4/djstripe/urls.py
+-rw-r--r--   0        0        0     3486 2023-02-08 11:19:52.979141 dj_stripe-2.8.4/djstripe/utils.py
+-rw-r--r--   0        0        0     2158 2024-04-16 11:26:34.550198 dj_stripe-2.8.4/djstripe/views.py
+-rw-r--r--   0        0        0     3045 2024-04-16 11:26:34.550198 dj_stripe-2.8.4/djstripe/webhooks.py
+-rw-r--r--   0        0        0     3635 2023-06-28 16:43:05.267132 dj_stripe-2.8.4/docs/README.md
+-rw-r--r--   0        0        0     4699 2024-04-16 11:27:10.070197 dj_stripe-2.8.4/pyproject.toml
+-rw-r--r--   0        0        0     5115 1970-01-01 00:00:00.000000 dj_stripe-2.8.4/PKG-INFO
```

### Comparing `dj_stripe-2.8.3/LICENSE` & `dj_stripe-2.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/admin/actions.py` & `dj_stripe-2.8.4/djstripe/admin/actions.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/admin/admin.py` & `dj_stripe-2.8.4/djstripe/admin/admin.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/admin/admin_inline.py` & `dj_stripe-2.8.4/djstripe/admin/admin_inline.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/admin/filters.py` & `dj_stripe-2.8.4/djstripe/admin/filters.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/admin/forms.py` & `dj_stripe-2.8.4/djstripe/admin/forms.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/admin/utils.py` & `dj_stripe-2.8.4/djstripe/admin/utils.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/admin/views.py` & `dj_stripe-2.8.4/djstripe/admin/views.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/apps.py` & `dj_stripe-2.8.4/djstripe/apps.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/checks.py` & `dj_stripe-2.8.4/djstripe/checks.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/enums.py` & `dj_stripe-2.8.4/djstripe/enums.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/event_handlers.py` & `dj_stripe-2.8.4/djstripe/event_handlers.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/exceptions.py` & `dj_stripe-2.8.4/djstripe/exceptions.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/fields.py` & `dj_stripe-2.8.4/djstripe/fields.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/locale/fr/LC_MESSAGES/django.po` & `dj_stripe-2.8.4/djstripe/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/locale/ru/LC_MESSAGES/django.po` & `dj_stripe-2.8.4/djstripe/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/management/commands/djstripe_init_customers.py` & `dj_stripe-2.8.4/djstripe/management/commands/djstripe_init_customers.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/management/commands/djstripe_process_events.py` & `dj_stripe-2.8.4/djstripe/management/commands/djstripe_process_events.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/management/commands/djstripe_sync_customers.py` & `dj_stripe-2.8.4/djstripe/management/commands/djstripe_sync_customers.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/management/commands/djstripe_sync_models.py` & `dj_stripe-2.8.4/djstripe/management/commands/djstripe_sync_models.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/management/commands/djstripe_update_invoiceitem_ids.py` & `dj_stripe-2.8.4/djstripe/management/commands/djstripe_update_invoiceitem_ids.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/managers.py` & `dj_stripe-2.8.4/djstripe/managers.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/migrations/0001_initial.py` & `dj_stripe-2.8.4/djstripe/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/migrations/0008_2_5.py` & `dj_stripe-2.8.4/djstripe/migrations/0008_2_5.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/migrations/0009_2_6.py` & `dj_stripe-2.8.4/djstripe/migrations/0009_2_6.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/migrations/0011_2_7.py` & `dj_stripe-2.8.4/djstripe/migrations/0011_2_7.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/migrations/0012_2_8.py` & `dj_stripe-2.8.4/djstripe/migrations/0012_2_8.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/migrations/sql/migrate_mysql_backward.sql` & `dj_stripe-2.8.4/djstripe/migrations/sql/migrate_mysql_backward.sql`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/migrations/sql/migrate_mysql_forward.sql` & `dj_stripe-2.8.4/djstripe/migrations/sql/migrate_mysql_forward.sql`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/migrations/sql/migrate_postgresql_backward.sql` & `dj_stripe-2.8.4/djstripe/migrations/sql/migrate_postgresql_backward.sql`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/migrations/sql/migrate_postgresql_forward.sql` & `dj_stripe-2.8.4/djstripe/migrations/sql/migrate_postgresql_forward.sql`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/migrations/sql/migrate_sqlite_backward.sql` & `dj_stripe-2.8.4/djstripe/migrations/sql/migrate_sqlite_backward.sql`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/migrations/sql/migrate_sqlite_forward.sql` & `dj_stripe-2.8.4/djstripe/migrations/sql/migrate_sqlite_forward.sql`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/mixins.py` & `dj_stripe-2.8.4/djstripe/mixins.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/models/__init__.py` & `dj_stripe-2.8.4/djstripe/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/models/account.py` & `dj_stripe-2.8.4/djstripe/models/account.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/models/api.py` & `dj_stripe-2.8.4/djstripe/models/api.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/models/base.py` & `dj_stripe-2.8.4/djstripe/models/base.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/models/billing.py` & `dj_stripe-2.8.4/djstripe/models/billing.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/models/checkout.py` & `dj_stripe-2.8.4/djstripe/models/checkout.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/models/connect.py` & `dj_stripe-2.8.4/djstripe/models/connect.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/models/core.py` & `dj_stripe-2.8.4/djstripe/models/core.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/models/identity.py` & `dj_stripe-2.8.4/djstripe/models/identity.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-import stripe
-from django.db import models
-
-from .. import enums
-from ..fields import JSONField, StripeEnumField, StripeForeignKey
-from .base import StripeModel
-
-
-class VerificationSession(StripeModel):
-    """
-    Stripe documentation: https://stripe.com/docs/api/identity/verification_sessions
-    """
-
-    stripe_class = stripe.identity.VerificationSession
-
-    last_error = JSONField(null=True, blank=True)
-    last_verification_report = StripeForeignKey(
-        "djstripe.VerificationReport", on_delete=models.SET_NULL, null=True, blank=True
-    )
-    redaction = JSONField(null=True, blank=True)
-    verified_outputs = JSONField(null=True, blank=True)
-    status = StripeEnumField(enum=enums.VerificationSessionStatus)
-    type = StripeEnumField(enum=enums.VerificationType)
-
-    # The following attributes are not stored because they are sensitive.
-    url = None
-    client_secret = None
-
-
-class VerificationReport(StripeModel):
-    """
-    Stripe documentation: https://stripe.com/docs/api/identity/verification_reports
-    """
-
-    stripe_class = stripe.identity.VerificationReport
-
-    document = JSONField(null=True, blank=True)
-    id_number = JSONField(null=True, blank=True)
-    options = JSONField(null=True, blank=True)
-    selfie = JSONField(null=True, blank=True)
-    type = StripeEnumField(enum=enums.VerificationType)
+import stripe
+from django.db import models
+
+from .. import enums
+from ..fields import JSONField, StripeEnumField, StripeForeignKey
+from .base import StripeModel
+
+
+class VerificationSession(StripeModel):
+    """
+    Stripe documentation: https://stripe.com/docs/api/identity/verification_sessions
+    """
+
+    stripe_class = stripe.identity.VerificationSession
+
+    last_error = JSONField(null=True, blank=True)
+    last_verification_report = StripeForeignKey(
+        "djstripe.VerificationReport", on_delete=models.SET_NULL, null=True, blank=True
+    )
+    redaction = JSONField(null=True, blank=True)
+    verified_outputs = JSONField(null=True, blank=True)
+    status = StripeEnumField(enum=enums.VerificationSessionStatus)
+    type = StripeEnumField(enum=enums.VerificationType)
+
+    # The following attributes are not stored because they are sensitive.
+    url = None
+    client_secret = None
+
+
+class VerificationReport(StripeModel):
+    """
+    Stripe documentation: https://stripe.com/docs/api/identity/verification_reports
+    """
+
+    stripe_class = stripe.identity.VerificationReport
+    expand_fields = ["document.dob", "document.expiration_date", "document.number"]
+
+    document = JSONField(null=True, blank=True)
+    id_number = JSONField(null=True, blank=True)
+    options = JSONField(null=True, blank=True)
+    selfie = JSONField(null=True, blank=True)
+    type = StripeEnumField(enum=enums.VerificationType)
```

### Comparing `dj_stripe-2.8.3/djstripe/models/orders.py` & `dj_stripe-2.8.4/djstripe/models/orders.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/models/payment_methods.py` & `dj_stripe-2.8.4/djstripe/models/payment_methods.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/models/sigma.py` & `dj_stripe-2.8.4/djstripe/models/sigma.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/models/webhooks.py` & `dj_stripe-2.8.4/djstripe/models/webhooks.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/settings.py` & `dj_stripe-2.8.4/djstripe/settings.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/signals.py` & `dj_stripe-2.8.4/djstripe/signals.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/sync.py` & `dj_stripe-2.8.4/djstripe/sync.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/templates/djstripe/admin/change_form.html` & `dj_stripe-2.8.4/djstripe/templates/djstripe/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/templates/djstripe/admin/confirm_action.html` & `dj_stripe-2.8.4/djstripe/templates/djstripe/admin/confirm_action.html`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/templates/djstripe/admin/webhook_endpoint/delete_confirmation.html` & `dj_stripe-2.8.4/djstripe/templates/djstripe/admin/webhook_endpoint/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/urls.py` & `dj_stripe-2.8.4/djstripe/urls.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/utils.py` & `dj_stripe-2.8.4/djstripe/utils.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/djstripe/views.py` & `dj_stripe-2.8.4/djstripe/views.py`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/docs/README.md` & `dj_stripe-2.8.4/docs/README.md`

 * *Files identical despite different names*

### Comparing `dj_stripe-2.8.3/pyproject.toml` & `dj_stripe-2.8.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 [tool.poetry]
 name = "dj-stripe"
-version = "2.8.3"
+version = "2.8.4"
 description = "Django + Stripe made easy"
 license = "MIT"
 authors = [
     "Alexander Kavanaugh <alex@kavdev.io>",
     "Jerome Leclanche <jerome@leclan.ch>",
-    "Arnav Choudhury <arnav13@gmail.com>",
 ]
 readme = "docs/README.md"
 homepage = "https://dj-stripe.dev"
 repository = "https://github.com/dj-stripe/dj-stripe"
 documentation = "https://dj-stripe.dev/dj-stripe/"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -19,14 +18,15 @@
     "Topic :: Office/Business :: Financial",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Framework :: Django",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
     "Framework :: Django :: 4.2",
+    "Framework :: Django :: 5.0",
 ]
 
 packages = [{ include = "djstripe" }]
 include = ["AUTHORS.md", "CONTRIBUTING.md", "HISTORY.md", "LICENSE"]
 exclude = ["manage.py"]
 
 [tool.poetry.urls]
```

### Comparing `dj_stripe-2.8.3/PKG-INFO` & `dj_stripe-2.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dj-stripe
-Version: 2.8.3
+Version: 2.8.4
 Summary: Django + Stripe made easy
 Home-page: https://dj-stripe.dev
 License: MIT
 Author: Alexander Kavanaugh
 Author-email: alex@kavdev.io
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: dj-stripe Version: 2.8.3 Summary: Django + Stripe
+Metadata-Version: 2.1 Name: dj-stripe Version: 2.8.4 Summary: Django + Stripe
 made easy Home-page: https://dj-stripe.dev License: MIT Author: Alexander
 Kavanaugh Author-email: alex@kavdev.io Requires-Python: >=3.8.0,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Web Environment Classifier: Framework :: Django Classifier: Framework ::
 Django :: 3.2 Classifier: Framework :: Django :: 4.0 Classifier: Framework ::
-Django :: 4.1 Classifier: Framework :: Django :: 4.2 Classifier: Intended
-Audience :: Developers Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Office/Business :: Financial
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Provides-Extra: mysql Provides-Extra: postgres Requires-Dist: django (>=3.2)
-Requires-Dist: mysqlclient (>=1.4.0) ; extra == "mysql" Requires-Dist: psycopg2
-(>=2.8.5,<3.0.0) ; extra == "postgres" Requires-Dist: stripe (>=2.48.0,<5.0.0)
-Project-URL: Documentation, https://dj-stripe.dev/dj-stripe/ Project-URL:
-Funding, https://github.com/sponsors/dj-stripe Project-URL: Repository, https:/
-/github.com/dj-stripe/dj-stripe Description-Content-Type: text/markdown # dj-
-stripe - Django + Stripe Made Easy [![Stripe Verified Partner](https://
-img.shields.io/static/
+Django :: 4.1 Classifier: Framework :: Django :: 4.2 Classifier: Framework ::
+Django :: 5.0 Classifier: Intended Audience :: Developers Classifier: License
+:: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic :: Office/
+Business :: Financial Classifier: Topic :: Software Development :: Libraries ::
+Python Modules Provides-Extra: mysql Provides-Extra: postgres Requires-Dist:
+django (>=3.2) Requires-Dist: mysqlclient (>=1.4.0) ; extra == "mysql"
+Requires-Dist: psycopg2 (>=2.8.5,<3.0.0) ; extra == "postgres" Requires-Dist:
+stripe (>=2.48.0,<5.0.0) Project-URL: Documentation, https://dj-stripe.dev/dj-
+stripe/ Project-URL: Funding, https://github.com/sponsors/dj-stripe Project-
+URL: Repository, https://github.com/dj-stripe/dj-stripe Description-Content-
+Type: text/markdown # dj-stripe - Django + Stripe Made Easy [![Stripe Verified
+Partner](https://img.shields.io/static/
 v1?label=Stripe&message=Verified%20Partner&color=red&style=for-the-badge)]
 (https://stripe.com/docs/libraries#community-libraries)
 [![CI tests](https://github.com/dj-stripe/dj-stripe/actions/workflows/ci.yml/
 badge.svg)](https://github.com/dj-stripe/dj-stripe/actions/workflows/ci.yml) [!
 [Package Downloads](https://img.shields.io/pypi/dm/dj-stripe)](https://
 pypi.org/project/dj-stripe/) [![Documentation](https://img.shields.io/static/
 v1?label=Docs&message=READ&color=informational&style=plastic)](https://dj-
```


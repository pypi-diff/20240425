# Comparing `tmp/django-jutil-4.1.8.tar.gz` & `tmp/django-jutil-4.1.9.tar.gz`

## Comparing `django-jutil-4.1.8.tar` & `django-jutil-4.1.9.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-02-21 04:06:35.000000 django-jutil-4.1.8/
--rw-r--r--   0 jani      (1000) jani      (1000)    16348 2024-02-21 04:06:31.000000 django-jutil-4.1.8/PKG-INFO
--rw-rw-r--   0 jani      (1000) jani      (1000)      301 2023-06-21 12:01:35.000000 django-jutil-4.1.8/requirements-dev.txt
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-02-21 04:06:31.000000 django-jutil-4.1.8/jutil/
--rw-rw-r--   0 jani      (1000) jani      (1000)     1345 2023-05-15 21:51:19.000000 django-jutil-4.1.8/jutil/bank_const_iban.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    15881 2024-01-05 00:11:18.000000 django-jutil-4.1.8/jutil/bank_const_fi.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    23566 2024-01-05 01:14:49.000000 django-jutil-4.1.8/jutil/validators.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-02-21 04:06:31.000000 django-jutil-4.1.8/jutil/management/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-02-21 04:06:31.000000 django-jutil-4.1.8/jutil/management/commands/
--rw-rw-r--   0 jani      (1000) jani      (1000)     3592 2023-11-12 04:19:57.000000 django-jutil-4.1.8/jutil/management/commands/list_users.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      528 2023-05-15 21:51:19.000000 django-jutil-4.1.8/jutil/management/commands/geo_ip.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      804 2023-05-15 21:51:19.000000 django-jutil-4.1.8/jutil/management/commands/setpass.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3176 2024-01-05 00:11:18.000000 django-jutil-4.1.8/jutil/management/commands/make_bank_const_fi.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1162 2023-05-15 21:51:19.000000 django-jutil-4.1.8/jutil/management/commands/list_files.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     5130 2023-05-25 22:07:00.000000 django-jutil-4.1.8/jutil/management/commands/make_bank_const_se.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2779 2023-05-15 21:51:19.000000 django-jutil-4.1.8/jutil/management/commands/send_email.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      752 2023-05-15 21:51:19.000000 django-jutil-4.1.8/jutil/management/commands/apps.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2180 2023-05-25 22:07:00.000000 django-jutil-4.1.8/jutil/management/commands/make_bank_const_dk.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:51:19.000000 django-jutil-4.1.8/jutil/management/commands/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:51:19.000000 django-jutil-4.1.8/jutil/management/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2787 2023-05-25 22:07:00.000000 django-jutil-4.1.8/jutil/responses.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     8760 2023-10-13 23:32:33.000000 django-jutil-4.1.8/jutil/xml.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     5958 2023-10-13 23:32:33.000000 django-jutil-4.1.8/jutil/model.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    13763 2023-11-12 04:19:57.000000 django-jutil-4.1.8/jutil/email.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-02-21 04:06:31.000000 django-jutil-4.1.8/jutil/templatetags/
--rw-rw-r--   0 jani      (1000) jani      (1000)     4198 2023-11-16 03:27:18.000000 django-jutil-4.1.8/jutil/templatetags/jutil_admin.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:51:19.000000 django-jutil-4.1.8/jutil/templatetags/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3188 2024-02-21 04:06:22.000000 django-jutil-4.1.8/jutil/parse.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2694 2023-10-29 23:15:22.000000 django-jutil-4.1.8/jutil/redis_admin_helpers.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1689 2023-05-15 21:51:19.000000 django-jutil-4.1.8/jutil/testing.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-02-21 04:06:31.000000 django-jutil-4.1.8/jutil/locale/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-02-21 04:06:31.000000 django-jutil-4.1.8/jutil/locale/fi/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-02-21 04:06:31.000000 django-jutil-4.1.8/jutil/locale/fi/LC_MESSAGES/
--rw-rw-r--   0 jani      (1000) jani      (1000)     2784 2023-09-13 01:08:49.000000 django-jutil-4.1.8/jutil/locale/fi/LC_MESSAGES/django.mo
--rw-rw-r--   0 jani      (1000) jani      (1000)     6265 2023-09-13 01:08:58.000000 django-jutil-4.1.8/jutil/locale/fi/LC_MESSAGES/django.po
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-02-21 04:06:31.000000 django-jutil-4.1.8/jutil/locale/sv/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-02-21 04:06:31.000000 django-jutil-4.1.8/jutil/locale/sv/LC_MESSAGES/
--rw-rw-r--   0 jani      (1000) jani      (1000)     3326 2023-09-13 01:08:58.000000 django-jutil-4.1.8/jutil/locale/sv/LC_MESSAGES/django.mo
--rw-rw-r--   0 jani      (1000) jani      (1000)     6339 2023-09-13 01:08:58.000000 django-jutil-4.1.8/jutil/locale/sv/LC_MESSAGES/django.po
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-02-21 04:06:31.000000 django-jutil-4.1.8/jutil/locale/en/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-02-21 04:06:31.000000 django-jutil-4.1.8/jutil/locale/en/LC_MESSAGES/
--rw-rw-r--   0 jani      (1000) jani      (1000)      381 2023-09-13 01:08:49.000000 django-jutil-4.1.8/jutil/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 jani      (1000) jani      (1000)     5260 2023-09-13 01:08:58.000000 django-jutil-4.1.8/jutil/locale/en/LC_MESSAGES/django.po
--rw-rw-r--   0 jani      (1000) jani      (1000)     1135 2023-05-25 22:07:00.000000 django-jutil-4.1.8/jutil/auth.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      983 2023-05-25 22:07:00.000000 django-jutil-4.1.8/jutil/decorators.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    22659 2023-12-06 03:57:32.000000 django-jutil-4.1.8/jutil/admin.py
--rw-rw-r--   0 jani      (1000) jani      (1000)       26 2021-10-20 18:28:57.000000 django-jutil-4.1.8/jutil/py.typed
--rw-rw-r--   0 jani      (1000) jani      (1000)    58659 2023-12-17 21:36:37.000000 django-jutil-4.1.8/jutil/tests.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3739 2024-02-21 04:06:22.000000 django-jutil-4.1.8/jutil/openpyxl_helpers.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     5883 2023-05-25 22:07:00.000000 django-jutil-4.1.8/jutil/middleware.py
--rw-rw-r--   0 jani      (1000) jani      (1000)       85 2023-05-15 21:51:19.000000 django-jutil-4.1.8/jutil/apps.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    93215 2023-05-15 21:51:19.000000 django-jutil-4.1.8/jutil/bank_const_dk.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     5108 2023-12-17 21:36:37.000000 django-jutil-4.1.8/jutil/command.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      348 2023-05-15 21:51:19.000000 django-jutil-4.1.8/jutil/dict.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    22897 2023-05-15 21:51:19.000000 django-jutil-4.1.8/jutil/bank_const_be.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     6094 2023-11-12 03:07:29.000000 django-jutil-4.1.8/jutil/redis_helpers.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2088 2023-05-15 21:51:19.000000 django-jutil-4.1.8/jutil/bank_const_se.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1372 2024-01-12 21:52:58.000000 django-jutil-4.1.8/jutil/sms.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3208 2023-10-13 23:32:33.000000 django-jutil-4.1.8/jutil/cache.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     7249 2023-10-13 23:32:33.000000 django-jutil-4.1.8/jutil/request.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      905 2023-05-15 21:51:19.000000 django-jutil-4.1.8/jutil/urls.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1989 2023-10-13 23:32:33.000000 django-jutil-4.1.8/jutil/drf_exceptions.py
--rw-rw-r--   0 jani      (1000) jani      (1000)       46 2023-05-15 21:51:19.000000 django-jutil-4.1.8/jutil/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    19444 2023-10-13 23:32:33.000000 django-jutil-4.1.8/jutil/format.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      856 2023-10-13 23:32:33.000000 django-jutil-4.1.8/jutil/permissions.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    14719 2024-02-21 04:06:22.000000 django-jutil-4.1.8/jutil/dates.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3327 2023-05-25 22:07:00.000000 django-jutil-4.1.8/jutil/files.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      837 2023-11-01 03:06:03.000000 django-jutil-4.1.8/jutil/modelfields.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-02-21 04:06:31.000000 django-jutil-4.1.8/jutil/templates/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-02-21 04:06:31.000000 django-jutil-4.1.8/jutil/templates/jutil/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-02-21 04:06:31.000000 django-jutil-4.1.8/jutil/templates/jutil/admin/
--rw-rw-r--   0 jani      (1000) jani      (1000)     2101 2023-11-11 22:20:07.000000 django-jutil-4.1.8/jutil/templates/jutil/admin/object_history.html
--rw-rw-r--   0 jani      (1000) jani      (1000)      913 2023-04-04 05:29:53.000000 django-jutil-4.1.8/pyproject.toml
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-02-21 04:06:31.000000 django-jutil-4.1.8/django_jutil.egg-info/
--rw-rw-r--   0 jani      (1000) jani      (1000)   587199 2024-02-21 04:06:31.000000 django-jutil-4.1.8/django_jutil.egg-info/SOURCES.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)        6 2024-02-21 04:06:24.000000 django-jutil-4.1.8/django_jutil.egg-info/top_level.txt
--rw-r--r--   0 jani      (1000) jani      (1000)    16348 2024-02-21 04:06:24.000000 django-jutil-4.1.8/django_jutil.egg-info/PKG-INFO
--rw-rw-r--   0 jani      (1000) jani      (1000)      126 2024-02-21 04:06:24.000000 django-jutil-4.1.8/django_jutil.egg-info/requires.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)        1 2020-05-25 23:15:54.000000 django-jutil-4.1.8/django_jutil.egg-info/not-zip-safe
--rw-rw-r--   0 jani      (1000) jani      (1000)        1 2024-02-21 04:06:24.000000 django-jutil-4.1.8/django_jutil.egg-info/dependency_links.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)       38 2024-02-21 04:06:31.000000 django-jutil-4.1.8/setup.cfg
--rw-rw-r--   0 jani      (1000) jani      (1000)    15843 2023-12-13 01:44:39.000000 django-jutil-4.1.8/README.md
--rw-rw-r--   0 jani      (1000) jani      (1000)     1082 2020-05-21 16:43:46.000000 django-jutil-4.1.8/LICENSE.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)      120 2023-12-06 03:44:02.000000 django-jutil-4.1.8/requirements.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)      313 2023-10-27 21:57:33.000000 django-jutil-4.1.8/mypy.ini
--rw-rw-r--   0 jani      (1000) jani      (1000)      928 2024-02-21 04:06:22.000000 django-jutil-4.1.8/setup.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      249 2020-05-27 20:28:20.000000 django-jutil-4.1.8/MANIFEST.in
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-04-24 22:59:52.000000 django-jutil-4.1.9/
+-rw-r--r--   0 jani      (1000) jani      (1000)    16348 2024-04-24 22:59:47.000000 django-jutil-4.1.9/PKG-INFO
+-rw-rw-r--   0 jani      (1000) jani      (1000)      301 2023-06-21 12:01:35.000000 django-jutil-4.1.9/requirements-dev.txt
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-04-24 22:59:47.000000 django-jutil-4.1.9/jutil/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1345 2023-05-15 21:51:19.000000 django-jutil-4.1.9/jutil/bank_const_iban.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    15881 2024-01-05 00:11:18.000000 django-jutil-4.1.9/jutil/bank_const_fi.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    23566 2024-01-05 01:14:49.000000 django-jutil-4.1.9/jutil/validators.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-04-24 22:59:47.000000 django-jutil-4.1.9/jutil/management/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-04-24 22:59:47.000000 django-jutil-4.1.9/jutil/management/commands/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3592 2023-11-12 04:19:57.000000 django-jutil-4.1.9/jutil/management/commands/list_users.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      528 2023-05-15 21:51:19.000000 django-jutil-4.1.9/jutil/management/commands/geo_ip.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      804 2023-05-15 21:51:19.000000 django-jutil-4.1.9/jutil/management/commands/setpass.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3176 2024-01-05 00:11:18.000000 django-jutil-4.1.9/jutil/management/commands/make_bank_const_fi.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1162 2023-05-15 21:51:19.000000 django-jutil-4.1.9/jutil/management/commands/list_files.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     5130 2023-05-25 22:07:00.000000 django-jutil-4.1.9/jutil/management/commands/make_bank_const_se.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2779 2023-05-15 21:51:19.000000 django-jutil-4.1.9/jutil/management/commands/send_email.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      752 2023-05-15 21:51:19.000000 django-jutil-4.1.9/jutil/management/commands/apps.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2180 2023-05-25 22:07:00.000000 django-jutil-4.1.9/jutil/management/commands/make_bank_const_dk.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:51:19.000000 django-jutil-4.1.9/jutil/management/commands/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:51:19.000000 django-jutil-4.1.9/jutil/management/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2787 2023-05-25 22:07:00.000000 django-jutil-4.1.9/jutil/responses.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     8760 2024-03-04 22:27:00.000000 django-jutil-4.1.9/jutil/xml.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     5958 2023-10-13 23:32:33.000000 django-jutil-4.1.9/jutil/model.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    13763 2023-11-12 04:19:57.000000 django-jutil-4.1.9/jutil/email.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-04-24 22:59:47.000000 django-jutil-4.1.9/jutil/templatetags/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4198 2023-11-16 03:27:18.000000 django-jutil-4.1.9/jutil/templatetags/jutil_admin.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:51:19.000000 django-jutil-4.1.9/jutil/templatetags/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3188 2024-02-21 04:06:22.000000 django-jutil-4.1.9/jutil/parse.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2694 2023-10-29 23:15:22.000000 django-jutil-4.1.9/jutil/redis_admin_helpers.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1689 2023-05-15 21:51:19.000000 django-jutil-4.1.9/jutil/testing.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-04-24 22:59:46.000000 django-jutil-4.1.9/jutil/locale/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-04-24 22:59:46.000000 django-jutil-4.1.9/jutil/locale/fi/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-04-24 22:59:47.000000 django-jutil-4.1.9/jutil/locale/fi/LC_MESSAGES/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2784 2023-09-13 01:08:49.000000 django-jutil-4.1.9/jutil/locale/fi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 jani      (1000) jani      (1000)     6265 2023-09-13 01:08:58.000000 django-jutil-4.1.9/jutil/locale/fi/LC_MESSAGES/django.po
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-04-24 22:59:46.000000 django-jutil-4.1.9/jutil/locale/sv/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-04-24 22:59:47.000000 django-jutil-4.1.9/jutil/locale/sv/LC_MESSAGES/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3326 2023-09-13 01:08:58.000000 django-jutil-4.1.9/jutil/locale/sv/LC_MESSAGES/django.mo
+-rw-rw-r--   0 jani      (1000) jani      (1000)     6339 2023-09-13 01:08:58.000000 django-jutil-4.1.9/jutil/locale/sv/LC_MESSAGES/django.po
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-04-24 22:59:46.000000 django-jutil-4.1.9/jutil/locale/en/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-04-24 22:59:47.000000 django-jutil-4.1.9/jutil/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 jani      (1000) jani      (1000)      381 2023-09-13 01:08:49.000000 django-jutil-4.1.9/jutil/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 jani      (1000) jani      (1000)     5260 2023-09-13 01:08:58.000000 django-jutil-4.1.9/jutil/locale/en/LC_MESSAGES/django.po
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1135 2023-05-25 22:07:00.000000 django-jutil-4.1.9/jutil/auth.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      983 2023-05-25 22:07:00.000000 django-jutil-4.1.9/jutil/decorators.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    22659 2023-12-06 03:57:32.000000 django-jutil-4.1.9/jutil/admin.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)       26 2021-10-20 18:28:57.000000 django-jutil-4.1.9/jutil/py.typed
+-rw-rw-r--   0 jani      (1000) jani      (1000)    58659 2023-12-17 21:36:37.000000 django-jutil-4.1.9/jutil/tests.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3739 2024-02-21 04:06:22.000000 django-jutil-4.1.9/jutil/openpyxl_helpers.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     5883 2023-05-25 22:07:00.000000 django-jutil-4.1.9/jutil/middleware.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)       85 2023-05-15 21:51:19.000000 django-jutil-4.1.9/jutil/apps.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    93215 2023-05-15 21:51:19.000000 django-jutil-4.1.9/jutil/bank_const_dk.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     5108 2023-12-17 21:36:37.000000 django-jutil-4.1.9/jutil/command.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      348 2023-05-15 21:51:19.000000 django-jutil-4.1.9/jutil/dict.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    22897 2023-05-15 21:51:19.000000 django-jutil-4.1.9/jutil/bank_const_be.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     6094 2023-11-12 03:07:29.000000 django-jutil-4.1.9/jutil/redis_helpers.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2088 2023-05-15 21:51:19.000000 django-jutil-4.1.9/jutil/bank_const_se.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1372 2024-01-12 21:52:58.000000 django-jutil-4.1.9/jutil/sms.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3208 2023-10-13 23:32:33.000000 django-jutil-4.1.9/jutil/cache.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     7249 2023-10-13 23:32:33.000000 django-jutil-4.1.9/jutil/request.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      905 2023-05-15 21:51:19.000000 django-jutil-4.1.9/jutil/urls.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1989 2023-10-13 23:32:33.000000 django-jutil-4.1.9/jutil/drf_exceptions.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)       46 2023-05-15 21:51:19.000000 django-jutil-4.1.9/jutil/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    20062 2024-04-24 22:59:34.000000 django-jutil-4.1.9/jutil/format.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      856 2023-10-13 23:32:33.000000 django-jutil-4.1.9/jutil/permissions.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    14719 2024-02-21 04:06:22.000000 django-jutil-4.1.9/jutil/dates.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3327 2023-05-25 22:07:00.000000 django-jutil-4.1.9/jutil/files.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      837 2023-11-01 03:06:03.000000 django-jutil-4.1.9/jutil/modelfields.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-04-24 22:59:46.000000 django-jutil-4.1.9/jutil/templates/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-04-24 22:59:46.000000 django-jutil-4.1.9/jutil/templates/jutil/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-04-24 22:59:47.000000 django-jutil-4.1.9/jutil/templates/jutil/admin/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2101 2023-11-11 22:20:07.000000 django-jutil-4.1.9/jutil/templates/jutil/admin/object_history.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)      913 2023-04-04 05:29:53.000000 django-jutil-4.1.9/pyproject.toml
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-04-24 22:59:47.000000 django-jutil-4.1.9/django_jutil.egg-info/
+-rw-rw-r--   0 jani      (1000) jani      (1000)   587199 2024-04-24 22:59:46.000000 django-jutil-4.1.9/django_jutil.egg-info/SOURCES.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)        6 2024-04-24 22:59:36.000000 django-jutil-4.1.9/django_jutil.egg-info/top_level.txt
+-rw-r--r--   0 jani      (1000) jani      (1000)    16348 2024-04-24 22:59:36.000000 django-jutil-4.1.9/django_jutil.egg-info/PKG-INFO
+-rw-rw-r--   0 jani      (1000) jani      (1000)      126 2024-04-24 22:59:36.000000 django-jutil-4.1.9/django_jutil.egg-info/requires.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)        1 2020-05-25 23:15:54.000000 django-jutil-4.1.9/django_jutil.egg-info/not-zip-safe
+-rw-rw-r--   0 jani      (1000) jani      (1000)        1 2024-04-24 22:59:36.000000 django-jutil-4.1.9/django_jutil.egg-info/dependency_links.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)       38 2024-04-24 22:59:47.000000 django-jutil-4.1.9/setup.cfg
+-rw-rw-r--   0 jani      (1000) jani      (1000)    15843 2023-12-13 01:44:39.000000 django-jutil-4.1.9/README.md
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1082 2020-05-21 16:43:46.000000 django-jutil-4.1.9/LICENSE.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)      120 2023-12-06 03:44:02.000000 django-jutil-4.1.9/requirements.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)      313 2023-10-27 21:57:33.000000 django-jutil-4.1.9/mypy.ini
+-rw-rw-r--   0 jani      (1000) jani      (1000)      928 2024-04-24 22:59:34.000000 django-jutil-4.1.9/setup.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      249 2020-05-27 20:28:20.000000 django-jutil-4.1.9/MANIFEST.in
```

### Comparing `django-jutil-4.1.8/PKG-INFO` & `django-jutil-4.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jutil
-Version: 4.1.8
+Version: 4.1.9
 Summary: Collection of small utilities for Django and Django REST framework projects
 Home-page: https://github.com/kajala/django-jutil
 Author: Jani Kajala
 Author-email: kajala@gmail.com
 License: MIT licence, see LICENCE.txt
 License-File: LICENSE.txt
 Requires-Dist: Django>=2.1.7
```

### Comparing `django-jutil-4.1.8/jutil/bank_const_iban.py` & `django-jutil-4.1.9/jutil/bank_const_iban.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/bank_const_fi.py` & `django-jutil-4.1.9/jutil/bank_const_fi.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/validators.py` & `django-jutil-4.1.9/jutil/validators.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/management/commands/list_users.py` & `django-jutil-4.1.9/jutil/management/commands/list_users.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/management/commands/geo_ip.py` & `django-jutil-4.1.9/jutil/management/commands/geo_ip.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/management/commands/setpass.py` & `django-jutil-4.1.9/jutil/management/commands/setpass.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/management/commands/make_bank_const_fi.py` & `django-jutil-4.1.9/jutil/management/commands/make_bank_const_fi.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/management/commands/list_files.py` & `django-jutil-4.1.9/jutil/management/commands/list_files.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/management/commands/make_bank_const_se.py` & `django-jutil-4.1.9/jutil/management/commands/make_bank_const_se.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/management/commands/send_email.py` & `django-jutil-4.1.9/jutil/management/commands/send_email.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/management/commands/apps.py` & `django-jutil-4.1.9/jutil/management/commands/apps.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/management/commands/make_bank_const_dk.py` & `django-jutil-4.1.9/jutil/management/commands/make_bank_const_dk.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/responses.py` & `django-jutil-4.1.9/jutil/responses.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/xml.py` & `django-jutil-4.1.9/jutil/xml.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/model.py` & `django-jutil-4.1.9/jutil/model.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/email.py` & `django-jutil-4.1.9/jutil/email.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/templatetags/jutil_admin.py` & `django-jutil-4.1.9/jutil/templatetags/jutil_admin.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/parse.py` & `django-jutil-4.1.9/jutil/parse.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/redis_admin_helpers.py` & `django-jutil-4.1.9/jutil/redis_admin_helpers.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/testing.py` & `django-jutil-4.1.9/jutil/testing.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/locale/fi/LC_MESSAGES/django.mo` & `django-jutil-4.1.9/jutil/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/locale/fi/LC_MESSAGES/django.po` & `django-jutil-4.1.9/jutil/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/locale/sv/LC_MESSAGES/django.mo` & `django-jutil-4.1.9/jutil/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/locale/sv/LC_MESSAGES/django.po` & `django-jutil-4.1.9/jutil/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/locale/en/LC_MESSAGES/django.po` & `django-jutil-4.1.9/jutil/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/auth.py` & `django-jutil-4.1.9/jutil/auth.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/decorators.py` & `django-jutil-4.1.9/jutil/decorators.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/admin.py` & `django-jutil-4.1.9/jutil/admin.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/tests.py` & `django-jutil-4.1.9/jutil/tests.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/openpyxl_helpers.py` & `django-jutil-4.1.9/jutil/openpyxl_helpers.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/middleware.py` & `django-jutil-4.1.9/jutil/middleware.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/bank_const_dk.py` & `django-jutil-4.1.9/jutil/bank_const_dk.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/command.py` & `django-jutil-4.1.9/jutil/command.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/bank_const_be.py` & `django-jutil-4.1.9/jutil/bank_const_be.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/redis_helpers.py` & `django-jutil-4.1.9/jutil/redis_helpers.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/bank_const_se.py` & `django-jutil-4.1.9/jutil/bank_const_se.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/sms.py` & `django-jutil-4.1.9/jutil/sms.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/cache.py` & `django-jutil-4.1.9/jutil/cache.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/request.py` & `django-jutil-4.1.9/jutil/request.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/urls.py` & `django-jutil-4.1.9/jutil/urls.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/drf_exceptions.py` & `django-jutil-4.1.9/jutil/drf_exceptions.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/format.py` & `django-jutil-4.1.9/jutil/format.py`

 * *Files 3% similar despite different names*

```diff
@@ -201,26 +201,30 @@
 
     Returns:
         str
     """
     return json.dumps(value, indent=indent, cls=cls)
 
 
-def format_csv(rows: List[List[Any]], dialect: str = "excel") -> str:
-    """Formats rows to CSV string content.
+def format_csv(rows: List[List[Any]], dialect: str = "excel", delimiter: str = ",", doublequote: bool = True, lineterminator: str = "\r\n") -> str:
+    """Formats rows to CSV string content. Thin wrapper around csv.writer() for convenience.
 
     Args:
         rows: List[List[Any]]
         dialect: See csv.writer dialect
+        delimiter: A one-character string used to separate fields. It defaults to ','.
+        doublequote: Controls how instances of quote character appearing inside a field should themselves be quoted. When True, the character is doubled.
+                     When False, the escape character is used as a prefix to the quotechar. It defaults to True.
+        lineterminator: The string used to terminate lines
 
     Returns:
         str
     """
     f = StringIO()
-    writer = csv.writer(f, dialect=dialect)
+    writer = csv.writer(f, dialect=dialect, delimiter=delimiter, doublequote=doublequote, lineterminator=lineterminator)
     for row in rows:
         writer.writerow(row)
     return f.getvalue()
 
 
 def format_table(  # noqa
     rows: List[List[Any]],
```

### Comparing `django-jutil-4.1.8/jutil/permissions.py` & `django-jutil-4.1.9/jutil/permissions.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/dates.py` & `django-jutil-4.1.9/jutil/dates.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/files.py` & `django-jutil-4.1.9/jutil/files.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/modelfields.py` & `django-jutil-4.1.9/jutil/modelfields.py`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/jutil/templates/jutil/admin/object_history.html` & `django-jutil-4.1.9/jutil/templates/jutil/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/pyproject.toml` & `django-jutil-4.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/django_jutil.egg-info/SOURCES.txt` & `django-jutil-4.1.9/django_jutil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/django_jutil.egg-info/PKG-INFO` & `django-jutil-4.1.9/django_jutil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jutil
-Version: 4.1.8
+Version: 4.1.9
 Summary: Collection of small utilities for Django and Django REST framework projects
 Home-page: https://github.com/kajala/django-jutil
 Author: Jani Kajala
 Author-email: kajala@gmail.com
 License: MIT licence, see LICENCE.txt
 License-File: LICENSE.txt
 Requires-Dist: Django>=2.1.7
```

### Comparing `django-jutil-4.1.8/README.md` & `django-jutil-4.1.9/README.md`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/LICENSE.txt` & `django-jutil-4.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-jutil-4.1.8/setup.py` & `django-jutil-4.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     return [line for line in lineiter if line and not line.startswith("#")]
 
 
 install_requires = parse_requirements("requirements.txt", session=False)
 
 setup(
     name="django-jutil",
-    version="4.1.8",
+    version="4.1.9",
     author="Jani Kajala",
     author_email="kajala@gmail.com",
     packages=find_packages(exclude=["project", "venv"]),
     include_package_data=True,
     url="https://github.com/kajala/django-jutil",
     license="MIT licence, see LICENCE.txt",
     description="Collection of small utilities for Django and Django REST framework projects",
```


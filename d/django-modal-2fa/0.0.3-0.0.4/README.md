# Comparing `tmp/django-modal-2fa-0.0.3.tar.gz` & `tmp/django-modal-2fa-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-modal-2fa-0.0.3.tar", last modified: Sun Mar 17 14:44:34 2024, max compression
+gzip compressed data, was "django-modal-2fa-0.0.4.tar", last modified: Thu Apr 25 12:42:48 2024, max compression
```

## Comparing `django-modal-2fa-0.0.3.tar` & `django-modal-2fa-0.0.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2024-03-17 14:44:34.179050 django-modal-2fa-0.0.3/
--rw-rw-rw-   0        0        0     1085 2021-06-03 13:39:20.000000 django-modal-2fa-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       64 2021-09-03 12:40:14.000000 django-modal-2fa-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1763 2024-03-17 14:44:34.178083 django-modal-2fa-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-17 14:44:34.177080 django-modal-2fa-0.0.3/django_modal_2fa.egg-info/
--rw-rw-rw-   0        0        0     1763 2024-03-17 14:44:34.000000 django-modal-2fa-0.0.3/django_modal_2fa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1469 2024-03-17 14:44:34.000000 django-modal-2fa-0.0.3/django_modal_2fa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-17 14:44:34.000000 django-modal-2fa-0.0.3/django_modal_2fa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-03-17 14:44:34.000000 django-modal-2fa-0.0.3/django_modal_2fa.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-17 14:44:34.000000 django-modal-2fa-0.0.3/django_modal_2fa.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-17 14:44:34.155082 django-modal-2fa-0.0.3/modal_2fa/
--rw-rw-rw-   0        0        0        6 2021-06-28 10:13:19.000000 django-modal-2fa-0.0.3/modal_2fa/__init__.py
--rw-rw-rw-   0        0        0      614 2024-01-31 15:21:51.000000 django-modal-2fa-0.0.3/modal_2fa/admin.py
--rw-rw-rw-   0        0        0      168 2024-01-02 13:57:25.000000 django-modal-2fa-0.0.3/modal_2fa/admin_apps.py
--rw-rw-rw-   0        0        0      652 2024-01-02 13:58:16.000000 django-modal-2fa-0.0.3/modal_2fa/admin_site.py
--rw-rw-rw-   0        0        0       98 2024-01-02 12:39:58.000000 django-modal-2fa-0.0.3/modal_2fa/apps.py
--rw-rw-rw-   0        0        0    13624 2024-03-17 13:51:04.000000 django-modal-2fa-0.0.3/modal_2fa/auth.py
--rw-rw-rw-   0        0        0     2050 2024-01-03 10:06:41.000000 django-modal-2fa-0.0.3/modal_2fa/backends.py
--rw-rw-rw-   0        0        0     2226 2021-09-03 10:54:26.000000 django-modal-2fa-0.0.3/modal_2fa/customise.py
--rw-rw-rw-   0        0        0     4297 2024-03-17 13:51:04.000000 django-modal-2fa-0.0.3/modal_2fa/forms.py
-drwxrwxrwx   0        0        0        0 2024-03-17 14:44:34.158079 django-modal-2fa-0.0.3/modal_2fa/management/
--rw-rw-rw-   0        0        0        0 2024-01-03 15:23:27.000000 django-modal-2fa-0.0.3/modal_2fa/management/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-17 14:44:34.160051 django-modal-2fa-0.0.3/modal_2fa/management/commands/
--rw-rw-rw-   0        0        0        0 2024-01-03 15:23:45.000000 django-modal-2fa-0.0.3/modal_2fa/management/commands/__init__.py
--rw-rw-rw-   0        0        0      760 2024-01-03 16:15:27.000000 django-modal-2fa-0.0.3/modal_2fa/management/commands/clear_failed_logins.py
--rw-rw-rw-   0        0        0     1890 2021-09-08 09:06:19.000000 django-modal-2fa-0.0.3/modal_2fa/menus.py
-drwxrwxrwx   0        0        0        0 2024-03-17 14:44:34.163049 django-modal-2fa-0.0.3/modal_2fa/migrations/
--rw-rw-rw-   0        0        0     1287 2021-08-24 09:18:48.000000 django-modal-2fa-0.0.3/modal_2fa/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1753 2024-01-03 16:15:46.000000 django-modal-2fa-0.0.3/modal_2fa/migrations/0002_failedloginattempt_webauthncredential.py
--rw-rw-rw-   0        0        0      473 2024-01-31 08:35:40.000000 django-modal-2fa-0.0.3/modal_2fa/migrations/0003_webauthncredential_rp_id.py
--rw-rw-rw-   0        0        0        0 2021-06-28 10:56:22.000000 django-modal-2fa-0.0.3/modal_2fa/migrations/__init__.py
--rw-rw-rw-   0        0        0     5609 2024-01-31 14:06:36.000000 django-modal-2fa-0.0.3/modal_2fa/models.py
--rw-rw-rw-   0        0        0      253 2024-01-02 12:43:51.000000 django-modal-2fa-0.0.3/modal_2fa/settings_helper.py
-drwxrwxrwx   0        0        0        0 2024-03-17 14:44:34.105725 django-modal-2fa-0.0.3/modal_2fa/static/
-drwxrwxrwx   0        0        0        0 2024-03-17 14:44:34.164049 django-modal-2fa-0.0.3/modal_2fa/static/modal_2fa/
--rw-rw-rw-   0        0        0     8705 2023-12-30 11:48:01.000000 django-modal-2fa-0.0.3/modal_2fa/static/modal_2fa/webauthn.js
-drwxrwxrwx   0        0        0        0 2024-03-17 14:44:34.105725 django-modal-2fa-0.0.3/modal_2fa/templates/
-drwxrwxrwx   0        0        0        0 2024-03-17 14:44:34.169050 django-modal-2fa-0.0.3/modal_2fa/templates/modal_2fa/
--rw-rw-rw-   0        0        0      673 2021-09-01 19:13:10.000000 django-modal-2fa-0.0.3/modal_2fa/templates/modal_2fa/base.html
--rw-rw-rw-   0        0        0      724 2024-01-31 11:08:52.000000 django-modal-2fa-0.0.3/modal_2fa/templates/modal_2fa/database_cookies.html
-drwxrwxrwx   0        0        0        0 2024-03-17 14:44:34.176053 django-modal-2fa-0.0.3/modal_2fa/templates/modal_2fa/emails/
--rw-rw-rw-   0        0        0      451 2021-09-03 08:26:14.000000 django-modal-2fa-0.0.3/modal_2fa/templates/modal_2fa/emails/invite.html
--rw-rw-rw-   0        0        0      137 2021-09-01 12:00:23.000000 django-modal-2fa-0.0.3/modal_2fa/templates/modal_2fa/emails/invite_subject.txt
--rw-rw-rw-   0        0        0      418 2021-09-03 08:26:14.000000 django-modal-2fa-0.0.3/modal_2fa/templates/modal_2fa/emails/invite_txt.html
--rw-rw-rw-   0        0        0      601 2021-09-03 08:15:02.000000 django-modal-2fa-0.0.3/modal_2fa/templates/modal_2fa/emails/password_reset_email.html
--rw-rw-rw-   0        0        0      124 2020-05-27 09:29:10.000000 django-modal-2fa-0.0.3/modal_2fa/templates/modal_2fa/emails/password_reset_subject.txt
--rw-rw-rw-   0        0        0      260 2024-01-06 15:57:23.000000 django-modal-2fa-0.0.3/modal_2fa/templates/modal_2fa/new_totp.html
--rw-rw-rw-   0        0        0      105 2021-09-02 19:14:49.000000 django-modal-2fa-0.0.3/modal_2fa/templates/modal_2fa/user_admin_modal.html
--rw-rw-rw-   0        0        0      676 2024-01-31 11:15:43.000000 django-modal-2fa-0.0.3/modal_2fa/templates/modal_2fa/webauthn_devices.html
--rw-rw-rw-   0        0        0     2080 2023-12-29 11:51:42.000000 django-modal-2fa-0.0.3/modal_2fa/urls.py
--rw-rw-rw-   0        0        0     2670 2021-09-02 18:59:57.000000 django-modal-2fa-0.0.3/modal_2fa/user_admin.py
--rw-rw-rw-   0        0        0     1834 2021-09-02 16:48:18.000000 django-modal-2fa-0.0.3/modal_2fa/users.py
--rw-rw-rw-   0        0        0      477 2021-09-02 16:48:18.000000 django-modal-2fa-0.0.3/modal_2fa/utils.py
--rw-rw-rw-   0        0        0     5709 2024-03-17 13:51:04.000000 django-modal-2fa-0.0.3/modal_2fa/webauthn.py
--rw-rw-rw-   0        0        0       42 2024-03-17 14:44:34.179050 django-modal-2fa-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      783 2024-03-17 14:35:25.000000 django-modal-2fa-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:42:48.165398 django-modal-2fa-0.0.4/
+-rw-rw-rw-   0        0        0     1085 2021-06-03 13:39:20.000000 django-modal-2fa-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       64 2021-09-03 12:40:14.000000 django-modal-2fa-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1763 2024-04-25 12:42:48.164397 django-modal-2fa-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 12:42:48.163398 django-modal-2fa-0.0.4/django_modal_2fa.egg-info/
+-rw-rw-rw-   0        0        0     1763 2024-04-25 12:42:47.000000 django-modal-2fa-0.0.4/django_modal_2fa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1469 2024-04-25 12:42:48.000000 django-modal-2fa-0.0.4/django_modal_2fa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 12:42:47.000000 django-modal-2fa-0.0.4/django_modal_2fa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-25 12:42:47.000000 django-modal-2fa-0.0.4/django_modal_2fa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-25 12:42:47.000000 django-modal-2fa-0.0.4/django_modal_2fa.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 12:42:48.142397 django-modal-2fa-0.0.4/modal_2fa/
+-rw-rw-rw-   0        0        0        6 2021-06-28 10:13:19.000000 django-modal-2fa-0.0.4/modal_2fa/__init__.py
+-rw-rw-rw-   0        0        0      614 2024-01-31 15:21:51.000000 django-modal-2fa-0.0.4/modal_2fa/admin.py
+-rw-rw-rw-   0        0        0      168 2024-01-02 13:57:25.000000 django-modal-2fa-0.0.4/modal_2fa/admin_apps.py
+-rw-rw-rw-   0        0        0      652 2024-01-02 13:58:16.000000 django-modal-2fa-0.0.4/modal_2fa/admin_site.py
+-rw-rw-rw-   0        0        0       98 2024-01-02 12:39:58.000000 django-modal-2fa-0.0.4/modal_2fa/apps.py
+-rw-rw-rw-   0        0        0    13624 2024-03-17 13:51:04.000000 django-modal-2fa-0.0.4/modal_2fa/auth.py
+-rw-rw-rw-   0        0        0     2050 2024-01-03 10:06:41.000000 django-modal-2fa-0.0.4/modal_2fa/backends.py
+-rw-rw-rw-   0        0        0     2226 2021-09-03 10:54:26.000000 django-modal-2fa-0.0.4/modal_2fa/customise.py
+-rw-rw-rw-   0        0        0     4297 2024-03-17 13:51:04.000000 django-modal-2fa-0.0.4/modal_2fa/forms.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:42:48.143397 django-modal-2fa-0.0.4/modal_2fa/management/
+-rw-rw-rw-   0        0        0        0 2024-01-03 15:23:27.000000 django-modal-2fa-0.0.4/modal_2fa/management/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:42:48.146397 django-modal-2fa-0.0.4/modal_2fa/management/commands/
+-rw-rw-rw-   0        0        0        0 2024-01-03 15:23:45.000000 django-modal-2fa-0.0.4/modal_2fa/management/commands/__init__.py
+-rw-rw-rw-   0        0        0      760 2024-01-03 16:15:27.000000 django-modal-2fa-0.0.4/modal_2fa/management/commands/clear_failed_logins.py
+-rw-rw-rw-   0        0        0     1890 2021-09-08 09:06:19.000000 django-modal-2fa-0.0.4/modal_2fa/menus.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:42:48.149401 django-modal-2fa-0.0.4/modal_2fa/migrations/
+-rw-rw-rw-   0        0        0     1287 2021-08-24 09:18:48.000000 django-modal-2fa-0.0.4/modal_2fa/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1753 2024-01-03 16:15:46.000000 django-modal-2fa-0.0.4/modal_2fa/migrations/0002_failedloginattempt_webauthncredential.py
+-rw-rw-rw-   0        0        0      473 2024-01-31 08:35:40.000000 django-modal-2fa-0.0.4/modal_2fa/migrations/0003_webauthncredential_rp_id.py
+-rw-rw-rw-   0        0        0        0 2021-06-28 10:56:22.000000 django-modal-2fa-0.0.4/modal_2fa/migrations/__init__.py
+-rw-rw-rw-   0        0        0     5609 2024-01-31 14:06:36.000000 django-modal-2fa-0.0.4/modal_2fa/models.py
+-rw-rw-rw-   0        0        0      253 2024-01-02 12:43:51.000000 django-modal-2fa-0.0.4/modal_2fa/settings_helper.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:42:48.091432 django-modal-2fa-0.0.4/modal_2fa/static/
+drwxrwxrwx   0        0        0        0 2024-04-25 12:42:48.150397 django-modal-2fa-0.0.4/modal_2fa/static/modal_2fa/
+-rw-rw-rw-   0        0        0     8705 2023-12-30 11:48:01.000000 django-modal-2fa-0.0.4/modal_2fa/static/modal_2fa/webauthn.js
+drwxrwxrwx   0        0        0        0 2024-04-25 12:42:48.092438 django-modal-2fa-0.0.4/modal_2fa/templates/
+drwxrwxrwx   0        0        0        0 2024-04-25 12:42:48.155397 django-modal-2fa-0.0.4/modal_2fa/templates/modal_2fa/
+-rw-rw-rw-   0        0        0      673 2021-09-01 19:13:10.000000 django-modal-2fa-0.0.4/modal_2fa/templates/modal_2fa/base.html
+-rw-rw-rw-   0        0        0      724 2024-01-31 11:08:52.000000 django-modal-2fa-0.0.4/modal_2fa/templates/modal_2fa/database_cookies.html
+drwxrwxrwx   0        0        0        0 2024-04-25 12:42:48.162398 django-modal-2fa-0.0.4/modal_2fa/templates/modal_2fa/emails/
+-rw-rw-rw-   0        0        0      451 2021-09-03 08:26:14.000000 django-modal-2fa-0.0.4/modal_2fa/templates/modal_2fa/emails/invite.html
+-rw-rw-rw-   0        0        0      137 2021-09-01 12:00:23.000000 django-modal-2fa-0.0.4/modal_2fa/templates/modal_2fa/emails/invite_subject.txt
+-rw-rw-rw-   0        0        0      418 2021-09-03 08:26:14.000000 django-modal-2fa-0.0.4/modal_2fa/templates/modal_2fa/emails/invite_txt.html
+-rw-rw-rw-   0        0        0      601 2021-09-03 08:15:02.000000 django-modal-2fa-0.0.4/modal_2fa/templates/modal_2fa/emails/password_reset_email.html
+-rw-rw-rw-   0        0        0      124 2020-05-27 09:29:10.000000 django-modal-2fa-0.0.4/modal_2fa/templates/modal_2fa/emails/password_reset_subject.txt
+-rw-rw-rw-   0        0        0      260 2024-01-06 15:57:23.000000 django-modal-2fa-0.0.4/modal_2fa/templates/modal_2fa/new_totp.html
+-rw-rw-rw-   0        0        0      105 2021-09-02 19:14:49.000000 django-modal-2fa-0.0.4/modal_2fa/templates/modal_2fa/user_admin_modal.html
+-rw-rw-rw-   0        0        0      676 2024-01-31 11:15:43.000000 django-modal-2fa-0.0.4/modal_2fa/templates/modal_2fa/webauthn_devices.html
+-rw-rw-rw-   0        0        0     2080 2023-12-29 11:51:42.000000 django-modal-2fa-0.0.4/modal_2fa/urls.py
+-rw-rw-rw-   0        0        0     2670 2021-09-02 18:59:57.000000 django-modal-2fa-0.0.4/modal_2fa/user_admin.py
+-rw-rw-rw-   0        0        0     1834 2021-09-02 16:48:18.000000 django-modal-2fa-0.0.4/modal_2fa/users.py
+-rw-rw-rw-   0        0        0      477 2021-09-02 16:48:18.000000 django-modal-2fa-0.0.4/modal_2fa/utils.py
+-rw-rw-rw-   0        0        0     5709 2024-03-17 13:51:04.000000 django-modal-2fa-0.0.4/modal_2fa/webauthn.py
+-rw-rw-rw-   0        0        0       42 2024-04-25 12:42:48.165398 django-modal-2fa-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      783 2024-04-25 12:41:54.000000 django-modal-2fa-0.0.4/setup.py
```

### Comparing `django-modal-2fa-0.0.3/LICENSE` & `django-modal-2fa-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-modal-2fa-0.0.3/PKG-INFO` & `django-modal-2fa-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-modal-2fa
-Version: 0.0.3
+Version: 0.0.4
 Summary: Django app to implement two factor authentication with bootstrap modals
 Home-page: https://github.com/jonesim/django-2fa
 Author: Ian Jones
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `django-modal-2fa-0.0.3/django_modal_2fa.egg-info/PKG-INFO` & `django-modal-2fa-0.0.4/django_modal_2fa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-modal-2fa
-Version: 0.0.3
+Version: 0.0.4
 Summary: Django app to implement two factor authentication with bootstrap modals
 Home-page: https://github.com/jonesim/django-2fa
 Author: Ian Jones
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `django-modal-2fa-0.0.3/django_modal_2fa.egg-info/SOURCES.txt` & `django-modal-2fa-0.0.4/django_modal_2fa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-modal-2fa-0.0.3/modal_2fa/admin.py` & `django-modal-2fa-0.0.4/modal_2fa/admin.py`

 * *Files identical despite different names*

### Comparing `django-modal-2fa-0.0.3/modal_2fa/admin_site.py` & `django-modal-2fa-0.0.4/modal_2fa/admin_site.py`

 * *Files identical despite different names*

### Comparing `django-modal-2fa-0.0.3/modal_2fa/auth.py` & `django-modal-2fa-0.0.4/modal_2fa/auth.py`

 * *Files identical despite different names*

### Comparing `django-modal-2fa-0.0.3/modal_2fa/backends.py` & `django-modal-2fa-0.0.4/modal_2fa/backends.py`

 * *Files identical despite different names*

### Comparing `django-modal-2fa-0.0.3/modal_2fa/customise.py` & `django-modal-2fa-0.0.4/modal_2fa/customise.py`

 * *Files identical despite different names*

### Comparing `django-modal-2fa-0.0.3/modal_2fa/forms.py` & `django-modal-2fa-0.0.4/modal_2fa/forms.py`

 * *Files identical despite different names*

### Comparing `django-modal-2fa-0.0.3/modal_2fa/management/commands/clear_failed_logins.py` & `django-modal-2fa-0.0.4/modal_2fa/management/commands/clear_failed_logins.py`

 * *Files identical despite different names*

### Comparing `django-modal-2fa-0.0.3/modal_2fa/menus.py` & `django-modal-2fa-0.0.4/modal_2fa/menus.py`

 * *Files identical despite different names*

### Comparing `django-modal-2fa-0.0.3/modal_2fa/migrations/0001_initial.py` & `django-modal-2fa-0.0.4/modal_2fa/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-modal-2fa-0.0.3/modal_2fa/migrations/0002_failedloginattempt_webauthncredential.py` & `django-modal-2fa-0.0.4/modal_2fa/migrations/0002_failedloginattempt_webauthncredential.py`

 * *Files identical despite different names*

### Comparing `django-modal-2fa-0.0.3/modal_2fa/models.py` & `django-modal-2fa-0.0.4/modal_2fa/models.py`

 * *Files identical despite different names*

### Comparing `django-modal-2fa-0.0.3/modal_2fa/static/modal_2fa/webauthn.js` & `django-modal-2fa-0.0.4/modal_2fa/static/modal_2fa/webauthn.js`

 * *Files identical despite different names*

### Comparing `django-modal-2fa-0.0.3/modal_2fa/templates/modal_2fa/base.html` & `django-modal-2fa-0.0.4/modal_2fa/templates/modal_2fa/base.html`

 * *Files identical despite different names*

### Comparing `django-modal-2fa-0.0.3/modal_2fa/templates/modal_2fa/database_cookies.html` & `django-modal-2fa-0.0.4/modal_2fa/templates/modal_2fa/database_cookies.html`

 * *Files identical despite different names*

### Comparing `django-modal-2fa-0.0.3/modal_2fa/templates/modal_2fa/emails/password_reset_email.html` & `django-modal-2fa-0.0.4/modal_2fa/templates/modal_2fa/emails/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `django-modal-2fa-0.0.3/modal_2fa/templates/modal_2fa/webauthn_devices.html` & `django-modal-2fa-0.0.4/modal_2fa/templates/modal_2fa/webauthn_devices.html`

 * *Files identical despite different names*

### Comparing `django-modal-2fa-0.0.3/modal_2fa/urls.py` & `django-modal-2fa-0.0.4/modal_2fa/urls.py`

 * *Files identical despite different names*

### Comparing `django-modal-2fa-0.0.3/modal_2fa/user_admin.py` & `django-modal-2fa-0.0.4/modal_2fa/user_admin.py`

 * *Files identical despite different names*

### Comparing `django-modal-2fa-0.0.3/modal_2fa/users.py` & `django-modal-2fa-0.0.4/modal_2fa/users.py`

 * *Files identical despite different names*

### Comparing `django-modal-2fa-0.0.3/modal_2fa/webauthn.py` & `django-modal-2fa-0.0.4/modal_2fa/webauthn.py`

 * *Files identical despite different names*

### Comparing `django-modal-2fa-0.0.3/setup.py` & `django-modal-2fa-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-modal-2fa",
-    version="0.0.3",
+    version="0.0.4",
     author="Ian Jones",
     description="Django app to implement two factor authentication with bootstrap modals",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jonesim/django-2fa",
     include_package_data = True,
     packages=['modal_2fa'],
```


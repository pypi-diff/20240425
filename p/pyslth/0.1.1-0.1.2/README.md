# Comparing `tmp/pyslth-0.1.1.tar.gz` & `tmp/pyslth-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.1.1.tar", last modified: Thu Apr 25 14:56:25 2024, max compression
+gzip compressed data, was "pyslth-0.1.2.tar", last modified: Thu Apr 25 15:37:00 2024, max compression
```

## Comparing `pyslth-0.1.1.tar` & `pyslth-0.1.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-25 14:56:25.129640 pyslth-0.1.1/
--rw-r--r--   0 breno      (501) staff       (20)       59 2024-04-13 21:50:18.000000 pyslth-0.1.1/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-25 14:56:25.129425 pyslth-0.1.1/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-25 14:56:25.116414 pyslth-0.1.1/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-25 14:56:25.000000 pyslth-0.1.1/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)     1072 2024-04-25 14:56:25.000000 pyslth-0.1.1/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-04-25 14:56:25.000000 pyslth-0.1.1/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      146 2024-04-25 14:56:25.000000 pyslth-0.1.1/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-04-25 14:56:25.000000 pyslth-0.1.1/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      138 2024-04-14 18:56:42.000000 pyslth-0.1.1/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-04-25 14:56:25.129702 pyslth-0.1.1/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-04-25 14:56:16.000000 pyslth-0.1.1/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-25 14:56:25.122828 pyslth-0.1.1/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3774 2024-04-23 12:02:55.000000 pyslth-0.1.1/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6908 2024-04-16 09:47:23.000000 pyslth-0.1.1/slth/components.py
--rw-r--r--   0 breno      (501) staff       (20)     2149 2024-04-14 19:04:32.000000 pyslth-0.1.1/slth/conf.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-25 14:56:25.123494 pyslth-0.1.1/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.1.1/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.1.1/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    20172 2024-04-25 14:38:34.000000 pyslth-0.1.1/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.1.1/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)     2174 2024-04-22 07:56:01.000000 pyslth-0.1.1/slth/factory.py
--rw-r--r--   0 breno      (501) staff       (20)    25116 2024-04-24 14:52:21.000000 pyslth-0.1.1/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-25 14:56:25.123788 pyslth-0.1.1/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.1/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-25 14:56:25.124424 pyslth-0.1.1/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.1/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.1.1/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.1.1/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-25 14:56:25.126989 pyslth-0.1.1/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1396 2024-04-09 12:56:09.000000 pyslth-0.1.1/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.1.1/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)      602 2024-04-18 19:49:54.000000 pyslth-0.1.1/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
--rw-r--r--   0 breno      (501) staff       (20)      452 2024-04-23 08:05:28.000000 pyslth-0.1.1/slth/migrations/0004_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      451 2024-04-23 12:54:25.000000 pyslth-0.1.1/slth/migrations/0005_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.1/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     5330 2024-04-23 11:48:55.000000 pyslth-0.1.1/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.1.1/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.1.1/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    19210 2024-04-25 14:39:52.000000 pyslth-0.1.1/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.1.1/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-25 14:56:25.127497 pyslth-0.1.1/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     8995 2024-04-14 00:29:15.000000 pyslth-0.1.1/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    10955 2024-04-14 10:37:29.000000 pyslth-0.1.1/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    14390 2024-04-22 11:20:25.000000 pyslth-0.1.1/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-25 14:56:25.114724 pyslth-0.1.1/slth/static/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-25 14:56:25.128582 pyslth-0.1.1/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.1.1/slth/static/images/logo.png
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.1.1/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.1.1/slth/static/images/user.png
--rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.1.1/slth/statistics.py
--rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.1.1/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      893 2024-04-12 02:07:28.000000 pyslth-0.1.1/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1112 2024-04-24 15:04:09.000000 pyslth-0.1.1/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     1995 2024-04-18 12:26:48.000000 pyslth-0.1.1/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-25 15:37:00.995545 pyslth-0.1.2/
+-rw-r--r--   0 breno      (501) staff       (20)       59 2024-04-13 21:50:18.000000 pyslth-0.1.2/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-25 15:37:00.995353 pyslth-0.1.2/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-25 15:37:00.982915 pyslth-0.1.2/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-25 15:37:00.000000 pyslth-0.1.2/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)     1072 2024-04-25 15:37:00.000000 pyslth-0.1.2/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-04-25 15:37:00.000000 pyslth-0.1.2/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      146 2024-04-25 15:37:00.000000 pyslth-0.1.2/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-04-25 15:37:00.000000 pyslth-0.1.2/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      138 2024-04-14 18:56:42.000000 pyslth-0.1.2/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-04-25 15:37:00.995601 pyslth-0.1.2/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-04-25 15:36:43.000000 pyslth-0.1.2/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-25 15:37:00.989215 pyslth-0.1.2/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3774 2024-04-23 12:02:55.000000 pyslth-0.1.2/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6908 2024-04-16 09:47:23.000000 pyslth-0.1.2/slth/components.py
+-rw-r--r--   0 breno      (501) staff       (20)     2149 2024-04-14 19:04:32.000000 pyslth-0.1.2/slth/conf.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-25 15:37:00.989816 pyslth-0.1.2/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.1.2/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.1.2/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    20152 2024-04-25 15:33:18.000000 pyslth-0.1.2/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.1.2/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)     2174 2024-04-22 07:56:01.000000 pyslth-0.1.2/slth/factory.py
+-rw-r--r--   0 breno      (501) staff       (20)    25162 2024-04-25 15:16:26.000000 pyslth-0.1.2/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-25 15:37:00.990094 pyslth-0.1.2/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.2/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-25 15:37:00.990740 pyslth-0.1.2/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.2/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.1.2/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.1.2/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-25 15:37:00.993209 pyslth-0.1.2/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1396 2024-04-09 12:56:09.000000 pyslth-0.1.2/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.1.2/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)      602 2024-04-18 19:49:54.000000 pyslth-0.1.2/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
+-rw-r--r--   0 breno      (501) staff       (20)      452 2024-04-23 08:05:28.000000 pyslth-0.1.2/slth/migrations/0004_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      451 2024-04-23 12:54:25.000000 pyslth-0.1.2/slth/migrations/0005_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.2/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     5330 2024-04-23 11:48:55.000000 pyslth-0.1.2/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.1.2/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.1.2/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    19210 2024-04-25 14:39:52.000000 pyslth-0.1.2/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.1.2/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-25 15:37:00.993709 pyslth-0.1.2/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     8995 2024-04-14 00:29:15.000000 pyslth-0.1.2/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    10955 2024-04-14 10:37:29.000000 pyslth-0.1.2/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    14390 2024-04-22 11:20:25.000000 pyslth-0.1.2/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-25 15:37:00.981481 pyslth-0.1.2/slth/static/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-25 15:37:00.994718 pyslth-0.1.2/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.1.2/slth/static/images/logo.png
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.1.2/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.1.2/slth/static/images/user.png
+-rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.1.2/slth/statistics.py
+-rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.1.2/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      893 2024-04-12 02:07:28.000000 pyslth-0.1.2/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1112 2024-04-24 15:04:09.000000 pyslth-0.1.2/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     1995 2024-04-18 12:26:48.000000 pyslth-0.1.2/slth/views.py
```

### Comparing `pyslth-0.1.1/PKG-INFO` & `pyslth-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.1.1
+Version: 0.1.2
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.1.1/pyslth.egg-info/PKG-INFO` & `pyslth-0.1.2/pyslth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.1.1
+Version: 0.1.2
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.1.1/pyslth.egg-info/SOURCES.txt` & `pyslth-0.1.2/pyslth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/setup.py` & `pyslth-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.1.1/slth/__init__.py` & `pyslth-0.1.2/slth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/slth/components.py` & `pyslth-0.1.2/slth/components.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/slth/conf.py` & `pyslth-0.1.2/slth/conf.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/slth/db/models.py` & `pyslth-0.1.2/slth/db/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/slth/endpoints.py` & `pyslth-0.1.2/slth/endpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -528,16 +528,16 @@
 
     def get(self):
         return dict(
             {
                 "name": APPLICATON['title'],
                 "short_name": APPLICATON['title'],
                 "lang": 'pt-BR',
-                "start_url": build_url(self.request, "/app/login/"),
-                "scope": build_url(self.request, "/app/login/"),
+                "start_url": build_url(self.request, "/"),
+                "scope": build_url(self.request, "/"),
                 "display": "standalone",
                 "icons": [{
                     "src": build_url(self.request, APPLICATON['logo']),
                     "sizes": "192x192",
                     "type": "image/png"
                 }]
             }
```

### Comparing `pyslth-0.1.1/slth/factory.py` & `pyslth-0.1.2/slth/factory.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/slth/forms.py` & `pyslth-0.1.2/slth/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,14 +353,15 @@
 class Form(DjangoForm, FormMixin):
     
     def __init__(self, *args, request=None, endpoint=None, **kwargs):
         self.fieldsets = {}
         self.fields = dict(self.fieldsets)
         self.display_data = []
         self.controls = dict(hide=[], show=[], set={})
+        self.instance = kwargs.pop('instance', None)
         self.endpoint = endpoint
         self.request = request
         self._info = None
         self._values = {}
         self._title = type(self).__name__
         self._actions = {}
         self.parse_json()
@@ -572,15 +573,15 @@
         self.instance.user.save()
         return Response(message='Ação realizada com sucesso.', redirect='/api/dashboard/', store=dict(application=None))
 
 class SendPushNotificationForm(Form):
     message = CharField(label='Text', widget=Textarea())
 
     def submit(self):
-        send_push_web_notification(self.endpoint.source, self.cleaned_data['message'])
+        send_push_web_notification(self.instance, self.cleaned_data['message'])
         return Response(message='Notificação enviada com sucesso.')
 
 
 FIELD_TYPES = {
     'CharField': 'text',
     'EmailField': 'email',
     'DecimalField': 'decimal',
```

### Comparing `pyslth-0.1.1/slth/management/commands/integration_test.py` & `pyslth-0.1.2/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/slth/management/commands/sync.py` & `pyslth-0.1.2/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/slth/migrations/0001_initial.py` & `pyslth-0.1.2/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.1.2/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/slth/migrations/0003_rename_photo_profile_alter_profile_options.py` & `pyslth-0.1.2/slth/migrations/0003_rename_photo_profile_alter_profile_options.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/slth/models.py` & `pyslth-0.1.2/slth/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/slth/permissions.py` & `pyslth-0.1.2/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/slth/queryset.py` & `pyslth-0.1.2/slth/queryset.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/slth/roles.py` & `pyslth-0.1.2/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/slth/selenium/__init__.py` & `pyslth-0.1.2/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/slth/selenium/browser.py` & `pyslth-0.1.2/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/slth/serializer.py` & `pyslth-0.1.2/slth/serializer.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/slth/static/images/logo.png` & `pyslth-0.1.2/slth/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/slth/static/images/logo.svg` & `pyslth-0.1.2/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/slth/static/images/user.png` & `pyslth-0.1.2/slth/static/images/user.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/slth/statistics.py` & `pyslth-0.1.2/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/slth/tests.py` & `pyslth-0.1.2/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/slth/urls.py` & `pyslth-0.1.2/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/slth/utils.py` & `pyslth-0.1.2/slth/utils.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.1/slth/views.py` & `pyslth-0.1.2/slth/views.py`

 * *Files identical despite different names*


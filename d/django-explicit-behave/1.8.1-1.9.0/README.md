# Comparing `tmp/django-explicit-behave-1.8.1.tar.gz` & `tmp/django-explicit-behave-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/mpilia/workspace/django-explicit-behave/dist/tmp9z5cndcj/django-explicit-behave-1.8.1.tar", last modified: Wed May 25 13:10:53 2022, max compression
+gzip compressed data, was "/Users/mpilia/workspace/django-explicit-behave/dist/tmpcj_zj5_m/django-explicit-behave-1.9.0.tar", last modified: Tue Jun 28 13:59:43 2022, max compression
```

## Comparing `django-explicit-behave-1.8.1.tar` & `django-explicit-behave-1.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2022-05-25 13:10:53.705131 django-explicit-behave-1.8.1/
--rw-r--r--   0 mpilia     (501) staff       (20)        0 2020-12-22 16:12:37.000000 django-explicit-behave-1.8.1/MANIFEST.in
--rw-r--r--   0 mpilia     (501) staff       (20)      784 2022-05-25 13:10:53.705307 django-explicit-behave-1.8.1/PKG-INFO
--rw-r--r--   0 mpilia     (501) staff       (20)      118 2022-05-25 13:10:42.000000 django-explicit-behave-1.8.1/README.md
-drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2022-05-25 13:10:53.695850 django-explicit-behave-1.8.1/django_explicit_behave.egg-info/
--rw-r--r--   0 mpilia     (501) staff       (20)      784 2022-05-25 13:10:53.000000 django-explicit-behave-1.8.1/django_explicit_behave.egg-info/PKG-INFO
--rw-r--r--   0 mpilia     (501) staff       (20)      464 2022-05-25 13:10:53.000000 django-explicit-behave-1.8.1/django_explicit_behave.egg-info/SOURCES.txt
--rw-r--r--   0 mpilia     (501) staff       (20)        1 2022-05-25 13:10:53.000000 django-explicit-behave-1.8.1/django_explicit_behave.egg-info/dependency_links.txt
--rw-r--r--   0 mpilia     (501) staff       (20)        1 2020-12-22 16:48:16.000000 django-explicit-behave-1.8.1/django_explicit_behave.egg-info/not-zip-safe
--rw-r--r--   0 mpilia     (501) staff       (20)      124 2022-05-25 13:10:53.000000 django-explicit-behave-1.8.1/django_explicit_behave.egg-info/requires.txt
--rw-r--r--   0 mpilia     (501) staff       (20)       16 2022-05-25 13:10:53.000000 django-explicit-behave-1.8.1/django_explicit_behave.egg-info/top_level.txt
-drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2022-05-25 13:10:53.704451 django-explicit-behave-1.8.1/explicit_behave/
--rw-r--r--   0 mpilia     (501) staff       (20)       35 2022-05-25 13:10:42.000000 django-explicit-behave-1.8.1/explicit_behave/__init__.py
--rw-r--r--   0 mpilia     (501) staff       (20)     1013 2022-05-09 10:56:33.000000 django-explicit-behave-1.8.1/explicit_behave/_steps.py
--rw-r--r--   0 mpilia     (501) staff       (20)    14855 2022-05-09 10:56:33.000000 django-explicit-behave-1.8.1/explicit_behave/db.py
--rw-r--r--   0 mpilia     (501) staff       (20)     8291 2021-07-08 08:09:56.000000 django-explicit-behave-1.8.1/explicit_behave/http.py
--rw-r--r--   0 mpilia     (501) staff       (20)    13050 2020-12-22 15:15:07.000000 django-explicit-behave-1.8.1/explicit_behave/mocks.py
--rw-r--r--   0 mpilia     (501) staff       (20)    18930 2022-05-25 13:10:42.000000 django-explicit-behave-1.8.1/explicit_behave/utils.py
--rw-r--r--   0 mpilia     (501) staff       (20)       96 2022-05-25 13:10:53.706037 django-explicit-behave-1.8.1/setup.cfg
--rw-r--r--   0 mpilia     (501) staff       (20)     1355 2021-08-19 13:55:48.000000 django-explicit-behave-1.8.1/setup.py
+drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2022-06-28 13:59:43.861681 django-explicit-behave-1.9.0/
+-rw-r--r--   0 mpilia     (501) staff       (20)        0 2020-12-22 16:12:37.000000 django-explicit-behave-1.9.0/MANIFEST.in
+-rw-r--r--   0 mpilia     (501) staff       (20)      784 2022-06-28 13:59:43.861867 django-explicit-behave-1.9.0/PKG-INFO
+-rw-r--r--   0 mpilia     (501) staff       (20)      118 2022-05-25 13:10:42.000000 django-explicit-behave-1.9.0/README.md
+drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2022-06-28 13:59:43.854277 django-explicit-behave-1.9.0/django_explicit_behave.egg-info/
+-rw-r--r--   0 mpilia     (501) staff       (20)      784 2022-06-28 13:59:43.000000 django-explicit-behave-1.9.0/django_explicit_behave.egg-info/PKG-INFO
+-rw-r--r--   0 mpilia     (501) staff       (20)      464 2022-06-28 13:59:43.000000 django-explicit-behave-1.9.0/django_explicit_behave.egg-info/SOURCES.txt
+-rw-r--r--   0 mpilia     (501) staff       (20)        1 2022-06-28 13:59:43.000000 django-explicit-behave-1.9.0/django_explicit_behave.egg-info/dependency_links.txt
+-rw-r--r--   0 mpilia     (501) staff       (20)        1 2020-12-22 16:48:16.000000 django-explicit-behave-1.9.0/django_explicit_behave.egg-info/not-zip-safe
+-rw-r--r--   0 mpilia     (501) staff       (20)      124 2022-06-28 13:59:43.000000 django-explicit-behave-1.9.0/django_explicit_behave.egg-info/requires.txt
+-rw-r--r--   0 mpilia     (501) staff       (20)       16 2022-06-28 13:59:43.000000 django-explicit-behave-1.9.0/django_explicit_behave.egg-info/top_level.txt
+drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2022-06-28 13:59:43.860429 django-explicit-behave-1.9.0/explicit_behave/
+-rw-r--r--   0 mpilia     (501) staff       (20)       35 2022-06-28 13:57:42.000000 django-explicit-behave-1.9.0/explicit_behave/__init__.py
+-rw-r--r--   0 mpilia     (501) staff       (20)     1013 2022-05-09 10:56:33.000000 django-explicit-behave-1.9.0/explicit_behave/_steps.py
+-rw-r--r--   0 mpilia     (501) staff       (20)    14855 2022-05-09 10:56:33.000000 django-explicit-behave-1.9.0/explicit_behave/db.py
+-rw-r--r--   0 mpilia     (501) staff       (20)     8291 2021-07-08 08:09:56.000000 django-explicit-behave-1.9.0/explicit_behave/http.py
+-rw-r--r--   0 mpilia     (501) staff       (20)    13050 2020-12-22 15:15:07.000000 django-explicit-behave-1.9.0/explicit_behave/mocks.py
+-rw-r--r--   0 mpilia     (501) staff       (20)    19042 2022-06-28 09:07:55.000000 django-explicit-behave-1.9.0/explicit_behave/utils.py
+-rw-r--r--   0 mpilia     (501) staff       (20)       96 2022-06-28 13:59:43.862571 django-explicit-behave-1.9.0/setup.cfg
+-rw-r--r--   0 mpilia     (501) staff       (20)     1355 2021-08-19 13:55:48.000000 django-explicit-behave-1.9.0/setup.py
```

### Comparing `django-explicit-behave-1.8.1/PKG-INFO` & `django-explicit-behave-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-explicit-behave
-Version: 1.8.1
+Version: 1.9.0
 Summary: A collection of explicit behave steps for API testing
 Home-page: https://github.com/MaurizioPilia/django-explicit-behave
 Author: Maurizio Pilia, Javier Buzzi
 Author-email: piliamaurizio@gmail.com, buzzi.javier@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `django-explicit-behave-1.8.1/django_explicit_behave.egg-info/PKG-INFO` & `django-explicit-behave-1.9.0/django_explicit_behave.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-explicit-behave
-Version: 1.8.1
+Version: 1.9.0
 Summary: A collection of explicit behave steps for API testing
 Home-page: https://github.com/MaurizioPilia/django-explicit-behave
 Author: Maurizio Pilia, Javier Buzzi
 Author-email: piliamaurizio@gmail.com, buzzi.javier@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `django-explicit-behave-1.8.1/explicit_behave/_steps.py` & `django-explicit-behave-1.9.0/explicit_behave/_steps.py`

 * *Files identical despite different names*

### Comparing `django-explicit-behave-1.8.1/explicit_behave/db.py` & `django-explicit-behave-1.9.0/explicit_behave/db.py`

 * *Files identical despite different names*

### Comparing `django-explicit-behave-1.8.1/explicit_behave/http.py` & `django-explicit-behave-1.9.0/explicit_behave/http.py`

 * *Files identical despite different names*

### Comparing `django-explicit-behave-1.8.1/explicit_behave/mocks.py` & `django-explicit-behave-1.9.0/explicit_behave/mocks.py`

 * *Files identical despite different names*

### Comparing `django-explicit-behave-1.8.1/explicit_behave/utils.py` & `django-explicit-behave-1.9.0/explicit_behave/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import django
 from django.contrib.contenttypes.fields import GenericForeignKey
 
 if django.VERSION[0] >= 3:
     from django.db.models import JSONField
 else:
     from django.contrib.postgres.fields.jsonb import JSONField
+from django.db.models import UUIDField
 from django.core.exceptions import ValidationError, FieldDoesNotExist
 from django.core.management.color import no_style
 from django.core.serializers import python as serializers
 from django.core.serializers.json import DjangoJSONEncoder
 from django.db import connection
 from django.db.models import ForeignKey, TextField, CharField
 from django.db.models import fields as django_fields
@@ -345,18 +346,21 @@
     Reset a DB table's sequence to desired next_value.
 
     :param Model :type Model
     :param next_value :type int. If specified, set the sequence so the next value assigned is next_value.
                                  If unspecified, set the sequence so the next value is max(id) + 1.
     """
     try:
-        Model._meta.get_field('id')
+        primary_key = Model._meta.get_field('id')
     except FieldDoesNotExist:
         return  # If id field does not exist, do not reset the sequence.
 
+    if isinstance(primary_key, UUIDField):
+        return
+
     with connection.cursor() as cursor:
         if not next_value:
             # Find the highest id value in use if next_value is None or 0.
             cursor.execute(f"SELECT MAX(id) FROM {Model._meta.db_table}")
             highest_value = cursor.fetchone()[0]
 
             # If the table has a max(id) of None, it is empty so start the next value at 1.
```

### Comparing `django-explicit-behave-1.8.1/setup.py` & `django-explicit-behave-1.9.0/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/django-tcb-blog-0.9.1.tar.gz` & `tmp/django-tcb-blog-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-tcb-blog-0.9.1.tar", last modified: Mon Feb  1 11:04:49 2021, max compression
+gzip compressed data, was "django-tcb-blog-0.9.2.tar", last modified: Tue Feb  2 11:43:32 2021, max compression
```

## Comparing `django-tcb-blog-0.9.1.tar` & `django-tcb-blog-0.9.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 bjameson   (501) staff       (20)        0 2021-02-01 11:04:48.997427 django-tcb-blog-0.9.1/
--rw-r--r--   0 bjameson   (501) staff       (20)     1071 2020-06-16 22:51:02.000000 django-tcb-blog-0.9.1/LICENSE
--rw-r--r--   0 bjameson   (501) staff       (20)      102 2020-06-16 22:54:09.000000 django-tcb-blog-0.9.1/MANIFEST.in
--rw-r--r--   0 bjameson   (501) staff       (20)      880 2021-02-01 11:04:48.997715 django-tcb-blog-0.9.1/PKG-INFO
--rw-r--r--   0 bjameson   (501) staff       (20)      644 2020-09-21 09:56:39.000000 django-tcb-blog-0.9.1/README.rst
-drwxr-xr-x   0 bjameson   (501) staff       (20)        0 2021-02-01 11:04:48.971595 django-tcb-blog-0.9.1/blog/
--rw-r--r--   0 bjameson   (501) staff       (20)       45 2020-10-10 07:29:27.000000 django-tcb-blog-0.9.1/blog/__init__.py
--rw-r--r--   0 bjameson   (501) staff       (20)     1425 2021-01-24 20:56:29.000000 django-tcb-blog-0.9.1/blog/admin.py
--rw-r--r--   0 bjameson   (501) staff       (20)      133 2020-10-10 07:29:27.000000 django-tcb-blog-0.9.1/blog/apps.py
-drwxr-xr-x   0 bjameson   (501) staff       (20)        0 2021-02-01 11:04:48.994477 django-tcb-blog-0.9.1/blog/migrations/
--rw-r--r--   0 bjameson   (501) staff       (20)     1055 2020-03-04 11:38:59.000000 django-tcb-blog-0.9.1/blog/migrations/0001_initial.py
--rw-r--r--   0 bjameson   (501) staff       (20)      364 2020-03-04 11:38:59.000000 django-tcb-blog-0.9.1/blog/migrations/0002_entry_title.py
--rw-r--r--   0 bjameson   (501) staff       (20)      535 2020-03-04 11:38:59.000000 django-tcb-blog-0.9.1/blog/migrations/0003_auto_20200302_0056.py
--rw-r--r--   0 bjameson   (501) staff       (20)      538 2020-03-04 11:38:59.000000 django-tcb-blog-0.9.1/blog/migrations/0004_auto_20200302_0126.py
--rw-r--r--   0 bjameson   (501) staff       (20)      999 2020-03-04 11:38:59.000000 django-tcb-blog-0.9.1/blog/migrations/0005_profile.py
--rw-r--r--   0 bjameson   (501) staff       (20)      997 2020-03-04 11:38:59.000000 django-tcb-blog-0.9.1/blog/migrations/0006_comment.py
--rw-r--r--   0 bjameson   (501) staff       (20)      379 2020-03-04 11:38:59.000000 django-tcb-blog-0.9.1/blog/migrations/0007_entry_entry_id.py
--rw-r--r--   0 bjameson   (501) staff       (20)      408 2020-05-31 20:59:49.000000 django-tcb-blog-0.9.1/blog/migrations/0008_profile_gravatar_url.py
--rw-r--r--   0 bjameson   (501) staff       (20)      281 2020-05-31 20:59:49.000000 django-tcb-blog-0.9.1/blog/migrations/0009_auto_20200309_1619.py
--rw-r--r--   0 bjameson   (501) staff       (20)      362 2020-05-31 20:59:49.000000 django-tcb-blog-0.9.1/blog/migrations/0010_auto_20200309_1619.py
--rw-r--r--   0 bjameson   (501) staff       (20)      382 2020-10-10 07:29:27.000000 django-tcb-blog-0.9.1/blog/migrations/0011_entryenvelope_slug.py
--rw-r--r--   0 bjameson   (501) staff       (20)      766 2020-10-10 07:29:27.000000 django-tcb-blog-0.9.1/blog/migrations/0012_auto_20200604_0048.py
--rw-r--r--   0 bjameson   (501) staff       (20)      411 2020-10-10 07:29:27.000000 django-tcb-blog-0.9.1/blog/migrations/0013_entryenvelope_version.py
--rw-r--r--   0 bjameson   (501) staff       (20)      911 2020-10-10 07:29:27.000000 django-tcb-blog-0.9.1/blog/migrations/0014_auto_20200609_0947.py
--rw-r--r--   0 bjameson   (501) staff       (20)      392 2020-10-10 07:29:27.000000 django-tcb-blog-0.9.1/blog/migrations/0015_entryenvelope_defunct.py
--rw-r--r--   0 bjameson   (501) staff       (20)      408 2020-10-10 07:29:27.000000 django-tcb-blog-0.9.1/blog/migrations/0016_profile_token.py
--rw-r--r--   0 bjameson   (501) staff       (20)      398 2020-10-10 07:29:27.000000 django-tcb-blog-0.9.1/blog/migrations/0017_profile_url.py
--rw-r--r--   0 bjameson   (501) staff       (20)      438 2020-10-10 07:29:27.000000 django-tcb-blog-0.9.1/blog/migrations/0018_auto_20201009_2216.py
--rw-r--r--   0 bjameson   (501) staff       (20)      695 2020-10-10 10:39:19.000000 django-tcb-blog-0.9.1/blog/migrations/0019_auto_20201010_0842.py
--rw-r--r--   0 bjameson   (501) staff       (20)     1420 2021-01-19 12:37:13.000000 django-tcb-blog-0.9.1/blog/migrations/0020_auto_20210119_1042.py
--rw-r--r--   0 bjameson   (501) staff       (20)      392 2021-01-19 12:37:13.000000 django-tcb-blog-0.9.1/blog/migrations/0021_view_session_uid.py
--rw-r--r--   0 bjameson   (501) staff       (20)      401 2021-01-22 17:24:31.000000 django-tcb-blog-0.9.1/blog/migrations/0022_view_entry_id.py
--rw-r--r--   0 bjameson   (501) staff       (20)      532 2021-01-22 17:42:15.000000 django-tcb-blog-0.9.1/blog/migrations/0023_auto_20210122_1725.py
--rw-r--r--   0 bjameson   (501) staff       (20)     1162 2021-01-24 18:17:40.000000 django-tcb-blog-0.9.1/blog/migrations/0024_visitorprofile.py
--rw-r--r--   0 bjameson   (501) staff       (20)     1245 2021-01-24 19:19:08.000000 django-tcb-blog-0.9.1/blog/migrations/0025_auto_20210124_1919.py
--rw-r--r--   0 bjameson   (501) staff       (20)      568 2021-01-24 20:49:16.000000 django-tcb-blog-0.9.1/blog/migrations/0026_auto_20210124_2049.py
--rw-r--r--   0 bjameson   (501) staff       (20)      399 2021-01-24 20:53:29.000000 django-tcb-blog-0.9.1/blog/migrations/0027_visitorprofile_language.py
--rw-r--r--   0 bjameson   (501) staff       (20)     1326 2021-01-26 23:04:27.000000 django-tcb-blog-0.9.1/blog/migrations/0028_auto_20210126_2304.py
--rw-r--r--   0 bjameson   (501) staff       (20)     1245 2021-01-26 23:05:54.000000 django-tcb-blog-0.9.1/blog/migrations/0029_auto_20210126_2305.py
--rw-r--r--   0 bjameson   (501) staff       (20)      399 2021-01-27 22:51:43.000000 django-tcb-blog-0.9.1/blog/migrations/0030_interaction_session_uid.py
--rw-r--r--   0 bjameson   (501) staff       (20)        0 2020-03-04 11:38:59.000000 django-tcb-blog-0.9.1/blog/migrations/__init__.py
--rw-r--r--   0 bjameson   (501) staff       (20)     8187 2021-01-27 13:13:21.000000 django-tcb-blog-0.9.1/blog/models.py
--rw-r--r--   0 bjameson   (501) staff       (20)     1545 2021-01-24 21:08:46.000000 django-tcb-blog-0.9.1/blog/permissions.py
--rw-r--r--   0 bjameson   (501) staff       (20)     4775 2021-01-24 21:06:15.000000 django-tcb-blog-0.9.1/blog/serializers.py
--rw-r--r--   0 bjameson   (501) staff       (20)      539 2020-10-10 07:29:27.000000 django-tcb-blog-0.9.1/blog/signals.py
--rw-r--r--   0 bjameson   (501) staff       (20)      919 2020-10-10 07:29:27.000000 django-tcb-blog-0.9.1/blog/tasks.py
--rw-r--r--   0 bjameson   (501) staff       (20)      846 2021-02-01 10:40:17.000000 django-tcb-blog-0.9.1/blog/urls.py
--rw-r--r--   0 bjameson   (501) staff       (20)    10511 2021-02-01 11:04:06.000000 django-tcb-blog-0.9.1/blog/views.py
-drwxr-xr-x   0 bjameson   (501) staff       (20)        0 2021-02-01 11:04:48.996762 django-tcb-blog-0.9.1/django_tcb_blog.egg-info/
--rw-r--r--   0 bjameson   (501) staff       (20)      880 2021-02-01 11:04:48.000000 django-tcb-blog-0.9.1/django_tcb_blog.egg-info/PKG-INFO
--rw-r--r--   0 bjameson   (501) staff       (20)     1630 2021-02-01 11:04:48.000000 django-tcb-blog-0.9.1/django_tcb_blog.egg-info/SOURCES.txt
--rw-r--r--   0 bjameson   (501) staff       (20)        1 2021-02-01 11:04:48.000000 django-tcb-blog-0.9.1/django_tcb_blog.egg-info/dependency_links.txt
--rw-r--r--   0 bjameson   (501) staff       (20)        5 2021-02-01 11:04:48.000000 django-tcb-blog-0.9.1/django_tcb_blog.egg-info/top_level.txt
--rw-r--r--   0 bjameson   (501) staff       (20)      802 2021-02-01 11:04:48.998677 django-tcb-blog-0.9.1/setup.cfg
--rw-r--r--   0 bjameson   (501) staff       (20)       38 2020-06-16 22:52:46.000000 django-tcb-blog-0.9.1/setup.py
+drwxr-xr-x   0 bjameson   (501) staff       (20)        0 2021-02-02 11:43:32.959332 django-tcb-blog-0.9.2/
+-rw-r--r--   0 bjameson   (501) staff       (20)     1071 2020-06-16 22:51:02.000000 django-tcb-blog-0.9.2/LICENSE
+-rw-r--r--   0 bjameson   (501) staff       (20)      102 2020-06-16 22:54:09.000000 django-tcb-blog-0.9.2/MANIFEST.in
+-rw-r--r--   0 bjameson   (501) staff       (20)     2300 2021-02-02 11:43:32.959581 django-tcb-blog-0.9.2/PKG-INFO
+-rw-r--r--   0 bjameson   (501) staff       (20)     1017 2021-02-02 11:42:50.000000 django-tcb-blog-0.9.2/README.rst
+drwxr-xr-x   0 bjameson   (501) staff       (20)        0 2021-02-02 11:43:32.934294 django-tcb-blog-0.9.2/blog/
+-rw-r--r--   0 bjameson   (501) staff       (20)       45 2020-10-10 07:29:27.000000 django-tcb-blog-0.9.2/blog/__init__.py
+-rw-r--r--   0 bjameson   (501) staff       (20)     1425 2021-01-24 20:56:29.000000 django-tcb-blog-0.9.2/blog/admin.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      133 2020-10-10 07:29:27.000000 django-tcb-blog-0.9.2/blog/apps.py
+drwxr-xr-x   0 bjameson   (501) staff       (20)        0 2021-02-02 11:43:32.957364 django-tcb-blog-0.9.2/blog/migrations/
+-rw-r--r--   0 bjameson   (501) staff       (20)     1055 2020-03-04 11:38:59.000000 django-tcb-blog-0.9.2/blog/migrations/0001_initial.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      364 2020-03-04 11:38:59.000000 django-tcb-blog-0.9.2/blog/migrations/0002_entry_title.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      535 2020-03-04 11:38:59.000000 django-tcb-blog-0.9.2/blog/migrations/0003_auto_20200302_0056.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      538 2020-03-04 11:38:59.000000 django-tcb-blog-0.9.2/blog/migrations/0004_auto_20200302_0126.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      999 2020-03-04 11:38:59.000000 django-tcb-blog-0.9.2/blog/migrations/0005_profile.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      997 2020-03-04 11:38:59.000000 django-tcb-blog-0.9.2/blog/migrations/0006_comment.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      379 2020-03-04 11:38:59.000000 django-tcb-blog-0.9.2/blog/migrations/0007_entry_entry_id.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      408 2020-05-31 20:59:49.000000 django-tcb-blog-0.9.2/blog/migrations/0008_profile_gravatar_url.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      281 2020-05-31 20:59:49.000000 django-tcb-blog-0.9.2/blog/migrations/0009_auto_20200309_1619.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      362 2020-05-31 20:59:49.000000 django-tcb-blog-0.9.2/blog/migrations/0010_auto_20200309_1619.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      382 2020-10-10 07:29:27.000000 django-tcb-blog-0.9.2/blog/migrations/0011_entryenvelope_slug.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      766 2020-10-10 07:29:27.000000 django-tcb-blog-0.9.2/blog/migrations/0012_auto_20200604_0048.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      411 2020-10-10 07:29:27.000000 django-tcb-blog-0.9.2/blog/migrations/0013_entryenvelope_version.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      911 2020-10-10 07:29:27.000000 django-tcb-blog-0.9.2/blog/migrations/0014_auto_20200609_0947.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      392 2020-10-10 07:29:27.000000 django-tcb-blog-0.9.2/blog/migrations/0015_entryenvelope_defunct.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      408 2020-10-10 07:29:27.000000 django-tcb-blog-0.9.2/blog/migrations/0016_profile_token.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      398 2020-10-10 07:29:27.000000 django-tcb-blog-0.9.2/blog/migrations/0017_profile_url.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      438 2020-10-10 07:29:27.000000 django-tcb-blog-0.9.2/blog/migrations/0018_auto_20201009_2216.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      695 2020-10-10 10:39:19.000000 django-tcb-blog-0.9.2/blog/migrations/0019_auto_20201010_0842.py
+-rw-r--r--   0 bjameson   (501) staff       (20)     1420 2021-01-19 12:37:13.000000 django-tcb-blog-0.9.2/blog/migrations/0020_auto_20210119_1042.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      392 2021-01-19 12:37:13.000000 django-tcb-blog-0.9.2/blog/migrations/0021_view_session_uid.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      401 2021-01-22 17:24:31.000000 django-tcb-blog-0.9.2/blog/migrations/0022_view_entry_id.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      532 2021-01-22 17:42:15.000000 django-tcb-blog-0.9.2/blog/migrations/0023_auto_20210122_1725.py
+-rw-r--r--   0 bjameson   (501) staff       (20)     1162 2021-01-24 18:17:40.000000 django-tcb-blog-0.9.2/blog/migrations/0024_visitorprofile.py
+-rw-r--r--   0 bjameson   (501) staff       (20)     1245 2021-01-24 19:19:08.000000 django-tcb-blog-0.9.2/blog/migrations/0025_auto_20210124_1919.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      568 2021-01-24 20:49:16.000000 django-tcb-blog-0.9.2/blog/migrations/0026_auto_20210124_2049.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      399 2021-01-24 20:53:29.000000 django-tcb-blog-0.9.2/blog/migrations/0027_visitorprofile_language.py
+-rw-r--r--   0 bjameson   (501) staff       (20)     1326 2021-01-26 23:04:27.000000 django-tcb-blog-0.9.2/blog/migrations/0028_auto_20210126_2304.py
+-rw-r--r--   0 bjameson   (501) staff       (20)     1245 2021-01-26 23:05:54.000000 django-tcb-blog-0.9.2/blog/migrations/0029_auto_20210126_2305.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      399 2021-01-27 22:51:43.000000 django-tcb-blog-0.9.2/blog/migrations/0030_interaction_session_uid.py
+-rw-r--r--   0 bjameson   (501) staff       (20)        0 2020-03-04 11:38:59.000000 django-tcb-blog-0.9.2/blog/migrations/__init__.py
+-rw-r--r--   0 bjameson   (501) staff       (20)     8187 2021-01-27 13:13:21.000000 django-tcb-blog-0.9.2/blog/models.py
+-rw-r--r--   0 bjameson   (501) staff       (20)     1545 2021-01-24 21:08:46.000000 django-tcb-blog-0.9.2/blog/permissions.py
+-rw-r--r--   0 bjameson   (501) staff       (20)     4775 2021-01-24 21:06:15.000000 django-tcb-blog-0.9.2/blog/serializers.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      539 2020-10-10 07:29:27.000000 django-tcb-blog-0.9.2/blog/signals.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      919 2020-10-10 07:29:27.000000 django-tcb-blog-0.9.2/blog/tasks.py
+-rw-r--r--   0 bjameson   (501) staff       (20)      846 2021-02-01 10:40:17.000000 django-tcb-blog-0.9.2/blog/urls.py
+-rw-r--r--   0 bjameson   (501) staff       (20)    11972 2021-02-02 11:30:36.000000 django-tcb-blog-0.9.2/blog/views.py
+drwxr-xr-x   0 bjameson   (501) staff       (20)        0 2021-02-02 11:43:32.959022 django-tcb-blog-0.9.2/django_tcb_blog.egg-info/
+-rw-r--r--   0 bjameson   (501) staff       (20)     2300 2021-02-02 11:43:32.000000 django-tcb-blog-0.9.2/django_tcb_blog.egg-info/PKG-INFO
+-rw-r--r--   0 bjameson   (501) staff       (20)     1630 2021-02-02 11:43:32.000000 django-tcb-blog-0.9.2/django_tcb_blog.egg-info/SOURCES.txt
+-rw-r--r--   0 bjameson   (501) staff       (20)        1 2021-02-02 11:43:32.000000 django-tcb-blog-0.9.2/django_tcb_blog.egg-info/dependency_links.txt
+-rw-r--r--   0 bjameson   (501) staff       (20)        5 2021-02-02 11:43:32.000000 django-tcb-blog-0.9.2/django_tcb_blog.egg-info/top_level.txt
+-rw-r--r--   0 bjameson   (501) staff       (20)      820 2021-02-02 11:43:32.960319 django-tcb-blog-0.9.2/setup.cfg
+-rw-r--r--   0 bjameson   (501) staff       (20)      361 2021-02-02 11:34:20.000000 django-tcb-blog-0.9.2/setup.py
```

### Comparing `django-tcb-blog-0.9.1/LICENSE` & `django-tcb-blog-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-tcb-blog-0.9.1/blog/admin.py` & `django-tcb-blog-0.9.2/blog/admin.py`

 * *Files identical despite different names*

### Comparing `django-tcb-blog-0.9.1/blog/migrations/0001_initial.py` & `django-tcb-blog-0.9.2/blog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tcb-blog-0.9.1/blog/migrations/0003_auto_20200302_0056.py` & `django-tcb-blog-0.9.2/blog/migrations/0003_auto_20200302_0056.py`

 * *Files identical despite different names*

### Comparing `django-tcb-blog-0.9.1/blog/migrations/0004_auto_20200302_0126.py` & `django-tcb-blog-0.9.2/blog/migrations/0004_auto_20200302_0126.py`

 * *Files identical despite different names*

### Comparing `django-tcb-blog-0.9.1/blog/migrations/0005_profile.py` & `django-tcb-blog-0.9.2/blog/migrations/0005_profile.py`

 * *Files identical despite different names*

### Comparing `django-tcb-blog-0.9.1/blog/migrations/0006_comment.py` & `django-tcb-blog-0.9.2/blog/migrations/0006_comment.py`

 * *Files identical despite different names*

### Comparing `django-tcb-blog-0.9.1/blog/migrations/0012_auto_20200604_0048.py` & `django-tcb-blog-0.9.2/blog/migrations/0012_auto_20200604_0048.py`

 * *Files identical despite different names*

### Comparing `django-tcb-blog-0.9.1/blog/migrations/0014_auto_20200609_0947.py` & `django-tcb-blog-0.9.2/blog/migrations/0014_auto_20200609_0947.py`

 * *Files identical despite different names*

### Comparing `django-tcb-blog-0.9.1/blog/migrations/0019_auto_20201010_0842.py` & `django-tcb-blog-0.9.2/blog/migrations/0019_auto_20201010_0842.py`

 * *Files identical despite different names*

### Comparing `django-tcb-blog-0.9.1/blog/migrations/0020_auto_20210119_1042.py` & `django-tcb-blog-0.9.2/blog/migrations/0020_auto_20210119_1042.py`

 * *Files identical despite different names*

### Comparing `django-tcb-blog-0.9.1/blog/migrations/0023_auto_20210122_1725.py` & `django-tcb-blog-0.9.2/blog/migrations/0023_auto_20210122_1725.py`

 * *Files identical despite different names*

### Comparing `django-tcb-blog-0.9.1/blog/migrations/0024_visitorprofile.py` & `django-tcb-blog-0.9.2/blog/migrations/0024_visitorprofile.py`

 * *Files identical despite different names*

### Comparing `django-tcb-blog-0.9.1/blog/migrations/0025_auto_20210124_1919.py` & `django-tcb-blog-0.9.2/blog/migrations/0025_auto_20210124_1919.py`

 * *Files identical despite different names*

### Comparing `django-tcb-blog-0.9.1/blog/migrations/0026_auto_20210124_2049.py` & `django-tcb-blog-0.9.2/blog/migrations/0026_auto_20210124_2049.py`

 * *Files identical despite different names*

### Comparing `django-tcb-blog-0.9.1/blog/migrations/0028_auto_20210126_2304.py` & `django-tcb-blog-0.9.2/blog/migrations/0028_auto_20210126_2304.py`

 * *Files identical despite different names*

### Comparing `django-tcb-blog-0.9.1/blog/migrations/0029_auto_20210126_2305.py` & `django-tcb-blog-0.9.2/blog/migrations/0029_auto_20210126_2305.py`

 * *Files identical despite different names*

### Comparing `django-tcb-blog-0.9.1/blog/models.py` & `django-tcb-blog-0.9.2/blog/models.py`

 * *Files identical despite different names*

### Comparing `django-tcb-blog-0.9.1/blog/permissions.py` & `django-tcb-blog-0.9.2/blog/permissions.py`

 * *Files identical despite different names*

### Comparing `django-tcb-blog-0.9.1/blog/serializers.py` & `django-tcb-blog-0.9.2/blog/serializers.py`

 * *Files identical despite different names*

### Comparing `django-tcb-blog-0.9.1/blog/signals.py` & `django-tcb-blog-0.9.2/blog/signals.py`

 * *Files identical despite different names*

### Comparing `django-tcb-blog-0.9.1/blog/tasks.py` & `django-tcb-blog-0.9.2/blog/tasks.py`

 * *Files identical despite different names*

### Comparing `django-tcb-blog-0.9.1/blog/urls.py` & `django-tcb-blog-0.9.2/blog/urls.py`

 * *Files identical despite different names*

### Comparing `django-tcb-blog-0.9.1/blog/views.py` & `django-tcb-blog-0.9.2/blog/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import json
 import uuid
 from typing import Any
 from urllib.request import Request
 
+from django.conf import settings
 from django.contrib.auth.models import User, AnonymousUser
 from django.db.models import Q
 from django.utils import timezone
 from django_filters.rest_framework import DjangoFilterBackend
-from django.contrib.syndication.views import Feed
+from django.contrib.syndication.views import Feed, add_domain
 from django.contrib.sites.shortcuts import get_current_site
 
 from rest_framework import viewsets, generics, status, mixins
 from rest_framework.exceptions import PermissionDenied
 from rest_framework.permissions import IsAuthenticated
 from rest_framework.response import Response
 from rest_framework.decorators import action
@@ -260,23 +261,64 @@
 
             serializer.instance.save()
 
             headers = self.get_success_headers(serializer.data)
             return Response(serializer.data, status=status.HTTP_201_CREATED, headers=headers)
 
 
+USE_DEFAULTS = False
+
+
+DEFAULTS = {
+    'RSS_FEED_TITLE': 'Blog Feed',
+    'RSS_FEED_LINK': '/blog/',
+    'RSS_FEED_ITEM_DESC_TEMPLATE': 'feed/entries.html'
+}
+
+
+if not hasattr(settings, 'TCB_BLOG_SETTINGS'):
+    USE_DEFAULTS = True
+
+
+def get_setting(setting, USE_DEFAULTS):
+    if USE_DEFAULTS:
+        return DEFAULTS.get(setting)
+    else:
+        return settings.TCB_BLOG_SETTINGS.get(setting)
+
 class EntriesFeed(Feed):
-    title = "All Articles"
-    link = "/blog/"
-    description = "Every article posted to this blog"
+    title = get_setting('RSS_FEED_TITLE', USE_DEFAULTS)
+    link = get_setting('RSS_FEED_LINK', USE_DEFAULTS)
+    description_template = get_setting('RSS_FEED_ITEM_DESC_TEMPLATE', USE_DEFAULTS)
 
     def items(self):
         return EntryEnvelope.objects.filter(published=True, defunct=False).order_by('-create_date', 'entry_id',
                                                                      '-version').distinct('create_date', 'entry_id')
     def item_title(self, item):
         return item.title
 
-    def item_description(self, item):
-        return ""
-
     def item_link(self, item):
-        return '/blog/' + str(item.slug) + '/';
+        return self.link + str(item.slug) + '/';
+
+    def get_context_data(self, item, request, **kwargs):
+        context = super().get_context_data(**kwargs)
+        try:
+            current_site = get_current_site(request)
+            first_content_type = item.entry.get('sections')[0].get('contents')[0].get('type')
+            if first_content_type == 'media':
+                value = item.entry.get('sections')[0].get('contents')[0].get('value')
+                if 'http' in value:
+                    desc = '<img src=' + value + '>'
+                else:
+                    desc = '<img src=http://' + str(current_site) + '/' + value + '>'
+            else:
+                desc = '<p>' + item.entry.get('sections')[0].get('contents')[0].get('value') + '</p>'
+        except:
+            desc = ''
+
+        title = item.title
+        readmore_link = self.link + str(item.slug) + '/';
+
+        context['desc'] = desc
+        context['title'] = title
+        context['readmore_link'] = readmore_link
+        return context
```

### Comparing `django-tcb-blog-0.9.1/django_tcb_blog.egg-info/SOURCES.txt` & `django-tcb-blog-0.9.2/django_tcb_blog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-tcb-blog-0.9.1/setup.cfg` & `django-tcb-blog-0.9.2/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = django-tcb-blog
-version = 0.9.1
-description = A Django backend based on DRF for blogging
+version = 0.9.2
+description = A Django backend based on DRF for blogging from TheCodeBlogs
 url = https://www.thecodeblogs.com/
 author = Brent Jameson
 author_email = admin@thecodeblogs.com
 license = MIT
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
```


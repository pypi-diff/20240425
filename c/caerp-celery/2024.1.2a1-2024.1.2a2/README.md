# Comparing `tmp/caerp_celery-2024.1.2a1.tar.gz` & `tmp/caerp_celery-2024.1.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caerp_celery-2024.1.2a1.tar", last modified: Fri Mar 15 11:25:24 2024, max compression
+gzip compressed data, was "caerp_celery-2024.1.2a2.tar", last modified: Thu Apr 25 10:37:02 2024, max compression
```

## Comparing `caerp_celery-2024.1.2a1.tar` & `caerp_celery-2024.1.2a2.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-03-15 11:25:24.398501 caerp_celery-2024.1.2a1/
--rw-r--r--   0 gas       (1000) gas       (1000)      334 2024-03-06 11:08:10.000000 caerp_celery-2024.1.2a1/CHANGELOG
--rw-r--r--   0 gas       (1000) gas       (1000)       11 2024-03-15 11:24:47.000000 caerp_celery-2024.1.2a1/CURRENT_VERSION
--rw-r--r--   0 gas       (1000) gas       (1000)    35147 2020-06-24 14:37:06.000000 caerp_celery-2024.1.2a1/LICENSE.txt
--rw-r--r--   0 gas       (1000) gas       (1000)      210 2024-03-06 10:24:06.000000 caerp_celery-2024.1.2a1/MANIFEST.in
--rw-r--r--   0 gas       (1000) gas       (1000)     3213 2024-03-15 11:25:24.398501 caerp_celery-2024.1.2a1/PKG-INFO
--rw-r--r--   0 gas       (1000) gas       (1000)     2627 2024-03-05 16:04:43.000000 caerp_celery-2024.1.2a1/README.rst
--rw-r--r--   0 gas       (1000) gas       (1000)       46 2024-03-08 17:12:36.000000 caerp_celery-2024.1.2a1/requirements.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       38 2024-03-15 11:25:24.398501 caerp_celery-2024.1.2a1/setup.cfg
--rw-r--r--   0 gas       (1000) gas       (1000)     1372 2024-03-06 11:04:59.000000 caerp_celery-2024.1.2a1/setup.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-03-15 11:25:24.385502 caerp_celery-2024.1.2a1/src/
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-03-15 11:25:24.390502 caerp_celery-2024.1.2a1/src/caerp_celery/
--rw-r--r--   0 gas       (1000) gas       (1000)     4579 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a1/src/caerp_celery/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)     1789 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a1/src/caerp_celery/conf.py
--rw-r--r--   0 gas       (1000) gas       (1000)      585 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a1/src/caerp_celery/exception.py
--rw-r--r--   0 gas       (1000) gas       (1000)      576 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a1/src/caerp_celery/hacks.py
--rw-r--r--   0 gas       (1000) gas       (1000)      753 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a1/src/caerp_celery/interfaces.py
--rw-r--r--   0 gas       (1000) gas       (1000)      483 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a1/src/caerp_celery/locks.py
--rw-r--r--   0 gas       (1000) gas       (1000)     5747 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a1/src/caerp_celery/mail.py
--rw-r--r--   0 gas       (1000) gas       (1000)     7465 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a1/src/caerp_celery/models.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-03-15 11:25:24.394502 caerp_celery-2024.1.2a1/src/caerp_celery/parsers/
--rw-r--r--   0 gas       (1000) gas       (1000)     2163 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a1/src/caerp_celery/parsers/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3533 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a1/src/caerp_celery/parsers/cegid.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3133 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a1/src/caerp_celery/parsers/ebp.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3376 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a1/src/caerp_celery/parsers/isacompta.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3264 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a1/src/caerp_celery/parsers/quadra.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3391 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a1/src/caerp_celery/parsers/sage.py
--rw-r--r--   0 gas       (1000) gas       (1000)     5798 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a1/src/caerp_celery/parsers/sage_generation_expert.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-03-15 11:25:24.394502 caerp_celery-2024.1.2a1/src/caerp_celery/schedulers/
--rw-r--r--   0 gas       (1000) gas       (1000)       29 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a1/src/caerp_celery/schedulers/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)      428 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a1/src/caerp_celery/schedulers/tasks.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-03-15 11:25:24.397502 caerp_celery-2024.1.2a1/src/caerp_celery/tasks/
--rw-r--r--   0 gas       (1000) gas       (1000)    10899 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a1/src/caerp_celery/tasks/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)    39090 2024-03-05 16:01:26.000000 caerp_celery-2024.1.2a1/src/caerp_celery/tasks/accounting_measure_compute.py
--rw-r--r--   0 gas       (1000) gas       (1000)    14135 2024-03-05 16:01:26.000000 caerp_celery-2024.1.2a1/src/caerp_celery/tasks/accounting_parser.py
--rw-r--r--   0 gas       (1000) gas       (1000)    29193 2024-03-05 16:01:26.000000 caerp_celery-2024.1.2a1/src/caerp_celery/tasks/csv_import.py
--rw-r--r--   0 gas       (1000) gas       (1000)    21494 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a1/src/caerp_celery/tasks/export.py
--rw-r--r--   0 gas       (1000) gas       (1000)     2015 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a1/src/caerp_celery/tasks/json_import.py
--rw-r--r--   0 gas       (1000) gas       (1000)     4428 2024-03-05 16:01:26.000000 caerp_celery-2024.1.2a1/src/caerp_celery/tasks/mail.py
--rw-r--r--   0 gas       (1000) gas       (1000)     1423 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a1/src/caerp_celery/tasks/notification.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3397 2024-03-15 11:24:28.000000 caerp_celery-2024.1.2a1/src/caerp_celery/tasks/tasks.py
--rw-r--r--   0 gas       (1000) gas       (1000)      509 2024-03-15 11:23:43.000000 caerp_celery-2024.1.2a1/src/caerp_celery/tasks/user_connections.py
--rw-r--r--   0 gas       (1000) gas       (1000)     6914 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a1/src/caerp_celery/tasks/utils.py
--rw-r--r--   0 gas       (1000) gas       (1000)     2765 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a1/src/caerp_celery/transactional_task.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-03-15 11:25:24.392502 caerp_celery-2024.1.2a1/src/caerp_celery.egg-info/
--rw-r--r--   0 gas       (1000) gas       (1000)     3213 2024-03-15 11:25:23.000000 caerp_celery-2024.1.2a1/src/caerp_celery.egg-info/PKG-INFO
--rw-r--r--   0 gas       (1000) gas       (1000)     1379 2024-03-15 11:25:24.000000 caerp_celery-2024.1.2a1/src/caerp_celery.egg-info/SOURCES.txt
--rw-r--r--   0 gas       (1000) gas       (1000)        1 2024-03-15 11:25:24.000000 caerp_celery-2024.1.2a1/src/caerp_celery.egg-info/dependency_links.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       84 2024-03-15 11:25:24.000000 caerp_celery-2024.1.2a1/src/caerp_celery.egg-info/entry_points.txt
--rw-r--r--   0 gas       (1000) gas       (1000)        1 2024-03-06 10:23:24.000000 caerp_celery-2024.1.2a1/src/caerp_celery.egg-info/not-zip-safe
--rw-r--r--   0 gas       (1000) gas       (1000)       45 2024-03-15 11:25:24.000000 caerp_celery-2024.1.2a1/src/caerp_celery.egg-info/requires.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       13 2024-03-15 11:25:24.000000 caerp_celery-2024.1.2a1/src/caerp_celery.egg-info/top_level.txt
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-04-25 10:37:02.019475 caerp_celery-2024.1.2a2/
+-rw-r--r--   0 gas       (1000) gas       (1000)      334 2024-03-06 11:08:10.000000 caerp_celery-2024.1.2a2/CHANGELOG
+-rw-r--r--   0 gas       (1000) gas       (1000)       11 2024-04-25 10:36:14.000000 caerp_celery-2024.1.2a2/CURRENT_VERSION
+-rw-r--r--   0 gas       (1000) gas       (1000)    35147 2020-06-24 14:37:06.000000 caerp_celery-2024.1.2a2/LICENSE.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)      210 2024-03-06 10:24:06.000000 caerp_celery-2024.1.2a2/MANIFEST.in
+-rw-r--r--   0 gas       (1000) gas       (1000)     3213 2024-04-25 10:37:02.018475 caerp_celery-2024.1.2a2/PKG-INFO
+-rw-r--r--   0 gas       (1000) gas       (1000)     2627 2024-03-05 16:04:43.000000 caerp_celery-2024.1.2a2/README.rst
+-rw-r--r--   0 gas       (1000) gas       (1000)       46 2024-03-08 17:12:36.000000 caerp_celery-2024.1.2a2/requirements.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       38 2024-04-25 10:37:02.019475 caerp_celery-2024.1.2a2/setup.cfg
+-rw-r--r--   0 gas       (1000) gas       (1000)     1372 2024-03-06 11:04:59.000000 caerp_celery-2024.1.2a2/setup.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-04-25 10:37:02.001475 caerp_celery-2024.1.2a2/src/
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-04-25 10:37:02.006475 caerp_celery-2024.1.2a2/src/caerp_celery/
+-rw-r--r--   0 gas       (1000) gas       (1000)     4579 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     1789 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/conf.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      585 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/exception.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      576 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/hacks.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      753 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/interfaces.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      852 2024-04-25 10:10:38.000000 caerp_celery-2024.1.2a2/src/caerp_celery/locks.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     5747 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/mail.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     7465 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/models.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-04-25 10:37:02.010475 caerp_celery-2024.1.2a2/src/caerp_celery/parsers/
+-rw-r--r--   0 gas       (1000) gas       (1000)     2163 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/parsers/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3533 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/parsers/cegid.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3133 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/parsers/ebp.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3376 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/parsers/isacompta.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3264 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/parsers/quadra.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3391 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/parsers/sage.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     5798 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/parsers/sage_generation_expert.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-04-25 10:37:02.011475 caerp_celery-2024.1.2a2/src/caerp_celery/schedulers/
+-rw-r--r--   0 gas       (1000) gas       (1000)       29 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/schedulers/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      428 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/schedulers/tasks.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-04-25 10:37:02.018475 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/
+-rw-r--r--   0 gas       (1000) gas       (1000)    10899 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    39090 2024-03-05 16:01:26.000000 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/accounting_measure_compute.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    14135 2024-03-05 16:01:26.000000 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/accounting_parser.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    29193 2024-03-05 16:01:26.000000 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/csv_import.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    21494 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/export.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     2015 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/json_import.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      392 2024-04-25 07:56:31.000000 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/locks.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     4428 2024-03-05 16:01:26.000000 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/mail.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     1423 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/notification.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3397 2024-03-15 11:24:28.000000 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/tasks.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      509 2024-03-15 11:23:43.000000 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/user_connections.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     6912 2024-04-25 09:04:32.000000 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/utils.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     2765 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/transactional_task.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-04-25 10:37:02.008475 caerp_celery-2024.1.2a2/src/caerp_celery.egg-info/
+-rw-r--r--   0 gas       (1000) gas       (1000)     3213 2024-04-25 10:37:01.000000 caerp_celery-2024.1.2a2/src/caerp_celery.egg-info/PKG-INFO
+-rw-r--r--   0 gas       (1000) gas       (1000)     1411 2024-04-25 10:37:01.000000 caerp_celery-2024.1.2a2/src/caerp_celery.egg-info/SOURCES.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)        1 2024-04-25 10:37:01.000000 caerp_celery-2024.1.2a2/src/caerp_celery.egg-info/dependency_links.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       84 2024-04-25 10:37:01.000000 caerp_celery-2024.1.2a2/src/caerp_celery.egg-info/entry_points.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)        1 2024-03-06 10:23:24.000000 caerp_celery-2024.1.2a2/src/caerp_celery.egg-info/not-zip-safe
+-rw-r--r--   0 gas       (1000) gas       (1000)       45 2024-04-25 10:37:01.000000 caerp_celery-2024.1.2a2/src/caerp_celery.egg-info/requires.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       13 2024-04-25 10:37:01.000000 caerp_celery-2024.1.2a2/src/caerp_celery.egg-info/top_level.txt
```

### Comparing `caerp_celery-2024.1.2a1/LICENSE.txt` & `caerp_celery-2024.1.2a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/PKG-INFO` & `caerp_celery-2024.1.2a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caerp_celery
-Version: 2024.1.2a1
+Version: 2024.1.2a2
 Summary: caerp_celery
 Home-page: https://framagit.org/caerp/caerp_celery
 Author: Coopérer Pour Entreprendre
 Author-email: contact@endi.coop
 License: GPLv3
 Keywords: web wsgi bfg pylons pyramid celery
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `caerp_celery-2024.1.2a1/README.rst` & `caerp_celery-2024.1.2a2/README.rst`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/setup.py` & `caerp_celery-2024.1.2a2/setup.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/__init__.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/__init__.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/conf.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/conf.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/exception.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/exception.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/hacks.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/hacks.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/interfaces.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/interfaces.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/mail.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/mail.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/models.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/models.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/parsers/__init__.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/parsers/cegid.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/parsers/cegid.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/parsers/ebp.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/parsers/ebp.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/parsers/isacompta.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/parsers/isacompta.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/parsers/quadra.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/parsers/quadra.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/parsers/sage.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/parsers/sage.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/parsers/sage_generation_expert.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/parsers/sage_generation_expert.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/tasks/__init__.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/tasks/accounting_measure_compute.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/tasks/accounting_measure_compute.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/tasks/accounting_parser.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/tasks/accounting_parser.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/tasks/csv_import.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/tasks/csv_import.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/tasks/export.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/tasks/export.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/tasks/json_import.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/tasks/json_import.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/tasks/mail.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/tasks/mail.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/tasks/notification.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/tasks/notification.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/tasks/tasks.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/tasks/utils.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/tasks/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,15 +193,15 @@
     """
     Check the redis service is available
     """
     from pyramid_celery import celery_app
     from redis.exceptions import ConnectionError
 
     return_code = True
-    return_msg = None
+    return_msg = ""
     try:
         from celery.app.control import Inspect
 
         insp = Inspect(app=celery_app)
 
         stats = insp.stats()
         if not stats:
```

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery/transactional_task.py` & `caerp_celery-2024.1.2a2/src/caerp_celery/transactional_task.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery.egg-info/PKG-INFO` & `caerp_celery-2024.1.2a2/src/caerp_celery.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caerp-celery
-Version: 2024.1.2a1
+Version: 2024.1.2a2
 Summary: caerp_celery
 Home-page: https://framagit.org/caerp/caerp_celery
 Author: Coopérer Pour Entreprendre
 Author-email: contact@endi.coop
 License: GPLv3
 Keywords: web wsgi bfg pylons pyramid celery
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `caerp_celery-2024.1.2a1/src/caerp_celery.egg-info/SOURCES.txt` & `caerp_celery-2024.1.2a2/src/caerp_celery.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,12 +32,13 @@
 src/caerp_celery/schedulers/tasks.py
 src/caerp_celery/tasks/__init__.py
 src/caerp_celery/tasks/accounting_measure_compute.py
 src/caerp_celery/tasks/accounting_parser.py
 src/caerp_celery/tasks/csv_import.py
 src/caerp_celery/tasks/export.py
 src/caerp_celery/tasks/json_import.py
+src/caerp_celery/tasks/locks.py
 src/caerp_celery/tasks/mail.py
 src/caerp_celery/tasks/notification.py
 src/caerp_celery/tasks/tasks.py
 src/caerp_celery/tasks/user_connections.py
 src/caerp_celery/tasks/utils.py
```


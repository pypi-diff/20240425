# Comparing `tmp/wc-django-device-recognizer-0.1.1.tar.gz` & `tmp/wc-django-device-recognizer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wc-django-device-recognizer-0.1.1.tar", last modified: Fri Jul 22 09:54:43 2022, max compression
+gzip compressed data, was "wc-django-device-recognizer-0.1.2.tar", last modified: Thu Apr 25 08:24:19 2024, max compression
```

## Comparing `wc-django-device-recognizer-0.1.1.tar` & `wc-django-device-recognizer-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,377 @@
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-22 09:54:43.115090 wc-django-device-recognizer-0.1.1/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      342 2022-07-22 09:29:53.000000 wc-django-device-recognizer-0.1.1/CHANGELOG.md
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1072 2022-07-21 09:50:00.000000 wc-django-device-recognizer-0.1.1/LICENSE
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      163 2022-07-21 09:50:00.000000 wc-django-device-recognizer-0.1.1/MANIFEST.in
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1260 2022-07-21 09:50:00.000000 wc-django-device-recognizer-0.1.1/Makefile
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2580 2022-07-22 09:54:43.115090 wc-django-device-recognizer-0.1.1/PKG-INFO
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1638 2022-07-22 09:54:23.000000 wc-django-device-recognizer-0.1.1/README.md
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)       79 2022-07-22 09:54:43.115090 wc-django-device-recognizer-0.1.1/setup.cfg
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1643 2022-07-22 09:31:50.000000 wc-django-device-recognizer-0.1.1/setup.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      562 2022-07-21 09:50:00.000000 wc-django-device-recognizer-0.1.1/tox.ini
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-22 09:54:43.115090 wc-django-device-recognizer-0.1.1/wc_django_device_recognizer.egg-info/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2580 2022-07-22 09:54:42.000000 wc-django-device-recognizer-0.1.1/wc_django_device_recognizer.egg-info/PKG-INFO
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      847 2022-07-22 09:54:43.000000 wc-django-device-recognizer-0.1.1/wc_django_device_recognizer.egg-info/SOURCES.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2022-07-22 09:54:42.000000 wc-django-device-recognizer-0.1.1/wc_django_device_recognizer.egg-info/dependency_links.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      186 2022-07-22 09:54:42.000000 wc-django-device-recognizer-0.1.1/wc_django_device_recognizer.egg-info/requires.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       22 2022-07-22 09:54:42.000000 wc-django-device-recognizer-0.1.1/wc_django_device_recognizer.egg-info/top_level.txt
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-22 09:54:43.115090 wc-django-device-recognizer-0.1.1/wcd_device_recognizer/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      131 2022-07-22 09:54:34.000000 wc-django-device-recognizer-0.1.1/wcd_device_recognizer/__init__.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1527 2022-07-22 09:30:39.000000 wc-django-device-recognizer-0.1.1/wcd_device_recognizer/admin.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      352 2022-07-21 09:50:00.000000 wc-django-device-recognizer-0.1.1/wcd_device_recognizer/apps.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      259 2022-07-21 09:50:00.000000 wc-django-device-recognizer-0.1.1/wcd_device_recognizer/conf.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)       82 2022-07-21 09:50:00.000000 wc-django-device-recognizer-0.1.1/wcd_device_recognizer/const.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)       57 2022-07-21 09:50:00.000000 wc-django-device-recognizer-0.1.1/wcd_device_recognizer/discovery.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1125 2022-07-21 09:50:00.000000 wc-django-device-recognizer-0.1.1/wcd_device_recognizer/dtos.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-22 09:54:43.115090 wc-django-device-recognizer-0.1.1/wcd_device_recognizer/migrations/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     5876 2022-07-21 09:50:00.000000 wc-django-device-recognizer-0.1.1/wcd_device_recognizer/migrations/0001_initial.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-21 09:50:00.000000 wc-django-device-recognizer-0.1.1/wcd_device_recognizer/migrations/__init__.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     5795 2022-07-21 09:50:00.000000 wc-django-device-recognizer-0.1.1/wcd_device_recognizer/models.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-22 09:54:43.115090 wc-django-device-recognizer-0.1.1/wcd_device_recognizer/services/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-07-21 09:50:00.000000 wc-django-device-recognizer-0.1.1/wcd_device_recognizer/services/__init__.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     2558 2022-07-21 09:50:00.000000 wc-django-device-recognizer-0.1.1/wcd_device_recognizer/services/registry.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     4908 2022-07-22 09:30:57.000000 wc-django-device-recognizer-0.1.1/wcd_device_recognizer/services/request_resolver.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1478 2022-07-21 09:50:00.000000 wc-django-device-recognizer-0.1.1/wcd_device_recognizer/utils.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.405945 wc-django-device-recognizer-0.1.2/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      335 2024-04-25 08:22:20.000000 wc-django-device-recognizer-0.1.2/CHANGELOG.md
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1072 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/LICENSE
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      163 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/MANIFEST.in
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1254 2024-04-25 08:24:06.000000 wc-django-device-recognizer-0.1.2/Makefile
+-rw-r--r--   0 preusx    (1000) preusx    (1000)     2945 2024-04-25 08:24:19.405945 wc-django-device-recognizer-0.1.2/PKG-INFO
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1638 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/README.md
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)       79 2024-04-25 08:24:19.405945 wc-django-device-recognizer-0.1.2/setup.cfg
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1628 2024-04-25 08:03:50.000000 wc-django-device-recognizer-0.1.2/setup.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.381945 wc-django-device-recognizer-0.1.2/tests/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     2871 2024-04-25 08:21:10.000000 wc-django-device-recognizer-0.1.2/tests/test_registry.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     2444 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/tests/test_request_resolver.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      562 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/tox.ini
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.405945 wc-django-device-recognizer-0.1.2/wc_django_device_recognizer.egg-info/
+-rw-r--r--   0 preusx    (1000) preusx    (1000)     2945 2024-04-25 08:24:19.000000 wc-django-device-recognizer-0.1.2/wc_django_device_recognizer.egg-info/PKG-INFO
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)    10091 2024-04-25 08:24:19.000000 wc-django-device-recognizer-0.1.2/wc_django_device_recognizer.egg-info/SOURCES.txt
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)        1 2024-04-25 08:24:19.000000 wc-django-device-recognizer-0.1.2/wc_django_device_recognizer.egg-info/dependency_links.txt
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      171 2024-04-25 08:24:19.000000 wc-django-device-recognizer-0.1.2/wc_django_device_recognizer.egg-info/requires.txt
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)       22 2024-04-25 08:24:19.000000 wc-django-device-recognizer-0.1.2/wc_django_device_recognizer.egg-info/top_level.txt
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.381945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      131 2024-04-25 08:21:23.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/__init__.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1527 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/admin.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      352 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/apps.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      259 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/conf.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)       82 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/const.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)       57 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/discovery.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1138 2024-04-25 07:57:05.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/dtos.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.381945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/af/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/af/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/af/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/af/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ar/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ar/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      463 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ar/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3562 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ar/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ast/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ast/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ast/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ast/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/az/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/az/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/az/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/az/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/be/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/be/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      518 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/be/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3620 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/be/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bg/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bg/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bg/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bg/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bn/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/br/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/br/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      671 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/br/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3779 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/br/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bs/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bs/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      454 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bs/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3553 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bs/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ca/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ca/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ca/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ca/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/cs/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/cs/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      460 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/cs/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3559 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/cs/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/cy/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/cy/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      425 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/cy/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3524 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/cy/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/da/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/da/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/da/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/da/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/de/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/dsb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/dsb/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/dsb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3531 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/dsb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/el/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/el/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/el/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/el/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/en/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/eo/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/eo/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/eo/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/eo/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/es/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/et/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/et/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/et/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/et/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/eu/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/eu/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/eu/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/eu/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fa/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fa/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fa/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3475 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fa/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fi/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fi/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fi/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3475 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fy/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fy/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fy/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fy/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ga/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ga/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      418 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ga/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3517 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ga/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/gd/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/gd/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      441 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/gd/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3540 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/gd/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/gl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/gl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/gl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/gl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/he/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/he/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      474 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/he/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3573 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/he/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hi/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hi/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hi/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      452 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3551 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hsb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hsb/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hsb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3531 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hsb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hu/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hu/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hu/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hu/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hy/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hy/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hy/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hy/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ia/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ia/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ia/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ia/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/id/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/id/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ig/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ig/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ig/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ig/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/io/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/io/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/io/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/io/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/is/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/is/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      402 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/is/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3498 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/is/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/it/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ja/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ja/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ja/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ka/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ka/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      378 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ka/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3474 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ka/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kab/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kab/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kab/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kab/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      378 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3474 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/km/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/km/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/km/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/km/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kn/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3475 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ko/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ko/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ko/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ko/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ky/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ky/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ky/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ky/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lb/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lt/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lt/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      511 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3613 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lt/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lv/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lv/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      415 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lv/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3514 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lv/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      410 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3506 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ml/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ml/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ml/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ml/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mn/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ms/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ms/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ms/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ms/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/my/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/my/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/my/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/my/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nb/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ne/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ne/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ne/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ne/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nn/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/os/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/os/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/os/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/os/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pa/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pa/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pa/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pa/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      526 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3628 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pt/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pt/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pt/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ro/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ro/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      421 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ro/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3520 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ro/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ru/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      518 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3620 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      455 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3554 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3531 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sq/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sq/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sq/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sq/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      454 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3553 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sv/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sv/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sv/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sv/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sw/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sw/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sw/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sw/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ta/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ta/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ta/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ta/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/te/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/te/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/te/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/te/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tg/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tg/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tg/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tg/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/th/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/th/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/th/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/th/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3475 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tt/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tt/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tt/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/udm/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.405945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/udm/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/udm/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/udm/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/uk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.405945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/uk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      602 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/uk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3707 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/uk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.381945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ur/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.405945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ur/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ur/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ur/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.381945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/uz/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.405945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/uz/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/uz/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/uz/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.381945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/vi/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.405945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/vi/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/vi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/vi/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.405945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/migrations/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     5876 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/migrations/0001_initial.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/migrations/__init__.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     5795 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/models.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.405945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/services/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/services/__init__.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     2558 2024-04-25 08:00:59.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/services/registry.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     5000 2024-04-25 07:58:53.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/services/request_resolver.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1478 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/utils.py
```

### Comparing `wc-django-device-recognizer-0.1.1/LICENSE` & `wc-django-device-recognizer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.1/Makefile` & `wc-django-device-recognizer-0.1.2/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 package-publish:
 	rm -rf ./dist
 	python setup.py sdist
 	twine upload dist/*
 
 translations:
 	mkdir -p wcd_device_recognizer/locale
-	django-admin.py makemessages --ignore=pilot/* --ignore=tests/* --ignore=dist/* \
+	django-admin makemessages --ignore=pilot/* --ignore=tests/* --ignore=dist/* \
 		-l af \
 		-l ar \
 		-l ar-dz \
 		-l ast \
 		-l az \
 		-l bg \
 		-l be \
@@ -99,8 +99,8 @@
 		-l udm \
 		-l uk \
 		-l ur \
 		-l uz \
 		-l vi \
 		-l zh-hans \
 		-l zh-hant
-	django-admin.py compilemessages
+	django-admin compilemessages
```

### Comparing `wc-django-device-recognizer-0.1.1/PKG-INFO` & `wc-django-device-recognizer-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 Metadata-Version: 2.1
 Name: wc-django-device-recognizer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Django device recognizing utility.
-Home-page: UNKNOWN
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: px-settings<0.2.0,>=0.1.3
+Requires-Dist: django-user-agents<1.0.0,>=0.4.0
+Provides-Extra: dev
+Requires-Dist: pytest<7.0,>=6.0; extra == "dev"
+Requires-Dist: pytest-watch<5.0,>=4.2; extra == "dev"
+Requires-Dist: pytest-django<5.0,>=4.3; extra == "dev"
+Requires-Dist: django-environ; extra == "dev"
+Requires-Dist: django-stubs; extra == "dev"
+Requires-Dist: django; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 
 # WebCase device recognizing utility
 
 ## Installation
 
 ```sh
 pip install wc-django-device-recognizer
@@ -90,15 +97,13 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
-## [0.1.4]
+## [0.1.2]
 ### Added
-- Translation strings.
+- IPv6 support.
 
 ## [0.1.1]
 Initial version.
-
-
```

### Comparing `wc-django-device-recognizer-0.1.1/README.md` & `wc-django-device-recognizer-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.1/setup.py` & `wc-django-device-recognizer-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     ),
     include_package_data=True,
     extras_require={
         'dev': (
             'pytest>=6.0,<7.0',
             'pytest-watch>=4.2,<5.0',
             'pytest-django>=4.3,<5.0',
-            'django-environ==0.4.5',
+            'django-environ',
             'django-stubs',
-            'django>=2.2,<4',
+            'django',
             'twine',
         ),
     },
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(exclude=(
         'tests', 'tests.*',
```

### Comparing `wc-django-device-recognizer-0.1.1/tox.ini` & `wc-django-device-recognizer-0.1.2/tox.ini`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.1/wc_django_device_recognizer.egg-info/PKG-INFO` & `wc-django-device-recognizer-0.1.2/wc_django_device_recognizer.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 Metadata-Version: 2.1
 Name: wc-django-device-recognizer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Django device recognizing utility.
-Home-page: UNKNOWN
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: px-settings<0.2.0,>=0.1.3
+Requires-Dist: django-user-agents<1.0.0,>=0.4.0
+Provides-Extra: dev
+Requires-Dist: pytest<7.0,>=6.0; extra == "dev"
+Requires-Dist: pytest-watch<5.0,>=4.2; extra == "dev"
+Requires-Dist: pytest-django<5.0,>=4.3; extra == "dev"
+Requires-Dist: django-environ; extra == "dev"
+Requires-Dist: django-stubs; extra == "dev"
+Requires-Dist: django; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 
 # WebCase device recognizing utility
 
 ## Installation
 
 ```sh
 pip install wc-django-device-recognizer
@@ -90,15 +97,13 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
-## [0.1.4]
+## [0.1.2]
 ### Added
-- Translation strings.
+- IPv6 support.
 
 ## [0.1.1]
 Initial version.
-
-
```

### Comparing `wc-django-device-recognizer-0.1.1/wcd_device_recognizer/admin.py` & `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/admin.py`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.1/wcd_device_recognizer/dtos.py` & `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/dtos.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from typing import *
 from dataclasses import dataclass, field
-from ipaddress import IPv4Address
+from ipaddress import IPv4Address, IPv6Address
 from decimal import Decimal
-from typing import Dict, Optional, Tuple
 from user_agents.parsers import UserAgent
 
 from .const import DEFAULT_DPR
 
 
 __all__ = 'AppDTO', 'OSDTO', 'DeviceDTO', 'InterlocutorDTO',
 
@@ -44,8 +44,8 @@
 class InterlocutorDTO:
     os: OSDTO
     app: AppDTO
     device: DeviceDTO
 
     user_agent: UserAgent
     client_hints: Dict[str, str] = field(default_factory=dict)
-    ip: Optional[IPv4Address] = None
+    ip: Optional[Union[IPv4Address, IPv6Address]] = None
```

### Comparing `wc-django-device-recognizer-0.1.1/wcd_device_recognizer/migrations/0001_initial.py` & `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.1/wcd_device_recognizer/models.py` & `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/models.py`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.1/wcd_device_recognizer/services/registry.py` & `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/services/registry.py`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.1/wcd_device_recognizer/services/request_resolver.py` & `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/services/request_resolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from decimal import Decimal
-from ipaddress import IPv4Address
+from ipaddress import ip_address
 from django.http import HttpRequest
 
 from django_user_agents.utils import get_user_agent
 from user_agents.parsers import UserAgent, parse_version
 from ua_parser.user_agent_parser import ParseUserAgent
 
 from ..const import DEFAULT_DPR
@@ -153,16 +153,22 @@
     ip = request.META.get('HTTP_X_FORWARDED_FOR')
 
     if ip:
         ip = ip.split(',')[0]
     else:
         ip = request.META.get('REMOTE_ADDR')
 
+    if ip:
+        try:
+            ip = ip_address(ip)
+        except ValueError:
+            ip = None
+
     return InterlocutorDTO(
-        ip=IPv4Address(ip) if ip else None,
+        ip=ip if ip else None,
         os=collect_os_data(ua, client_hints),
         app=collect_app_data(ua, client_hints),
         device=collect_device_data(ua, client_hints),
 
         user_agent=ua,
         client_hints=client_hints,
     )
```

### Comparing `wc-django-device-recognizer-0.1.1/wcd_device_recognizer/utils.py` & `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/utils.py`

 * *Files identical despite different names*


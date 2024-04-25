# Comparing `tmp/m9s_nereid_catalog-7.0.0.tar.gz` & `tmp/m9s_nereid_catalog-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m9s_nereid_catalog-7.0.0.tar", last modified: Mon Feb  5 10:23:41 2024, max compression
+gzip compressed data, was "m9s_nereid_catalog-7.0.1.tar", last modified: Thu Apr 25 14:10:48 2024, max compression
```

## Comparing `m9s_nereid_catalog-7.0.0.tar` & `m9s_nereid_catalog-7.0.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-05 10:23:41.239182 m9s_nereid_catalog-7.0.0/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       84 2024-01-22 10:56:08.000000 m9s_nereid_catalog-7.0.0/.coveragerc
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-13 19:22:51.000000 m9s_nereid_catalog-7.0.0/.drone.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-01-22 10:56:08.000000 m9s_nereid_catalog-7.0.0/.flake8
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-01-22 10:56:08.000000 m9s_nereid_catalog-7.0.0/.gitlab-ci-m9s.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1905 2024-01-22 10:56:08.000000 m9s_nereid_catalog-7.0.0/.gitlab-ci.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2024-01-22 10:56:08.000000 m9s_nereid_catalog-7.0.0/.isort.cfg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      234 2021-01-25 09:35:18.000000 m9s_nereid_catalog-7.0.0/.travis.yml
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-05 10:23:41.235182 m9s_nereid_catalog-7.0.0/.woodpecker/
--rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2024-01-22 10:56:08.000000 m9s_nereid_catalog-7.0.0/.woodpecker/mail_curl.sh
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2024-01-22 10:56:08.000000 m9s_nereid_catalog-7.0.0/.woodpecker/report.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2024-01-22 10:56:08.000000 m9s_nereid_catalog-7.0.0/.woodpecker/test.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1335 2022-11-13 21:11:37.000000 m9s_nereid_catalog-7.0.0/.woodpecker.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      995 2021-01-25 09:35:18.000000 m9s_nereid_catalog-7.0.0/CHANGELOG
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      794 2024-01-22 10:56:08.000000 m9s_nereid_catalog-7.0.0/COPYRIGHT
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2024-01-22 10:56:08.000000 m9s_nereid_catalog-7.0.0/INSTALL
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2024-01-22 10:56:08.000000 m9s_nereid_catalog-7.0.0/LICENSE
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2024-01-22 10:56:08.000000 m9s_nereid_catalog-7.0.0/MANIFEST.in
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3419 2024-02-05 10:23:41.239182 m9s_nereid_catalog-7.0.0/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1245 2024-01-22 10:56:08.000000 m9s_nereid_catalog-7.0.0/README.md
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       44 2024-01-22 10:56:08.000000 m9s_nereid_catalog-7.0.0/README.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      465 2024-01-22 10:56:08.000000 m9s_nereid_catalog-7.0.0/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-01-22 10:56:08.000000 m9s_nereid_catalog-7.0.0/dev_requirements.txt
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-05 10:23:41.235182 m9s_nereid_catalog-7.0.0/doc/
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-05 10:23:41.235182 m9s_nereid_catalog-7.0.0/doc/de/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       43 2024-01-22 10:56:08.000000 m9s_nereid_catalog-7.0.0/doc/de/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       44 2024-01-22 10:56:08.000000 m9s_nereid_catalog-7.0.0/doc/index.rst
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-05 10:23:41.235182 m9s_nereid_catalog-7.0.0/locale/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4607 2021-02-26 18:50:58.000000 m9s_nereid_catalog-7.0.0/locale/de.po
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-05 10:23:41.239182 m9s_nereid_catalog-7.0.0/m9s_nereid_catalog.egg-info/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3419 2024-02-05 10:23:41.000000 m9s_nereid_catalog-7.0.0/m9s_nereid_catalog.egg-info/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1182 2024-02-05 10:23:41.000000 m9s_nereid_catalog-7.0.0/m9s_nereid_catalog.egg-info/SOURCES.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-02-05 10:23:41.000000 m9s_nereid_catalog-7.0.0/m9s_nereid_catalog.egg-info/dependency_links.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       66 2024-02-05 10:23:41.000000 m9s_nereid_catalog-7.0.0/m9s_nereid_catalog.egg-info/entry_points.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2021-03-02 23:30:39.000000 m9s_nereid_catalog-7.0.0/m9s_nereid_catalog.egg-info/not-zip-safe
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      147 2024-02-05 10:23:41.000000 m9s_nereid_catalog-7.0.0/m9s_nereid_catalog.egg-info/requires.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-02-05 10:23:41.000000 m9s_nereid_catalog-7.0.0/m9s_nereid_catalog.egg-info/top_level.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      334 2022-02-15 12:42:45.000000 m9s_nereid_catalog-7.0.0/message.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    16973 2024-02-05 10:23:29.000000 m9s_nereid_catalog-7.0.0/product.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2345 2024-02-04 13:03:39.000000 m9s_nereid_catalog-7.0.0/product.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2024-01-22 10:56:08.000000 m9s_nereid_catalog-7.0.0/requirements.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      207 2024-02-05 10:23:41.239182 m9s_nereid_catalog-7.0.0/setup.cfg
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4510 2024-02-04 13:15:24.000000 m9s_nereid_catalog-7.0.0/setup.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-05 10:23:41.235182 m9s_nereid_catalog-7.0.0/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      115 2024-01-22 10:56:08.000000 m9s_nereid_catalog-7.0.0/tests/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    24038 2024-02-05 08:34:17.000000 m9s_nereid_catalog-7.0.0/tests/test_module.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2024-01-22 10:56:08.000000 m9s_nereid_catalog-7.0.0/tox.ini
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      129 2024-02-04 13:01:56.000000 m9s_nereid_catalog-7.0.0/tryton.cfg
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-05 10:23:41.235182 m9s_nereid_catalog-7.0.0/view/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      395 2021-01-25 09:35:18.000000 m9s_nereid_catalog-7.0.0/view/nereid_website_product.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1270 2021-12-11 18:21:21.000000 m9s_nereid_catalog-7.0.0/view/product_form_nereid.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      278 2021-01-25 09:35:18.000000 m9s_nereid_catalog-7.0.0/view/product_media_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      217 2021-01-25 09:35:18.000000 m9s_nereid_catalog-7.0.0/view/product_media_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      926 2021-01-25 09:35:18.000000 m9s_nereid_catalog-7.0.0/view/template_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1011 2024-01-22 10:56:08.000000 m9s_nereid_catalog-7.0.0/website.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:10:48.126110 m9s_nereid_catalog-7.0.1/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       84 2024-04-25 09:39:28.000000 m9s_nereid_catalog-7.0.1/.coveragerc
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-13 19:22:51.000000 m9s_nereid_catalog-7.0.1/.drone.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-04-25 09:39:28.000000 m9s_nereid_catalog-7.0.1/.flake8
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-04-25 09:39:28.000000 m9s_nereid_catalog-7.0.1/.gitlab-ci-m9s.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2217 2024-04-25 09:39:28.000000 m9s_nereid_catalog-7.0.1/.gitlab-ci.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2024-04-25 09:39:28.000000 m9s_nereid_catalog-7.0.1/.isort.cfg
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      234 2021-01-25 09:35:18.000000 m9s_nereid_catalog-7.0.1/.travis.yml
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:10:48.122110 m9s_nereid_catalog-7.0.1/.woodpecker/
+-rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2024-04-25 09:39:28.000000 m9s_nereid_catalog-7.0.1/.woodpecker/mail_curl.sh
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2024-04-25 09:39:28.000000 m9s_nereid_catalog-7.0.1/.woodpecker/report.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2024-04-25 09:39:28.000000 m9s_nereid_catalog-7.0.1/.woodpecker/test.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1335 2022-11-13 21:11:37.000000 m9s_nereid_catalog-7.0.1/.woodpecker.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      995 2021-01-25 09:35:18.000000 m9s_nereid_catalog-7.0.1/CHANGELOG
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      794 2024-04-25 09:39:28.000000 m9s_nereid_catalog-7.0.1/COPYRIGHT
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2024-04-25 09:39:28.000000 m9s_nereid_catalog-7.0.1/INSTALL
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2024-04-25 09:39:28.000000 m9s_nereid_catalog-7.0.1/LICENSE
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2024-04-25 09:39:28.000000 m9s_nereid_catalog-7.0.1/MANIFEST.in
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3231 2024-04-25 14:10:48.126110 m9s_nereid_catalog-7.0.1/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1057 2024-04-25 09:39:28.000000 m9s_nereid_catalog-7.0.1/README.md
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       44 2024-04-25 09:39:28.000000 m9s_nereid_catalog-7.0.1/README.rst
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      465 2024-04-25 09:39:28.000000 m9s_nereid_catalog-7.0.1/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       86 2024-04-25 09:39:28.000000 m9s_nereid_catalog-7.0.1/dev_requirements.txt
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:10:48.122110 m9s_nereid_catalog-7.0.1/doc/
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:10:48.122110 m9s_nereid_catalog-7.0.1/doc/de/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       43 2024-04-25 09:39:28.000000 m9s_nereid_catalog-7.0.1/doc/de/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       44 2024-04-25 09:39:28.000000 m9s_nereid_catalog-7.0.1/doc/index.rst
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:10:48.122110 m9s_nereid_catalog-7.0.1/locale/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4607 2021-02-26 18:50:58.000000 m9s_nereid_catalog-7.0.1/locale/de.po
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:10:48.126110 m9s_nereid_catalog-7.0.1/m9s_nereid_catalog.egg-info/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3231 2024-04-25 14:10:47.000000 m9s_nereid_catalog-7.0.1/m9s_nereid_catalog.egg-info/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1182 2024-04-25 14:10:48.000000 m9s_nereid_catalog-7.0.1/m9s_nereid_catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-04-25 14:10:47.000000 m9s_nereid_catalog-7.0.1/m9s_nereid_catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       66 2024-04-25 14:10:47.000000 m9s_nereid_catalog-7.0.1/m9s_nereid_catalog.egg-info/entry_points.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2021-03-02 23:30:39.000000 m9s_nereid_catalog-7.0.1/m9s_nereid_catalog.egg-info/not-zip-safe
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      147 2024-04-25 14:10:47.000000 m9s_nereid_catalog-7.0.1/m9s_nereid_catalog.egg-info/requires.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-04-25 14:10:47.000000 m9s_nereid_catalog-7.0.1/m9s_nereid_catalog.egg-info/top_level.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      334 2022-02-15 12:42:45.000000 m9s_nereid_catalog-7.0.1/message.xml
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    17382 2024-04-25 09:34:16.000000 m9s_nereid_catalog-7.0.1/product.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2345 2024-02-04 13:03:39.000000 m9s_nereid_catalog-7.0.1/product.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2024-04-25 09:39:28.000000 m9s_nereid_catalog-7.0.1/requirements.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      207 2024-04-25 14:10:48.126110 m9s_nereid_catalog-7.0.1/setup.cfg
+-rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     4510 2024-04-25 09:39:28.000000 m9s_nereid_catalog-7.0.1/setup.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:10:48.122110 m9s_nereid_catalog-7.0.1/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      115 2024-04-25 09:39:28.000000 m9s_nereid_catalog-7.0.1/tests/__init__.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    24038 2024-04-25 09:39:28.000000 m9s_nereid_catalog-7.0.1/tests/test_module.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2024-04-25 09:39:28.000000 m9s_nereid_catalog-7.0.1/tox.ini
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      129 2024-04-25 09:39:28.000000 m9s_nereid_catalog-7.0.1/tryton.cfg
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:10:48.122110 m9s_nereid_catalog-7.0.1/view/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      395 2021-01-25 09:35:18.000000 m9s_nereid_catalog-7.0.1/view/nereid_website_product.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1270 2021-12-11 18:21:21.000000 m9s_nereid_catalog-7.0.1/view/product_form_nereid.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      278 2021-01-25 09:35:18.000000 m9s_nereid_catalog-7.0.1/view/product_media_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      217 2021-01-25 09:35:18.000000 m9s_nereid_catalog-7.0.1/view/product_media_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      926 2021-01-25 09:35:18.000000 m9s_nereid_catalog-7.0.1/view/template_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1011 2024-01-22 10:56:08.000000 m9s_nereid_catalog-7.0.1/website.py
```

### Comparing `m9s_nereid_catalog-7.0.0/.drone.yml` & `m9s_nereid_catalog-7.0.1/.drone.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog-7.0.0/.gitlab-ci.yml` & `m9s_nereid_catalog-7.0.1/.gitlab-ci.yml`

 * *Files 15% similar despite different names*

```diff
@@ -47,37 +47,43 @@
 #    - tox -e py311-postgresql -vv -- -v
 #  tags:
 #    - postgres
 
 test-sqlite:
   <<: *test_base
   script:
-    - tox -e py311-sqlite -vv -- -v
+    - tox -e py311-sqlite -vv -- -v --output-file junit.xml
+    - coverage xml
     - coverage html
     - coverage report -m
-    # 20131213: coverage-badge not Python 3.12 ready
-    - coverage-badge
-
-  coverage: '/TOTAL.+ ([0-9]{1,3}%)/'
-      
+    - genbadge tests -i - < junit.xml -o reports/junit/junit-badge.svg
+    - genbadge coverage -i - < coverage.xml -o reports/coverage/coverage-badge.svg
+  coverage: '/(?i)total.*? (100(?:\.0+)?\%|[1-9]?\d(?:\.\d+)?\%)$/'
   artifacts:
     when: always
+    reports:
+      junit: junit.xml
+      coverage_report:
+        coverage_format: cobertura
+        path: coverage.xml
     paths:
       - htmlcov
+      - reports
     expire_in: 30 days
 
 pages:
   stage: pages
   #dependencies:
   #   - test-sqlite
   script:
     # delete everything in the current public folder
     # and replace with code coverage HTML report
     - mkdir -p public
     - rm -rf public/*
     - cp -r htmlcov/* public/
+    - cp -r reports/* public/
   artifacts:
     paths:
       - public
     expire_in: 30 days
   only:
     - develop
```

### Comparing `m9s_nereid_catalog-7.0.0/.woodpecker/mail_curl.sh` & `m9s_nereid_catalog-7.0.1/.woodpecker/mail_curl.sh`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog-7.0.0/.woodpecker/report.yml` & `m9s_nereid_catalog-7.0.1/.woodpecker/report.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog-7.0.0/.woodpecker/test.yml` & `m9s_nereid_catalog-7.0.1/.woodpecker/test.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog-7.0.0/.woodpecker.yml` & `m9s_nereid_catalog-7.0.1/.woodpecker.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog-7.0.0/CHANGELOG` & `m9s_nereid_catalog-7.0.1/CHANGELOG`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog-7.0.0/COPYRIGHT` & `m9s_nereid_catalog-7.0.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog-7.0.0/INSTALL` & `m9s_nereid_catalog-7.0.1/INSTALL`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog-7.0.0/LICENSE` & `m9s_nereid_catalog-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog-7.0.0/PKG-INFO` & `m9s_nereid_catalog-7.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s_nereid_catalog
-Version: 7.0.0
+Version: 7.0.1
 Summary: Tryton Nereid Catalog Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/nereid_catalog.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
 Project-URL: Bug Tracker, https://support.m9s.biz/
@@ -47,25 +47,17 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-Master
-
-[![Pipeline status](https://gitlab.com/m9s/nereid_catalog/badges/master/pipeline.svg)](https://gitlab.com/m9s/nereid_catalog/commits/master)
-
-Develop
-
-[![Pipeline status](https://gitlab.com/m9s/nereid_catalog/badges/develop/pipeline.svg)](https://gitlab.com/m9s/nereid_catalog/commits/develop)
-
-[![Coverage report](https://gitlab.com/m9s/nereid_catalog/badges/develop/coverage.svg)](http://m9s.gitlab.io/nereid_catalog)
-
+[![Tests Status](https://m9s.gitlab.io/nereid_catalog/junit/junit-badge.svg)](https://m9s.gitlab.io/nereid_catalog)
 
+[![Coverage Status](https://m9s.gitlab.io/nereid_catalog/coverage/coverage-badge.svg)](https://m9s.gitlab.io/nereid_catalog)
 
 This module runs with the Tryton application platform.
 
 Installing
 ----------
 
 See INSTALL
```

### Comparing `m9s_nereid_catalog-7.0.0/README.md` & `m9s_nereid_catalog-7.0.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,10 @@
-Master
-
-[![Pipeline status](https://gitlab.com/m9s/nereid_catalog/badges/master/pipeline.svg)](https://gitlab.com/m9s/nereid_catalog/commits/master)
-
-Develop
-
-[![Pipeline status](https://gitlab.com/m9s/nereid_catalog/badges/develop/pipeline.svg)](https://gitlab.com/m9s/nereid_catalog/commits/develop)
-
-[![Coverage report](https://gitlab.com/m9s/nereid_catalog/badges/develop/coverage.svg)](http://m9s.gitlab.io/nereid_catalog)
-
+[![Tests Status](https://m9s.gitlab.io/nereid_catalog/junit/junit-badge.svg)](https://m9s.gitlab.io/nereid_catalog)
 
+[![Coverage Status](https://m9s.gitlab.io/nereid_catalog/coverage/coverage-badge.svg)](https://m9s.gitlab.io/nereid_catalog)
 
 This module runs with the Tryton application platform.
 
 Installing
 ----------
 
 See INSTALL
```

### Comparing `m9s_nereid_catalog-7.0.0/locale/de.po` & `m9s_nereid_catalog-7.0.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog-7.0.0/m9s_nereid_catalog.egg-info/PKG-INFO` & `m9s_nereid_catalog-7.0.1/m9s_nereid_catalog.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s-nereid-catalog
-Version: 7.0.0
+Version: 7.0.1
 Summary: Tryton Nereid Catalog Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/nereid_catalog.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
 Project-URL: Bug Tracker, https://support.m9s.biz/
@@ -47,25 +47,17 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-Master
-
-[![Pipeline status](https://gitlab.com/m9s/nereid_catalog/badges/master/pipeline.svg)](https://gitlab.com/m9s/nereid_catalog/commits/master)
-
-Develop
-
-[![Pipeline status](https://gitlab.com/m9s/nereid_catalog/badges/develop/pipeline.svg)](https://gitlab.com/m9s/nereid_catalog/commits/develop)
-
-[![Coverage report](https://gitlab.com/m9s/nereid_catalog/badges/develop/coverage.svg)](http://m9s.gitlab.io/nereid_catalog)
-
+[![Tests Status](https://m9s.gitlab.io/nereid_catalog/junit/junit-badge.svg)](https://m9s.gitlab.io/nereid_catalog)
 
+[![Coverage Status](https://m9s.gitlab.io/nereid_catalog/coverage/coverage-badge.svg)](https://m9s.gitlab.io/nereid_catalog)
 
 This module runs with the Tryton application platform.
 
 Installing
 ----------
 
 See INSTALL
```

### Comparing `m9s_nereid_catalog-7.0.0/m9s_nereid_catalog.egg-info/SOURCES.txt` & `m9s_nereid_catalog-7.0.1/m9s_nereid_catalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog-7.0.0/product.py` & `m9s_nereid_catalog-7.0.1/product.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from flask_babel import format_currency
 from sql import Null
 from werkzeug.exceptions import NotFound
 
 from trytond.exceptions import UserError
 from trytond.i18n import gettext
-from trytond.model import ModelSQL, ModelView, fields, sequence_ordered
+from trytond.model import Index, ModelSQL, ModelView, fields, sequence_ordered
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Bool, Eval, Not
 
 from nereid import Markup, current_locale, jsonify, render_template, route
 from nereid.contrib.pagination import Pagination
 from nereid.contrib.sitemap import SitemapIndex, SitemapSection
 from nereid.globals import current_app, request, session
@@ -34,14 +34,23 @@
     product = fields.Many2One("product.product", "Product")
     template = fields.Many2One("product.template", "Template")
     url = fields.Function(fields.Char("URL"), "get_url")
 
     def get_url(self, name):
         return self.static_file.url
 
+    @classmethod
+    def __setup__(cls):
+        super().__setup__()
+        t = cls.__table__()
+        cls._sql_indexes.update({
+                Index(t, (t.product, Index.Equality())),
+                Index(t, (t.template, Index.Equality())),
+                })
+
 
 class ProductTemplate(metaclass=PoolMeta):
     __name__ = "product.template"
 
     products_displayed_on_eshop = fields.Function(
         fields.One2Many('product.product', None, 'Products (Disp. on eShop)'),
         'get_products_displayed_on_eshop')
@@ -108,14 +117,18 @@
     @classmethod
     def __setup__(cls):
         # Prevent NotImplementedError for setter
         if not hasattr(cls, '_no_template_field'):
             cls._no_template_field = set()
         cls._no_template_field.update(['products_displayed_on_eshop'])
         super().__setup__()
+        t = cls.__table__()
+        cls._sql_indexes.update({
+                Index(t, (t.uri, Index.Similarity())),
+                })
         cls.description.states['invisible'] = Bool(
             Eval('use_template_description'))
         cls.per_page = 12
 
     @staticmethod
     def default_displayed_on_eshop():
         return False
```

### Comparing `m9s_nereid_catalog-7.0.0/product.xml` & `m9s_nereid_catalog-7.0.1/product.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog-7.0.0/setup.py` & `m9s_nereid_catalog-7.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog-7.0.0/tests/test_module.py` & `m9s_nereid_catalog-7.0.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog-7.0.0/tox.ini` & `m9s_nereid_catalog-7.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog-7.0.0/view/product_form_nereid.xml` & `m9s_nereid_catalog-7.0.1/view/product_form_nereid.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog-7.0.0/view/template_form.xml` & `m9s_nereid_catalog-7.0.1/view/template_form.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog-7.0.0/website.py` & `m9s_nereid_catalog-7.0.1/website.py`

 * *Files identical despite different names*


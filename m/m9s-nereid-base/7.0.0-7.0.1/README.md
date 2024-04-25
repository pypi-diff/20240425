# Comparing `tmp/m9s_nereid_base-7.0.0.tar.gz` & `tmp/m9s_nereid_base-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m9s_nereid_base-7.0.0.tar", last modified: Fri Feb  2 15:03:58 2024, max compression
+gzip compressed data, was "m9s_nereid_base-7.0.1.tar", last modified: Thu Apr 25 14:14:33 2024, max compression
```

## Comparing `m9s_nereid_base-7.0.0.tar` & `m9s_nereid_base-7.0.1.tar`

### file list

```diff
@@ -1,97 +1,94 @@
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-02 15:03:58.032995 m9s_nereid_base-7.0.0/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       81 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.0/.coveragerc
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-15 11:09:33.000000 m9s_nereid_base-7.0.0/.drone.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.0/.flake8
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.0/.gitlab-ci-m9s.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1892 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.0/.gitlab-ci.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.0/.isort.cfg
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-02 15:03:58.028995 m9s_nereid_base-7.0.0/.woodpecker/
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.0/.woodpecker/mail_curl.sh
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.0/.woodpecker/report.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.0/.woodpecker/test.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      862 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.0/COPYRIGHT
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.0/INSTALL
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.0/LICENSE
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.0/MANIFEST.in
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3386 2024-02-02 15:03:58.032995 m9s_nereid_base-7.0.0/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1224 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.0/README.md
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.0/README.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1088 2024-01-25 12:48:43.000000 m9s_nereid_base-7.0.0/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       16 2020-03-16 09:24:45.000000 m9s_nereid_base-7.0.0/babel.cfg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4861 2024-01-24 19:18:39.000000 m9s_nereid_base-7.0.0/configuration.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1458 2024-01-25 11:36:59.000000 m9s_nereid_base-7.0.0/country.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      986 2024-01-24 19:10:30.000000 m9s_nereid_base-7.0.0/currency.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.0/dev_requirements.txt
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-02 15:03:58.028995 m9s_nereid_base-7.0.0/doc/
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-02 15:03:58.028995 m9s_nereid_base-7.0.0/doc/de/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       37 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.0/doc/de/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.0/doc/index.rst
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-02 15:03:58.016995 m9s_nereid_base-7.0.0/icons/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      296 2021-02-14 10:44:50.000000 m9s_nereid_base-7.0.0/icons/tryton-media.svg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      989 2021-02-14 10:44:50.000000 m9s_nereid_base-7.0.0/icons/tryton-web.svg
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-02 15:03:58.020995 m9s_nereid_base-7.0.0/locale/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    12688 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.0/locale/ca.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    14142 2022-04-12 07:18:45.000000 m9s_nereid_base-7.0.0/locale/de.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    13174 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.0/locale/es.po
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-02 15:03:58.028995 m9s_nereid_base-7.0.0/m9s_nereid_base.egg-info/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3386 2024-02-02 15:03:57.000000 m9s_nereid_base-7.0.0/m9s_nereid_base.egg-info/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2666 2024-02-02 15:03:57.000000 m9s_nereid_base-7.0.0/m9s_nereid_base.egg-info/SOURCES.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-02-02 15:03:57.000000 m9s_nereid_base-7.0.0/m9s_nereid_base.egg-info/dependency_links.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       60 2024-02-02 15:03:57.000000 m9s_nereid_base-7.0.0/m9s_nereid_base.egg-info/entry_points.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-01-26 11:11:06.000000 m9s_nereid_base-7.0.0/m9s_nereid_base.egg-info/not-zip-safe
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      105 2024-02-02 15:03:57.000000 m9s_nereid_base-7.0.0/m9s_nereid_base.egg-info/requires.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-02-02 15:03:57.000000 m9s_nereid_base-7.0.0/m9s_nereid_base.egg-info/top_level.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1311 2022-04-08 10:03:51.000000 m9s_nereid_base-7.0.0/message.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      646 2024-01-24 19:10:30.000000 m9s_nereid_base-7.0.0/model.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    12383 2024-01-26 20:14:57.000000 m9s_nereid_base-7.0.0/party.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3509 2022-03-29 15:04:46.000000 m9s_nereid_base-7.0.0/party.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.0/requirements.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-02-02 15:03:58.032995 m9s_nereid_base-7.0.0/setup.cfg
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4466 2024-01-26 19:58:30.000000 m9s_nereid_base-7.0.0/setup.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     8081 2024-02-02 14:44:21.000000 m9s_nereid_base-7.0.0/static_file.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3259 2022-03-25 09:26:04.000000 m9s_nereid_base-7.0.0/static_file.xml
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-02 15:03:58.028995 m9s_nereid_base-7.0.0/templates/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        0 2020-03-16 09:24:45.000000 m9s_nereid_base-7.0.0/templates/home.html
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        0 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.0/templates/new-password.jinja
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-02 15:03:58.028995 m9s_nereid_base-7.0.0/templates/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      129 2020-03-16 09:24:45.000000 m9s_nereid_base-7.0.0/templates/tests/exists-both.html
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       12 2020-03-16 09:24:45.000000 m9s_nereid_base-7.0.0/templates/tests/from-module.html
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-02 15:03:58.024995 m9s_nereid_base-7.0.0/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    47055 2024-02-01 09:41:43.000000 m9s_nereid_base-7.0.0/tests/1_auth.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      839 2024-02-02 08:14:23.000000 m9s_nereid_base-7.0.0/tests/1_test_module.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     8244 2024-02-02 08:24:04.000000 m9s_nereid_base-7.0.0/tests/2_test_module.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      115 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.0/tests/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    14689 2024-01-26 17:54:49.000000 m9s_nereid_base-7.0.0/tests/address.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    46806 2024-02-02 08:53:15.000000 m9s_nereid_base-7.0.0/tests/auth.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3603 2024-01-26 15:35:20.000000 m9s_nereid_base-7.0.0/tests/common.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4881 2024-01-26 15:58:13.000000 m9s_nereid_base-7.0.0/tests/country.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5334 2024-02-02 08:57:14.000000 m9s_nereid_base-7.0.0/tests/currency.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    10378 2024-02-02 11:36:11.000000 m9s_nereid_base-7.0.0/tests/i18n.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     9772 2024-02-02 11:12:55.000000 m9s_nereid_base-7.0.0/tests/routing.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4442 2024-02-02 09:58:30.000000 m9s_nereid_base-7.0.0/tests/static_file.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1011 2024-02-02 14:47:58.000000 m9s_nereid_base-7.0.0/tests/test_module.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    14582 2024-02-02 09:59:17.000000 m9s_nereid_base-7.0.0/tests/translation.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4390 2024-02-02 09:59:53.000000 m9s_nereid_base-7.0.0/tests/user.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1435 2024-02-02 09:59:53.000000 m9s_nereid_base-7.0.0/tests/website.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.0/tox.ini
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    28638 2024-02-02 10:32:01.000000 m9s_nereid_base-7.0.0/translation.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      442 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.0/translation.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      156 2024-01-24 12:58:52.000000 m9s_nereid_base-7.0.0/tryton.cfg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    36445 2024-02-02 14:48:48.000000 m9s_nereid_base-7.0.0/user.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-02 15:03:58.028995 m9s_nereid_base-7.0.0/view/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      366 2022-03-29 15:04:46.000000 m9s_nereid_base-7.0.0/view/contact_mechanism_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      290 2022-03-29 15:04:46.000000 m9s_nereid_base-7.0.0/view/contact_mechanism_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      290 2022-03-29 15:04:46.000000 m9s_nereid_base-7.0.0/view/contact_mechanism_tree_sequence.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      765 2021-05-14 10:34:06.000000 m9s_nereid_base-7.0.0/view/nereid_user_form2.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      265 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.0/view/nereid_user_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      338 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.0/view/party_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      631 2021-03-16 09:13:55.000000 m9s_nereid_base-7.0.0/view/static_file_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      210 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.0/view/static_file_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      459 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.0/view/static_folder_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      182 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.0/view/static_folder_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      367 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.0/view/translation_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1007 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.0/view/website_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      322 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.0/view/website_locale_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      239 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.0/view/website_locale_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      210 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.0/view/website_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    14790 2024-01-26 10:04:00.000000 m9s_nereid_base-7.0.0/website.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:14:33.892678 m9s_nereid_base-7.0.1/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       81 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/.coveragerc
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-15 11:09:33.000000 m9s_nereid_base-7.0.1/.drone.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/.flake8
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/.gitlab-ci-m9s.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2217 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/.gitlab-ci.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/.isort.cfg
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:14:33.888678 m9s_nereid_base-7.0.1/.woodpecker/
+-rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/.woodpecker/mail_curl.sh
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/.woodpecker/report.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/.woodpecker/test.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      862 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/COPYRIGHT
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/INSTALL
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/LICENSE
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/MANIFEST.in
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3204 2024-04-25 14:14:33.892678 m9s_nereid_base-7.0.1/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1042 2024-04-25 14:06:28.000000 m9s_nereid_base-7.0.1/README.md
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/README.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1088 2024-01-25 12:48:43.000000 m9s_nereid_base-7.0.1/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       16 2020-03-16 09:24:45.000000 m9s_nereid_base-7.0.1/babel.cfg
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4861 2024-01-24 19:18:39.000000 m9s_nereid_base-7.0.1/configuration.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1458 2024-01-25 11:36:59.000000 m9s_nereid_base-7.0.1/country.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      986 2024-01-24 19:10:30.000000 m9s_nereid_base-7.0.1/currency.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       86 2024-04-25 14:06:28.000000 m9s_nereid_base-7.0.1/dev_requirements.txt
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:14:33.892678 m9s_nereid_base-7.0.1/doc/
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:14:33.892678 m9s_nereid_base-7.0.1/doc/de/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       37 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/doc/de/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/doc/index.rst
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:14:33.888678 m9s_nereid_base-7.0.1/icons/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      296 2021-02-14 10:44:50.000000 m9s_nereid_base-7.0.1/icons/tryton-media.svg
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      989 2021-02-14 10:44:50.000000 m9s_nereid_base-7.0.1/icons/tryton-web.svg
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:14:33.888678 m9s_nereid_base-7.0.1/locale/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    12688 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/locale/ca.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    14142 2022-04-12 07:18:45.000000 m9s_nereid_base-7.0.1/locale/de.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    13174 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/locale/es.po
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:14:33.892678 m9s_nereid_base-7.0.1/m9s_nereid_base.egg-info/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3204 2024-04-25 14:14:33.000000 m9s_nereid_base-7.0.1/m9s_nereid_base.egg-info/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2598 2024-04-25 14:14:33.000000 m9s_nereid_base-7.0.1/m9s_nereid_base.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-04-25 14:14:33.000000 m9s_nereid_base-7.0.1/m9s_nereid_base.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       60 2024-04-25 14:14:33.000000 m9s_nereid_base-7.0.1/m9s_nereid_base.egg-info/entry_points.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-01-26 11:11:06.000000 m9s_nereid_base-7.0.1/m9s_nereid_base.egg-info/not-zip-safe
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      105 2024-04-25 14:14:33.000000 m9s_nereid_base-7.0.1/m9s_nereid_base.egg-info/requires.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-04-25 14:14:33.000000 m9s_nereid_base-7.0.1/m9s_nereid_base.egg-info/top_level.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1311 2022-04-08 10:03:51.000000 m9s_nereid_base-7.0.1/message.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      646 2024-01-24 19:10:30.000000 m9s_nereid_base-7.0.1/model.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    12383 2024-01-26 20:14:57.000000 m9s_nereid_base-7.0.1/party.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3509 2022-03-29 15:04:46.000000 m9s_nereid_base-7.0.1/party.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/requirements.txt
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-04-25 14:14:33.892678 m9s_nereid_base-7.0.1/setup.cfg
+-rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4466 2024-01-26 19:58:30.000000 m9s_nereid_base-7.0.1/setup.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     8146 2024-04-25 09:34:16.000000 m9s_nereid_base-7.0.1/static_file.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3259 2022-03-25 09:26:04.000000 m9s_nereid_base-7.0.1/static_file.xml
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:14:33.892678 m9s_nereid_base-7.0.1/templates/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        0 2020-03-16 09:24:45.000000 m9s_nereid_base-7.0.1/templates/home.html
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        0 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/templates/new-password.jinja
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:14:33.892678 m9s_nereid_base-7.0.1/templates/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      129 2020-03-16 09:24:45.000000 m9s_nereid_base-7.0.1/templates/tests/exists-both.html
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       12 2020-03-16 09:24:45.000000 m9s_nereid_base-7.0.1/templates/tests/from-module.html
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:14:33.888678 m9s_nereid_base-7.0.1/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      115 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/tests/__init__.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    14559 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/tests/address.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    46720 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/tests/auth.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3603 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/tests/common.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     4865 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/tests/country.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     5316 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/tests/currency.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    10378 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/tests/i18n.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     9772 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/tests/routing.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     4442 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/tests/static_file.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     1011 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/tests/test_module.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    14582 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/tests/translation.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     4390 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/tests/user.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     1435 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/tests/website.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/tox.ini
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    28638 2024-02-02 10:32:01.000000 m9s_nereid_base-7.0.1/translation.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      442 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/translation.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      156 2024-02-02 15:04:04.000000 m9s_nereid_base-7.0.1/tryton.cfg
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    35790 2024-04-25 09:34:16.000000 m9s_nereid_base-7.0.1/user.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:14:33.888678 m9s_nereid_base-7.0.1/view/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      366 2022-03-29 15:04:46.000000 m9s_nereid_base-7.0.1/view/contact_mechanism_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      290 2022-03-29 15:04:46.000000 m9s_nereid_base-7.0.1/view/contact_mechanism_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      290 2022-03-29 15:04:46.000000 m9s_nereid_base-7.0.1/view/contact_mechanism_tree_sequence.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      765 2021-05-14 10:34:06.000000 m9s_nereid_base-7.0.1/view/nereid_user_form2.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      265 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/view/nereid_user_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      338 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/view/party_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      631 2021-03-16 09:13:55.000000 m9s_nereid_base-7.0.1/view/static_file_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      210 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/view/static_file_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      459 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/view/static_folder_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      182 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/view/static_folder_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      367 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/view/translation_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1007 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/view/website_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      322 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/view/website_locale_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      239 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/view/website_locale_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      210 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/view/website_tree.xml
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    14802 2024-03-28 10:37:04.000000 m9s_nereid_base-7.0.1/website.py
```

### Comparing `m9s_nereid_base-7.0.0/.drone.yml` & `m9s_nereid_base-7.0.1/.drone.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/.gitlab-ci.yml` & `m9s_nereid_base-7.0.1/.gitlab-ci.yml`

 * *Files 16% similar despite different names*

```diff
@@ -30,54 +30,60 @@
       #only:
       #- releases/all
       #- releases/docker
       #- releases/python
       #- staging
       #- nightly
 
-test-postgres:
-  <<: *test_base
-  variables:
-    POSTGRESQL_URI: postgresql://postgres@postgresql:5432/
-    POSTGRES_HOST_AUTH_METHOD: trust
-  services:
-    - name: postgres
-      alias: postgresql
-      command: ["-c", "fsync=off", "-c", "synchronous_commit=off", "-c", "full_page_writes=off"]
-  script:
-    - tox -e py311-postgresql -vv -- -v
-  tags:
-    - postgres
+#test-postgres:
+#  <<: *test_base
+#  variables:
+#    POSTGRESQL_URI: postgresql://postgres@postgresql:5432/
+#    POSTGRES_HOST_AUTH_METHOD: trust
+#  services:
+#    - name: postgres
+#      alias: postgresql
+#      command: ["-c", "fsync=off", "-c", "synchronous_commit=off", "-c", "full_page_writes=off"]
+#  script:
+#    - tox -e py311-postgresql -vv -- -v
+#  tags:
+#    - postgres
 
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

### Comparing `m9s_nereid_base-7.0.0/.woodpecker/mail_curl.sh` & `m9s_nereid_base-7.0.1/.woodpecker/mail_curl.sh`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/.woodpecker/report.yml` & `m9s_nereid_base-7.0.1/.woodpecker/report.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/.woodpecker/test.yml` & `m9s_nereid_base-7.0.1/.woodpecker/test.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/COPYRIGHT` & `m9s_nereid_base-7.0.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/INSTALL` & `m9s_nereid_base-7.0.1/INSTALL`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/LICENSE` & `m9s_nereid_base-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/PKG-INFO` & `m9s_nereid_base-7.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s_nereid_base
-Version: 7.0.0
+Version: 7.0.1
 Summary: Tryton Nereid Base Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/nereid_base.git
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
-[![Pipeline status](https://gitlab.com/m9s/nereid_base/badges/master/pipeline.svg)](https://gitlab.com/m9s/nereid_base/commits/master)
-
-Develop
-
-[![Pipeline status](https://gitlab.com/m9s/nereid_base/badges/develop/pipeline.svg)](https://gitlab.com/m9s/nereid_base/commits/develop)
-
-[![Coverage report](https://gitlab.com/m9s/nereid_base/badges/develop/coverage.svg)](http://m9s.gitlab.io/nereid_base)
-
+[![Tests Status](https://m9s.gitlab.io/nereid_base/junit/junit-badge.svg)](https://m9s.gitlab.io/nereid_base)
 
+[![Coverage Status](https://m9s.gitlab.io/nereid_base/coverage/coverage-badge.svg)](https://m9s.gitlab.io/nereid_base)
 
 This module runs with the Tryton application platform.
 
 Installing
 ----------
 
 See INSTALL
```

### Comparing `m9s_nereid_base-7.0.0/README.md` & `m9s_nereid_base-7.0.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,10 @@
-Master
-
-[![Pipeline status](https://gitlab.com/m9s/nereid_base/badges/master/pipeline.svg)](https://gitlab.com/m9s/nereid_base/commits/master)
-
-Develop
-
-[![Pipeline status](https://gitlab.com/m9s/nereid_base/badges/develop/pipeline.svg)](https://gitlab.com/m9s/nereid_base/commits/develop)
-
-[![Coverage report](https://gitlab.com/m9s/nereid_base/badges/develop/coverage.svg)](http://m9s.gitlab.io/nereid_base)
-
+[![Tests Status](https://m9s.gitlab.io/nereid_base/junit/junit-badge.svg)](https://m9s.gitlab.io/nereid_base)
 
+[![Coverage Status](https://m9s.gitlab.io/nereid_base/coverage/coverage-badge.svg)](https://m9s.gitlab.io/nereid_base)
 
 This module runs with the Tryton application platform.
 
 Installing
 ----------
 
 See INSTALL
```

### Comparing `m9s_nereid_base-7.0.0/__init__.py` & `m9s_nereid_base-7.0.1/__init__.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/configuration.xml` & `m9s_nereid_base-7.0.1/configuration.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/country.py` & `m9s_nereid_base-7.0.1/country.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/currency.py` & `m9s_nereid_base-7.0.1/currency.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/icons/tryton-web.svg` & `m9s_nereid_base-7.0.1/icons/tryton-web.svg`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/locale/ca.po` & `m9s_nereid_base-7.0.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/locale/de.po` & `m9s_nereid_base-7.0.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/locale/es.po` & `m9s_nereid_base-7.0.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/m9s_nereid_base.egg-info/PKG-INFO` & `m9s_nereid_base-7.0.1/m9s_nereid_base.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s-nereid-base
-Version: 7.0.0
+Version: 7.0.1
 Summary: Tryton Nereid Base Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/nereid_base.git
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
-[![Pipeline status](https://gitlab.com/m9s/nereid_base/badges/master/pipeline.svg)](https://gitlab.com/m9s/nereid_base/commits/master)
-
-Develop
-
-[![Pipeline status](https://gitlab.com/m9s/nereid_base/badges/develop/pipeline.svg)](https://gitlab.com/m9s/nereid_base/commits/develop)
-
-[![Coverage report](https://gitlab.com/m9s/nereid_base/badges/develop/coverage.svg)](http://m9s.gitlab.io/nereid_base)
-
+[![Tests Status](https://m9s.gitlab.io/nereid_base/junit/junit-badge.svg)](https://m9s.gitlab.io/nereid_base)
 
+[![Coverage Status](https://m9s.gitlab.io/nereid_base/coverage/coverage-badge.svg)](https://m9s.gitlab.io/nereid_base)
 
 This module runs with the Tryton application platform.
 
 Installing
 ----------
 
 See INSTALL
```

### Comparing `m9s_nereid_base-7.0.0/m9s_nereid_base.egg-info/SOURCES.txt` & `m9s_nereid_base-7.0.1/m9s_nereid_base.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -46,17 +46,14 @@
 ./user.py
 ./website.py
 ./icons/tryton-media.svg
 ./icons/tryton-web.svg
 ./locale/ca.po
 ./locale/de.po
 ./locale/es.po
-./tests/1_auth.py
-./tests/1_test_module.py
-./tests/2_test_module.py
 ./tests/__init__.py
 ./tests/address.py
 ./tests/auth.py
 ./tests/common.py
 ./tests/country.py
 ./tests/currency.py
 ./tests/i18n.py
```

### Comparing `m9s_nereid_base-7.0.0/message.xml` & `m9s_nereid_base-7.0.1/message.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/model.py` & `m9s_nereid_base-7.0.1/model.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/party.py` & `m9s_nereid_base-7.0.1/party.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/party.xml` & `m9s_nereid_base-7.0.1/party.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/setup.py` & `m9s_nereid_base-7.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/static_file.py` & `m9s_nereid_base-7.0.1/static_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,53 +4,54 @@
 import os
 
 from werkzeug.exceptions import abort
 
 from trytond.config import config
 from trytond.exceptions import UserError
 from trytond.i18n import gettext
-from trytond.model import ModelSQL, ModelView, Unique, fields, sequence_ordered
+from trytond.model import (
+    Index, ModelSQL, ModelView, Unique, fields, sequence_ordered)
 from trytond.pyson import Bool, Eval
 from trytond.transaction import Transaction
 
 from nereid import route
 from nereid.ctx import has_request_context
-from nereid.globals import request_ctx
 from nereid.helpers import send_file, url_for
 
 READONLY_IF_FILES = {
     'readonly': Bool(Eval('files'))
 }
 
 
 class NereidStaticFolder(ModelSQL, ModelView):
     "Static Folder"
     __name__ = "nereid.static.folder"
 
     name = fields.Char(
         'Name', required=True, states=READONLY_IF_FILES,
-        depends=['files']
     )
     description = fields.Char(
         'Description', states=READONLY_IF_FILES,
-        depends=['files']
     )
     files = fields.One2Many('nereid.static.file', 'folder', 'Files')
     type = fields.Selection([
         ('local', 'Local File'),
-    ], 'File Type', states=READONLY_IF_FILES, depends=['files'])
+    ], 'File Type', states=READONLY_IF_FILES)
 
     @classmethod
     def __setup__(cls):
-        super(NereidStaticFolder, cls).__setup__()
-        table = cls.__table__()
+        super().__setup__()
+        t = cls.__table__()
+        cls._sql_indexes.update({
+                Index(t, (t.description, Index.Similarity())),
+                })
         cls._sql_constraints += [
-            ('unique_folder', Unique(table, table.name),
+            ('unique_folder', Unique(t, t.name),
              'Folder name needs to be unique')
-        ]
+            ]
 
     @classmethod
     def validate(cls, folders):
         """
         Validates the records.
 
         :param folders: active record list of folders
@@ -99,20 +100,23 @@
     url = fields.Function(fields.Char('URL'), 'get_url')
 
     # File mimetype
     mimetype = fields.Function(fields.Char('Mimetype'), getter='get_mimetype')
 
     @classmethod
     def __setup__(cls):
-        super(NereidStaticFile, cls).__setup__()
-        table = cls.__table__()
+        super().__setup__()
+        t = cls.__table__()
+        cls._sql_indexes.update({
+                Index(t, (t.folder, Index.Equality())),
+                })
         cls._sql_constraints += [
-            ('name_folder_uniq', Unique(table, table.name, table.folder),
+            ('name_folder_uniq', Unique(t, t.name, t.folder),
                 'The Name of the Static File must be unique in a folder.!'),
-        ]
+            ]
 
     def get_mimetype(self, name):
         """
         This method detects and returns the mimetype for the static file.
 
         The python mimetypes module returns a tuple of the form -:
```

### Comparing `m9s_nereid_base-7.0.0/static_file.xml` & `m9s_nereid_base-7.0.1/static_file.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/tests/1_auth.py` & `m9s_nereid_base-7.0.1/tests/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # The COPYRIGHT file at the top level of this repository contains the full
 # copyright notices and license terms.
 import base64
 import json
-import unittest
 import urllib.error
 import urllib.parse
 import urllib.request
 
 from unittest.mock import ANY, patch
 
 import trytond.tests.test_tryton
 
 from trytond.config import config
 from trytond.model.modelsql import SQLConstraintError
 from trytond.modules.nereid_base import user as user_module
-from trytond.pool import Pool
-from trytond.sendmail import get_smtp_server
+#from trytond.sendmail import get_smtp_server
 from trytond.tests.test_tryton import with_transaction
 from trytond.transaction import Transaction
 
-from nereid.testing import POOL as pool
 from nereid.testing import NereidTestCase
 
 from common import setup_objects
 
 FROM = 'no-reply@localhost'
-FROM = 'mathiasb'
+
+# issue5137: run for now with default From, config settings have no effect
+from getpass import getuser
+FROM = getuser()
 
 
 class AuthTestCase(NereidTestCase):
     """
     Test Authentication Layer
     """
     def setUp(self):
@@ -94,31 +94,30 @@
     def get_template_source(self, name):
         """
         Return templates
         """
 
         return self.templates.get(name)
 
-    @patch('trytond.sendmail.get_smtp_server')
+    # issue5137: it seems no more necessary to patch get_smtp_server
+    #@patch('trytond.sendmail.get_smtp_server')
+    #@with_transaction()
+    #def test_0010_register(self, get_smtp_server):
     @with_transaction()
-    def test_0010_register(self, get_smtp_server):
+    def test_0010_register(self):
         """
         Registration must create a new party
         """
         self.setup_defaults()
         app = self.get_app()
         with patch.object(
                 user_module, 'sendmail_transactional') as sendmail, \
                 patch.object(user_module, 'SMTPDataManager') as dm, \
                 app.test_client() as c:
-            config.set('email', 'from', FROM)
-
-            print('****************', config.get('email', 'from'))
-            #print('****************', dir(sendmail))
-            #print('****************', dir(dm))
+            #print('****************', config.get('email', 'from'))
             response = c.get('/registration')
             self.assertEqual(response.status_code, 200)   # GET Request
 
             email_user = 'regd_user@m9s.biz'
             data = {
                 'name': 'Registered User',
                 'email': email_user,
@@ -132,16 +131,16 @@
             sendmail.assert_not_called()
 
             data['confirm'] = 'password'
             response = c.post('/registration', data=data)
             self.assertEqual(response.status_code, 302)
 
             # Test if an email was sent
-            print(sendmail.call_args)
-            print(dm.call_args)
+            #print(sendmail.call_args)
+            #print(dm.call_args)
             sendmail.assert_called_once_with(
                 FROM, email_user, ANY,
                 datamanager=ANY)
             _, _, msg = sendmail.call_args[0]
             self.assertEqual(msg['From'], FROM)
             self.assertEqual(msg['Subject'], 'Account Activation')
             self.assertEqual(msg['To'], email_user)
@@ -363,351 +362,351 @@
             # verify the email
             response = c.get(registered_user.get_email_verification_link())
             self.assertEqual(response.status_code, 302)
 
             # Email should now be verified
             self.assertTrue(registered_user.email_verified)
 
-    #@with_transaction()
-    #def test_0020_activation(self):
-    #    """
-    #    Activation must happen before login is possible
-    #    """
-    #    self.setup_defaults()
-    #    app = self.get_app()
-
-    #    with patch.object(
-    #            user_module, 'sendmail_transactional') as sendmail, \
-        #            patch.object(user_module, 'SMTPDataManager') as dm, \
-        #            app.test_client() as c:
-    #        data = {
-    #            'name': 'Registered User',
-    #            'email': 'regd_user@m9s.biz',
-    #            'password': 'password',
-    #            'confirm': 'password',
-    #            }
-    #        response = c.post('/registration', data=data)
-    #        self.assertEqual(response.status_code, 302)
-
-    #        with Transaction().set_context(active_test=False):
-    #            registered_user, = self.nereid_user_obj.search(
-    #                [('email', '=', data['email'].lower())])
-    #        self.assertFalse(registered_user.active)
-
-    #        # Login should fail since there is activation code
-    #        response = c.post('/login',
-    #            data={
-    #                'email': data['email'],
-    #                'password': data['password'],
-    #                })
-    #        self.assertEqual(response.status_code, 200)
-    #        self.assertTrue(
-    #            "Registration Complete. Check your email for activation"
-    #            in response.data.decode('utf-8'))
-    #        self.assertTrue(
-    #            "Invalid login credentials"
-    #            in response.data.decode('utf-8'))
-
-    #        # Activate the account
-    #        response = c.get(registered_user.get_activation_link())
-    #        self.assertEqual(response.status_code, 302)
-    #        registered_user = self.nereid_user_obj(registered_user.id)
-
-    #        # The account must be active
-    #        self.assertTrue(registered_user.active)
-    #        # Email should be verified
-    #        self.assertTrue(registered_user.email_verified)
-
-    #        # Login should work
-    #        response = c.post('/login',
-    #            data={
-    #                'email': data['email'],
-    #                'password': data['password'],
-    #                })
-    #        registered_user = self.nereid_user_obj(registered_user.id)
-    #        self.assertEqual(response.status_code, 302)
+    @with_transaction()
+    def test_0020_activation(self):
+        """
+        Activation must happen before login is possible
+        """
+        self.setup_defaults()
+        app = self.get_app()
 
-    #@with_transaction()
-    #def test_0030_change_password(self):
-    #    """
-    #    Check password changing functionality
-    #    """
-    #    self.setup_defaults()
-    #    app = self.get_app()
-
-    #    party, = self.party_obj.create([{'name': 'Registered user'}])
-    #    data = {
-    #        'party': party,
-    #        'name': 'Registered User',
-    #        'email': 'info@m9s.biz',
-    #        'password': 'password',
-    #        'company': self.company,
-    #        }
-    #    self.nereid_user_obj.create([data.copy()])
-
-    #    with app.test_client() as c:
-    #        # try the page without login
-    #        response = c.get('/change-password')
-    #        self.assertEqual(response.status_code, 302)
-
-    #        # try the post without login
-    #        response = c.post('/change-password',
-    #            data={
-    #                'password': data['password'],
-    #                'confirm': data['password'],
-    #                })
-    #        self.assertEqual(response.status_code, 302)
-
-    #        # Login now
-    #        response = c.post(
-    #            '/login',
-    #            data={
-    #                'email': data['email'],
-    #                'password': data['password']
-    #                })
-    #        self.assertEqual(response.status_code, 302)
-
-    #        # send wrong password confirm
-    #        response = c.post('/change-password',
-    #            data={
-    #                'password': 'new-password',
-    #                'confirm': 'password',
-    #                })
-    #        self.assertEqual(response.status_code, 200)
-    #        self.assertTrue("Passwords must match"
-    #            in response.data.decode('utf-8'))
-
-    #        # send wrong password confirm as XHR
-    #        response = c.post('/change-password',
-    #            data={
-    #                'password': 'new-password',
-    #                'confirm': 'password',
-    #                }, headers={'X-Requested-With': 'XMLHTTPRequest'})
-    #        res = json.loads(response.data)
-    #        self.assertEqual(response.status_code, 400)
-    #        self.assertEqual(res['errors']['password'][0],
-    #            "Passwords must match")
-    #        self.assertEqual(res['errors']['old_password'][0],
-    #            "This field is required.")
-
-    #        # send correct password confirm but not old password
-    #        response = c.post('/change-password',
-    #            data={
-    #                'password': 'new-password',
-    #                'confirm': 'new-password'
-    #                })
-    #        self.assertEqual(response.status_code, 200)
-
-    #        # send correct password confirm but incorrect old password
-    #        response = c.post('/change-password',
-    #            data={
-    #                'old_password': 'passw',
-    #                'password': 'new-password',
-    #                'confirm': 'new-password'
-    #                })
-    #        self.assertEqual(response.status_code, 200)
-    #        self.assertTrue("The current password you entered is invalid"
-    #            in response.data.decode('utf-8'))
-
-    #        # send correct password confirm but incorrect old password as XHR
-    #        response = c.post('/change-password',
-    #            data={
-    #                'old_password': 'passw',
-    #                'password': 'new-password',
-    #                'confirm': 'new-password'
-    #                }, headers={'X-Requested-With': 'XMLHTTPRequest'})
-    #        res = json.loads(response.data)
-    #        self.assertEqual(response.status_code, 400)
-    #        self.assertEqual(res['message'],
-    #            "The current password you entered is invalid")
-
-    #        response = c.post('/change-password',
-    #            data={
-    #                'old_password': data['password'],
-    #                'password': 'new-password',
-    #                'confirm': 'new-password'
-    #                })
-    #        self.assertEqual(response.status_code, 302)
-    #        response = c.get('/')
-
-    #        # Login now using new password
-    #        response = c.post('/login',
-    #            data={
-    #                'email': data['email'],
-    #                'password': 'new-password'
-    #                })
-    #        self.assertEqual(response.status_code, 302)
-
-    #        # Change password with XHR
-    #        response = c.post('/change-password',
-    #            data={
-    #                'old_password': 'new-password',
-    #                'password': 'password',
-    #                'confirm': 'password'
-    #                }, headers={'X-Requested-With': 'XMLHTTPRequest'})
-    #        res = json.loads(response.data)
-    #        self.assertEqual(response.status_code, 200)
-    #        self.assertEqual(res['message'],
-    #            'Your password has been successfully changed! '
-    #                'Please login again',)
+        with patch.object(
+                user_module, 'sendmail_transactional') as sendmail, \
+                patch.object(user_module, 'SMTPDataManager') as dm, \
+                app.test_client() as c:
+            data = {
+                'name': 'Registered User',
+                'email': 'regd_user@m9s.biz',
+                'password': 'password',
+                'confirm': 'password',
+                }
+            response = c.post('/registration', data=data)
+            self.assertEqual(response.status_code, 302)
 
-    #@with_transaction()
-    #def test_0040_reset_account(self):
-    #    """
-    #    Allow resetting password of the user
-    #    """
-    #    self.setup_defaults()
-    #    app = self.get_app()
-
-    #    party, = self.party_obj.create([{'name': 'Registered user'}])
-    #    data = {
-    #        'party': party,
-    #        'name': 'Registered User',
-    #        'email': 'info@m9s.biz',
-    #        'password': 'password',
-    #        'company': self.company,
-    #        }
-    #    regd_user, = self.nereid_user_obj.create([data.copy()])
-
-    #    with patch.object(
-    #            user_module, 'sendmail_transactional') as sendmail, \
-        #            patch.object(user_module, 'SMTPDataManager') as dm, \
-        #            app.test_client() as c:
-
-    #        # Try reset without login and page should render
-    #        response = c.get('/reset-account')
-    #        self.assertEqual(response.status_code, 200)
-
-    #        # Try resetting password through email
-    #        response = c.post('/reset-account',
-    #            data={
-    #                'email': data['email'],
-    #                })
-    #        self.assertEqual(response.status_code, 302)
-
-    #        response = c.post('/reset-account',
-    #            data={
-    #                'email': data['email'],
-    #                },
-    #            headers={'X-Requested-With': 'XMLHTTPRequest'})
-    #        self.assertEqual(response.status_code, 200)
-
-    #        rv = c.post('/reset-account',
-    #            data={
-    #                'email': 'made_up_email@test.com',
-    #                }, headers={'X-Requested-With': 'XMLHTTPRequest'})
-    #        self.assertEqual(rv.status_code, 400)
-    #        self.assertEqual(json.loads(rv.data),
-    #            {'message': 'Invalid email address'})
-
-    #        # A successful login after requesting activation code should
-    #        # not do anything but just allow login
-    #        response = c.post('/login',
-    #            data={
-    #                'email': data['email'],
-    #                'password': data['password'],
-    #                })
-    #        self.assertEqual(response.status_code, 302)
-
-    #    with patch.object(
-    #            user_module, 'sendmail_transactional') as sendmail, \
-        #            patch.object(user_module, 'SMTPDataManager') as dm, \
-        #            app.test_client() as c:
-    #        # Try to reset again - with good intentions
-    #        response = c.post('/reset-account',
-    #            data={
-    #                'email': data['email'],
-    #                })
-    #        self.assertEqual(response.status_code, 302)
-
-    #        # Try to reset password with invalid code
-    #        invalid_code = 'thisistheinvalidcode'
-    #        response = c.post(
-    #            '/new-password/%s/%s' % (regd_user.id, invalid_code),
-    #            data={
-    #                'password': 'reset-password',
-    #                'confirm': 'reset-password'
-    #                })
-    #        self.assertEqual(response.status_code, 302)
-
-    #        response = c.post('/login',
-    #            data={
-    #                'email': data['email'],
-    #                'password': 'reset-password'
-    #                })
-    #        self.assertEqual(response.status_code, 200)  # Login rejected
-
-    #        # Reset password with valid code, but too simple password
-    #        response = c.post(regd_user.get_reset_password_link(),
-    #            data={
-    #                'password': 'aaaaaaaaa',
-    #                'confirm': 'aaaaaaaaa'
-    #                })
-    #        self.assertEqual(response.status_code, 200) # Login rejected
-
-    #        # Reset password with valid code, but complex password
-    #        response = c.post(regd_user.get_reset_password_link(),
-    #            data={
-    #                'password': 'rEset-paSswoRd',
-    #                'confirm': 'rEset-paSswoRd'
-    #                })
-    #        self.assertEqual(response.status_code, 302)
-
-    #        regd_user = self.nereid_user_obj(regd_user.id)
-
-    #        response = c.post('/login',
-    #            data={
-    #                'email': data['email'],
-    #                'password': 'wrong-password'
-    #                })
-    #        self.assertEqual(response.status_code, 200)     # Login rejected
-
-    #        response = c.post('/login',
-    #            data={
-    #                'email': data['email'],
-    #                'password': 'rEset-paSswoRd'
-    #                })
-    #        self.assertEqual(response.status_code, 302)     # Login approved
-
-    #    with app.test_client() as c:
-    #        # Try to reset again - with bad intentions
-
-    #        # Bad request because there is no email
-    #        response = c.post(
-    #            '/reset-account', data={},
-    #            headers={'X-Requested-With': 'XMLHTTPRequest'})
-    #        self.assertEqual(response.status_code, 400)
-
-    #        response = c.post('/reset-account', data={})
-    #        self.assertEqual(response.status_code, 200)
-    #        self.assertTrue(
-    #            'Invalid email address' in response.data.decode('utf-8'))
-
-    #        # Bad request because there is empty email
-    #        response = c.post('/reset-account', data={'email': ''})
-    #        self.assertEqual(response.status_code, 200)
-    #        self.assertTrue(
-    #            'Invalid email address' in response.data.decode('utf-8'))
-
-    #    data = {
-    #        'party': party,
-    #        'name': 'User without email',
-    #        'email': '',
-    #        'password': 'password',
-    #        'company': self.company,
-    #        }
-    #    email_less_user, = self.nereid_user_obj.create([data.copy()])
-    #    with app.test_client() as c:
-    #        # Bad request because there is empty email
-    #        # this is a special case where there is an user
-    #        # with empty email
-    #        response = c.post('/reset-account', data={'email': ''})
-    #        self.assertEqual(response.status_code, 200)
-    #        self.assertTrue(
-    #            'Invalid email address' in response.data.decode('utf-8'))
+            with Transaction().set_context(active_test=False):
+                registered_user, = self.nereid_user_obj.search(
+                    [('email', '=', data['email'].lower())])
+            self.assertFalse(registered_user.active)
+
+            # Login should fail since there is activation code
+            response = c.post('/login',
+                data={
+                    'email': data['email'],
+                    'password': data['password'],
+                    })
+            self.assertEqual(response.status_code, 200)
+            self.assertTrue(
+                "Registration Complete. Check your email for activation"
+                in response.data.decode('utf-8'))
+            self.assertTrue(
+                "Invalid login credentials"
+                in response.data.decode('utf-8'))
+
+            # Activate the account
+            response = c.get(registered_user.get_activation_link())
+            self.assertEqual(response.status_code, 302)
+            registered_user = self.nereid_user_obj(registered_user.id)
+
+            # The account must be active
+            self.assertTrue(registered_user.active)
+            # Email should be verified
+            self.assertTrue(registered_user.email_verified)
+
+            # Login should work
+            response = c.post('/login',
+                data={
+                    'email': data['email'],
+                    'password': data['password'],
+                    })
+            registered_user = self.nereid_user_obj(registered_user.id)
+            self.assertEqual(response.status_code, 302)
+
+    @with_transaction()
+    def test_0030_change_password(self):
+        """
+        Check password changing functionality
+        """
+        self.setup_defaults()
+        app = self.get_app()
+
+        party, = self.party_obj.create([{'name': 'Registered user'}])
+        data = {
+            'party': party,
+            'name': 'Registered User',
+            'email': 'info@m9s.biz',
+            'password': 'password',
+            'company': self.company,
+            }
+        self.nereid_user_obj.create([data.copy()])
+
+        with app.test_client() as c:
+            # try the page without login
+            response = c.get('/change-password')
+            self.assertEqual(response.status_code, 302)
+
+            # try the post without login
+            response = c.post('/change-password',
+                data={
+                    'password': data['password'],
+                    'confirm': data['password'],
+                    })
+            self.assertEqual(response.status_code, 302)
+
+            # Login now
+            response = c.post(
+                '/login',
+                data={
+                    'email': data['email'],
+                    'password': data['password']
+                    })
+            self.assertEqual(response.status_code, 302)
+
+            # send wrong password confirm
+            response = c.post('/change-password',
+                data={
+                    'password': 'new-password',
+                    'confirm': 'password',
+                    })
+            self.assertEqual(response.status_code, 200)
+            self.assertTrue("Passwords must match"
+                in response.data.decode('utf-8'))
+
+            # send wrong password confirm as XHR
+            response = c.post('/change-password',
+                data={
+                    'password': 'new-password',
+                    'confirm': 'password',
+                    }, headers={'X-Requested-With': 'XMLHTTPRequest'})
+            res = json.loads(response.data)
+            self.assertEqual(response.status_code, 400)
+            self.assertEqual(res['errors']['password'][0],
+                "Passwords must match")
+            self.assertEqual(res['errors']['old_password'][0],
+                "This field is required.")
+
+            # send correct password confirm but not old password
+            response = c.post('/change-password',
+                data={
+                    'password': 'new-password',
+                    'confirm': 'new-password'
+                    })
+            self.assertEqual(response.status_code, 200)
+
+            # send correct password confirm but incorrect old password
+            response = c.post('/change-password',
+                data={
+                    'old_password': 'passw',
+                    'password': 'new-password',
+                    'confirm': 'new-password'
+                    })
+            self.assertEqual(response.status_code, 200)
+            self.assertTrue("The current password you entered is invalid"
+                in response.data.decode('utf-8'))
+
+            # send correct password confirm but incorrect old password as XHR
+            response = c.post('/change-password',
+                data={
+                    'old_password': 'passw',
+                    'password': 'new-password',
+                    'confirm': 'new-password'
+                    }, headers={'X-Requested-With': 'XMLHTTPRequest'})
+            res = json.loads(response.data)
+            self.assertEqual(response.status_code, 400)
+            self.assertEqual(res['message'],
+                "The current password you entered is invalid")
+
+            response = c.post('/change-password',
+                data={
+                    'old_password': data['password'],
+                    'password': 'new-password',
+                    'confirm': 'new-password'
+                    })
+            self.assertEqual(response.status_code, 302)
+            response = c.get('/')
+
+            # Login now using new password
+            response = c.post('/login',
+                data={
+                    'email': data['email'],
+                    'password': 'new-password'
+                    })
+            self.assertEqual(response.status_code, 302)
+
+            # Change password with XHR
+            response = c.post('/change-password',
+                data={
+                    'old_password': 'new-password',
+                    'password': 'password',
+                    'confirm': 'password'
+                    }, headers={'X-Requested-With': 'XMLHTTPRequest'})
+            res = json.loads(response.data)
+            self.assertEqual(response.status_code, 200)
+            self.assertEqual(res['message'],
+                'Your password has been successfully changed! '
+                    'Please login again',)
+
+    @with_transaction()
+    def test_0040_reset_account(self):
+        """
+        Allow resetting password of the user
+        """
+        self.setup_defaults()
+        app = self.get_app()
+
+        party, = self.party_obj.create([{'name': 'Registered user'}])
+        data = {
+            'party': party,
+            'name': 'Registered User',
+            'email': 'info@m9s.biz',
+            'password': 'password',
+            'company': self.company,
+            }
+        regd_user, = self.nereid_user_obj.create([data.copy()])
+
+        with patch.object(
+                user_module, 'sendmail_transactional') as sendmail, \
+                patch.object(user_module, 'SMTPDataManager') as dm, \
+                app.test_client() as c:
+
+            # Try reset without login and page should render
+            response = c.get('/reset-account')
+            self.assertEqual(response.status_code, 200)
+
+            # Try resetting password through email
+            response = c.post('/reset-account',
+                data={
+                    'email': data['email'],
+                    })
+            self.assertEqual(response.status_code, 302)
+
+            response = c.post('/reset-account',
+                data={
+                    'email': data['email'],
+                    },
+                headers={'X-Requested-With': 'XMLHTTPRequest'})
+            self.assertEqual(response.status_code, 200)
+
+            rv = c.post('/reset-account',
+                data={
+                    'email': 'made_up_email@test.com',
+                    }, headers={'X-Requested-With': 'XMLHTTPRequest'})
+            self.assertEqual(rv.status_code, 400)
+            self.assertEqual(json.loads(rv.data),
+                {'message': 'Invalid email address'})
+
+            # A successful login after requesting activation code should
+            # not do anything but just allow login
+            response = c.post('/login',
+                data={
+                    'email': data['email'],
+                    'password': data['password'],
+                    })
+            self.assertEqual(response.status_code, 302)
+
+        with patch.object(
+                user_module, 'sendmail_transactional') as sendmail, \
+                patch.object(user_module, 'SMTPDataManager') as dm, \
+                app.test_client() as c:
+            # Try to reset again - with good intentions
+            response = c.post('/reset-account',
+                data={
+                    'email': data['email'],
+                    })
+            self.assertEqual(response.status_code, 302)
+
+            # Try to reset password with invalid code
+            invalid_code = 'thisistheinvalidcode'
+            response = c.post(
+                '/new-password/%s/%s' % (regd_user.id, invalid_code),
+                data={
+                    'password': 'reset-password',
+                    'confirm': 'reset-password'
+                    })
+            self.assertEqual(response.status_code, 302)
+
+            response = c.post('/login',
+                data={
+                    'email': data['email'],
+                    'password': 'reset-password'
+                    })
+            self.assertEqual(response.status_code, 200)  # Login rejected
+
+            # Reset password with valid code, but too simple password
+            response = c.post(regd_user.get_reset_password_link(),
+                data={
+                    'password': 'a',
+                    'confirm': 'a'
+                    })
+            self.assertEqual(response.status_code, 200) # Login rejected
+
+            # Reset password with valid code, but complex password
+            response = c.post(regd_user.get_reset_password_link(),
+                data={
+                    'password': 'rEset-paSswoRd',
+                    'confirm': 'rEset-paSswoRd'
+                    })
+            self.assertEqual(response.status_code, 302)
+
+            regd_user = self.nereid_user_obj(regd_user.id)
+
+            response = c.post('/login',
+                data={
+                    'email': data['email'],
+                    'password': 'wrong-password'
+                    })
+            self.assertEqual(response.status_code, 200)     # Login rejected
+
+            response = c.post('/login',
+                data={
+                    'email': data['email'],
+                    'password': 'rEset-paSswoRd'
+                    })
+            self.assertEqual(response.status_code, 302)     # Login approved
+
+        with app.test_client() as c:
+            # Try to reset again - with bad intentions
+
+            # Bad request because there is no email
+            response = c.post(
+                '/reset-account', data={},
+                headers={'X-Requested-With': 'XMLHTTPRequest'})
+            self.assertEqual(response.status_code, 400)
+
+            response = c.post('/reset-account', data={})
+            self.assertEqual(response.status_code, 200)
+            self.assertTrue(
+                'Invalid email address' in response.data.decode('utf-8'))
+
+            # Bad request because there is empty email
+            response = c.post('/reset-account', data={'email': ''})
+            self.assertEqual(response.status_code, 200)
+            self.assertTrue(
+                'Invalid email address' in response.data.decode('utf-8'))
+
+        data = {
+            'party': party,
+            'name': 'User without email',
+            'email': '',
+            'password': 'password',
+            'company': self.company,
+            }
+        email_less_user, = self.nereid_user_obj.create([data.copy()])
+        with app.test_client() as c:
+            # Bad request because there is empty email
+            # this is a special case where there is an user
+            # with empty email
+            response = c.post('/reset-account', data={'email': ''})
+            self.assertEqual(response.status_code, 200)
+            self.assertTrue(
+                'Invalid email address' in response.data.decode('utf-8'))
 
     @with_transaction()
     def test_0050_logout(self):
         """
         Check for logout
         """
         self.setup_defaults()
```

### Comparing `m9s_nereid_base-7.0.0/tests/1_test_module.py` & `m9s_nereid_base-7.0.1/tests/test_module.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # The COPYRIGHT file at the top level of this repository contains
 # the full copyright notices and license terms.
 
-#from address import AddressTestCase
+from address import AddressTestCase
 from auth import AuthTestCase
+from country import CountryTestCase
+from currency import CurrencyTestCase
+from i18n import I18NTestCase
+from routing import RoutingTestCase
+from static_file import StaticFileTestCase
+from translation import TranslationTestCase
+from user import UserTestCase
+from website import WebsiteTestCase
 
 from trytond.config import config
 
 # Use NereidModuleTestCase as a wrapper for ModuleTestCase
 from nereid.testing import NereidModuleTestCase
 
-#from country import CountryTestCase
-
+# s. #5137
 FROM = 'no-reply@localhost'
 
-class NereidBaseTestCase(
-        NereidModuleTestCase,
-        #AuthTestCase,
-        #AddressTestCase,
-        #CountryTestCase
-        ):
+class NereidBaseTestCase(NereidModuleTestCase):
     "Test Nereid Base module"
     module = 'nereid_base'
 
     def setUp(self):
         super().setUp()
         reset_from = config.get('email', 'from', default='')
         config.set('email', 'from', FROM)
```

### Comparing `m9s_nereid_base-7.0.0/tests/2_test_module.py` & `m9s_nereid_base-7.0.1/tests/routing.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,239 +1,300 @@
-# The COPYRIGHT file at the top level of this repository contains
-# the full copyright notices and license terms.
-
-#from address import AddressTestCase
-#from auth import AuthTestCase
-
-from trytond.config import config
-
-# Use NereidModuleTestCase as a wrapper for ModuleTestCase
-from nereid.testing import NereidModuleTestCase
-
-#from country import CountryTestCase
-
-FROM = 'no-reply@localhost'
-
-
-##########################
-import base64
-import json
+# The COPYRIGHT file at the top level of this repository contains the full
+# copyright notices and license terms.
 import unittest
-import urllib.error
-import urllib.parse
-import urllib.request
 
-from unittest.mock import ANY, patch
+from decimal import Decimal
+
+from wtforms import ValidationError
 
 import trytond.tests.test_tryton
 
-from trytond.config import config
-from trytond.model.modelsql import SQLConstraintError
-from trytond.modules.nereid_base import user as user_module
-from trytond.pool import Pool
-from trytond.sendmail import get_smtp_server
 from trytond.tests.test_tryton import with_transaction
 from trytond.transaction import Transaction
 
-from nereid.testing import POOL as pool
 from nereid.testing import NereidTestCase
 
 from common import setup_objects
-from getpass import getuser
-
-FROM = 'no-reply@localhost'
-#FROM = getuser()
-
 
-#############################
 
-
-
-
-class NereidBaseTestCase(
-        NereidModuleTestCase,
-        #AuthTestCase,
-        #AddressTestCase,
-        #CountryTestCase
-        ):
-    "Test Nereid Base module"
-    module = 'nereid_base'
+class RoutingTestCase(NereidTestCase):
+    'Test URL Routing'
 
     def setUp(self):
-        super().setUp()
-        reset_from = config.get('email', 'from', default='')
-        config.set('email', 'from', FROM)
-        self.addCleanup(lambda: config.set('email', 'from', reset_from))
-
-        trytond.tests.test_tryton.activate_module('nereid_base')
+        trytond.tests.test_tryton.activate_module('nereid_test')
         setup_objects(self)
         self.templates = {
-            'home.jinja': '{{get_flashed_messages()}}',
-            'login.jinja':
-            '{{ login_form.errors }} {{get_flashed_messages()}}',
-            'registration.jinja':
-            '{{ form.errors }} {{get_flashed_messages()}}',
-            'reset-password.jinja': '{{get_flashed_messages()}}',
-            'change-password.jinja':
-            '''{{ change_password_form.errors }}
-            {{get_flashed_messages()}}''',
-            'address-edit.jinja': 'Address Edit {{ form.errors }}',
-            'address.jinja': '',
-            'account.jinja': '',
-            'profile.jinja': '{{ current_user.name }}',
-            'emails/activation-text.jinja': 'activation-email-text',
-            'emails/activation-html.jinja': 'activation-email-html',
-            'emails/reset-text.jinja': 'reset-email-text',
-            'emails/reset-html.jinja': 'reset-email-html',
+            'home.jinja': '{{ Transaction().language }}',
             }
 
     def setup_defaults(self):
         """
         Setup the defaults
         """
-        usd, = self.currency_obj.create([{
+        self.usd, self.eur = self.currency_obj.create([{
             'name': 'US Dollar',
             'code': 'USD',
             'symbol': '$',
+            }, {
+            'name': 'Euro',
+            'code': 'EUR',
+            'symbol': 'E',
+            'rates': [('create', [{'rate': Decimal('2')}])],
             }])
         self.party, = self.party_obj.create([{
             'name': 'MBSolutions',
             }])
         self.company, = self.company_obj.create([{
             'party': self.party,
-            'currency': usd,
+            'currency': self.usd,
+            }])
+        party, = self.party_obj.create([{
+            'name': 'Registered User',
+            }])
+        self.registered_user, = self.nereid_user_obj.create([{
+            'party': party,
+            'name': 'Registered User',
+            'email': 'info@m9s.biz',
+            'password': 'password',
+            'company': self.company,
             }])
 
-        en, = self.language_obj.search([('code', '=', 'en')])
-        currency, = self.currency_obj.search([('code', '=', 'USD')])
-        locale, = self.nereid_website_locale_obj.create([{
+        self.en, = self.language_obj.search([('code', '=', 'en')])
+        self.es, = self.language_obj.search([('code', '=', 'es')])
+        self.locale_en, self.locale_es = self.nereid_website_locale_obj.create(
+            [{
             'code': 'en',
-            'language': en,
-            'currency': currency,
+            'language': self.en,
+            'currency': self.usd,
+            }, {
+            'code': 'es',
+            'language': self.es,
+            'currency': self.eur,
             }])
-        self.nereid_website_obj.create([{
+
+        self.nereid_website, = self.nereid_website_obj.create([{
             'name': 'localhost',
             'company': self.company,
             'application_user': 1,
-            'default_locale': locale,
+            'default_locale': self.locale_en,
+            'locales': [('add', [self.locale_en.id, self.locale_es.id])],
             }])
 
     def get_template_source(self, name):
         """
         Return templates
         """
-
         return self.templates.get(name)
 
+    def get_app(self):
+        """
+        Inject transaction into the template context for the home template
+        """
+        app = super().get_app()
+        app.jinja_env.globals['Transaction'] = Transaction
+        return app
+
     @with_transaction()
-    def test_0010_register(self):
-        #def test_0010_register(self, get_smtp_server):
+    def test_0010_home_with_locales(self):
         """
-        Registration must create a new party
+        When accessing / for website with locales defined, there should be a
+        redirect to the /locale
         """
         self.setup_defaults()
         app = self.get_app()
-        with patch.object(
-                user_module, 'sendmail_transactional') as sendmail, \
-                patch.object(user_module, 'SMTPDataManager') as dm, \
-                app.test_client() as c:
-            print('****************', config.get('email', 'from'))
-            response = c.get('/registration')
-            self.assertEqual(response.status_code, 200)   # GET Request
-
-            email_user = 'regd_user@m9s.biz'
-            data = {
-                'name': 'Registered User',
-                'email': email_user,
-                'password': 'password'
-            }
-            # Post with missing password
-            response = c.post('/registration', data=data)
-            self.assertEqual(response.status_code, 200)  # Form rejected
-
-            # Test that NO email was sent
-            sendmail.assert_not_called()
-
-            data['confirm'] = 'password'
-            response = c.post('/registration', data=data)
-            self.assertEqual(response.status_code, 302)
-
-            # Test if an email was sent
-            print(sendmail.call_args)
-            print(dm.call_args)
-            sendmail.assert_called_once_with(
-                FROM, email_user, ANY,
-                datamanager=ANY)
-            _, _, msg = sendmail.call_args[0]
-            self.assertEqual(msg['From'], FROM)
-            self.assertEqual(msg['Subject'], 'Account Activation')
-            self.assertEqual(msg['To'], email_user)
-            self.assertEqual(msg.get_content_type(), 'multipart/alternative')
-            self.assertEqual(
-                msg.get_payload(0).get_payload(), 'activation-email-text')
-
-        parties = self.party_obj.search([('name', '=', data['name'])])
-
-        self.assertEqual(len(parties), 1)
-        self.assertEqual(len(parties[0].contact_mechanisms), 1)
-        self.assertEqual(parties[0].contact_mechanisms[0].type, 'email')
-        self.assertEqual(parties[0].contact_mechanisms[0].value,
-            'regd_user@m9s.biz')
-
-        with Transaction().set_context(active_test=False):
-            self.assertEqual(self.nereid_user_obj.search(
-                    [('email', '=', data['email'].lower())], count=True), 1)
-
-        # Try to register the same user again (no activated user yet)
-        response = c.post('/registration', data=data)
-        self.assertEqual(response.status_code, 302)
-        with Transaction().set_context(active_test=False):
-            self.assertEqual(self.nereid_user_obj.search(
-                    [('email', '=', data['email'].lower())], count=True), 2)
-
-        # Activate one of the users
-        with Transaction().set_context(active_test=False):
-            user1, user2 = self.nereid_user_obj.search([
-                    ('email', '=', data['email'].lower())
-                    ])
-        user1.active = True
-        user1.email_verified = True
-        user1.save()
-        # Account of user1 must be activated
-        self.assertTrue(user1.active)
-        self.assertTrue(user1.email_verified)
-        self.assertEqual(self.nereid_user_obj.search([
-                    ('email', '=', data['email'].lower()),
-                    ], count=True), 1)
-
-        # Try to activate the second user
-        user2.active = True
-        user2.email_verified = True
-        with self.assertRaises(SQLConstraintError) as cm:
-            user2.save()
-        self.assertEqual(cm.exception.code, 1)
-        self.assertTrue("Email must be unique in a company" in
-            cm.exception.message)
-
-        # Try to register the same user again (activated user present)
-        response = c.post('/registration', data=data)
-        self.assertEqual(response.status_code, 200)
-        self.assertTrue("A registration already exists with this email" in
-            response.data.decode('utf-8'))
-
-        # Deactivate (block) the user
-        user1.active = False
-        user1.save()
-        # Account of user1 must be deactivated (blocked)
-        self.assertFalse(user1.active)
-        self.assertTrue(user1.email_verified)
-
-        # Try to register the same user again (blocked user present)
-        response = c.post('/registration', data=data)
-        self.assertEqual(response.status_code, 200)
-        self.assertTrue("A registration already exists with this email" in
-            response.data.decode('utf-8'))
 
+        with app.test_client() as c:
+            response = c.get('/')
+            self.assertEqual(response.status_code, 308)
+            self.assertEqual(response.location,
+                'http://localhost/%s' % self.locale_en.code)
+
+        # Change the default locale to es and then check
+        self.nereid_website.default_locale = self.locale_es
+        self.nereid_website.save()
+
+        app = self.get_app()
+
+        with app.test_client() as c:
+            response = c.get('/')
+            self.assertEqual(response.status_code, 308)
+            self.assertEqual(response.location,
+                'http://localhost/%s' % self.locale_es.code)
+
+    @with_transaction()
+    def test_0020_home_without_locales(self):
+        """
+        When accessed without locales the site should return 200 on /
+        """
+        self.setup_defaults()
+
+        # unset the locales
+        self.nereid_website.locales = []
+        self.nereid_website.save()
+
+        app = self.get_app()
+
+        with app.test_client() as c:
+            response = c.get('/')
+            self.assertEqual(response.status_code, 200)
+            self.assertEqual(response.data.decode('utf-8'), 'en')
+
+    @with_transaction()
+    def test_0030_lang_context_with_locale(self):
+        """
+        Test that the language available in the context is the right one
+        """
+        self.setup_defaults()
+        app = self.get_app()
+
+        with app.test_client() as c:
+            response = c.get('/en/')
+            self.assertEqual(response.data.decode('utf-8'), 'en')
+
+        with app.test_client() as c:
+            response = c.get('/es/')
+            self.assertEqual(response.data.decode('utf-8'), 'es')
+
+    @with_transaction()
+    def test_0040_lang_context_without_locale(self):
+        """
+        Test that the language available in the context is the right one
+        """
+        self.setup_defaults()
+        self.nereid_website.locales = []
+        self.nereid_website.save()
+        app = self.get_app()
+
+        with app.test_client() as c:
+            response = c.get('/')
+            self.assertEqual(response.data.decode('utf-8'), 'en')
+
+        # Change the default locale to es and then check
+        self.nereid_website.default_locale = self.locale_es
+        self.nereid_website.save()
+
+        with app.test_client() as c:
+            response = c.get('/')
+            self.assertEqual(response.data.decode('utf-8'), 'es')
 
+    @with_transaction()
+    def test_0050_website_routing(self):
+        """
+        Test should not check for match on single website.
+        """
+        self.setup_defaults()
+        self.nereid_website.locales = []
+        self.nereid_website.save()
+        app = self.get_app()
 
+        with app.test_client() as c:
+            response = c.get('http://localhost/')
+            self.assertEqual(response.data.decode('utf-8'), 'en')
+
+            response = c.get('http://any_single_website_should_generally_work/')
+            self.assertEqual(response.data.decode('utf-8'), 'en')
+
+            self.nereid_website_obj.create([{
+                'name': 'another_website',
+                'company': self.company,
+                'application_user': 1,
+                'default_locale': self.locale_en,
+            }])
+
+            # Should break, as there are more than 1 website.
+            response = c.get('http://this_should_break/')
+            self.assertEqual(response.status_code, 404)
+            self.assertIn(
+                'The requested website was not found on the server',
+                response.data.decode('utf-8'))
+
+    @with_transaction()
+    def test_0060_invalid_active_id_url(self):
+        """
+        Test that the url in 404 if record for active_id doesn't exist
+        """
+        self.setup_defaults()
+        self.nereid_website.locales = []
+        self.nereid_website.save()
+        app = self.get_app()
+        country, = self.country_obj.create([{
+            'name': 'India',
+            'code': 'IN'
+            }])
+
+        with app.test_client() as c:
+            response = c.get('/countries/%d/subdivisions' % country.id)
+            self.assertEqual(response.status_code, 200)
+
+            response = c.get('/countries/6/subdivisions')  # Invalid record
+            self.assertEqual(response.status_code, 404)
+
+    @with_transaction()
+    def test_0070_csrf(self):
+        """
+        Test that the csrf for POST request works
+        """
+        self.setup_defaults()
+        self.nereid_website.locales = []
+        self.nereid_website.save()
+        app = self.get_app()
+        # Enable CSRF
+        app.config['WTF_CSRF_ENABLED'] = True
+
+        with app.test_client() as c:
+            # NO csrf-token
+            response = c.post('/test-csrf',
+                data={
+                    'name': 'dummy name'
+                })
+            self.assertEqual(response.status_code, 400)
+            self.assertIn(
+                'The CSRF token is missing.',
+                response.data.decode('utf-8'))
+
+            # csrf token with invalid form
+            csrf_token = c.get('/gen-csrf').data.decode('utf-8')
+            response = c.post('/test-csrf',
+                data={
+                    'csrf_token': csrf_token,
+                })
+            self.assertEqual(response.status_code, 200)
+            self.assertEqual(response.data.decode('utf-8'), 'Failure')
+
+            # csrf token with valid form
+            csrf_token = c.get('/gen-csrf').data.decode('utf-8')
+            response = c.post('/test-csrf',
+                data={
+                    'name': 'dummy name',
+                    'csrf_token': csrf_token,
+                })
+            self.assertEqual(response.status_code, 200)
+            self.assertEqual(response.data.decode('utf-8'), 'Success')
+
+    @with_transaction()
+    def test_0070_csrf_exempt(self):
+        """
+        Test that the csrf exempt for POST request works
+        """
+        self.setup_defaults()
+        self.nereid_website.locales = []
+        self.nereid_website.save()
+        app = self.get_app()
+        # Enable CSRF
+        app.config['WTF_CSRF_ENABLED'] = True
 
-del NereidModuleTestCase
+        with app.test_client() as c:
+            # invalid form
+            response = c.post('/test-csrf-exempt',
+                data={
+                    'name': '',
+                })
+            self.assertEqual(response.status_code, 200)
+            self.assertEqual(response.data.decode('utf-8'), 'Failure')
+
+            # valid form
+            response = c.post('/test-csrf-exempt',
+                data={
+                    'name': 'dummy name',
+                })
+            self.assertEqual(response.status_code, 200)
+            self.assertEqual(response.data.decode('utf-8'), 'Success')
```

### Comparing `m9s_nereid_base-7.0.0/tests/address.py` & `m9s_nereid_base-7.0.1/tests/address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 # The COPYRIGHT file at the top level of this repository contains the full
 # copyright notices and license terms.
 import json
-import unittest
 
 from unittest.mock import patch
 
 import pycountry
 
 import trytond.tests.test_tryton
 
 from trytond.config import config
-from trytond.pool import Pool
 from trytond.tests.test_tryton import with_transaction
-from trytond.transaction import Transaction
 
-from nereid.testing import POOL as pool
 from nereid.testing import NereidTestCase
 
 from common import setup_objects
 
 config.set('email', 'from', 'from@xyz.com')
```

### Comparing `m9s_nereid_base-7.0.0/tests/common.py` & `m9s_nereid_base-7.0.1/tests/common.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/tests/country.py` & `m9s_nereid_base-7.0.1/tests/country.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
 # The COPYRIGHT file at the top level of this repository contains the full
 # copyright notices and license terms.
 import json
-import unittest
 
 from decimal import Decimal
 
 import trytond.tests.test_tryton
 
 from trytond.tests.test_tryton import with_transaction
```

### Comparing `m9s_nereid_base-7.0.0/tests/currency.py` & `m9s_nereid_base-7.0.1/tests/currency.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # The COPYRIGHT file at the top level of this repository contains the full
 # copyright notices and license terms.
-import unittest
-
 from decimal import Decimal
 
+from common import setup_objects
+
 import trytond.tests.test_tryton
 
 from trytond.tests.test_tryton import with_transaction
 
 from nereid import render_template
 from nereid.testing import NereidTestCase
 
-from common import setup_objects
-
 
 class CurrencyTestCase(NereidTestCase):
     """
     Test Currency
     """
 
     def setUp(self):
@@ -151,20 +149,19 @@
                 Decimal('200'))
 
     @with_transaction()
     def test_0030_get_currencies(self):
         """
         Test and ensure that get_currencies() works (includes caching)
         """
+        self.setup_defaults()
         self.templates = {
             'home.jinja':
                 '''
                 {{ current_website.get_currencies() }}
                 ''',
                 }
-
-        self.setup_defaults()
         app = self.get_app()
 
         with app.test_request_context('/en/'):
             home_template = render_template('home.jinja')
             self.assertTrue('1' in home_template)
```

### Comparing `m9s_nereid_base-7.0.0/tests/i18n.py` & `m9s_nereid_base-7.0.1/tests/i18n.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/tests/static_file.py` & `m9s_nereid_base-7.0.1/tests/static_file.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/tests/translation.py` & `m9s_nereid_base-7.0.1/tests/translation.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/tests/user.py` & `m9s_nereid_base-7.0.1/tests/user.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/tests/website.py` & `m9s_nereid_base-7.0.1/tests/website.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/tox.ini` & `m9s_nereid_base-7.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/translation.py` & `m9s_nereid_base-7.0.1/translation.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/user.py` & `m9s_nereid_base-7.0.1/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,22 @@
 import pytz
 
 from flask_login import AnonymousUserMixin, login_url, login_user, logout_user
 from flask_wtf import FlaskForm as Form
 from flask_wtf import RecaptchaField
 from itsdangerous import BadSignature, SignatureExpired, URLSafeTimedSerializer
 from sql import Literal
-from sql.conditionals import Coalesce
-from sql.operators import Concat, Equal
+from sql.operators import Equal
 from werkzeug.exceptions import abort
 from werkzeug.utils import redirect
 from wtforms import PasswordField, SelectField, StringField, validators
 
 from trytond.config import config
 from trytond.model import (
-    DeactivableMixin, Exclude, ModelSQL, ModelView, fields)
+    DeactivableMixin, Exclude, Index, ModelSQL, ModelView, fields)
 from trytond.pool import Pool
 from trytond.pyson import Bool, Eval, Not
 from trytond.res.user import CRYPT_CONTEXT, PasswordError
 from trytond.rpc import RPC
 from trytond.sendmail import SMTPDataManager, sendmail_transactional
 from trytond.transaction import Transaction
 
@@ -114,15 +113,14 @@
         description="Your Login Email."
     )
 
 
 class NereidUser(DeactivableMixin, ModelSQL, ModelView):
     "Web User"
     __name__ = "nereid.user"
-    _rec_name = 'name'
 
     party = fields.Many2One('party.party', 'Party', required=True,
         ondelete='CASCADE',
         context={
             'company': Eval('company', -1),
             },
         depends=['company'])
@@ -150,44 +148,34 @@
 
     # .. versionchanged:: 7.0
     #     Use the URLSafeTimedSerializer, remove the separate signer
     #     Only use the serializer and pass through the options for the signer
 
     @classmethod
     def __setup__(cls):
-        super(NereidUser, cls).__setup__()
-        table = cls.__table__()
+        cls.email.search_unaccented = False
+        super().__setup__()
+        t = cls.__table__()
+        cls._sql_indexes.update({
+                Index(t, (t.email, Index.Similarity())),
+                })
         cls._sql_constraints += [
             ('email_exclude',
-                Exclude(table, (table.email, Equal), (table.company, Equal),
-                    where=table.active == Literal(True)),
+                Exclude(t, (t.email, Equal), (t.company, Equal),
+                    where=t.active == Literal(True)),
                 'nereid_base.msg_user_email_unique'),
             ]
         cls.__rpc__.update({
             'match_password': RPC(readonly=True, instantiate=0),
-        })
+            })
 
-    @classmethod
-    def __register__(cls, module_name):
-        cursor = Transaction().connection.cursor()
-        super(NereidUser, cls).__register__(module_name)
-        table = cls.__table_handler__(module_name)
-
-        # Migration from 4.0
-        if table.column_exist('password') and table.column_exist('salt'):
-            sqltable = cls.__table__()
-            password_hash_new = Concat('sha1$', Concat(sqltable.password,
-                Concat('$', Coalesce(sqltable.salt, ''))))
-            cursor.execute(*sqltable.update(
-                columns=[sqltable.password_hash],
-                values=[password_hash_new]))
-            table.drop_column('password')
-            table.drop_column('salt')
-        # Migration from 5.2.23: Replace Unique by Exclude constraint
-        table.drop_constraint('unique_email_company')
+    def get_rec_name(self, name):
+        if self.name:
+            return self.name
+        return self.party.rec_name
 
     @classmethod
     def search_rec_name(cls, name, clause):
         return ['OR',
             ('party',) + tuple(clause[1:]),
             ('name',) + tuple(clause[1:]),
             ('email',) + tuple(clause[1:]),
```

### Comparing `m9s_nereid_base-7.0.0/view/nereid_user_form2.xml` & `m9s_nereid_base-7.0.1/view/nereid_user_form2.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/view/static_file_form.xml` & `m9s_nereid_base-7.0.1/view/static_file_form.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/view/website_form.xml` & `m9s_nereid_base-7.0.1/view/website_form.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.0/website.py` & `m9s_nereid_base-7.0.1/website.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,16 @@
     #:  .. versionadded: 0.3
     application_user = fields.Many2One(
         'res.user', 'Application User', required=True
     )
 
     timezone = fields.Function(
         fields.Selection(
-            [(x, x) for x in pytz.common_timezones], 'Timezone', translate=False
+            [(x, x) for x in pytz.common_timezones],
+            'Timezone', translate=False
         ), getter="get_timezone"
     )
     #: Remove deprecated post method user_status.
     #: Login state is better performed with current_user.is_anonymous
     #:
     #: .. versionchanged:: 6.0.11
```


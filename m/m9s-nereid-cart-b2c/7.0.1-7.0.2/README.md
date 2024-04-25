# Comparing `tmp/m9s_nereid_cart_b2c-7.0.1.tar.gz` & `tmp/m9s_nereid_cart_b2c-7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m9s_nereid_cart_b2c-7.0.1.tar", last modified: Wed Feb  7 15:38:04 2024, max compression
+gzip compressed data, was "m9s_nereid_cart_b2c-7.0.2.tar", last modified: Thu Apr 25 14:09:26 2024, max compression
```

## Comparing `m9s_nereid_cart_b2c-7.0.1.tar` & `m9s_nereid_cart_b2c-7.0.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-07 15:38:04.419000 m9s_nereid_cart_b2c-7.0.1/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       85 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/.coveragerc
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-13 19:22:51.000000 m9s_nereid_cart_b2c-7.0.1/.drone.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/.flake8
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/.gitlab-ci-m9s.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1905 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/.gitlab-ci.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/.isort.cfg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      175 2018-02-28 18:26:37.000000 m9s_nereid_cart_b2c-7.0.1/.travis.yml
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-07 15:38:04.419000 m9s_nereid_cart_b2c-7.0.1/.woodpecker/
--rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/.woodpecker/mail_curl.sh
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/.woodpecker/report.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/.woodpecker/test.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1584 2018-02-28 18:26:37.000000 m9s_nereid_cart_b2c-7.0.1/CHANGELOG
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      798 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/COPYRIGHT
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/INSTALL
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/LICENSE
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/MANIFEST.in
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3430 2024-02-07 15:38:04.419000 m9s_nereid_cart_b2c-7.0.1/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1252 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/README.md
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/README.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      447 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       15 2018-02-28 18:26:37.000000 m9s_nereid_cart_b2c-7.0.1/babel.cfg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    18076 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/cart.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      424 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/channel.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/dev_requirements.txt
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-07 15:38:04.419000 m9s_nereid_cart_b2c-7.0.1/doc/
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-07 15:38:04.419000 m9s_nereid_cart_b2c-7.0.1/doc/de/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       45 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/doc/de/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/doc/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      583 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/forms.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-07 15:38:04.419000 m9s_nereid_cart_b2c-7.0.1/locale/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4838 2022-04-12 07:18:46.000000 m9s_nereid_cart_b2c-7.0.1/locale/de.po
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-07 15:38:04.419000 m9s_nereid_cart_b2c-7.0.1/m9s_nereid_cart_b2c.egg-info/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3430 2024-02-07 15:38:04.000000 m9s_nereid_cart_b2c-7.0.1/m9s_nereid_cart_b2c.egg-info/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1199 2024-02-07 15:38:04.000000 m9s_nereid_cart_b2c-7.0.1/m9s_nereid_cart_b2c.egg-info/SOURCES.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-02-07 15:38:04.000000 m9s_nereid_cart_b2c-7.0.1/m9s_nereid_cart_b2c.egg-info/dependency_links.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       68 2024-02-07 15:38:04.000000 m9s_nereid_cart_b2c-7.0.1/m9s_nereid_cart_b2c.egg-info/entry_points.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2021-05-15 14:09:14.000000 m9s_nereid_cart_b2c-7.0.1/m9s_nereid_cart_b2c.egg-info/not-zip-safe
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      177 2024-02-07 15:38:04.000000 m9s_nereid_cart_b2c-7.0.1/m9s_nereid_cart_b2c.egg-info/requires.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-02-07 15:38:04.000000 m9s_nereid_cart_b2c-7.0.1/m9s_nereid_cart_b2c.egg-info/top_level.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      368 2022-02-15 16:36:58.000000 m9s_nereid_cart_b2c-7.0.1/message.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    10139 2024-02-06 17:29:20.000000 m9s_nereid_cart_b2c-7.0.1/product.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      448 2020-02-16 22:15:22.000000 m9s_nereid_cart_b2c-7.0.1/product.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/requirements.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     7497 2024-02-07 15:05:31.000000 m9s_nereid_cart_b2c-7.0.1/sale.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      959 2021-02-01 00:55:51.000000 m9s_nereid_cart_b2c-7.0.1/sale.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      223 2024-02-07 15:38:04.423000 m9s_nereid_cart_b2c-7.0.1/setup.cfg
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4679 2024-02-05 17:42:06.000000 m9s_nereid_cart_b2c-7.0.1/setup.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      278 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/signals.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-07 15:38:04.419000 m9s_nereid_cart_b2c-7.0.1/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      330 2024-02-07 15:37:19.000000 m9s_nereid_cart_b2c-7.0.1/tests/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    17584 2022-04-30 16:01:46.000000 m9s_nereid_cart_b2c-7.0.1/tests/scenario.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    61589 2024-02-07 10:50:13.000000 m9s_nereid_cart_b2c-7.0.1/tests/test_module.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/tox.ini
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      181 2024-02-07 15:12:34.000000 m9s_nereid_cart_b2c-7.0.1/tryton.cfg
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-07 15:38:04.419000 m9s_nereid_cart_b2c-7.0.1/view/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      769 2020-02-16 22:14:59.000000 m9s_nereid_cart_b2c-7.0.1/view/product_form_nereid.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      504 2020-02-16 22:14:59.000000 m9s_nereid_cart_b2c-7.0.1/view/website_view_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6358 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.1/website.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      435 2024-02-05 18:24:51.000000 m9s_nereid_cart_b2c-7.0.1/website.xml
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:09:26.346629 m9s_nereid_cart_b2c-7.0.2/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       85 2024-04-25 09:39:28.000000 m9s_nereid_cart_b2c-7.0.2/.coveragerc
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-13 19:22:51.000000 m9s_nereid_cart_b2c-7.0.2/.drone.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-04-25 09:39:28.000000 m9s_nereid_cart_b2c-7.0.2/.flake8
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-04-25 09:39:28.000000 m9s_nereid_cart_b2c-7.0.2/.gitlab-ci-m9s.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2217 2024-04-25 09:39:28.000000 m9s_nereid_cart_b2c-7.0.2/.gitlab-ci.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2024-04-25 09:39:28.000000 m9s_nereid_cart_b2c-7.0.2/.isort.cfg
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      175 2018-02-28 18:26:37.000000 m9s_nereid_cart_b2c-7.0.2/.travis.yml
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:09:26.346629 m9s_nereid_cart_b2c-7.0.2/.woodpecker/
+-rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2024-04-25 09:39:28.000000 m9s_nereid_cart_b2c-7.0.2/.woodpecker/mail_curl.sh
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2024-04-25 09:39:28.000000 m9s_nereid_cart_b2c-7.0.2/.woodpecker/report.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2024-04-25 09:39:28.000000 m9s_nereid_cart_b2c-7.0.2/.woodpecker/test.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1584 2018-02-28 18:26:37.000000 m9s_nereid_cart_b2c-7.0.2/CHANGELOG
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      798 2024-04-25 09:39:28.000000 m9s_nereid_cart_b2c-7.0.2/COPYRIGHT
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2024-04-25 09:39:28.000000 m9s_nereid_cart_b2c-7.0.2/INSTALL
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2024-04-25 09:39:28.000000 m9s_nereid_cart_b2c-7.0.2/LICENSE
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2024-04-25 09:39:28.000000 m9s_nereid_cart_b2c-7.0.2/MANIFEST.in
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3240 2024-04-25 14:09:26.346629 m9s_nereid_cart_b2c-7.0.2/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1062 2024-04-25 09:39:28.000000 m9s_nereid_cart_b2c-7.0.2/README.md
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-04-25 09:39:28.000000 m9s_nereid_cart_b2c-7.0.2/README.rst
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      447 2024-04-25 09:39:28.000000 m9s_nereid_cart_b2c-7.0.2/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       15 2018-02-28 18:26:37.000000 m9s_nereid_cart_b2c-7.0.2/babel.cfg
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    18342 2024-04-25 09:34:16.000000 m9s_nereid_cart_b2c-7.0.2/cart.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      424 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.2/channel.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       86 2024-04-25 09:39:28.000000 m9s_nereid_cart_b2c-7.0.2/dev_requirements.txt
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:09:26.346629 m9s_nereid_cart_b2c-7.0.2/doc/
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:09:26.346629 m9s_nereid_cart_b2c-7.0.2/doc/de/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       45 2024-04-25 09:39:28.000000 m9s_nereid_cart_b2c-7.0.2/doc/de/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-04-25 09:39:28.000000 m9s_nereid_cart_b2c-7.0.2/doc/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      583 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.2/forms.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:09:26.346629 m9s_nereid_cart_b2c-7.0.2/locale/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4838 2022-04-12 07:18:46.000000 m9s_nereid_cart_b2c-7.0.2/locale/de.po
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:09:26.346629 m9s_nereid_cart_b2c-7.0.2/m9s_nereid_cart_b2c.egg-info/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3240 2024-04-25 14:09:26.000000 m9s_nereid_cart_b2c-7.0.2/m9s_nereid_cart_b2c.egg-info/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1199 2024-04-25 14:09:26.000000 m9s_nereid_cart_b2c-7.0.2/m9s_nereid_cart_b2c.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-04-25 14:09:26.000000 m9s_nereid_cart_b2c-7.0.2/m9s_nereid_cart_b2c.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       68 2024-04-25 14:09:26.000000 m9s_nereid_cart_b2c-7.0.2/m9s_nereid_cart_b2c.egg-info/entry_points.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2021-05-15 14:09:14.000000 m9s_nereid_cart_b2c-7.0.2/m9s_nereid_cart_b2c.egg-info/not-zip-safe
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      177 2024-04-25 14:09:26.000000 m9s_nereid_cart_b2c-7.0.2/m9s_nereid_cart_b2c.egg-info/requires.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-04-25 14:09:26.000000 m9s_nereid_cart_b2c-7.0.2/m9s_nereid_cart_b2c.egg-info/top_level.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      368 2022-02-15 16:36:58.000000 m9s_nereid_cart_b2c-7.0.2/message.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    10139 2024-02-06 17:29:20.000000 m9s_nereid_cart_b2c-7.0.2/product.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      448 2020-02-16 22:15:22.000000 m9s_nereid_cart_b2c-7.0.2/product.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2024-04-25 09:39:28.000000 m9s_nereid_cart_b2c-7.0.2/requirements.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     7497 2024-02-07 15:05:31.000000 m9s_nereid_cart_b2c-7.0.2/sale.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      959 2021-02-01 00:55:51.000000 m9s_nereid_cart_b2c-7.0.2/sale.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      223 2024-04-25 14:09:26.346629 m9s_nereid_cart_b2c-7.0.2/setup.cfg
+-rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     4679 2024-04-25 09:39:28.000000 m9s_nereid_cart_b2c-7.0.2/setup.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      278 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.2/signals.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:09:26.346629 m9s_nereid_cart_b2c-7.0.2/tests/
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      330 2024-04-25 09:39:28.000000 m9s_nereid_cart_b2c-7.0.2/tests/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    17584 2022-04-30 16:01:46.000000 m9s_nereid_cart_b2c-7.0.2/tests/scenario.rst
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    61589 2024-04-25 09:39:28.000000 m9s_nereid_cart_b2c-7.0.2/tests/test_module.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2024-04-25 09:39:28.000000 m9s_nereid_cart_b2c-7.0.2/tox.ini
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      181 2024-04-25 09:39:28.000000 m9s_nereid_cart_b2c-7.0.2/tryton.cfg
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:09:26.346629 m9s_nereid_cart_b2c-7.0.2/view/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      769 2020-02-16 22:14:59.000000 m9s_nereid_cart_b2c-7.0.2/view/product_form_nereid.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      504 2020-02-16 22:14:59.000000 m9s_nereid_cart_b2c-7.0.2/view/website_view_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6358 2024-01-22 10:56:08.000000 m9s_nereid_cart_b2c-7.0.2/website.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      435 2024-02-05 18:24:51.000000 m9s_nereid_cart_b2c-7.0.2/website.xml
```

### Comparing `m9s_nereid_cart_b2c-7.0.1/.drone.yml` & `m9s_nereid_cart_b2c-7.0.2/.drone.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_cart_b2c-7.0.1/.gitlab-ci.yml` & `m9s_nereid_cart_b2c-7.0.2/.gitlab-ci.yml`

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

### Comparing `m9s_nereid_cart_b2c-7.0.1/.woodpecker/mail_curl.sh` & `m9s_nereid_cart_b2c-7.0.2/.woodpecker/mail_curl.sh`

 * *Files identical despite different names*

### Comparing `m9s_nereid_cart_b2c-7.0.1/.woodpecker/report.yml` & `m9s_nereid_cart_b2c-7.0.2/.woodpecker/report.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_cart_b2c-7.0.1/.woodpecker/test.yml` & `m9s_nereid_cart_b2c-7.0.2/.woodpecker/test.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_cart_b2c-7.0.1/CHANGELOG` & `m9s_nereid_cart_b2c-7.0.2/CHANGELOG`

 * *Files identical despite different names*

### Comparing `m9s_nereid_cart_b2c-7.0.1/COPYRIGHT` & `m9s_nereid_cart_b2c-7.0.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `m9s_nereid_cart_b2c-7.0.1/INSTALL` & `m9s_nereid_cart_b2c-7.0.2/INSTALL`

 * *Files identical despite different names*

### Comparing `m9s_nereid_cart_b2c-7.0.1/LICENSE` & `m9s_nereid_cart_b2c-7.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `m9s_nereid_cart_b2c-7.0.1/PKG-INFO` & `m9s_nereid_cart_b2c-7.0.2/m9s_nereid_cart_b2c.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: m9s_nereid_cart_b2c
-Version: 7.0.1
+Name: m9s-nereid-cart-b2c
+Version: 7.0.2
 Summary: Tryton Nereid Cart B2C Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/nereid_cart_b2c.git
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
-[![Pipeline status](https://gitlab.com/m9s/nereid_cart_b2c/badges/master/pipeline.svg)](https://gitlab.com/m9s/nereid_cart_b2c/commits/master)
-
-Develop
-
-[![Pipeline status](https://gitlab.com/m9s/nereid_cart_b2c/badges/develop/pipeline.svg)](https://gitlab.com/m9s/nereid_cart_b2c/commits/develop)
-
-[![Coverage report](https://gitlab.com/m9s/nereid_cart_b2c/badges/develop/coverage.svg)](http://m9s.gitlab.io/nereid_cart_b2c)
-
+[![Tests Status](https://m9s.gitlab.io/nereid_cart_b2c/junit/junit-badge.svg)](https://m9s.gitlab.io/nereid_cart_b2c)
 
+[![Coverage Status](https://m9s.gitlab.io/nereid_cart_b2c/coverage/coverage-badge.svg)](https://m9s.gitlab.io/nereid_cart_b2c)
 
 This module runs with the Tryton application platform.
 
 Installing
 ----------
 
 See INSTALL
```

### Comparing `m9s_nereid_cart_b2c-7.0.1/README.md` & `m9s_nereid_cart_b2c-7.0.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,10 @@
-Master
-
-[![Pipeline status](https://gitlab.com/m9s/nereid_cart_b2c/badges/master/pipeline.svg)](https://gitlab.com/m9s/nereid_cart_b2c/commits/master)
-
-Develop
-
-[![Pipeline status](https://gitlab.com/m9s/nereid_cart_b2c/badges/develop/pipeline.svg)](https://gitlab.com/m9s/nereid_cart_b2c/commits/develop)
-
-[![Coverage report](https://gitlab.com/m9s/nereid_cart_b2c/badges/develop/coverage.svg)](http://m9s.gitlab.io/nereid_cart_b2c)
-
+[![Tests Status](https://m9s.gitlab.io/nereid_cart_b2c/junit/junit-badge.svg)](https://m9s.gitlab.io/nereid_cart_b2c)
 
+[![Coverage Status](https://m9s.gitlab.io/nereid_cart_b2c/coverage/coverage-badge.svg)](https://m9s.gitlab.io/nereid_cart_b2c)
 
 This module runs with the Tryton application platform.
 
 Installing
 ----------
 
 See INSTALL
```

### Comparing `m9s_nereid_cart_b2c-7.0.1/cart.py` & `m9s_nereid_cart_b2c-7.0.2/cart.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from decimal import Decimal
 from functools import partial
 
 from babel import numbers
 from flask_login import user_logged_in
 from werkzeug.utils import redirect
 
-from trytond.model import ModelSQL, ModelView, fields
+from trytond.model import Index, ModelSQL, ModelView, fields
 from trytond.pool import Pool
 
 from nereid import (
     Nereid, abort, context_processor, current_locale, current_user,
     current_website, flash, jsonify, login_required, render_template, request,
     route, url_for)
 from nereid.contrib.locale import make_lazy_gettext
@@ -39,14 +39,23 @@
     """
 
     user = fields.Many2One('nereid.user', 'Cart owner')
     sale = fields.Many2One('sale.sale', 'Sale Order')
     sessionid = fields.Char('Session ID')
     website = fields.Many2One('nereid.website', 'Website')
 
+    @classmethod
+    def __setup__(cls):
+        super().__setup__()
+        t = cls.__table__()
+        cls._sql_indexes.update({
+                Index(t, (t.user, Index.Equality())),
+                Index(t, (t.sale, Index.Equality())),
+                })
+
     @staticmethod
     def default_user():
         if has_request_context() and not current_user.is_anonymous:
             return current_user.id
 
     @staticmethod
     def default_sessionid():
```

### Comparing `m9s_nereid_cart_b2c-7.0.1/forms.py` & `m9s_nereid_cart_b2c-7.0.2/forms.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_cart_b2c-7.0.1/locale/de.po` & `m9s_nereid_cart_b2c-7.0.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `m9s_nereid_cart_b2c-7.0.1/m9s_nereid_cart_b2c.egg-info/PKG-INFO` & `m9s_nereid_cart_b2c-7.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: m9s-nereid-cart-b2c
-Version: 7.0.1
+Name: m9s_nereid_cart_b2c
+Version: 7.0.2
 Summary: Tryton Nereid Cart B2C Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/nereid_cart_b2c.git
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
-[![Pipeline status](https://gitlab.com/m9s/nereid_cart_b2c/badges/master/pipeline.svg)](https://gitlab.com/m9s/nereid_cart_b2c/commits/master)
-
-Develop
-
-[![Pipeline status](https://gitlab.com/m9s/nereid_cart_b2c/badges/develop/pipeline.svg)](https://gitlab.com/m9s/nereid_cart_b2c/commits/develop)
-
-[![Coverage report](https://gitlab.com/m9s/nereid_cart_b2c/badges/develop/coverage.svg)](http://m9s.gitlab.io/nereid_cart_b2c)
-
+[![Tests Status](https://m9s.gitlab.io/nereid_cart_b2c/junit/junit-badge.svg)](https://m9s.gitlab.io/nereid_cart_b2c)
 
+[![Coverage Status](https://m9s.gitlab.io/nereid_cart_b2c/coverage/coverage-badge.svg)](https://m9s.gitlab.io/nereid_cart_b2c)
 
 This module runs with the Tryton application platform.
 
 Installing
 ----------
 
 See INSTALL
```

### Comparing `m9s_nereid_cart_b2c-7.0.1/m9s_nereid_cart_b2c.egg-info/SOURCES.txt` & `m9s_nereid_cart_b2c-7.0.2/m9s_nereid_cart_b2c.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m9s_nereid_cart_b2c-7.0.1/product.py` & `m9s_nereid_cart_b2c-7.0.2/product.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_cart_b2c-7.0.1/sale.py` & `m9s_nereid_cart_b2c-7.0.2/sale.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_cart_b2c-7.0.1/sale.xml` & `m9s_nereid_cart_b2c-7.0.2/sale.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_cart_b2c-7.0.1/setup.py` & `m9s_nereid_cart_b2c-7.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_cart_b2c-7.0.1/tests/scenario.rst` & `m9s_nereid_cart_b2c-7.0.2/tests/scenario.rst`

 * *Files identical despite different names*

### Comparing `m9s_nereid_cart_b2c-7.0.1/tests/test_module.py` & `m9s_nereid_cart_b2c-7.0.2/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_cart_b2c-7.0.1/tox.ini` & `m9s_nereid_cart_b2c-7.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `m9s_nereid_cart_b2c-7.0.1/view/product_form_nereid.xml` & `m9s_nereid_cart_b2c-7.0.2/view/product_form_nereid.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_cart_b2c-7.0.1/website.py` & `m9s_nereid_cart_b2c-7.0.2/website.py`

 * *Files identical despite different names*


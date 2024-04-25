# Comparing `tmp/m9s_nereid_catalog_tree-7.0.0.tar.gz` & `tmp/m9s_nereid_catalog_tree-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m9s_nereid_catalog_tree-7.0.0.tar", last modified: Mon Feb  5 11:05:39 2024, max compression
+gzip compressed data, was "m9s_nereid_catalog_tree-7.0.1.tar", last modified: Thu Apr 25 14:12:34 2024, max compression
```

## Comparing `m9s_nereid_catalog_tree-7.0.0.tar` & `m9s_nereid_catalog_tree-7.0.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-05 11:05:39.086818 m9s_nereid_catalog_tree-7.0.0/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       89 2024-01-22 10:56:08.000000 m9s_nereid_catalog_tree-7.0.0/.coveragerc
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-13 19:22:51.000000 m9s_nereid_catalog_tree-7.0.0/.drone.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-01-22 10:56:08.000000 m9s_nereid_catalog_tree-7.0.0/.flake8
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-01-22 10:56:08.000000 m9s_nereid_catalog_tree-7.0.0/.gitlab-ci-m9s.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1905 2024-01-22 10:56:08.000000 m9s_nereid_catalog_tree-7.0.0/.gitlab-ci.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2024-01-22 10:56:08.000000 m9s_nereid_catalog_tree-7.0.0/.isort.cfg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      310 2018-02-28 18:26:33.000000 m9s_nereid_catalog_tree-7.0.0/.travis.yml
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-05 11:05:39.086818 m9s_nereid_catalog_tree-7.0.0/.woodpecker/
--rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2024-01-22 10:56:08.000000 m9s_nereid_catalog_tree-7.0.0/.woodpecker/mail_curl.sh
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2024-01-22 10:56:08.000000 m9s_nereid_catalog_tree-7.0.0/.woodpecker/report.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2024-01-22 10:56:08.000000 m9s_nereid_catalog_tree-7.0.0/.woodpecker/test.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      135 2018-02-28 18:26:33.000000 m9s_nereid_catalog_tree-7.0.0/CHANGELOG.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      798 2024-01-22 10:56:08.000000 m9s_nereid_catalog_tree-7.0.0/COPYRIGHT
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2024-01-22 10:56:08.000000 m9s_nereid_catalog_tree-7.0.0/INSTALL
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2024-01-22 10:56:08.000000 m9s_nereid_catalog_tree-7.0.0/LICENSE
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2024-01-22 10:56:08.000000 m9s_nereid_catalog_tree-7.0.0/MANIFEST.in
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3474 2024-02-05 11:05:39.086818 m9s_nereid_catalog_tree-7.0.0/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1280 2024-01-22 10:56:08.000000 m9s_nereid_catalog_tree-7.0.0/README.md
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       54 2024-01-22 10:56:08.000000 m9s_nereid_catalog_tree-7.0.0/README.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      410 2024-01-22 10:56:08.000000 m9s_nereid_catalog_tree-7.0.0/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6192 2018-05-20 21:10:01.000000 m9s_nereid_catalog_tree-7.0.0/de.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-01-22 10:56:08.000000 m9s_nereid_catalog_tree-7.0.0/dev_requirements.txt
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-05 11:05:39.086818 m9s_nereid_catalog_tree-7.0.0/doc/
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-05 11:05:39.086818 m9s_nereid_catalog_tree-7.0.0/doc/de/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       53 2024-01-22 10:56:08.000000 m9s_nereid_catalog_tree-7.0.0/doc/de/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       54 2024-01-22 10:56:08.000000 m9s_nereid_catalog_tree-7.0.0/doc/index.rst
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-05 11:05:39.086818 m9s_nereid_catalog_tree-7.0.0/locale/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6267 2023-10-25 11:36:03.000000 m9s_nereid_catalog_tree-7.0.0/locale/de.po
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-05 11:05:39.086818 m9s_nereid_catalog_tree-7.0.0/m9s_nereid_catalog_tree.egg-info/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3474 2024-02-05 11:05:38.000000 m9s_nereid_catalog_tree-7.0.0/m9s_nereid_catalog_tree.egg-info/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1213 2024-02-05 11:05:39.000000 m9s_nereid_catalog_tree-7.0.0/m9s_nereid_catalog_tree.egg-info/SOURCES.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-02-05 11:05:38.000000 m9s_nereid_catalog_tree-7.0.0/m9s_nereid_catalog_tree.egg-info/dependency_links.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       76 2024-02-05 11:05:38.000000 m9s_nereid_catalog_tree-7.0.0/m9s_nereid_catalog_tree.egg-info/entry_points.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2020-01-11 14:42:36.000000 m9s_nereid_catalog_tree-7.0.0/m9s_nereid_catalog_tree.egg-info/not-zip-safe
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       69 2024-02-05 11:05:38.000000 m9s_nereid_catalog_tree-7.0.0/m9s_nereid_catalog_tree.egg-info/requires.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-02-05 11:05:38.000000 m9s_nereid_catalog_tree-7.0.0/m9s_nereid_catalog_tree.egg-info/top_level.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2024-01-22 10:56:08.000000 m9s_nereid_catalog_tree-7.0.0/requirements.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-02-05 11:05:39.086818 m9s_nereid_catalog_tree-7.0.0/setup.cfg
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4500 2024-02-05 10:34:43.000000 m9s_nereid_catalog_tree-7.0.0/setup.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-05 11:05:39.086818 m9s_nereid_catalog_tree-7.0.0/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      115 2024-01-22 10:56:08.000000 m9s_nereid_catalog_tree-7.0.0/tests/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    28906 2024-02-05 11:03:09.000000 m9s_nereid_catalog_tree-7.0.0/tests/test_module.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2024-01-22 10:56:08.000000 m9s_nereid_catalog_tree-7.0.0/tox.ini
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    11550 2024-02-05 11:03:57.000000 m9s_nereid_catalog_tree-7.0.0/tree.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5712 2024-02-05 10:37:45.000000 m9s_nereid_catalog_tree-7.0.0/tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      104 2024-01-22 10:56:08.000000 m9s_nereid_catalog_tree-7.0.0/tryton.cfg
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-05 11:05:39.086818 m9s_nereid_catalog_tree-7.0.0/view/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      401 2020-01-11 16:44:15.000000 m9s_nereid_catalog_tree-7.0.0/view/product_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      254 2022-02-15 17:51:35.000000 m9s_nereid_catalog_tree-7.0.0/view/product_node_list.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      228 2022-02-15 17:52:56.000000 m9s_nereid_catalog_tree-7.0.0/view/product_node_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1243 2023-10-25 11:36:03.000000 m9s_nereid_catalog_tree-7.0.0/view/tree_node_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      208 2020-01-11 16:44:15.000000 m9s_nereid_catalog_tree-7.0.0/view/tree_node_list.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      295 2020-01-11 16:44:15.000000 m9s_nereid_catalog_tree-7.0.0/view/tree_node_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      598 2020-01-11 16:44:15.000000 m9s_nereid_catalog_tree-7.0.0/view/website_view_form.xml
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:12:34.401436 m9s_nereid_catalog_tree-7.0.1/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       89 2024-04-25 09:39:28.000000 m9s_nereid_catalog_tree-7.0.1/.coveragerc
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-13 19:22:51.000000 m9s_nereid_catalog_tree-7.0.1/.drone.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-04-25 09:39:28.000000 m9s_nereid_catalog_tree-7.0.1/.flake8
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-04-25 09:39:28.000000 m9s_nereid_catalog_tree-7.0.1/.gitlab-ci-m9s.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2217 2024-04-25 09:39:28.000000 m9s_nereid_catalog_tree-7.0.1/.gitlab-ci.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2024-04-25 09:39:28.000000 m9s_nereid_catalog_tree-7.0.1/.isort.cfg
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      310 2018-02-28 18:26:33.000000 m9s_nereid_catalog_tree-7.0.1/.travis.yml
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:12:34.401436 m9s_nereid_catalog_tree-7.0.1/.woodpecker/
+-rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2024-04-25 09:39:28.000000 m9s_nereid_catalog_tree-7.0.1/.woodpecker/mail_curl.sh
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2024-04-25 09:39:28.000000 m9s_nereid_catalog_tree-7.0.1/.woodpecker/report.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2024-04-25 09:39:28.000000 m9s_nereid_catalog_tree-7.0.1/.woodpecker/test.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      135 2018-02-28 18:26:33.000000 m9s_nereid_catalog_tree-7.0.1/CHANGELOG.rst
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      798 2024-04-25 09:39:28.000000 m9s_nereid_catalog_tree-7.0.1/COPYRIGHT
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2024-04-25 09:39:28.000000 m9s_nereid_catalog_tree-7.0.1/INSTALL
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2024-04-25 09:39:28.000000 m9s_nereid_catalog_tree-7.0.1/LICENSE
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2024-04-25 09:39:28.000000 m9s_nereid_catalog_tree-7.0.1/MANIFEST.in
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3276 2024-04-25 14:12:34.401436 m9s_nereid_catalog_tree-7.0.1/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1082 2024-04-25 09:39:28.000000 m9s_nereid_catalog_tree-7.0.1/README.md
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       54 2024-04-25 09:39:28.000000 m9s_nereid_catalog_tree-7.0.1/README.rst
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      410 2024-04-25 09:39:28.000000 m9s_nereid_catalog_tree-7.0.1/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6192 2018-05-20 21:10:01.000000 m9s_nereid_catalog_tree-7.0.1/de.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       86 2024-04-25 09:39:28.000000 m9s_nereid_catalog_tree-7.0.1/dev_requirements.txt
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:12:34.401436 m9s_nereid_catalog_tree-7.0.1/doc/
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:12:34.401436 m9s_nereid_catalog_tree-7.0.1/doc/de/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       53 2024-04-25 09:39:28.000000 m9s_nereid_catalog_tree-7.0.1/doc/de/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       54 2024-04-25 09:39:28.000000 m9s_nereid_catalog_tree-7.0.1/doc/index.rst
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:12:34.397436 m9s_nereid_catalog_tree-7.0.1/locale/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6267 2023-10-25 11:36:03.000000 m9s_nereid_catalog_tree-7.0.1/locale/de.po
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:12:34.401436 m9s_nereid_catalog_tree-7.0.1/m9s_nereid_catalog_tree.egg-info/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3276 2024-04-25 14:12:34.000000 m9s_nereid_catalog_tree-7.0.1/m9s_nereid_catalog_tree.egg-info/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1213 2024-04-25 14:12:34.000000 m9s_nereid_catalog_tree-7.0.1/m9s_nereid_catalog_tree.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-04-25 14:12:34.000000 m9s_nereid_catalog_tree-7.0.1/m9s_nereid_catalog_tree.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       76 2024-04-25 14:12:34.000000 m9s_nereid_catalog_tree-7.0.1/m9s_nereid_catalog_tree.egg-info/entry_points.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2020-01-11 14:42:36.000000 m9s_nereid_catalog_tree-7.0.1/m9s_nereid_catalog_tree.egg-info/not-zip-safe
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       69 2024-04-25 14:12:34.000000 m9s_nereid_catalog_tree-7.0.1/m9s_nereid_catalog_tree.egg-info/requires.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-04-25 14:12:34.000000 m9s_nereid_catalog_tree-7.0.1/m9s_nereid_catalog_tree.egg-info/top_level.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2024-04-25 09:39:28.000000 m9s_nereid_catalog_tree-7.0.1/requirements.txt
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-04-25 14:12:34.401436 m9s_nereid_catalog_tree-7.0.1/setup.cfg
+-rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     4500 2024-04-25 09:39:28.000000 m9s_nereid_catalog_tree-7.0.1/setup.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:12:34.401436 m9s_nereid_catalog_tree-7.0.1/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      115 2024-04-25 09:39:28.000000 m9s_nereid_catalog_tree-7.0.1/tests/__init__.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    28906 2024-04-25 09:39:28.000000 m9s_nereid_catalog_tree-7.0.1/tests/test_module.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2024-04-25 09:39:28.000000 m9s_nereid_catalog_tree-7.0.1/tox.ini
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    11844 2024-04-25 09:34:17.000000 m9s_nereid_catalog_tree-7.0.1/tree.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5712 2024-02-05 10:37:45.000000 m9s_nereid_catalog_tree-7.0.1/tree.xml
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      104 2024-04-25 09:39:28.000000 m9s_nereid_catalog_tree-7.0.1/tryton.cfg
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:12:34.401436 m9s_nereid_catalog_tree-7.0.1/view/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      401 2020-01-11 16:44:15.000000 m9s_nereid_catalog_tree-7.0.1/view/product_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      254 2022-02-15 17:51:35.000000 m9s_nereid_catalog_tree-7.0.1/view/product_node_list.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      228 2022-02-15 17:52:56.000000 m9s_nereid_catalog_tree-7.0.1/view/product_node_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1243 2023-10-25 11:36:03.000000 m9s_nereid_catalog_tree-7.0.1/view/tree_node_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      208 2020-01-11 16:44:15.000000 m9s_nereid_catalog_tree-7.0.1/view/tree_node_list.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      295 2020-01-11 16:44:15.000000 m9s_nereid_catalog_tree-7.0.1/view/tree_node_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      598 2020-01-11 16:44:15.000000 m9s_nereid_catalog_tree-7.0.1/view/website_view_form.xml
```

### Comparing `m9s_nereid_catalog_tree-7.0.0/.drone.yml` & `m9s_nereid_catalog_tree-7.0.1/.drone.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog_tree-7.0.0/.gitlab-ci.yml` & `m9s_nereid_catalog_tree-7.0.1/.gitlab-ci.yml`

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

### Comparing `m9s_nereid_catalog_tree-7.0.0/.woodpecker/mail_curl.sh` & `m9s_nereid_catalog_tree-7.0.1/.woodpecker/mail_curl.sh`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog_tree-7.0.0/.woodpecker/report.yml` & `m9s_nereid_catalog_tree-7.0.1/.woodpecker/report.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog_tree-7.0.0/.woodpecker/test.yml` & `m9s_nereid_catalog_tree-7.0.1/.woodpecker/test.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog_tree-7.0.0/COPYRIGHT` & `m9s_nereid_catalog_tree-7.0.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog_tree-7.0.0/INSTALL` & `m9s_nereid_catalog_tree-7.0.1/INSTALL`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog_tree-7.0.0/LICENSE` & `m9s_nereid_catalog_tree-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog_tree-7.0.0/PKG-INFO` & `m9s_nereid_catalog_tree-7.0.1/m9s_nereid_catalog_tree.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: m9s_nereid_catalog_tree
-Version: 7.0.0
+Name: m9s-nereid-catalog-tree
+Version: 7.0.1
 Summary: Tryton Nereid Catalog Tree Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/nereid_catalog_tree.git
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
-[![Pipeline status](https://gitlab.com/m9s/nereid_catalog_tree/badges/master/pipeline.svg)](https://gitlab.com/m9s/nereid_catalog_tree/commits/master)
-
-Develop
-
-[![Pipeline status](https://gitlab.com/m9s/nereid_catalog_tree/badges/develop/pipeline.svg)](https://gitlab.com/m9s/nereid_catalog_tree/commits/develop)
-
-[![Coverage report](https://gitlab.com/m9s/nereid_catalog_tree/badges/develop/coverage.svg)](http://m9s.gitlab.io/nereid_catalog_tree)
-
+[![Tests Status](https://m9s.gitlab.io/nereid_catalog_tree/junit/junit-badge.svg)](https://m9s.gitlab.io/nereid_catalog_tree)
 
+[![Coverage Status](https://m9s.gitlab.io/nereid_catalog_tree/coverage/coverage-badge.svg)](https://m9s.gitlab.io/nereid_catalog_tree)
 
 This module runs with the Tryton application platform.
 
 Installing
 ----------
 
 See INSTALL
```

### Comparing `m9s_nereid_catalog_tree-7.0.0/README.md` & `m9s_nereid_catalog_tree-7.0.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,10 @@
-Master
-
-[![Pipeline status](https://gitlab.com/m9s/nereid_catalog_tree/badges/master/pipeline.svg)](https://gitlab.com/m9s/nereid_catalog_tree/commits/master)
-
-Develop
-
-[![Pipeline status](https://gitlab.com/m9s/nereid_catalog_tree/badges/develop/pipeline.svg)](https://gitlab.com/m9s/nereid_catalog_tree/commits/develop)
-
-[![Coverage report](https://gitlab.com/m9s/nereid_catalog_tree/badges/develop/coverage.svg)](http://m9s.gitlab.io/nereid_catalog_tree)
-
+[![Tests Status](https://m9s.gitlab.io/nereid_catalog_tree/junit/junit-badge.svg)](https://m9s.gitlab.io/nereid_catalog_tree)
 
+[![Coverage Status](https://m9s.gitlab.io/nereid_catalog_tree/coverage/coverage-badge.svg)](https://m9s.gitlab.io/nereid_catalog_tree)
 
 This module runs with the Tryton application platform.
 
 Installing
 ----------
 
 See INSTALL
```

### Comparing `m9s_nereid_catalog_tree-7.0.0/de.po` & `m9s_nereid_catalog_tree-7.0.1/de.po`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog_tree-7.0.0/locale/de.po` & `m9s_nereid_catalog_tree-7.0.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog_tree-7.0.0/m9s_nereid_catalog_tree.egg-info/PKG-INFO` & `m9s_nereid_catalog_tree-7.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: m9s-nereid-catalog-tree
-Version: 7.0.0
+Name: m9s_nereid_catalog_tree
+Version: 7.0.1
 Summary: Tryton Nereid Catalog Tree Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/nereid_catalog_tree.git
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
-[![Pipeline status](https://gitlab.com/m9s/nereid_catalog_tree/badges/master/pipeline.svg)](https://gitlab.com/m9s/nereid_catalog_tree/commits/master)
-
-Develop
-
-[![Pipeline status](https://gitlab.com/m9s/nereid_catalog_tree/badges/develop/pipeline.svg)](https://gitlab.com/m9s/nereid_catalog_tree/commits/develop)
-
-[![Coverage report](https://gitlab.com/m9s/nereid_catalog_tree/badges/develop/coverage.svg)](http://m9s.gitlab.io/nereid_catalog_tree)
-
+[![Tests Status](https://m9s.gitlab.io/nereid_catalog_tree/junit/junit-badge.svg)](https://m9s.gitlab.io/nereid_catalog_tree)
 
+[![Coverage Status](https://m9s.gitlab.io/nereid_catalog_tree/coverage/coverage-badge.svg)](https://m9s.gitlab.io/nereid_catalog_tree)
 
 This module runs with the Tryton application platform.
 
 Installing
 ----------
 
 See INSTALL
```

### Comparing `m9s_nereid_catalog_tree-7.0.0/m9s_nereid_catalog_tree.egg-info/SOURCES.txt` & `m9s_nereid_catalog_tree-7.0.1/m9s_nereid_catalog_tree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog_tree-7.0.0/setup.py` & `m9s_nereid_catalog_tree-7.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog_tree-7.0.0/tests/test_module.py` & `m9s_nereid_catalog_tree-7.0.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog_tree-7.0.0/tox.ini` & `m9s_nereid_catalog_tree-7.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog_tree-7.0.0/tree.py` & `m9s_nereid_catalog_tree-7.0.1/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # The COPYRIGHT file at the top level of this repository contains the full
 # copyright notices and license terms.
 from sql import Literal
 from werkzeug.exceptions import NotFound
 
-from trytond.exceptions import UserError
 from trytond.model import (
-    DeactivableMixin, ModelSQL, ModelView, fields, sequence_ordered, tree)
+    DeactivableMixin, Index, ModelSQL, ModelView, fields, sequence_ordered,
+    tree)
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Eval
 
 from nereid import abort, render_template, request, route, url_for
 from nereid.contrib.pagination import QueryPagination
 from nereid.contrib.sitemap import SitemapIndex, SitemapSection
 from nereid.helpers import context_processor, slugify
@@ -72,14 +72,25 @@
     display = fields.Selection([
             ('product.product', 'Product Variants'),
             ('product.template', 'Product Templates'),
             ('product.tree_node', 'Sub Collections'),
             ], 'Display', required=True)
     template = fields.Selection('get_template', 'Template', required=True)
 
+    @classmethod
+    def __setup__(cls):
+        super().__setup__()
+        t = cls.__table__()
+        cls._sql_indexes.update({
+                Index(t, (t.slug, Index.Similarity())),
+                Index(t,
+                    (t.left, Index.Range()),
+                    (t.right, Index.Range())),
+                })
+
     # parent for rec_name needed
     @fields.depends('name', 'slug', 'parent', '_parent_parent.id')
     def on_change_with_slug(self):
         """
         On change the name and slug, ensure that the slug field is auto
         filled with a generated slug, if the field is empty
         """
```

### Comparing `m9s_nereid_catalog_tree-7.0.0/tree.xml` & `m9s_nereid_catalog_tree-7.0.1/tree.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog_tree-7.0.0/view/tree_node_form.xml` & `m9s_nereid_catalog_tree-7.0.1/view/tree_node_form.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_catalog_tree-7.0.0/view/website_view_form.xml` & `m9s_nereid_catalog_tree-7.0.1/view/website_view_form.xml`

 * *Files identical despite different names*


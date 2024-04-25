# Comparing `tmp/jaraco.mongodb-9.4.tar.gz` & `tmp/jaraco.mongodb-9.4b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmp6_wy_iy2/jaraco.mongodb-9.4.tar", last modified: Fri Dec 14 17:05:52 2018, max compression
+gzip compressed data, was "/tmp/tmp2slm8vw_/jaraco.mongodb-9.4b5.tar", last modified: Thu Dec 13 00:15:54 2018, max compression
```

## Comparing `jaraco.mongodb-9.4.tar` & `jaraco.mongodb-9.4b5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-12-14 17:05:52.000000 jaraco.mongodb-9.4/
--rw-rw-r--   0 travis    (2000) travis    (2000)      284 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/.flake8
--rw-rw-r--   0 travis    (2000) travis    (2000)       74 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/.readthedocs.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1662 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     9461 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/CHANGES.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1050 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     9459 2018-12-14 17:05:52.000000 jaraco.mongodb-9.4/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     7409 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      454 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/appveyor.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      507 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/conftest.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-12-14 17:05:52.000000 jaraco.mongodb-9.4/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      620 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       81 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/docs/history.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1272 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      339 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/install-pip-master.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-12-14 17:05:52.000000 jaraco.mongodb-9.4/jaraco/
--rw-rw-r--   0 travis    (2000) travis    (2000)       56 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-12-14 17:05:52.000000 jaraco.mongodb-9.4/jaraco/mongodb/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1530 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/check-gridfs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      622 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1373 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/compat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      739 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/fields.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      825 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/fixtures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1877 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/helper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      584 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/insert-doc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1032 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/manage.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3701 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/migration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      813 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/monitor-index-creation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3420 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/move-gridfs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15940 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/oplog.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      714 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/pmxbot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1785 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/query.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1870 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/repair-gridfs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7679 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/service.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5609 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/sessions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1647 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/sharding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1750 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/testing.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-12-14 17:05:52.000000 jaraco.mongodb-9.4/jaraco/mongodb/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1094 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/tests/test_compat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      346 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/tests/test_fields.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      490 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/tests/test_insert_doc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      416 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/tests/test_manage.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2681 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/tests/test_oplog.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      757 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/tests/test_service.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2365 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/tests/test_sessions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1782 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/tests/test_testing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      554 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/timers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      558 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/jaraco/mongodb/uri.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-12-14 17:05:52.000000 jaraco.mongodb-9.4/jaraco.mongodb.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9459 2018-12-14 17:05:51.000000 jaraco.mongodb-9.4/jaraco.mongodb.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1411 2018-12-14 17:05:51.000000 jaraco.mongodb-9.4/jaraco.mongodb.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-12-14 17:05:51.000000 jaraco.mongodb-9.4/jaraco.mongodb.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      113 2018-12-14 17:05:51.000000 jaraco.mongodb-9.4/jaraco.mongodb.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2018-12-14 17:05:51.000000 jaraco.mongodb-9.4/jaraco.mongodb.egg-info/namespace_packages.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      339 2018-12-14 17:05:51.000000 jaraco.mongodb-9.4/jaraco.mongodb.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2018-12-14 17:05:51.000000 jaraco.mongodb-9.4/jaraco.mongodb.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      120 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)      339 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/pytest.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)     1286 2018-12-14 17:05:52.000000 jaraco.mongodb-9.4/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      178 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-12-14 17:05:52.000000 jaraco.mongodb-9.4/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9076 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/tests/oplog.js
--rw-rw-r--   0 travis    (2000) travis    (2000)      741 2018-12-14 17:05:17.000000 jaraco.mongodb-9.4/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-12-13 00:15:54.000000 jaraco.mongodb-9.4b5/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      284 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/.flake8
+-rw-rw-r--   0 travis    (2000) travis    (2000)       74 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/.readthedocs.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1612 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/.travis.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9420 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/CHANGES.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1050 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9461 2018-12-13 00:15:54.000000 jaraco.mongodb-9.4b5/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7409 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      454 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/appveyor.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      507 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/conftest.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-12-13 00:15:54.000000 jaraco.mongodb-9.4b5/docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      620 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/docs/conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       81 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/docs/history.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1272 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/docs/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      339 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/install-pip-master.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-12-13 00:15:54.000000 jaraco.mongodb-9.4b5/jaraco/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       56 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-12-13 00:15:54.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1530 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/check-gridfs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      622 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1373 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/compat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      739 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/fields.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      825 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/fixtures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1877 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/helper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      584 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/insert-doc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1032 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/manage.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3701 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/migration.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      813 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/monitor-index-creation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3420 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/move-gridfs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15940 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/oplog.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      714 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/pmxbot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1785 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/query.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1870 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/repair-gridfs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7679 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/service.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5609 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/sessions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1599 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/sharding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1750 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/testing.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-12-13 00:15:54.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1094 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/tests/test_compat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      346 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/tests/test_fields.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      490 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/tests/test_insert_doc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      416 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/tests/test_manage.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2681 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/tests/test_oplog.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      757 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/tests/test_service.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2365 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/tests/test_sessions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1782 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/tests/test_testing.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      554 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/timers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      558 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/jaraco/mongodb/uri.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-12-13 00:15:54.000000 jaraco.mongodb-9.4b5/jaraco.mongodb.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9461 2018-12-13 00:15:54.000000 jaraco.mongodb-9.4b5/jaraco.mongodb.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1411 2018-12-13 00:15:54.000000 jaraco.mongodb-9.4b5/jaraco.mongodb.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-12-13 00:15:54.000000 jaraco.mongodb-9.4b5/jaraco.mongodb.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      113 2018-12-13 00:15:54.000000 jaraco.mongodb-9.4b5/jaraco.mongodb.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        7 2018-12-13 00:15:54.000000 jaraco.mongodb-9.4b5/jaraco.mongodb.egg-info/namespace_packages.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      339 2018-12-13 00:15:54.000000 jaraco.mongodb-9.4b5/jaraco.mongodb.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        7 2018-12-13 00:15:54.000000 jaraco.mongodb-9.4b5/jaraco.mongodb.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      120 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      339 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/pytest.ini
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1286 2018-12-13 00:15:54.000000 jaraco.mongodb-9.4b5/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      178 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-12-13 00:15:54.000000 jaraco.mongodb-9.4b5/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9076 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/tests/oplog.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)      741 2018-12-13 00:15:24.000000 jaraco.mongodb-9.4b5/tox.ini
```

### Comparing `jaraco.mongodb-9.4/.travis.yml` & `jaraco.mongodb-9.4b5/.travis.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 dist: xenial
 sudo: false
 language: python
 
 env:
-- MONGODB_VERSION=3.4
-- MONGODB_VERSION=3.6
 - MONGODB_VERSION=4.0
 python:
-- 2.7
 - 3.5
 - &latest_py3 3.7
 
 jobs:
   fast_finish: true
   include:
   - stage: deploy
```

### Comparing `jaraco.mongodb-9.4/CHANGES.rst` & `jaraco.mongodb-9.4b5/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 9.4
 ===
 
-``create_database_in_shard`` now also reports the 'nodes'
-on which the database was created.
+Update project metadata, now building using pep517.
 
 9.3
 ===
 
 Added ``testing.assert_index_used`` function.
 
 9.2.1
```

### Comparing `jaraco.mongodb-9.4/LICENSE` & `jaraco.mongodb-9.4b5/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/PKG-INFO` & `jaraco.mongodb-9.4b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.mongodb
-Version: 9.4
+Version: 9.4b5
 Summary: Routines and classes supporting MongoDB environments
 Home-page: https://github.com/jaraco/jaraco.mongodb
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 License: UNKNOWN
 Description: .. image:: https://img.shields.io/pypi/v/jaraco.mongodb.svg
            :target: https://pypi.org/project/jaraco.mongodb
@@ -187,9 +187,9 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Pytest
 Requires-Python: >=2.7,!=3.0,!=3.1,!=3.2
-Provides-Extra: testing
 Provides-Extra: docs
+Provides-Extra: testing
```

### Comparing `jaraco.mongodb-9.4/README.rst` & `jaraco.mongodb-9.4b5/README.rst`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/docs/conf.py` & `jaraco.mongodb-9.4b5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/docs/index.rst` & `jaraco.mongodb-9.4b5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/check-gridfs.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/check-gridfs.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/cli.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/cli.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/compat.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/compat.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/fields.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/fields.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/fixtures.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/fixtures.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/helper.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/helper.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/insert-doc.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/insert-doc.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/manage.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/manage.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/migration.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/migration.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/monitor-index-creation.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/monitor-index-creation.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/move-gridfs.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/move-gridfs.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/oplog.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/oplog.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/pmxbot.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/pmxbot.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/query.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/query.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/repair-gridfs.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/repair-gridfs.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/service.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/service.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/sessions.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/sessions.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/sharding.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/sharding.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,10 +33,8 @@
                 raise ValueError("database has collections")
         primary = client['config'].databases.find_one(db_name)['primary']
         if primary != shard:
                 res = client.admin.command(
                     'movePrimary', value=db_name, to=shard)
                 if not res.get('ok'):
                         raise RuntimeError(str(res))
-        return nf(
-            "Successfully created {db_name} in {shard} via {client.nodes} "
-            "from {hostname}")
+        return nf("Successfully created {db_name} in {shard} via {hostname}")
```

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/testing.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/testing.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/tests/test_compat.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/tests/test_oplog.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/tests/test_oplog.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/tests/test_service.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/tests/test_sessions.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/tests/test_testing.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/timers.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/timers.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco/mongodb/uri.py` & `jaraco.mongodb-9.4b5/jaraco/mongodb/uri.py`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/jaraco.mongodb.egg-info/PKG-INFO` & `jaraco.mongodb-9.4b5/jaraco.mongodb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.mongodb
-Version: 9.4
+Version: 9.4b5
 Summary: Routines and classes supporting MongoDB environments
 Home-page: https://github.com/jaraco/jaraco.mongodb
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 License: UNKNOWN
 Description: .. image:: https://img.shields.io/pypi/v/jaraco.mongodb.svg
            :target: https://pypi.org/project/jaraco.mongodb
@@ -187,9 +187,9 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Pytest
 Requires-Python: >=2.7,!=3.0,!=3.1,!=3.2
-Provides-Extra: testing
 Provides-Extra: docs
+Provides-Extra: testing
```

### Comparing `jaraco.mongodb-9.4/jaraco.mongodb.egg-info/SOURCES.txt` & `jaraco.mongodb-9.4b5/jaraco.mongodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/setup.cfg` & `jaraco.mongodb-9.4b5/setup.cfg`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/tests/oplog.js` & `jaraco.mongodb-9.4b5/tests/oplog.js`

 * *Files identical despite different names*

### Comparing `jaraco.mongodb-9.4/tox.ini` & `jaraco.mongodb-9.4b5/tox.ini`

 * *Files identical despite different names*


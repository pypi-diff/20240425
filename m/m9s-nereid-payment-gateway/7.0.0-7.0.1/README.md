# Comparing `tmp/m9s_nereid_payment_gateway-7.0.0.tar.gz` & `tmp/m9s_nereid_payment_gateway-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m9s_nereid_payment_gateway-7.0.0.tar", last modified: Sat Feb  3 20:09:08 2024, max compression
+gzip compressed data, was "m9s_nereid_payment_gateway-7.0.1.tar", last modified: Thu Apr 25 14:16:24 2024, max compression
```

## Comparing `m9s_nereid_payment_gateway-7.0.0.tar` & `m9s_nereid_payment_gateway-7.0.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-03 20:09:08.529405 m9s_nereid_payment_gateway-7.0.0/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-01-22 10:56:08.000000 m9s_nereid_payment_gateway-7.0.0/.coveragerc
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-13 19:22:52.000000 m9s_nereid_payment_gateway-7.0.0/.drone.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-01-22 10:56:08.000000 m9s_nereid_payment_gateway-7.0.0/.flake8
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-01-22 10:56:08.000000 m9s_nereid_payment_gateway-7.0.0/.gitlab-ci-m9s.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1905 2024-01-22 10:56:08.000000 m9s_nereid_payment_gateway-7.0.0/.gitlab-ci.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2024-01-22 10:56:08.000000 m9s_nereid_payment_gateway-7.0.0/.isort.cfg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      206 2021-01-25 09:35:16.000000 m9s_nereid_payment_gateway-7.0.0/.travis.yml
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-03 20:09:08.525406 m9s_nereid_payment_gateway-7.0.0/.woodpecker/
--rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2024-01-22 10:56:08.000000 m9s_nereid_payment_gateway-7.0.0/.woodpecker/mail_curl.sh
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2024-01-22 10:56:08.000000 m9s_nereid_payment_gateway-7.0.0/.woodpecker/report.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2024-01-22 10:56:08.000000 m9s_nereid_payment_gateway-7.0.0/.woodpecker/test.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      798 2024-01-22 10:56:08.000000 m9s_nereid_payment_gateway-7.0.0/COPYRIGHT
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2024-01-22 10:56:08.000000 m9s_nereid_payment_gateway-7.0.0/INSTALL
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2024-01-22 10:56:08.000000 m9s_nereid_payment_gateway-7.0.0/LICENSE
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2024-01-22 10:56:08.000000 m9s_nereid_payment_gateway-7.0.0/MANIFEST.in
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3507 2024-02-03 20:09:08.529405 m9s_nereid_payment_gateway-7.0.0/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1301 2024-01-22 10:56:08.000000 m9s_nereid_payment_gateway-7.0.0/README.md
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       60 2024-01-22 10:56:08.000000 m9s_nereid_payment_gateway-7.0.0/README.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      367 2024-01-22 10:56:08.000000 m9s_nereid_payment_gateway-7.0.0/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-01-22 10:56:08.000000 m9s_nereid_payment_gateway-7.0.0/dev_requirements.txt
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-03 20:09:08.525406 m9s_nereid_payment_gateway-7.0.0/doc/
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-03 20:09:08.529405 m9s_nereid_payment_gateway-7.0.0/doc/de/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       59 2024-01-22 10:56:08.000000 m9s_nereid_payment_gateway-7.0.0/doc/de/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       60 2024-01-22 10:56:08.000000 m9s_nereid_payment_gateway-7.0.0/doc/index.rst
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-03 20:09:08.525406 m9s_nereid_payment_gateway-7.0.0/locale/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2292 2022-04-11 08:20:32.000000 m9s_nereid_payment_gateway-7.0.0/locale/de.po
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-03 20:09:08.529405 m9s_nereid_payment_gateway-7.0.0/m9s_nereid_payment_gateway.egg-info/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3507 2024-02-03 20:09:08.000000 m9s_nereid_payment_gateway-7.0.0/m9s_nereid_payment_gateway.egg-info/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      938 2024-02-03 20:09:08.000000 m9s_nereid_payment_gateway-7.0.0/m9s_nereid_payment_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-02-03 20:09:08.000000 m9s_nereid_payment_gateway-7.0.0/m9s_nereid_payment_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       82 2024-02-03 20:09:08.000000 m9s_nereid_payment_gateway-7.0.0/m9s_nereid_payment_gateway.egg-info/entry_points.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2021-03-02 23:35:17.000000 m9s_nereid_payment_gateway-7.0.0/m9s_nereid_payment_gateway.egg-info/not-zip-safe
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       96 2024-02-03 20:09:08.000000 m9s_nereid_payment_gateway-7.0.0/m9s_nereid_payment_gateway.egg-info/requires.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-02-03 20:09:08.000000 m9s_nereid_payment_gateway-7.0.0/m9s_nereid_payment_gateway.egg-info/top_level.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5846 2024-01-22 10:56:08.000000 m9s_nereid_payment_gateway-7.0.0/party.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2024-01-22 10:56:08.000000 m9s_nereid_payment_gateway-7.0.0/requirements.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       89 2024-02-03 20:09:08.529405 m9s_nereid_payment_gateway-7.0.0/setup.cfg
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4557 2024-02-03 19:21:19.000000 m9s_nereid_payment_gateway-7.0.0/setup.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-03 20:09:08.525406 m9s_nereid_payment_gateway-7.0.0/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      115 2024-01-22 10:56:08.000000 m9s_nereid_payment_gateway-7.0.0/tests/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      322 2024-01-22 10:56:08.000000 m9s_nereid_payment_gateway-7.0.0/tests/test_module.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2024-01-22 10:56:08.000000 m9s_nereid_payment_gateway-7.0.0/tox.ini
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       89 2024-02-03 19:10:06.000000 m9s_nereid_payment_gateway-7.0.0/tryton.cfg
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-03 20:09:08.525406 m9s_nereid_payment_gateway-7.0.0/view/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      860 2021-01-25 09:35:16.000000 m9s_nereid_payment_gateway-7.0.0/view/website_view.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1006 2024-02-03 20:08:52.000000 m9s_nereid_payment_gateway-7.0.0/website.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      454 2024-02-03 20:04:13.000000 m9s_nereid_payment_gateway-7.0.0/website.xml
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:16:24.291978 m9s_nereid_payment_gateway-7.0.1/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-04-25 09:39:28.000000 m9s_nereid_payment_gateway-7.0.1/.coveragerc
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-13 19:22:52.000000 m9s_nereid_payment_gateway-7.0.1/.drone.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-04-25 09:39:28.000000 m9s_nereid_payment_gateway-7.0.1/.flake8
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-04-25 09:39:28.000000 m9s_nereid_payment_gateway-7.0.1/.gitlab-ci-m9s.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2217 2024-04-25 09:39:28.000000 m9s_nereid_payment_gateway-7.0.1/.gitlab-ci.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2024-04-25 09:39:28.000000 m9s_nereid_payment_gateway-7.0.1/.isort.cfg
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      206 2021-01-25 09:35:16.000000 m9s_nereid_payment_gateway-7.0.1/.travis.yml
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:16:24.287978 m9s_nereid_payment_gateway-7.0.1/.woodpecker/
+-rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2024-04-25 09:39:28.000000 m9s_nereid_payment_gateway-7.0.1/.woodpecker/mail_curl.sh
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2024-04-25 09:39:28.000000 m9s_nereid_payment_gateway-7.0.1/.woodpecker/report.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2024-04-25 09:39:28.000000 m9s_nereid_payment_gateway-7.0.1/.woodpecker/test.yml
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      798 2024-04-25 09:39:28.000000 m9s_nereid_payment_gateway-7.0.1/COPYRIGHT
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2024-04-25 09:39:28.000000 m9s_nereid_payment_gateway-7.0.1/INSTALL
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2024-04-25 09:39:28.000000 m9s_nereid_payment_gateway-7.0.1/LICENSE
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2024-04-25 09:39:28.000000 m9s_nereid_payment_gateway-7.0.1/MANIFEST.in
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3303 2024-04-25 14:16:24.291978 m9s_nereid_payment_gateway-7.0.1/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1097 2024-04-25 09:39:28.000000 m9s_nereid_payment_gateway-7.0.1/README.md
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       60 2024-04-25 09:39:28.000000 m9s_nereid_payment_gateway-7.0.1/README.rst
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      367 2024-04-25 09:39:28.000000 m9s_nereid_payment_gateway-7.0.1/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       86 2024-04-25 09:39:28.000000 m9s_nereid_payment_gateway-7.0.1/dev_requirements.txt
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:16:24.291978 m9s_nereid_payment_gateway-7.0.1/doc/
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:16:24.291978 m9s_nereid_payment_gateway-7.0.1/doc/de/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       59 2024-04-25 09:39:28.000000 m9s_nereid_payment_gateway-7.0.1/doc/de/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       60 2024-04-25 09:39:28.000000 m9s_nereid_payment_gateway-7.0.1/doc/index.rst
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:16:24.287978 m9s_nereid_payment_gateway-7.0.1/locale/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2292 2022-04-11 08:20:32.000000 m9s_nereid_payment_gateway-7.0.1/locale/de.po
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:16:24.291978 m9s_nereid_payment_gateway-7.0.1/m9s_nereid_payment_gateway.egg-info/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3303 2024-04-25 14:16:24.000000 m9s_nereid_payment_gateway-7.0.1/m9s_nereid_payment_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      938 2024-04-25 14:16:24.000000 m9s_nereid_payment_gateway-7.0.1/m9s_nereid_payment_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-04-25 14:16:24.000000 m9s_nereid_payment_gateway-7.0.1/m9s_nereid_payment_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       82 2024-04-25 14:16:24.000000 m9s_nereid_payment_gateway-7.0.1/m9s_nereid_payment_gateway.egg-info/entry_points.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2021-03-02 23:35:17.000000 m9s_nereid_payment_gateway-7.0.1/m9s_nereid_payment_gateway.egg-info/not-zip-safe
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       96 2024-04-25 14:16:24.000000 m9s_nereid_payment_gateway-7.0.1/m9s_nereid_payment_gateway.egg-info/requires.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-04-25 14:16:24.000000 m9s_nereid_payment_gateway-7.0.1/m9s_nereid_payment_gateway.egg-info/top_level.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5846 2024-01-22 10:56:08.000000 m9s_nereid_payment_gateway-7.0.1/party.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2024-04-25 09:39:28.000000 m9s_nereid_payment_gateway-7.0.1/requirements.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       89 2024-04-25 14:16:24.291978 m9s_nereid_payment_gateway-7.0.1/setup.cfg
+-rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     4557 2024-04-25 09:39:28.000000 m9s_nereid_payment_gateway-7.0.1/setup.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:16:24.287978 m9s_nereid_payment_gateway-7.0.1/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      115 2024-04-25 09:39:28.000000 m9s_nereid_payment_gateway-7.0.1/tests/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      322 2024-04-25 09:39:28.000000 m9s_nereid_payment_gateway-7.0.1/tests/test_module.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2024-04-25 09:39:28.000000 m9s_nereid_payment_gateway-7.0.1/tox.ini
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)       89 2024-04-25 09:39:28.000000 m9s_nereid_payment_gateway-7.0.1/tryton.cfg
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:16:24.287978 m9s_nereid_payment_gateway-7.0.1/view/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      860 2021-01-25 09:35:16.000000 m9s_nereid_payment_gateway-7.0.1/view/website_view.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      932 2024-02-03 20:32:22.000000 m9s_nereid_payment_gateway-7.0.1/website.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      454 2024-02-03 20:04:13.000000 m9s_nereid_payment_gateway-7.0.1/website.xml
```

### Comparing `m9s_nereid_payment_gateway-7.0.0/.drone.yml` & `m9s_nereid_payment_gateway-7.0.1/.drone.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_payment_gateway-7.0.0/.gitlab-ci.yml` & `m9s_nereid_payment_gateway-7.0.1/.gitlab-ci.yml`

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

### Comparing `m9s_nereid_payment_gateway-7.0.0/.woodpecker/mail_curl.sh` & `m9s_nereid_payment_gateway-7.0.1/.woodpecker/mail_curl.sh`

 * *Files identical despite different names*

### Comparing `m9s_nereid_payment_gateway-7.0.0/.woodpecker/report.yml` & `m9s_nereid_payment_gateway-7.0.1/.woodpecker/report.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_payment_gateway-7.0.0/.woodpecker/test.yml` & `m9s_nereid_payment_gateway-7.0.1/.woodpecker/test.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_payment_gateway-7.0.0/COPYRIGHT` & `m9s_nereid_payment_gateway-7.0.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `m9s_nereid_payment_gateway-7.0.0/INSTALL` & `m9s_nereid_payment_gateway-7.0.1/INSTALL`

 * *Files identical despite different names*

### Comparing `m9s_nereid_payment_gateway-7.0.0/LICENSE` & `m9s_nereid_payment_gateway-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `m9s_nereid_payment_gateway-7.0.0/PKG-INFO` & `m9s_nereid_payment_gateway-7.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s_nereid_payment_gateway
-Version: 7.0.0
+Version: 7.0.1
 Summary: Tryton Nereid Payment Gateway Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/nereid_payment_gateway.git
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
-[![Pipeline status](https://gitlab.com/m9s/nereid_payment_gateway/badges/master/pipeline.svg)](https://gitlab.com/m9s/nereid_payment_gateway/commits/master)
-
-Develop
-
-[![Pipeline status](https://gitlab.com/m9s/nereid_payment_gateway/badges/develop/pipeline.svg)](https://gitlab.com/m9s/nereid_payment_gateway/commits/develop)
-
-[![Coverage report](https://gitlab.com/m9s/nereid_payment_gateway/badges/develop/coverage.svg)](http://m9s.gitlab.io/nereid_payment_gateway)
-
+[![Tests Status](https://m9s.gitlab.io/nereid_payment_gateway/junit/junit-badge.svg)](https://m9s.gitlab.io/nereid_payment_gateway)
 
+[![Coverage Status](https://m9s.gitlab.io/nereid_payment_gateway/coverage/coverage-badge.svg)](https://m9s.gitlab.io/nereid_payment_gateway)
 
 This module runs with the Tryton application platform.
 
 Installing
 ----------
 
 See INSTALL
```

### Comparing `m9s_nereid_payment_gateway-7.0.0/README.md` & `m9s_nereid_payment_gateway-7.0.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,10 @@
-Master
-
-[![Pipeline status](https://gitlab.com/m9s/nereid_payment_gateway/badges/master/pipeline.svg)](https://gitlab.com/m9s/nereid_payment_gateway/commits/master)
-
-Develop
-
-[![Pipeline status](https://gitlab.com/m9s/nereid_payment_gateway/badges/develop/pipeline.svg)](https://gitlab.com/m9s/nereid_payment_gateway/commits/develop)
-
-[![Coverage report](https://gitlab.com/m9s/nereid_payment_gateway/badges/develop/coverage.svg)](http://m9s.gitlab.io/nereid_payment_gateway)
-
+[![Tests Status](https://m9s.gitlab.io/nereid_payment_gateway/junit/junit-badge.svg)](https://m9s.gitlab.io/nereid_payment_gateway)
 
+[![Coverage Status](https://m9s.gitlab.io/nereid_payment_gateway/coverage/coverage-badge.svg)](https://m9s.gitlab.io/nereid_payment_gateway)
 
 This module runs with the Tryton application platform.
 
 Installing
 ----------
 
 See INSTALL
```

### Comparing `m9s_nereid_payment_gateway-7.0.0/locale/de.po` & `m9s_nereid_payment_gateway-7.0.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `m9s_nereid_payment_gateway-7.0.0/m9s_nereid_payment_gateway.egg-info/PKG-INFO` & `m9s_nereid_payment_gateway-7.0.1/m9s_nereid_payment_gateway.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s-nereid-payment-gateway
-Version: 7.0.0
+Version: 7.0.1
 Summary: Tryton Nereid Payment Gateway Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/nereid_payment_gateway.git
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
-[![Pipeline status](https://gitlab.com/m9s/nereid_payment_gateway/badges/master/pipeline.svg)](https://gitlab.com/m9s/nereid_payment_gateway/commits/master)
-
-Develop
-
-[![Pipeline status](https://gitlab.com/m9s/nereid_payment_gateway/badges/develop/pipeline.svg)](https://gitlab.com/m9s/nereid_payment_gateway/commits/develop)
-
-[![Coverage report](https://gitlab.com/m9s/nereid_payment_gateway/badges/develop/coverage.svg)](http://m9s.gitlab.io/nereid_payment_gateway)
-
+[![Tests Status](https://m9s.gitlab.io/nereid_payment_gateway/junit/junit-badge.svg)](https://m9s.gitlab.io/nereid_payment_gateway)
 
+[![Coverage Status](https://m9s.gitlab.io/nereid_payment_gateway/coverage/coverage-badge.svg)](https://m9s.gitlab.io/nereid_payment_gateway)
 
 This module runs with the Tryton application platform.
 
 Installing
 ----------
 
 See INSTALL
```

### Comparing `m9s_nereid_payment_gateway-7.0.0/m9s_nereid_payment_gateway.egg-info/SOURCES.txt` & `m9s_nereid_payment_gateway-7.0.1/m9s_nereid_payment_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m9s_nereid_payment_gateway-7.0.0/party.py` & `m9s_nereid_payment_gateway-7.0.1/party.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_payment_gateway-7.0.0/setup.py` & `m9s_nereid_payment_gateway-7.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_payment_gateway-7.0.0/tox.ini` & `m9s_nereid_payment_gateway-7.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `m9s_nereid_payment_gateway-7.0.0/view/website_view.xml` & `m9s_nereid_payment_gateway-7.0.1/view/website_view.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_payment_gateway-7.0.0/website.py` & `m9s_nereid_payment_gateway-7.0.1/website.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,16 @@
     "Define the credit card handler"
     __name__ = 'nereid.website'
 
     accept_credit_card = fields.Boolean('Accept Credit Card')
     save_payment_profile = fields.Boolean(
         'Allow Saving Payment Profiles', states={
             'invisible': ~Bool(Eval('accept_credit_card'))
-        }, depends=['accept_credit_card']
-    )
+        })
     credit_card_gateway = fields.Many2One(
         'payment_gateway.gateway', 'Credit Card Gateway',
         states={
             'required': Bool(Eval('accept_credit_card')),
             'invisible': ~Bool(Eval('accept_credit_card'))
-        }, depends=['accept_credit_card'],
-        domain=[('method', 'in', ['credit_card', 'dummy'])]
-    )
+        },
+        domain=[('method', 'in', ['credit_card', 'dummy'])])
     instructions = fields.Text('Credit Card Instructions', translate=True)
```


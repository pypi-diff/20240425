# Comparing `tmp/rhdzmota-4.0.0.tar.gz` & `tmp/rhdzmota-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhdzmota-4.0.0.tar", last modified: Tue Apr  9 04:44:18 2024, max compression
+gzip compressed data, was "rhdzmota-4.0.1.tar", last modified: Thu Apr 25 06:54:18 2024, max compression
```

## Comparing `rhdzmota-4.0.0.tar` & `rhdzmota-4.0.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:18.550530 rhdzmota-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-09 04:44:18.550530 rhdzmota-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:18.542530 rhdzmota-4.0.0/bin/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/bin/rhdzmota
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 04:44:18.550530 rhdzmota-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:18.542530 rhdzmota-4.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:18.542530 rhdzmota-4.0.0/src/main/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:18.546530 rhdzmota-4.0.0/src/main/rhdzmota/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/celery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:18.546530 rhdzmota-4.0.0/src/main/rhdzmota/celery_workers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/celery_workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/celery_workers/hello.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:18.546530 rhdzmota-4.0.0/src/main/rhdzmota/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/cli/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:18.546530 rhdzmota-4.0.0/src/main/rhdzmota/ext/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/ext/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:18.546530 rhdzmota-4.0.0/src/main/rhdzmota/google_services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/google_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/google_services/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/google_services/gmail.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:18.546530 rhdzmota-4.0.0/src/main/rhdzmota/heartbeat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/heartbeat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/heartbeat/daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/heartbeat/daemon_heart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:18.546530 rhdzmota-4.0.0/src/main/rhdzmota/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/interface/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:18.546530 rhdzmota-4.0.0/src/main/rhdzmota/iso3166/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/iso3166/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/iso3166/country_codes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:18.546530 rhdzmota-4.0.0/src/main/rhdzmota/iso3166/datafiles/
--rw-r--r--   0 runner    (1001) docker     (127)    25179 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/iso3166/datafiles/countries.json
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/iso3166/datafiles/default.json
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/iso3166/datafiles/mx.json
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/iso3166/datafiles/us.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:18.546530 rhdzmota-4.0.0/src/main/rhdzmota/mail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/mail/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/mail/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/mail/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:18.546530 rhdzmota-4.0.0/src/main/rhdzmota/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/utils/gists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/utils/json_web_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/utils/rsa_encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/utils/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/version
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:18.550530 rhdzmota-4.0.0/src/main/rhdzmota/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-09 04:44:03.000000 rhdzmota-4.0.0/src/main/rhdzmota/wrappers/sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:44:18.546530 rhdzmota-4.0.0/src/main/rhdzmota.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-09 04:44:18.000000 rhdzmota-4.0.0/src/main/rhdzmota.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-09 04:44:18.000000 rhdzmota-4.0.0/src/main/rhdzmota.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 04:44:18.000000 rhdzmota-4.0.0/src/main/rhdzmota.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 04:44:18.000000 rhdzmota-4.0.0/src/main/rhdzmota.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-09 04:44:18.000000 rhdzmota-4.0.0/src/main/rhdzmota.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 04:44:18.000000 rhdzmota-4.0.0/src/main/rhdzmota.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:18.479368 rhdzmota-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-25 06:54:18.479368 rhdzmota-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:18.471368 rhdzmota-4.0.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/bin/rhdzmota
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 06:54:18.479368 rhdzmota-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:18.471368 rhdzmota-4.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:18.471368 rhdzmota-4.0.1/src/main/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:18.471368 rhdzmota-4.0.1/src/main/rhdzmota/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/celery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:18.475368 rhdzmota-4.0.1/src/main/rhdzmota/celery_workers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/celery_workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/celery_workers/hello.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:18.475368 rhdzmota-4.0.1/src/main/rhdzmota/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/cli/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:18.475368 rhdzmota-4.0.1/src/main/rhdzmota/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/ext/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:18.475368 rhdzmota-4.0.1/src/main/rhdzmota/google_services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/google_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/google_services/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/google_services/gmail.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:18.475368 rhdzmota-4.0.1/src/main/rhdzmota/heartbeat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/heartbeat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/heartbeat/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/heartbeat/daemon_heart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:18.475368 rhdzmota-4.0.1/src/main/rhdzmota/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/interface/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:18.475368 rhdzmota-4.0.1/src/main/rhdzmota/iso3166/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/iso3166/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/iso3166/country_codes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:18.475368 rhdzmota-4.0.1/src/main/rhdzmota/iso3166/datafiles/
+-rw-r--r--   0 runner    (1001) docker     (127)    25179 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/iso3166/datafiles/countries.json
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/iso3166/datafiles/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/iso3166/datafiles/mx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/iso3166/datafiles/us.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:18.475368 rhdzmota-4.0.1/src/main/rhdzmota/mail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/mail/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/mail/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/mail/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:18.479368 rhdzmota-4.0.1/src/main/rhdzmota/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/utils/gists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/utils/json_web_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/utils/rsa_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/utils/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/version
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:18.479368 rhdzmota-4.0.1/src/main/rhdzmota/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-25 06:54:01.000000 rhdzmota-4.0.1/src/main/rhdzmota/wrappers/sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:54:18.475368 rhdzmota-4.0.1/src/main/rhdzmota.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-25 06:54:18.000000 rhdzmota-4.0.1/src/main/rhdzmota.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-25 06:54:18.000000 rhdzmota-4.0.1/src/main/rhdzmota.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 06:54:18.000000 rhdzmota-4.0.1/src/main/rhdzmota.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-25 06:54:18.000000 rhdzmota-4.0.1/src/main/rhdzmota.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-25 06:54:18.000000 rhdzmota-4.0.1/src/main/rhdzmota.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 06:54:18.000000 rhdzmota-4.0.1/src/main/rhdzmota.egg-info/top_level.txt
```

### Comparing `rhdzmota-4.0.0/PKG-INFO` & `rhdzmota-4.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhdzmota
-Version: 4.0.0
+Version: 4.0.1
 Summary: RHDZMOTA Package
 Home-page: https://github.com/rhdzmota/package.rhdzmota.com
 Author: Rodrigo H. Mota
 Author-email: info@rhdzmota.com
 Requires-Python: >=3.8.10
 Description-Content-Type: text/markdown
 Provides-Extra: baseline
```

### Comparing `rhdzmota-4.0.0/README.md` & `rhdzmota-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/requirements.txt` & `rhdzmota-4.0.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/setup.py` & `rhdzmota-4.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota/celery.py` & `rhdzmota-4.0.1/src/main/rhdzmota/celery.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota/cli/ext.py` & `rhdzmota-4.0.1/src/main/rhdzmota/cli/ext.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota/cli/main.py` & `rhdzmota-4.0.1/src/main/rhdzmota/cli/main.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota/google_services/auth.py` & `rhdzmota-4.0.1/src/main/rhdzmota/google_services/auth.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota/google_services/gmail.py` & `rhdzmota-4.0.1/src/main/rhdzmota/google_services/gmail.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota/heartbeat/daemon.py` & `rhdzmota-4.0.1/src/main/rhdzmota/heartbeat/daemon.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota/heartbeat/daemon_heart.py` & `rhdzmota-4.0.1/src/main/rhdzmota/heartbeat/daemon_heart.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota/interface/cli.py` & `rhdzmota-4.0.1/src/main/rhdzmota/interface/cli.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota/iso3166/country_codes.py` & `rhdzmota-4.0.1/src/main/rhdzmota/iso3166/country_codes.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota/iso3166/datafiles/countries.json` & `rhdzmota-4.0.1/src/main/rhdzmota/iso3166/datafiles/countries.json`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota/iso3166/datafiles/mx.json` & `rhdzmota-4.0.1/src/main/rhdzmota/iso3166/datafiles/mx.json`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota/iso3166/datafiles/us.json` & `rhdzmota-4.0.1/src/main/rhdzmota/iso3166/datafiles/us.json`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota/mail/message.py` & `rhdzmota-4.0.1/src/main/rhdzmota/mail/message.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota/mail/server.py` & `rhdzmota-4.0.1/src/main/rhdzmota/mail/server.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota/settings.py` & `rhdzmota-4.0.1/src/main/rhdzmota/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -139,14 +139,19 @@
                 cls._Singleton.value.get_logger(name=__name__).warning("Creating a new logger manager instance.")
         return cls._Singleton.value
 
 
 logger_manager = LoggerManager.singleton()
 logger = logger_manager.get_logger(name=__name__)
 
+stonebase_install = "pip install 'stonebase[standalone]'"
+logger.warning(
+    f"The RHDZMOTA Package has been deprecated! Use stonebase instead: {stonebase_install}"
+)
+
 # Celery
 
 RHDZMOTA_CELERY_BROKER_HOST = get_environ_variable(
     name="RHDZMOTA_CELERY_BROKER_HOST",
     default="127.0.0.1"
 )
```

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota/utils/gists.py` & `rhdzmota-4.0.1/src/main/rhdzmota/utils/gists.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota/utils/json_web_token.py` & `rhdzmota-4.0.1/src/main/rhdzmota/utils/json_web_token.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota/utils/misc.py` & `rhdzmota-4.0.1/src/main/rhdzmota/utils/misc.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota/utils/rsa_encryption.py` & `rhdzmota-4.0.1/src/main/rhdzmota/utils/rsa_encryption.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota/utils/runtime.py` & `rhdzmota-4.0.1/src/main/rhdzmota/utils/runtime.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota/version.py` & `rhdzmota-4.0.1/src/main/rhdzmota/version.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota/wrappers/sentry.py` & `rhdzmota-4.0.1/src/main/rhdzmota/wrappers/sentry.py`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota.egg-info/PKG-INFO` & `rhdzmota-4.0.1/src/main/rhdzmota.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhdzmota
-Version: 4.0.0
+Version: 4.0.1
 Summary: RHDZMOTA Package
 Home-page: https://github.com/rhdzmota/package.rhdzmota.com
 Author: Rodrigo H. Mota
 Author-email: info@rhdzmota.com
 Requires-Python: >=3.8.10
 Description-Content-Type: text/markdown
 Provides-Extra: baseline
```

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota.egg-info/SOURCES.txt` & `rhdzmota-4.0.1/src/main/rhdzmota.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rhdzmota-4.0.0/src/main/rhdzmota.egg-info/requires.txt` & `rhdzmota-4.0.1/src/main/rhdzmota.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,120 +1,120 @@
 rsa==4.8
-fire==0.4.0
 pyyaml==6.0.1
-psutil==5.9.2
+fire==0.4.0
 requests==2.31.0
+psutil==5.9.2
 
 [all]
-sentry-sdk==1.40.6
-waitress==2.0.0
+Flask==2.0.1
+mypy-extensions==0.4.3
+ipython==7.34.0
 flower==1.2.0
+mypy==0.971
 oauth2client==4.1.3
-pyyaml==6.0.1
-google-auth-oauthlib==0.5.3
-typed-ast==1.5.4
 requests==2.31.0
-google-api-python-client==2.63.0
-Flask==2.0.1
-fire==0.4.0
 psutil==5.9.2
+typed-ast==1.5.4
+sentry-sdk==1.40.6
+waitress==2.0.0
 jupyter==1.0.0
+google-api-python-client==2.63.0
+rhdzmota-extension-streamlit-webapps<1.0.0,>=0.5.1
+fire==0.4.0
+celery[redis]==5.1.2
 rsa==4.8
-scalene==1.3.12
 pycodestyle==2.7.0
+rhdzmota-extension-hello-world<1.0.0,>=0.1.2
 typing_extensions==4.3.0
-mypy-extensions==0.4.3
-ipython==7.34.0
+pyyaml==6.0.1
 PyJWT==2.3.0
-rhdzmota-extension-hello-world<1.0.0,>=0.1.2
-mypy==0.971
-rhdzmota-extension-streamlit-webapps<1.0.0,>=0.5.1
-celery[redis]==5.1.2
+scalene==1.3.12
+google-auth-oauthlib==0.5.3
 
 [backend]
+Flask==2.0.1
+fire==0.4.0
+requests==2.31.0
 rsa==4.8
-waitress==2.0.0
-sentry-sdk==1.40.6
 pyyaml==6.0.1
 PyJWT==2.3.0
-requests==2.31.0
-Flask==2.0.1
-fire==0.4.0
+waitress==2.0.0
 psutil==5.9.2
+sentry-sdk==1.40.6
 
 [baseline]
 rsa==4.8
-fire==0.4.0
 pyyaml==6.0.1
-psutil==5.9.2
+fire==0.4.0
 requests==2.31.0
+psutil==5.9.2
 
 [celery]
-rsa==4.8
-sentry-sdk==1.40.6
 flower==1.2.0
-pyyaml==6.0.1
-requests==2.31.0
 fire==0.4.0
 celery[redis]==5.1.2
+rsa==4.8
+pyyaml==6.0.1
+requests==2.31.0
 psutil==5.9.2
+sentry-sdk==1.40.6
 
 [develop]
+jupyter==1.0.0
+mypy-extensions==0.4.3
+ipython==7.34.0
+typed-ast==1.5.4
+psutil==5.9.2
+fire==0.4.0
 rsa==4.8
-scalene==1.3.12
-sentry-sdk==1.40.6
 pycodestyle==2.7.0
-ipython==7.34.0
 typing_extensions==4.3.0
-mypy-extensions==0.4.3
 pyyaml==6.0.1
-typed-ast==1.5.4
-requests==2.31.0
 mypy==0.971
-fire==0.4.0
-psutil==5.9.2
-jupyter==1.0.0
+requests==2.31.0
+scalene==1.3.12
+sentry-sdk==1.40.6
 
 [ext.hello_world]
-rhdzmota-extension-hello-world<1.0.0,>=0.1.2
 rsa==4.8
-sentry-sdk==1.40.6
-fire==0.4.0
+rhdzmota-extension-hello-world<1.0.0,>=0.1.2
 pyyaml==6.0.1
-psutil==5.9.2
+fire==0.4.0
 requests==2.31.0
+psutil==5.9.2
+sentry-sdk==1.40.6
 
 [ext.streamlit_webapps]
+rhdzmota-extension-streamlit-webapps<1.0.0,>=0.5.1
+fire==0.4.0
 rsa==4.8
 pyyaml==6.0.1
 requests==2.31.0
-rhdzmota-extension-streamlit-webapps<1.0.0,>=0.5.1
-fire==0.4.0
 psutil==5.9.2
 
 [google_services]
-rsa==4.8
 sentry-sdk==1.40.6
-oauth2client==4.1.3
-pyyaml==6.0.1
 google-api-python-client==2.63.0
-requests==2.31.0
 fire==0.4.0
-google-auth-oauthlib==0.5.3
+rsa==4.8
+pyyaml==6.0.1
+oauth2client==4.1.3
+requests==2.31.0
 psutil==5.9.2
+google-auth-oauthlib==0.5.3
 
 [standalone]
 rsa==4.8
-sentry-sdk==1.40.6
-fire==0.4.0
 pyyaml==6.0.1
-psutil==5.9.2
+fire==0.4.0
 requests==2.31.0
+psutil==5.9.2
+sentry-sdk==1.40.6
 
 [tools]
 rsa==4.8
-sentry-sdk==1.40.6
-fire==0.4.0
 pyyaml==6.0.1
-psutil==5.9.2
 PyJWT==2.3.0
+fire==0.4.0
 requests==2.31.0
+psutil==5.9.2
+sentry-sdk==1.40.6
```


# Comparing `tmp/m9s_payment_gateway-7.0.5.tar.gz` & `tmp/m9s_payment_gateway-7.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m9s_payment_gateway-7.0.5.tar", last modified: Fri Feb  2 17:22:59 2024, max compression
+gzip compressed data, was "m9s_payment_gateway-7.0.6.tar", last modified: Thu Apr 25 15:10:01 2024, max compression
```

## Comparing `m9s_payment_gateway-7.0.5.tar` & `m9s_payment_gateway-7.0.6.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-02 17:22:59.951176 m9s_payment_gateway-7.0.5/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       85 2023-12-21 15:13:57.000000 m9s_payment_gateway-7.0.5/.coveragerc
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2023-12-21 15:13:57.000000 m9s_payment_gateway-7.0.5/.flake8
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2023-12-21 15:13:57.000000 m9s_payment_gateway-7.0.5/.gitlab-ci-m9s.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1892 2023-12-21 15:13:57.000000 m9s_payment_gateway-7.0.5/.gitlab-ci.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2023-12-21 15:13:57.000000 m9s_payment_gateway-7.0.5/.isort.cfg
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-02 17:22:59.943176 m9s_payment_gateway-7.0.5/.woodpecker/
--rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2023-12-21 15:13:57.000000 m9s_payment_gateway-7.0.5/.woodpecker/mail_curl.sh
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2023-12-21 15:13:57.000000 m9s_payment_gateway-7.0.5/.woodpecker/report.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2023-12-21 15:13:57.000000 m9s_payment_gateway-7.0.5/.woodpecker/test.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      798 2023-12-21 15:13:57.000000 m9s_payment_gateway-7.0.5/COPYRIGHT
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2023-12-21 15:13:57.000000 m9s_payment_gateway-7.0.5/INSTALL
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2023-12-21 15:13:57.000000 m9s_payment_gateway-7.0.5/LICENSE
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2023-12-21 15:13:57.000000 m9s_payment_gateway-7.0.5/MANIFEST.in
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3430 2024-02-02 17:22:59.951176 m9s_payment_gateway-7.0.5/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1252 2023-12-21 15:13:57.000000 m9s_payment_gateway-7.0.5/README.md
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2023-12-21 15:13:57.000000 m9s_payment_gateway-7.0.5/README.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1125 2023-12-21 15:13:57.000000 m9s_payment_gateway-7.0.5/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2023-12-21 15:13:57.000000 m9s_payment_gateway-7.0.5/dev_requirements.txt
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-02 17:22:59.943176 m9s_payment_gateway-7.0.5/doc/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6818 2018-02-28 18:26:36.000000 m9s_payment_gateway-7.0.5/doc/Makefile
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2093 2018-02-28 18:26:36.000000 m9s_payment_gateway-7.0.5/doc/api_reference.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     9066 2024-01-17 10:54:55.000000 m9s_payment_gateway-7.0.5/doc/conf.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-02 17:22:59.943176 m9s_payment_gateway-7.0.5/doc/de/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       45 2023-12-21 15:13:57.000000 m9s_payment_gateway-7.0.5/doc/de/index.rst
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-02 17:22:59.951176 m9s_payment_gateway-7.0.5/doc/images/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)   302320 2018-02-28 18:26:36.000000 m9s_payment_gateway-7.0.5/doc/images/payment-gateways-add.png
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)   269848 2018-02-28 18:26:36.000000 m9s_payment_gateway-7.0.5/doc/images/payment-gateways.png
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)   363503 2018-02-28 18:26:36.000000 m9s_payment_gateway-7.0.5/doc/images/payment-profile-add.png
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)   308733 2018-02-28 18:26:36.000000 m9s_payment_gateway-7.0.5/doc/images/payment-profiles.png
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)   119650 2018-02-28 18:26:36.000000 m9s_payment_gateway-7.0.5/doc/images/payment-transaction-enter-card.png
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)   247886 2018-02-28 18:26:36.000000 m9s_payment_gateway-7.0.5/doc/images/payment-transaction-use-card.png
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)   259455 2018-02-28 18:26:36.000000 m9s_payment_gateway-7.0.5/doc/images/payment-transaction-using-profile.png
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2023-12-21 15:13:57.000000 m9s_payment_gateway-7.0.5/doc/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5383 2018-02-28 18:26:36.000000 m9s_payment_gateway-7.0.5/doc/introduction.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    20312 2018-02-28 18:26:36.000000 m9s_payment_gateway-7.0.5/doc/write_a_gateway.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4067 2023-12-21 15:13:57.000000 m9s_payment_gateway-7.0.5/dummy.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-02 17:22:59.939176 m9s_payment_gateway-7.0.5/locale/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    19590 2022-11-25 23:13:54.000000 m9s_payment_gateway-7.0.5/locale/de.po
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-02 17:22:59.951176 m9s_payment_gateway-7.0.5/m9s_payment_gateway.egg-info/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3430 2024-02-02 17:22:59.000000 m9s_payment_gateway-7.0.5/m9s_payment_gateway.egg-info/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1974 2024-02-02 17:22:59.000000 m9s_payment_gateway-7.0.5/m9s_payment_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-02-02 17:22:59.000000 m9s_payment_gateway-7.0.5/m9s_payment_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       68 2024-02-02 17:22:59.000000 m9s_payment_gateway-7.0.5/m9s_payment_gateway.egg-info/entry_points.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2021-11-25 00:03:02.000000 m9s_payment_gateway-7.0.5/m9s_payment_gateway.egg-info/not-zip-safe
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      104 2024-02-02 17:22:59.000000 m9s_payment_gateway-7.0.5/m9s_payment_gateway.egg-info/requires.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-02-02 17:22:59.000000 m9s_payment_gateway-7.0.5/m9s_payment_gateway.egg-info/top_level.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2183 2023-12-21 15:13:57.000000 m9s_payment_gateway-7.0.5/manual.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1860 2023-12-26 13:19:11.000000 m9s_payment_gateway-7.0.5/message.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1651 2023-12-21 15:13:57.000000 m9s_payment_gateway-7.0.5/party.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2023-12-21 15:13:57.000000 m9s_payment_gateway-7.0.5/requirements.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      218 2024-02-02 17:22:59.951176 m9s_payment_gateway-7.0.5/setup.cfg
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4454 2024-02-02 17:18:30.000000 m9s_payment_gateway-7.0.5/setup.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-02 17:22:59.939176 m9s_payment_gateway-7.0.5/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      320 2023-12-26 19:57:38.000000 m9s_payment_gateway-7.0.5/tests/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    11142 2024-01-17 10:48:51.000000 m9s_payment_gateway-7.0.5/tests/test_module.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2023-12-21 15:13:57.000000 m9s_payment_gateway-7.0.5/tox.ini
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    38702 2023-12-27 20:01:46.000000 m9s_payment_gateway-7.0.5/transaction.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    19022 2022-11-25 23:13:54.000000 m9s_payment_gateway-7.0.5/transaction.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       95 2024-01-17 10:54:55.000000 m9s_payment_gateway-7.0.5/tryton.cfg
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-02-02 17:22:59.939176 m9s_payment_gateway-7.0.5/view/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      834 2020-01-14 23:15:35.000000 m9s_payment_gateway-7.0.5/view/gateway_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      292 2020-01-14 23:15:35.000000 m9s_payment_gateway-7.0.5/view/gateway_list.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      567 2020-01-14 23:15:35.000000 m9s_payment_gateway-7.0.5/view/party_payment_profile_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      727 2020-01-14 23:15:35.000000 m9s_payment_gateway-7.0.5/view/payment_profile_add_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1009 2020-01-14 23:15:35.000000 m9s_payment_gateway-7.0.5/view/payment_profile_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      391 2020-01-14 23:15:35.000000 m9s_payment_gateway-7.0.5/view/payment_profile_list.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3086 2021-05-12 07:36:45.000000 m9s_payment_gateway-7.0.5/view/transaction_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      367 2020-01-14 23:15:35.000000 m9s_payment_gateway-7.0.5/view/transaction_list.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      461 2021-05-12 07:36:45.000000 m9s_payment_gateway-7.0.5/view/transaction_log_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      296 2021-05-12 07:36:45.000000 m9s_payment_gateway-7.0.5/view/transaction_log_list.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      987 2020-01-14 23:15:35.000000 m9s_payment_gateway-7.0.5/view/transaction_use_card_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      362 2020-01-14 23:15:35.000000 m9s_payment_gateway-7.0.5/view/user_form.xml
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 15:10:01.203488 m9s_payment_gateway-7.0.6/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       85 2024-04-25 09:53:46.000000 m9s_payment_gateway-7.0.6/.coveragerc
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-04-25 09:53:46.000000 m9s_payment_gateway-7.0.6/.flake8
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-04-25 09:53:46.000000 m9s_payment_gateway-7.0.6/.gitlab-ci-m9s.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2204 2024-04-25 09:53:46.000000 m9s_payment_gateway-7.0.6/.gitlab-ci.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2024-04-25 09:53:46.000000 m9s_payment_gateway-7.0.6/.isort.cfg
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 15:10:01.191489 m9s_payment_gateway-7.0.6/.woodpecker/
+-rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2024-04-25 09:53:46.000000 m9s_payment_gateway-7.0.6/.woodpecker/mail_curl.sh
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2024-04-25 09:53:46.000000 m9s_payment_gateway-7.0.6/.woodpecker/report.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2024-04-25 09:53:46.000000 m9s_payment_gateway-7.0.6/.woodpecker/test.yml
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      798 2024-04-25 09:53:46.000000 m9s_payment_gateway-7.0.6/COPYRIGHT
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2024-04-25 09:53:46.000000 m9s_payment_gateway-7.0.6/INSTALL
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2024-04-25 09:53:46.000000 m9s_payment_gateway-7.0.6/LICENSE
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2024-04-25 09:53:46.000000 m9s_payment_gateway-7.0.6/MANIFEST.in
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3240 2024-04-25 15:10:01.203488 m9s_payment_gateway-7.0.6/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1062 2024-04-25 09:53:46.000000 m9s_payment_gateway-7.0.6/README.md
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-04-25 09:53:46.000000 m9s_payment_gateway-7.0.6/README.rst
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     1125 2024-04-25 09:53:46.000000 m9s_payment_gateway-7.0.6/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       86 2024-04-25 09:53:46.000000 m9s_payment_gateway-7.0.6/dev_requirements.txt
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 15:10:01.191489 m9s_payment_gateway-7.0.6/doc/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6818 2018-02-28 18:26:36.000000 m9s_payment_gateway-7.0.6/doc/Makefile
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2093 2018-02-28 18:26:36.000000 m9s_payment_gateway-7.0.6/doc/api_reference.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     9066 2024-02-02 17:23:06.000000 m9s_payment_gateway-7.0.6/doc/conf.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 15:10:01.191489 m9s_payment_gateway-7.0.6/doc/de/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       45 2024-04-25 09:53:46.000000 m9s_payment_gateway-7.0.6/doc/de/index.rst
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 15:10:01.203488 m9s_payment_gateway-7.0.6/doc/images/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)   302320 2018-02-28 18:26:36.000000 m9s_payment_gateway-7.0.6/doc/images/payment-gateways-add.png
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)   269848 2018-02-28 18:26:36.000000 m9s_payment_gateway-7.0.6/doc/images/payment-gateways.png
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)   363503 2018-02-28 18:26:36.000000 m9s_payment_gateway-7.0.6/doc/images/payment-profile-add.png
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)   308733 2018-02-28 18:26:36.000000 m9s_payment_gateway-7.0.6/doc/images/payment-profiles.png
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)   119650 2018-02-28 18:26:36.000000 m9s_payment_gateway-7.0.6/doc/images/payment-transaction-enter-card.png
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)   247886 2018-02-28 18:26:36.000000 m9s_payment_gateway-7.0.6/doc/images/payment-transaction-use-card.png
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)   259455 2018-02-28 18:26:36.000000 m9s_payment_gateway-7.0.6/doc/images/payment-transaction-using-profile.png
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-04-25 09:53:46.000000 m9s_payment_gateway-7.0.6/doc/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5383 2018-02-28 18:26:36.000000 m9s_payment_gateway-7.0.6/doc/introduction.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    20312 2018-02-28 18:26:36.000000 m9s_payment_gateway-7.0.6/doc/write_a_gateway.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4061 2024-02-02 21:27:24.000000 m9s_payment_gateway-7.0.6/dummy.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 15:10:01.187488 m9s_payment_gateway-7.0.6/locale/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    19590 2022-11-25 23:13:54.000000 m9s_payment_gateway-7.0.6/locale/de.po
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 15:10:01.203488 m9s_payment_gateway-7.0.6/m9s_payment_gateway.egg-info/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3240 2024-04-25 15:10:00.000000 m9s_payment_gateway-7.0.6/m9s_payment_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1974 2024-04-25 15:10:01.000000 m9s_payment_gateway-7.0.6/m9s_payment_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-04-25 15:10:00.000000 m9s_payment_gateway-7.0.6/m9s_payment_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       68 2024-04-25 15:10:00.000000 m9s_payment_gateway-7.0.6/m9s_payment_gateway.egg-info/entry_points.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2021-11-25 00:03:02.000000 m9s_payment_gateway-7.0.6/m9s_payment_gateway.egg-info/not-zip-safe
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      104 2024-04-25 15:10:00.000000 m9s_payment_gateway-7.0.6/m9s_payment_gateway.egg-info/requires.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-04-25 15:10:00.000000 m9s_payment_gateway-7.0.6/m9s_payment_gateway.egg-info/top_level.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2177 2024-02-02 21:27:54.000000 m9s_payment_gateway-7.0.6/manual.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1860 2023-12-26 13:19:11.000000 m9s_payment_gateway-7.0.6/message.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1651 2024-02-02 18:08:14.000000 m9s_payment_gateway-7.0.6/party.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2024-04-25 09:53:46.000000 m9s_payment_gateway-7.0.6/requirements.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      218 2024-04-25 15:10:01.203488 m9s_payment_gateway-7.0.6/setup.cfg
+-rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     4454 2024-04-25 09:53:46.000000 m9s_payment_gateway-7.0.6/setup.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 15:10:01.187488 m9s_payment_gateway-7.0.6/tests/
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      320 2024-04-25 09:53:46.000000 m9s_payment_gateway-7.0.6/tests/__init__.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    11142 2024-04-25 09:53:46.000000 m9s_payment_gateway-7.0.6/tests/test_module.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      595 2024-04-25 09:53:46.000000 m9s_payment_gateway-7.0.6/tox.ini
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    39259 2024-04-24 07:04:51.000000 m9s_payment_gateway-7.0.6/transaction.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    19022 2022-11-25 23:13:54.000000 m9s_payment_gateway-7.0.6/transaction.xml
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)       95 2024-04-25 09:53:46.000000 m9s_payment_gateway-7.0.6/tryton.cfg
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 15:10:01.191489 m9s_payment_gateway-7.0.6/view/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      834 2020-01-14 23:15:35.000000 m9s_payment_gateway-7.0.6/view/gateway_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      292 2020-01-14 23:15:35.000000 m9s_payment_gateway-7.0.6/view/gateway_list.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      567 2020-01-14 23:15:35.000000 m9s_payment_gateway-7.0.6/view/party_payment_profile_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      727 2020-01-14 23:15:35.000000 m9s_payment_gateway-7.0.6/view/payment_profile_add_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1009 2020-01-14 23:15:35.000000 m9s_payment_gateway-7.0.6/view/payment_profile_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      391 2020-01-14 23:15:35.000000 m9s_payment_gateway-7.0.6/view/payment_profile_list.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3086 2021-05-12 07:36:45.000000 m9s_payment_gateway-7.0.6/view/transaction_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      367 2020-01-14 23:15:35.000000 m9s_payment_gateway-7.0.6/view/transaction_list.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      461 2021-05-12 07:36:45.000000 m9s_payment_gateway-7.0.6/view/transaction_log_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      296 2021-05-12 07:36:45.000000 m9s_payment_gateway-7.0.6/view/transaction_log_list.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      987 2020-01-14 23:15:35.000000 m9s_payment_gateway-7.0.6/view/transaction_use_card_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      362 2020-01-14 23:15:35.000000 m9s_payment_gateway-7.0.6/view/user_form.xml
```

### Comparing `m9s_payment_gateway-7.0.5/.gitlab-ci.yml` & `m9s_payment_gateway-7.0.6/.gitlab-ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -47,37 +47,43 @@
     - tox -e py311-postgresql -vv -- -v
   tags:
     - postgres
 
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

### Comparing `m9s_payment_gateway-7.0.5/.woodpecker/mail_curl.sh` & `m9s_payment_gateway-7.0.6/.woodpecker/mail_curl.sh`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/.woodpecker/report.yml` & `m9s_payment_gateway-7.0.6/.woodpecker/report.yml`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/.woodpecker/test.yml` & `m9s_payment_gateway-7.0.6/.woodpecker/test.yml`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/COPYRIGHT` & `m9s_payment_gateway-7.0.6/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/INSTALL` & `m9s_payment_gateway-7.0.6/INSTALL`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/LICENSE` & `m9s_payment_gateway-7.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/PKG-INFO` & `m9s_payment_gateway-7.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s_payment_gateway
-Version: 7.0.5
+Version: 7.0.6
 Summary: Tryton Payment Gateway Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/payment_gateway.git
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
-[![Pipeline status](https://gitlab.com/m9s/payment_gateway/badges/master/pipeline.svg)](https://gitlab.com/m9s/payment_gateway/commits/master)
-
-Develop
-
-[![Pipeline status](https://gitlab.com/m9s/payment_gateway/badges/develop/pipeline.svg)](https://gitlab.com/m9s/payment_gateway/commits/develop)
-
-[![Coverage report](https://gitlab.com/m9s/payment_gateway/badges/develop/coverage.svg)](http://m9s.gitlab.io/payment_gateway)
-
+[![Tests Status](https://m9s.gitlab.io/payment_gateway/junit/junit-badge.svg)](https://m9s.gitlab.io/payment_gateway)
 
+[![Coverage Status](https://m9s.gitlab.io/payment_gateway/coverage/coverage-badge.svg)](https://m9s.gitlab.io/payment_gateway)
 
 This module runs with the Tryton application platform.
 
 Installing
 ----------
 
 See INSTALL
```

### Comparing `m9s_payment_gateway-7.0.5/README.md` & `m9s_payment_gateway-7.0.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,10 @@
-Master
-
-[![Pipeline status](https://gitlab.com/m9s/payment_gateway/badges/master/pipeline.svg)](https://gitlab.com/m9s/payment_gateway/commits/master)
-
-Develop
-
-[![Pipeline status](https://gitlab.com/m9s/payment_gateway/badges/develop/pipeline.svg)](https://gitlab.com/m9s/payment_gateway/commits/develop)
-
-[![Coverage report](https://gitlab.com/m9s/payment_gateway/badges/develop/coverage.svg)](http://m9s.gitlab.io/payment_gateway)
-
+[![Tests Status](https://m9s.gitlab.io/payment_gateway/junit/junit-badge.svg)](https://m9s.gitlab.io/payment_gateway)
 
+[![Coverage Status](https://m9s.gitlab.io/payment_gateway/coverage/coverage-badge.svg)](https://m9s.gitlab.io/payment_gateway)
 
 This module runs with the Tryton application platform.
 
 Installing
 ----------
 
 See INSTALL
```

### Comparing `m9s_payment_gateway-7.0.5/__init__.py` & `m9s_payment_gateway-7.0.6/__init__.py`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/doc/Makefile` & `m9s_payment_gateway-7.0.6/doc/Makefile`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/doc/api_reference.rst` & `m9s_payment_gateway-7.0.6/doc/api_reference.rst`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/doc/conf.py` & `m9s_payment_gateway-7.0.6/doc/conf.py`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/doc/images/payment-gateways-add.png` & `m9s_payment_gateway-7.0.6/doc/images/payment-gateways-add.png`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/doc/images/payment-gateways.png` & `m9s_payment_gateway-7.0.6/doc/images/payment-gateways.png`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/doc/images/payment-profile-add.png` & `m9s_payment_gateway-7.0.6/doc/images/payment-profile-add.png`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/doc/images/payment-profiles.png` & `m9s_payment_gateway-7.0.6/doc/images/payment-profiles.png`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/doc/images/payment-transaction-enter-card.png` & `m9s_payment_gateway-7.0.6/doc/images/payment-transaction-enter-card.png`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/doc/images/payment-transaction-use-card.png` & `m9s_payment_gateway-7.0.6/doc/images/payment-transaction-use-card.png`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/doc/images/payment-transaction-using-profile.png` & `m9s_payment_gateway-7.0.6/doc/images/payment-transaction-using-profile.png`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/doc/introduction.rst` & `m9s_payment_gateway-7.0.6/doc/introduction.rst`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/doc/write_a_gateway.rst` & `m9s_payment_gateway-7.0.6/doc/write_a_gateway.rst`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/dummy.py` & `m9s_payment_gateway-7.0.6/dummy.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                 'journal': journal_cash,
                 'account': expense,
                 'provider': 'dummy',
                 'method': 'credit_card',
             }])
 '''
 from trytond.model import fields
-from trytond.pool import Pool, PoolMeta
+from trytond.pool import PoolMeta
 from trytond.transaction import Transaction
 
 
 class PaymentGatewayDummy(metaclass=PoolMeta):
     "A Dummy Credit Card Processor for writing tests"
     __name__ = 'payment_gateway.gateway'
```

### Comparing `m9s_payment_gateway-7.0.5/locale/de.po` & `m9s_payment_gateway-7.0.6/locale/de.po`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/m9s_payment_gateway.egg-info/PKG-INFO` & `m9s_payment_gateway-7.0.6/m9s_payment_gateway.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s-payment-gateway
-Version: 7.0.5
+Version: 7.0.6
 Summary: Tryton Payment Gateway Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/payment_gateway.git
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
-[![Pipeline status](https://gitlab.com/m9s/payment_gateway/badges/master/pipeline.svg)](https://gitlab.com/m9s/payment_gateway/commits/master)
-
-Develop
-
-[![Pipeline status](https://gitlab.com/m9s/payment_gateway/badges/develop/pipeline.svg)](https://gitlab.com/m9s/payment_gateway/commits/develop)
-
-[![Coverage report](https://gitlab.com/m9s/payment_gateway/badges/develop/coverage.svg)](http://m9s.gitlab.io/payment_gateway)
-
+[![Tests Status](https://m9s.gitlab.io/payment_gateway/junit/junit-badge.svg)](https://m9s.gitlab.io/payment_gateway)
 
+[![Coverage Status](https://m9s.gitlab.io/payment_gateway/coverage/coverage-badge.svg)](https://m9s.gitlab.io/payment_gateway)
 
 This module runs with the Tryton application platform.
 
 Installing
 ----------
 
 See INSTALL
```

### Comparing `m9s_payment_gateway-7.0.5/m9s_payment_gateway.egg-info/SOURCES.txt` & `m9s_payment_gateway-7.0.6/m9s_payment_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/manual.py` & `m9s_payment_gateway-7.0.6/manual.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     Manual payment gateway
 
     Often payment modes are offline like cash, external credit card terminals
     etc. This gateway implements that
 '''
 
 from trytond.model import fields
-from trytond.pool import Pool, PoolMeta
+from trytond.pool import PoolMeta
 
 
 class PaymentGatewayManual(metaclass=PoolMeta):
     "COD, Cheque and Bank Transfer Implementation"
     __name__ = 'payment_gateway.gateway'
 
     @classmethod
```

### Comparing `m9s_payment_gateway-7.0.5/message.xml` & `m9s_payment_gateway-7.0.6/message.xml`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/party.py` & `m9s_payment_gateway-7.0.6/party.py`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/setup.py` & `m9s_payment_gateway-7.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/tests/test_module.py` & `m9s_payment_gateway-7.0.6/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/tox.ini` & `m9s_payment_gateway-7.0.6/tox.ini`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/transaction.py` & `m9s_payment_gateway-7.0.6/transaction.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 # The COPYRIGHT file at the top level of this repository contains
 # the full copyright notices and license terms.
+import logging
 import re
+import time
 
 from datetime import datetime
-from decimal import Decimal
 from uuid import uuid4
 
 import yaml
 
 from babel import dates, numbers
 
+from trytond.config import config
 from trytond.exceptions import UserError
 from trytond.i18n import gettext
 from trytond.model import (
     DeactivableMixin, ModelSQL, ModelView, Workflow, fields)
 from trytond.modules.currency.fields import Monetary
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Bool, Eval, If
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, _TransactionLockError
 from trytond.wizard import (
     Button, StateAction, StateTransition, StateView, Wizard)
 
 READONLY_IF_NOT_DRAFT = {'readonly': Eval('state') != 'draft'}
 STATES = {
     'readonly': ~Eval('active', True),
 }
 
+_retry = config.getint('database', 'retry')
+
+logger = logging.getLogger(__name__)
+
 
 class PaymentGateway(DeactivableMixin, ModelSQL, ModelView):
     """
     Payment Gateway
 
     Payment gateway record is a specific configuration for a `provider`
     """
@@ -74,16 +80,16 @@
 
     @classmethod
     @ModelView.button
     def test_gateway_configuration(cls, gateways):
         for gateway in gateways:
             journal = gateway.journal
             configured = bool(
-                journal.debit_account and
-                not journal.debit_account.party_required
+                journal.debit_account
+                and not journal.debit_account.party_required
             )
             gateway.configured = configured
             gateway.save()
 
     @staticmethod
     def default_provider():
         return 'self'
@@ -239,69 +245,69 @@
             ('authorized', 'completed'),
             ('completed', 'posted'),
             ('draft', 'posted'),       # direct charges for e.g. credit cards
         ))
         cls._buttons.update({
             'process': {
                 'invisible': ~(
-                    (Eval('state') == 'draft') &
-                    (Eval('method') == 'manual') &
-                    (Eval('type') == 'charge')
+                    (Eval('state') == 'draft')
+                    & (Eval('method') == 'manual')
+                    & (Eval('type') == 'charge')
                 ),
             },
             'cancel': {
                 'invisible': ~Eval('state').in_(['in-progress', 'authorized']),
             },
             'authorize': {
                 'invisible': ~(
-                    (Eval('state') == 'draft') &
-                    Eval('payment_profile', True) &
-                    (Eval('method') == 'credit_card') &
-                    (Eval('type') == 'charge')
+                    (Eval('state') == 'draft')
+                    & Eval('payment_profile', True)
+                    & (Eval('method') == 'credit_card')
+                    & (Eval('type') == 'charge')
                 ),
             },
             'settle': {
                 'invisible': ~(
-                    (Eval('state') == 'authorized') &
-                    (Eval('method') == 'credit_card') &
-                    (Eval('type') == 'charge')
+                    (Eval('state') == 'authorized')
+                    & (Eval('method') == 'credit_card')
+                    & (Eval('type') == 'charge')
                 ),
             },
             'retry': {
                 'invisible': ~(
-                    (Eval('state') == 'failed') &
-                    (Eval('type') == 'charge')
+                    (Eval('state') == 'failed')
+                    & (Eval('type') == 'charge')
                 )
             },
             'capture': {
                 'invisible': ~(
-                    (Eval('state') == 'draft') &
-                    (Eval('type') == 'charge')
+                    (Eval('state') == 'draft')
+                    & (Eval('type') == 'charge')
                 ),
             },
             'post': {
                 'invisible': ~(
-                    (Eval('state') == 'completed') &
-                    (Eval('type').in_(['charge', 'refund']))
+                    (Eval('state') == 'completed')
+                    & (Eval('type').in_(['charge', 'refund']))
                 )
             },
             'use_card': {
                 'invisible': ~(
-                    (Eval('state') == 'draft') &
-                    ~Bool(Eval('payment_profile')) &
-                    (Eval('method') == 'credit_card')
+                    (Eval('state') == 'draft')
+                    & ~Bool(Eval('payment_profile'))
+                    & (Eval('method') == 'credit_card')
                 ),
             },
             'update_status': {
                 'invisible': ~Eval('state').in_(['in-progress'])
             },
             'refund': {
                 'invisible': ~(
-                    (Eval('type') == 'refund') &
-                    (Eval('state') == 'draft')
+                    (Eval('type') == 'refund')
+                    & (Eval('state') == 'draft')
                 )
             }
         })
 
     @staticmethod
     def default_uuid():
         return str(uuid4())
@@ -589,32 +595,41 @@
         journal is not completed, marking as done could fail. In
         such cases, just mark as in-progress and let the user to
         manually mark as done.
 
         Failing  would otherwise rollback transaction but its
         not possible to rollback the payment
         """
-        try:
-            self.post([self])
-        except UserError as exc:
-            log = 'Could not mark as done\n'
-            log += str(exc)
-
-            # Delete the account move if there's one
-            # We need to do this because if we post transactions
-            # asyncronously using workers, the unwanted move will be
-            # commited causing duplicate moves
-            move_exists, move_number = self.delete_move_if_exists()
-            if move_exists:
-                log += "\nDeleted account move %s" % move_number
-
-            TransactionLog.create([{
-                'transaction': self,
-                'log': log
-            }])
+        count = 0
+        while True:
+            if count:
+                time.sleep(0.002 * (_retry - count))
+            try:
+                self.post([self])
+            except UserError as exc:
+                log = 'Could not mark as done\n'
+                log += str(exc)
+                # Delete the account move if there's one
+                # We need to do this because if we post transactions
+                # asyncronously using workers, the unwanted move will be
+                # committed causing duplicate moves
+                move_exists, move_number = self.delete_move_if_exists()
+                if move_exists:
+                    log += "\nDeleted account move %s" % move_number
+                TransactionLog.create([{
+                    'transaction': self,
+                    'log': log
+                }])
+            except _TransactionLockError as e:
+                if count < _retry:
+                    count += 1
+                    logger.debug(f"Retry: {count} for {e}")
+                    continue
+                raise
+            break
 
     def delete_move_if_exists(self):
         """
         Delete the account move if there's one
         """
         Move = Pool().get('account.move')
```

### Comparing `m9s_payment_gateway-7.0.5/transaction.xml` & `m9s_payment_gateway-7.0.6/transaction.xml`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/view/gateway_form.xml` & `m9s_payment_gateway-7.0.6/view/gateway_form.xml`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/view/party_payment_profile_form.xml` & `m9s_payment_gateway-7.0.6/view/party_payment_profile_form.xml`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/view/payment_profile_add_form.xml` & `m9s_payment_gateway-7.0.6/view/payment_profile_add_form.xml`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/view/payment_profile_form.xml` & `m9s_payment_gateway-7.0.6/view/payment_profile_form.xml`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/view/transaction_form.xml` & `m9s_payment_gateway-7.0.6/view/transaction_form.xml`

 * *Files identical despite different names*

### Comparing `m9s_payment_gateway-7.0.5/view/transaction_use_card_form.xml` & `m9s_payment_gateway-7.0.6/view/transaction_use_card_form.xml`

 * *Files identical despite different names*


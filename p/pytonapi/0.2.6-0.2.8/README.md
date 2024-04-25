# Comparing `tmp/pytonapi-0.2.6.tar.gz` & `tmp/pytonapi-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytonapi-0.2.6.tar", last modified: Tue Apr 23 02:18:51 2024, max compression
+gzip compressed data, was "pytonapi-0.2.8.tar", last modified: Thu Apr 25 11:24:44 2024, max compression
```

## Comparing `pytonapi-0.2.6.tar` & `pytonapi-0.2.8.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-23 02:18:51.648599 pytonapi-0.2.6/
--rw-rw-r--   0 ness      (1000) ness      (1000)     1060 2024-04-04 18:07:04.000000 pytonapi-0.2.6/LICENSE
--rw-r--r--   0 ness      (1000) ness      (1000)     5377 2024-04-23 02:18:51.648599 pytonapi-0.2.6/PKG-INFO
--rw-rw-r--   0 ness      (1000) ness      (1000)     4653 2024-04-04 18:07:04.000000 pytonapi-0.2.6/README.md
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-23 02:18:51.636599 pytonapi-0.2.6/pytonapi/
--rw-rw-r--   0 ness      (1000) ness      (1000)      129 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/__init__.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-23 02:18:51.636599 pytonapi-0.2.6/pytonapi/async_tonapi/
--rw-rw-r--   0 ness      (1000) ness      (1000)     3349 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/async_tonapi/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     9657 2024-04-22 23:59:07.000000 pytonapi-0.2.6/pytonapi/async_tonapi/client.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-23 02:18:51.640599 pytonapi-0.2.6/pytonapi/async_tonapi/methods/
--rw-rw-r--   0 ness      (1000) ness      (1000)      967 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/async_tonapi/methods/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)    14416 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/async_tonapi/methods/accounts.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     9152 2024-04-20 19:32:54.000000 pytonapi-0.2.6/pytonapi/async_tonapi/methods/blockchain.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1655 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/async_tonapi/methods/dns.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     4670 2024-04-20 20:11:38.000000 pytonapi-0.2.6/pytonapi/async_tonapi/methods/emulate.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1347 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/async_tonapi/methods/events.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     4176 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/async_tonapi/methods/inscriptions.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2633 2024-04-11 12:27:47.000000 pytonapi-0.2.6/pytonapi/async_tonapi/methods/jettons.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     8021 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/async_tonapi/methods/liteserver.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     4509 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/async_tonapi/methods/nft.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1791 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/async_tonapi/methods/rates.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     3780 2024-04-23 02:03:10.000000 pytonapi-0.2.6/pytonapi/async_tonapi/methods/sse.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2455 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/async_tonapi/methods/staking.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      476 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/async_tonapi/methods/storage.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      895 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/async_tonapi/methods/tonconnect.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      768 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/async_tonapi/methods/traces.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2343 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/async_tonapi/methods/wallet.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2349 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/async_tonapi/methods/websocket.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2279 2024-04-22 23:25:05.000000 pytonapi-0.2.6/pytonapi/exceptions.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-23 02:18:51.644599 pytonapi-0.2.6/pytonapi/schema/
--rw-rw-r--   0 ness      (1000) ness      (1000)      678 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/schema/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      874 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/schema/_address.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      896 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/schema/_balance.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1787 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/schema/accounts.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     7591 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/schema/blockchain.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      575 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/schema/dns.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      500 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/schema/domains.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     6158 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/schema/events.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      245 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/schema/inscriptions.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1486 2024-04-11 13:28:19.000000 pytonapi-0.2.6/pytonapi/schema/jettons.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1856 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/schema/liteserver.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1164 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/schema/nft.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      369 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/schema/rates.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1152 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/schema/staking.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      364 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/schema/storage.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      169 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/schema/tonconnect.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     3133 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/schema/traces.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-23 02:18:51.644599 pytonapi-0.2.6/pytonapi/tonapi/
--rw-rw-r--   0 ness      (1000) ness      (1000)     3028 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/tonapi/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     7813 2024-04-18 22:10:30.000000 pytonapi-0.2.6/pytonapi/tonapi/client.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-23 02:18:51.648599 pytonapi-0.2.6/pytonapi/tonapi/methods/
--rw-rw-r--   0 ness      (1000) ness      (1000)      905 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/tonapi/methods/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)    14172 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/tonapi/methods/accounts.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     8771 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/tonapi/methods/blockchain.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1592 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/tonapi/methods/dns.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     4594 2024-04-20 20:13:33.000000 pytonapi-0.2.6/pytonapi/tonapi/methods/emulate.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1310 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/tonapi/methods/events.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     4112 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/tonapi/methods/inscriptions.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2568 2024-04-11 12:29:15.000000 pytonapi-0.2.6/pytonapi/tonapi/methods/jettons.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     7825 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/tonapi/methods/liteserver.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     4324 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/tonapi/methods/nft.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1680 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/tonapi/methods/rates.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2313 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/tonapi/methods/sse.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2325 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/tonapi/methods/staking.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      448 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/tonapi/methods/storage.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      855 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/tonapi/methods/tonconnect.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      731 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/tonapi/methods/traces.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2279 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/tonapi/methods/wallet.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     3256 2024-04-04 18:07:04.000000 pytonapi-0.2.6/pytonapi/utils.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-23 02:18:51.636599 pytonapi-0.2.6/pytonapi.egg-info/
--rw-r--r--   0 ness      (1000) ness      (1000)     5377 2024-04-23 02:18:51.000000 pytonapi-0.2.6/pytonapi.egg-info/PKG-INFO
--rw-rw-r--   0 ness      (1000) ness      (1000)     2165 2024-04-23 02:18:51.000000 pytonapi-0.2.6/pytonapi.egg-info/SOURCES.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)        1 2024-04-23 02:18:51.000000 pytonapi-0.2.6/pytonapi.egg-info/dependency_links.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       45 2024-04-23 02:18:51.000000 pytonapi-0.2.6/pytonapi.egg-info/requires.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)        9 2024-04-23 02:18:51.000000 pytonapi-0.2.6/pytonapi.egg-info/top_level.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       38 2024-04-23 02:18:51.648599 pytonapi-0.2.6/setup.cfg
--rw-rw-r--   0 ness      (1000) ness      (1000)      970 2024-04-23 02:18:44.000000 pytonapi-0.2.6/setup.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-25 11:24:44.729197 pytonapi-0.2.8/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1060 2024-04-04 18:07:04.000000 pytonapi-0.2.8/LICENSE
+-rw-r--r--   0 ness      (1000) ness      (1000)     5377 2024-04-25 11:24:44.729197 pytonapi-0.2.8/PKG-INFO
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4653 2024-04-04 18:07:04.000000 pytonapi-0.2.8/README.md
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-25 11:24:44.717196 pytonapi-0.2.8/pytonapi/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      129 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/__init__.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-25 11:24:44.717196 pytonapi-0.2.8/pytonapi/async_tonapi/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3349 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     9657 2024-04-22 23:59:07.000000 pytonapi-0.2.8/pytonapi/async_tonapi/client.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-25 11:24:44.721197 pytonapi-0.2.8/pytonapi/async_tonapi/methods/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      967 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)    14416 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/accounts.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     9152 2024-04-20 19:32:54.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/blockchain.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1655 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/dns.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4670 2024-04-20 20:11:38.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/emulate.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1347 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/events.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4176 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/inscriptions.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2633 2024-04-11 12:27:47.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/jettons.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     8021 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/liteserver.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4509 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/nft.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1791 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/rates.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3798 2024-04-25 11:21:31.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/sse.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2455 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/staking.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      476 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/storage.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      895 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/tonconnect.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      768 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/traces.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2343 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/wallet.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2367 2024-04-25 11:21:42.000000 pytonapi-0.2.8/pytonapi/async_tonapi/methods/websocket.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2279 2024-04-22 23:25:05.000000 pytonapi-0.2.8/pytonapi/exceptions.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)        0 2024-04-25 11:21:31.000000 pytonapi-0.2.8/pytonapi/py.typed
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-25 11:24:44.725196 pytonapi-0.2.8/pytonapi/schema/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      735 2024-04-25 11:21:31.000000 pytonapi-0.2.8/pytonapi/schema/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      874 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/_address.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      896 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/_balance.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1787 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/accounts.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     7591 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/blockchain.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      575 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/dns.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      500 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/domains.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     6158 2024-04-25 11:21:31.000000 pytonapi-0.2.8/pytonapi/schema/events.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      245 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/inscriptions.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1486 2024-04-11 13:28:19.000000 pytonapi-0.2.8/pytonapi/schema/jettons.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1856 2024-04-25 11:21:31.000000 pytonapi-0.2.8/pytonapi/schema/liteserver.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1164 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/nft.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      369 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/rates.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1152 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/staking.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      364 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/storage.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      169 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/tonconnect.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3133 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/schema/traces.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-25 11:24:44.725196 pytonapi-0.2.8/pytonapi/tonapi/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3028 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     7813 2024-04-18 22:10:30.000000 pytonapi-0.2.8/pytonapi/tonapi/client.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-25 11:24:44.729197 pytonapi-0.2.8/pytonapi/tonapi/methods/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      905 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)    14172 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/accounts.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     8771 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/blockchain.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1592 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/dns.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4594 2024-04-20 20:13:33.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/emulate.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1310 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/events.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4112 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/inscriptions.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2568 2024-04-11 12:29:15.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/jettons.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     7825 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/liteserver.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4330 2024-04-25 11:21:31.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/nft.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1680 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/rates.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2553 2024-04-25 11:21:31.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/sse.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2325 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/staking.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      448 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/storage.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      855 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/tonconnect.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      731 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/traces.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2279 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/tonapi/methods/wallet.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3256 2024-04-04 18:07:04.000000 pytonapi-0.2.8/pytonapi/utils.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-25 11:24:44.717196 pytonapi-0.2.8/pytonapi.egg-info/
+-rw-r--r--   0 ness      (1000) ness      (1000)     5377 2024-04-25 11:24:44.000000 pytonapi-0.2.8/pytonapi.egg-info/PKG-INFO
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2183 2024-04-25 11:24:44.000000 pytonapi-0.2.8/pytonapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)        1 2024-04-25 11:24:44.000000 pytonapi-0.2.8/pytonapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       45 2024-04-25 11:24:44.000000 pytonapi-0.2.8/pytonapi.egg-info/requires.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)        9 2024-04-25 11:24:44.000000 pytonapi-0.2.8/pytonapi.egg-info/top_level.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       38 2024-04-25 11:24:44.729197 pytonapi-0.2.8/setup.cfg
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1023 2024-04-25 11:24:37.000000 pytonapi-0.2.8/setup.py
```

### Comparing `pytonapi-0.2.6/LICENSE` & `pytonapi-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/PKG-INFO` & `pytonapi-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytonapi
-Version: 0.2.6
+Version: 0.2.8
 Summary: Provide access to indexed TON blockchain.
 Home-page: https://github.com/tonkeeper/pytonapi/
 Author: nessshon
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pytonapi-0.2.6/README.md` & `pytonapi-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/async_tonapi/__init__.py` & `pytonapi-0.2.8/pytonapi/async_tonapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/async_tonapi/client.py` & `pytonapi-0.2.8/pytonapi/async_tonapi/client.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/async_tonapi/methods/__init__.py` & `pytonapi-0.2.8/pytonapi/async_tonapi/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/async_tonapi/methods/accounts.py` & `pytonapi-0.2.8/pytonapi/async_tonapi/methods/accounts.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/async_tonapi/methods/blockchain.py` & `pytonapi-0.2.8/pytonapi/async_tonapi/methods/blockchain.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/async_tonapi/methods/dns.py` & `pytonapi-0.2.8/pytonapi/async_tonapi/methods/dns.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/async_tonapi/methods/emulate.py` & `pytonapi-0.2.8/pytonapi/async_tonapi/methods/emulate.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/async_tonapi/methods/events.py` & `pytonapi-0.2.8/pytonapi/async_tonapi/methods/events.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/async_tonapi/methods/inscriptions.py` & `pytonapi-0.2.8/pytonapi/async_tonapi/methods/inscriptions.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/async_tonapi/methods/jettons.py` & `pytonapi-0.2.8/pytonapi/async_tonapi/methods/jettons.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/async_tonapi/methods/liteserver.py` & `pytonapi-0.2.8/pytonapi/async_tonapi/methods/liteserver.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/async_tonapi/methods/nft.py` & `pytonapi-0.2.8/pytonapi/async_tonapi/methods/nft.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/async_tonapi/methods/rates.py` & `pytonapi-0.2.8/pytonapi/async_tonapi/methods/rates.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/async_tonapi/methods/sse.py` & `pytonapi-0.2.8/pytonapi/async_tonapi/methods/sse.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pytonapi.schema.events import TransactionEventData, TraceEventData, MempoolEventData
 
 
 class SSEMethod(AsyncTonapiClient):
 
     async def subscribe_to_transactions(
             self,
-            handler: Callable[[TransactionEventData, ...], Awaitable[Any]],
+            handler: Callable[[TransactionEventData, List[Any]], Awaitable[Any]],
             accounts: List[str],
             operations: Optional[List[str]] = None,
             args: Tuple[Any, ...] = (),
     ) -> Any:
         """
         Subscribes to transactions SSE events for the specified accounts.
 
@@ -41,15 +41,15 @@
             result = await handler(event, *args)
             if result is not None:
                 return result
 
     async def subscribe_to_traces(
             self,
             accounts: List[str],
-            handler: Callable[[TraceEventData, ...], Awaitable[Any]],
+            handler: Callable[[TraceEventData, List[Any]], Awaitable[Any]],
             args: Tuple[Any, ...] = (),
     ) -> Any:
         """
         Subscribes to traces SSE events for the specified accounts.
 
         :handler: A callable function to handle the SSEEvent
         :accounts: A list of account addresses to subscribe to
@@ -61,15 +61,15 @@
             result = await handler(event, *args)
             if result is not None:
                 return result
 
     async def subscribe_to_mempool(
             self,
             accounts: List[str],
-            handler: Callable[[MempoolEventData, ...], Awaitable[Any]],
+            handler: Callable[[MempoolEventData, List[Any]], Awaitable[Any]],
             args: Tuple[Any, ...] = (),
     ) -> Any:
         """
         Subscribes to mempool SSE events for the specified accounts.
 
         :handler: A callable function to handle the SSEEvent
         :accounts: A list of account addresses to subscribe to
```

### Comparing `pytonapi-0.2.6/pytonapi/async_tonapi/methods/staking.py` & `pytonapi-0.2.8/pytonapi/async_tonapi/methods/staking.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/async_tonapi/methods/tonconnect.py` & `pytonapi-0.2.8/pytonapi/async_tonapi/methods/tonconnect.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/async_tonapi/methods/traces.py` & `pytonapi-0.2.8/pytonapi/async_tonapi/methods/traces.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/async_tonapi/methods/wallet.py` & `pytonapi-0.2.8/pytonapi/async_tonapi/methods/wallet.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/async_tonapi/methods/websocket.py` & `pytonapi-0.2.8/pytonapi/async_tonapi/methods/websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class WebSocketMethod(AsyncTonapiClient):
 
     async def subscribe_to_transactions(
             self,
             accounts: List[str],
-            handler: Callable[[TransactionEventData, ...], Awaitable[Any]],
+            handler: Callable[[TransactionEventData, List[Any]], Awaitable[Any]],
             args: Tuple[Any, ...] = (),
     ) -> None:
         """
         Subscribes to transactions WebSocket events for the specified accounts.
 
         :param handler: A callable function to handle the WSMessage
         :param accounts: A list of account addresses to subscribe to
@@ -24,15 +24,15 @@
         async for data in self._subscribe_websocket(method=method, params=params):
             event = TransactionEventData(**data)
             await handler(event, *args)
 
     async def subscribe_to_traces(
             self,
             accounts: List[str],
-            handler: Callable[[TraceEventData, ...], Awaitable[Any]],
+            handler: Callable[[TraceEventData, List[Any]], Awaitable[Any]],
             args: Tuple[Any, ...] = (),
     ) -> None:
         """
         Subscribes to traces WebSocket events for the specified accounts.
 
         :handler: A callable function to handle the WSMessage
         :accounts: A list of account addresses to subscribe to
@@ -42,15 +42,15 @@
         async for data in self._subscribe_websocket(method=method, params=params):
             event = TraceEventData(**data)
             await handler(event, *args)
 
     async def subscribe_to_mempool(
             self,
             accounts: List[str],
-            handler: Callable[[MempoolEventData, ...], Awaitable[Any]],
+            handler: Callable[[MempoolEventData, List[Any]], Awaitable[Any]],
             args: Tuple[Any, ...] = (),
     ) -> None:
         """
         Subscribes to mempool WebSocket events for the specified accounts.
 
         :handler: A callable function to handle the WSMessage
         :accounts: A list of account addresses to subscribe to
```

### Comparing `pytonapi-0.2.6/pytonapi/exceptions.py` & `pytonapi-0.2.8/pytonapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/schema/__init__.py` & `pytonapi-0.2.8/pytonapi/schema/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pytonapi.schema import accounts
 from pytonapi.schema import blockchain
 from pytonapi.schema import dns
 from pytonapi.schema import domains
 from pytonapi.schema import events
 from pytonapi.schema import inscriptions
 from pytonapi.schema import jettons
+from pytonapi.schema import liteserver
 from pytonapi.schema import nft
 from pytonapi.schema import rates
 from pytonapi.schema import staking
 from pytonapi.schema import storage
 from pytonapi.schema import tonconnect
 from pytonapi.schema import traces
 
@@ -16,14 +17,15 @@
     "accounts",
     "blockchain",
     "dns",
     "domains",
     "events",
     "inscriptions",
     "jettons",
+    "liteserver",
     "nft",
     "rates",
     "staking",
     "storage",
     "tonconnect",
     "traces",
 ]
```

### Comparing `pytonapi-0.2.6/pytonapi/schema/_address.py` & `pytonapi-0.2.8/pytonapi/schema/_address.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/schema/_balance.py` & `pytonapi-0.2.8/pytonapi/schema/_balance.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/schema/accounts.py` & `pytonapi-0.2.8/pytonapi/schema/accounts.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/schema/blockchain.py` & `pytonapi-0.2.8/pytonapi/schema/blockchain.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/schema/dns.py` & `pytonapi-0.2.8/pytonapi/schema/dns.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/schema/events.py` & `pytonapi-0.2.8/pytonapi/schema/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,15 @@
     quantity: int
 
 
 class ValueFlow(BaseModel):
     account: AccountAddress
     ton: int
     fees: int
-    jettons: Optional[list[ValueFlowJettonsInner]]
+    jettons: Optional[List[ValueFlowJettonsInner]]
 
 
 class Event(BaseModel):
     event_id: str
     timestamp: int
     actions: List[Action]
     value_flow: List[ValueFlow]
```

### Comparing `pytonapi-0.2.6/pytonapi/schema/jettons.py` & `pytonapi-0.2.8/pytonapi/schema/jettons.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/schema/liteserver.py` & `pytonapi-0.2.8/pytonapi/schema/liteserver.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Optional
 
 from pydantic.v1 import BaseModel, Field
 
 
 class BlockRaw(BaseModel):
     workchain: int
-    shard: int
+    shard: str
     seqno: int
     root_hash: str
     file_hash: str
 
 
 class InitStateRaw(BaseModel):
     workchain: int
```

### Comparing `pytonapi-0.2.6/pytonapi/schema/nft.py` & `pytonapi-0.2.8/pytonapi/schema/nft.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/schema/staking.py` & `pytonapi-0.2.8/pytonapi/schema/staking.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/schema/traces.py` & `pytonapi-0.2.8/pytonapi/schema/traces.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/tonapi/__init__.py` & `pytonapi-0.2.8/pytonapi/tonapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/tonapi/client.py` & `pytonapi-0.2.8/pytonapi/tonapi/client.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/tonapi/methods/__init__.py` & `pytonapi-0.2.8/pytonapi/tonapi/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/tonapi/methods/accounts.py` & `pytonapi-0.2.8/pytonapi/tonapi/methods/accounts.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/tonapi/methods/blockchain.py` & `pytonapi-0.2.8/pytonapi/tonapi/methods/blockchain.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/tonapi/methods/dns.py` & `pytonapi-0.2.8/pytonapi/tonapi/methods/dns.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/tonapi/methods/emulate.py` & `pytonapi-0.2.8/pytonapi/tonapi/methods/emulate.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/tonapi/methods/events.py` & `pytonapi-0.2.8/pytonapi/tonapi/methods/events.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/tonapi/methods/inscriptions.py` & `pytonapi-0.2.8/pytonapi/tonapi/methods/inscriptions.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/tonapi/methods/jettons.py` & `pytonapi-0.2.8/pytonapi/tonapi/methods/jettons.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/tonapi/methods/liteserver.py` & `pytonapi-0.2.8/pytonapi/tonapi/methods/liteserver.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/tonapi/methods/nft.py` & `pytonapi-0.2.8/pytonapi/tonapi/methods/nft.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import Optional, List
 
 from pytonapi.schema.events import AccountEvents
 from pytonapi.tonapi.client import TonapiClient
 
 from pytonapi.schema.nft import NftCollections, NftCollection, NftItems, NftItem
 
 
@@ -80,15 +80,15 @@
         :return: :class:`NftItem`
         """
         method = f"v2/nfts/{account_id}"
         response = self._get(method=method)
 
         return NftItem(**response)
 
-    def get_bulk_items(self, account_ids: list[str]) -> NftItems:
+    def get_bulk_items(self, account_ids: List[str]) -> NftItems:
         """
         Get NFT items by their addresses
 
         :param account_ids: a list of account IDs
         """
         method = f"v2/nfts/_bulk"
         params = {"account_ids": account_ids}
```

### Comparing `pytonapi-0.2.6/pytonapi/tonapi/methods/rates.py` & `pytonapi-0.2.8/pytonapi/tonapi/methods/rates.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/tonapi/methods/sse.py` & `pytonapi-0.2.8/pytonapi/tonapi/methods/sse.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,34 +6,36 @@
 
 
 class SSEMethod(TonapiClient):
 
     def subscribe_to_transactions(
             self,
             accounts: List[str],
-            handler: Callable[[TransactionEventData, ...], Any],
+            handler: Callable[[TransactionEventData, List[Any]], Any],
             args: Tuple[Any, ...] = (),
     ) -> None:
         """
         Subscribes to transactions SSE events for the specified accounts.
 
         :param handler: A callable function to handle the SSEEvent
         :param accounts: A list of account addresses to subscribe to
         :param args: Additional arguments to pass to the handler
         """
         method = "v2/sse/accounts/transactions"
         params = {'accounts': accounts}
         for data in self._subscribe(method=method, params=params):
             event = TransactionEventData(**json.loads(data))
-            handler(event, *args)
+            result = handler(event, *args)
+            if result is not None:
+                return result
 
     def subscribe_to_traces(
             self,
             accounts: List[str],
-            handler: Callable[[TraceEventData, ...], Any],
+            handler: Callable[[TraceEventData, List[Any]], Any],
             args: Tuple[Any, ...] = (),
     ) -> None:
         """
         Subscribes to traces SSE events for the specified accounts.
 
         :handler: A callable function to handle the SSEEvent
         :accounts: A list of account addresses to subscribe to
@@ -41,26 +43,30 @@
         Returns:
             None
         """
         method = "v2/sse/accounts/traces"
         params = {'accounts': accounts}
         for data in self._subscribe(method=method, params=params):
             event = TraceEventData(**json.loads(data))
-            handler(event, *args)
+            result = handler(event, *args)
+            if result is not None:
+                return result
 
     def subscribe_to_mempool(
             self,
             accounts: List[str],
-            handler: Callable[[MempoolEventData, ...], Any],
+            handler: Callable[[MempoolEventData, List[Any]], Any],
             args: Tuple[Any, ...] = (),
     ) -> None:
         """
         Subscribes to mempool SSE events for the specified accounts.
 
         :handler: A callable function to handle the SSEEvent
         :accounts: A list of account addresses to subscribe to
         """
         method = "v2/sse/mempool"
         params = {'accounts': accounts}
         for data in self._subscribe(method=method, params=params):
             event = MempoolEventData(**json.loads(data))
-            handler(event, *args)
+            result = handler(event, *args)
+            if result is not None:
+                return result
```

### Comparing `pytonapi-0.2.6/pytonapi/tonapi/methods/staking.py` & `pytonapi-0.2.8/pytonapi/tonapi/methods/staking.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/tonapi/methods/tonconnect.py` & `pytonapi-0.2.8/pytonapi/tonapi/methods/tonconnect.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/tonapi/methods/traces.py` & `pytonapi-0.2.8/pytonapi/tonapi/methods/traces.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/tonapi/methods/wallet.py` & `pytonapi-0.2.8/pytonapi/tonapi/methods/wallet.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi/utils.py` & `pytonapi-0.2.8/pytonapi/utils.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.2.6/pytonapi.egg-info/PKG-INFO` & `pytonapi-0.2.8/pytonapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytonapi
-Version: 0.2.6
+Version: 0.2.8
 Summary: Provide access to indexed TON blockchain.
 Home-page: https://github.com/tonkeeper/pytonapi/
 Author: nessshon
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pytonapi-0.2.6/pytonapi.egg-info/SOURCES.txt` & `pytonapi-0.2.8/pytonapi.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 pytonapi/__init__.py
 pytonapi/exceptions.py
+pytonapi/py.typed
 pytonapi/utils.py
 pytonapi.egg-info/PKG-INFO
 pytonapi.egg-info/SOURCES.txt
 pytonapi.egg-info/dependency_links.txt
 pytonapi.egg-info/requires.txt
 pytonapi.egg-info/top_level.txt
 pytonapi/async_tonapi/__init__.py
```

### Comparing `pytonapi-0.2.6/setup.py` & `pytonapi-0.2.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytonapi",
-    version="0.2.6",
+    version="0.2.8",
     author="nessshon",
     description="Provide access to indexed TON blockchain.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tonkeeper/pytonapi/",
     packages=setuptools.find_packages(exclude=["examples", "tests"]),
     install_requires=[
@@ -23,8 +23,11 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
+    package_data={
+        "": ["*py.typed"],
+    },
 )
```


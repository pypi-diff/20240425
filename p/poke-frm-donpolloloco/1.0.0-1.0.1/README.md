# Comparing `tmp/poke_frm_donpolloloco-1.0.0.tar.gz` & `tmp/poke_frm_donpolloloco-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poke_frm_donpolloloco-1.0.0.tar", last modified: Tue Apr 23 17:37:42 2024, max compression
+gzip compressed data, was "poke_frm_donpolloloco-1.0.1.tar", last modified: Wed Apr 24 18:57:06 2024, max compression
```

## Comparing `poke_frm_donpolloloco-1.0.0.tar` & `poke_frm_donpolloloco-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 17:37:42.779497 poke_frm_donpolloloco-1.0.0/
--rw-rw-rw-   0        0        0      236 2024-04-23 17:37:42.773854 poke_frm_donpolloloco-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      275 2024-04-23 17:30:43.000000 poke_frm_donpolloloco-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 17:37:42.767495 poke_frm_donpolloloco-1.0.0/poke_frm_donpolloloco.egg-info/
--rw-rw-rw-   0        0        0      236 2024-04-23 17:37:42.000000 poke_frm_donpolloloco-1.0.0/poke_frm_donpolloloco.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-04-23 17:37:42.000000 poke_frm_donpolloloco-1.0.0/poke_frm_donpolloloco.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 17:37:42.000000 poke_frm_donpolloloco-1.0.0/poke_frm_donpolloloco.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 17:37:42.000000 poke_frm_donpolloloco-1.0.0/poke_frm_donpolloloco.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 17:37:42.000000 poke_frm_donpolloloco-1.0.0/poke_frm_donpolloloco.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 17:37:42.780504 poke_frm_donpolloloco-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      411 2024-04-23 17:32:22.000000 poke_frm_donpolloloco-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:57:06.264024 poke_frm_donpolloloco-1.0.1/
+-rw-rw-rw-   0        0        0      236 2024-04-24 18:57:06.261919 poke_frm_donpolloloco-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 18:57:06.236624 poke_frm_donpolloloco-1.0.1/POKE_DONPOLLO/
+-rw-rw-rw-   0        0        0       43 2024-04-19 15:35:51.000000 poke_frm_donpolloloco-1.0.1/POKE_DONPOLLO/__init__.py
+-rw-rw-rw-   0        0        0    44028 2024-04-16 17:19:52.000000 poke_frm_donpolloloco-1.0.1/POKE_DONPOLLO/pokemon.csv
+-rw-rw-rw-   0        0        0     2408 2024-04-24 03:46:11.000000 poke_frm_donpolloloco-1.0.1/POKE_DONPOLLO/ramdom_pokemon.py
+-rw-rw-rw-   0        0        0      275 2024-04-23 17:30:43.000000 poke_frm_donpolloloco-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 18:57:06.260896 poke_frm_donpolloloco-1.0.1/poke_frm_donpolloloco.egg-info/
+-rw-rw-rw-   0        0        0      236 2024-04-24 18:57:05.000000 poke_frm_donpolloloco-1.0.1/poke_frm_donpolloloco.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2024-04-24 18:57:05.000000 poke_frm_donpolloloco-1.0.1/poke_frm_donpolloloco.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 18:57:05.000000 poke_frm_donpolloloco-1.0.1/poke_frm_donpolloloco.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 18:57:05.000000 poke_frm_donpolloloco-1.0.1/poke_frm_donpolloloco.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-24 18:57:05.000000 poke_frm_donpolloloco-1.0.1/poke_frm_donpolloloco.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 18:57:06.264024 poke_frm_donpolloloco-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      404 2024-04-24 18:57:00.000000 poke_frm_donpolloloco-1.0.1/setup.py
```


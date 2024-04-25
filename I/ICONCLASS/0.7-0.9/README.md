# Comparing `tmp/ICONCLASS-0.7.tar.gz` & `tmp/ICONCLASS-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ICONCLASS-0.7.tar", last modified: Mon Sep 30 09:12:01 2019, max compression
+gzip compressed data, was "dist/ICONCLASS-0.9.tar", last modified: Mon Nov 25 09:46:22 2019, max compression
```

## Comparing `ICONCLASS-0.7.tar` & `ICONCLASS-0.9.tar`

### file list

```diff
@@ -1,4 +1,4 @@
-drwxr-xr-x   0 etienne    (501) wheel        (0)        0 2019-09-30 09:12:01.000000 ICONCLASS-0.7/
--rw-r--r--   0 etienne    (501) wheel        (0)      374 2019-09-30 09:12:01.000000 ICONCLASS-0.7/PKG-INFO
--rw-r--r--   0 etienne    (501) wheel        (0)    14633 2019-09-30 09:08:34.000000 ICONCLASS-0.7/iconclass.py
--rw-r--r--   0 etienne    (501) wheel        (0)      426 2019-09-30 09:11:29.000000 ICONCLASS-0.7/setup.py
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2019-11-25 09:46:22.000000 ICONCLASS-0.9/
+-rw-r--r--   0 etienne    (501) staff       (20)      279 2019-11-25 09:46:22.000000 ICONCLASS-0.9/PKG-INFO
+-rw-r--r--   0 etienne    (501) staff       (20)    10386 2019-10-26 00:03:55.000000 ICONCLASS-0.9/iconclass.py
+-rw-r--r--   0 etienne    (501) staff       (20)      309 2019-10-17 03:42:33.000000 ICONCLASS-0.9/setup.py
```


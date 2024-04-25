# Comparing `tmp/lucien-0.0.1.tar.gz` & `tmp/lucien-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lucien-0.0.1.tar", last modified: Thu Apr  4 14:32:08 2024, max compression
+gzip compressed data, was "lucien-0.0.2.tar", last modified: Thu Apr 25 04:00:27 2024, max compression
```

## Comparing `lucien-0.0.1.tar` & `lucien-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,21 @@
-drwxr-xr-x   0 franciscome   (501) staff       (20)        0 2024-04-04 14:32:08.281787 lucien-0.0.1/
--rw-r--r--   0 franciscome   (501) staff       (20)    11357 2024-04-04 03:31:16.000000 lucien-0.0.1/LICENSE
--rw-r--r--   0 franciscome   (501) staff       (20)       86 2024-04-04 03:45:40.000000 lucien-0.0.1/MANIFEST.in
--rw-r--r--   0 franciscome   (501) staff       (20)      614 2024-04-04 14:32:08.281595 lucien-0.0.1/PKG-INFO
--rw-r--r--   0 franciscome   (501) staff       (20)       15 2024-04-04 03:45:31.000000 lucien-0.0.1/README.md
-drwxr-xr-x   0 franciscome   (501) staff       (20)        0 2024-04-04 14:32:08.281412 lucien-0.0.1/lucien.egg-info/
--rw-r--r--   0 franciscome   (501) staff       (20)      614 2024-04-04 14:32:08.000000 lucien-0.0.1/lucien.egg-info/PKG-INFO
--rw-r--r--   0 franciscome   (501) staff       (20)      200 2024-04-04 14:32:08.000000 lucien-0.0.1/lucien.egg-info/SOURCES.txt
--rw-r--r--   0 franciscome   (501) staff       (20)        1 2024-04-04 14:32:08.000000 lucien-0.0.1/lucien.egg-info/dependency_links.txt
--rw-r--r--   0 franciscome   (501) staff       (20)        1 2024-04-04 14:32:08.000000 lucien-0.0.1/lucien.egg-info/not-zip-safe
--rw-r--r--   0 franciscome   (501) staff       (20)        1 2024-04-04 14:32:08.000000 lucien-0.0.1/lucien.egg-info/top_level.txt
--rw-r--r--   0 franciscome   (501) staff       (20)      908 2024-04-04 14:31:51.000000 lucien-0.0.1/settings.ini
--rw-r--r--   0 franciscome   (501) staff       (20)       38 2024-04-04 14:32:08.281834 lucien-0.0.1/setup.cfg
--rw-r--r--   0 franciscome   (501) staff       (20)     1820 2024-04-04 04:41:41.000000 lucien-0.0.1/setup.py
+drwxr-xr-x   0 franciscome   (501) staff       (20)        0 2024-04-25 04:00:27.683900 lucien-0.0.2/
+-rw-r--r--   0 franciscome   (501) staff       (20)      524 2024-04-25 03:19:46.000000 lucien-0.0.2/Cargo.toml
+-rw-r--r--   0 franciscome   (501) staff       (20)      107 2024-04-25 02:10:46.000000 lucien-0.0.2/MANIFEST.in
+-rw-r--r--   0 franciscome   (501) staff       (20)       50 2024-04-25 04:00:27.683727 lucien-0.0.2/PKG-INFO
+-rw-r--r--   0 franciscome   (501) staff       (20)        9 2024-04-11 14:56:40.000000 lucien-0.0.2/README.md
+-rw-r--r--   0 franciscome   (501) staff       (20)      407 2024-04-25 01:32:52.000000 lucien-0.0.2/pyproject.toml
+drwxr-xr-x   0 franciscome   (501) staff       (20)        0 2024-04-25 04:00:27.682019 lucien-0.0.2/python/
+-rwxr-xr-x   0 franciscome   (501) staff       (20)  1031936 2024-04-24 23:59:24.000000 lucien-0.0.2/python/_lib.cpython-312-darwin.so
+drwxr-xr-x   0 franciscome   (501) staff       (20)        0 2024-04-25 04:00:27.682797 lucien-0.0.2/python/lucien/
+-rw-r--r--   0 franciscome   (501) staff       (20)      219 2024-04-25 03:56:00.000000 lucien-0.0.2/python/lucien/__init__.py
+-rw-r--r--   0 franciscome   (501) staff       (20)       32 2024-04-24 23:36:36.000000 lucien-0.0.2/python/lucien/printer.py
+drwxr-xr-x   0 franciscome   (501) staff       (20)        0 2024-04-25 04:00:27.683574 lucien-0.0.2/python/lucien.egg-info/
+-rw-r--r--   0 franciscome   (501) staff       (20)       50 2024-04-25 04:00:27.000000 lucien-0.0.2/python/lucien.egg-info/PKG-INFO
+-rw-r--r--   0 franciscome   (501) staff       (20)      314 2024-04-25 04:00:27.000000 lucien-0.0.2/python/lucien.egg-info/SOURCES.txt
+-rw-r--r--   0 franciscome   (501) staff       (20)        1 2024-04-25 04:00:27.000000 lucien-0.0.2/python/lucien.egg-info/dependency_links.txt
+-rw-r--r--   0 franciscome   (501) staff       (20)        7 2024-04-25 04:00:27.000000 lucien-0.0.2/python/lucien.egg-info/top_level.txt
+drwxr-xr-x   0 franciscome   (501) staff       (20)        0 2024-04-25 04:00:27.683321 lucien-0.0.2/rust/
+-rw-r--r--   0 franciscome   (501) staff       (20)     1716 2024-04-25 03:52:29.000000 lucien-0.0.2/rust/lib.rs
+-rw-r--r--   0 franciscome   (501) staff       (20)       38 2024-04-25 04:00:27.683934 lucien-0.0.2/setup.cfg
+drwxr-xr-x   0 franciscome   (501) staff       (20)        0 2024-04-25 04:00:27.683425 lucien-0.0.2/tests/
+-rw-r--r--   0 franciscome   (501) staff       (20)      117 2024-04-24 23:57:08.000000 lucien-0.0.2/tests/test_package.py
```


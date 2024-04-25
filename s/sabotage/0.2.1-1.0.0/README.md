# Comparing `tmp/sabotage-0.2.1.tar.gz` & `tmp/sabotage-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sabotage-0.2.1.tar", last modified: Sun Mar 17 09:59:36 2019, max compression
+gzip compressed data, was "sabotage-1.0.0.tar", last modified: Thu Apr 25 20:41:14 2024, max compression
```

## Comparing `sabotage-0.2.1.tar` & `sabotage-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-17 09:59:36.000000 sabotage-0.2.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-17 09:59:36.000000 sabotage-0.2.1/sabotage.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2019-03-17 09:59:36.000000 sabotage-0.2.1/sabotage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      972 2019-03-17 09:59:36.000000 sabotage-0.2.1/sabotage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       18 2019-03-17 09:59:36.000000 sabotage-0.2.1/sabotage.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      224 2019-03-17 09:59:36.000000 sabotage-0.2.1/sabotage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        9 2019-03-17 09:59:36.000000 sabotage-0.2.1/sabotage.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      972 2019-03-17 09:59:36.000000 sabotage-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2019-03-17 09:59:36.000000 sabotage-0.2.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-17 09:59:36.000000 sabotage-0.2.1/sabotage/
--rw-r--r--   0 root         (0) root         (0)     2169 2019-03-17 09:59:33.000000 sabotage-0.2.1/sabotage/_disconnected.py
--rw-r--r--   0 root         (0) root         (0)      175 2019-03-17 09:59:33.000000 sabotage-0.2.1/sabotage/__init__.py
--rw-r--r--   0 root         (0) root         (0)      399 2019-03-17 09:59:33.000000 sabotage-0.2.1/README.md
--rw-r--r--   0 root         (0) root         (0)      848 2019-03-17 09:59:33.000000 sabotage-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:41:14.455606 sabotage-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 20:41:06.000000 sabotage-1.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-25 20:41:14.455606 sabotage-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-25 20:41:06.000000 sabotage-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:41:14.451606 sabotage-1.0.0/sabotage/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-25 20:41:06.000000 sabotage-1.0.0/sabotage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-04-25 20:41:06.000000 sabotage-1.0.0/sabotage/_docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-25 20:41:06.000000 sabotage-1.0.0/sabotage/_sabotaged_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-25 20:41:06.000000 sabotage-1.0.0/sabotage/_sabotaged_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 20:41:06.000000 sabotage-1.0.0/sabotage/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:41:14.455606 sabotage-1.0.0/sabotage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-25 20:41:14.000000 sabotage-1.0.0/sabotage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-25 20:41:14.000000 sabotage-1.0.0/sabotage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 20:41:14.000000 sabotage-1.0.0/sabotage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 20:41:14.000000 sabotage-1.0.0/sabotage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 20:41:14.000000 sabotage-1.0.0/sabotage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-25 20:41:14.455606 sabotage-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-25 20:41:06.000000 sabotage-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:41:14.455606 sabotage-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-25 20:41:06.000000 sabotage-1.0.0/tests/test_sabotaged_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-25 20:41:06.000000 sabotage-1.0.0/tests/test_sabotaged_network.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```


# Comparing `tmp/types-gevent-24.2.0.20240315.tar.gz` & `tmp/types-gevent-24.2.0.20240425.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-gevent-24.2.0.20240315.tar", last modified: Fri Mar 15 02:14:14 2024, max compression
+gzip compressed data, was "types-gevent-24.2.0.20240425.tar", last modified: Thu Apr 25 02:19:29 2024, max compression
```

## Comparing `types-gevent-24.2.0.20240315.tar` & `types-gevent-24.2.0.20240425.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:14:14.166064 types-gevent-24.2.0.20240315/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-15 02:14:13.000000 types-gevent-24.2.0.20240315/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-15 02:14:13.000000 types-gevent-24.2.0.20240315/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-03-15 02:14:14.166064 types-gevent-24.2.0.20240315/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:14:14.162064 types-gevent-24.2.0.20240315/gevent-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-15 02:14:13.000000 types-gevent-24.2.0.20240315/gevent-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/_abstract_linkable.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/_config.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:14:14.162064 types-gevent-24.2.0.20240315/gevent-stubs/_ffi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/_ffi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/_ffi/loop.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/_ffi/watcher.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/_fileobjectcommon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/_greenlet_primitives.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/_hub_local.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/_hub_primitives.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/_ident.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/_imap.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/_monitor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/_threading.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/_types.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/_waiter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/ares.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/backdoor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/baseserver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/event.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/fileobject.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/greenlet.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/hub.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:14:14.162064 types-gevent-24.2.0.20240315/gevent-stubs/libev/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/libev/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/libev/corecext.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/libev/corecffi.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/libev/watcher.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:14:14.162064 types-gevent-24.2.0.20240315/gevent-stubs/libuv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/libuv/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/libuv/loop.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/libuv/watcher.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/local.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/lock.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/monkey.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/os.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/pool.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/pywsgi.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/queue.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:14:14.162064 types-gevent-24.2.0.20240315/gevent-stubs/resolver/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/resolver/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/resolver/ares.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/resolver/blocking.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/resolver/cares.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/resolver/dnspython.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/resolver/thread.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/resolver_ares.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/resolver_thread.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/select.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/selectors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/server.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/signal.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/socket.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/ssl.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/subprocess.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/threadpool.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/time.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/timeout.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-15 02:13:51.000000 types-gevent-24.2.0.20240315/gevent-stubs/win32util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 02:14:14.166064 types-gevent-24.2.0.20240315/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-03-15 02:14:13.000000 types-gevent-24.2.0.20240315/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 02:14:14.162064 types-gevent-24.2.0.20240315/types_gevent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-03-15 02:14:14.000000 types-gevent-24.2.0.20240315/types_gevent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-03-15 02:14:14.000000 types-gevent-24.2.0.20240315/types_gevent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 02:14:14.000000 types-gevent-24.2.0.20240315/types_gevent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-15 02:14:14.000000 types-gevent-24.2.0.20240315/types_gevent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-15 02:14:14.000000 types-gevent-24.2.0.20240315/types_gevent.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:29.634902 types-gevent-24.2.0.20240425/
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-25 02:19:29.000000 types-gevent-24.2.0.20240425/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 02:19:29.000000 types-gevent-24.2.0.20240425/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-25 02:19:29.634902 types-gevent-24.2.0.20240425/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:29.630902 types-gevent-24.2.0.20240425/gevent-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-25 02:19:29.000000 types-gevent-24.2.0.20240425/gevent-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/_abstract_linkable.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/_config.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:29.634902 types-gevent-24.2.0.20240425/gevent-stubs/_ffi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/_ffi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/_ffi/loop.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/_ffi/watcher.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11765 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/_fileobjectcommon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/_greenlet_primitives.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/_hub_local.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/_hub_primitives.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/_ident.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/_imap.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/_monitor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/_threading.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/_types.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/_waiter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/ares.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/backdoor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/baseserver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/event.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/fileobject.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/greenlet.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/hub.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:29.634902 types-gevent-24.2.0.20240425/gevent-stubs/libev/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/libev/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/libev/corecext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/libev/corecffi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/libev/watcher.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:29.634902 types-gevent-24.2.0.20240425/gevent-stubs/libuv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/libuv/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/libuv/loop.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/libuv/watcher.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/local.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/lock.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/monkey.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/os.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/pool.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:29.000000 types-gevent-24.2.0.20240425/gevent-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/pywsgi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/queue.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:29.634902 types-gevent-24.2.0.20240425/gevent-stubs/resolver/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/resolver/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/resolver/ares.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/resolver/blocking.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/resolver/cares.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/resolver/dnspython.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/resolver/thread.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/resolver_ares.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/resolver_thread.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/select.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/selectors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/server.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/signal.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/socket.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/ssl.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/subprocess.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/threadpool.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/time.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/timeout.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-25 02:18:23.000000 types-gevent-24.2.0.20240425/gevent-stubs/win32util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 02:19:29.634902 types-gevent-24.2.0.20240425/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-25 02:19:29.000000 types-gevent-24.2.0.20240425/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:29.634902 types-gevent-24.2.0.20240425/types_gevent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-25 02:19:29.000000 types-gevent-24.2.0.20240425/types_gevent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-25 02:19:29.000000 types-gevent-24.2.0.20240425/types_gevent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 02:19:29.000000 types-gevent-24.2.0.20240425/types_gevent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 02:19:29.000000 types-gevent-24.2.0.20240425/types_gevent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 02:19:29.000000 types-gevent-24.2.0.20240425/types_gevent.egg-info/top_level.txt
```

### Comparing `types-gevent-24.2.0.20240315/CHANGELOG.md` & `types-gevent-24.2.0.20240425/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 24.2.0.20240425 (2024-04-25)
+
+Bump pyright to v1.1.360 (#11810)
+
 ## 24.2.0.20240315 (2024-03-15)
 
 chore(deps): update pytype and pyright (#11595)
 
 ## 24.2.0.20240311 (2024-03-11)
 
 Use Python 3.11 for third-party stubtest in CI (#11562)
```

### Comparing `types-gevent-24.2.0.20240315/PKG-INFO` & `types-gevent-24.2.0.20240425/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-gevent
-Version: 24.2.0.20240315
+Version: 24.2.0.20240425
 Summary: Typing stubs for gevent
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/gevent.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-gevent` aims to provide accurate annotations
 for `gevent==24.2.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/gevent. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `449f70f1f1bc787eb56699a5ce153c3efbfe2f4f` and was tested
-with mypy 1.9.0, pyright 1.1.354, and
-pytype 2024.3.11.
+This package was generated from typeshed commit `273e9ea6ddc2d5cad2db7dd25a0383a61be15675` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
+pytype 2024.4.11.
```

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/METADATA.toml` & `types-gevent-24.2.0.20240425/gevent-stubs/METADATA.toml`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/__init__.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/_config.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/_config.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/_ffi/loop.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/_ffi/loop.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/_ffi/watcher.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/_ffi/watcher.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/_fileobjectcommon.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/_fileobjectcommon.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,17 @@
     def opened_raw(self) -> FileIO: ...
     @staticmethod
     def is_buffered(stream: object) -> bool: ...
     @classmethod
     def buffer_size_for_stream(cls, stream: object) -> int: ...
 
 class FileObjectBase(Generic[_IOT, AnyStr]):
-    def __init__(self: FileObjectBase[_IOT, AnyStr], descriptor: OpenDescriptor[_IOT]) -> None: ...
+    def __init__(
+        self: FileObjectBase[_IOT, AnyStr], descriptor: OpenDescriptor[_IOT]  # pyright: ignore[reportInvalidTypeVarUse]  #11780
+    ) -> None: ...
     io: _IOT
     @property
     def closed(self) -> bool: ...
     def close(self) -> None: ...
     def __getattr__(self, name: str) -> Any: ...
     def __enter__(self) -> Self: ...
     def __exit__(self, typ: type[BaseException] | None, value: BaseException | None, tb: TracebackType | None, /) -> None: ...
```

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/_hub_primitives.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/_hub_primitives.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/_imap.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/_imap.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/_monitor.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/_monitor.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/_threading.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/_threading.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/_types.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/_types.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/_util.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/_util.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,17 @@
     @overload
     def __get__(self, inst: None, class_: type[object]) -> Self: ...
     @overload
     def __get__(self, inst: object, class_: type[object]) -> _T: ...
 
 class readproperty(Generic[_T]):
     func: Callable[[Any], _T]
-    def __init__(self: readproperty[_T], func: Callable[[Any], _T]) -> None: ...
+    def __init__(
+        self: readproperty[_T], func: Callable[[Any], _T]  # pyright: ignore[reportInvalidTypeVarUse]  #11780
+    ) -> None: ...
     @overload
     def __get__(self, inst: None, class_: type[object]) -> Self: ...
     @overload
     def __get__(self, inst: object, class_: type[object]) -> _T: ...
 
 class LazyOnClass(Generic[_T]):
     @classmethod
```

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/_waiter.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/_waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/backdoor.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/backdoor.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/baseserver.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/baseserver.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/event.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/event.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/events.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/events.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/fileobject.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/fileobject.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/greenlet.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/greenlet.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,20 @@
 class Greenlet(greenlet.greenlet, Generic[_P, _T]):
     # we can't use _P.args/_P.kwargs here because pyright will complain
     # mypy doesn't seem to mind though
     args: tuple[Any, ...]
     kwargs: dict[str, Any]
     value: _T | None
     @overload
-    def __init__(self: Greenlet[_P, _T], run: Callable[_P, _T], *args: _P.args, **kwargs: _P.kwargs) -> None: ...
+    def __init__(
+        self: Greenlet[_P, _T],  # pyright: ignore[reportInvalidTypeVarUse]  #11780
+        run: Callable[_P, _T],
+        *args: _P.args,
+        **kwargs: _P.kwargs,
+    ) -> None: ...
     @overload
     def __init__(self: Greenlet[[], None]) -> None: ...
     @readproperty
     def name(self) -> str: ...
     @property
     def minimal_ident(self) -> int: ...
     @property
```

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/hub.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/hub.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/libev/corecext.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/libev/corecext.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/libev/corecffi.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/libev/corecffi.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/libev/watcher.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/libev/watcher.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/libuv/loop.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/libuv/loop.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/libuv/watcher.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/libuv/watcher.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/lock.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/lock.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/monkey.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/monkey.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/os.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/os.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/pool.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/pool.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/pywsgi.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/pywsgi.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/queue.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/queue.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/resolver/__init__.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/resolver/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/resolver/ares.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/resolver/ares.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/resolver/blocking.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/resolver/blocking.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/resolver/cares.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/resolver/cares.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/resolver/thread.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/resolver/thread.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/selectors.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/selectors.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/server.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/server.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/signal.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/signal.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/socket.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/socket.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/ssl.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/ssl.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/threadpool.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/threadpool.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/timeout.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/timeout.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/gevent-stubs/util.pyi` & `types-gevent-24.2.0.20240425/gevent-stubs/util.pyi`

 * *Files identical despite different names*

### Comparing `types-gevent-24.2.0.20240315/setup.py` & `types-gevent-24.2.0.20240425/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,34 +17,34 @@
 This version of `types-gevent` aims to provide accurate annotations
 for `gevent==24.2.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/gevent. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `449f70f1f1bc787eb56699a5ce153c3efbfe2f4f` and was tested
-with mypy 1.9.0, pyright 1.1.354, and
-pytype 2024.3.11.
+This package was generated from typeshed commit `273e9ea6ddc2d5cad2db7dd25a0383a61be15675` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="24.2.0.20240315",
+      version="24.2.0.20240425",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/gevent.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=['types-greenlet', 'types-psutil'],
       packages=['gevent-stubs'],
-      package_data={'gevent-stubs': ['__init__.pyi', '_abstract_linkable.pyi', '_config.pyi', '_ffi/__init__.pyi', '_ffi/loop.pyi', '_ffi/watcher.pyi', '_fileobjectcommon.pyi', '_greenlet_primitives.pyi', '_hub_local.pyi', '_hub_primitives.pyi', '_ident.pyi', '_imap.pyi', '_monitor.pyi', '_threading.pyi', '_types.pyi', '_util.pyi', '_waiter.pyi', 'ares.pyi', 'backdoor.pyi', 'baseserver.pyi', 'event.pyi', 'events.pyi', 'exceptions.pyi', 'fileobject.pyi', 'greenlet.pyi', 'hub.pyi', 'libev/__init__.pyi', 'libev/corecext.pyi', 'libev/corecffi.pyi', 'libev/watcher.pyi', 'libuv/__init__.pyi', 'libuv/loop.pyi', 'libuv/watcher.pyi', 'local.pyi', 'lock.pyi', 'monkey.pyi', 'os.pyi', 'pool.pyi', 'pywsgi.pyi', 'queue.pyi', 'resolver/__init__.pyi', 'resolver/ares.pyi', 'resolver/blocking.pyi', 'resolver/cares.pyi', 'resolver/dnspython.pyi', 'resolver/thread.pyi', 'resolver_ares.pyi', 'resolver_thread.pyi', 'select.pyi', 'selectors.pyi', 'server.pyi', 'signal.pyi', 'socket.pyi', 'ssl.pyi', 'subprocess.pyi', 'threadpool.pyi', 'time.pyi', 'timeout.pyi', 'util.pyi', 'win32util.pyi', 'METADATA.toml']},
+      package_data={'gevent-stubs': ['__init__.pyi', '_abstract_linkable.pyi', '_config.pyi', '_ffi/__init__.pyi', '_ffi/loop.pyi', '_ffi/watcher.pyi', '_fileobjectcommon.pyi', '_greenlet_primitives.pyi', '_hub_local.pyi', '_hub_primitives.pyi', '_ident.pyi', '_imap.pyi', '_monitor.pyi', '_threading.pyi', '_types.pyi', '_util.pyi', '_waiter.pyi', 'ares.pyi', 'backdoor.pyi', 'baseserver.pyi', 'event.pyi', 'events.pyi', 'exceptions.pyi', 'fileobject.pyi', 'greenlet.pyi', 'hub.pyi', 'libev/__init__.pyi', 'libev/corecext.pyi', 'libev/corecffi.pyi', 'libev/watcher.pyi', 'libuv/__init__.pyi', 'libuv/loop.pyi', 'libuv/watcher.pyi', 'local.pyi', 'lock.pyi', 'monkey.pyi', 'os.pyi', 'pool.pyi', 'pywsgi.pyi', 'queue.pyi', 'resolver/__init__.pyi', 'resolver/ares.pyi', 'resolver/blocking.pyi', 'resolver/cares.pyi', 'resolver/dnspython.pyi', 'resolver/thread.pyi', 'resolver_ares.pyi', 'resolver_thread.pyi', 'select.pyi', 'selectors.pyi', 'server.pyi', 'signal.pyi', 'socket.pyi', 'ssl.pyi', 'subprocess.pyi', 'threadpool.pyi', 'time.pyi', 'timeout.pyi', 'util.pyi', 'win32util.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-gevent-24.2.0.20240315/types_gevent.egg-info/PKG-INFO` & `types-gevent-24.2.0.20240425/types_gevent.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-gevent
-Version: 24.2.0.20240315
+Version: 24.2.0.20240425
 Summary: Typing stubs for gevent
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/gevent.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-gevent` aims to provide accurate annotations
 for `gevent==24.2.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/gevent. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `449f70f1f1bc787eb56699a5ce153c3efbfe2f4f` and was tested
-with mypy 1.9.0, pyright 1.1.354, and
-pytype 2024.3.11.
+This package was generated from typeshed commit `273e9ea6ddc2d5cad2db7dd25a0383a61be15675` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
+pytype 2024.4.11.
```

### Comparing `types-gevent-24.2.0.20240315/types_gevent.egg-info/SOURCES.txt` & `types-gevent-24.2.0.20240425/types_gevent.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 gevent-stubs/greenlet.pyi
 gevent-stubs/hub.pyi
 gevent-stubs/local.pyi
 gevent-stubs/lock.pyi
 gevent-stubs/monkey.pyi
 gevent-stubs/os.pyi
 gevent-stubs/pool.pyi
+gevent-stubs/py.typed
 gevent-stubs/pywsgi.pyi
 gevent-stubs/queue.pyi
 gevent-stubs/resolver_ares.pyi
 gevent-stubs/resolver_thread.pyi
 gevent-stubs/select.pyi
 gevent-stubs/selectors.pyi
 gevent-stubs/server.pyi
```


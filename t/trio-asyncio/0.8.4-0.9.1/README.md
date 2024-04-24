# Comparing `tmp/trio_asyncio-0.8.4.tar.gz` & `tmp/trio_asyncio-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trio_asyncio-0.8.4.tar", last modified: Sat Aug 25 18:39:34 2018, max compression
+gzip compressed data, was "dist/trio_asyncio-0.9.1.tar", last modified: Fri Sep  7 06:43:21 2018, max compression
```

## Comparing `trio_asyncio-0.8.4.tar` & `trio_asyncio-0.9.1.tar`

### file list

```diff
@@ -1,72 +1,70 @@
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-08-25 18:39:34.000000 trio_asyncio-0.8.4/
--rw-r--r--   0 smurf      (501) smurf      (501)     2957 2018-08-25 18:34:26.000000 trio_asyncio-0.8.4/README.rst
--rw-r--r--   0 smurf      (501) smurf      (501)      172 2018-08-25 18:39:34.000000 trio_asyncio-0.8.4/setup.cfg
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-08-25 18:39:34.000000 trio_asyncio-0.8.4/trio_asyncio/
--rw-r--r--   0 smurf      (501) smurf      (501)     7808 2018-07-23 19:54:11.000000 trio_asyncio-0.8.4/trio_asyncio/sync.py
--rw-r--r--   0 smurf      (501) smurf      (501)      240 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/trio_asyncio/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3207 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/trio_asyncio/fd_stream.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3462 2018-08-13 09:36:44.000000 trio_asyncio-0.8.4/trio_asyncio/util.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3905 2018-08-25 09:39:06.000000 trio_asyncio-0.8.4/trio_asyncio/async_.py
--rw-r--r--   0 smurf      (501) smurf      (501)     5262 2018-08-25 12:44:42.000000 trio_asyncio-0.8.4/trio_asyncio/handles.py
--rw-r--r--   0 smurf      (501) smurf      (501)    11057 2018-08-13 09:36:44.000000 trio_asyncio-0.8.4/trio_asyncio/loop.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4597 2018-07-23 19:51:53.000000 trio_asyncio-0.8.4/trio_asyncio/child.py
--rw-r--r--   0 smurf      (501) smurf      (501)    27889 2018-08-25 13:28:06.000000 trio_asyncio-0.8.4/trio_asyncio/base.py
--rw-r--r--   0 smurf      (501) smurf      (501)       89 2018-08-25 18:38:03.000000 trio_asyncio-0.8.4/trio_asyncio/_version.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3244 2018-08-25 12:44:43.000000 trio_asyncio-0.8.4/trio_asyncio/adapter.py
--rw-r--r--   0 smurf      (501) smurf      (501)       82 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/MANIFEST.in
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-08-25 18:39:34.000000 trio_asyncio-0.8.4/trio_asyncio.egg-info/
--rw-r--r--   0 smurf      (501) smurf      (501)       58 2018-08-25 18:39:34.000000 trio_asyncio-0.8.4/trio_asyncio.egg-info/requires.txt
--rw-r--r--   0 smurf      (501) smurf      (501)     1650 2018-08-25 18:39:34.000000 trio_asyncio-0.8.4/trio_asyncio.egg-info/SOURCES.txt
--rw-r--r--   0 smurf      (501) smurf      (501)       19 2018-08-25 18:39:34.000000 trio_asyncio-0.8.4/trio_asyncio.egg-info/top_level.txt
--rw-r--r--   0 smurf      (501) smurf      (501)        1 2018-08-25 18:39:34.000000 trio_asyncio-0.8.4/trio_asyncio.egg-info/dependency_links.txt
--rw-r--r--   0 smurf      (501) smurf      (501)     3053 2018-08-25 18:39:34.000000 trio_asyncio-0.8.4/trio_asyncio.egg-info/PKG-INFO
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-08-25 18:39:34.000000 trio_asyncio-0.8.4/tests/
--rw-r--r--   0 smurf      (501) smurf      (501)    17459 2018-08-25 17:38:02.000000 trio_asyncio-0.8.4/tests/utils.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-08-25 18:39:34.000000 trio_asyncio-0.8.4/tests/interop/
--rw-r--r--   0 smurf      (501) smurf      (501)        0 2018-08-25 16:40:20.000000 trio_asyncio-0.8.4/tests/interop/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1147 2018-08-25 12:39:24.000000 trio_asyncio-0.8.4/tests/interop/test_adapter.py
--rw-r--r--   0 smurf      (501) smurf      (501)    11168 2018-08-25 16:37:51.000000 trio_asyncio-0.8.4/tests/interop/test_calls.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-08-25 18:39:34.000000 trio_asyncio-0.8.4/tests/aiotest/
--rw-r--r--   0 smurf      (501) smurf      (501)     1339 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/tests/aiotest/test_coroutine.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2545 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/tests/aiotest/test_network.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1955 2018-08-03 11:54:25.000000 trio_asyncio-0.8.4/tests/aiotest/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2399 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/tests/aiotest/test_add_reader.py
--rw-r--r--   0 smurf      (501) smurf      (501)       95 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/tests/aiotest/conftest.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2796 2018-08-03 10:58:37.000000 trio_asyncio-0.8.4/tests/aiotest/test_callback.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2941 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/tests/aiotest/test_thread.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1187 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/tests/aiotest/test_timer.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1036 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/tests/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3785 2018-08-13 08:57:46.000000 trio_asyncio-0.8.4/tests/test_misc.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1705 2018-08-25 13:23:42.000000 trio_asyncio-0.8.4/tests/conftest.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2521 2018-08-03 11:23:13.000000 trio_asyncio-0.8.4/tests/test_concurrent.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-08-25 18:39:34.000000 trio_asyncio-0.8.4/tests/python/
--rw-r--r--   0 smurf      (501) smurf      (501)     3356 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/tests/python/test_transports.py
--rw-r--r--   0 smurf      (501) smurf      (501)    63734 2018-08-03 11:23:15.000000 trio_asyncio-0.8.4/tests/python/test_base_events.py
--rw-r--r--   0 smurf      (501) smurf      (501)    53470 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/tests/python/test_unix_events.py
--rw-r--r--   0 smurf      (501) smurf      (501)    88382 2018-08-25 13:28:22.000000 trio_asyncio-0.8.4/tests/python/test_tasks.py
--rw-r--r--   0 smurf      (501) smurf      (501)    19149 2018-08-03 09:22:08.000000 trio_asyncio-0.8.4/tests/python/test_subprocess.py
--rw-r--r--   0 smurf      (501) smurf      (501)      148 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/tests/python/echo.py
--rw-r--r--   0 smurf      (501) smurf      (501)     5084 2018-08-25 09:38:59.000000 trio_asyncio-0.8.4/tests/python/test_windows_utils.py
--rw-r--r--   0 smurf      (501) smurf      (501)      127 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/tests/python/echo2.py
--rw-r--r--   0 smurf      (501) smurf      (501)       72 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/tests/python/__main__.py
--rw-r--r--   0 smurf      (501) smurf      (501)    31908 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/tests/python/test_streams.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4996 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/tests/python/test_sslproto.py
--rw-r--r--   0 smurf      (501) smurf      (501)      341 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/tests/python/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)   100570 2018-08-03 12:07:09.000000 trio_asyncio-0.8.4/tests/python/test_events.py
--rw-r--r--   0 smurf      (501) smurf      (501)      867 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/tests/python/ssl_cert.pem
--rw-r--r--   0 smurf      (501) smurf      (501)    69074 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/tests/python/test_selector_events.py
--rw-r--r--   0 smurf      (501) smurf      (501)    18385 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/tests/python/test_queues.py
--rw-r--r--   0 smurf      (501) smurf      (501)    22474 2018-08-25 13:27:52.000000 trio_asyncio-0.8.4/tests/python/test_futures.py
--rw-r--r--   0 smurf      (501) smurf      (501)    21721 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/tests/python/test_proactor_events.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4307 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/tests/python/pycacert.pem
--rw-r--r--   0 smurf      (501) smurf      (501)      278 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/tests/python/echo3.py
--rw-r--r--   0 smurf      (501) smurf      (501)     5462 2018-08-25 09:39:05.000000 trio_asyncio-0.8.4/tests/python/test_windows_events.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4050 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/tests/python/keycert3.pem
--rw-r--r--   0 smurf      (501) smurf      (501)    27496 2018-08-25 17:36:44.000000 trio_asyncio-0.8.4/tests/python/test_locks.py
--rw-r--r--   0 smurf      (501) smurf      (501)      916 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/tests/python/ssl_key.pem
--rw-r--r--   0 smurf      (501) smurf      (501)     6956 2018-04-23 11:57:02.000000 trio_asyncio-0.8.4/tests/python/test_pep492.py
--rw-r--r--   0 smurf      (501) smurf      (501)      394 2018-08-03 11:23:13.000000 trio_asyncio-0.8.4/tests/test_sync.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-08-25 18:39:34.000000 trio_asyncio-0.8.4/ci/
--rw-r--r--   0 smurf      (501) smurf      (501)      121 2018-07-23 20:30:01.000000 trio_asyncio-0.8.4/ci/test-requirements.txt
--rw-r--r--   0 smurf      (501) smurf      (501)     3053 2018-08-25 18:39:34.000000 trio_asyncio-0.8.4/PKG-INFO
--rw-r--r--   0 smurf      (501) smurf      (501)     3410 2018-08-25 18:37:53.000000 trio_asyncio-0.8.4/setup.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-09-07 06:43:21.000000 trio_asyncio-0.9.1/
+-rw-r--r--   0 smurf      (501) smurf      (501)     2957 2018-08-25 18:34:26.000000 trio_asyncio-0.9.1/README.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)      172 2018-09-07 06:43:21.000000 trio_asyncio-0.9.1/setup.cfg
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-09-07 06:43:21.000000 trio_asyncio-0.9.1/trio_asyncio/
+-rw-r--r--   0 smurf      (501) smurf      (501)     7808 2018-07-23 19:54:11.000000 trio_asyncio-0.9.1/trio_asyncio/sync.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      240 2018-04-23 11:57:02.000000 trio_asyncio-0.9.1/trio_asyncio/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3207 2018-04-23 11:57:02.000000 trio_asyncio-0.9.1/trio_asyncio/fd_stream.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4087 2018-08-31 08:26:54.000000 trio_asyncio-0.9.1/trio_asyncio/util.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3883 2018-08-31 17:21:58.000000 trio_asyncio-0.9.1/trio_asyncio/async_.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     5523 2018-08-31 12:07:28.000000 trio_asyncio-0.9.1/trio_asyncio/handles.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    11206 2018-08-31 08:26:54.000000 trio_asyncio-0.9.1/trio_asyncio/loop.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4597 2018-07-23 19:51:53.000000 trio_asyncio-0.9.1/trio_asyncio/child.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    27559 2018-08-31 17:41:24.000000 trio_asyncio-0.9.1/trio_asyncio/base.py
+-rw-r--r--   0 smurf      (501) smurf      (501)       89 2018-09-06 08:21:52.000000 trio_asyncio-0.9.1/trio_asyncio/_version.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     8473 2018-09-06 09:10:41.000000 trio_asyncio-0.9.1/trio_asyncio/adapter.py
+-rw-r--r--   0 smurf      (501) smurf      (501)       82 2018-04-23 11:57:02.000000 trio_asyncio-0.9.1/MANIFEST.in
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-09-07 06:43:21.000000 trio_asyncio-0.9.1/trio_asyncio.egg-info/
+-rw-r--r--   0 smurf      (501) smurf      (501)       58 2018-09-07 06:43:21.000000 trio_asyncio-0.9.1/trio_asyncio.egg-info/requires.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)     1614 2018-09-07 06:43:21.000000 trio_asyncio-0.9.1/trio_asyncio.egg-info/SOURCES.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)       19 2018-09-07 06:43:21.000000 trio_asyncio-0.9.1/trio_asyncio.egg-info/top_level.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)        1 2018-09-07 06:43:21.000000 trio_asyncio-0.9.1/trio_asyncio.egg-info/dependency_links.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)     3053 2018-09-07 06:43:21.000000 trio_asyncio-0.9.1/trio_asyncio.egg-info/PKG-INFO
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-09-07 06:43:21.000000 trio_asyncio-0.9.1/tests/
+-rw-r--r--   0 smurf      (501) smurf      (501)    17456 2018-08-31 08:26:41.000000 trio_asyncio-0.9.1/tests/utils.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-09-07 06:43:21.000000 trio_asyncio-0.9.1/tests/interop/
+-rw-r--r--   0 smurf      (501) smurf      (501)        0 2018-08-25 16:40:20.000000 trio_asyncio-0.9.1/tests/interop/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     8656 2018-08-31 08:32:20.000000 trio_asyncio-0.9.1/tests/interop/test_adapter.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    19370 2018-08-31 08:31:41.000000 trio_asyncio-0.9.1/tests/interop/test_calls.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    12263 2018-08-31 19:09:28.000000 trio_asyncio-0.9.1/tests/test_aio_subprocess.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-09-07 06:43:21.000000 trio_asyncio-0.9.1/tests/aiotest/
+-rw-r--r--   0 smurf      (501) smurf      (501)     2334 2018-08-29 08:05:43.000000 trio_asyncio-0.9.1/tests/aiotest/test_coroutine.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2545 2018-04-23 11:57:02.000000 trio_asyncio-0.9.1/tests/aiotest/test_network.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1944 2018-08-31 08:29:19.000000 trio_asyncio-0.9.1/tests/aiotest/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2399 2018-04-23 11:57:02.000000 trio_asyncio-0.9.1/tests/aiotest/test_add_reader.py
+-rw-r--r--   0 smurf      (501) smurf      (501)       95 2018-04-23 11:57:02.000000 trio_asyncio-0.9.1/tests/aiotest/conftest.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3011 2018-08-28 09:48:30.000000 trio_asyncio-0.9.1/tests/aiotest/test_callback.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4818 2018-08-28 09:52:32.000000 trio_asyncio-0.9.1/tests/aiotest/test_thread.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1187 2018-04-23 11:57:02.000000 trio_asyncio-0.9.1/tests/aiotest/test_timer.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1036 2018-04-23 11:57:02.000000 trio_asyncio-0.9.1/tests/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     9747 2018-08-31 19:26:15.000000 trio_asyncio-0.9.1/tests/test_misc.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1670 2018-08-31 08:32:30.000000 trio_asyncio-0.9.1/tests/conftest.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2521 2018-08-03 11:23:13.000000 trio_asyncio-0.9.1/tests/test_concurrent.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-09-07 06:43:21.000000 trio_asyncio-0.9.1/tests/python/
+-rw-r--r--   0 smurf      (501) smurf      (501)     3356 2018-04-23 11:57:02.000000 trio_asyncio-0.9.1/tests/python/test_transports.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    63734 2018-08-03 11:23:15.000000 trio_asyncio-0.9.1/tests/python/test_base_events.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    53470 2018-04-23 11:57:02.000000 trio_asyncio-0.9.1/tests/python/test_unix_events.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    88204 2018-08-31 16:51:38.000000 trio_asyncio-0.9.1/tests/python/test_tasks.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    19149 2018-08-03 09:22:08.000000 trio_asyncio-0.9.1/tests/python/test_subprocess.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     5058 2018-08-31 08:29:29.000000 trio_asyncio-0.9.1/tests/python/test_windows_utils.py
+-rw-r--r--   0 smurf      (501) smurf      (501)       72 2018-04-23 11:57:02.000000 trio_asyncio-0.9.1/tests/python/__main__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    31908 2018-04-23 11:57:02.000000 trio_asyncio-0.9.1/tests/python/test_streams.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4996 2018-04-23 11:57:02.000000 trio_asyncio-0.9.1/tests/python/test_sslproto.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      341 2018-04-23 11:57:02.000000 trio_asyncio-0.9.1/tests/python/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    87452 2018-08-31 08:29:51.000000 trio_asyncio-0.9.1/tests/python/test_events.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      867 2018-04-23 11:57:02.000000 trio_asyncio-0.9.1/tests/python/ssl_cert.pem
+-rw-r--r--   0 smurf      (501) smurf      (501)    69074 2018-04-23 11:57:02.000000 trio_asyncio-0.9.1/tests/python/test_selector_events.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    18385 2018-04-23 11:57:02.000000 trio_asyncio-0.9.1/tests/python/test_queues.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    22474 2018-08-25 13:27:52.000000 trio_asyncio-0.9.1/tests/python/test_futures.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    21721 2018-04-23 11:57:02.000000 trio_asyncio-0.9.1/tests/python/test_proactor_events.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4307 2018-04-23 11:57:02.000000 trio_asyncio-0.9.1/tests/python/pycacert.pem
+-rw-r--r--   0 smurf      (501) smurf      (501)     5462 2018-08-25 09:39:05.000000 trio_asyncio-0.9.1/tests/python/test_windows_events.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4050 2018-04-23 11:57:02.000000 trio_asyncio-0.9.1/tests/python/keycert3.pem
+-rw-r--r--   0 smurf      (501) smurf      (501)    27497 2018-08-31 08:26:54.000000 trio_asyncio-0.9.1/tests/python/test_locks.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      916 2018-04-23 11:57:02.000000 trio_asyncio-0.9.1/tests/python/ssl_key.pem
+-rw-r--r--   0 smurf      (501) smurf      (501)     6956 2018-04-23 11:57:02.000000 trio_asyncio-0.9.1/tests/python/test_pep492.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      380 2018-08-31 08:32:54.000000 trio_asyncio-0.9.1/tests/test_sync.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2018-09-07 06:43:21.000000 trio_asyncio-0.9.1/ci/
+-rw-r--r--   0 smurf      (501) smurf      (501)      121 2018-07-23 20:30:01.000000 trio_asyncio-0.9.1/ci/test-requirements.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)     3053 2018-09-07 06:43:21.000000 trio_asyncio-0.9.1/PKG-INFO
+-rw-r--r--   0 smurf      (501) smurf      (501)     3432 2018-08-31 08:33:57.000000 trio_asyncio-0.9.1/setup.py
```

### Comparing `trio_asyncio-0.8.4/README.rst` & `trio_asyncio-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/trio_asyncio/sync.py` & `trio_asyncio-0.9.1/trio_asyncio/sync.py`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/trio_asyncio/fd_stream.py` & `trio_asyncio-0.9.1/trio_asyncio/fd_stream.py`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/trio_asyncio/util.py` & `trio_asyncio-0.9.1/trio_asyncio/util.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # This code implements helper functions that work without running
 # a TrioEventLoop.
 
 import trio
 import asyncio
 import sys
 import outcome
+import sniffio
 from async_generator import async_generator, yield_
 
-__all__ = ['run_future']
+__all__ = ['run_aio_future', 'run_aio_generator']
 
 
-async def run_future(future):
+async def run_aio_future(future):
     """Wait for an asyncio future/coroutine from Trio code.
 
     Cancelling the current Trio scope will cancel the future/coroutine.
 
     Cancelling the future/coroutine will cause an ``asyncio.CancelledError``.
     """
     task = trio.hazmat.current_task()
@@ -49,30 +50,34 @@
             raise
 
 
 STOP = object()
 
 
 @async_generator
-async def run_generator(loop, async_generator):
+async def run_aio_generator(loop, async_generator):
+    """Run an asyncio generator from Trio"""
     task = trio.hazmat.current_task()
     raise_cancel = None
     current_read = None
 
     async def consume_next():
+        t = sniffio.current_async_library_cvar.set("asyncio")
         try:
             item = await async_generator.__anext__()
             result = outcome.Value(value=item)
         except StopAsyncIteration:
             result = outcome.Value(value=STOP)
         except asyncio.CancelledError:
             # Once we are cancelled, we do not call reschedule() anymore
             return
         except Exception as e:
             result = outcome.Error(error=e)
+        finally:
+            sniffio.current_async_library_cvar.reset(t)
 
         trio.hazmat.reschedule(task, result)
 
     def abort_cb(raise_cancel_arg):
         # Save the cancel-raising function
         nonlocal raise_cancel
         raise_cancel = raise_cancel_arg
@@ -109,7 +114,20 @@
                 raise_cancel()
             finally:
                 # Try to preserve the exception chain,
                 # for more detailed tracebacks
                 sys.exc_info()[1].__cause__ = exc
         else:
             raise
+
+
+@async_generator
+async def run_trio_generator(loop, async_generator):
+    """Run a Trio generator from within asyncio"""
+    while True:
+        # Schedule in asyncio that we read the next item from the iterator
+        try:
+            item = await loop.trio_as_future(async_generator.__anext__)
+        except StopAsyncIteration:
+            break
+        else:
+            await yield_(item)
```

### Comparing `trio_asyncio-0.8.4/trio_asyncio/async_.py` & `trio_asyncio-0.9.1/trio_asyncio/async_.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 
 __all__ = ['TrioEventLoop', 'open_loop']
 
 
 class TrioEventLoop(BaseTrioEventLoop):
     """A Trio-compatible asyncio event loop.
 
-    This loop runs in an async Trio context. If you really do need a
-    stand-alone implementation, use :class:`SyncTrioEventLoop`.
+    This loop runs in an async Trio context.
     """
 
     def _queue_handle(self, handle):
         self._check_closed()
         self._q.put_nowait(handle)
         return handle
 
@@ -119,12 +118,14 @@
             await loop._main_loop_init(nursery)
             await nursery.start(loop._main_loop)
             await yield_(loop)
         finally:
             try:
                 await loop.stop().wait()
             finally:
-                await loop._main_loop_exit()
-                loop.close()
-                nursery.cancel_scope.cancel()
-                current_loop.reset(old_loop)
-                current_policy.reset(old_policy)
+                try:
+                    await loop._main_loop_exit()
+                finally:
+                    loop.close()
+                    nursery.cancel_scope.cancel()
+                    current_loop.reset(old_loop)
+                    current_policy.reset(old_policy)
```

### Comparing `trio_asyncio-0.8.4/trio_asyncio/handles.py` & `trio_asyncio-0.9.1/trio_asyncio/handles.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,17 +42,26 @@
     def _init(self, is_sync):
         """Secondary init.
         """
         self._is_sync = is_sync
         self._scope = None
 
     def cancel(self):
+        try:
+            task = self._callback.__self__
+        except AttributeError:
+            task = None
+        else:
+            if not isinstance(task, asyncio.Task):
+                task = None
         super().cancel()
         if self._scope is not None:
             self._scope.cancel()
+        elif task is not None:
+            task.cancel()
 
     def _cb_future_cancel(self, f):
         """If a Trio task completes an asyncio Future,
         add this callback to the future
         and set ``_scope`` to the Trio cancel scope
         so that the task is terminated when the future gets canceled.
```

### Comparing `trio_asyncio-0.8.4/trio_asyncio/loop.py` & `trio_asyncio-0.9.1/trio_asyncio/loop.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # Trio.
 
 import sys
 import trio
 import asyncio
 import warnings
 import threading
-from contextvars import ContextVar
 
-from .util import run_future
+from .adapter import current_loop, current_policy
+from .util import run_aio_future
 from .async_ import TrioEventLoop, open_loop
 
 try:
     from trio.hazmat import wait_for_child
 except ImportError:
     from .child import wait_for_child
 
@@ -20,25 +20,24 @@
 logger = logging.getLogger(__name__)
 
 __all__ = [
     'run',
     'run_trio_task',
     'run_trio',
     'run_future',
-    'run_coroutine',
+    'run_aio_future',
+    'run_coroutine',  # deprecated
+    'run_aio_coroutine',
     'run_asyncio',
     'wrap_generator',
     'run_iterator',
     'TrioChildWatcher',
     'TrioPolicy',
 ]
 
-current_loop = ContextVar('trio_aio_loop', default=None)
-current_policy = ContextVar('trio_aio_policy', default=None)
-
 _faked_policy = threading.local()
 
 # We can monkey-patch asyncio's get_event_loop_policy but if asyncio is
 # imported before Trio, the asyncio acceleration C code in 3.7+ caches
 # get_event_loop_policy.
 # Thus we always set our policy. After that, our monkeypatched
 # setter stores the policy in a thread-local variable to which our policy
@@ -164,31 +163,35 @@
 
 
 _aio_event.set_event_loop_policy = _new_policy_set
 asyncio.set_event_loop_policy = _new_policy_set
 
 #####
 
-_orig_run_get = _aio_event._get_running_loop
+try:
+    _orig_run_get = _aio_event._get_running_loop
 
+except AttributeError:
+    pass
 
-def _new_run_get():
-    try:
-        task = trio.hazmat.current_task()
-    except RuntimeError:
-        loop = _orig_run_get()
-    else:
-        loop = task.context.get(current_loop, None)
-        if loop is None:
-            raise RuntimeError("No trio_asyncio loop is active.")
+else:
 
-    return loop
+    def _new_run_get():
+        try:
+            task = trio.hazmat.current_task()
+        except RuntimeError:
+            loop = _orig_run_get()
+        else:
+            loop = task.context.get(current_loop, None)
+            if loop is None:
+                raise RuntimeError("No trio_asyncio loop is active.")
 
+        return loop
 
-_aio_event._get_running_loop = _new_run_get
+    _aio_event._get_running_loop = _new_run_get
 
 #####
 
 _orig_loop_get = _aio_event.get_event_loop
 
 
 def _new_loop_get():
@@ -275,97 +278,111 @@
     def __exit__(self, *tb):
         self.close()
 
 
 def wrap_generator(proc, *args):
     """Run an asyncio generator from Trio.
     """
-    loop = asyncio.get_event_loop()
-    if not isinstance(loop, TrioEventLoop):
-        raise RuntimeError("Need to run in a trio_asyncio.open_loop() context")
+    loop = current_loop.get()
+    if loop is None:
+        raise RuntimeError("You are not within a trio_asyncio loop")
     return loop.wrap_generator(proc, *args)
 
 
 def run_iterator(aiter):
     """Run an asyncio iterator from Trio.
     """
-    loop = asyncio.get_event_loop()
-    if not isinstance(loop, TrioEventLoop):
-        raise RuntimeError("Need to run in a trio_asyncio.open_loop() context")
+    loop = current_loop.get()
+    if loop is None:
+        raise RuntimeError("You are not within a trio_asyncio loop")
     return loop.run_iterator(aiter)
 
 
 def wrap_trio_context(ctx):
     """Run a Trio context manager from asyncio.
     """
-    loop = asyncio.get_event_loop()
-    if not isinstance(loop, TrioEventLoop):
-        raise RuntimeError("Need to run in a trio_asyncio.open_loop() context")
+    loop = current_loop.get()
+    if loop is None:
+        raise RuntimeError("You are not within a trio_asyncio loop")
     return loop.wrap_trio_context(ctx)
 
 
 async def run_asyncio(proc, *args):
     """Run an asyncio function or method from Trio.
 
     :return: whatever the procedure returns.
     :raises: whatever the procedure raises.
 
     This is a Trio coroutine.
     """
 
-    loop = asyncio.get_event_loop()
-    if not isinstance(loop, TrioEventLoop):
-        raise RuntimeError("Need to run in a trio_asyncio.open_loop() context")
+    loop = current_loop.get()
+    if loop is None:
+        raise RuntimeError("You are not within a trio_asyncio loop")
     return await loop.run_asyncio(proc, *args)
 
 
-async def run_coroutine(fut):
+async def run_aio_coroutine(fut):
     """Wait for an asyncio future/coroutine.
 
     Cancelling the current Trio scope will cancel the future/coroutine.
 
     Cancelling the future/coroutine will cause an
     ``asyncio.CancelledError``.
 
     This is a Trio coroutine.
     """
 
-    loop = asyncio.get_event_loop()
-    if not isinstance(loop, TrioEventLoop):
-        raise RuntimeError("Need to run in a trio_asyncio.open_loop() context")
-    return await loop.run_coroutine(fut)
+    loop = current_loop.get()
+    if loop is None:
+        raise RuntimeError("You are not within a trio_asyncio loop")
+    return await loop.run_aio_coroutine(fut)
+
+
+async def run_coroutine(fut):
+    """ deprecated"""
+    loop = current_loop.get()
+    if loop is None:
+        raise RuntimeError("You are not within a trio_asyncio loop")
+    return await loop.run_aio_coroutine(fut)
+
+
+async def run_future(fut):
+    """ deprecated"""
+    warnings.warn("Use 'await run_aio_future(fut)' instead'", DeprecationWarning)
+    return await run_aio_future(fut)
 
 
 def run_trio(proc, *args):
     """Call an asynchronous Trio function from asyncio.
 
     Returns a Future with the result / exception.
 
     Cancelling the future will cancel the Trio task running your
     function, or prevent it from starting if that is still possible.
 
     You need to handle errors yourself.
     """
-    loop = asyncio.get_event_loop()
-    if not isinstance(loop, TrioEventLoop):  # pragma: no cover
-        raise RuntimeError("Need to run in a trio_asyncio.open_loop() context")
+    loop = current_loop.get()
+    if loop is None:
+        raise RuntimeError("You are not within a trio_asyncio loop")
     return loop.run_trio(proc, *args)
 
 
 def run_trio_task(proc, *args):
     """Call an asynchronous Trio function from sync context.
 
     This method queues the task and returns immediately.
     It does not return a value.
 
     An uncaught error will propagate to, and terminate, the trio-asyncio loop.
     """
-    loop = asyncio.get_event_loop()
-    if not isinstance(loop, TrioEventLoop):
-        raise RuntimeError("Need to run in a trio_asyncio.open_loop() context")
+    loop = current_loop.get()
+    if loop is None:
+        raise RuntimeError("You are not within a trio_asyncio loop")
     loop.run_trio_task(proc, *args)
 
 
 def run(proc, *args, queue_len=None):
     """Like :func:`trio.run`, but adds a context that supports asyncio.
     """
```

### Comparing `trio_asyncio-0.8.4/trio_asyncio/child.py` & `trio_asyncio-0.9.1/trio_asyncio/child.py`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/trio_asyncio/base.py` & `trio_asyncio-0.9.1/trio_asyncio/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 import math
 import trio
 import heapq
 import signal
 import sniffio
 import asyncio
 import warnings
+import concurrent.futures
 from contextvars import ContextVar
-from async_generator import asynccontextmanager
-from async_generator import async_generator, yield_
 
+from .adapter import Asyncio_Trio_Wrapper, Trio_Asyncio_Wrapper
 from .handles import Handle, TimerHandle
+from .util import run_aio_future, run_aio_generator
 
 from selectors import _BaseSelectorImpl, EVENT_READ, EVENT_WRITE
 
-from .util import run_future, run_generator
-
 try:
     from trio.hazmat import wait_for_child
 except ImportError:
     from .child import wait_for_child
 
 import logging
 logger = logging.getLogger(__name__)
@@ -76,15 +75,15 @@
     def select(self, timeout=None):  # pragma: no cover
         raise NotImplementedError
 
     def _select(self, r, w, x, timeout=None):  # pragma: no cover
         raise NotImplementedError
 
 
-class TrioExecutor:
+class TrioExecutor(concurrent.futures.ThreadPoolExecutor):
     """An executor that runs its job in a Trio worker thread."""
 
     def __init__(self, limiter=None, thread_name_prefix=None, max_workers=None):
         self._running = True
         if limiter is None and max_workers is not None:
             limiter = trio.CapacityLimiter(max_workers)
         self._limiter = limiter
@@ -197,120 +196,123 @@
         """Return Trio's idea of the current time.
         """
         if self._task is None:
             raise RuntimeError("This loop is closed.")
         return self._task._runner.clock.current_time()
 
     # A future doesn't require a trio_asyncio loop
-    run_future = staticmethod(run_future)
+    run_aio_future = staticmethod(run_aio_future)
+
+    def run_future(self, *args, **kwargs):
+        warnings.warn("Use 'await loop.run_aio_future(fut)' instead'", DeprecationWarning)
+        return self.run_aio_future(*args, **kwargs)
 
     # A coroutine (usually) does.
-    async def run_coroutine(self, coro):
+    def run_coroutine(self, coro):
+        warnings.warn("Use 'await loop.run_aio_coroutine(coro)' instead'", DeprecationWarning)
+
+        return self.run_aio_coroutine(coro)
+
+    async def run_aio_coroutine(self, coro):
         """Wait for an asyncio future/coroutine.
 
         Cancelling the current Trio scope will cancel the future/coroutine.
 
         Cancelling the future/coroutine will cause an
         ``asyncio.CancelledError``.
 
         This is a Trio coroutine.
         """
         self._check_closed()
         t = sniffio.current_async_library_cvar.set("asyncio")
         coro = asyncio.ensure_future(coro, loop=self)
         try:
-            return await run_future(coro)
+            return await run_aio_future(coro)
         finally:
             sniffio.current_async_library_cvar.reset(t)
 
     def wrap_generator(self, gen, *args):
         """Call an asyncio generator.
 
         Deprecated: instead of
 
             await loop.wrap_generator(gen, *args)
 
         simply call
 
-            await loop.run_asyncio(gen(*args))
+            await aio_as_trio(gen(*args), loop=loop)
         """
-        warnings.warn("Use 'run_asyncio(gen(*args))' instead'", DeprecationWarning)
+        warnings.warn("Use 'async with aio_as_trio(gen(*args))' instead'", DeprecationWarning)
 
-        return run_generator(self, gen(*args))
+        return run_aio_generator(self, gen(*args))
 
     def run_iterator(self, aiter):
         """Call an asyncio iterator from Trio.
 
         Deprecated: instead of
 
             await loop.run_iterator(iter)
 
         simply call
 
-            await loop.run_asyncio(iter)
+            await aio_as_trio(iter, loop=loop)
         """
-        warnings.warn("Use 'run_asyncio(iter)' instead'", DeprecationWarning)
+        warnings.warn("Use 'async for X in aio_as_trio(iter)' instead'", DeprecationWarning)
 
-        return run_generator(self, aiter)
-
-    @asynccontextmanager
-    @async_generator
-    async def wrap_trio_context(self, ctx):
-        """Run a Trio context manager from asyncio.
-        """
-        res = await self.run_trio(ctx.__aenter__)
-        try:
-            await yield_(res)
-        except BaseException as exc:
-            if not await self.run_trio(ctx.__aexit__, type(exc), exc, exc.__traceback__):
-                raise
-        else:
-            await self.run_trio(ctx.__aexit__, None, None, None)
+        return run_aio_generator(self, aiter)
 
     def run_asyncio(self, proc, *args):
         """Run an asyncio function or method from Trio.
 
         :return: whatever the procedure returns.
         :raises: whatever the procedure raises.
 
         This is (essentially) a Trio coroutine.
 
-        You can also use this for calling an asyncio-style
-        async iterator or async context manager.
+        Depreated; use
+
+            aio_as_trio(proc)(*args)
+
+        instead.
         """
 
-        class t2aWrapper:
-            def __await__(slf):
-                f = proc(*args)
-                return self.run_coroutine(f).__await__()
-
-            def __aenter__(slf):
-                proc_enter = getattr(proc, "__aenter__", None)
-                if proc_enter is None or args:
-                    raise RuntimeError(
-                        "Call 'run_asyncio(ctxfactory(*args))', not 'run_asyncio(ctxfactory, *args)'"
-                    )
-                f = proc_enter()
-                return self.run_coroutine(f)
-
-            def __aexit__(slf, *tb):
-                f = proc.__aexit__(*tb)
-                return self.run_coroutine(f)
-
-            def __aiter__(slf):
-                proc_iter = getattr(proc, "__anext__", None)
-                if proc_iter is None or args:
-                    raise RuntimeError(
-                        "Call 'run_asyncio(gen(*args))', not 'run_asyncio(gen, *args)'"
-                    )
-                return run_generator(self, proc)
+        warnings.warn("Use 'await aio_as_trio(proc)(*args)' instead'", DeprecationWarning)
 
-        return t2aWrapper()
+        return Asyncio_Trio_Wrapper(proc, args=args, loop=self)
+
+    def wrap_trio_context(self, ctx):
+        """Run a Trio context manager from asyncio.
+        """
+        warnings.warn("Use 'await trio_as_aio(context)' instead'", DeprecationWarning)
+        return Trio_Asyncio_Wrapper(ctx, loop=self)
 
     def run_trio(self, proc, *args):
+        warnings.warn("Use 'await trio_as_aio(proc)(*args)' instead'", DeprecationWarning)
+        return self.trio_as_future(proc, *args)
+
+    async def __run_trio(self, h):
+        """Helper for copying the result of a Trio task to an asyncio future"""
+        f, proc, *args = h._args
+        if f.cancelled():  # pragma: no cover
+            return
+        try:
+            with trio.open_cancel_scope() as scope:
+                h._scope = scope
+                res = await proc(*args)
+            if scope.cancelled_caught:
+                f.cancel()
+                return
+        except BaseException as exc:
+            if not f.cancelled():  # pragma: no branch
+                f.set_exception(exc)
+        else:
+            if not f.cancelled():  # pragma: no branch
+                f.set_result(res)
+
+    def trio_as_future(self, proc, *args):
         """Run an asynchronous Trio function from asyncio.
 
         Returns a Future with the result / exception.
 
         Cancelling the future will cancel the Trio task running your
         function, or prevent it from starting if that is still possible.
 
@@ -344,33 +346,14 @@
         :return: a trio-asyncio Handle
 
         The returned handle may be used to cancel the background task.
 
         """
         return self._queue_handle(Handle(proc, args, self, is_sync=False))
 
-    async def __run_trio(self, h):
-        """Helper for copying the result of a Trio task to an asyncio future"""
-        f, proc, *args = h._args
-        if f.cancelled():  # pragma: no cover
-            return
-        try:
-            with trio.open_cancel_scope() as scope:
-                h._scope = scope
-                res = await proc(*args)
-            if scope.cancelled_caught:
-                f.cancel()
-                return
-        except BaseException as exc:
-            if not f.cancelled():  # pragma: no branch
-                f.set_exception(exc)
-        else:
-            if not f.cancelled():  # pragma: no branch
-                f.set_result(res)
-
     # Callback handling #
 
     def _queue_handle(self, handle):
         """Queue a :class:`Handle` or :class:`TimerHandle` to be executed
         by the event loop.
 
         :param handle: A handle for the code to be executed
@@ -470,19 +453,18 @@
                 **kwargs
             )
 
             async def child_wait(transp):
                 returncode = await wait_for_child(transp.get_pid())
                 transp._process_exited(returncode)
 
-            self.run_trio(child_wait, transp)
-            # XXX error handling
+            self.run_trio_task(child_wait, transp)
             try:
                 await waiter
-            except Exception as exc:
+            except BaseException as exc:
                 # Workaround CPython bug #23353: using yield/yield-from in an
                 # except block of a generator doesn't clear properly
                 # sys.exc_info()
                 err = exc
             else:
                 err = None
 
@@ -505,15 +487,15 @@
         Returns an asyncio.Future.
         """
         self._check_callback(func, 'run_in_executor')
         self._check_closed()
         if executor is None:  # pragma: no branch
             executor = self._default_executor
         assert isinstance(executor, TrioExecutor)
-        return self.run_trio(executor.submit, func, *args)
+        return Trio_Asyncio_Wrapper(executor.submit, loop=self)(func, *args)
 
     async def synchronize(self):
         """Sync with the main loop by passing an event through it.
 
         This is a Trio coroutine.
 
         From asyncio, call ``await trio_asyncio.run_trio(loop.synchronize)``
@@ -563,26 +545,24 @@
     # reading from a file descriptor
 
     def add_reader(self, fd, callback, *args):
         """asyncio's method to call a function when a file descriptor is
         ready for reading.
 
         This creates a new Trio task. You may want to use "await
-        :meth:`trio.hazmat.wait_readable`(fd) instead, or
+        :obj:`trio.hazmat.wait_readable`\ (fd)" instead, or
 
         :param fd: Either an integer (Unix file descriptor) or an object
-                   with a :meth:`fileno` methor providing one.
+                   with a ``fileno`` method providing one.
         :return: A handle. To remove the listener, either call
-                 ``handle.cancel()`` or :meth:`remove_reader`(fd).
+                 ``handle.cancel()`` or :meth:`.remove_reader`\ (fd).
         """
         self._ensure_fd_no_transport(fd)
         return self._add_reader(fd, callback, *args)
 
-    # remove_reader: unchanged from asyncio
-
     def _add_reader(self, fd, callback, *args):
         self._check_closed()
         handle = Handle(callback, args, self, context=None, is_sync=True)
         reader = self._set_read_handle(fd, handle)
         if reader is not None:
             reader.cancel()
         if self._token is None:
@@ -618,20 +598,20 @@
     # writing to a file descriptor
 
     def add_writer(self, fd, callback, *args):
         """asyncio's method to call a function when a file descriptor is
         ready for writing.
 
         This creates a new Trio task. You may want to use "await
-        :meth:`trio.hazmat.wait_writable`(fd) instead, or
+        :obj:`trio.hazmat.wait_writable`\ (fd) instead, or
 
         :param fd: Either an integer (Unix file descriptor) or an object
-                   with a :meth:`fileno` methor providing one.
+                   with a ``fileno`` method providing one.
         :return: A handle. To remove the listener, either call
-                 ``handle.cancel()`` or :meth:`remove_writer`(fd).
+                 ``handle.cancel()`` or :meth:`remove_writer`\ (fd).
         """
         self._ensure_fd_no_transport(fd)
         return self._add_writer(fd, callback, *args)
 
     # remove_writer: unchanged from asyncio
 
     def _add_writer(self, fd, callback, *args):
@@ -675,15 +655,15 @@
 
         This is a safety measure. You also should use appropriate
         finalizers.
 
         Calling this method twice has no effect.
 
         :param fd: Either an integer (Unix file descriptor) or an object
-                   with a :meth:`fileno` methor providing one.
+                   with a ``fileno`` method providing one.
         """
         if hasattr(fd, 'fileno'):
             fd = fd.fileno()
         self._close_files.add(fd)
 
     def no_autoclose(self, fd):
         """
@@ -797,14 +777,22 @@
         """Finalize the loop. It may not be re-entered."""
         if self._closed:
             return
 
         self.stop()
         await self.wait_stopped()
 
+        while True:
+            try:
+                await self._main_loop_one(no_wait=True)
+            except trio.WouldBlock:
+                break
+            except StopAsyncIteration:
+                pass
+
         # Kill off unprocessed work
         self._cancel_fds()
         self._cancel_timers()
 
         # clean core fields
         self._nursery = None
         self._task = None
```

### Comparing `trio_asyncio-0.8.4/trio_asyncio.egg-info/SOURCES.txt` & `trio_asyncio-0.9.1/trio_asyncio.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 ci/test-requirements.txt
 tests/__init__.py
 tests/conftest.py
+tests/test_aio_subprocess.py
 tests/test_concurrent.py
 tests/test_misc.py
 tests/test_sync.py
 tests/utils.py
 tests/aiotest/__init__.py
 tests/aiotest/conftest.py
 tests/aiotest/test_add_reader.py
@@ -18,17 +19,14 @@
 tests/aiotest/test_thread.py
 tests/aiotest/test_timer.py
 tests/interop/__init__.py
 tests/interop/test_adapter.py
 tests/interop/test_calls.py
 tests/python/__init__.py
 tests/python/__main__.py
-tests/python/echo.py
-tests/python/echo2.py
-tests/python/echo3.py
 tests/python/keycert3.pem
 tests/python/pycacert.pem
 tests/python/ssl_cert.pem
 tests/python/ssl_key.pem
 tests/python/test_base_events.py
 tests/python/test_events.py
 tests/python/test_futures.py
```

### Comparing `trio_asyncio-0.8.4/trio_asyncio.egg-info/PKG-INFO` & `trio_asyncio-0.9.1/trio_asyncio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: trio-asyncio
-Version: 0.8.4
+Version: 0.9.1
 Summary: A re-implementation of the asyncio mainloop on top of Trio
 Home-page: https://github.com/python-trio/trio-asyncio
 Author: Matthias Urlichs
 Author-email: matthias@urlichs.de
 License: MIT -or- Apache License 2.0
 Description: ``trio-asyncio`` is a re-implementation of the ``asyncio`` mainloop on top of
         Trio.
@@ -67,8 +67,8 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: System :: Networking
 Classifier: Framework :: Trio
 Classifier: Framework :: AsyncIO
-Requires-Python: >=3.5.3
+Requires-Python: >=3.5.2
```

### Comparing `trio_asyncio-0.8.4/tests/utils.py` & `trio_asyncio-0.9.1/tests/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -579,15 +579,14 @@
 def get_function_source(func):
     source = _get_function_source(func)
     if source is None:
         raise ValueError("unable to get the source of %r" % (func,))
     return source
 
 
-
 def deprecate(tc, vers=None):
     if vers is None or sys.version_info >= vers:
         return pytest.deprecated_call()
 
     class _deprecate:
         def __init__(self, tc):
             pass
@@ -595,9 +594,7 @@
         def __enter__(self):
             return self
 
         def __exit__(self, *tb):
             pass
 
     return _deprecate(tc)
-
-
```

### Comparing `trio_asyncio-0.8.4/tests/interop/test_calls.py` & `trio_asyncio-0.9.1/tests/interop/test_calls.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import pytest
 import asyncio
 import trio
 import sniffio
+from trio_asyncio import aio_as_trio, trio_as_aio
 from tests import aiotest
 from functools import partial
 import sys
-from .. import utils
+from .. import utils as test_utils
 
 
 class Seen:
     flag = 0
 
 
 async def async_gen_to_list(generator):
@@ -55,77 +56,141 @@
         assert self.parent.did_it == 3
         self.parent.did_it = 4
 
 
 class TestCalls(aiotest.TestCase):
     async def call_t_a(self, proc, *args, loop=None):
         """called from Trio"""
-        return await loop.run_asyncio(proc, *args)
+        return await aio_as_trio(proc, loop=loop)(*args)
+
+    async def call_t_a_depr(self, proc, *args, loop=None):
+        """called from Trio"""
+        with test_utils.deprecate(self):
+            return await loop.run_asyncio(proc, *args)
 
     async def call_a_t(self, proc, *args, loop=None):
         """call from asyncio to an async trio function"""
-        return await loop.run_trio(proc, *args)
+        return await trio_as_aio(proc, loop=loop)(*args)
+
+    async def call_a_t_depr(self, proc, *args, loop=None):
+        """call from asyncio to an async trio function"""
+        with test_utils.deprecate(self):
+            return await loop.run_trio(proc, *args)
 
     async def call_a_ts(self, proc, *args, loop=None):
         """called from asyncio to a sync trio function"""
         return proc(*args)
 
     @pytest.mark.trio
     async def test_call_at(self, loop):
         async def delay(t):
             done = asyncio.Event(loop=loop)
             loop.call_at(t, done.set)
             await done.wait()
 
         t = loop.time() + 0.1
-        await loop.run_asyncio(delay, t)
+        await aio_as_trio(delay, loop=loop)(t)
+
+    @pytest.mark.trio
+    async def test_call_at_depr(self, loop):
+        async def delay(t):
+            done = asyncio.Event(loop=loop)
+            loop.call_at(t, done.set)
+            await done.wait()
+
+        t = loop.time() + 0.1
+        with test_utils.deprecate(self):
+            await loop.run_asyncio(delay, t)
 
     @pytest.mark.trio
     async def test_asyncio_trio(self, loop):
         """Call asyncio from trio"""
 
         async def dly_trio(seen):
             await trio.sleep(0.01)
             seen.flag |= 2
             return 8
 
         seen = Seen()
-        res = await loop.run_asyncio(partial(self.call_a_t, loop=loop), dly_trio, seen)
+        res = await aio_as_trio(partial(self.call_a_t, loop=loop), loop=loop)(dly_trio, seen)
+        assert res == 8
+        assert seen.flag == 2
+
+    @pytest.mark.trio
+    async def test_asyncio_trio_depr(self, loop):
+        """Call asyncio from trio"""
+
+        async def dly_trio(seen):
+            await trio.sleep(0.01)
+            seen.flag |= 2
+            return 8
+
+        seen = Seen()
+        res = await aio_as_trio(partial(self.call_a_t_depr, loop=loop), loop=loop)(dly_trio, seen)
         assert res == 8
         assert seen.flag == 2
 
     @pytest.mark.trio
     async def test_call_asyncio_ctx(self, loop):
         self.did_it = 0
-        async with loop.run_asyncio(AioContext(self, loop)) as ctx:
+        async with aio_as_trio(AioContext(self, loop), loop=loop) as ctx:
+            assert ctx.parent is self
             assert self.did_it == 2
             self.did_it = 3
         assert self.did_it == 4
 
     @pytest.mark.trio
     async def test_call_trio_ctx(self, loop):
         async def _call_trio_ctx():
             self.did_it = 0
+            async with trio_as_aio(TrioContext(self)) as ctx:
+                assert ctx.parent is self
+                assert self.did_it == 2
+                self.did_it = 3
+            assert self.did_it == 4
+
+        await aio_as_trio(_call_trio_ctx, loop=loop)()
+
+    @pytest.mark.trio
+    async def test_call_trio_ctx_depr(self, loop):
+        async def _call_trio_ctx():
+            self.did_it = 0
             async with loop.wrap_trio_context(TrioContext(self)) as ctx:
+                assert ctx.parent is self
                 assert self.did_it == 2
                 self.did_it = 3
             assert self.did_it == 4
 
-        await loop.run_asyncio(_call_trio_ctx)
+        with test_utils.deprecate(self):
+            await loop.run_asyncio(_call_trio_ctx)
 
     @pytest.mark.trio
     async def test_asyncio_trio_sync(self, loop):
         """Call asyncio from trio"""
 
         def dly_trio(seen):
             seen.flag |= 2
             return 8
 
         seen = Seen()
-        res = await loop.run_asyncio(partial(self.call_a_ts, loop=loop), dly_trio, seen)
+        res = await aio_as_trio(partial(self.call_a_ts, loop=loop), loop=loop)(dly_trio, seen)
+        assert res == 8
+        assert seen.flag == 2
+
+    @pytest.mark.trio
+    async def test_asyncio_trio_sync_depr(self, loop):
+        """Call asyncio from trio"""
+
+        def dly_trio(seen):
+            seen.flag |= 2
+            return 8
+
+        seen = Seen()
+        with test_utils.deprecate(self):
+            res = await loop.run_asyncio(partial(self.call_a_ts, loop=loop), dly_trio, seen)
         assert res == 8
         assert seen.flag == 2
 
     @pytest.mark.trio
     async def test_trio_asyncio(self, loop):
         async def dly_asyncio(seen):
             await asyncio.sleep(0.01, loop=loop)
@@ -134,57 +199,122 @@
 
         seen = Seen()
         res = await self.call_t_a(dly_asyncio, seen, loop=loop)
         assert res == 4
         assert seen.flag == 1
 
     @pytest.mark.trio
+    async def test_trio_asyncio_depr(self, loop):
+        async def dly_asyncio(seen):
+            await asyncio.sleep(0.01, loop=loop)
+            seen.flag |= 1
+            return 4
+
+        seen = Seen()
+        res = await self.call_t_a_depr(dly_asyncio, seen, loop=loop)
+        assert res == 4
+        assert seen.flag == 1
+
+    @pytest.mark.trio
     async def test_asyncio_trio_error(self, loop):
         async def err_trio():
             await trio.sleep(0.01)
             raise RuntimeError("I has another owie")
 
         with pytest.raises(RuntimeError) as err:
-            await loop.run_asyncio(partial(self.call_a_t, loop=loop), err_trio)
+            await aio_as_trio(partial(self.call_a_t, loop=loop), loop=loop)(err_trio)
+        assert err.value.args[0] == "I has another owie"
+
+    @pytest.mark.trio
+    async def test_asyncio_trio_error_depr1(self, loop):
+        async def err_trio():
+            await trio.sleep(0.01)
+            raise RuntimeError("I has another owie")
+
+        with pytest.raises(RuntimeError) as err:
+            await aio_as_trio(partial(self.call_a_t_depr, loop=loop), loop=loop)(err_trio)
+        assert err.value.args[0] == "I has another owie"
+
+    @pytest.mark.trio
+    async def test_asyncio_trio_error_depr2(self, loop):
+        async def err_trio():
+            await trio.sleep(0.01)
+            raise RuntimeError("I has another owie")
+
+        with pytest.raises(RuntimeError) as err:
+            with test_utils.deprecate(self):
+                await loop.run_asyncio(partial(self.call_a_t, loop=loop), err_trio)
+        assert err.value.args[0] == "I has another owie"
+
+    @pytest.mark.trio
+    async def test_asyncio_trio_error_depr3(self, loop):
+        async def err_trio():
+            await trio.sleep(0.01)
+            raise RuntimeError("I has another owie")
+
+        with pytest.raises(RuntimeError) as err:
+            with test_utils.deprecate(self):
+                await loop.run_asyncio(partial(self.call_a_t_depr, loop=loop), err_trio)
         assert err.value.args[0] == "I has another owie"
 
     @pytest.mark.trio
     async def test_asyncio_trio_sync_error(self, loop):
         def err_trio_sync():
             loop.time()  # verify that the loop is running
             raise RuntimeError("I has more owie")
 
         with pytest.raises(RuntimeError) as err:
-            await loop.run_asyncio(partial(self.call_a_ts, loop=loop), err_trio_sync)
+            await aio_as_trio(partial(self.call_a_ts, loop=loop), loop=loop)(err_trio_sync)
+        assert err.value.args[0] == "I has more owie"
+
+    @pytest.mark.trio
+    async def test_asyncio_trio_sync_error_depr(self, loop):
+        def err_trio_sync():
+            loop.time()  # verify that the loop is running
+            raise RuntimeError("I has more owie")
+
+        with pytest.raises(RuntimeError) as err:
+            with test_utils.deprecate(self):
+                await loop.run_asyncio(partial(self.call_a_ts, loop=loop), err_trio_sync)
         assert err.value.args[0] == "I has more owie"
 
     @pytest.mark.trio
     async def test_trio_asyncio_error(self, loop):
         async def err_asyncio():
             await asyncio.sleep(0.01, loop=loop)
             raise RuntimeError("I has an owie")
 
         with pytest.raises(RuntimeError) as err:
             await self.call_t_a(err_asyncio, loop=loop)
         assert err.value.args[0] == "I has an owie"
 
     @pytest.mark.trio
+    async def test_trio_asyncio_error_depr(self, loop):
+        async def err_asyncio():
+            await asyncio.sleep(0.01, loop=loop)
+            raise RuntimeError("I has an owie")
+
+        with pytest.raises(RuntimeError) as err:
+            await self.call_t_a_depr(err_asyncio, loop=loop)
+        assert err.value.args[0] == "I has an owie"
+
+    @pytest.mark.trio
     async def test_asyncio_trio_cancel_out(self, loop):
         async def cancelled_trio(seen):
             seen.flag |= 1
             await trio.sleep(0.01)
             scope = trio.hazmat.current_task()._cancel_stack[-1]
             scope.cancel()
             seen.flag |= 2
             await trio.sleep(0.01)
             seen.flag |= 4
 
         seen = Seen()
         with pytest.raises(asyncio.CancelledError):
-            await loop.run_asyncio(partial(self.call_a_t, loop=loop), cancelled_trio, seen)
+            await aio_as_trio(partial(self.call_a_t, loop=loop), loop=loop)(cancelled_trio, seen)
         assert seen.flag == 3
 
     @pytest.mark.trio
     async def test_trio_asyncio_cancel_out(self, loop):
         async def cancelled_asyncio(seen):
             seen.flag |= 1
             await asyncio.sleep(0.01, loop=loop)
@@ -210,14 +340,44 @@
         assert seen.flag == 1 | 4
 
         seen = Seen()
         await check_cancel(cancelled_asyncio, seen)
         assert seen.flag == 1 | 4
 
     @pytest.mark.trio
+    async def test_trio_asyncio_cancel_out_depr(self, loop):
+        async def cancelled_asyncio(seen):
+            seen.flag |= 1
+            await asyncio.sleep(0.01, loop=loop)
+            f = asyncio.Future(loop=loop)
+            f.cancel()
+            return f.result()  # raises error
+
+        def cancelled_future(seen):
+            seen.flag |= 1
+            f = asyncio.Future(loop=loop)
+            f.cancel()
+            return f  # contains error
+
+        async def check_cancel(proc, seen):
+            with trio.open_cancel_scope() as scope:
+                with pytest.raises(asyncio.CancelledError):
+                    await self.call_t_a_depr(proc, seen, loop=loop)
+            assert not scope.cancel_called
+            seen.flag |= 4
+
+        seen = Seen()
+        await check_cancel(cancelled_future, seen)
+        assert seen.flag == 1 | 4
+
+        seen = Seen()
+        await check_cancel(cancelled_asyncio, seen)
+        assert seen.flag == 1 | 4
+
+    @pytest.mark.trio
     async def test_asyncio_trio_cancel_in(self, loop):
         async def in_trio(started, seen):
             started.set()
             try:
                 await trio.sleep(1)
             except trio.Cancelled:
                 seen.flag |= 1
@@ -232,15 +392,15 @@
             await started.wait()
             f.cancel()
             with pytest.raises(asyncio.CancelledError):
                 await f
             seen.flag |= 8
 
         seen = Seen()
-        await loop.run_asyncio(cancel_asyncio, seen)
+        await aio_as_trio(cancel_asyncio, loop=loop)(seen)
         assert seen.flag == 1 | 2 | 8
 
     @pytest.mark.trio
     async def test_trio_asyncio_cancel_in(self, loop):
         async def in_asyncio(started, seen):
             started.set()
             try:
@@ -263,14 +423,43 @@
             seen.flag |= 8
 
         seen = Seen()
         await cancel_trio(seen)
         assert seen.flag == 1 | 2 | 8
 
     @pytest.mark.trio
+    async def test_trio_asyncio_cancel_in_depr(self, loop):
+        async def in_asyncio(started, seen):
+            started.set()
+            try:
+                await asyncio.sleep(9999, loop=loop)
+            except asyncio.CancelledError:
+                seen.flag |= 1
+            except trio.Cancelled:
+                seen.flag |= 16
+            else:
+                seen.flag |= 4
+            finally:
+                seen.flag |= 2
+
+        async def cancel_trio(seen):
+            started = trio.Event()
+            async with trio.open_nursery() as nursery:
+                nursery.start_soon(
+                    partial(self.call_t_a_depr, loop=loop), in_asyncio, started, seen
+                )
+                await started.wait()
+                nursery.cancel_scope.cancel()
+            seen.flag |= 8
+
+        seen = Seen()
+        await cancel_trio(seen)
+        assert seen.flag == 1 | 2 | 8
+
+    @pytest.mark.trio
     async def test_trio_asyncio_cancel_direct(self, loop):
         def in_asyncio(started, seen):
             # This is intentionally not async
             seen.flag |= 1
             raise asyncio.CancelledError()
 
         async def cancel_trio(seen):
@@ -287,42 +476,76 @@
 
         seen = Seen()
         with pytest.raises(asyncio.CancelledError):
             await cancel_trio(seen)
         assert seen.flag == 1 | 8
 
     @pytest.mark.trio
+    async def test_trio_asyncio_cancel_direct_depr(self, loop):
+        def in_asyncio(started, seen):
+            # This is intentionally not async
+            seen.flag |= 1
+            raise asyncio.CancelledError()
+
+        async def cancel_trio(seen):
+            started = trio.Event()
+            try:
+                async with trio.open_nursery() as nursery:
+                    nursery.start_soon(
+                        partial(self.call_t_a_depr, loop=loop), in_asyncio, started, seen
+                    )
+                    await started.wait()
+                    nursery.cancel_scope.cancel()
+            finally:
+                seen.flag |= 8
+
+        seen = Seen()
+        with pytest.raises(asyncio.CancelledError):
+            await cancel_trio(seen)
+        assert seen.flag == 1 | 8
+
+    @pytest.mark.trio
     async def test_trio_asyncio_error_direct(self, loop):
         def err_asyncio():
             # This is intentionally not async
             raise RuntimeError("I has an owie")
 
         with pytest.raises(RuntimeError) as err:
             await self.call_t_a(err_asyncio, loop=loop)
         assert err.value.args[0] == "I has an owie"
 
     @pytest.mark.trio
+    async def test_trio_asyncio_error_direct_depr(self, loop):
+        def err_asyncio():
+            # This is intentionally not async
+            raise RuntimeError("I has an owie")
+
+        with pytest.raises(RuntimeError) as err:
+            await self.call_t_a_depr(err_asyncio, loop=loop)
+        assert err.value.args[0] == "I has an owie"
+
+    @pytest.mark.trio
     async def test_trio_asyncio_generator(self, loop):
         async def dly_asyncio():
             yield 1
             await asyncio.sleep(0.01, loop=loop)
             yield 2
 
-        with utils.deprecate(self):
+        with test_utils.deprecate(self):
             res = await async_gen_to_list(loop.wrap_generator(dly_asyncio))
         assert res == [1, 2]
 
     @pytest.mark.trio
     async def test_trio_asyncio_generator_with_error(self, loop):
         async def dly_asyncio():
             yield 1
             raise RuntimeError("I has an owie")
             yield 2
 
-        with utils.deprecate(self):
+        with test_utils.deprecate(self):
             with pytest.raises(RuntimeError) as err:
                 await async_gen_to_list(loop.wrap_generator(dly_asyncio))
         assert err.value.args[0] == "I has an owie"
 
     @pytest.mark.trio
     async def test_trio_asyncio_generator_with_cancellation(self, loop):
         async def dly_asyncio(hold, seen):
@@ -333,25 +556,40 @@
         async def cancel_soon(nursery):
             await trio.sleep(0.01)
             nursery.cancel_scope.cancel()
 
         hold = asyncio.Event(loop=loop)
         seen = Seen()
 
-        with utils.deprecate(self):
+        with test_utils.deprecate(self):
             async with trio.open_nursery() as nursery:
                 nursery.start_soon(async_gen_to_list, loop.wrap_generator(dly_asyncio, hold, seen))
                 nursery.start_soon(cancel_soon, nursery)
         assert nursery.cancel_scope.cancel_called
         assert seen.flag == 1
 
     @pytest.mark.trio
     async def test_trio_asyncio_iterator(self, loop):
         async def slow_nums():
             for n in range(1, 6):
                 asyncio.sleep(0.01, loop=loop)
                 yield n
 
         sum = 0
-        async for n in loop.run_asyncio(slow_nums()):
+        async for n in aio_as_trio(slow_nums()):
+            sum += n
+        assert sum == 15
+
+    @pytest.mark.trio
+    async def test_trio_asyncio_iterator_depr(self, loop):
+        async def slow_nums():
+            for n in range(1, 6):
+                asyncio.sleep(0.01, loop=loop)
+                yield n
+
+        sum = 0
+        # with test_utils.deprecate(self): ## not yet
+        async for n in aio_as_trio(
+            slow_nums(), loop=loop
+        ):
             sum += n
         assert sum == 15
```

### Comparing `trio_asyncio-0.8.4/tests/aiotest/test_coroutine.py` & `trio_asyncio-0.9.1/tests/aiotest/test_coroutine.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from tests import aiotest
+import trio_asyncio
 import pytest
+from .. import utils as test_utils
 
 
 async def hello_world(asyncio, result, delay, loop):
     result.append("Hello")
     # retrieve the event loop from the policy
     await asyncio.sleep(delay, loop=loop)
     result.append('World')
@@ -11,15 +13,23 @@
 
 
 class TestCoroutine(aiotest.TestCase):
     @pytest.mark.trio
     async def test_hello_world(self, loop, config):
         result = []
         coro = hello_world(config.asyncio, result, 0.001, loop)
-        await loop.run_coroutine(config.asyncio.ensure_future(coro, loop=loop))
+        await loop.run_aio_coroutine(config.asyncio.ensure_future(coro, loop=loop))
+        assert result == ['Hello', 'World']
+
+    @pytest.mark.trio
+    async def test_hello_world_depr(self, loop, config):
+        result = []
+        coro = hello_world(config.asyncio, result, 0.001, loop)
+        with test_utils.deprecate(self):
+            await loop.run_coroutine(config.asyncio.ensure_future(coro, loop=loop))
         assert result == ['Hello', 'World']
 
     @pytest.mark.trio
     async def run_hello_world(self, loop, config):
         result = []
         await loop.run_asyncio(hello_world, config.asyncio, result, 0.001, loop)
         assert result == ['Hello', 'World']
@@ -33,9 +43,26 @@
             value = await fut
             result.append(value)
 
             value = await hello_world(asyncio, result, 0.001, loop)
             result.append(value)
 
         result = []
-        await loop.run_asyncio(waiter, config.asyncio, hello_world, result)
+        await trio_asyncio.aio_as_trio(waiter)(config.asyncio, hello_world, result)
+        assert result == ['Future', 'Hello', 'World', '.']
+
+    @pytest.mark.trio
+    async def test_waiter_depr(self, loop, config):
+        async def waiter(asyncio, hello_world, result):
+            fut = asyncio.Future(loop=loop)
+            loop.call_soon(fut.set_result, "Future")
+
+            value = await fut
+            result.append(value)
+
+            value = await hello_world(asyncio, result, 0.001, loop)
+            result.append(value)
+
+        result = []
+        with test_utils.deprecate(self):
+            await loop.run_asyncio(waiter, config.asyncio, hello_world, result)
         assert result == ['Future', 'Hello', 'World', '.']
```

### Comparing `trio_asyncio-0.8.4/tests/aiotest/test_network.py` & `trio_asyncio-0.9.1/tests/aiotest/test_network.py`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/tests/aiotest/__init__.py` & `trio_asyncio-0.9.1/tests/aiotest/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import socket
-import sys
 import threading
 import time
 
 import asyncio as _asyncio
 socketpair = socket.socketpair
```

### Comparing `trio_asyncio-0.8.4/tests/aiotest/test_add_reader.py` & `trio_asyncio-0.9.1/tests/aiotest/test_add_reader.py`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/tests/aiotest/test_callback.py` & `trio_asyncio-0.9.1/tests/aiotest/test_callback.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from tests import aiotest
 import signal
 import pytest
+from .. import utils as test_utils
 
 
 class TestCallback(aiotest.TestCase):
     @pytest.mark.trio
     async def test_call_soon(self, loop):
         result = []
 
@@ -66,12 +67,15 @@
             with pytest.raises(RuntimeError, match='Event loop is closed'):
                 loop.call_later(1.0, func)
             with pytest.raises(RuntimeError, match='Event loop is closed'):
                 loop.call_at(loop.time() + .0, func)
             with pytest.raises(RuntimeError, match='Event loop is closed'):
                 loop.run_in_executor(None, func)
             with pytest.raises(RuntimeError, match='Event loop is closed'):
-                await loop.run_coroutine(coro)
+                await loop.run_aio_coroutine(coro)
+            with test_utils.deprecate(self):
+                with pytest.raises(RuntimeError, match='Event loop is closed'):
+                    await loop.run_coroutine(coro)
             with pytest.raises(RuntimeError, match='Event loop is closed'):
                 loop.add_signal_handler(signal.SIGTERM, func)
         finally:
             coro.close()
```

### Comparing `trio_asyncio-0.8.4/tests/aiotest/test_thread.py` & `trio_asyncio-0.9.1/tests/aiotest/test_thread.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from tests import aiotest
 import pytest
 import trio
 import trio_asyncio
+from .. import utils as test_utils
 
 
 class TestThread(aiotest.TestCase):
     @pytest.mark.trio
     async def test_ident(self, loop, config):
         threading = config.threading
         try:
@@ -15,35 +16,75 @@
 
         result = {'ident': None}
 
         def work():
             result['ident'] = get_ident()
 
         fut = loop.run_in_executor(None, work)
-        await loop.run_coroutine(fut)
+        await loop.run_aio_coroutine(fut)
+
+        # ensure that work() was executed in a different thread
+        work_ident = result['ident']
+        assert work_ident is not None
+        assert work_ident != get_ident()
+
+    @pytest.mark.trio
+    async def test_ident_depr(self, loop, config):
+        threading = config.threading
+        try:
+            get_ident = threading.get_ident  # Python 3
+        except AttributeError:
+            get_ident = threading._get_ident  # Python 2
+
+        result = {'ident': None}
+
+        def work():
+            result['ident'] = get_ident()
+
+        fut = loop.run_in_executor(None, work)
+        with test_utils.deprecate(self):
+            await loop.run_coroutine(fut)
 
         # ensure that work() was executed in a different thread
         work_ident = result['ident']
         assert work_ident is not None
         assert work_ident != get_ident()
 
     @pytest.mark.trio
     async def test_run_twice(self, loop):
         result = []
 
         def work():
             result.append("run")
 
         fut = loop.run_in_executor(None, work)
-        await loop.run_future(fut)
+        await loop.run_aio_future(fut)
+        assert result == ["run"]
+
+        # ensure that run_in_executor() can be called twice
+        fut = loop.run_in_executor(None, work)
+        await loop.run_aio_future(fut)
+        assert result == ["run", "run"]
+
+    @pytest.mark.trio
+    async def test_run_twice_depr(self, loop):
+        result = []
+
+        def work():
+            result.append("run")
+
+        fut = loop.run_in_executor(None, work)
+        with test_utils.deprecate(self):
+            await loop.run_future(fut)
         assert result == ["run"]
 
         # ensure that run_in_executor() can be called twice
         fut = loop.run_in_executor(None, work)
-        await loop.run_future(fut)
+        with test_utils.deprecate(self):
+            await loop.run_future(fut)
         assert result == ["run", "run"]
 
     @pytest.mark.trio
     async def test_policy(self, loop, config):
         asyncio = config.asyncio
         result = {'loop': 'not set'}  # sentinel, different than None
 
@@ -51,15 +92,32 @@
             try:
                 result['loop'] = asyncio.get_event_loop()
             except Exception as exc:
                 result['loop'] = exc
 
         # get_event_loop() must return None in a different thread
         fut = loop.run_in_executor(None, work)
-        await loop.run_future(fut)
+        await loop.run_aio_future(fut)
+        assert isinstance(result['loop'], (AssertionError, RuntimeError))
+
+    @pytest.mark.trio
+    async def test_policy_depr(self, loop, config):
+        asyncio = config.asyncio
+        result = {'loop': 'not set'}  # sentinel, different than None
+
+        def work():
+            try:
+                result['loop'] = asyncio.get_event_loop()
+            except Exception as exc:
+                result['loop'] = exc
+
+        # get_event_loop() must return None in a different thread
+        fut = loop.run_in_executor(None, work)
+        with test_utils.deprecate(self):
+            await loop.run_future(fut)
         assert isinstance(result['loop'], (AssertionError, RuntimeError))
 
     @pytest.mark.trio
     async def test_run_in_thread(self, config):
         threading = config.threading
 
         class LoopThread(threading.Thread):
```

### Comparing `trio_asyncio-0.8.4/tests/aiotest/test_timer.py` & `trio_asyncio-0.9.1/tests/aiotest/test_timer.py`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/tests/__init__.py` & `trio_asyncio-0.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/tests/conftest.py` & `trio_asyncio-0.9.1/tests/conftest.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # copy-paste...
 #
 # this stuff should become a proper pytest plugin
 
 import pytest
 import asyncio
 import trio_asyncio
-import trio_asyncio.loop as loop_
 import inspect
 from async_generator import async_generator, yield_
 
 # Hacks for <3.7
 if not hasattr(asyncio, 'run'):
 
     def run(main, *, debug=False):
@@ -52,15 +51,15 @@
 
 
 @pytest.fixture
 @async_generator
 async def loop():
     async with trio_asyncio.open_loop() as loop:
         try:
-            await yield_( loop)
+            await yield_(loop)
         finally:
             await loop.stop().wait()
 
 
 # auto-trio-ize all async functions
 @pytest.hookimpl(tryfirst=True)
 def pytest_pyfunc_call(pyfuncitem):
```

### Comparing `trio_asyncio-0.8.4/tests/test_concurrent.py` & `trio_asyncio-0.9.1/tests/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/tests/python/test_transports.py` & `trio_asyncio-0.9.1/tests/python/test_transports.py`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/tests/python/test_base_events.py` & `trio_asyncio-0.9.1/tests/python/test_base_events.py`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/tests/python/test_unix_events.py` & `trio_asyncio-0.9.1/tests/python/test_unix_events.py`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/tests/python/test_tasks.py` & `trio_asyncio-0.9.1/tests/python/test_tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,30 +305,30 @@
             self.assertEqual(gen.__qualname__, coro_qualname)
 
         # test pending Task
         t = self.new_task(self.loop, gen)
         t.add_done_callback(Dummy())
 
         coro = format_coroutine(coro_qualname, 'running', src, t._source_traceback, generator=True)
-        self.assertEqual(repr(t), '<Task pending %s cb=[<Dummy>()]>' % coro)
+        assert " pending " in repr(t)
 
         # test cancelling Task
         t.cancel()  # Does not take immediate effect!
-        self.assertEqual(repr(t), '<Task cancelling %s cb=[<Dummy>()]>' % coro)
+        assert " cancelling " in repr(t)
 
         # test cancelled Task
         self.assertRaises(asyncio.CancelledError, self.loop.run_until_complete, t)
         coro = format_coroutine(coro_qualname, 'done', src, t._source_traceback)
-        self.assertEqual(repr(t), '<Task cancelled %s>' % coro)
+        assert " cancelled " in repr(t)
 
         # test finished Task
         t = self.new_task(self.loop, notmuch())
         self.loop.run_until_complete(t)
         coro = format_coroutine(coro_qualname, 'done', src, t._source_traceback)
-        self.assertEqual(repr(t), "<Task finished %s result='abc'>" % coro)
+        assert " finished " in repr(t)
 
     def test_task_repr_coro_decorator(self):
         self.loop.set_debug(False)
 
         @asyncio.coroutine
         def notmuch():
             # notmuch() function doesn't use yield from: it will be wrapped by
@@ -388,15 +388,15 @@
             src = '%s:%s' % test_utils.get_function_source(notmuch)
         else:
             code = gen.gi_code
             src = '%s:%s' % (code.co_filename, code.co_firstlineno)
         coro = format_coroutine(
             coro_qualname, 'running', src, t._source_traceback, generator=not coroutines._DEBUG
         )
-        self.assertEqual(repr(t), '<Task pending %s cb=[<Dummy>()]>' % coro)
+        assert " pending " in repr(t)
         self.loop.run_until_complete(t)
 
     def test_task_repr_wait_for(self):
         self.loop.set_debug(False)
 
         @asyncio.coroutine
         def wait_for(fut):
```

### Comparing `trio_asyncio-0.8.4/tests/python/test_subprocess.py` & `trio_asyncio-0.9.1/tests/python/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/tests/python/test_windows_utils.py` & `trio_asyncio-0.9.1/tests/python/test_windows_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Tests for window_utils"""
 
 import socket
 import sys
 import unittest
 import warnings
-from unittest import mock
 
 if sys.platform != 'win32':
     raise unittest.SkipTest('Windows only')
 
 import _winapi
 
 try:
```

### Comparing `trio_asyncio-0.8.4/tests/python/test_streams.py` & `trio_asyncio-0.9.1/tests/python/test_streams.py`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/tests/python/test_sslproto.py` & `trio_asyncio-0.9.1/tests/python/test_sslproto.py`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/tests/python/test_events.py` & `trio_asyncio-0.9.1/tests/python/test_events.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,30 +9,28 @@
 import re
 import signal
 import socket
 try:
     import ssl
 except ImportError:
     ssl = None
-import subprocess
 import sys
 import threading
 import errno
 import unittest
 from unittest import mock
 import weakref
 
 if sys.platform != 'win32':
     import tty
 
 import asyncio
 from asyncio import coroutines
 from asyncio import proactor_events
 from asyncio import selector_events
-from asyncio import sslproto
 from .. import utils as test_utils
 try:
     from test import support
 except ImportError:
     from asyncio import test_support as support
 
 import time
@@ -218,53 +216,14 @@
     def connection_lost(self, exc):
         assert self.state == 'CONNECTED', self.state
         self.state = 'CLOSED'
         if self.done:
             self.done.set_result(None)
 
 
-class MySubprocessProtocol(asyncio.SubprocessProtocol):
-    def __init__(self, loop):
-        self.state = 'INITIAL'
-        self.transport = None
-        self.connected = asyncio.Future(loop=loop)
-        self.completed = asyncio.Future(loop=loop)
-        self.disconnects = {fd: asyncio.Future(loop=loop) for fd in range(3)}
-        self.data = {1: b'', 2: b''}
-        self.returncode = None
-        self.got_data = {1: asyncio.Event(loop=loop), 2: asyncio.Event(loop=loop)}
-
-    def connection_made(self, transport):
-        self.transport = transport
-        assert self.state == 'INITIAL', self.state
-        self.state = 'CONNECTED'
-        self.connected.set_result(None)
-
-    def connection_lost(self, exc):
-        assert self.state == 'CONNECTED', self.state
-        self.state = 'CLOSED'
-        self.completed.set_result(None)
-
-    def pipe_data_received(self, fd, data):
-        assert self.state == 'CONNECTED', self.state
-        self.data[fd] += data
-        self.got_data[fd].set()
-
-    def pipe_connection_lost(self, fd, exc):
-        assert self.state == 'CONNECTED', self.state
-        if exc:
-            self.disconnects[fd].set_exception(exc)
-        else:
-            self.disconnects[fd].set_result(exc)
-
-    def process_exited(self):
-        assert self.state == 'CONNECTED', self.state
-        self.returncode = self.transport.get_returncode()
-
-
 class EventLoopTestsMixin:
     def setUp(self):
         super().setUp()
         self.loop = self.create_event_loop()
         self.set_event_loop(self.loop)
 
     def tearDown(self):
@@ -1792,304 +1751,21 @@
             self.loop.run_in_executor(None, func)
         with self.assertRaises(RuntimeError):
             self.loop.create_task(coro)
         with self.assertRaises(RuntimeError):
             self.loop.add_signal_handler(signal.SIGTERM, func)
 
 
-class SubprocessTestsMixin:
-    def check_terminated(self, returncode):
-        if sys.platform == 'win32':
-            self.assertIsInstance(returncode, int)
-            # expect 1 but sometimes get 0
-        else:
-            self.assertEqual(-signal.SIGTERM, returncode)
-
-    def check_killed(self, returncode):
-        if sys.platform == 'win32':
-            self.assertIsInstance(returncode, int)
-            # expect 1 but sometimes get 0
-        else:
-            self.assertEqual(-signal.SIGKILL, returncode)
-
-    def test_subprocess_exec(self):
-        prog = os.path.join(os.path.dirname(__file__), 'echo.py')
-
-        connect = self.loop.subprocess_exec(
-            functools.partial(MySubprocessProtocol, self.loop), sys.executable, prog
-        )
-        transp, proto = self.loop.run_until_complete(connect)
-        self.assertIsInstance(proto, MySubprocessProtocol)
-        self.loop.run_until_complete(proto.connected)
-        self.assertEqual('CONNECTED', proto.state)
-
-        stdin = transp.get_pipe_transport(0)
-        stdin.write(b'Python The Winner')
-        self.loop.run_until_complete(proto.got_data[1].wait())
-        with test_utils.disable_logger():
-            transp.close()
-        self.loop.run_until_complete(proto.completed)
-        self.check_killed(proto.returncode)
-        self.assertEqual(b'Python The Winner', proto.data[1])
-
-    def test_subprocess_interactive(self):
-        prog = os.path.join(os.path.dirname(__file__), 'echo.py')
-
-        connect = self.loop.subprocess_exec(
-            functools.partial(MySubprocessProtocol, self.loop), sys.executable, prog
-        )
-        transp, proto = self.loop.run_until_complete(connect)
-        self.assertIsInstance(proto, MySubprocessProtocol)
-        self.loop.run_until_complete(proto.connected)
-        self.assertEqual('CONNECTED', proto.state)
-
-        stdin = transp.get_pipe_transport(0)
-        stdin.write(b'Python ')
-        self.loop.run_until_complete(proto.got_data[1].wait())
-        proto.got_data[1].clear()
-        self.assertEqual(b'Python ', proto.data[1])
-
-        stdin.write(b'The Winner')
-        self.loop.run_until_complete(proto.got_data[1].wait())
-        self.assertEqual(b'Python The Winner', proto.data[1])
-
-        with test_utils.disable_logger():
-            transp.close()
-        self.loop.run_until_complete(proto.completed)
-        self.check_killed(proto.returncode)
-
-    def test_subprocess_shell(self):
-        connect = self.loop.subprocess_shell(
-            functools.partial(MySubprocessProtocol, self.loop), 'echo Python'
-        )
-        transp, proto = self.loop.run_until_complete(connect)
-        self.assertIsInstance(proto, MySubprocessProtocol)
-        self.loop.run_until_complete(proto.connected)
-
-        transp.get_pipe_transport(0).close()
-        self.loop.run_until_complete(proto.completed)
-        self.assertEqual(0, proto.returncode)
-        self.assertTrue(all(f.done() for f in proto.disconnects.values()))
-        self.assertEqual(proto.data[1].rstrip(b'\r\n'), b'Python')
-        self.assertEqual(proto.data[2], b'')
-        transp.close()
-
-    def test_subprocess_exitcode(self):
-        connect = self.loop.subprocess_shell(
-            functools.partial(MySubprocessProtocol, self.loop),
-            'exit 7',
-            stdin=None,
-            stdout=None,
-            stderr=None
-        )
-        transp, proto = self.loop.run_until_complete(connect)
-        self.assertIsInstance(proto, MySubprocessProtocol)
-        self.loop.run_until_complete(proto.completed)
-        self.assertEqual(7, proto.returncode)
-        transp.close()
-
-    def test_subprocess_close_after_finish(self):
-        connect = self.loop.subprocess_shell(
-            functools.partial(MySubprocessProtocol, self.loop),
-            'exit 7',
-            stdin=None,
-            stdout=None,
-            stderr=None
-        )
-        transp, proto = self.loop.run_until_complete(connect)
-        self.assertIsInstance(proto, MySubprocessProtocol)
-        self.assertIsNone(transp.get_pipe_transport(0))
-        self.assertIsNone(transp.get_pipe_transport(1))
-        self.assertIsNone(transp.get_pipe_transport(2))
-        self.loop.run_until_complete(proto.completed)
-        self.assertEqual(7, proto.returncode)
-        self.assertIsNone(transp.close())
-
-    def test_subprocess_kill(self):
-        prog = os.path.join(os.path.dirname(__file__), 'echo.py')
-
-        connect = self.loop.subprocess_exec(
-            functools.partial(MySubprocessProtocol, self.loop), sys.executable, prog
-        )
-        transp, proto = self.loop.run_until_complete(connect)
-        self.assertIsInstance(proto, MySubprocessProtocol)
-        self.loop.run_until_complete(proto.connected)
-
-        transp.kill()
-        self.loop.run_until_complete(proto.completed)
-        self.check_killed(proto.returncode)
-        transp.close()
-
-    def test_subprocess_terminate(self):
-        prog = os.path.join(os.path.dirname(__file__), 'echo.py')
-
-        connect = self.loop.subprocess_exec(
-            functools.partial(MySubprocessProtocol, self.loop), sys.executable, prog
-        )
-        transp, proto = self.loop.run_until_complete(connect)
-        self.assertIsInstance(proto, MySubprocessProtocol)
-        self.loop.run_until_complete(proto.connected)
-
-        transp.terminate()
-        self.loop.run_until_complete(proto.completed)
-        self.check_terminated(proto.returncode)
-        transp.close()
-
-    @unittest.skipIf(sys.platform == 'win32', "Don't have SIGHUP")
-    def test_subprocess_send_signal(self):
-        # bpo-31034: Make sure that we get the default signal handler (killing
-        # the process). The parent process may have decided to ignore SIGHUP,
-        # and signal handlers are inherited.
-        old_handler = signal.signal(signal.SIGHUP, signal.SIG_DFL)
-        try:
-            prog = os.path.join(os.path.dirname(__file__), 'echo.py')
-
-            connect = self.loop.subprocess_exec(
-                functools.partial(MySubprocessProtocol, self.loop), sys.executable, prog
-            )
-            transp, proto = self.loop.run_until_complete(connect)
-            self.assertIsInstance(proto, MySubprocessProtocol)
-            self.loop.run_until_complete(proto.connected)
-
-            transp.send_signal(signal.SIGHUP)
-            self.loop.run_until_complete(proto.completed)
-            self.assertEqual(-signal.SIGHUP, proto.returncode)
-            transp.close()
-        finally:
-            signal.signal(signal.SIGHUP, old_handler)
-
-    def test_subprocess_stderr(self):
-        prog = os.path.join(os.path.dirname(__file__), 'echo2.py')
-
-        connect = self.loop.subprocess_exec(
-            functools.partial(MySubprocessProtocol, self.loop), sys.executable, prog
-        )
-        transp, proto = self.loop.run_until_complete(connect)
-        self.assertIsInstance(proto, MySubprocessProtocol)
-        self.loop.run_until_complete(proto.connected)
-
-        stdin = transp.get_pipe_transport(0)
-        stdin.write(b'test')
-
-        self.loop.run_until_complete(proto.completed)
-
-        transp.close()
-        self.assertEqual(b'OUT:test', proto.data[1])
-        self.assertTrue(proto.data[2].startswith(b'ERR:test'), proto.data[2])
-        self.assertEqual(0, proto.returncode)
-
-    def test_subprocess_stderr_redirect_to_stdout(self):
-        prog = os.path.join(os.path.dirname(__file__), 'echo2.py')
-
-        connect = self.loop.subprocess_exec(
-            functools.partial(MySubprocessProtocol, self.loop),
-            sys.executable,
-            prog,
-            stderr=subprocess.STDOUT
-        )
-        transp, proto = self.loop.run_until_complete(connect)
-        self.assertIsInstance(proto, MySubprocessProtocol)
-        self.loop.run_until_complete(proto.connected)
-
-        stdin = transp.get_pipe_transport(0)
-        self.assertIsNotNone(transp.get_pipe_transport(1))
-        self.assertIsNone(transp.get_pipe_transport(2))
-
-        stdin.write(b'test')
-        self.loop.run_until_complete(proto.completed)
-        self.assertTrue(proto.data[1].startswith(b'OUT:testERR:test'), proto.data[1])
-        self.assertEqual(b'', proto.data[2])
-
-        transp.close()
-        self.assertEqual(0, proto.returncode)
-
-    def test_subprocess_close_client_stream(self):
-        prog = os.path.join(os.path.dirname(__file__), 'echo3.py')
-
-        connect = self.loop.subprocess_exec(
-            functools.partial(MySubprocessProtocol, self.loop), sys.executable, prog
-        )
-        transp, proto = self.loop.run_until_complete(connect)
-        self.assertIsInstance(proto, MySubprocessProtocol)
-        self.loop.run_until_complete(proto.connected)
-
-        stdin = transp.get_pipe_transport(0)
-        stdout = transp.get_pipe_transport(1)
-        stdin.write(b'test')
-        self.loop.run_until_complete(proto.got_data[1].wait())
-        self.assertEqual(b'OUT:test', proto.data[1])
-
-        stdout.close()
-        self.loop.run_until_complete(proto.disconnects[1])
-        stdin.write(b'xxx')
-        self.loop.run_until_complete(proto.got_data[2].wait())
-        if sys.platform != 'win32':
-            self.assertEqual(b'ERR:BrokenPipeError', proto.data[2])
-        else:
-            # After closing the read-end of a pipe, writing to the
-            # write-end using os.write() fails with errno==EINVAL and
-            # GetLastError()==ERROR_INVALID_NAME on Windows!?!  (Using
-            # WriteFile() we get ERROR_BROKEN_PIPE as expected.)
-            self.assertEqual(b'ERR:OSError', proto.data[2])
-        with test_utils.disable_logger():
-            transp.close()
-        self.loop.run_until_complete(proto.completed)
-        self.check_killed(proto.returncode)
-
-    def test_subprocess_wait_no_same_group(self):
-        # start the new process in a new session
-        connect = self.loop.subprocess_shell(
-            functools.partial(MySubprocessProtocol, self.loop),
-            'exit 7',
-            stdin=None,
-            stdout=None,
-            stderr=None,
-            start_new_session=True
-        )
-        _, proto = yield self.loop.run_until_complete(connect)
-        self.assertIsInstance(proto, MySubprocessProtocol)
-        self.loop.run_until_complete(proto.completed)
-        self.assertEqual(7, proto.returncode)
-
-    def test_subprocess_exec_invalid_args(self):
-        @asyncio.coroutine
-        def connect(**kwds):
-            yield from self.loop.subprocess_exec(asyncio.SubprocessProtocol, 'pwd', **kwds)
-
-        with self.assertRaises(ValueError):
-            self.loop.run_until_complete(connect(universal_newlines=True))
-        with self.assertRaises(ValueError):
-            self.loop.run_until_complete(connect(bufsize=4096))
-        with self.assertRaises(ValueError):
-            self.loop.run_until_complete(connect(shell=True))
-
-    def test_subprocess_shell_invalid_args(self):
-        @asyncio.coroutine
-        def connect(cmd=None, **kwds):
-            if not cmd:
-                cmd = 'pwd'
-            yield from self.loop.subprocess_shell(asyncio.SubprocessProtocol, cmd, **kwds)
-
-        with self.assertRaises(ValueError):
-            self.loop.run_until_complete(connect(['ls', '-l']))
-        with self.assertRaises(ValueError):
-            self.loop.run_until_complete(connect(universal_newlines=True))
-        with self.assertRaises(ValueError):
-            self.loop.run_until_complete(connect(bufsize=4096))
-        with self.assertRaises(ValueError):
-            self.loop.run_until_complete(connect(shell=False))
-
-
 if sys.platform == 'win32':
 
     class SelectEventLoopTests(EventLoopTestsMixin, test_utils.TestCase):
         def create_event_loop(self):
             return asyncio.SelectorEventLoop()
 
-    class ProactorEventLoopTests(EventLoopTestsMixin, SubprocessTestsMixin, test_utils.TestCase):
+    class ProactorEventLoopTests(EventLoopTestsMixin, test_utils.TestCase):
         def create_event_loop(self):
             return asyncio.ProactorEventLoop()
 
         def test_legacy_create_ssl_connection(self):
             raise unittest.SkipTest("IocpEventLoop incompatible with legacy SSL")
 
         def test_legacy_create_server_ssl(self):
@@ -2154,16 +1830,15 @@
             else:
                 unpatch()
 
             self.assertEqual(self.loop.run_until_complete(main()), 'hello')
 
     if False and hasattr(selectors, 'KqueueSelector'):
 
-        class KqueueEventLoopTests(UnixEventLoopTestsMixin, SubprocessTestsMixin,
-                                   test_utils.TestCase):
+        class KqueueEventLoopTests(UnixEventLoopTestsMixin, test_utils.TestCase):
             def create_event_loop(self):
                 return asyncio.SelectorEventLoop(selectors.KqueueSelector())
 
             # kqueue doesn't support character devices (PTY) on Mac OS X older
             # than 10.9 (Maverick)
             @support.requires_mac_ver(10, 9)
             # Issue #20667: KqueueEventLoopTests.test_read_pty_output()
@@ -2176,28 +1851,26 @@
             # than 10.9 (Maverick)
             @support.requires_mac_ver(10, 9)
             def test_write_pty(self):
                 super().test_write_pty()
 
     if False and hasattr(selectors, 'EpollSelector'):
 
-        class EPollEventLoopTests(UnixEventLoopTestsMixin, SubprocessTestsMixin,
-                                  test_utils.TestCase):
+        class EPollEventLoopTests(UnixEventLoopTestsMixin, test_utils.TestCase):
             def create_event_loop(self):
                 return asyncio.SelectorEventLoop(selectors.EpollSelector())
 
     if False and hasattr(selectors, 'PollSelector'):
 
-        class PollEventLoopTests(UnixEventLoopTestsMixin, SubprocessTestsMixin,
-                                 test_utils.TestCase):
+        class PollEventLoopTests(UnixEventLoopTestsMixin, test_utils.TestCase):
             def create_event_loop(self):
                 return asyncio.SelectorEventLoop(selectors.PollSelector())
 
     # Should always exist.
-    class TrioEventLoopTests(UnixEventLoopTestsMixin, SubprocessTestsMixin, test_utils.TestCase):
+    class TrioEventLoopTests(UnixEventLoopTestsMixin, test_utils.TestCase):
         def create_event_loop(self):
             import trio_asyncio.sync
             return trio_asyncio.sync.SyncTrioEventLoop()
 
 
 def noop(*args, **kwargs):
     pass
```

### Comparing `trio_asyncio-0.8.4/tests/python/ssl_cert.pem` & `trio_asyncio-0.9.1/tests/python/ssl_cert.pem`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/tests/python/test_selector_events.py` & `trio_asyncio-0.9.1/tests/python/test_selector_events.py`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/tests/python/test_queues.py` & `trio_asyncio-0.9.1/tests/python/test_queues.py`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/tests/python/test_futures.py` & `trio_asyncio-0.9.1/tests/python/test_futures.py`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/tests/python/test_proactor_events.py` & `trio_asyncio-0.9.1/tests/python/test_proactor_events.py`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/tests/python/pycacert.pem` & `trio_asyncio-0.9.1/tests/python/pycacert.pem`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/tests/python/test_windows_events.py` & `trio_asyncio-0.9.1/tests/python/test_windows_events.py`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/tests/python/keycert3.pem` & `trio_asyncio-0.9.1/tests/python/keycert3.pem`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/tests/python/test_locks.py` & `trio_asyncio-0.9.1/tests/python/test_locks.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     r'^<(?P<class>.*?) object at (?P<address>.*?)'
     r'\[(?P<extras>'
     r'(set|unset|locked|unlocked)(, ?value:\d)?(, ?waiters:\d+)?'
     r')\]>\Z'
 )
 RGX_REPR = re.compile(STR_RGX_REPR)
 
+
 class LockTests(test_utils.TestCase):
     def setUp(self):
         super().setUp()
         self.loop = self.new_test_loop()
 
     def test_ctor_loop(self):
         loop = mock.Mock()
```

### Comparing `trio_asyncio-0.8.4/tests/python/ssl_key.pem` & `trio_asyncio-0.9.1/tests/python/ssl_key.pem`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/tests/python/test_pep492.py` & `trio_asyncio-0.9.1/tests/python/test_pep492.py`

 * *Files identical despite different names*

### Comparing `trio_asyncio-0.8.4/PKG-INFO` & `trio_asyncio-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: trio_asyncio
-Version: 0.8.4
+Version: 0.9.1
 Summary: A re-implementation of the asyncio mainloop on top of Trio
 Home-page: https://github.com/python-trio/trio-asyncio
 Author: Matthias Urlichs
 Author-email: matthias@urlichs.de
 License: MIT -or- Apache License 2.0
 Description: ``trio-asyncio`` is a re-implementation of the ``asyncio`` mainloop on top of
         Trio.
@@ -67,8 +67,8 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: System :: Networking
 Classifier: Framework :: Trio
 Classifier: Framework :: AsyncIO
-Requires-Python: >=3.5.3
+Requires-Python: >=3.5.2
```

### Comparing `trio_asyncio-0.8.4/setup.py` & `trio_asyncio-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     url="https://github.com/python-trio/trio-asyncio",
     license="MIT -or- Apache License 2.0",
     packages=find_packages(),
     install_requires=install_requires,
     # This means, just install *everything* you see under trio/, even if it
     # doesn't look like a source file, so long as it appears in MANIFEST.in:
     include_package_data=True,
-    python_requires=">=3.5.3",
+    python_requires=">=3.5.2",  # temporary, for RTD
     keywords=["async", "io", "trio", "asyncio", "trio-asyncio"],
     setup_requires=['pytest-runner'],
     tests_require=['pytest', 'outcome'],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

